# Comparing `tmp/funasr-0.7.0.tar.gz` & `tmp/funasr-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.7.0.tar", last modified: Fri Jul 14 11:07:13 2023, max compression
+gzip compressed data, was "funasr-0.7.1.tar", last modified: Mon Jul 24 10:53:51 2023, max compression
```

## Comparing `funasr-0.7.0.tar` & `funasr-0.7.1.tar`

### file list

```diff
@@ -1,446 +1,460 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.900815 funasr-0.7.0/
--rw-r--r--   0 zhifu      (502) staff       (20)    10026 2023-07-14 11:07:13.900558 funasr-0.7.0/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     9049 2023-07-14 07:04:33.000000 funasr-0.7.0/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.504896 funasr-0.7.0/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.537545 funasr-0.7.0/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    71935 2023-07-14 11:00:31.000000 funasr-0.7.0/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.7.0/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5565 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12181 2023-07-14 11:00:09.000000 funasr-0.7.0/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.543590 funasr-0.7.0/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.7.0/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18908 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_model_from_file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_streaming_iterator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_sv_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.7.0/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.545767 funasr-0.7.0/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.546897 funasr-0.7.0/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.565961 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.572755 funasr-0.7.0/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3118 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.575120 funasr-0.7.0/funasr/datasets/small_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.7.0/funasr/datasets/small_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/datasets/small_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/datasets/small_datasets/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.575966 funasr-0.7.0/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.7.0/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.582351 funasr-0.7.0/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.584123 funasr-0.7.0/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.586876 funasr-0.7.0/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.7.0/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.589334 funasr-0.7.0/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.590155 funasr-0.7.0/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.7.0/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.592458 funasr-0.7.0/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.7.0/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.593201 funasr-0.7.0/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.7.0/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.597759 funasr-0.7.0/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.600592 funasr-0.7.0/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.668629 funasr-0.7.0/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.669178 funasr-0.7.0/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.7.0/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.702733 funasr-0.7.0/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.732041 funasr-0.7.0/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.738613 funasr-0.7.0/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/e2e_asr_bat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-05 02:29:20.000000 funasr-0.7.0/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100274 2023-07-07 03:08:26.000000 funasr-0.7.0/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.773296 funasr-0.7.0/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20694 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/models/encoder/branchformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17014 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/models/encoder/e_branchformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.7.0/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.775695 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.782351 funasr-0.7.0/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.783439 funasr-0.7.0/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.784277 funasr-0.7.0/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.785459 funasr-0.7.0/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.786119 funasr-0.7.0/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-02 01:20:55.000000 funasr-0.7.0/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.787910 funasr-0.7.0/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.789111 funasr-0.7.0/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.798122 funasr-0.7.0/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.800897 funasr-0.7.0/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.7.0/funasr/modules/beam_search/beam_search_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3480 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/cgmlp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.803738 funasr-0.7.0/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.7.0/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.804611 funasr-0.7.0/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/modules/eend_ola/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.806217 funasr-0.7.0/funasr/modules/eend_ola/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/modules/eend_ola/utils/report.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-05 02:28:53.000000 funasr-0.7.0/funasr/modules/embedding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5282 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/fastformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.808662 funasr-0.7.0/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-06 11:07:58.000000 funasr-0.7.0/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.7.0/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4283 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.811110 funasr-0.7.0/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.812401 funasr-0.7.0/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.813814 funasr-0.7.0/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.7.0/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.814802 funasr-0.7.0/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.815201 funasr-0.7.0/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.815389 funasr-0.7.0/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.816368 funasr-0.7.0/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.7.0/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.817141 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.819711 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-06-30 02:11:21.000000 funasr-0.7.0/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.823282 funasr-0.7.0/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.825611 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.830272 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr-0.7.0/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.833912 funasr-0.7.0/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.835661 funasr-0.7.0/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-05 02:28:54.000000 funasr-0.7.0/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.840134 funasr-0.7.0/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    62140 2023-07-13 09:35:41.000000 funasr-0.7.0/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.850601 funasr-0.7.0/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.854034 funasr-0.7.0/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.7.0/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.855775 funasr-0.7.0/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.7.0/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.874817 funasr-0.7.0/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.7.0/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.7.0/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.7.0/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.7.0/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.7.0/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.7.0/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-07 03:08:09.000000 funasr-0.7.0/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.7.0/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.7.0/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.7.0/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.7.0/funasr/utils/runtime_sdk_download_tool.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.7.0/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.7.0/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.7.0/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.7.0/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-14 11:02:23.000000 funasr-0.7.0/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.506233 funasr-0.7.0/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)    10026 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    14184 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      757 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-14 11:07:13.000000 funasr-0.7.0/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-14 11:07:13.900886 funasr-0.7.0/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     3630 2023-06-30 02:11:21.000000 funasr-0.7.0/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-14 11:07:13.900006 funasr-0.7.0/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-05 02:29:20.000000 funasr-0.7.0/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.7.0/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.7.0/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.7.0/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.7.0/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-05 02:28:54.000000 funasr-0.7.0/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.7.0/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.161891 funasr-0.7.1/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8016 2023-07-24 10:53:51.161639 funasr-0.7.1/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7039 2023-07-24 05:54:34.000000 funasr-0.7.1/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.722039 funasr-0.7.1/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.744846 funasr-0.7.1/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72259 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6109 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12386 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18267 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12181 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.771938 funasr-0.7.1/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.7.1/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18908 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.780536 funasr-0.7.1/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.789547 funasr-0.7.1/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3795 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.812804 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.819080 funasr-0.7.1/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3114 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32729 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.828678 funasr-0.7.1/funasr/datasets/small_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/datasets/small_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/datasets/small_datasets/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.836788 funasr-0.7.1/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5045 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/export_conformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.844622 funasr-0.7.1/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1724 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.849379 funasr-0.7.1/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4105 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/decoder/xformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2454 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/e2e_asr_conformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.852017 funasr-0.7.1/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.7.1/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.869598 funasr-0.7.1/funasr/export/models/language_models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14582 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/embed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2590 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/seq_rnn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5481 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3907 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/export/models/language_models/transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.871805 funasr-0.7.1/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.872516 funasr-0.7.1/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.7.1/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.874588 funasr-0.7.1/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.7.1/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.875352 funasr-0.7.1/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.7.1/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.878238 funasr-0.7.1/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.900590 funasr-0.7.1/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.940229 funasr-0.7.1/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.940802 funasr-0.7.1/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.7.1/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.944544 funasr-0.7.1/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.959535 funasr-0.7.1/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.965712 funasr-0.7.1/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75537 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_bat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100274 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.974893 funasr-0.7.1/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20694 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17014 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/e_branchformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.7.1/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.976805 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56561 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.982167 funasr-0.7.1/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.983725 funasr-0.7.1/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.984555 funasr-0.7.1/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.7.1/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.986770 funasr-0.7.1/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.987498 funasr-0.7.1/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.989842 funasr-0.7.1/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.990895 funasr-0.7.1/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.009528 funasr-0.7.1/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40008 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.039857 funasr-0.7.1/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.7.1/funasr/modules/beam_search/beam_search_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3480 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/cgmlp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.042750 funasr-0.7.1/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.7.1/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.043471 funasr-0.7.1/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.045489 funasr-0.7.1/funasr/modules/eend_ola/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/eend_ola/utils/report.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/embedding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5282 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/fastformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.053949 funasr-0.7.1/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/lightconv2d.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.054805 funasr-0.7.1/funasr/modules/lora/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12553 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/layers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1839 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/modules/lora/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.7.1/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4283 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.060990 funasr-0.7.1/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.062427 funasr-0.7.1/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.063865 funasr-0.7.1/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/modules/subsampling_without_posenc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2782 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/modules/vgg2l.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.064995 funasr-0.7.1/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.065261 funasr-0.7.1/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.065568 funasr-0.7.1/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.066509 funasr-0.7.1/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.7.1/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.067258 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.069802 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.072269 funasr-0.7.1/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.073602 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.078128 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.080498 funasr-0.7.1/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.081596 funasr-0.7.1/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.094409 funasr-0.7.1/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73020 2023-07-21 07:26:44.000000 funasr-0.7.1/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    62140 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.133998 funasr-0.7.1/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.138709 funasr-0.7.1/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.7.1/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.148461 funasr-0.7.1/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.7.1/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38500 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.158716 funasr-0.7.1/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.7.1/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.7.1/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.7.1/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.7.1/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/runtime_sdk_download_tool.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13725 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.7.1/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-07-21 03:47:46.000000 funasr-0.7.1/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.7.1/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-24 10:52:35.000000 funasr-0.7.1/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:50.724327 funasr-0.7.1/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8016 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    14670 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      763 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-24 10:53:50.000000 funasr-0.7.1/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-24 10:53:51.161961 funasr-0.7.1/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3648 2023-07-21 03:47:46.000000 funasr-0.7.1/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-24 10:53:51.160660 funasr-0.7.1/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.7.1/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.7.1/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-07-21 03:47:46.000000 funasr-0.7.1/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.7.0/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.7.1/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/asr_infer.py` & `funasr-0.7.1/funasr/bin/asr_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/asr_inference_launch.py` & `funasr-0.7.1/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,15 @@
             logging.info("decoding, utt_id: {}".format(keys))
             # N-best list of (text, token, token_int, hyp_object)
 
             time_beg = time.time()
             results = speech2text(**batch)
             if len(results) < 1:
                 hyp = Hypothesis(score=0.0, scores={}, states={}, yseq=[])
-                results = [[" ", ["sil"], [2], hyp, 10, 6]] * nbest
+                results = [[" ", ["sil"], [2], hyp, 10, 6, []]] * nbest
             time_end = time.time()
             forward_time = time_end - time_beg
             lfr_factor = results[0][-1]
             length = results[0][-2]
             forward_time_total += forward_time
             length_total += length
             rtf_cur = "decoding, feature length: {}, forward_time: {:.4f}, rtf: {:.4f}".format(length, forward_time,
@@ -561,14 +561,16 @@
         hotword_list_or_file = None
         if param_dict is not None:
             hotword_list_or_file = param_dict.get('hotword')
 
         if 'hotword' in kwargs:
             hotword_list_or_file = kwargs['hotword']
 
+        speech2vadsegment.vad_model.vad_opts.max_single_segment_time = kwargs.get("max_single_segment_time", 60000)
+        batch_size_token_threshold_s = kwargs.get("batch_size_token_threshold_s", int(speech2vadsegment.vad_model.vad_opts.max_single_segment_time*0.67/1000)) * 1000
         batch_size_token = kwargs.get("batch_size_token", 6000)
         print("batch_size_token: ", batch_size_token)
 
         if speech2text.hotword_list is None:
             speech2text.hotword_list = speech2text.generate_hotwords_list(hotword_list_or_file)
 
         # 3. Build data-iterator
@@ -643,16 +645,15 @@
             if len(sorted_data) > 0 and len(sorted_data[0]) > 0:
                 batch_size_token_ms = max(batch_size_token_ms, sorted_data[0][0][1] - sorted_data[0][0][0])
             
             batch_size_token_ms_cum = 0
             beg_idx = 0
             for j, _ in enumerate(range(0, n)):
                 batch_size_token_ms_cum += (sorted_data[j][0][1] - sorted_data[j][0][0])
-                if j < n - 1 and (batch_size_token_ms_cum + sorted_data[j + 1][0][1] - sorted_data[j + 1][0][
-                    0]) < batch_size_token_ms:
+                if j < n - 1 and (batch_size_token_ms_cum + sorted_data[j + 1][0][1] - sorted_data[j + 1][0][0]) < batch_size_token_ms and (sorted_data[j + 1][0][1] - sorted_data[j + 1][0][0]) < batch_size_token_threshold_s:
                     continue
                 batch_size_token_ms_cum = 0
                 end_idx = j + 1
                 speech_j, speech_lengths_j = slice_padding_fbank(speech, speech_lengths, sorted_data[beg_idx:end_idx])
                 beg_idx = end_idx
                 batch = {"speech": speech_j, "speech_lengths": speech_lengths_j}
                 batch = to_device(batch, device=device)
@@ -1336,15 +1337,15 @@
         raise NotImplementedError("only single GPU decoding is supported")
 
     logging.basicConfig(
         level=log_level,
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
-    if ngpu >= 1:
+    if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
     # 1. Set random-seed
     set_all_random_seed(seed)
 
     # 2. Build speech2text
@@ -1367,18 +1368,15 @@
         quantize_dtype=quantize_dtype,
         streaming=streaming,
         simu_streaming=simu_streaming,
         chunk_size=chunk_size,
         left_context=left_context,
         right_context=right_context,
     )
-    speech2text = Speech2TextTransducer.from_pretrained(
-        model_tag=model_tag,
-        **speech2text_kwargs,
-    )
+    speech2text = Speech2TextTransducer(**speech2text_kwargs)
 
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
```

### Comparing `funasr-0.7.0/funasr/bin/asr_train.py` & `funasr-0.7.1/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/build_trainer.py` & `funasr-0.7.1/funasr/bin/build_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 import yaml
 
-
 def update_dct(fin_configs, root):
     if root == {}:
         return {}
     for root_key, root_value in root.items():
         if not isinstance(root[root_key], dict):
             fin_configs[root_key] = root[root_key]
         else:
@@ -51,15 +50,15 @@
                   max_epoch=None,
                   optim=None,
                   lr=None,
                   scheduler=None,
                   scheduler_conf=None,
                   specaug=None,
                   specaug_conf=None,
-                  param_dict=None,
+                  mate_params=None,
                   **kwargs):
     mode = modelscope_dict['mode']
     args, ASRTask = parse_args(mode=mode)
     # ddp related
     if args.local_rank is not None:
         distributed = True
     else:
@@ -88,28 +87,39 @@
             # finetune_configs["dataset_conf"]["data_types"] = "sound,text"
             if 'data_types' not in finetune_configs['dataset_conf']:
                 finetune_configs["dataset_conf"]["data_types"] = "sound,text"
     finetune_configs = update_dct(configs, finetune_configs)
     for key, value in finetune_configs.items():
         if hasattr(args, key):
             setattr(args, key, value)
+    if mate_params is not None:
+        for key, value in mate_params.items():
+            if hasattr(args, key):
+                setattr(args, key, value)
+    if mate_params is not None and "lora_params" in mate_params:
+        lora_params = mate_params['lora_params']
+        configs['encoder_conf'].update(lora_params) 
+        configs['decoder_conf'].update(lora_params) 
 
     # prepare data
     args.dataset_type = dataset_type
     if args.dataset_type == "small":
         args.train_data_path_and_name_and_type = [["{}/{}/wav.scp".format(data_dir, train_set), "speech", "sound"],
                                                   ["{}/{}/text".format(data_dir, train_set), "text", "text"]]
         args.valid_data_path_and_name_and_type = [["{}/{}/wav.scp".format(data_dir, dev_set), "speech", "sound"],
                                                   ["{}/{}/text".format(data_dir, dev_set), "text", "text"]]
     elif args.dataset_type == "large":
         args.train_data_file = None
         args.valid_data_file = None
     else:
         raise ValueError(f"Not supported dataset_type={args.dataset_type}")
     args.init_param = [init_param]
+    if mate_params is not None and "init_param" in mate_params:
+        if len(mate_params["init_param"]) != 0:
+            args.init_param = mate_params["init_param"]
     args.cmvn_file = cmvn_file
     if os.path.exists(seg_dict_file):
         args.seg_dict_file = seg_dict_file
     else:
         args.seg_dict_file = None
     args.data_dir = data_dir
     args.train_set = train_set
```

### Comparing `funasr-0.7.0/funasr/bin/data2vec_train.py` & `funasr-0.7.1/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/diar_infer.py` & `funasr-0.7.1/funasr/bin/diar_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/diar_inference_launch.py` & `funasr-0.7.1/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/diar_train.py` & `funasr-0.7.1/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/lm_inference_launch.py` & `funasr-0.7.1/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/lm_train.py` & `funasr-0.7.1/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/punc_infer.py` & `funasr-0.7.1/funasr/bin/punc_infer.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #  MIT License  (https://opensource.org/licenses/MIT)
 
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import torch
+import os
 
 from funasr.build_utils.build_model_from_file import build_model_from_file
 from funasr.datasets.preprocessor import CodeMixTokenizerCommonPreprocessor
 from funasr.datasets.preprocessor import split_to_mini_sentence
 from funasr.torch_utils.device_funcs import to_device
 from funasr.torch_utils.forward_adaptor import ForwardAdaptor
 
@@ -37,23 +38,30 @@
         for i in range(len(self.punc_list)):
             if self.punc_list[i] == ",":
                 self.punc_list[i] = "，"
             elif self.punc_list[i] == "?":
                 self.punc_list[i] = "？"
             elif self.punc_list[i] == "。":
                 self.period = i
+        self.seg_dict_file = None
+        self.seg_jieba = False
+        if "seg_jieba" in train_args:
+            self.seg_jieba = train_args.seg_jieba
+            self.seg_dict_file = os.path.dirname(model_file)+"/"+ "jieba_usr_dict"
         self.preprocessor = CodeMixTokenizerCommonPreprocessor(
             train=False,
             token_type=train_args.token_type,
             token_list=train_args.token_list,
             bpemodel=train_args.bpemodel,
             text_cleaner=train_args.cleaner,
             g2p_type=train_args.g2p,
             text_name="text",
             non_linguistic_symbols=train_args.non_linguistic_symbols,
+            seg_jieba=self.seg_jieba,
+            seg_dict_file=self.seg_dict_file
         )
 
     @torch.no_grad()
     def __call__(self, text: Union[list, str], split_size=20):
         data = {"text": text}
         result = self.preprocessor(data=data, uid="12938712838719")
         split_text = self.preprocessor.pop_split_text_data(result)
```

### Comparing `funasr-0.7.0/funasr/bin/punc_inference_launch.py` & `funasr-0.7.1/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/punc_train.py` & `funasr-0.7.1/funasr/bin/punc_train.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,8 +40,14 @@
 
     # DDP settings
     if args.ngpu > 1:
         args.distributed = True
     else:
         args.distributed = False
 
+    if args.dataset_type == "small":
+        if args.batch_size is not None:
+            args.batch_size = args.batch_size * args.ngpu * args.num_worker_count
+        if args.batch_bins is not None:
+            args.batch_bins = args.batch_bins * args.ngpu * args.num_worker_count
+
     main(args=args)
```

### Comparing `funasr-0.7.0/funasr/bin/sa_asr_train.py` & `funasr-0.7.1/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/sv_infer.py` & `funasr-0.7.1/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/sv_inference_launch.py` & `funasr-0.7.1/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/tokenize_text.py` & `funasr-0.7.1/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/tp_infer.py` & `funasr-0.7.1/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/tp_inference_launch.py` & `funasr-0.7.1/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/train.py` & `funasr-0.7.1/funasr/bin/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from funasr.torch_utils.set_all_random_seed import set_all_random_seed
 from funasr.utils.nested_dict_action import NestedDictAction
 from funasr.utils.prepare_data import prepare_data
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str_or_none
 from funasr.utils.yaml_no_alias_safe_dump import yaml_no_alias_safe_dump
+from funasr.modules.lora.utils import mark_only_lora_as_trainable
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
         description="FunASR Common Training Parser",
     )
 
@@ -474,14 +475,26 @@
         help="The bucket name for oss.",
     )
     parser.add_argument(
         "--oss_bucket",
         default=None,
         help="oss bucket.",
     )
+    parser.add_argument(
+        "--enable_lora",
+        type=str2bool,
+        default=False,
+        help="Apply lora for finetuning.",
+    )
+    parser.add_argument(
+        "--lora_bias",
+        type=str,
+        default="none",
+        help="lora bias.",
+    )
 
     return parser
 
 
 if __name__ == '__main__':
     parser = get_parser()
     args, extra_task_params = parser.parse_known_args()
@@ -517,14 +530,16 @@
     prepare_data(args, distributed_option)
 
     model = build_model(args)
     model = model.to(
         dtype=getattr(torch, args.train_dtype),
         device="cuda" if args.ngpu > 0 else "cpu",
     )
+    if args.enable_lora:
+        mark_only_lora_as_trainable(model, args.lora_bias)
     for t in args.freeze_param:
         for k, p in model.named_parameters():
             if k.startswith(t + ".") or k == t:
                 logging.info(f"Setting {k}.requires_grad = False")
                 p.requires_grad = False
 
     optimizers = build_optimizer(args, model=model)
```

### Comparing `funasr-0.7.0/funasr/bin/vad_infer.py` & `funasr-0.7.1/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/bin/vad_inference_launch.py` & `funasr-0.7.1/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_args.py` & `funasr-0.7.1/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_asr_model.py` & `funasr-0.7.1/funasr/build_utils/build_asr_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_dataloader.py` & `funasr-0.7.1/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_diar_model.py` & `funasr-0.7.1/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_distributed.py` & `funasr-0.7.1/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_lm_model.py` & `funasr-0.7.1/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_model.py` & `funasr-0.7.1/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_model_from_file.py` & `funasr-0.7.1/funasr/build_utils/build_model_from_file.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_optimizer.py` & `funasr-0.7.1/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_pretrain_model.py` & `funasr-0.7.1/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_punc_model.py` & `funasr-0.7.1/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_scheduler.py` & `funasr-0.7.1/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_streaming_iterator.py` & `funasr-0.7.1/funasr/build_utils/build_streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_sv_model.py` & `funasr-0.7.1/funasr/build_utils/build_sv_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_trainer.py` & `funasr-0.7.1/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/build_utils/build_vad_model.py` & `funasr-0.7.1/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/collate_fn.py` & `funasr-0.7.1/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/dataset.py` & `funasr-0.7.1/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/iterable_dataset.py` & `funasr-0.7.1/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.7.1/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,20 +65,23 @@
 class LargeDataLoader(AbsIterFactory):
     def __init__(self, args, mode="train"):
         symbol_table, seg_dict, punc_dict, bpe_tokenizer = None, None, None, None
         if hasattr(args, "token_list") and args.token_list is not None:
             symbol_table = read_symbol_table(args.token_list)
         if hasattr(args, "seg_dict_file") and args.seg_dict_file is not None:
             seg_dict = load_seg_dict(args.seg_dict_file)
-        if hasattr(args, "punc_dict_file") and args.punc_dict_file is not None:
-            punc_dict = read_symbol_table(args.punc_dict_file)
+        if hasattr(args, "punc_list") and args.punc_list is not None:
+            punc_dict = read_symbol_table(args.punc_list)
         if hasattr(args, "bpemodel") and args.bpemodel is not None:
             bpe_tokenizer = SentencepiecesTokenizer(args.bpemodel)
         self.dataset_conf = args.dataset_conf
-        self.frontend_conf = args.frontend_conf
+        if "frontend_conf" not in args:
+            self.frontend_conf =  None
+        else:
+            self.frontend_conf = args.frontend_conf
         self.speed_perturb = args.speed_perturb if hasattr(args, "speed_perturb") else None 
         logging.info("dataloader config: {}".format(self.dataset_conf))
         batch_mode = self.dataset_conf.get("batch_mode", "padding")
         data_list = args.train_data_file if mode == "train" else args.valid_data_file
         self.dataset = Dataset(data_list, symbol_table, seg_dict, punc_dict, bpe_tokenizer,
                                self.dataset_conf, self.frontend_conf,
                                speed_perturb=self.speed_perturb if mode == "train" else None,
```

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.7.1/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.7.1/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/dataset.py` & `funasr-0.7.1/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.7.1/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
         text = bpe_tokenizer.text2tokens(" ".join(text))
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         text = seg_tokenize(text, seg_dict)
 
     length = len(text)
     if 'hw_tag' in data:
+        pre_index = None
         if hw_config['pre_hwlist'] is not None and hw_config['pre_prob'] > 0:
             # enable preset hotword detect in sampling
-            pre_index = None
             for hw in hw_config['pre_hwlist']:
                 hw = " ".join(seg_tokenize(hw, seg_dict))
                 _find = " ".join(text).find(hw)
                 if _find != -1:
                     # _find = text[:_find].count(" ")  # bpe sometimes
                     pre_index = [_find, _find + max(hw.count(" "), 1)]
                     break
```

### Comparing `funasr-0.7.0/funasr/datasets/ms_dataset.py` & `funasr-0.7.1/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/preprocessor.py` & `funasr-0.7.1/funasr/datasets/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List
 from typing import Union
 
 import numpy as np
 import scipy.signal
 import soundfile
 
+
 from funasr.text.build_tokenizer import build_tokenizer
 from funasr.text.cleaner import TextCleaner
 from funasr.text.token_id_converter import TokenIDConverter
 
 
 class AbsPreprocessor(ABC):
     def __init__(self, train: bool):
@@ -624,14 +625,15 @@
             noise_apply_prob: float = 1.0,
             noise_db_range: str = "3_10",
             speech_volume_normalize: float = None,
             speech_name: str = "speech",
             text_name: str = "text",
             split_text_name: str = "split_text",
             split_with_space: bool = False,
+            seg_jieba: bool = False,
             seg_dict_file: str = None,
     ):
         super().__init__(
             train=train,
             # Force to use word.
             token_type="word",
             token_list=token_list,
@@ -651,14 +653,18 @@
             noise_db_range=noise_db_range,
             speech_volume_normalize=speech_volume_normalize,
             split_with_space=split_with_space,
             seg_dict_file=seg_dict_file,
         )
         # The data field name for split text.
         self.split_text_name = split_text_name
+        self.seg_jieba = seg_jieba
+        if self.seg_jieba:
+            import jieba
+            jieba.load_userdict(seg_dict_file)
 
     @classmethod
     def split_words(cls, text: str):
         words = []
         segs = text.split()
         for seg in segs:
             # There is no space in seg.
@@ -673,20 +679,81 @@
                         words.append(current_word)
                         current_word = ""
                     words.append(c)
             if len(current_word) > 0:
                 words.append(current_word)
         return words
 
+    @classmethod
+    def isEnglish(cls, text:str):
+        if re.search('^[a-zA-Z\']+$', text):
+            return True
+        else:
+            return False
+
+    @classmethod
+    def join_chinese_and_english(cls, input_list):
+        line = ''
+        for token in input_list:
+            if cls.isEnglish(token):
+                line = line + ' ' + token
+            else:
+                line = line + token
+
+        line = line.strip()
+        return line   
+
+    @classmethod
+    def split_words_jieba(cls, text: str):
+        input_list = text.split()
+        token_list_all = []
+        langauge_list = []
+        token_list_tmp = []
+        language_flag = None
+        for token in input_list:
+            if cls.isEnglish(token) and language_flag == 'Chinese':
+                token_list_all.append(token_list_tmp)
+                langauge_list.append('Chinese')
+                token_list_tmp = []
+            elif not cls.isEnglish(token) and language_flag == 'English':
+                token_list_all.append(token_list_tmp)
+                langauge_list.append('English')
+                token_list_tmp = []
+
+            token_list_tmp.append(token)
+
+            if cls.isEnglish(token):
+                language_flag = 'English'
+            else:
+                language_flag = 'Chinese'
+
+        if token_list_tmp:
+            token_list_all.append(token_list_tmp)
+            langauge_list.append(language_flag)
+
+        result_list = []
+        for token_list_tmp, language_flag in zip(token_list_all, langauge_list):
+            if language_flag == 'English':
+                result_list.extend(token_list_tmp)
+            else:
+                seg_list = jieba.cut(cls.join_chinese_and_english(token_list_tmp), HMM=False)
+                result_list.extend(seg_list)
+
+        return result_list
+
     def __call__(
             self, uid: str, data: Dict[str, Union[list, str, np.ndarray]]
     ) -> Dict[str, Union[list, np.ndarray]]:
         # Split words.
         if isinstance(data[self.text_name], str):
-            split_text = self.split_words(data[self.text_name])
+            if self.seg_jieba:
+  #              jieba.load_userdict(seg_dict_file)
+                split_text = self.split_words_jieba(data[self.text_name])
+            else:
+                split_text = self.split_words(data[self.text_name])
         else:
             split_text = data[self.text_name]
         data[self.text_name] = " ".join(split_text)
         data = self._speech_process(data)
         data = self._text_process(data)
         data[self.split_text_name] = split_text
         return data
@@ -778,15 +845,14 @@
         self.vad_name = vad_name
 
     def _text_process(
             self, data: Dict[str, Union[str, np.ndarray]]
     ) -> Dict[str, np.ndarray]:
         for i in range(self.num_tokenizer):
             text_name = self.text_name[i]
-            #import pdb; pdb.set_trace()
             if text_name in data and self.tokenizer[i] is not None:
                 text = data[text_name]
                 text = self.text_cleaner(text)
                 tokens = self.tokenizer[i].text2tokens(text)
                 if "vad:" in tokens[-1]:
                     vad = tokens[-1][4:]
                     tokens = tokens[:-1]
```

### Comparing `funasr-0.7.0/funasr/datasets/small_datasets/collate_fn.py` & `funasr-0.7.1/funasr/datasets/small_datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/small_datasets/dataset.py` & `funasr-0.7.1/funasr/datasets/small_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/small_datasets/length_batch_sampler.py` & `funasr-0.7.1/funasr/datasets/small_datasets/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/small_datasets/preprocessor.py` & `funasr-0.7.1/funasr/datasets/small_datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/datasets/small_datasets/sequence_iter_factory.py` & `funasr-0.7.1/funasr/datasets/small_datasets/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/export_model.py` & `funasr-0.7.1/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/CT_Transformer.py` & `funasr-0.7.1/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/__init__.py` & `funasr-0.7.1/funasr/export/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from funasr.models.e2e_asr_paraformer import Paraformer, BiCifParaformer
 from funasr.export.models.e2e_asr_paraformer import Paraformer as Paraformer_export
 from funasr.export.models.e2e_asr_paraformer import BiCifParaformer as BiCifParaformer_export
+from funasr.export.models.e2e_asr_conformer import Conformer as Conformer_export
+
 from funasr.models.e2e_vad import E2EVadModel
 from funasr.export.models.e2e_vad import E2EVadModel as E2EVadModel_export
 from funasr.models.target_delay_transformer import TargetDelayTransformer
 from funasr.export.models.CT_Transformer import CT_Transformer as CT_Transformer_export
 from funasr.train.abs_model import PunctuationModel
 from funasr.models.vad_realtime_transformer import VadRealtimeTransformer
 from funasr.export.models.CT_Transformer import CT_Transformer_VadRealtime as CT_Transformer_VadRealtime_export
 
 def get_model(model, export_config=None):
     if isinstance(model, BiCifParaformer):
         return BiCifParaformer_export(model, **export_config)
     elif isinstance(model, Paraformer):
         return Paraformer_export(model, **export_config)
+    elif isinstance(model, Conformer_export):
+        return Conformer_export(model, **export_config)
     elif isinstance(model, E2EVadModel):
         return E2EVadModel_export(model, **export_config)
     elif isinstance(model, PunctuationModel):
         if isinstance(model.punc_model, TargetDelayTransformer):
             return CT_Transformer_export(model.punc_model, **export_config)
         elif isinstance(model.punc_model, VadRealtimeTransformer):
             return CT_Transformer_VadRealtime_export(model.punc_model, **export_config)
```

### Comparing `funasr-0.7.0/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.7.1/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.7.1/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.7.1/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/e2e_vad.py` & `funasr-0.7.1/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.7.1/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.7.1/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.7.1/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/modules/decoder_layer.py` & `funasr-0.7.1/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/modules/encoder_layer.py` & `funasr-0.7.1/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/modules/feedforward.py` & `funasr-0.7.1/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/modules/multihead_att.py` & `funasr-0.7.1/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/models/predictor/cif.py` & `funasr-0.7.1/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/test/test_onnx.py` & `funasr-0.7.1/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/test/test_onnx_punc.py` & `funasr-0.7.1/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.7.1/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/test/test_onnx_vad.py` & `funasr-0.7.1/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/export/utils/torch_function.py` & `funasr-0.7.1/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/fileio/datadir_writer.py` & `funasr-0.7.1/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/fileio/npy_scp.py` & `funasr-0.7.1/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/fileio/rand_gen_dataset.py` & `funasr-0.7.1/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/fileio/read_text.py` & `funasr-0.7.1/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/fileio/sound_scp.py` & `funasr-0.7.1/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/iterators/chunk_iter_factory.py` & `funasr-0.7.1/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/iterators/multiple_iter_factory.py` & `funasr-0.7.1/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/iterators/sequence_iter_factory.py` & `funasr-0.7.1/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/complex_utils.py` & `funasr-0.7.1/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/global_mvn.py` & `funasr-0.7.1/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/label_aggregation.py` & `funasr-0.7.1/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/log_mel.py` & `funasr-0.7.1/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/mask_along_axis.py` & `funasr-0.7.1/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/sinc_conv.py` & `funasr-0.7.1/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/stft.py` & `funasr-0.7.1/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/time_warp.py` & `funasr-0.7.1/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/layers/utterance_mvn.py` & `funasr-0.7.1/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/losses/label_smoothing_loss.py` & `funasr-0.7.1/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/main_funcs/average_nbest_models.py` & `funasr-0.7.1/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.7.1/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/main_funcs/collect_stats.py` & `funasr-0.7.1/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/main_funcs/pack_funcs.py` & `funasr-0.7.1/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/ctc.py` & `funasr-0.7.1/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/data2vec.py` & `funasr-0.7.1/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/decoder/contextual_decoder.py` & `funasr-0.7.1/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/decoder/rnn_decoder.py` & `funasr-0.7.1/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.7.1/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/decoder/sanm_decoder.py` & `funasr-0.7.1/funasr/models/decoder/sanm_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -829,14 +829,18 @@
         use_output_layer: bool = True,
         pos_enc_class=PositionalEncoding,
         normalize_before: bool = True,
         concat_after: bool = False,
         att_layer_num: int = 6,
         kernel_size: int = 21,
         sanm_shfit: int = 0,
+        lora_list: List[str] = None,
+        lora_rank: int = 8,
+        lora_alpha: int = 16,
+        lora_dropout: float = 0.1,
         tf2torch_tensor_name_prefix_torch: str = "decoder",
         tf2torch_tensor_name_prefix_tf: str = "seq2seq/decoder",
     ):
         super().__init__(
             vocab_size=vocab_size,
             encoder_output_size=encoder_output_size,
             dropout_rate=dropout_rate,
@@ -881,15 +885,15 @@
             att_layer_num,
             lambda lnum: DecoderLayerSANM(
                 attention_dim,
                 MultiHeadedAttentionSANMDecoder(
                     attention_dim, self_attention_dropout_rate, kernel_size, sanm_shfit=sanm_shfit
                 ),
                 MultiHeadedAttentionCrossAtt(
-                    attention_heads, attention_dim, src_attention_dropout_rate
+                    attention_heads, attention_dim, src_attention_dropout_rate, lora_list, lora_rank, lora_alpha, lora_dropout
                 ),
                 PositionwiseFeedForwardDecoderSANM(attention_dim, linear_units, dropout_rate),
                 dropout_rate,
                 normalize_before,
                 concat_after,
             ),
         )
```

### Comparing `funasr-0.7.0/funasr/models/decoder/sv_decoder.py` & `funasr-0.7.1/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/decoder/transformer_decoder.py` & `funasr-0.7.1/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr.py` & `funasr-0.7.1/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_bat.py` & `funasr-0.7.1/funasr/models/e2e_asr_bat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_common.py` & `funasr-0.7.1/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.7.1/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_mfcca.py` & `funasr-0.7.1/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_paraformer.py` & `funasr-0.7.1/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_asr_transducer.py` & `funasr-0.7.1/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.7.1/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_diar_sond.py` & `funasr-0.7.1/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_sa_asr.py` & `funasr-0.7.1/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_sv.py` & `funasr-0.7.1/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_tp.py` & `funasr-0.7.1/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_uni_asr.py` & `funasr-0.7.1/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/e2e_vad.py` & `funasr-0.7.1/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/branchformer_encoder.py` & `funasr-0.7.1/funasr/models/encoder/branchformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/conformer_encoder.py` & `funasr-0.7.1/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.7.1/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/e_branchformer_encoder.py` & `funasr-0.7.1/funasr/models/encoder/e_branchformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.7.1/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.7.1/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.7.1/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.7.1/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.7.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.7.1/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/rnn_encoder.py` & `funasr-0.7.1/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/encoder/sanm_encoder.py` & `funasr-0.7.1/funasr/models/encoder/sanm_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,18 @@
         positionwise_layer_type: str = "linear",
         positionwise_conv_kernel_size: int = 1,
         padding_idx: int = -1,
         interctc_layer_idx: List[int] = [],
         interctc_use_conditioning: bool = False,
         kernel_size : int = 11,
         sanm_shfit : int = 0,
+        lora_list: List[str] = None,
+        lora_rank: int = 8,
+        lora_alpha: int = 16,
+        lora_dropout: float = 0.1,
         selfattention_layer_type: str = "sanm",
         tf2torch_tensor_name_prefix_torch: str = "encoder",
         tf2torch_tensor_name_prefix_tf: str = "seq2seq/encoder",
     ):
         super().__init__()
         self._output_size = output_size
 
@@ -225,23 +229,31 @@
             encoder_selfattn_layer_args0 = (
                 attention_heads,
                 input_size,
                 output_size,
                 attention_dropout_rate,
                 kernel_size,
                 sanm_shfit,
+                lora_list,
+                lora_rank,
+                lora_alpha,
+                lora_dropout,
             )
 
             encoder_selfattn_layer_args = (
                 attention_heads,
                 output_size,
                 output_size,
                 attention_dropout_rate,
                 kernel_size,
                 sanm_shfit,
+                lora_list,
+                lora_rank,
+                lora_alpha,
+                lora_dropout,
             )
         self.encoders0 = repeat(
             1,
             lambda lnum: EncoderLayerSANM(
                 input_size,
                 output_size,
                 encoder_selfattn_layer(*encoder_selfattn_layer_args0),
```

### Comparing `funasr-0.7.0/funasr/models/encoder/transformer_encoder.py` & `funasr-0.7.1/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/default.py` & `funasr-0.7.1/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.7.1/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/fused.py` & `funasr-0.7.1/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/s3prl.py` & `funasr-0.7.1/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/wav_frontend.py` & `funasr-0.7.1/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.7.1/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/frontend/windowing.py` & `funasr-0.7.1/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/joint_net/joint_network.py` & `funasr-0.7.1/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/pooling/statistic_pooling.py` & `funasr-0.7.1/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.7.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/predictor/cif.py` & `funasr-0.7.1/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/preencoder/linear.py` & `funasr-0.7.1/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/preencoder/sinc.py` & `funasr-0.7.1/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/seq_rnn_lm.py` & `funasr-0.7.1/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/specaug/specaug.py` & `funasr-0.7.1/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/target_delay_transformer.py` & `funasr-0.7.1/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/transformer_lm.py` & `funasr-0.7.1/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/models/vad_realtime_transformer.py` & `funasr-0.7.1/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/add_sos_eos.py` & `funasr-0.7.1/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/attention.py` & `funasr-0.7.1/funasr/modules/attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy
 import torch
 from torch import nn
 from typing import Optional, Tuple
 
 import torch.nn.functional as F
 from funasr.modules.nets_utils import make_pad_mask
+import funasr.modules.lora.layers as lora
 
 class MultiHeadedAttention(nn.Module):
     """Multi-Head Attention layer.
 
     Args:
         n_head (int): The number of heads.
         n_feat (int): The number of features.
@@ -317,26 +318,37 @@
     Args:
         n_head (int): The number of heads.
         n_feat (int): The number of features.
         dropout_rate (float): Dropout rate.
 
     """
 
-    def __init__(self, n_head, in_feat, n_feat, dropout_rate, kernel_size, sanm_shfit=0):
+    def __init__(self, n_head, in_feat, n_feat, dropout_rate, kernel_size, sanm_shfit=0, lora_list=None, lora_rank=8, lora_alpha=16, lora_dropout=0.1):
         """Construct an MultiHeadedAttention object."""
         super(MultiHeadedAttentionSANM, self).__init__()
         assert n_feat % n_head == 0
         # We assume d_v always equals d_k
         self.d_k = n_feat // n_head
         self.h = n_head
         # self.linear_q = nn.Linear(n_feat, n_feat)
         # self.linear_k = nn.Linear(n_feat, n_feat)
         # self.linear_v = nn.Linear(n_feat, n_feat)
-        self.linear_out = nn.Linear(n_feat, n_feat)
-        self.linear_q_k_v = nn.Linear(in_feat, n_feat * 3)
+        if lora_list is not None:
+            if "o" in lora_list:
+                self.linear_out = lora.Linear(n_feat, n_feat, r=lora_rank, lora_alpha=lora_alpha, lora_dropout=lora_dropout)
+            else:
+                self.linear_out = nn.Linear(n_feat, n_feat)
+            lora_qkv_list = ["q" in lora_list, "k" in lora_list, "v" in lora_list]
+            if lora_qkv_list == [False, False, False]:
+                self.linear_q_k_v = nn.Linear(in_feat, n_feat * 3)
+            else:
+                self.linear_q_k_v = lora.MergedLinear(in_feat, n_feat * 3, r=lora_rank, lora_alpha=lora_alpha, lora_dropout=lora_dropout, enable_lora=lora_qkv_list)
+        else:
+            self.linear_out = nn.Linear(n_feat, n_feat)
+            self.linear_q_k_v = nn.Linear(in_feat, n_feat * 3)
         self.attn = None
         self.dropout = nn.Dropout(p=dropout_rate)
 
         self.fsmn_block = nn.Conv1d(n_feat, n_feat, kernel_size, stride=1, padding=0, groups=n_feat, bias=False)
         # padding
         left_padding = (kernel_size - 1) // 2
         if sanm_shfit > 0:
@@ -539,26 +551,40 @@
     Args:
         n_head (int): The number of heads.
         n_feat (int): The number of features.
         dropout_rate (float): Dropout rate.
 
     """
 
-    def __init__(self, n_head, n_feat, dropout_rate, encoder_output_size=None):
+    def __init__(self, n_head, n_feat, dropout_rate, lora_list=None, lora_rank=8, lora_alpha=16, lora_dropout=0.1, encoder_output_size=None):
         """Construct an MultiHeadedAttention object."""
         super(MultiHeadedAttentionCrossAtt, self).__init__()
         assert n_feat % n_head == 0
         # We assume d_v always equals d_k
         self.d_k = n_feat // n_head
         self.h = n_head
-        self.linear_q = nn.Linear(n_feat, n_feat)
-        # self.linear_k = nn.Linear(n_feat, n_feat)
-        # self.linear_v = nn.Linear(n_feat, n_feat)
-        self.linear_k_v = nn.Linear(n_feat if encoder_output_size is None else encoder_output_size, n_feat*2)
-        self.linear_out = nn.Linear(n_feat, n_feat)
+        if lora_list is not None:
+            if "q" in lora_list:
+                self.linear_q = lora.Linear(n_feat, n_feat, r=lora_rank, lora_alpha=lora_alpha, lora_dropout=lora_dropout)
+            else:
+                self.linear_q = nn.Linear(n_feat, n_feat)
+            lora_kv_list = ["k" in lora_list, "v" in lora_list]
+            if lora_kv_list == [False, False]:
+                self.linear_k_v = nn.Linear(n_feat if encoder_output_size is None else encoder_output_size, n_feat*2)
+            else:
+                self.linear_k_v = lora.MergedLinear(n_feat if encoder_output_size is None else encoder_output_size, n_feat * 2, 
+                                      r=lora_rank, lora_alpha=lora_alpha, lora_dropout=lora_dropout, enable_lora=lora_kv_list)
+            if "o" in lora_list:
+                self.linear_out = lora.Linear(n_feat, n_feat, r=lora_rank, lora_alpha=lora_alpha, lora_dropout=lora_dropout)
+            else:
+                self.linear_out = nn.Linear(n_feat, n_feat)
+        else:
+            self.linear_q = nn.Linear(n_feat, n_feat)
+            self.linear_k_v = nn.Linear(n_feat if encoder_output_size is None else encoder_output_size, n_feat*2)
+            self.linear_out = nn.Linear(n_feat, n_feat)
         self.attn = None
         self.dropout = nn.Dropout(p=dropout_rate)
 
     def forward_qkv(self, x, memory):
         """Transform query, key and value.
 
         Args:
```

### Comparing `funasr-0.7.0/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.7.1/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.7.1/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/beam_search/beam_search.py` & `funasr-0.7.1/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.7.1/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.7.1/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/cgmlp.py` & `funasr-0.7.1/funasr/modules/cgmlp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/data_utils.py` & `funasr-0.7.1/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/ema_module.py` & `funasr-0.7.1/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.7.1/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/quant_noise.py` & `funasr-0.7.1/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/utils.py` & `funasr-0.7.1/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.7.1/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/dynamic_conv.py` & `funasr-0.7.1/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/dynamic_conv2d.py` & `funasr-0.7.1/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/e2e_asr_common.py` & `funasr-0.7.1/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/eend_ola/encoder.py` & `funasr-0.7.1/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.7.1/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/eend_ola/utils/losses.py` & `funasr-0.7.1/funasr/modules/eend_ola/utils/losses.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/eend_ola/utils/power.py` & `funasr-0.7.1/funasr/modules/eend_ola/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/eend_ola/utils/report.py` & `funasr-0.7.1/funasr/modules/eend_ola/utils/report.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/embedding.py` & `funasr-0.7.1/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/fastformer.py` & `funasr-0.7.1/funasr/modules/fastformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/beamformer.py` & `funasr-0.7.1/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.7.1/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.7.1/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/feature_transform.py` & `funasr-0.7.1/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/frontend.py` & `funasr-0.7.1/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/frontends/mask_estimator.py` & `funasr-0.7.1/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/layer_norm.py` & `funasr-0.7.1/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/lightconv.py` & `funasr-0.7.1/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/lightconv2d.py` & `funasr-0.7.1/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/mask.py` & `funasr-0.7.1/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/multi_layer_conv.py` & `funasr-0.7.1/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/nets_utils.py` & `funasr-0.7.1/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/positionwise_feed_forward.py` & `funasr-0.7.1/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/repeat.py` & `funasr-0.7.1/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/rnn/argument.py` & `funasr-0.7.1/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/rnn/attentions.py` & `funasr-0.7.1/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/rnn/decoders.py` & `funasr-0.7.1/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/rnn/encoders.py` & `funasr-0.7.1/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/scorers/ctc.py` & `funasr-0.7.1/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.7.1/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/scorers/length_bonus.py` & `funasr-0.7.1/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/scorers/scorer_interface.py` & `funasr-0.7.1/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.7.1/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.7.1/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/streaming_utils/utils.py` & `funasr-0.7.1/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/subsampling.py` & `funasr-0.7.1/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/modules/subsampling_without_posenc.py` & `funasr-0.7.1/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/optimizers/fairseq_adam.py` & `funasr-0.7.1/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/optimizers/sgd.py` & `funasr-0.7.1/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/demo.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/libtorch/setup.py` & `funasr-0.7.1/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.7.1/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/build_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/folded_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/length_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.7.1/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/schedulers/abs_scheduler.py` & `funasr-0.7.1/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/schedulers/noam_lr.py` & `funasr-0.7.1/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.7.1/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/schedulers/warmup_lr.py` & `funasr-0.7.1/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/abs_task.py` & `funasr-0.7.1/funasr/tasks/abs_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 from funasr.utils.types import int_or_none
 from funasr.utils.types import str2bool
 from funasr.utils.types import str2triple_str
 from funasr.utils.types import str_or_int
 from funasr.utils.types import str_or_none
 from funasr.utils.wav_utils import calc_shape, generate_data_list, filter_wav_text
 from funasr.utils.yaml_no_alias_safe_dump import yaml_no_alias_safe_dump
+from funasr.modules.lora.utils import mark_only_lora_as_trainable
 
 try:
     import wandb
 except Exception:
     wandb = None
 
 if LooseVersion(torch.__version__) >= LooseVersion("1.5.0"):
@@ -948,14 +949,26 @@
             help="The bucket name for oss.",
         )
         group.add_argument(
             "--oss_bucket",
             default=None,
             help="oss bucket.",
         )
+        group.add_argument(
+            "--enable_lora",
+            type=str2bool,
+            default=False,
+            help="Apply lora for finetuning.",
+        )
+        group.add_argument(
+            "--lora_bias",
+            type=str,
+            default="none",
+            help="lora bias.",
+        )
 
         cls.trainer.add_arguments(parser)
         cls.add_task_arguments(parser)
 
         return parser
 
     @classmethod
@@ -1242,14 +1255,16 @@
             raise RuntimeError(
                 f"model must inherit {FunASRModel.__name__}, but got {type(model)}"
             )
         model = model.to(
             dtype=getattr(torch, args.train_dtype),
             device="cuda" if args.ngpu > 0 else "cpu",
         )
+        if args.enable_lora:
+            mark_only_lora_as_trainable(model, args.lora_bias)
         for t in args.freeze_param:
             for k, p in model.named_parameters():
                 if k.startswith(t + ".") or k == t:
                     logging.info(f"Setting {k}.requires_grad = False")
                     p.requires_grad = False
 
         # 3. Build optimizer
```

### Comparing `funasr-0.7.0/funasr/tasks/asr.py` & `funasr-0.7.1/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/data2vec.py` & `funasr-0.7.1/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/diar.py` & `funasr-0.7.1/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/lm.py` & `funasr-0.7.1/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/punctuation.py` & `funasr-0.7.1/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/sa_asr.py` & `funasr-0.7.1/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/sv.py` & `funasr-0.7.1/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/tasks/vad.py` & `funasr-0.7.1/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/build_tokenizer.py` & `funasr-0.7.1/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/char_tokenizer.py` & `funasr-0.7.1/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/cleaner.py` & `funasr-0.7.1/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/korean_cleaner.py` & `funasr-0.7.1/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/phoneme_tokenizer.py` & `funasr-0.7.1/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.7.1/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/token_id_converter.py` & `funasr-0.7.1/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/text/word_tokenizer.py` & `funasr-0.7.1/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.7.1/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/device_funcs.py` & `funasr-0.7.1/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/forward_adaptor.py` & `funasr-0.7.1/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/initialize.py` & `funasr-0.7.1/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.7.1/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/model_summary.py` & `funasr-0.7.1/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/torch_utils/recursive_op.py` & `funasr-0.7.1/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/train/abs_model.py` & `funasr-0.7.1/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/train/class_choices.py` & `funasr-0.7.1/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/train/distributed_utils.py` & `funasr-0.7.1/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/train/reporter.py` & `funasr-0.7.1/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/train/trainer.py` & `funasr-0.7.1/funasr/train/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
                             "optimizers": [o.state_dict() for o in optimizers],
                             "schedulers": [
                                 s.state_dict() if s is not None else None
                                 for s in schedulers
                             ],
                             "scaler": scaler.state_dict() if scaler is not None else None,
                             "ema_model": model.encoder.ema.model.state_dict()
-                            if hasattr(model.encoder, "ema") and model.encoder.ema is not None else None,
+                            if hasattr(model, "encoder") and hasattr(model.encoder, "ema") and model.encoder.ema is not None else None,
                         },
                         buffer,
                     )
                     trainer_options.oss_bucket.put_object(os.path.join(trainer_options.output_dir, "checkpoint.pb"), buffer.getvalue())
                 else:
                     torch.save(
                         {
```

### Comparing `funasr-0.7.0/funasr/utils/asr_env_checking.py` & `funasr-0.7.1/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/asr_utils.py` & `funasr-0.7.1/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/cli_utils.py` & `funasr-0.7.1/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/compute_eer.py` & `funasr-0.7.1/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/compute_min_dcf.py` & `funasr-0.7.1/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/compute_wer.py` & `funasr-0.7.1/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/config_argparse.py` & `funasr-0.7.1/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/get_default_kwargs.py` & `funasr-0.7.1/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/griffin_lim.py` & `funasr-0.7.1/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/job_runner.py` & `funasr-0.7.1/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/misc.py` & `funasr-0.7.1/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/modelscope_param.py` & `funasr-0.7.1/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/modelscope_utils.py` & `funasr-0.7.1/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/nested_dict_action.py` & `funasr-0.7.1/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/postprocess_utils.py` & `funasr-0.7.1/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/prepare_data.py` & `funasr-0.7.1/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/runtime_sdk_download_tool.py` & `funasr-0.7.1/funasr/utils/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/sized_dict.py` & `funasr-0.7.1/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/timestamp_tools.py` & `funasr-0.7.1/funasr/utils/timestamp_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from itertools import zip_longest
-
 import torch
-import copy
 import codecs
 import logging
-import edit_distance
 import argparse
-import pdb
 import numpy as np
-from typing import Any, List, Tuple, Union
+import edit_distance
+from itertools import zip_longest
 
 
 def ts_prediction_lfr6_standard(us_alphas, 
                        us_peaks, 
                        char_list, 
                        vad_offset=0.0, 
                        force_time_shift=-1.5,
@@ -32,15 +28,22 @@
         char_list = char_list[:-1]
     timestamp_list = []
     new_char_list = []
     # for bicif model trained with large data, cif2 actually fires when a character starts
     # so treat the frames between two peaks as the duration of the former token
     fire_place = torch.where(peaks>1.0-1e-4)[0].cpu().numpy() + force_time_shift  # total offset
     num_peak = len(fire_place)
-    assert num_peak == len(char_list) + 1 # number of peaks is supposed to be number of tokens + 1
+    if num_peak != len(char_list) + 1:
+        logging.warning("length mismatch, result might be incorrect.")
+        logging.warning("num_peaks: {}, num_chars+1: {}, which is supposed to be same.".format(num_peak, len(char_list)+1))
+    if num_peak > len(char_list) + 1:
+        fire_place = fire_place[:len(char_list) - 1]
+    elif num_peak < len(char_list) + 1:
+        char_list = char_list[:num_peak + 1]
+    # assert num_peak == len(char_list) + 1 # number of peaks is supposed to be number of tokens + 1
     # begin silence
     if fire_place[0] > START_END_THRESHOLD:
         # char_list.insert(0, '<sil>')
         timestamp_list.append([0.0, fire_place[0]*TIME_RATE])
         new_char_list.append('<sil>')
     # tokens timestamp
     for i in range(len(fire_place)-1):
```

### Comparing `funasr-0.7.0/funasr/utils/types.py` & `funasr-0.7.1/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/vad_utils.py` & `funasr-0.7.1/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr/utils/wav_utils.py` & `funasr-0.7.1/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/funasr.egg-info/SOURCES.txt` & `funasr-0.7.1/funasr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,26 +71,34 @@
 funasr/datasets/small_datasets/__init__.py
 funasr/datasets/small_datasets/collate_fn.py
 funasr/datasets/small_datasets/dataset.py
 funasr/datasets/small_datasets/length_batch_sampler.py
 funasr/datasets/small_datasets/preprocessor.py
 funasr/datasets/small_datasets/sequence_iter_factory.py
 funasr/export/__init__.py
+funasr/export/export_conformer.py
 funasr/export/export_model.py
 funasr/export/models/CT_Transformer.py
 funasr/export/models/__init__.py
+funasr/export/models/e2e_asr_conformer.py
 funasr/export/models/e2e_asr_paraformer.py
 funasr/export/models/e2e_vad.py
 funasr/export/models/decoder/__init__.py
 funasr/export/models/decoder/sanm_decoder.py
 funasr/export/models/decoder/transformer_decoder.py
+funasr/export/models/decoder/xformer_decoder.py
 funasr/export/models/encoder/__init__.py
 funasr/export/models/encoder/conformer_encoder.py
 funasr/export/models/encoder/fsmn_encoder.py
 funasr/export/models/encoder/sanm_encoder.py
+funasr/export/models/language_models/__init__.py
+funasr/export/models/language_models/embed.py
+funasr/export/models/language_models/seq_rnn.py
+funasr/export/models/language_models/subsampling.py
+funasr/export/models/language_models/transformer.py
 funasr/export/models/modules/__init__.py
 funasr/export/models/modules/decoder_layer.py
 funasr/export/models/modules/encoder_layer.py
 funasr/export/models/modules/feedforward.py
 funasr/export/models/modules/multihead_att.py
 funasr/export/models/predictor/__init__.py
 funasr/export/models/predictor/cif.py
@@ -221,14 +229,15 @@
 funasr/modules/mask.py
 funasr/modules/multi_layer_conv.py
 funasr/modules/nets_utils.py
 funasr/modules/positionwise_feed_forward.py
 funasr/modules/repeat.py
 funasr/modules/subsampling.py
 funasr/modules/subsampling_without_posenc.py
+funasr/modules/vgg2l.py
 funasr/modules/beam_search/__init__.py
 funasr/modules/beam_search/batch_beam_search.py
 funasr/modules/beam_search/batch_beam_search_online_sim.py
 funasr/modules/beam_search/beam_search.py
 funasr/modules/beam_search/beam_search_sa_asr.py
 funasr/modules/beam_search/beam_search_transducer.py
 funasr/modules/data2vec/__init__.py
@@ -249,14 +258,17 @@
 funasr/modules/frontends/__init__.py
 funasr/modules/frontends/beamformer.py
 funasr/modules/frontends/dnn_beamformer.py
 funasr/modules/frontends/dnn_wpe.py
 funasr/modules/frontends/feature_transform.py
 funasr/modules/frontends/frontend.py
 funasr/modules/frontends/mask_estimator.py
+funasr/modules/lora/__init__.py
+funasr/modules/lora/layers.py
+funasr/modules/lora/utils.py
 funasr/modules/rnn/__init__.py
 funasr/modules/rnn/argument.py
 funasr/modules/rnn/attentions.py
 funasr/modules/rnn/decoders.py
 funasr/modules/rnn/encoders.py
 funasr/modules/scorers/__init__.py
 funasr/modules/scorers/ctc.py
```

### Comparing `funasr-0.7.0/funasr.egg-info/requires.txt` & `funasr-0.7.1/funasr.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 setuptools>=38.5.1
 humanfriendly
 scipy>=1.4.1
 librosa
 jamo
 PyYAML>=5.1.2
-soundfile>=0.10.2
+soundfile>=0.12.1
 h5py>=2.10.0
 kaldiio>=2.17.0
 torch_complex
 nltk>=3.4.5
 sentencepiece
+jieba
 pypinyin>=0.44.0
 espnet_tts_frontend
 pytorch_wpe
 editdistance>=0.5.2
 tensorboard
 g2p
 oss2
```

### Comparing `funasr-0.7.0/setup.py` & `funasr-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,22 @@
     "install": [
         "setuptools>=38.5.1",
         "humanfriendly",
         "scipy>=1.4.1",
         "librosa",
         "jamo",  # For kss
         "PyYAML>=5.1.2",
-        "soundfile>=0.10.2",
+        "soundfile>=0.12.1",
         "h5py>=2.10.0",
         "kaldiio>=2.17.0",
         "torch_complex",
         "nltk>=3.4.5",
         # ASR
         "sentencepiece",
+        "jieba",
         # TTS
         "pypinyin>=0.44.0",
         "espnet_tts_frontend",
         # ENH
         "pytorch_wpe",
         "editdistance>=0.5.2",
         "tensorboard",
@@ -118,8 +119,8 @@
         "Programming Language :: Python :: 3.9",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-)
+)
```

### Comparing `funasr-0.7.0/tests/test_asr_inference_pipeline.py` & `funasr-0.7.1/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.7.1/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_lm_pipeline.py` & `funasr-0.7.1/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_punctuation_pipeline.py` & `funasr-0.7.1/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_sv_inference_pipeline.py` & `funasr-0.7.1/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_tp_pipeline.py` & `funasr-0.7.1/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.7.0/tests/test_vad_inference_pipeline.py` & `funasr-0.7.1/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

