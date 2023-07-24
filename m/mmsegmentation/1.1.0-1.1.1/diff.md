# Comparing `tmp/mmsegmentation-1.1.0.tar.gz` & `tmp/mmsegmentation-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmsegmentation-1.1.0.tar", last modified: Tue Jul  4 03:20:55 2023, max compression
+gzip compressed data, was "dist/mmsegmentation-1.1.1.tar", last modified: Mon Jul 24 07:37:29 2023, max compression
```

## Comparing `mmsegmentation-1.1.0.tar` & `mmsegmentation-1.1.1.tar`

### file list

```diff
@@ -1,1197 +1,1198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17883 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/levir_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/vaihingen.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/erfnet_fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_mla.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_pup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_240k.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_320k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ann/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/beit/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb8-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-amp-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/danet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)    44665 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)    49026 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/encnet_r50s-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    36768 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-160k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-80k_cityscapes-832x832.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/knet/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mae/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r101-d32_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/
--rw-r--r--   0 runner    (1001) docker     (123)    24899 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-l_2xb6-120k_1024x1024-cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-m_2xb6-120k_1024x1024-cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_m36_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_m48_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s24_8xb4-40k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s36_8x4_512x512_40k_ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/
--rw-r--r--   0 runner    (1001) docker     (123)    55003 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_isaid-896x896.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_loveda-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_potsdam-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_vaihingen-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d32_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-769x769.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb2-80k_cityscapes512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb4-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb1-160k_cityscapes-1024x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-b_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_fcn_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/metafile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_in1k-pre_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc2_4xb12-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc2_in1k-pre_4xb12-80k_cityscapes-512x1024.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-b_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-l_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-b_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/
--rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet_s5-d16_deeplabv3_4xb4-40k_chase-db1-128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r101_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r18_4xb4-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/metafile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmseg/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/analyze_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/get_flops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/levircd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/synapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/vaihingen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/voc_aug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/pytorch2torchscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dist_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/dist_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/misc/publish_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/beit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/mit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/stdc2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/swin2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/twins2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vit2mmseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vitjax2mmseg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg2torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/test_torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/.mim/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/apis/mmseg_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/basesegdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/coco_stuff.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dark_zurich.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/decathlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/dsdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/isaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/isprs.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/levir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/lip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/loveda.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/mapillary.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/night_driving.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/potsdam.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/refuge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/synapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    79624 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/transforms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/citys_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/evaluation/metrics/iou_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/ddrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/erfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/icnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/mscan.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/pidnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25701 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29843 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/timm_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)    23612 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/twins.py
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/data_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ddr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/dpt_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ham_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/isa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/knet_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/mask2former_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/maskformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/pid_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/segformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/segmenter_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_mla_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_up_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/stdc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/boundary_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/huasdorff_distance_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/ohem_cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/featurepyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/ic_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/jpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/mla_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14659 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/segmentors/seg_tta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/basic_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/ppm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/shape_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/models/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/sampler/ohem_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/structures/seg_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/set_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/utils/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmseg/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/mmseg/visualization/local_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    67418 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 03:20:54.000000 mmsegmentation-1.1.0/mmsegmentation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/albu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7387 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_digit_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_erfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_icnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_pidnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_stdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_swin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_timm_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)    30209 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_backbones/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_dpt_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ham_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_isa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_mask2former_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_maskformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_pidnet_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_segformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_segmenter_mask_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_mla_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_up_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/test_uper_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_heads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_feature2pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_ic_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_jpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_mla_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_necks/test_multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_seg_tta_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_segmentors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 03:20:55.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_models/test_utils/test_shape_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-04 03:20:49.000000 mmsegmentation-1.1.0/tests/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18004 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/bdd100k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/levir_256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/vaihingen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/erfnet_fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_mla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_pup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_240k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_320k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/ann_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ann/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/apcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/beit/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb8-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32-in1k-pre_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-amp-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/ccnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/danet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/danet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44665 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d16-mg124_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49026 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/dmnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dpt/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dsdl/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/dsdl/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/encnet_r50s-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/erfnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/erfnet/erfnet_fcn_4xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/erfnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_psp_4xb4-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastscnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fastscnn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r101b-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50b-d16_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41494 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/gcnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18s_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr48_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36768 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r101-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r101-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r18-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r18-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r50-d8-in1k-pre_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-160k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/icnet_r50-d8_4xb2-80k_cityscapes-832x832.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/isanet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/knet/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mae/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mae/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r101_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-160k_ade20k-640x640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_r101-d32_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_fcn_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/mobilenet-v2-d8_pspnet_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch_lraspp_4xb4-320k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/nonlocal_r50-d8_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    24899 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18s_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/pidnet-l_2xb6-120k_1024x1024-cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/pidnet-m_2xb6-120k_1024x1024-cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_m36_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_m48_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_s24_8xb4-40k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_s36_8x4_512x512_40k_ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/psanet_r50-d8_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    55003 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb2-amp-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r101b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r18b-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d32_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-160k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-320k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_coco-stuff10k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_coco-stuff164k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_isaid-896x896.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_loveda-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_potsdam-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_vaihingen-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50b-d32_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50b-d8_4xb2-80k_cityscapes-769x769.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_deeplabv3plus_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_fcn_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb2-80k_cityscapes512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/resnest_s101-d8_pspnet_4xb4-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b1_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b2_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b3_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b4_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb1-160k_cityscapes-1024x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-b_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-s_fcn_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/fpn_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/fpn_r50_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/metafile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/stdc1_in1k-pre_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/stdc2_4xb12-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/stdc2_in1k-pre_4xb12-80k_cityscapes-512x1024.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-large-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-b_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-l_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-b_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-b_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-l_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_deeplabv3_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_chase-db1-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_drive-64x64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_hrf-256x256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_pspnet_4xb4-ce-1.0-dice-3.0-40k_stare-128x128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet_s5-d16_deeplabv3_4xb4-40k_chase-db1-128x128.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r101_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r18_4xb4-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb2-40k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-512x1024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb2-80k_cityscapes-769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb4-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb4-20k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb4-40k_voc12aug-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/upernet_r50_4xb4-80k_ade20k-512x512.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/metafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-b16_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-s16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-s16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_deit-s16_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-24 07:37:28.000000 mmsegmentation-1.1.1/mmseg/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/analyze_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/get_flops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/levircd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/synapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/vaihingen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/voc_aug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/deployment/pytorch2torchscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dist_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/dist_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/misc/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/misc/print_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/misc/publish_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/beit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/mit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/stdc2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/swin2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/twins2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/vit2mmseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/vitjax2mmseg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/slurm_test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/mmseg2torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/mmseg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/test_torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/.mim/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/apis/mmseg_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/basesegdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/bdd100k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/coco_stuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/dark_zurich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/decathlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/dsdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/isaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/isprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/levir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/lip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/loveda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/mapillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/night_driving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/potsdam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/refuge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/synapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79578 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/transforms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/evaluation/metrics/citys_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/evaluation/metrics/iou_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/bisenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/ddrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/erfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15548 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/icnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/mscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25701 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29843 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/timm_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23612 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/data_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/ddr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/dpt_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/ham_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/isa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/knet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/mask2former_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/maskformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/pid_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/segformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/segmenter_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/setr_mla_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/setr_up_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/stdc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/boundary_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/huasdorff_distance_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/ohem_cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/featurepyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/ic_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/jpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/mla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/segmentors/seg_tta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/basic_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/shape_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/models/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/structures/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/sampler/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/sampler/ohem_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/structures/seg_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24730 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/set_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/utils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmseg/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/mmseg/visualization/local_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    67452 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/mmsegmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/albu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7387 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_digit_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_bisenetv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_bisenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_erfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_icnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_stdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_timm_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30209 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_backbones/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_dpt_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_ham_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_isa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_mask2former_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_maskformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_pidnet_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_segformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_segmenter_mask_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_setr_mla_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_setr_up_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/test_uper_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_heads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_feature2pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_ic_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_jpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_mla_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_necks/test_multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_seg_tta_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_segmentors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:37:29.000000 mmsegmentation-1.1.1/tests/test_models/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_utils/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_models/test_utils/test_shape_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-24 07:37:24.000000 mmsegmentation-1.1.1/tests/test_sampler.py
```

### Comparing `mmsegmentation-1.1.0/PKG-INFO` & `mmsegmentation-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmsegmentation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Open MMLab Semantic Segmentation Toolbox and Benchmark
 Home-page: https://github.com/open-mmlab/mmsegmentation
 Author: MMSegmentation Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmseg-logo.png" width="600"/>
@@ -92,15 +92,15 @@
         
         - **High efficiency**
         
           The training speed is faster than or comparable to other codebases.
         
         ## What's New
         
-        v1.1.0 was released on 07/04/2023.
+        v1.1.1 was released on 07/24/2023.
         Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
         
         - Support 24 medical image datasets in [projects](./projects/medical/).
         - Add GDAL backend and support remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/pull/2903).
         - Support [DDRNet](https://github.com/open-mmlab/mmsegmentation/pull/2855).
         
         ## Installation
@@ -257,14 +257,15 @@
         - [x] [Nighttime Driving](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#nighttime-driving)
         - [x] [LoveDA](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#loveda)
         - [x] [Potsdam](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-potsdam)
         - [x] [Vaihingen](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-vaihingen)
         - [x] [iSAID](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
         - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets)
         - [x] [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#levir-cd)
+        - [x] [BDD100K](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#bdd100K)
         
         </details>
         
         Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
         
         ## Projects
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmsegmentation Version: 1.1.0 Summary: Open MMLab
+Metadata-Version: 2.1 Name: mmsegmentation Version: 1.1.1 Summary: Open MMLab
 Semantic Segmentation Toolbox and Benchmark Home-page: https://github.com/open-
 mmlab/mmsegmentation Author: MMSegmentation Contributors Author-email:
 openmmlab@gmail.com License: Apache License 2.0 Description:
                           [resources/mmseg-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
@@ -48,16 +48,16 @@
 features - **Unified Benchmark** We provide a unified benchmark toolbox for
 various semantic segmentation methods. - **Modular Design** We decompose the
 semantic segmentation framework into different components and one can easily
 construct a customized semantic segmentation framework by combining different
 modules. - **Support of multiple methods out of box** The toolbox directly
 supports popular and contemporary semantic segmentation frameworks, *e.g.*
 PSPNet, DeepLabV3, PSANet, DeepLabV3+, etc. - **High efficiency** The training
-speed is faster than or comparable to other codebases. ## What's New v1.1.0 was
-released on 07/04/2023. Please refer to [changelog.md](docs/en/notes/
+speed is faster than or comparable to other codebases. ## What's New v1.1.1 was
+released on 07/24/2023. Please refer to [changelog.md](docs/en/notes/
 changelog.md) for details and release history. - Support 24 medical image
 datasets in [projects](./projects/medical/). - Add GDAL backend and support
 remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/
 mmsegmentation/pull/2903). - Support [DDRNet](https://github.com/open-mmlab/
 mmsegmentation/pull/2855). ## Installation Please refer to [get_started.md]
 (docs/en/get_started.md#installation) for installation and [dataset_prepare.md]
 (docs/en/user_guides/2_dataset_prepare.md#prepare-datasets) for dataset
@@ -157,62 +157,64 @@
 user_guides/2_dataset_prepare.md#isprs-potsdam) - [x] [Vaihingen](https://
 github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
 2_dataset_prepare.md#isprs-vaihingen) - [x] [iSAID](https://github.com/open-
 mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
 - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/
 main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets) - [x]
 [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/
-user_guides/2_dataset_prepare.md#levir-cd)  Please refer to [FAQ](docs/en/
-notes/faq.md) for frequently asked questions. ## Projects [Here](projects/
-README.md) are some implementations of SOTA models and solutions built on
-MMSegmentation, which are supported and maintained by community users. These
-projects demonstrate the best practices based on MMSegmentation for research
-and product development. We welcome and appreciate all the contributions to
-OpenMMLab ecosystem. ## Contributing We appreciate all contributions to improve
-MMSegmentation. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for
-the contributing guideline. ## Acknowledgement MMSegmentation is an open source
-project that welcome any contribution and feedback. We wish that the toolbox
-and benchmark could serve the growing research community by providing a
-flexible as well as standardized toolkit to reimplement existing methods and
-develop their own new semantic segmentation methods. ## Citation If you find
-this project useful in your research, please consider cite: ```bibtex @misc
-{mmseg2020, title={{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox
-and Benchmark}, author={MMSegmentation Contributors}, howpublished = {\url
-{https://github.com/open-mmlab/mmsegmentation}}, year={2020} } ``` ## License
-This project is released under the [Apache 2.0 license](LICENSE). ## OpenMMLab
-Family - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab
-pre-training toolbox and benchmark. - [MMagic](https://github.com/open-mmlab/
-mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent
-**C**reation toolbox. - [MMDetection](https://github.com/open-mmlab/
-mmdetection): OpenMMLab detection toolbox and benchmark. - [MMYOLO](https://
-github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
-video perception toolbox and benchmark. - [MMSegmentation](https://github.com/
-open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and
-benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
-detection, recognition, and understanding toolbox. - [MMPose](https://
-github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
-parametric model toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMFlow](https://
-github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. -
-[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment
-Framework. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model
-compression toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim):
-MIM installs OpenMMLab packages. - [Playground](https://github.com/open-mmlab/
-playground): A central hub for gathering and showcasing amazing projects built
-upon OpenMMLab. Keywords: computer vision,semantic segmentation Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown Provides-Extra: all Provides-Extra: tests Provides-
-Extra: optional Provides-Extra: mim
+user_guides/2_dataset_prepare.md#levir-cd) - [x] [BDD100K](https://github.com/
+open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
+2_dataset_prepare.md#bdd100K)  Please refer to [FAQ](docs/en/notes/faq.md) for
+frequently asked questions. ## Projects [Here](projects/README.md) are some
+implementations of SOTA models and solutions built on MMSegmentation, which are
+supported and maintained by community users. These projects demonstrate the
+best practices based on MMSegmentation for research and product development. We
+welcome and appreciate all the contributions to OpenMMLab ecosystem. ##
+Contributing We appreciate all contributions to improve MMSegmentation. Please
+refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
+guideline. ## Acknowledgement MMSegmentation is an open source project that
+welcome any contribution and feedback. We wish that the toolbox and benchmark
+could serve the growing research community by providing a flexible as well as
+standardized toolkit to reimplement existing methods and develop their own new
+semantic segmentation methods. ## Citation If you find this project useful in
+your research, please consider cite: ```bibtex @misc{mmseg2020, title={
+{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox and Benchmark},
+author={MMSegmentation Contributors}, howpublished = {\url{https://github.com/
+open-mmlab/mmsegmentation}}, year={2020} } ``` ## License This project is
+released under the [Apache 2.0 license](LICENSE). ## OpenMMLab Family -
+[MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational
+library for training deep learning models. - [MMCV](https://github.com/open-
+mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+benchmark. - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab
+**A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMYOLO](https://github.com/open-mmlab/mmyolo):
+OpenMMLab YOLO series toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
+general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
+mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video
+perception toolbox and benchmark. - [MMSegmentation](https://github.com/open-
+mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark. -
+[MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D]
+(https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMFlow](https://github.com/open-mmlab/
+mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMDeploy](https://
+github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment Framework. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [Playground](https://github.com/open-mmlab/playground): A
+central hub for gathering and showcasing amazing projects built upon OpenMMLab.
+Keywords: computer vision,semantic segmentation Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+Provides-Extra: all Provides-Extra: tests Provides-Extra: optional Provides-
+Extra: mim
```

### Comparing `mmsegmentation-1.1.0/README.md` & `mmsegmentation-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 - **High efficiency**
 
   The training speed is faster than or comparable to other codebases.
 
 ## What's New
 
-v1.1.0 was released on 07/04/2023.
+v1.1.1 was released on 07/24/2023.
 Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
 
 - Support 24 medical image datasets in [projects](./projects/medical/).
 - Add GDAL backend and support remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/pull/2903).
 - Support [DDRNet](https://github.com/open-mmlab/mmsegmentation/pull/2855).
 
 ## Installation
@@ -249,14 +249,15 @@
 - [x] [Nighttime Driving](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#nighttime-driving)
 - [x] [LoveDA](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#loveda)
 - [x] [Potsdam](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-potsdam)
 - [x] [Vaihingen](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-vaihingen)
 - [x] [iSAID](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
 - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets)
 - [x] [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#levir-cd)
+- [x] [BDD100K](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#bdd100K)
 
 </details>
 
 Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
 
 ## Projects
```

#### html2text {}

```diff
@@ -44,16 +44,16 @@
 features - **Unified Benchmark** We provide a unified benchmark toolbox for
 various semantic segmentation methods. - **Modular Design** We decompose the
 semantic segmentation framework into different components and one can easily
 construct a customized semantic segmentation framework by combining different
 modules. - **Support of multiple methods out of box** The toolbox directly
 supports popular and contemporary semantic segmentation frameworks, *e.g.*
 PSPNet, DeepLabV3, PSANet, DeepLabV3+, etc. - **High efficiency** The training
-speed is faster than or comparable to other codebases. ## What's New v1.1.0 was
-released on 07/04/2023. Please refer to [changelog.md](docs/en/notes/
+speed is faster than or comparable to other codebases. ## What's New v1.1.1 was
+released on 07/24/2023. Please refer to [changelog.md](docs/en/notes/
 changelog.md) for details and release history. - Support 24 medical image
 datasets in [projects](./projects/medical/). - Add GDAL backend and support
 remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/
 mmsegmentation/pull/2903). - Support [DDRNet](https://github.com/open-mmlab/
 mmsegmentation/pull/2855). ## Installation Please refer to [get_started.md]
 (docs/en/get_started.md#installation) for installation and [dataset_prepare.md]
 (docs/en/user_guides/2_dataset_prepare.md#prepare-datasets) for dataset
@@ -153,55 +153,56 @@
 user_guides/2_dataset_prepare.md#isprs-potsdam) - [x] [Vaihingen](https://
 github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
 2_dataset_prepare.md#isprs-vaihingen) - [x] [iSAID](https://github.com/open-
 mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
 - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/
 main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets) - [x]
 [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/
-user_guides/2_dataset_prepare.md#levir-cd)  Please refer to [FAQ](docs/en/
-notes/faq.md) for frequently asked questions. ## Projects [Here](projects/
-README.md) are some implementations of SOTA models and solutions built on
-MMSegmentation, which are supported and maintained by community users. These
-projects demonstrate the best practices based on MMSegmentation for research
-and product development. We welcome and appreciate all the contributions to
-OpenMMLab ecosystem. ## Contributing We appreciate all contributions to improve
-MMSegmentation. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for
-the contributing guideline. ## Acknowledgement MMSegmentation is an open source
-project that welcome any contribution and feedback. We wish that the toolbox
-and benchmark could serve the growing research community by providing a
-flexible as well as standardized toolkit to reimplement existing methods and
-develop their own new semantic segmentation methods. ## Citation If you find
-this project useful in your research, please consider cite: ```bibtex @misc
-{mmseg2020, title={{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox
-and Benchmark}, author={MMSegmentation Contributors}, howpublished = {\url
-{https://github.com/open-mmlab/mmsegmentation}}, year={2020} } ``` ## License
-This project is released under the [Apache 2.0 license](LICENSE). ## OpenMMLab
-Family - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab
-pre-training toolbox and benchmark. - [MMagic](https://github.com/open-mmlab/
-mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent
-**C**reation toolbox. - [MMDetection](https://github.com/open-mmlab/
-mmdetection): OpenMMLab detection toolbox and benchmark. - [MMYOLO](https://
-github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
-video perception toolbox and benchmark. - [MMSegmentation](https://github.com/
-open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and
-benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
-detection, recognition, and understanding toolbox. - [MMPose](https://
-github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
-parametric model toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMFlow](https://
-github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. -
-[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment
-Framework. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model
-compression toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim):
-MIM installs OpenMMLab packages. - [Playground](https://github.com/open-mmlab/
-playground): A central hub for gathering and showcasing amazing projects built
-upon OpenMMLab.
+user_guides/2_dataset_prepare.md#levir-cd) - [x] [BDD100K](https://github.com/
+open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
+2_dataset_prepare.md#bdd100K)  Please refer to [FAQ](docs/en/notes/faq.md) for
+frequently asked questions. ## Projects [Here](projects/README.md) are some
+implementations of SOTA models and solutions built on MMSegmentation, which are
+supported and maintained by community users. These projects demonstrate the
+best practices based on MMSegmentation for research and product development. We
+welcome and appreciate all the contributions to OpenMMLab ecosystem. ##
+Contributing We appreciate all contributions to improve MMSegmentation. Please
+refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
+guideline. ## Acknowledgement MMSegmentation is an open source project that
+welcome any contribution and feedback. We wish that the toolbox and benchmark
+could serve the growing research community by providing a flexible as well as
+standardized toolkit to reimplement existing methods and develop their own new
+semantic segmentation methods. ## Citation If you find this project useful in
+your research, please consider cite: ```bibtex @misc{mmseg2020, title={
+{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox and Benchmark},
+author={MMSegmentation Contributors}, howpublished = {\url{https://github.com/
+open-mmlab/mmsegmentation}}, year={2020} } ``` ## License This project is
+released under the [Apache 2.0 license](LICENSE). ## OpenMMLab Family -
+[MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational
+library for training deep learning models. - [MMCV](https://github.com/open-
+mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+benchmark. - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab
+**A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMYOLO](https://github.com/open-mmlab/mmyolo):
+OpenMMLab YOLO series toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
+general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
+mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video
+perception toolbox and benchmark. - [MMSegmentation](https://github.com/open-
+mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark. -
+[MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D]
+(https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMFlow](https://github.com/open-mmlab/
+mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMDeploy](https://
+github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment Framework. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [Playground](https://github.com/open-mmlab/playground): A
+central hub for gathering and showcasing amazing projects built upon OpenMMLab.
```

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/chase_db1.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/coco-stuff164k.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     num_workers=4,
     persistent_workers=True,
     sampler=dict(type='InfiniteSampler', shuffle=True),
     dataset=dict(
         type=dataset_type,
         data_root=data_root,
         data_prefix=dict(
-            img_path='images/train2017', seg_map_path='annotations/val2017'),
+            img_path='images/train2017', seg_map_path='annotations/train2017'),
         pipeline=train_pipeline))
 val_dataloader = dict(
     batch_size=1,
     num_workers=4,
     persistent_workers=True,
     sampler=dict(type='DefaultSampler', shuffle=False),
     dataset=dict(
```

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/drive.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/hrf.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/isaid.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/isaid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/levir_256x256.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/levir_256x256.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/loveda.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v1_65.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/mapillary_v2.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/mapillary_v2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/pascal_voc12_aug.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/potsdam.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/refuge.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/stare.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/synapse.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/datasets/vaihingen.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/datasets/vaihingen.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ann_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/bisenetv1_r18-d32.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/bisenetv2.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/cgnet.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/danet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/dpt_vit-b16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/erfnet_fcn.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/erfnet_fcn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fast_scnn.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fastfcn_r50-d32_jpu_psp.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_hr18.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fpn_poolformer_s12.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/fpn_r50.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/icnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/isanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pointrend_r50.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/segformer_mit-b0.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/segmenter_vit-b16_mask.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_mla.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_mla.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_naive.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_naive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/setr_pup.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/setr_pup.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/stdc.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/twins_pcpvt-s_upernet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_beit.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_convnext.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_convnext.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_mae.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_r50.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_swin.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_swin.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/models/upernet_vit-b16_ln_mln.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_160k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_160k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_20k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_20k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_240k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_240k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_320k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_320k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_40k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_40k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/_base_/schedules/schedule_80k.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/_base_/schedules/schedule_80k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ann/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ann/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/apcnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/apcnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-base_upernet_8xb2-160k_ade20k-640x640_ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/beit/beit-large_upernet_8xb1-amp-160k_ade20k-640x640_ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/beit/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/beit/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r101-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32-in1k-pre_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r18-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/bisenetv1_r50-d32_4xb4-160k_coco-stuff164k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv1/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv1/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb4-ohem-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/bisenetv2_fcn_4xb8-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/bisenetv2/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/bisenetv2/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ccnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ccnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb4-60k_cityscapes-680x680.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/cgnet_fcn_4xb8-60k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/cgnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/cgnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-base_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-large_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-small_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-tiny_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/convnext-xlarge_upernet_8xb2-amp-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/convnext/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/convnext/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/danet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/danet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/ddrnet_23-slim_in1k-pre_2xb6-120k_cityscapes-1024x1024.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # The class_weight is borrowed from https://github.com/openseg-group/OCNet.pytorch/issues/14 # noqa
 # Licensed under the MIT License
 class_weight = [
     0.8373, 0.918, 0.866, 1.0345, 1.0166, 0.9969, 0.9754, 1.0489, 0.8786,
     1.0023, 0.9539, 0.9843, 1.1116, 0.9037, 1.0865, 1.0955, 1.0865, 1.1529,
     1.0507
 ]
-
+checkpoint = 'https://download.openmmlab.com/mmsegmentation/v0.5/ddrnet/pretrain/ddrnet23s-in1kpre_3rdparty-1ccac5b1.pth'  # noqa
 crop_size = (1024, 1024)
 data_preprocessor = dict(
     type='SegDataPreProcessor',
     size=crop_size,
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     bgr_to_rgb=True,
@@ -27,17 +27,15 @@
     backbone=dict(
         type='DDRNet',
         in_channels=3,
         channels=32,
         ppm_channels=128,
         norm_cfg=norm_cfg,
         align_corners=False,
-        init_cfg=dict(
-            type='Pretrained',
-            checkpoint='pretrained/ddrnet23s_in1k_mmseg.pth')),
+        init_cfg=dict(type='Pretrained', checkpoint=checkpoint)),
     decode_head=dict(
         type='DDRHead',
         in_channels=32 * 4,
         channels=64,
         dropout_ratio=0.,
         num_classes=19,
         align_corners=False,
```

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ddrnet/ddrnet_23_in1k-pre_2xb6-120k_cityscapes-1024x1024.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # The class_weight is borrowed from https://github.com/openseg-group/OCNet.pytorch/issues/14 # noqa
 # Licensed under the MIT License
 class_weight = [
     0.8373, 0.918, 0.866, 1.0345, 1.0166, 0.9969, 0.9754, 1.0489, 0.8786,
     1.0023, 0.9539, 0.9843, 1.1116, 0.9037, 1.0865, 1.0955, 1.0865, 1.1529,
     1.0507
 ]
-
+checkpoint = 'https://download.openmmlab.com/mmsegmentation/v0.5/ddrnet/pretrain/ddrnet23-in1kpre_3rdparty-9ca29f62.pth'  # noqa
 crop_size = (1024, 1024)
 data_preprocessor = dict(
     type='SegDataPreProcessor',
     size=crop_size,
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     bgr_to_rgb=True,
@@ -27,17 +27,15 @@
     backbone=dict(
         type='DDRNet',
         in_channels=3,
         channels=64,
         ppm_channels=128,
         norm_cfg=norm_cfg,
         align_corners=False,
-        init_cfg=dict(
-            type='Pretrained',
-            checkpoint='pretrained/ddrnet23_in1k_mmseg.pth')),
+        init_cfg=dict(type='Pretrained', checkpoint=checkpoint)),
     decode_head=dict(
         type='DDRHead',
         in_channels=64 * 4,
         channels=128,
         dropout_ratio=0.,
         num_classes=19,
         align_corners=False,
```

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/deeplabv3_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb2-300k_mapillay_v1_65-1280x1280.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/deeplabv3plus_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/deeplabv3plus/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/deeplabv3plus/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dmnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dmnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dnlnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dnlnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dpt/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dpt/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/cityscapes.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dsdl/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/dsdl/voc.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/dsdl/voc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/emanet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/emanet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/encnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/encnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/erfnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/erfnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_aspp_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/fastfcn_r50-d32_jpu_enc_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastfcn/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastfcn/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastscnn/fast_scnn_8xb4-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fastscnn/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fastscnn/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-40k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn-d6_r50-d16_4xb2-80k_cityscapes-769x769.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/fcn_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/fcn/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/fcn/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/gcnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/gcnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/fcn_hr18_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/hrnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/hrnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/icnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/icnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/isanet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/isanet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_deeplabv3_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_fcn_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_pspnet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_r50-d8_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-l_upernet_8xb2-adamw-80k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/knet-s3_swin-t_upernet_8xb2-adamw-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/knet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/knet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512-ms.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mae/mae-base_upernet_8xb2-amp-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mae/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mae/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_r50_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-b-in1k-384x384-pre_8xb2-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-b-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-l-in22k-384x384-pre_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-s_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/mask2former_swin-t_8xb2-90k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mask2former/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mask2former/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_r50-d32_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_swin-s_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/maskformer_swin-t_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/maskformer/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/maskformer/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v2/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v2/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-s_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8-scratch-s_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/mobilenet_v3/mobilenet-v3-d8_lraspp_4xb4-320k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/nonlocal_net/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/nonlocal_net/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-20k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-40k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr18_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-40k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-20k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-40k_voc12aug-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_hr48_4xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-40k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/ocrnet/ocrnet_r101-d8_8xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pidnet/pidnet-s_2xb6-120k_1024x1024-cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r50_4xb2-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/point_rend/pointrend_r50_4xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/fpn_poolformer_s12_8xb4-40k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/poolformer/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/poolformer/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/psanet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/psanet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d32_rsb_4xb2-adamw-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8-rsb_4xb2-adamw-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_dark-zurich-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-40k_cityscapes-512x1024_night-driving-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_dark-zurich-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024_night-driving-1920x1080.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-40k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/pspnet/pspnet_r50-d8_4xb4-80k_pascal-context-59-480x480.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/resnest/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/resnest/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb1-160k_cityscapes-1024x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b0_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segformer/segformer_mit-b5_8xb2-160k_ade20k-640x640.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-l_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-s_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segmenter/segmenter_vit-t_mask_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-b_1xb16-adamw-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-l_1xb16-adamw-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-s_1xb16-adamw-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/segnext/segnext_mscan-t_1xb16-adamw-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/sem_fpn/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/sem_fpn/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l-mla_8xb1-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_mla_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_naive_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb1-80k_cityscapes-768x768.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/setr/setr_vit-l_pup_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/stdc/stdc1_4xb12-80k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-base-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-large-patch4-window7-in22k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/swin/swin-tiny-patch4-window7_upernet_1xb8-20k_levir-256x256.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/twins/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_pcpvt-s_uperhead_8xb4-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-l_uperhead_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-s_fpn_fpnhead_8xb4-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/twins/twins_svt-s_uperhead_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/unet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/unet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/unet/unet-s5-d16_fcn_4xb4-160k_cityscapes-512x1024.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/upernet/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/upernet/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/metafile.yaml` & `mmsegmentation-1.1.1/mmseg/.mim/configs/vit/metafile.yaml`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16-ln_mln_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py` & `mmsegmentation-1.1.1/mmseg/.mim/configs/vit/vit_vit-b16_mln_upernet_8xb2-80k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/model-index.yml` & `mmsegmentation-1.1.1/mmseg/.mim/model-index.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 - configs/danet/metafile.yaml
 - configs/ddrnet/metafile.yaml
 - configs/deeplabv3/metafile.yaml
 - configs/deeplabv3plus/metafile.yaml
 - configs/dmnet/metafile.yaml
 - configs/dnlnet/metafile.yaml
 - configs/dpt/metafile.yaml
-- configs/dsdl/metafile.yaml
 - configs/emanet/metafile.yaml
 - configs/encnet/metafile.yaml
 - configs/erfnet/metafile.yaml
 - configs/fastfcn/metafile.yaml
 - configs/fastscnn/metafile.yaml
 - configs/fcn/metafile.yaml
 - configs/gcnet/metafile.yaml
```

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/analyze_logs.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/benchmark.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/browse_dataset.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/confusion_matrix.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/analysis_tools/get_flops.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/chase_db1.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/chase_db1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/cityscapes.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/coco_stuff10k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/coco_stuff164k.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/drive.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/drive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/hrf.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/hrf.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/isaid.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/isaid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/levircd.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/levircd.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/loveda.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/pascal_context.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/potsdam.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/refuge.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/stare.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/stare.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/synapse.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/vaihingen.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/vaihingen.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/dataset_converters/voc_aug.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/dataset_converters/voc_aug.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/deployment/pytorch2torchscript.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/deployment/pytorch2torchscript.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/misc/browse_dataset.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/misc/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/misc/print_config.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/beit2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/beit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/mit2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/mit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/stdc2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/stdc2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/swin2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/swin2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/twins2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/twins2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vit2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/vit2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/model_converters/vitjax2mmseg.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/model_converters/vitjax2mmseg.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_test.sh` & `mmsegmentation-1.1.1/mmseg/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/slurm_train.sh` & `mmsegmentation-1.1.1/mmseg/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/test.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/test.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg2torchserve.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/mmseg2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/mmseg_handler.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/mmseg_handler.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/torchserve/test_torchserve.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/torchserve/test_torchserve.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/.mim/tools/train.py` & `mmsegmentation-1.1.1/mmseg/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/__init__.py` & `mmsegmentation-1.1.1/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/apis/inference.py` & `mmsegmentation-1.1.1/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/apis/mmseg_inferencer.py` & `mmsegmentation-1.1.1/mmseg/apis/mmseg_inferencer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/__init__.py` & `mmsegmentation-1.1.1/mmseg/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 # yapf: disable
 from .ade import ADE20KDataset
 from .basesegdataset import BaseCDDataset, BaseSegDataset
+from .bdd100k import BDD100KDataset
 from .chase_db1 import ChaseDB1Dataset
 from .cityscapes import CityscapesDataset
 from .coco_stuff import COCOStuffDataset
 from .dark_zurich import DarkZurichDataset
 from .dataset_wrappers import MultiImageMixDataset
 from .decathlon import DecathlonDataset
 from .drive import DRIVEDataset
@@ -53,9 +54,9 @@
     'LoadBiomedicalAnnotation', 'LoadBiomedicalData', 'GenerateEdge',
     'DecathlonDataset', 'LIPDataset', 'ResizeShortestEdge',
     'BioMedicalGaussianNoise', 'BioMedicalGaussianBlur',
     'BioMedicalRandomGamma', 'BioMedical3DPad', 'RandomRotFlip',
     'SynapseDataset', 'REFUGEDataset', 'MapillaryDataset_v1',
     'MapillaryDataset_v2', 'Albu', 'LEVIRCDDataset',
     'LoadMultipleRSImageFromFile', 'LoadSingleRSImageFromFile',
-    'ConcatCDInput', 'BaseCDDataset', 'DSDLSegDataset'
+    'ConcatCDInput', 'BaseCDDataset', 'DSDLSegDataset', 'BDD100KDataset'
 ]
```

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/ade.py` & `mmsegmentation-1.1.1/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/basesegdataset.py` & `mmsegmentation-1.1.1/mmseg/datasets/basesegdataset.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/chase_db1.py` & `mmsegmentation-1.1.1/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/cityscapes.py` & `mmsegmentation-1.1.1/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/coco_stuff.py` & `mmsegmentation-1.1.1/mmseg/datasets/coco_stuff.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/dataset_wrappers.py` & `mmsegmentation-1.1.1/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/decathlon.py` & `mmsegmentation-1.1.1/mmseg/datasets/decathlon.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/drive.py` & `mmsegmentation-1.1.1/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/dsdl.py` & `mmsegmentation-1.1.1/mmseg/datasets/dsdl.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/hrf.py` & `mmsegmentation-1.1.1/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/isaid.py` & `mmsegmentation-1.1.1/mmseg/datasets/isaid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/isprs.py` & `mmsegmentation-1.1.1/mmseg/datasets/isprs.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/levir.py` & `mmsegmentation-1.1.1/mmseg/datasets/levir.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/lip.py` & `mmsegmentation-1.1.1/mmseg/datasets/lip.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/loveda.py` & `mmsegmentation-1.1.1/mmseg/datasets/loveda.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/mapillary.py` & `mmsegmentation-1.1.1/mmseg/datasets/mapillary.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/night_driving.py` & `mmsegmentation-1.1.1/mmseg/datasets/night_driving.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/pascal_context.py` & `mmsegmentation-1.1.1/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/potsdam.py` & `mmsegmentation-1.1.1/mmseg/datasets/potsdam.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/refuge.py` & `mmsegmentation-1.1.1/mmseg/datasets/refuge.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/stare.py` & `mmsegmentation-1.1.1/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/synapse.py` & `mmsegmentation-1.1.1/mmseg/datasets/synapse.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/transforms/__init__.py` & `mmsegmentation-1.1.1/mmseg/datasets/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/transforms/formatting.py` & `mmsegmentation-1.1.1/mmseg/datasets/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/transforms/loading.py` & `mmsegmentation-1.1.1/mmseg/datasets/transforms/loading.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/transforms/transforms.py` & `mmsegmentation-1.1.1/mmseg/datasets/transforms/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -2202,18 +2202,15 @@
         self.transforms = transforms
         self.keymap = keymap
         self.update_pad_shape = update_pad_shape
 
         self.aug = Compose([self.albu_builder(t) for t in self.transforms])
 
         if not keymap:
-            self.keymap_to_albu = {
-                'img': 'image',
-                'gt_masks': 'masks',
-            }
+            self.keymap_to_albu = {'img': 'image', 'gt_seg_map': 'mask'}
         else:
             self.keymap_to_albu = copy.deepcopy(keymap)
         self.keymap_back = {v: k for k, v in self.keymap_to_albu.items()}
 
     def albu_builder(self, cfg: dict) -> object:
         """Build a callable object from a dict containing albu arguments.
```

### Comparing `mmsegmentation-1.1.0/mmseg/datasets/voc.py` & `mmsegmentation-1.1.1/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/engine/hooks/visualization_hook.py` & `mmsegmentation-1.1.1/mmseg/engine/hooks/visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py` & `mmsegmentation-1.1.1/mmseg/engine/optimizers/layer_decay_optimizer_constructor.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/evaluation/metrics/citys_metric.py` & `mmsegmentation-1.1.1/mmseg/evaluation/metrics/citys_metric.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/evaluation/metrics/iou_metric.py` & `mmsegmentation-1.1.1/mmseg/evaluation/metrics/iou_metric.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/__init__.py` & `mmsegmentation-1.1.1/mmseg/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/__init__.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/beit.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv1.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/bisenetv1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/bisenetv2.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/cgnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/ddrnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/ddrnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/erfnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/erfnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/fast_scnn.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/hrnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/icnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/icnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/mae.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/mit.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/mit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v2.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/mobilenet_v3.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/mscan.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/mscan.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/pidnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/pidnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/resnest.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/resnet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/resnext.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/stdc.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/swin.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/swin.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/timm_backbone.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/timm_backbone.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/twins.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/twins.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/unet.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/backbones/vit.py` & `mmsegmentation-1.1.1/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/builder.py` & `mmsegmentation-1.1.1/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/data_preprocessor.py` & `mmsegmentation-1.1.1/mmseg/models/data_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,17 @@
                 pad_val=self.pad_val,
                 seg_pad_val=self.seg_pad_val)
 
             if self.batch_augments is not None:
                 inputs, data_samples = self.batch_augments(
                     inputs, data_samples)
         else:
-            assert len(inputs) == 1, (
-                'Batch inference is not support currently, '
-                'as the image size might be different in a batch')
+            img_size = inputs[0].shape[1:]
+            assert all(input_.shape[1:] == img_size for input_ in inputs),  \
+                'The image size in a batch should be the same.'
             # pad images when testing
             if self.test_cfg:
                 inputs, padded_samples = stack_batch(
                     inputs=inputs,
                     size=self.test_cfg.get('size', None),
                     size_divisor=self.test_cfg.get('size_divisor', None),
                     pad_val=self.pad_val,
```

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/__init__.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/ann_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/apc_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/aspp_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/cascade_decode_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/cc_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/da_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/ddr_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/ddr_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/decode_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/dm_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/dnl_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/dpt_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/dpt_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/ema_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/enc_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/fcn_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/fpn_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/gc_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/ham_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/ham_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/isa_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/isa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/knet_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/knet_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/lraspp_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/mask2former_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/mask2former_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/maskformer_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/maskformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/nl_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/ocr_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/pid_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/pid_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/point_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/psa_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/psp_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/segformer_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/segformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/segmenter_mask_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/segmenter_mask_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_aspp_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/sep_fcn_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_mla_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/setr_mla_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/setr_up_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/setr_up_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/stdc_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/stdc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/decode_heads/uper_head.py` & `mmsegmentation-1.1.1/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/__init__.py` & `mmsegmentation-1.1.1/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/accuracy.py` & `mmsegmentation-1.1.1/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/boundary_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/boundary_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/cross_entropy_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/dice_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/focal_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/huasdorff_distance_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/huasdorff_distance_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/lovasz_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/ohem_cross_entropy_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/ohem_cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/tversky_loss.py` & `mmsegmentation-1.1.1/mmseg/models/losses/tversky_loss.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/losses/utils.py` & `mmsegmentation-1.1.1/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/featurepyramid.py` & `mmsegmentation-1.1.1/mmseg/models/necks/featurepyramid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/fpn.py` & `mmsegmentation-1.1.1/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/ic_neck.py` & `mmsegmentation-1.1.1/mmseg/models/necks/ic_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/jpu.py` & `mmsegmentation-1.1.1/mmseg/models/necks/jpu.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/mla_neck.py` & `mmsegmentation-1.1.1/mmseg/models/necks/mla_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/necks/multilevel_neck.py` & `mmsegmentation-1.1.1/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/segmentors/base.py` & `mmsegmentation-1.1.1/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/segmentors/cascade_encoder_decoder.py` & `mmsegmentation-1.1.1/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/segmentors/encoder_decoder.py` & `mmsegmentation-1.1.1/mmseg/models/segmentors/encoder_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+import logging
 from typing import List, Optional
 
 import torch.nn as nn
 import torch.nn.functional as F
+from mmengine.logging import print_log
 from torch import Tensor
 
 from mmseg.registry import MODELS
 from mmseg.utils import (ConfigType, OptConfigType, OptMultiConfig,
                          OptSampleList, SampleList, add_prefix)
 from .base import BaseSegmentor
 
@@ -326,15 +328,19 @@
             Tensor: The segmentation results, seg_logits from model of each
                 input image.
         """
         assert self.test_cfg.get('mode', 'whole') in ['slide', 'whole'], \
             f'Only "slide" or "whole" test mode are supported, but got ' \
             f'{self.test_cfg["mode"]}.'
         ori_shape = batch_img_metas[0]['ori_shape']
-        assert all(_['ori_shape'] == ori_shape for _ in batch_img_metas)
+        if not all(_['ori_shape'] == ori_shape for _ in batch_img_metas):
+            print_log(
+                'Image shapes are different in the batch.',
+                logger='current',
+                level=logging.WARN)
         if self.test_cfg.mode == 'slide':
             seg_logit = self.slide_inference(inputs, batch_img_metas)
         else:
             seg_logit = self.whole_inference(inputs, batch_img_metas)
 
         return seg_logit
```

### Comparing `mmsegmentation-1.1.0/mmseg/models/segmentors/seg_tta.py` & `mmsegmentation-1.1.1/mmseg/models/segmentors/seg_tta.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import List
 
 import torch
 from mmengine.model import BaseTTAModel
 from mmengine.structures import PixelData
 
 from mmseg.registry import MODELS
-from mmseg.structures import SegDataSample
 from mmseg.utils import SampleList
 
 
 @MODELS.register_module()
 class SegTTAModel(BaseTTAModel):
 
     def merge_preds(self, data_samples_list: List[SampleList]) -> SampleList:
@@ -35,15 +34,14 @@
                     logits += seg_logit.sigmoid()
             logits /= len(data_samples)
             if self.module.out_channels == 1:
                 seg_pred = (logits > self.module.decode_head.threshold
                             ).to(logits).squeeze(1)
             else:
                 seg_pred = logits.argmax(dim=0)
-            data_sample = SegDataSample(
-                **{
-                    'pred_sem_seg': PixelData(data=seg_pred),
-                    'gt_sem_seg': data_samples[0].gt_sem_seg
-                })
+            data_sample.set_data({'pred_sem_seg': PixelData(data=seg_pred)})
+            if hasattr(data_samples[0], 'gt_sem_seg'):
+                data_sample.set_data(
+                    {'gt_sem_seg': data_samples[0].gt_sem_seg})
             data_sample.set_metainfo({'img_path': data_samples[0].img_path})
             predictions.append(data_sample)
         return predictions
```

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/__init__.py` & `mmsegmentation-1.1.1/mmseg/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/basic_block.py` & `mmsegmentation-1.1.1/mmseg/models/utils/basic_block.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/embed.py` & `mmsegmentation-1.1.1/mmseg/models/utils/embed.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/encoding.py` & `mmsegmentation-1.1.1/mmseg/models/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/inverted_residual.py` & `mmsegmentation-1.1.1/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/make_divisible.py` & `mmsegmentation-1.1.1/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/ppm.py` & `mmsegmentation-1.1.1/mmseg/models/utils/ppm.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/res_layer.py` & `mmsegmentation-1.1.1/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/se_layer.py` & `mmsegmentation-1.1.1/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/self_attention_block.py` & `mmsegmentation-1.1.1/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/shape_convert.py` & `mmsegmentation-1.1.1/mmseg/models/utils/shape_convert.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/up_conv_block.py` & `mmsegmentation-1.1.1/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/models/utils/wrappers.py` & `mmsegmentation-1.1.1/mmseg/models/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/registry/__init__.py` & `mmsegmentation-1.1.1/mmseg/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/registry/registry.py` & `mmsegmentation-1.1.1/mmseg/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/structures/sampler/ohem_pixel_sampler.py` & `mmsegmentation-1.1.1/mmseg/structures/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/structures/seg_data_sample.py` & `mmsegmentation-1.1.1/mmseg/structures/seg_data_sample.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/utils/__init__.py` & `mmsegmentation-1.1.1/mmseg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/utils/class_names.py` & `mmsegmentation-1.1.1/mmseg/utils/class_names.py`

 * *Files 7% similar despite different names*

```diff
@@ -415,14 +415,34 @@
         'Background', 'Hat', 'Hair', 'Glove', 'Sunglasses', 'UpperClothes',
         'Dress', 'Coat', 'Socks', 'Pants', 'Jumpsuits', 'Scarf', 'Skirt',
         'Face', 'Left-arm', 'Right-arm', 'Left-leg', 'Right-leg', 'Left-shoe',
         'Right-shoe'
     ]
 
 
+def bdd100k_classes():
+    """BDD100K class names for external use(the class name is compatible with
+    Cityscapes )."""
+    return [
+        'road', 'sidewalk', 'building', 'wall', 'fence', 'pole',
+        'traffic light', 'traffic sign', 'vegetation', 'terrain', 'sky',
+        'person', 'rider', 'car', 'truck', 'bus', 'train', 'motorcycle',
+        'bicycle'
+    ]
+
+
+def bdd100k_palette():
+    """bdd100k palette for external use(same with cityscapes)"""
+    return [[128, 64, 128], [244, 35, 232], [70, 70, 70], [102, 102, 156],
+            [190, 153, 153], [153, 153, 153], [250, 170, 30], [220, 220, 0],
+            [107, 142, 35], [152, 251, 152], [70, 130, 180], [220, 20, 60],
+            [255, 0, 0], [0, 0, 142], [0, 0, 70], [0, 60, 100], [0, 80, 100],
+            [0, 0, 230], [119, 11, 32]]
+
+
 dataset_aliases = {
     'cityscapes': ['cityscapes'],
     'ade': ['ade', 'ade20k'],
     'voc': ['voc', 'pascal_voc', 'voc12', 'voc12aug'],
     'loveda': ['loveda'],
     'potsdam': ['potsdam'],
     'vaihingen': ['vaihingen'],
@@ -431,15 +451,16 @@
         'coco-stuff10k', 'coco-stuff164k', 'coco_stuff', 'coco_stuff10k',
         'coco_stuff164k'
     ],
     'isaid': ['isaid', 'iSAID'],
     'stare': ['stare', 'STARE'],
     'lip': ['LIP', 'lip'],
     'mapillary_v1': ['mapillary_v1'],
-    'mapillary_v2': ['mapillary_v2']
+    'mapillary_v2': ['mapillary_v2'],
+    'bdd100k': ['bdd100k']
 }
 
 
 def get_classes(dataset):
     """Get class names of a dataset."""
     alias2name = {}
     for name, aliases in dataset_aliases.items():
```

### Comparing `mmsegmentation-1.1.0/mmseg/utils/io.py` & `mmsegmentation-1.1.1/mmseg/utils/io.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/utils/misc.py` & `mmsegmentation-1.1.1/mmseg/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/utils/set_env.py` & `mmsegmentation-1.1.1/mmseg/utils/set_env.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/utils/typing_utils.py` & `mmsegmentation-1.1.1/mmseg/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmseg/visualization/local_visualizer.py` & `mmsegmentation-1.1.1/mmseg/visualization/local_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/mmsegmentation.egg-info/PKG-INFO` & `mmsegmentation-1.1.1/mmsegmentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmsegmentation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Open MMLab Semantic Segmentation Toolbox and Benchmark
 Home-page: https://github.com/open-mmlab/mmsegmentation
 Author: MMSegmentation Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="resources/mmseg-logo.png" width="600"/>
@@ -92,15 +92,15 @@
         
         - **High efficiency**
         
           The training speed is faster than or comparable to other codebases.
         
         ## What's New
         
-        v1.1.0 was released on 07/04/2023.
+        v1.1.1 was released on 07/24/2023.
         Please refer to [changelog.md](docs/en/notes/changelog.md) for details and release history.
         
         - Support 24 medical image datasets in [projects](./projects/medical/).
         - Add GDAL backend and support remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/pull/2903).
         - Support [DDRNet](https://github.com/open-mmlab/mmsegmentation/pull/2855).
         
         ## Installation
@@ -257,14 +257,15 @@
         - [x] [Nighttime Driving](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#nighttime-driving)
         - [x] [LoveDA](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#loveda)
         - [x] [Potsdam](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-potsdam)
         - [x] [Vaihingen](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isprs-vaihingen)
         - [x] [iSAID](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
         - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets)
         - [x] [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#levir-cd)
+        - [x] [BDD100K](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#bdd100K)
         
         </details>
         
         Please refer to [FAQ](docs/en/notes/faq.md) for frequently asked questions.
         
         ## Projects
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmsegmentation Version: 1.1.0 Summary: Open MMLab
+Metadata-Version: 2.1 Name: mmsegmentation Version: 1.1.1 Summary: Open MMLab
 Semantic Segmentation Toolbox and Benchmark Home-page: https://github.com/open-
 mmlab/mmsegmentation Author: MMSegmentation Contributors Author-email:
 openmmlab@gmail.com License: Apache License 2.0 Description:
                           [resources/mmseg-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
@@ -48,16 +48,16 @@
 features - **Unified Benchmark** We provide a unified benchmark toolbox for
 various semantic segmentation methods. - **Modular Design** We decompose the
 semantic segmentation framework into different components and one can easily
 construct a customized semantic segmentation framework by combining different
 modules. - **Support of multiple methods out of box** The toolbox directly
 supports popular and contemporary semantic segmentation frameworks, *e.g.*
 PSPNet, DeepLabV3, PSANet, DeepLabV3+, etc. - **High efficiency** The training
-speed is faster than or comparable to other codebases. ## What's New v1.1.0 was
-released on 07/04/2023. Please refer to [changelog.md](docs/en/notes/
+speed is faster than or comparable to other codebases. ## What's New v1.1.1 was
+released on 07/24/2023. Please refer to [changelog.md](docs/en/notes/
 changelog.md) for details and release history. - Support 24 medical image
 datasets in [projects](./projects/medical/). - Add GDAL backend and support
 remote sensing datasets [LEVIR-CD](https://github.com/open-mmlab/
 mmsegmentation/pull/2903). - Support [DDRNet](https://github.com/open-mmlab/
 mmsegmentation/pull/2855). ## Installation Please refer to [get_started.md]
 (docs/en/get_started.md#installation) for installation and [dataset_prepare.md]
 (docs/en/user_guides/2_dataset_prepare.md#prepare-datasets) for dataset
@@ -157,62 +157,64 @@
 user_guides/2_dataset_prepare.md#isprs-potsdam) - [x] [Vaihingen](https://
 github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
 2_dataset_prepare.md#isprs-vaihingen) - [x] [iSAID](https://github.com/open-
 mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#isaid)
 - [x] [Mapillary Vistas](https://github.com/open-mmlab/mmsegmentation/blob/
 main/docs/en/user_guides/2_dataset_prepare.md#mapillary-vistas-datasets) - [x]
 [LEVIR-CD](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/
-user_guides/2_dataset_prepare.md#levir-cd)  Please refer to [FAQ](docs/en/
-notes/faq.md) for frequently asked questions. ## Projects [Here](projects/
-README.md) are some implementations of SOTA models and solutions built on
-MMSegmentation, which are supported and maintained by community users. These
-projects demonstrate the best practices based on MMSegmentation for research
-and product development. We welcome and appreciate all the contributions to
-OpenMMLab ecosystem. ## Contributing We appreciate all contributions to improve
-MMSegmentation. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for
-the contributing guideline. ## Acknowledgement MMSegmentation is an open source
-project that welcome any contribution and feedback. We wish that the toolbox
-and benchmark could serve the growing research community by providing a
-flexible as well as standardized toolkit to reimplement existing methods and
-develop their own new semantic segmentation methods. ## Citation If you find
-this project useful in your research, please consider cite: ```bibtex @misc
-{mmseg2020, title={{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox
-and Benchmark}, author={MMSegmentation Contributors}, howpublished = {\url
-{https://github.com/open-mmlab/mmsegmentation}}, year={2020} } ``` ## License
-This project is released under the [Apache 2.0 license](LICENSE). ## OpenMMLab
-Family - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab
-foundational library for training deep learning models. - [MMCV](https://
-github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer
-vision. - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab
-pre-training toolbox and benchmark. - [MMagic](https://github.com/open-mmlab/
-mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent
-**C**reation toolbox. - [MMDetection](https://github.com/open-mmlab/
-mmdetection): OpenMMLab detection toolbox and benchmark. - [MMYOLO](https://
-github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
-video perception toolbox and benchmark. - [MMSegmentation](https://github.com/
-open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and
-benchmark. - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text
-detection, recognition, and understanding toolbox. - [MMPose](https://
-github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human
-parametric model toolbox and benchmark. - [MMFewShot](https://github.com/open-
-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark. -
-[MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-
-generation action understanding toolbox and benchmark. - [MMFlow](https://
-github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. -
-[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment
-Framework. - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model
-compression toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim):
-MIM installs OpenMMLab packages. - [Playground](https://github.com/open-mmlab/
-playground): A central hub for gathering and showcasing amazing projects built
-upon OpenMMLab. Keywords: computer vision,semantic segmentation Platform:
-UNKNOWN Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Description-
-Content-Type: text/markdown Provides-Extra: all Provides-Extra: tests Provides-
-Extra: optional Provides-Extra: mim
+user_guides/2_dataset_prepare.md#levir-cd) - [x] [BDD100K](https://github.com/
+open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/
+2_dataset_prepare.md#bdd100K)  Please refer to [FAQ](docs/en/notes/faq.md) for
+frequently asked questions. ## Projects [Here](projects/README.md) are some
+implementations of SOTA models and solutions built on MMSegmentation, which are
+supported and maintained by community users. These projects demonstrate the
+best practices based on MMSegmentation for research and product development. We
+welcome and appreciate all the contributions to OpenMMLab ecosystem. ##
+Contributing We appreciate all contributions to improve MMSegmentation. Please
+refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
+guideline. ## Acknowledgement MMSegmentation is an open source project that
+welcome any contribution and feedback. We wish that the toolbox and benchmark
+could serve the growing research community by providing a flexible as well as
+standardized toolkit to reimplement existing methods and develop their own new
+semantic segmentation methods. ## Citation If you find this project useful in
+your research, please consider cite: ```bibtex @misc{mmseg2020, title={
+{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox and Benchmark},
+author={MMSegmentation Contributors}, howpublished = {\url{https://github.com/
+open-mmlab/mmsegmentation}}, year={2020} } ``` ## License This project is
+released under the [Apache 2.0 license](LICENSE). ## OpenMMLab Family -
+[MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational
+library for training deep learning models. - [MMCV](https://github.com/open-
+mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MMPreTrain]
+(https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and
+benchmark. - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab
+**A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox. -
+[MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection
+toolbox and benchmark. - [MMYOLO](https://github.com/open-mmlab/mmyolo):
+OpenMMLab YOLO series toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for
+general 3D object detection. - [MMRotate](https://github.com/open-mmlab/
+mmrotate): OpenMMLab rotated object detection toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video
+perception toolbox and benchmark. - [MMSegmentation](https://github.com/open-
+mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark. -
+[MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D]
+(https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model
+toolbox and benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot):
+OpenMMLab fewshot learning toolbox and benchmark. - [MMAction2](https://
+github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action
+understanding toolbox and benchmark. - [MMFlow](https://github.com/open-mmlab/
+mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMDeploy](https://
+github.com/open-mmlab/mmdeploy): OpenMMLab Model Deployment Framework. -
+[MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression
+toolbox and benchmark. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [Playground](https://github.com/open-mmlab/playground): A
+central hub for gathering and showcasing amazing projects built upon OpenMMLab.
+Keywords: computer vision,semantic segmentation Platform: UNKNOWN Classifier:
+Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+Provides-Extra: all Provides-Extra: tests Provides-Extra: optional Provides-
+Extra: mim
```

### Comparing `mmsegmentation-1.1.0/mmsegmentation.egg-info/SOURCES.txt` & `mmsegmentation-1.1.1/mmsegmentation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 mmseg/__init__.py
 mmseg/version.py
 mmseg/.mim/model-index.yml
 mmseg/.mim/configs/_base_/default_runtime.py
 mmseg/.mim/configs/_base_/datasets/ade20k.py
 mmseg/.mim/configs/_base_/datasets/ade20k_640x640.py
+mmseg/.mim/configs/_base_/datasets/bdd100k.py
 mmseg/.mim/configs/_base_/datasets/chase_db1.py
 mmseg/.mim/configs/_base_/datasets/cityscapes.py
 mmseg/.mim/configs/_base_/datasets/cityscapes_1024x1024.py
 mmseg/.mim/configs/_base_/datasets/cityscapes_768x768.py
 mmseg/.mim/configs/_base_/datasets/cityscapes_769x769.py
 mmseg/.mim/configs/_base_/datasets/cityscapes_832x832.py
 mmseg/.mim/configs/_base_/datasets/coco-stuff10k.py
@@ -305,15 +306,14 @@
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-160k_ade20k-512x512.py
 mmseg/.mim/configs/dnlnet/dnl_r50-d8_4xb4-80k_ade20k-512x512.py
 mmseg/.mim/configs/dnlnet/metafile.yaml
 mmseg/.mim/configs/dpt/dpt_vit-b16_8xb2-160k_ade20k-512x512.py
 mmseg/.mim/configs/dpt/metafile.yaml
 mmseg/.mim/configs/dsdl/cityscapes.py
-mmseg/.mim/configs/dsdl/metafile.yaml
 mmseg/.mim/configs/dsdl/voc.py
 mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/emanet/emanet_r101-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-512x1024.py
 mmseg/.mim/configs/emanet/emanet_r50-d8_4xb2-80k_cityscapes-769x769.py
 mmseg/.mim/configs/emanet/metafile.yaml
 mmseg/.mim/configs/encnet/encnet_r101-d8_4xb2-40k_cityscapes-512x1024.py
@@ -854,14 +854,15 @@
 mmseg/.mim/tools/torchserve/test_torchserve.py
 mmseg/apis/__init__.py
 mmseg/apis/inference.py
 mmseg/apis/mmseg_inferencer.py
 mmseg/datasets/__init__.py
 mmseg/datasets/ade.py
 mmseg/datasets/basesegdataset.py
+mmseg/datasets/bdd100k.py
 mmseg/datasets/chase_db1.py
 mmseg/datasets/cityscapes.py
 mmseg/datasets/coco_stuff.py
 mmseg/datasets/dark_zurich.py
 mmseg/datasets/dataset_wrappers.py
 mmseg/datasets/decathlon.py
 mmseg/datasets/drive.py
```

### Comparing `mmsegmentation-1.1.0/setup.cfg` & `mmsegmentation-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/setup.py` & `mmsegmentation-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_config.py` & `mmsegmentation-1.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_digit_version.py` & `mmsegmentation-1.1.1/tests/test_digit_version.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_beit.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_beit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv1.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_bisenetv1.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_bisenetv2.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_bisenetv2.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_blocks.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_blocks.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_cgnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_cgnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_erfnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_erfnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_fast_scnn.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_fast_scnn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_hrnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_hrnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_icnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_icnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mae.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mae.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mit.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mobilenet_v3.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_mscan.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_mscan.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_pidnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_pidnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnest.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnest.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_resnext.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_resnext.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_stdc.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_stdc.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_swin.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_swin.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_timm_backbone.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_timm_backbone.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_twins.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_twins.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_unet.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_unet.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/test_vit.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/test_vit.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_backbones/utils.py` & `mmsegmentation-1.1.1/tests/test_models/test_backbones/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_data_preprocessor.py` & `mmsegmentation-1.1.1/tests/test_models/test_data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_forward.py` & `mmsegmentation-1.1.1/tests/test_models/test_forward.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ann_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_ann_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_apc_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_apc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_aspp_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_aspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_cc_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_cc_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_decode_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_decode_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dm_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_dm_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dnl_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_dnl_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_dpt_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_dpt_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ema_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_ema_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_fcn_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_fcn_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ham_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_ham_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_isa_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_isa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_lraspp_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_lraspp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_mask2former_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_mask2former_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_maskformer_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_maskformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_ocr_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_ocr_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_pidnet_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_pidnet_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_psa_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_psa_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_psp_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_psp_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_segformer_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_segformer_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_segmenter_mask_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_segmenter_mask_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_mla_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_setr_mla_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_setr_up_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_setr_up_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/test_uper_head.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/test_uper_head.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_heads/utils.py` & `mmsegmentation-1.1.1/tests/test_models/test_heads/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_feature2pyramid.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_feature2pyramid.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_fpn.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_fpn.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_ic_neck.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_ic_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_jpu.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_jpu.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_mla_neck.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_mla_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_necks/test_multilevel_neck.py` & `mmsegmentation-1.1.1/tests/test_models/test_necks/test_multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py` & `mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_encoder_decoder.py` & `mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_segmentors/test_seg_tta_model.py` & `mmsegmentation-1.1.1/tests/test_models/test_segmentors/test_seg_tta_model.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_segmentors/utils.py` & `mmsegmentation-1.1.1/tests/test_models/test_segmentors/utils.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_utils/test_embed.py` & `mmsegmentation-1.1.1/tests/test_models/test_utils/test_embed.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_models/test_utils/test_shape_convert.py` & `mmsegmentation-1.1.1/tests/test_models/test_utils/test_shape_convert.py`

 * *Files identical despite different names*

### Comparing `mmsegmentation-1.1.0/tests/test_sampler.py` & `mmsegmentation-1.1.1/tests/test_sampler.py`

 * *Files identical despite different names*

