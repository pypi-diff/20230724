# Comparing `tmp/pybaseutils-0.8.5.tar.gz` & `tmp/pybaseutils-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.8.5.tar", last modified: Mon Jun 26 02:20:57 2023, max compression
+gzip compressed data, was "pybaseutils-0.8.6.tar", last modified: Mon Jul 24 08:49:16 2023, max compression
```

## Comparing `pybaseutils-0.8.5.tar` & `pybaseutils-0.8.6.tar`

### file list

```diff
@@ -1,138 +1,151 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.368254 pybaseutils-0.8.5/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.5/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-26 02:20:57.368025 pybaseutils-0.8.5/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.5/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.316336 pybaseutils-0.8.5/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-06-26 02:20:49.000000 pybaseutils-0.8.5/pybaseutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/base64_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.321150 pybaseutils-0.8.5/pybaseutils/base_audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.5/pybaseutils/base_audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4870 2023-06-20 02:36:58.000000 pybaseutils-0.8.5/pybaseutils/base_audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1841 2023-06-20 03:14:56.000000 pybaseutils-0.8.5/pybaseutils/base_audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.323783 pybaseutils-0.8.5/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.5/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.5/pybaseutils/config_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.326985 pybaseutils-0.8.5/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.5/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.5/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-0.8.5/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9734 2023-06-21 02:44:02.000000 pybaseutils-0.8.5/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.330403 pybaseutils-0.8.5/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32585 2023-06-19 09:57:39.000000 pybaseutils-0.8.5/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.331143 pybaseutils-0.8.5/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    97190 2023-06-14 03:03:27.000000 pybaseutils-0.8.5/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.5/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.335382 pybaseutils-0.8.5/pybaseutils/maker/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/maker/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/maker/maker_voc.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.339211 pybaseutils-0.8.5/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.5/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.340948 pybaseutils-0.8.5/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.5/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.5/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.5/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.5/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.342152 pybaseutils-0.8.5/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.5/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.5/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.5/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.319202 pybaseutils-0.8.5/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3558 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.5/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-06-26 02:20:57.000000 pybaseutils-0.8.5/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-06-26 02:20:57.368324 pybaseutils-0.8.5/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.5/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.357799 pybaseutils-0.8.5/test_py/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.5/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.363364 pybaseutils-0.8.5/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.5/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.5/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.5/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.5/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.5/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.5/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.5/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.5/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.5/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1259 2023-06-20 02:37:41.000000 pybaseutils-0.8.5/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1263 2023-06-21 00:19:31.000000 pybaseutils-0.8.5/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.5/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.5/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4664 2023-06-01 07:22:44.000000 pybaseutils-0.8.5/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.5/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.5/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.5/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2943 2023-06-15 00:54:20.000000 pybaseutils-0.8.5/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.5/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.5/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.5/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.5/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      834 2023-06-21 01:39:59.000000 pybaseutils-0.8.5/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2888 2023-06-25 08:37:27.000000 pybaseutils-0.8.5/test_py/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.5/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2440 2023-06-15 00:55:49.000000 pybaseutils-0.8.5/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.5/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.364264 pybaseutils-0.8.5/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.5/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.5/test_py/detector/detect_face_person.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.365608 pybaseutils-0.8.5/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.5/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.5/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.5/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-06-26 02:20:57.367507 pybaseutils-0.8.5/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.5/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.5/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.5/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.5/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.5/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.061786 pybaseutils-0.8.6/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.6/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-24 08:49:16.061470 pybaseutils-0.8.6/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.6/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.002518 pybaseutils-0.8.6/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2023-07-24 08:49:08.000000 pybaseutils-0.8.6/pybaseutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/base64_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.006375 pybaseutils-0.8.6/pybaseutils/base_audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.6/pybaseutils/base_audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4870 2023-06-20 02:36:58.000000 pybaseutils-0.8.6/pybaseutils/base_audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1841 2023-06-20 03:14:56.000000 pybaseutils-0.8.6/pybaseutils/base_audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.008854 pybaseutils-0.8.6/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.6/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.6/pybaseutils/config_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.012042 pybaseutils-0.8.6/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.6/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.6/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-0.8.6/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9770 2023-07-19 10:29:03.000000 pybaseutils-0.8.6/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.015579 pybaseutils-0.8.6/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12273 2023-06-30 00:42:01.000000 pybaseutils-0.8.6/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19469 2023-06-30 00:49:35.000000 pybaseutils-0.8.6/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-0.8.6/pybaseutils/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    32622 2023-07-24 08:48:54.000000 pybaseutils-0.8.6/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.016325 pybaseutils-0.8.6/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    99197 2023-07-19 08:43:17.000000 pybaseutils-0.8.6/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.6/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.021367 pybaseutils-0.8.6/pybaseutils/maker/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/maker/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5158 2023-07-14 03:43:40.000000 pybaseutils-0.8.6/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-0.8.6/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/maker/maker_voc.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.024928 pybaseutils-0.8.6/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.6/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.026399 pybaseutils-0.8.6/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.6/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.6/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.027383 pybaseutils-0.8.6/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-0.8.6/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-0.8.6/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.6/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.6/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.028346 pybaseutils-0.8.6/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.6/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.6/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.6/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.004733 pybaseutils-0.8.6/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3897 2023-07-24 08:49:15.000000 pybaseutils-0.8.6/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3912 2023-07-24 08:49:15.000000 pybaseutils-0.8.6/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2023-07-24 08:49:15.000000 pybaseutils-0.8.6/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.6/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2023-07-24 08:49:15.000000 pybaseutils-0.8.6/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2023-07-24 08:49:16.061882 pybaseutils-0.8.6/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-0.8.6/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.045581 pybaseutils-0.8.6/test_py/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      610 2023-07-18 02:51:24.000000 pybaseutils-0.8.6/test_py/apm_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.6/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.054393 pybaseutils-0.8.6/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.6/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-0.8.6/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.6/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.6/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.6/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.6/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-0.8.6/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.6/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      982 2023-07-20 09:35:42.000000 pybaseutils-0.8.6/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-0.8.6/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2320 2023-07-17 02:10:53.000000 pybaseutils-0.8.6/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.6/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.6/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1259 2023-06-20 02:37:41.000000 pybaseutils-0.8.6/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      519 2023-07-13 03:25:56.000000 pybaseutils-0.8.6/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1291 2023-06-29 02:15:47.000000 pybaseutils-0.8.6/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.6/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-0.8.6/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5086 2023-06-30 02:28:09.000000 pybaseutils-0.8.6/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-0.8.6/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-0.8.6/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.6/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4589 2023-07-17 09:31:14.000000 pybaseutils-0.8.6/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1690 2023-07-24 05:47:50.000000 pybaseutils-0.8.6/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      827 2023-06-30 00:39:21.000000 pybaseutils-0.8.6/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.6/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.6/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.6/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      803 2023-07-19 10:31:29.000000 pybaseutils-0.8.6/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2948 2023-07-24 08:43:20.000000 pybaseutils-0.8.6/test_py/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3593 2023-06-30 00:54:49.000000 pybaseutils-0.8.6/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2919 2023-07-17 08:48:13.000000 pybaseutils-0.8.6/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.6/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.056567 pybaseutils-0.8.6/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.6/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1863 2023-07-17 02:45:08.000000 pybaseutils-0.8.6/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-07-11 07:21:57.000000 pybaseutils-0.8.6/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6121 2023-07-18 07:56:37.000000 pybaseutils-0.8.6/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.058255 pybaseutils-0.8.6/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.6/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.6/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.6/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2023-07-24 08:49:16.060732 pybaseutils-0.8.6/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.6/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.6/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.6/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.6/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.6/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.6/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.6/test_py/performance.py
```

### Comparing `pybaseutils-0.8.5/LICENCE` & `pybaseutils-0.8.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/PKG-INFO` & `pybaseutils-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.5
+Version: 0.8.6
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.5/README.md` & `pybaseutils-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/base64_utils.py` & `pybaseutils-0.8.6/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/base_audio/audio_utils.py` & `pybaseutils-0.8.6/pybaseutils/base_audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/base_audio/pyaudio_utils.py` & `pybaseutils-0.8.6/pybaseutils/base_audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/batch_utils.py` & `pybaseutils-0.8.6/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.6/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.6/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.6/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/color_utils.py` & `pybaseutils-0.8.6/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/config_utils.py` & `pybaseutils-0.8.6/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/coords_utils.py` & `pybaseutils-0.8.6/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.6/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cvutils/monitor.py` & `pybaseutils-0.8.6/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.6/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.6/pybaseutils/cvutils/video_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     :param vis: 是否可视化显示
     :return:
     """
     name = os.path.basename(video_file).split(".")[0]
     if not out_dir:  out_dir = os.path.join(os.path.dirname(video_file), name)
     video_cap = get_video_capture(video_file)
     width, height, num_frames, fps = get_video_info(video_cap)
+    if not interval: interval = fps
     if not os.path.exists(out_dir): os.makedirs(out_dir)
     count = 0
     while True:
         if count % interval == 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
```

### Comparing `pybaseutils-0.8.5/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.6/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.6/pybaseutils/dataloader/parser_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,21 +253,24 @@
 
     def read_image(self, image_file: str, use_rgb=True):
         """
         :param image_file:
         :param use_rgb:
         :return:
         """
-        image = cv2.imread(image_file, cv2.IMREAD_COLOR)
-        if len(image.shape) == 2:
-            image = cv2.cvtColor(image, cv2.COLOR_GRAY2BGR)
-        elif image.shape[2] == 4:
-            image = image[:, :, 0:3]
-        if use_rgb:
-            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        try:
+            image = cv2.imread(image_file, cv2.IMREAD_COLOR)
+            if len(image.shape) == 2:
+                image = cv2.cvtColor(image, cv2.COLOR_GRAY2BGR)
+            elif image.shape[2] == 4:
+                image = image[:, :, 0:3]
+            if use_rgb:
+                image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        except Exception as e:
+            raise Exception("empty image:{}".format(image_file))
         return image
 
     @staticmethod
     def load_annotations(ann_file: str):
         with open(ann_file, "r") as f: annotation = json.load(f)
         annos = annotation["shapes"]
         return annos
```

### Comparing `pybaseutils-0.8.5/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.6/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.6/pybaseutils/dataloader/parser_voc.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
                           check=check)
         datasets.append(data)
     datasets = ConcatDataset(datasets, shuffle=shuffle)
     return datasets
 
 
 def show_target_image(image, bboxes, labels, normal=False, transpose=False, class_name=None, use_rgb=True,
-                      thickness=-1, fontScale=-1.0):
+                      thickness=2, fontScale=1.0):
     """
     :param image:
     :param targets_t:
                 bboxes = targets[idx][:, :4].data
                 keypoints = targets[idx][:, 4:14].data
                 labels = targets[idx][:, -1].data
     :return:
@@ -473,15 +473,15 @@
     landms_scale = np.asarray([w, h] * 5)
     bboxes_scale = np.asarray([w, h] * 2)
     if normal:
         bboxes = bboxes * bboxes_scale
     # image = image_processing.untranspose(image)
     # image = image_processing.convert_color_space(image, colorSpace="RGB")
     image = image_utils.draw_image_bboxes_labels(image, bboxes, labels, class_name=class_name,
-                                                 thickness=thickness, fontScale=fontScale, drawType="custom")
+                                                 thickness=thickness, fontScale=fontScale, drawType="chinese")
     image_utils.cv_show_image("image", image, delay=0, use_rgb=use_rgb)
     print("===" * 10)
     return image
 
 
 if __name__ == "__main__":
     # from models.transforms import data_transforms
```

### Comparing `pybaseutils-0.8.5/pybaseutils/file_utils.py` & `pybaseutils-0.8.6/pybaseutils/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,14 +577,15 @@
     :param dir1:
     :param filename:
     :return:
     """
     out_path = parent_dir
     if dir1:
         out_path = os.path.join(parent_dir, dir1)
+    if not out_path: return out_path
     if not os.path.exists(out_path):
         os.makedirs(out_path)
     if filename:
         out_path = os.path.join(out_path, filename)
     return out_path
```

### Comparing `pybaseutils-0.8.5/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.6/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/font_utils.py` & `pybaseutils-0.8.6/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.6/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.6/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/image_utils.py` & `pybaseutils-0.8.6/pybaseutils/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1073,15 +1073,15 @@
     :param rgb_image:
     :param bboxes:  [[x1,y1,x2,y2],[x1,y1,x2,y2]]
     :param labels:
     :return:
     """
     if isinstance(labels, np.ndarray): labels = labels.astype(np.int32).reshape(-1).tolist()
     for label, box in zip(labels, bboxes):
-        color_ = color if color else color_map[int(label) + 1]
+        color_ = color if color else color_table[int(label) + 1]
         box = [int(b) for b in box]
         if class_name: label = class_name[int(label)]
         rgb_image = custom_bbox_line(rgb_image, box, color_, str(label), thickness=thickness,
                                      fontScale=fontScale, drawType=drawType)
     return rgb_image
 
 
@@ -1130,15 +1130,15 @@
     :param drawType:
     :return:
     """
     thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
     labels = labels if isinstance(labels, list) else np.asarray(labels, dtype=np.int32).reshape(-1)
     probs = np.asarray(probs).reshape(-1)
     for label, box, prob in zip(labels, boxes, probs):
-        color = color_map[1] if isinstance(label, str) else color_map[int(label) + 1]
+        color = color_table[1] if isinstance(label, str) else color_table[int(label) + 1]
         box = [int(b) for b in box]
         if class_name:
             label = class_name[int(label)]
         boxes_name = "{}:{:3.2f}".format(label, prob)
         custom_bbox_line(image, box, color, boxes_name, thickness=thickness, fontScale=fontScale, drawType=drawType)
     return image
 
@@ -1184,49 +1184,14 @@
                 image = draw_image_bboxes_text(image, [dt_boxes[i]], [dt_label[i]], color=(255, 0, 0))
     else:
         image = draw_image_bboxes_text(image, gt_boxes, gt_label, color=(0, 255, 0))
         image = draw_image_bboxes_text(image, dt_boxes, dt_label, color=(255, 0, 0))
     return image
 
 
-def custom_bbox_line(image, bbox, color, name, thickness=2, fontScale=0.8, drawType="custom", top=True):
-    """
-    :param image:
-    :param bbox:
-    :param color:
-    :param name:
-    :param drawType:
-    :param top:
-    :return:
-    """
-    thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
-    if not name: drawType = "simple"
-    if drawType == "chinese":
-        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
-        cv2_putText(image, str(name), (bbox[0], bbox[1]), color=color, fontScale=fontScale, thickness=thickness)
-    elif drawType == "simple":
-        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness, 8, 0)
-        cv2.putText(image, str(name), (bbox[0], bbox[1]), cv2.FONT_HERSHEY_SIMPLEX, fontScale, color, thickness)
-    elif drawType == "custom":
-        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
-        text_size, baseline = cv2.getTextSize(str(name), cv2.FONT_HERSHEY_SIMPLEX, fontScale, thickness)
-        if top:
-            text_loc = (bbox[0], bbox[1] - text_size[1])
-        else:
-            # text_loc = (bbox[0], bbox[1])
-            text_loc = (bbox[0], bbox[3])
-            # text_loc = (bbox[2], bbox[1] + text_size[1])
-        cv2.rectangle(image, (text_loc[0] - 2 // 2, text_loc[1] - 2 - baseline),
-                      (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color, -1)
-        # draw score value
-        cv2.putText(image, str(name), (text_loc[0], text_loc[1] + baseline), cv2.FONT_HERSHEY_SIMPLEX, fontScale,
-                    (255, 255, 255), thickness)
-    return image
-
-
 def draw_landmark(image, landmarks, radius=2, fontScale=1.0, color=(0, 0, 255), vis_id=False):
     """
     :param image:
     :param landmarks:
     :param radius:
     :param thickness:
     :param fontScale:
@@ -1304,29 +1269,65 @@
     :param image:
     :param point:
     :param text:
     :param drawType: custom or simple
     :return:
     """
     thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
-    text_thickness = 1
     fontFace = cv2.FONT_HERSHEY_SIMPLEX
     # fontFace=cv2.FONT_HERSHEY_SIMPLEX
     if drawType == "custom" or drawType == "en":
         text_size, baseline = cv2.getTextSize(str(text), fontFace, fontScale, thickness)
         text_loc = (point[0], point[1] + text_size[1])
         cv2.rectangle(image, (text_loc[0] - 2 // 2, text_loc[1] - 2 - baseline),
-                      (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color=color, thickness=thickness)
+                      (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color=color, thickness=-1)
         # draw score value
-        cv2.putText(image, str(text), (text_loc[0], text_loc[1] + baseline), fontFace, fontScale,
-                    (255, 255, 255), text_thickness, 2)
+        cv2.putText(image, str(text), (text_loc[0], text_loc[1] + baseline), fontFace, fontScale, (255, 255, 255),
+                    thickness, 2)
     elif drawType == "simple":
-        cv2.putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
+        cv2.putText(image, str(text),  (point[0], point[1]), fontFace, fontScale, color=color, thickness=thickness)
     if drawType == "chinese" or drawType == "ch":
-        cv2_putText(image, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
+        cv2_putText(image, str(text),  (point[0], point[1]), fontFace, fontScale, color=color, thickness=thickness)
+    return image
+
+
+def custom_bbox_line(image, bbox, color, name, thickness=2, fontScale=0.8, drawType="custom", top=True):
+    """
+    :param image:
+    :param bbox:
+    :param color:
+    :param name:
+    :param drawType:
+    :param top:
+    :return:
+    """
+    thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
+    if not name: drawType = "simple"
+    if drawType == "chinese":
+        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
+        cv2_putText(image, str(name), (bbox[0], bbox[1]), color=color, fontScale=fontScale, thickness=thickness)
+    elif drawType == "simple":
+        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness, 8, 0)
+        cv2.putText(image, str(name), (bbox[0], bbox[1]), cv2.FONT_HERSHEY_SIMPLEX, fontScale, color, thickness)
+    elif drawType == "custom":
+        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
+        text_size, baseline = cv2.getTextSize(str(name), cv2.FONT_HERSHEY_SIMPLEX, fontScale, thickness)
+        if top:
+            text_loc = (bbox[0], bbox[1] + text_size[1])  # 在左上角下方绘制文字
+            # text_loc = (bbox[0], bbox[1] - baseline // 2)# 在左上角上方绘制文字
+        else:
+            text_loc = (bbox[0], bbox[3])
+        bg1 = (text_loc[0], text_loc[1] - text_size[1])
+        bg2 = (text_loc[0] + text_size[0], text_loc[1] + baseline // 2)  # 底纹等于字体的宽度
+        # bg2 = (max(bbox[2], text_loc[0] + text_size[0]), text_loc[1] + baseline // 2) # 底纹等于box的宽度
+        cv2.rectangle(image, bg1, bg2, color, thickness)  # 先绘制框，再填充
+        cv2.rectangle(image, bg1, bg2, color, -1)
+        # draw score value
+        cv2.putText(image, str(name), (text_loc[0], text_loc[1]), cv2.FONT_HERSHEY_SIMPLEX, fontScale,
+                    (255, 255, 255), thickness)
     return image
 
 
 def draw_text_line(image, point, text_line: str, bg_color=(255, 0, 0), thickness=-1, fontScale=-1.0, drawType="custom"):
     """
     :param image:
     :param point:
@@ -1888,14 +1889,56 @@
     y = int(round((h - crop_size[1]) / 2.))
     x = int(round((w - crop_size[0]) / 2.))
     rect = [x, y, crop_size[0], crop_size[1]]
     roi_image = get_rect_crop_padding(image, rect, color=color)
     return roi_image
 
 
+def center_crop_padding_mask_shift(mask, size=(256, 256), center=True, scale=1.0, color=(0, 0, 0)):
+    """
+    实现将白色区域平移到中心，居中显示(区域相对大小不会变化)
+    :param mask:
+    :param size: [crop_w,crop_h]
+    :param center: 是否居中
+    :param scale: 是否缩放
+    :param color: padding的颜色
+    :return:
+    """
+    mask = center_crop_padding(mask, crop_size=size, color=color)
+    if center:
+        box = get_mask_boundrect_cv(mask, binarize=False, shift=0)
+        if len(box) > 0:
+            cx, cy = (box[0] + box[2]) / 2, (box[1] + box[3]) / 2
+            new = (cx - size[0] / 2, cy - size[1] / 2,
+                   cx + size[0] / 2, cy + size[1] / 2)
+            mask = get_bbox_crop_padding(mask, new, color=color)
+    if scale < 1.0:
+        mask = get_scale_image(mask, scale=scale, color=color)
+    return mask
+
+
+def center_crop_padding_mask_resize(mask, size=(256, 256), center=True, scale=1.0, color=(0, 0, 0)):
+    """
+    实现将白色区域调整到中心，居中显示(区域相对大小会变化)
+    :param mask:
+    :param size: [crop_w,crop_h]
+    :param center: 是否居中
+    :param scale: 是否缩放
+    :param color: padding的颜色
+    :return:
+    """
+    if center:
+        box = get_mask_boundrect_cv(mask, binarize=False, shift=0)
+        if box: mask = get_bbox_crop(mask, box)
+    mask = resize_image_padding(mask, size=size, color=color, interpolation=cv2.INTER_LINEAR)
+    if scale < 1.0:
+        mask = get_scale_image(mask, scale=scale, color=color)
+    return mask
+
+
 def points2bbox(keypoints):
     joints_bbox = []
     for joints in keypoints:
         joints = np.asarray(joints)
         shape = joints.shape
         if len(shape) == 1:
             joints = joints.reshape(-1, 2)
@@ -2576,15 +2619,18 @@
     :param gif_file: 输出的GIF图的路径
     :param fps: 刷新频率
     :param loop: 循环次数
     :param use_rgb: frames是RGB格式，需要是BGR格式，use_bgr=True
     :return:
     """
     import imageio
-    writer = imageio.get_writer(uri=gif_file, mode='I', fps=fps, loop=loop)
+    "(in ms) instead, e.g. `fps=50` == `duration=20` (1000 * 1/50)."
+    duration = 1000 * 1 / fps
+    # writer = imageio.get_writer(uri=gif_file, mode='I', fps=fps, loop=loop)
+    writer = imageio.get_writer(uri=gif_file, mode='I', duration=duration, loop=loop)
     for image in frames:
         if use_rgb: image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
         writer.append_data(image)
     writer.close()
     # imageio.mimwrite(out_gif_path, frames, fps=20)
```

### Comparing `pybaseutils-0.8.5/pybaseutils/json_utils.py` & `pybaseutils-0.8.6/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/log.py` & `pybaseutils-0.8.6/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/logger.py` & `pybaseutils-0.8.6/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.6/pybaseutils/maker/convert_labelme2voc.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,67 +35,75 @@
                                                      check=False,
                                                      phase="val",
                                                      shuffle=False)
 
     def convert_dataset2voc(self, out_root, class_dict={}, out_image_dir=None, crop=False, rename=False, vis=True):
         """
         :param out_root: VOC输出根目录
-        :param class_dict: label映射 list或dict
+        :param class_dict: label映射 list或dict，如果label不在class_dict中，则使用原始label
         :param out_image_dir: 保存 JPEGImages
         :param crop: 是否进行目标裁剪
         :param rename: 是否重命名
         :param vis: 是否可视化
         :return:
         """
         out_xml_dir = os.path.join(out_root, "Annotations")
         out_crop_dir = os.path.join(out_root, "crops")
+        class_set = []
         for i in tqdm(range(len(self.dataset))):
             data = self.dataset.__getitem__(i)
             # data = self.dataset.__getitem__(307)
             image, points, bboxes, labels = data["image"], data["point"], data["box"], data["label"]
+            anno_file = data["anno_file"]
             image_file = data["image_file"]
             image_shape = image.shape
             if len(labels) == 0:
+                # file_utils.remove_file(anno_file)
+                # file_utils.remove_file(image_file)
                 print("empty dst_result:{}".format(image_file))
                 continue
             format = os.path.basename(image_file).split(".")[-1]
             image_id = os.path.basename(image_file)[:-len(format) - 1]
             if rename:
                 image_id = "{}_{:0=4d}".format(rename, i)
                 format = "jpg"
             newname = "{}.{}".format(image_id, format)
             xml_path = file_utils.create_dir(out_xml_dir, None, "{}.xml".format(image_id))
+            class_set = list(set(class_set + labels))
             objects = maker_voc.create_objects(bboxes, labels, keypoints=None, class_name=class_dict)
             maker_voc.write_voc_xml_objects(newname, image_shape, objects, xml_path)
             if crop and out_crop_dir:
                 self.save_object_crops(objects, image, out_crop_dir, image_id)
             if out_image_dir:
                 dst_file = file_utils.create_dir(out_image_dir, None, newname)
                 file_utils.copy_file(image_file, dst_file)
                 # cv2.imwrite(dst_file, image)
             if vis:
                 self.show_object_image(image, objects)
         if not out_image_dir: out_image_dir = self.image_dir
         file_utils.save_file_list(out_image_dir, filename=None, prefix="", postfix=file_utils.IMG_POSTFIX,
                                   only_id=False, shuffle=False, max_num=None)
+        class_set = sorted(class_set)
+        print("have class_set:{}\n{}".format(len(class_set), class_set))
 
     def save_object_crops(self, objects, image, out_dir, image_id):
         for i, item in enumerate(objects):
             label = item["name"]
             box = item["bndbox"]
             img = image_utils.get_bbox_crop(image, bbox=box)
             file = os.path.join(out_dir, str(label), "{}_{}_{:0=3d}.jpg".format(image_id, label, i))
             file_utils.create_file_path(file)
             cv2.imwrite(file, img)
 
     def show_object_image(self, image, objects):
         for item in objects:
             label = item["name"]
             box = item["bndbox"]
-            image = image_utils.draw_image_bboxes_text(image, [box], [label])
+            image = image_utils.draw_image_bboxes_text(image, [box], [label], thickness=3, fontScale=1.2,
+                                                       color=(0, 255, 0), drawType="chinese")
         image_utils.cv_show_image("image", image, use_rgb=False, delay=0)
 
 
 if __name__ == "__main__":
     json_dir = "/home/dm/nasdata/dataset/tmp/fall/fall-v3/json"
     out_root = os.path.dirname(json_dir)
     image_dir = os.path.join(out_root, "JPEGImages")
```

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.6/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.6/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.6/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.6/pybaseutils/maker/maker_labelme.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pybaseutils import image_utils, file_utils, coords_utils
 
 
 def maker_labelme(json_file, points, labels, image_name, image_size, image_bs64=None):
     """
     制作label数据格式
     :param json_file: 保存json文件路径
-    :param points: (num_labels,num_points,2)
+    :param points: (num_labels,num_points,2), points = image_utils.boxes2polygons(boxes)
     :param labels: (num_labels,)
     :param image_name: 图片名称，如果存在则进行拷贝到json_file同一级目录
     :param image_size: (W,H)
     :param image_bs64: 图片base64编码，可为None
     :return:
     """
     assert len(points) == len(labels)
```

### Comparing `pybaseutils-0.8.5/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.6/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.6/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.6/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.6/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.6/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.6/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.6/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.6/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/plot_utils.py` & `pybaseutils-0.8.6/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.6/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.6/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/setup_config.py` & `pybaseutils-0.8.6/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/thread_utils.py` & `pybaseutils-0.8.6/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/time_utils.py` & `pybaseutils-0.8.6/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.6/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.6/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.6/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/word_utils.py` & `pybaseutils-0.8.6/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/worker.py` & `pybaseutils-0.8.6/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.6/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.6/pybaseutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.5
+Version: 0.8.6
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.5/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.6/pybaseutils.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 pybaseutils/__init__.py
 pybaseutils/base64_utils.py
 pybaseutils/batch_utils.py
 pybaseutils/color_utils.py
 pybaseutils/config_utils.py
 pybaseutils/coords_utils.py
+pybaseutils/demo_nii.py
 pybaseutils/file_utils.py
 pybaseutils/font_utils.py
 pybaseutils/geometry_tools.py
 pybaseutils/heatmap_utils.py
 pybaseutils/image_utils.py
 pybaseutils/json_utils.py
 pybaseutils/log.py
@@ -61,29 +62,34 @@
 pybaseutils/metrics/average_meter.py
 pybaseutils/metrics/class_report.py
 pybaseutils/metrics/plot_pr.py
 pybaseutils/metrics/plot_roc.py
 pybaseutils/pycpp/__init__.py
 pybaseutils/pycpp/demo.py
 pybaseutils/pycpp/main.py
+pybaseutils/server/__init__.py
+pybaseutils/server/apm_server.py
 pybaseutils/transforms/__init__.py
 pybaseutils/transforms/affine_transform.py
 test_py/__init__.py
+test_py/apm_demo.py
 test_py/class_names.py
 test_py/demo1.py
 test_py/demo2.py
+test_py/demo3.py
 test_py/demo_async_await1.py
 test_py/demo_async_await2.py
 test_py/demo_copy_files.py
 test_py/demo_copy_files_for_voc.py
 test_py/demo_ffmpy.py
 test_py/demo_for_trt.py
 test_py/demo_get_file_list.py
 test_py/demo_gif.py
 test_py/demo_gif_video.py
+test_py/demo_labelme.py
 test_py/demo_metrics.py
 test_py/demo_mouse.py
 test_py/demo_pandas.py
 test_py/demo_plot.py
 test_py/demo_standard_image .py
 test_py/demo_standard_video .py
 test_py/demo_taichi.py
@@ -99,21 +105,27 @@
 test_py/performance.py
 test_py/converter/AffectNet.py
 test_py/converter/AsianMovie.py
 test_py/converter/BITVehicle2voc.py
 test_py/converter/BSTLD2voc.py
 test_py/converter/CCPD.py
 test_py/converter/CCPD2voc.py
+test_py/converter/FL3D_dataset.py
 test_py/converter/TT100K.py
 test_py/converter/__init__.py
+test_py/converter/convert_labelme2voc.py
+test_py/converter/fatigue_driving.py
+test_py/converter/fdd_dataset.py
 test_py/converter/insects_for_aichallenger.py
 test_py/converter/tt100k_utils.py
 test_py/converter/ua_detrac2voc.py
 test_py/detector/__init__.py
+test_py/detector/demo.py
 test_py/detector/detect_face_person.py
+test_py/detector/predet_labelme.py
 test_py/flask_demo/__init__.py
 test_py/flask_demo/func.py
 test_py/flask_demo/server.py
 test_py/image_correction/__init__.py
 test_py/image_correction/demo_correction_v1.py
 test_py/image_correction/demo_correction_v2.py
 test_py/image_correction/demo_correction_v3.py
```

### Comparing `pybaseutils-0.8.5/setup.py` & `pybaseutils-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/class_names.py` & `pybaseutils-0.8.6/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/AffectNet.py` & `pybaseutils-0.8.6/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.6/test_py/converter/AsianMovie.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         filename = file_utils.create_dir(os.path.join(out_dir, "origin"), None, "label.txt")
         print(filename)
         file_utils.write_data(filename, dst_item_list, split=",")
         return dst_item_list
 
 
 def main():
-    file = "/home/dm/nasdata/dataset/emotion/Asian_Facial_Expression/AsianMovie_0725_0730/list/total.txt"
-    image_dir = "/home/dm/nasdata/dataset/emotion/Asian_Facial_Expression/AsianMovie_0725_0730/images"
-    out_dir = "/home/dm/nasdata/dataset/csdn/emotion/emotion-domestic1"
+    file = "/home/PKing/nasdata/dataset/emotion/Asian_Facial_Expression/AsianMovie_0725_0730/list/total.txt"
+    image_dir = "/home/PKing/nasdata/dataset/emotion/Asian_Facial_Expression/AsianMovie_0725_0730/images"
+    out_dir = "/home/PKing/nasdata/dataset/emotion/Asian_Facial_Expression/dataset-pjq"
     wid = ParseAsian(file, image_dir)
     data_info = wid.parse_data(out_dir=out_dir, max_num=None, vis=False)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pybaseutils-0.8.5/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.6/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.6/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/CCPD.py` & `pybaseutils-0.8.6/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.6/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/TT100K.py` & `pybaseutils-0.8.6/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.6/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.6/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.6/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo1.py` & `pybaseutils-0.8.6/test_py/demo1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_async_await2.py` & `pybaseutils-0.8.6/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_copy_files.py` & `pybaseutils-0.8.6/test_py/demo_copy_files.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,50 +10,61 @@
 import xmltodict
 import random
 from tqdm import tqdm
 from pybaseutils import file_utils, image_utils
 
 
 def demo_copy_move_by_sub_names_v1():
-    image_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/train"
-    out_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/test"
-    file = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/形近字v1.txt"
+    """
+    按照整个文件夹，复制或者拷贝文件
+    :return:
+    """
+    # image_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/train"
+    # out_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/test"
+    # file = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/形近字v1.txt"
+    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-cls/dataset-v1/train"
+    out_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-cls/dataset-v1/test"
+    file = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-cls/dataset-v1/class_name.txt"
     # sub_names = ["玉", "王", "主", "玊", "壬", "玍", "生"]
     # sub_names += ["工", "土", "干", "士"]
     words = file_utils.read_data(file, split=",")
     sub_names = []
     for word in words:
         word = [w.strip() for w in word if w]  # 去除一些空格
         sub_names += word
     sub_names = list(set(sub_names))
     sub_names = sorted(sub_names)
-    file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=sub_names, max_nums=3000, shuffle=True, move=True)
-    out_file = os.path.join(os.path.dirname(file), "file.txt")
+    file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=sub_names, max_nums=30*6, shuffle=True, move=True)
+    out_file = os.path.join(os.path.dirname(file), "new_class_name.txt")
     file_utils.write_list_data(out_file, sub_names)
 
 
 def demo_copy_move_by_sub_names_v2():
+    """
+    按照每个类别的个数，复制或者拷贝文件
+    :return:
+    """
     # image_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/trainval/train"
     # out_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/train"
     # file = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/word-similar/dataset-clear/loss.txt"
 
-    image_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/trainval/similar/hardcase"
-    out_dir = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/trainval/similar/hardcase-test"
-    file = "/home/dm/cv/panjinquan/dataset-dmai/handwriting/word-class/trainval/similar/形近字v2.txt"
+    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-clothes/dataset-v1/trainval"
+    out_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-clothes/dataset-v1/test"
+    file = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-clothes/class_name.txt"
     words = file_utils.read_data(file, split=",")
     sub_names = []
     for word in words:
         word = [w.strip() for w in word if w]  # 去除一些空格
         sub_names += word
     sub_names = list(set(sub_names))
     sub_names = sorted(sub_names)
     # file_utils.copy_move_dir_dir(image_dir, out_dir, sub_names=sub_names, per_nums=90, shuffle=True, move=True)
-    file_utils.copy_move_dir_dir(image_dir, out_dir, sub_names=sub_names, per_nums=None, shuffle=True, move=False)
-    # out_file = os.path.join(os.path.dirname(file), "file.txt")
-    # file_utils.write_list_data(out_file, sub_names)
+    file_utils.copy_move_dir_dir(image_dir, out_dir, sub_names=sub_names, per_nums=20, shuffle=True, move=False)
+    out_file = os.path.join(os.path.dirname(file), "new_class_name.txt")
+    file_utils.write_list_data(out_file, sub_names)
 
 
 def demo_copy_move_by_sub_names_v3():
     image_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/train"
     out_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/test"
     # file_utils.copy_move_dir_dir(image_dir, out_dir, sub_names=sub_names, per_nums=10, shuffle=True, move=True)
     file_utils.copy_move_file_dir(image_dir, out_dir, sub_names=None, max_nums=10000, move=True, shuffle=True)
@@ -91,13 +102,13 @@
                 new = "{}_{}".format(sub, name)
                 dst = file_utils.create_dir(out, phase, new)
                 file_utils.copy_file(src, dst)
 
 
 if __name__ == "__main__":
     # demo_copy_move()
-    # demo_copy_move_by_sub_names_v1()
+    demo_copy_move_by_sub_names_v1()
     # demo_copy_move_by_sub_names_v2()
     # demo_copy_move_by_sub_names_v2()
     # demo_copy_move_by_sub_names_v3()
     # copy_files()
-    demo_copy_move()
+    # demo_copy_move()
```

### Comparing `pybaseutils-0.8.5/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.6/test_py/demo_copy_files_for_voc.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 import xmltodict
 import random
 from tqdm import tqdm
 from pybaseutils import file_utils, image_utils
 
 
-def image_dir_move_file(voc_root, out_dir, max_nums=5000, move=True, shuffle=True):
+def image_dir_move_file(voc_root, out_dir, max_nums=500, move=True, shuffle=True):
     image_dir = os.path.join(voc_root, "JPEGImages")
     annos_dir = os.path.join(voc_root, "Annotations")
     json_dir = os.path.join(voc_root, "json")
     image_list = file_utils.get_files_lists(image_dir, postfix=file_utils.IMG_POSTFIX + ["*.JPG"])
     if shuffle:
         random.seed(100)
         random.shuffle(image_list)
@@ -39,10 +39,10 @@
                 if move:
                     file_utils.move_file_to_dir(json_file, file_utils.create_dir(out_dir, "json"))
                 else:
                     file_utils.copy_file_to_dir(json_file, file_utils.create_dir(out_dir, "json"))
 
 
 if __name__ == "__main__":
-    voc_root = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/eyeglasses-v1/face1"
-    out_dir = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/eyeglasses-test/face1"
+    voc_root = "/home/PKing/nasdata/dataset/tmp/drowsy-driving/drowsy-driving/Drowsy-Driving-Det1/trainval"
+    out_dir = "/home/PKing/nasdata/dataset/tmp/drowsy-driving/drowsy-driving/Drowsy-Driving-Det1/test"
     image_dir_move_file(voc_root, out_dir, max_nums=500, shuffle=True)
```

### Comparing `pybaseutils-0.8.5/test_py/demo_get_file_list.py` & `pybaseutils-0.8.6/test_py/demo_get_file_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,11 +62,47 @@
     if max_num:
         max_num = min(max_num, len(file_list))
         file_list = file_list[0:max_num]
     file_utils.write_list_data(filename, file_list)
     print("num files:{},out_path:{}".format(len(file_list), filename))
 
 
+def get_voc_file_list(voc_root, prefix="", postfix=file_utils.IMG_POSTFIX, only_id=True, check=True, shuffle=False,
+                      max_num=None):
+    """
+    蝴蝶VOC数据集的文件列表
+    :param voc_root:
+    :param prefix:
+    :param postfix:
+    :param only_id:
+    :param check: 检测xml和图片是否存在
+    :param shuffle:
+    :param max_num:
+    :return:
+    """
+    image_dir = os.path.join(voc_root, "JPEGImages")
+    annos_dir = os.path.join(voc_root, "Annotations")
+    filename = os.path.join(os.path.dirname(image_dir), "file_list.txt")
+    file_list = file_utils.get_files_list(image_dir, prefix=prefix, postfix=postfix, basename=False)
+    file_list = file_utils.get_sub_list(file_list, dirname=image_dir)
+    if check:
+        xmls_list = file_utils.get_files_list(annos_dir, postfix=["*.xml"], basename=True)
+        print("xml file:{},image file:{}".format(len(xmls_list), len(file_list)))
+        xmls_ids = [str(f).split(".")[0] for f in xmls_list]
+        file_list = [f for f in file_list if str(f).split(".")[0] in xmls_ids]
+    if only_id:
+        file_list = [str(f).split(".")[0] for f in file_list]
+    if shuffle:
+        random.seed(100)
+        random.shuffle(file_list)
+    if max_num:
+        max_num = min(max_num, len(file_list))
+        file_list = file_list[0:max_num]
+    file_utils.write_list_data(filename, file_list)
+    print("num files:{},out_path:{}".format(len(file_list), filename))
+
+
 if __name__ == "__main__":
-    file_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/标注数据/岗评项目_室内电力操作检测-22labels/JPEGImages"
-    save_file_list(file_dir, prefix="", postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=False,
-                   max_num=None)
+    # file_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/标注数据/岗评项目_室内电力操作检测-22labels/JPEGImages"
+    # save_file_list(file_dir, postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=False, max_num=None)
+    voc_root = "/home/PKing/nasdata/dataset/tmp/drowsy-driving/drowsy-driving/Drowsy-Driving-Det1/test"
+    get_voc_file_list(voc_root, postfix=file_utils.IMG_POSTFIX + ["*.JPG"], only_id=False, shuffle=True, max_num=None)
```

### Comparing `pybaseutils-0.8.5/test_py/demo_gif.py` & `pybaseutils-0.8.6/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_gif_video.py` & `pybaseutils-0.8.6/test_py/demo_gif_video.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     frame = image_utils.resize_image(frame, size=(416, None))
     # frame = image_utils.resize_image(frame, size=(None, 640))  # android-video
     return frame
 
 
 def android_gif():
     # video_file = "/media/dm/新加卷/SDK/CSDN/双目测距/demo/image-nouse-wls.mp4"
-    video_file = "/home/dm/nasdata/dataset/tmp/Face-Recognition/demo/android-demo/android-人脸识别视频demo2.mp4"
-    video_utils.video2gif(video_file, interval=12, func=resize_android, fps=4, use_pil=False, vis=True)
+    video_file = "/home/PKing/nasdata/dataset/tmp/Drowsy-Driving/demo/android-demo-dd1.mp4"
+    video_utils.video2gif(video_file, interval=8, func=resize_android, fps=4, use_pil=False, vis=True)
 
 
 def python_gif():
-    video_file = "/media/dm/新加卷/SDK/face-recognition/Face-Recognition/Face-Recognition-Python/docs/result2.avi"
-    video_utils.video2gif(video_file, interval=7, func=resize_fun, fps=6, use_pil=False, vis=True)
+    video_file = "/home/PKing/nasdata/dataset/tmp/Drowsy-Driving/demo/python-demo-dd2.avi"
+    video_utils.video2gif(video_file, interval=6, func=resize_fun, fps=6, use_pil=False, vis=True)
 
 
 def image_gif():
     image_dir = "/home/dm/nasdata/dataset/tmp/Face-Recognition/demo/Cpp-demo/cpp-fr-demo"
     gif_file = image_dir + ".gif"
     frames = file_utils.get_images_list(image_dir)
     image_utils.image_file2gif(frames, size=(416, 416), padding=True, interval=1, gif_file=gif_file, fps=1,
```

### Comparing `pybaseutils-0.8.5/test_py/demo_metrics.py` & `pybaseutils-0.8.6/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_mouse.py` & `pybaseutils-0.8.6/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_pandas.py` & `pybaseutils-0.8.6/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_plot.py` & `pybaseutils-0.8.6/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_standard_image .py` & `pybaseutils-0.8.6/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_standard_video .py` & `pybaseutils-0.8.6/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_taichi.py` & `pybaseutils-0.8.6/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_video_aije.py` & `pybaseutils-0.8.6/test_py/demo_video_aije.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,11 +66,11 @@
     files = file_utils.get_files_list(root, postfix=["*.avi", "*.mp4", "*.flv"])
     for video_file in tqdm(files):
         print(video_file)
         video2frames_similarity(video_file, out_dir=out, func=None, interval=50, vis=True)
 
 
 if __name__ == "__main__":
-    root = "/home/PKing/nasdata/release/AIJE/岗评视频数据v1/videos"
+    root = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/开发数据/室内作业视频_0624-0712/20220707室内作业2"
     # root = "/home/PKing/nasdata/release/AIJE/岗评视频数据v1/videos"
     out = root + "-frame"
     video2frames_demo(root, out)
```

### Comparing `pybaseutils-0.8.5/test_py/demo_voc_crop.py` & `pybaseutils-0.8.6/test_py/demo_voc_crop.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,29 @@
 from tqdm import tqdm
 from pybaseutils.dataloader import parser_voc
 from pybaseutils import image_utils, file_utils
 
 
 def save_object_crops(image, out_dir, bboxes, labels, image_id, class_name=None,
                       scale=[], square=False, padding=False, flag="", vis=False):
+    """
+    对VOC的数据目标进行裁剪
+    :param image:
+    :param out_dir:
+    :param bboxes:
+    :param labels:
+    :param image_id:
+    :param class_name:
+    :param scale:
+    :param square:
+    :param padding:
+    :param flag:
+    :param vis:
+    :return:
+    """
     image_id = image_id.split(".")[0]
     if square:
         bboxes = image_utils.get_square_bboxes(bboxes, use_max=True, baseline=-1)
     if scale:
         bboxes = image_utils.extend_xyxy(bboxes, scale=scale)
     if padding:
         crops = image_utils.get_bboxes_crop_padding(image, bboxes)
@@ -26,44 +41,44 @@
     if vis:
         m = image_utils.draw_image_bboxes_labels(image.copy(), bboxes, labels, class_name=class_name,
                                                  thickness=2, fontScale=0.8, drawType="custom")
         image_utils.cv_show_image("image", m, use_rgb=False, delay=0)
     for i, img in enumerate(crops):
         name = class_name[int(labels[i])] if class_name else labels[i]
         if out_dir:
-            file_name = "{}_{:0=3d}_{}.jpg".format(image_id, i, flag) if flag else "{}_{:0=3d}.jpg".format(image_id, i)
+            file_name = "{}_{:0=4d}_{}.jpg".format(image_id, i, flag) if flag else "{}_{:0=4d}.jpg".format(image_id, i)
             img_file = file_utils.create_dir(out_dir, name, file_name)
             cv2.imwrite(img_file, img)
         if vis: image_utils.cv_show_image("crop", img, use_rgb=False, delay=0)
 
 
 if __name__ == "__main__":
     """
+    对VOC的数据目标进行裁剪
     """
-    # data_root = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v3"
-    filename = "/home/dm/nasdata/dataset/tmp/face_person/MPII/train5000.txt"
-    # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-old/train.txt"
+    # filename = "/home/PKing/nasdata/dataset/tmp/face_person/MPII/train5000.txt"
+    filename = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/equipment/dataset-v1/file_list.txt"
     # class_name = ["face", "face-eyeglasses"]
     # class_name = "/home/dm/nasdata/dataset/tmp/traffic-sign/TT100K/VOC/train/class_name.txt"
     # class_name = ["unique"]
-    # class_name = None
-    class_name = ['person']
-    out_dir = os.path.join(os.path.dirname(filename), "crops-train5000")
+    class_name = ['身穿工作服', '未穿工作服', '表箱关', '表箱开', '其他鞋', '绝缘鞋']
+    # class_name = ['person']
+    out_dir = os.path.join(os.path.dirname(filename), "crops")
     dataset = parser_voc.VOCDataset(filename=filename,
                                     data_root=None,
                                     anno_dir=None,
                                     image_dir=None,
                                     class_name=class_name,
                                     transform=None,
                                     check=False,
                                     use_rgb=False,
                                     shuffle=False)
     print("have num:{}".format(len(dataset)))
     class_name = dataset.class_name
-    scale = [1.1, 1.1]
+    scale = [1.0, 1.0]
     flag = str(scale[0]).replace(".", "p")
     flag = None
     # scale = None
     for i in tqdm(range(len(dataset))):
         try:
             data = dataset.__getitem__(i)
             image, targets, image_id = data["image"], data["target"], data["image_id"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybaseutils-0.8.5/test_py/demo_word_similar.py` & `pybaseutils-0.8.6/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_worker1.py` & `pybaseutils-0.8.6/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/demo_worker2.py` & `pybaseutils-0.8.6/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/detector/detect_face_person.py` & `pybaseutils-0.8.6/test_py/detector/detect_face_person.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,29 +68,29 @@
         :param vis:
         :return:
         """
         item_list = self.get_item_list_class(image_dir=image_dir, shuffle=shuffle)
         nums_sample = len(item_list)
         if max_num: nums_sample = min(max_num, nums_sample)
         for i in tqdm(range(nums_sample)):
-            image_file, label = item_list[i]
-            image_path = os.path.join(image_dir, image_file)
-            if not os.path.exists(image_path):
-                print("no path:{}".format(image_path))
+            image_name, label = item_list[i]
+            image_file = os.path.join(image_dir, image_name)
+            if not os.path.exists(image_file):
+                print("no path:{}".format(image_file))
                 continue
-            image = image_utils.read_image(image_path)
+            image = image_utils.read_image(image_file)
             if image is None:
-                print("empty file:{}".format(image_path))
+                print("empty file:{}".format(image_file))
                 continue
             h, w = image.shape[:2]
             rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             bbox_score, labels = self.detector.detect(rgb, vis=False)
             if len(bbox_score) == 0: continue
             dets = np.hstack((bbox_score, labels.reshape(-1, 1)))
-            image_id = "{}_{:0=6d}".format(flag, i) if flag else os.path.basename(image_file).split(".")[0]
+            image_id = "{}_{:0=6d}".format(flag, i) if flag else os.path.basename(image_name).split(".")[0]
             self.save_crops(image, dets, image_id, scale=scale, square=square, padding=padding, out_dir=out_dir,
                             vis=vis)
 
     def faceboxes2bodyup(self, xyxy, shift=(0, 0.5), scale=(1.0, 1.0)):
         """通过人脸框获得上半身"""
         if not isinstance(xyxy, np.ndarray): xyxy = np.asarray(xyxy)
         cxcywh = image_utils.xyxy2cxcywh(xyxy)
@@ -148,21 +148,21 @@
     padding = False
     flag = file_utils.get_time("s").replace("2023", "2018")
     # flag = ""
     data_info = dataset.parse_data(image_dir=image_dir, out_dir=out_dir, scale=scale, square=square,
                                    padding=padding, flag=flag, shuffle=False, vis=False)
 
 
-
 def demo_for_image_root():
     root = "/home/dm/nasdata/dataset/tmp/smoking-calling/train"
     out_root = "/home/dm/nasdata/dataset/tmp/smoking/smoking-person/dataset-v4/train"
     subs = file_utils.get_sub_paths(root)
     for sub in subs:
         image_dir = os.path.join(root, sub)
         out_dir = os.path.join(out_root, sub)
         demo_for_image_dir(image_dir, out_dir)
 
 
 if __name__ == '__main__':
-    demo_for_image_root()
-    # demo_for_image_dir()
+    """检测face person并裁剪"""
+    # demo_for_image_root()
+    demo_for_image_dir()
```

### Comparing `pybaseutils-0.8.5/test_py/flask_demo/server.py` & `pybaseutils-0.8.6/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-0.8.6/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-0.8.6/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-0.8.6/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/kafka_worker.py` & `pybaseutils-0.8.6/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/men_tracemalloc.py` & `pybaseutils-0.8.6/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.5/test_py/performance.py` & `pybaseutils-0.8.6/test_py/performance.py`

 * *Files identical despite different names*

