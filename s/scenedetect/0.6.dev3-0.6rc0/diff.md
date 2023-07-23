# Comparing `tmp/scenedetect-0.6.dev3.tar.gz` & `tmp/scenedetect-0.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scenedetect-0.6.dev3.tar", last modified: Sat Mar 12 04:40:52 2022, max compression
+gzip compressed data, was "dist\scenedetect-0.6rc0.tar", last modified: Mon Apr 25 01:28:44 2022, max compression
```

## Comparing `scenedetect-0.6.dev3.tar` & `scenedetect-0.6rc0.tar`

### file list

```diff
@@ -1,125 +1,135 @@
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/.github/
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      131 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/blank-template.md
--rw-rw-rw-   0        0        0     1551 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/bug-or-issue-report.md
--rw-rw-rw-   0        0        0     1044 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/feature-or-enhancement-request.md
--rw-rw-rw-   0        0        0      177 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/.gitignore
--rw-rw-rw-   0        0        0      140 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/.style.yapf
--rw-rw-rw-   0        0        0      356 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/.travis.yml
--rw-rw-rw-   0        0        0     5273 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/LICENSE
--rw-rw-rw-   0        0        0       47 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/MANIFEST.in
--rw-rw-rw-   0        0        0     4834 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     8260 2022-03-12 04:39:00.000000 scenedetect-0.6.dev3/README.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/docs/
--rw-rw-rw-   0        0        0    30519 2022-03-12 04:38:57.000000 scenedetect-0.6.dev3/docs/changelog.md
--rw-rw-rw-   0        0        0     4345 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/contributing.md
--rw-rw-rw-   0        0        0     7915 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/download.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/docs/examples/
--rw-rw-rw-   0        0        0     7004 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/examples/usage-example.md
--rw-rw-rw-   0        0        0    13151 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/examples/usage.md
--rw-rw-rw-   0        0        0     2344 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/faq.md
--rw-rw-rw-   0        0        0     5144 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/features.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/docs/img/
--rw-rw-rw-   0        0        0    28550 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/img/goldeneye-stats.png
--rw-rw-rw-   0        0        0    89719 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/img/params.png
--rw-rw-rw-   0        0        0     4857 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/img/pyscenedetect_logo.png
--rw-rw-rw-   0        0        0     3318 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/img/pyscenedetect_logo_small.png
--rw-rw-rw-   0        0        0     2810 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/index.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/docs/other/
--rw-rw-rw-   0        0        0     4331 2022-03-07 02:22:59.000000 scenedetect-0.6.dev3/docs/other/copyright.md
--rw-rw-rw-   0        0        0     2116 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/other/literature.md
--rw-rw-rw-   0        0        0      855 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/other/similar.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/docs/reference/
--rw-rw-rw-   0        0        0      510 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/reference/command-line.md
--rw-rw-rw-   0        0        0     2013 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/reference/config.md
--rw-rw-rw-   0        0        0     5550 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/reference/detection-methods.md
--rw-rw-rw-   0        0        0      367 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/reference/python-api.md
--rw-rw-rw-   0        0        0     2040 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/docs/reference/video-splitting.md
--rw-rw-rw-   0        0        0       17 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/requirements.txt
--rw-rw-rw-   0        0        0     2608 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/docs/supporting.md
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/manual/
--rw-rw-rw-   0        0        0      629 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/Makefile
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/manual/_static/
--rw-rw-rw-   0        0        0     3337 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/_static/pyscenedetect_logo.png
--rw-rw-rw-   0        0        0     4344 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/_static/pyscenedetect_logo_small.png
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/manual/api/
--rw-rw-rw-   0        0        0      567 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/backends.rst
--rw-rw-rw-   0        0        0      818 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/api/detectors.rst
--rw-rw-rw-   0        0        0     2302 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/frame_timecode.rst
--rw-rw-rw-   0        0        0     7729 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/migration_guide.rst
--rw-rw-rw-   0        0        0      256 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/api/scene_detector.rst
--rw-rw-rw-   0        0        0     4292 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/scene_manager.rst
--rw-rw-rw-   0        0        0      876 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/stats_manager.rst
--rw-rw-rw-   0        0        0      266 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/video_splitter.rst
--rw-rw-rw-   0        0        0     1153 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api/video_stream.rst
--rw-rw-rw-   0        0        0     8714 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/api.rst
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/manual/cli/
--rw-rw-rw-   0        0        0    15196 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/cli/commands.rst
--rw-rw-rw-   0        0        0     2449 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/cli/config_file.rst
--rw-rw-rw-   0        0        0     5987 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/cli/detectors.rst
--rw-rw-rw-   0        0        0     5891 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/cli/global_options.rst
--rw-rw-rw-   0        0        0     5857 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/conf.py
--rw-rw-rw-   0        0        0     2383 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/index.rst
--rwxrwxrwx   0        0        0      817 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/manual/make.bat
--rw-rw-rw-   0        0        0       39 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/manual/requirements.txt
--rw-rw-rw-   0        0        0     1736 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/mkdocs.yml
--rw-rw-rw-   0        0        0     2948 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/package-info.rst
--rw-rw-rw-   0        0        0      159 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect/
--rw-rw-rw-   0        0        0     5791 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/__init__.py
--rw-rw-rw-   0        0        0     2118 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/__main__.py
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect/backends/
--rw-rw-rw-   0        0        0     5735 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/backends/__init__.py
--rw-rw-rw-   0        0        0    11037 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/backends/opencv.py
--rw-rw-rw-   0        0        0    13117 2022-03-12 04:38:39.000000 scenedetect-0.6.dev3/scenedetect/backends/pyav.py
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect/cli/
--rw-rw-rw-   0        0        0    35720 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/cli/__init__.py
--rw-rw-rw-   0        0        0    14246 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/cli/config.py
--rw-rw-rw-   0        0        0    36655 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/cli/context.py
--rw-rw-rw-   0        0        0    11876 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/cli/controller.py
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect/detectors/
--rw-rw-rw-   0        0        0     4144 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/detectors/__init__.py
--rw-rw-rw-   0        0        0     7725 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/detectors/adaptive_detector.py
--rw-rw-rw-   0        0        0     8329 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/detectors/content_detector.py
--rw-rw-rw-   0        0        0     4041 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/detectors/motion_detector.py
--rw-rw-rw-   0        0        0     8131 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/detectors/threshold_detector.py
--rw-rw-rw-   0        0        0    19149 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/frame_timecode.py
--rw-rw-rw-   0        0        0     8305 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/platform.py
--rw-rw-rw-   0        0        0     5068 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/scene_detector.py
--rw-rw-rw-   0        0        0    39576 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/scene_manager.py
--rw-rw-rw-   0        0        0    14612 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/stats_manager.py
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/
--rw-rw-rw-   0        0        0     2570 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-CLICK
--rw-rw-rw-   0        0        0     1728 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-NUMPY
--rw-rw-rw-   0        0        0     1787 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-OPENCV
--rw-rw-rw-   0        0        0     1317 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-PYTEST
--rw-rw-rw-   0        0        0     2308 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-TQDM
--rw-rw-rw-   0        0        0      877 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/__init__.py
--rw-rw-rw-   0        0        0    10518 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect/thirdparty/simpletable.py
--rw-rw-rw-   0        0        0    11012 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/video_splitter.py
--rw-rw-rw-   0        0        0     8481 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect/video_stream.py
--rw-rw-rw-   0        0        0     5614 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect.cfg
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/scenedetect.egg-info/
--rw-rw-rw-   0        0        0     4834 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-03-12 04:40:51.000000 scenedetect-0.6.dev3/scenedetect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      894 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/scenedetect.py
--rw-rw-rw-   0        0        0      915 2022-02-23 01:56:06.000000 scenedetect-0.6.dev3/scenedetect.spec
--rw-rw-rw-   0        0        0      218 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/setup.cfg
--rw-rw-rw-   0        0        0     3790 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-12 04:40:52.000000 scenedetect-0.6.dev3/tests/
--rw-rw-rw-   0        0        0      901 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/__init__.py
--rw-rw-rw-   0        0        0     2421 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/conftest.py
--rw-rw-rw-   0        0        0     3748 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_api.py
--rw-rw-rw-   0        0        0     1347 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_backend_pyav.py
--rw-rw-rw-   0        0        0     6621 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_cli.py
--rw-rw-rw-   0        0        0     6781 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_detectors.py
--rw-rw-rw-   0        0        0    11801 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_frame_timecode.py
--rw-rw-rw-   0        0        0     2182 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_platform.py
--rw-rw-rw-   0        0        0     5979 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_scene_manager.py
--rw-rw-rw-   0        0        0    10384 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_stats_manager.py
--rw-rw-rw-   0        0        0    11749 2022-03-12 04:01:26.000000 scenedetect-0.6.dev3/tests/test_video_stream.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/.github/
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      131 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/blank-template.md
+-rw-rw-rw-   0        0        0     1551 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/bug-or-issue-report.md
+-rw-rw-rw-   0        0        0     1044 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/feature-or-enhancement-request.md
+-rw-rw-rw-   0        0        0      177 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/.gitignore
+-rw-rw-rw-   0        0        0      140 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/.style.yapf
+-rw-rw-rw-   0        0        0     1663 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/.travis.yml
+-rw-rw-rw-   0        0        0     5273 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/LICENSE
+-rw-rw-rw-   0        0        0       47 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4829 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     8295 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/README.md
+-rw-rw-rw-   0        0        0     2713 2022-04-20 22:35:55.000000 scenedetect-0.6rc0/appveyor.yml
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/dist/
+-rw-rw-rw-   0        0        0     1436 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/dist/.version_info
+-rw-rw-rw-   0        0        0     1087 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/dist/cleanup_dependencies.py
+-rw-rw-rw-   0        0        0     2945 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/dist/package-info.rst
+-rw-rw-rw-   0        0        0      247 2022-04-09 23:12:23.000000 scenedetect-0.6rc0/dist/requirements_windows.txt
+-rw-rw-rw-   0        0        0     1023 2022-04-20 22:37:49.000000 scenedetect-0.6rc0/dist/scenedetect.spec
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/docs/
+-rw-rw-rw-   0        0        0    32493 2022-04-25 01:24:13.000000 scenedetect-0.6rc0/docs/changelog.md
+-rw-rw-rw-   0        0        0     4345 2022-03-26 17:39:06.000000 scenedetect-0.6rc0/docs/contributing.md
+-rw-rw-rw-   0        0        0     7913 2022-04-25 01:24:13.000000 scenedetect-0.6rc0/docs/download.md
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/docs/examples/
+-rw-rw-rw-   0        0        0     5238 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/examples/usage-example.md
+-rw-rw-rw-   0        0        0    13149 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/examples/usage.md
+-rw-rw-rw-   0        0        0     2352 2022-03-18 01:58:43.000000 scenedetect-0.6rc0/docs/faq.md
+-rw-rw-rw-   0        0        0     5144 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/features.md
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/docs/img/
+-rw-rw-rw-   0        0        0    28550 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/img/goldeneye-stats.png
+-rw-rw-rw-   0        0        0    89719 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/img/params.png
+-rw-rw-rw-   0        0        0     4857 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/img/pyscenedetect_logo.png
+-rw-rw-rw-   0        0        0     3318 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/img/pyscenedetect_logo_small.png
+-rw-rw-rw-   0        0        0     2810 2022-04-25 01:24:13.000000 scenedetect-0.6rc0/docs/index.md
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/docs/other/
+-rw-rw-rw-   0        0        0     4331 2022-03-07 02:22:59.000000 scenedetect-0.6rc0/docs/other/copyright.md
+-rw-rw-rw-   0        0        0     2116 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/other/literature.md
+-rw-rw-rw-   0        0        0      855 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/other/similar.md
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/docs/reference/
+-rw-rw-rw-   0        0        0      510 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/reference/command-line.md
+-rw-rw-rw-   0        0        0     2013 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/reference/config.md
+-rw-rw-rw-   0        0        0     5550 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/reference/detection-methods.md
+-rw-rw-rw-   0        0        0      367 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/reference/python-api.md
+-rw-rw-rw-   0        0        0     2040 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/docs/reference/video-splitting.md
+-rw-rw-rw-   0        0        0       17 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/requirements.txt
+-rw-rw-rw-   0        0        0     2608 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/docs/supporting.md
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/manual/
+-rw-rw-rw-   0        0        0      629 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/Makefile
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/manual/_static/
+-rw-rw-rw-   0        0        0     3337 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/_static/pyscenedetect_logo.png
+-rw-rw-rw-   0        0        0     4344 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/_static/pyscenedetect_logo_small.png
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/manual/api/
+-rw-rw-rw-   0        0        0      553 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/api/backends.rst
+-rw-rw-rw-   0        0        0      818 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/api/detectors.rst
+-rw-rw-rw-   0        0        0     2302 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/api/frame_timecode.rst
+-rw-rw-rw-   0        0        0     7980 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/api/migration_guide.rst
+-rw-rw-rw-   0        0        0      801 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/api/platform.rst
+-rw-rw-rw-   0        0        0      256 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/api/scene_detector.rst
+-rw-rw-rw-   0        0        0     4282 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/api/scene_manager.rst
+-rw-rw-rw-   0        0        0      876 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/api/stats_manager.rst
+-rw-rw-rw-   0        0        0      266 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/api/video_splitter.rst
+-rw-rw-rw-   0        0        0     1153 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/api/video_stream.rst
+-rw-rw-rw-   0        0        0     9548 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/api.rst
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/manual/cli/
+-rw-rw-rw-   0        0        0     1478 2022-04-22 01:37:29.000000 scenedetect-0.6rc0/manual/cli/backends.rst
+-rw-rw-rw-   0        0        0    15196 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/cli/commands.rst
+-rw-rw-rw-   0        0        0     2296 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/cli/config_file.rst
+-rw-rw-rw-   0        0        0     5987 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/manual/cli/detectors.rst
+-rw-rw-rw-   0        0        0     6021 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/cli/global_options.rst
+-rw-rw-rw-   0        0        0     5856 2022-04-24 01:31:01.000000 scenedetect-0.6rc0/manual/conf.py
+-rw-rw-rw-   0        0        0     2419 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/index.rst
+-rwxrwxrwx   0        0        0      817 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/manual/make.bat
+-rw-rw-rw-   0        0        0       43 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/manual/requirements.txt
+-rw-rw-rw-   0        0        0     1736 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/mkdocs.yml
+-rw-rw-rw-   0        0        0      162 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/requirements.txt
+-rw-rw-rw-   0        0        0      183 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/requirements_headless.txt
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect/
+-rw-rw-rw-   0        0        0     8301 2022-04-24 01:31:01.000000 scenedetect-0.6rc0/scenedetect/__init__.py
+-rw-rw-rw-   0        0        0     2118 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/scenedetect/__main__.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect/backends/
+-rw-rw-rw-   0        0        0     3488 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/backends/__init__.py
+-rw-rw-rw-   0        0        0    13058 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/backends/opencv.py
+-rw-rw-rw-   0        0        0    14741 2022-04-09 14:24:29.000000 scenedetect-0.6rc0/scenedetect/backends/pyav.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect/cli/
+-rw-rw-rw-   0        0        0    36071 2022-04-22 01:38:59.000000 scenedetect-0.6rc0/scenedetect/cli/__init__.py
+-rw-rw-rw-   0        0        0    14610 2022-04-22 01:38:11.000000 scenedetect-0.6rc0/scenedetect/cli/config.py
+-rw-rw-rw-   0        0        0    36963 2022-04-22 02:49:10.000000 scenedetect-0.6rc0/scenedetect/cli/context.py
+-rw-rw-rw-   0        0        0    11597 2022-04-22 00:59:19.000000 scenedetect-0.6rc0/scenedetect/cli/controller.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect/detectors/
+-rw-rw-rw-   0        0        0     4144 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/scenedetect/detectors/__init__.py
+-rw-rw-rw-   0        0        0     8857 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/detectors/adaptive_detector.py
+-rw-rw-rw-   0        0        0     8210 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/detectors/content_detector.py
+-rw-rw-rw-   0        0        0     4041 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/scenedetect/detectors/motion_detector.py
+-rw-rw-rw-   0        0        0     8386 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/detectors/threshold_detector.py
+-rw-rw-rw-   0        0        0    19152 2022-04-20 21:56:17.000000 scenedetect-0.6rc0/scenedetect/frame_timecode.py
+-rw-rw-rw-   0        0        0     8463 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/platform.py
+-rw-rw-rw-   0        0        0     5181 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/scene_detector.py
+-rw-rw-rw-   0        0        0    40797 2022-04-22 00:59:14.000000 scenedetect-0.6rc0/scenedetect/scene_manager.py
+-rw-rw-rw-   0        0        0    14528 2022-04-22 01:26:42.000000 scenedetect-0.6rc0/scenedetect/stats_manager.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect/thirdparty/
+-rw-rw-rw-   0        0        0     2570 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-CLICK
+-rw-rw-rw-   0        0        0     1728 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-NUMPY
+-rw-rw-rw-   0        0        0     1787 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-OPENCV
+-rw-rw-rw-   0        0        0     1317 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-PYTEST
+-rw-rw-rw-   0        0        0     2308 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-TQDM
+-rw-rw-rw-   0        0        0      877 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/scenedetect/thirdparty/__init__.py
+-rw-rw-rw-   0        0        0    10518 2022-02-23 01:56:06.000000 scenedetect-0.6rc0/scenedetect/thirdparty/simpletable.py
+-rw-rw-rw-   0        0        0    33589 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/video_manager.py
+-rw-rw-rw-   0        0        0    12334 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/video_splitter.py
+-rw-rw-rw-   0        0        0     8508 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect/video_stream.py
+-rw-rw-rw-   0        0        0     6427 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/scenedetect.cfg
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/scenedetect.egg-info/
+-rw-rw-rw-   0        0        0     4829 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3049 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-04-25 01:28:43.000000 scenedetect-0.6rc0/scenedetect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      894 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/scenedetect.py
+-rw-rw-rw-   0        0        0      223 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/setup.cfg
+-rw-rw-rw-   0        0        0     3794 2022-04-24 01:31:07.000000 scenedetect-0.6rc0/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-25 01:28:44.000000 scenedetect-0.6rc0/tests/
+-rw-rw-rw-   0        0        0      901 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2383 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/tests/conftest.py
+-rw-rw-rw-   0        0        0     4210 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/tests/test_api.py
+-rw-rw-rw-   0        0        0     1368 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/tests/test_backend_pyav.py
+-rw-rw-rw-   0        0        0     4244 2022-04-22 01:26:05.000000 scenedetect-0.6rc0/tests/test_backwards_compat.py
+-rw-rw-rw-   0        0        0     7865 2022-03-28 22:11:44.000000 scenedetect-0.6rc0/tests/test_cli.py
+-rw-rw-rw-   0        0        0     6781 2022-04-20 22:02:29.000000 scenedetect-0.6rc0/tests/test_detectors.py
+-rw-rw-rw-   0        0        0    12687 2022-04-20 22:11:45.000000 scenedetect-0.6rc0/tests/test_frame_timecode.py
+-rw-rw-rw-   0        0        0     2182 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/tests/test_platform.py
+-rw-rw-rw-   0        0        0     5979 2022-03-13 21:24:38.000000 scenedetect-0.6rc0/tests/test_scene_manager.py
+-rw-rw-rw-   0        0        0     9040 2022-04-22 01:28:27.000000 scenedetect-0.6rc0/tests/test_stats_manager.py
+-rw-rw-rw-   0        0        0    11883 2022-04-20 22:01:55.000000 scenedetect-0.6rc0/tests/test_video_stream.py
```

### Comparing `scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/bug-or-issue-report.md` & `scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/bug-or-issue-report.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/.github/ISSUE_TEMPLATE/feature-or-enhancement-request.md` & `scenedetect-0.6rc0/.github/ISSUE_TEMPLATE/feature-or-enhancement-request.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/LICENSE` & `scenedetect-0.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/PKG-INFO` & `scenedetect-0.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenedetect
-Version: 0.6.dev3
+Version: 0.6rc0
 Summary: Video scene cut/shot detection program and Python library.
 Home-page: https://github.com/Breakthrough/PySceneDetect
 Author: Brandon Castellano
 Author-email: brandon248@gmail.com
 License: BSD 3-Clause
 Project-URL: Homepage, https://pyscenedetect.readthedocs.io/
 Project-URL: Manual, https://manual.scenedetect.com/en/v0.6/
@@ -30,15 +30,15 @@
            :target: http://pyscenedetect.readthedocs.org/en/latest/copyright/
         
         .. image:: https://img.shields.io/github/stars/Breakthrough/PySceneDetect.svg?style=social&label=View%20on%20Github
            :target: https://github.com/Breakthrough/PySceneDetect
         
         ----------------------------------------------------------
         
-        Website: http://py.scenedetect.com/
+        Website: http://scenedetect.com/
         
         Documentation: http://manual.scenedetect.com/
         
         Github Repo: https://github.com/Breakthrough/PySceneDetect/
         
         ----------------------------------------------------------
```

### Comparing `scenedetect-0.6.dev3/README.md` & `scenedetect-0.6rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 ----------------------------------------------------------
 
 ### Latest Release: v0.6-dev3 (March 11, 2022)
 
 **Website**:  http://www.scenedetect.com
 
-**Getting Started**: [Usage Example](https://scenedetect.com/examples/usage-example/)
+**Getting Started**: [Usage Example](https://scenedetect.com/en/v0.6/examples/usage-example/)
 
 **Documentation**:  http://manual.scenedetect.com
 
 **Discord**: https://discord.gg/H83HbJngk7
 
 ----------------------------------------------------------
 
 **Quick Install**: To install PySceneDetect via `pip` with all dependencies:
 
     pip install scenedetect[opencv] --pre
 
-For servers, you can use the headless (non-GUI) version of OpenCV by installing `scenedetect[opencv-headless]`.  To enable video splitting support, you will also need to have `mkvmerge` or `ffmpeg` installed - see the documentation on [Video Splitting Support](https://scenedetect.com/examples/video-splitting/) for details.
+For servers, you can use the headless (non-GUI) version of OpenCV by installing `scenedetect[opencv-headless]`.  To enable video splitting support, you will also need to have `mkvmerge` or `ffmpeg` installed - see the documentation on [Video Splitting Support](https://scenedetect.com/en/v0.6/examples/video-splitting/) for details.
 
 Requires Python modules `click`, `numpy`, OpenCV `cv2`, and (optional) `tqdm` for displaying progress.  For details, see the [dependencies on the downloads page](https://scenedetect.com/download/#dependencies).
 
 ----------------------------------------------------------
 
 **Quick Start (Command Line)**:
 
@@ -40,15 +40,15 @@
 
     scenedetect -i video.mp4 time -s 10s detect-content list-scenes
 
 To show a summary of all other options and commands:
 
     scenedetect help
 
-You can find more examples [on the website](https://scenedetect.com/examples/usage-example/) or [in the manual](https://manual.scenedetect.com/en/v0.6/cli/global_options.html).
+You can find more examples [on the website](https://scenedetect.com/en/v0.6/examples/usage-example/) or [in the manual](https://manual.scenedetect.com/en/v0.6/cli/global_options.html).
 
 **Quick Start (Python API)**:
 
 To get started, there is a high level function in the library that performs content-aware scene detection on a video (try it from a Python prompt):
 
 ```python
 from scenedetect import detect, ContentDetector
@@ -80,43 +80,43 @@
 ```python
 from scenedetect import open_video, SceneManager, split_video_ffmpeg
 from scenedetect.detectors import ContentDetector
 from scenedetect.video_splitter import split_video_ffmpeg
 
 def split_video_into_scenes(video_path, threshold=27.0):
     # Open our video, create a scene manager, and add a detector.
-    video = open_video(path=video_path)
+    video = open_video(video_path)
     scene_manager = SceneManager()
     scene_manager.add_detector(
         ContentDetector(threshold=threshold))
     scene_manager.detect_scenes(video, show_progress=True)
     scene_list = scene_manager.get_scene_list()
     split_video_ffmpeg(video_path, scene_list, show_progress=True)
 ```
 
 See [the manual](https://manual.scenedetect.com/en/v0.6/api.html) for the
 full PySceneDetect API documentation.
 
 ----------------------------------------------------------
 
-PySceneDetect is a command-line tool and Python library, which uses OpenCV to analyze a video to find each shot change (or "cut"/"scene").  If `ffmpeg` or `mkvmerge` is installed, the video can also be split into scenes automatically.  A frame-by-frame analysis can also be generated for a video, to help with determining optimal threshold values or detecting patterns/other analysis methods for a particular video.  See [the Usage documentation](https://scenedetect.com/examples/usage/) for details.
+PySceneDetect is a command-line tool and Python library, which uses OpenCV to analyze a video to find each shot change (or "cut"/"scene").  If `ffmpeg` or `mkvmerge` is installed, the video can also be split into scenes automatically.  A frame-by-frame analysis can also be generated for a video, to help with determining optimal threshold values or detecting patterns/other analysis methods for a particular video.  See [the Usage documentation](https://scenedetect.com/en/v0.6/examples/usage/) for details.
 
 There are two main detection methods PySceneDetect uses: `detect-threshold` (comparing each frame to a set black level, useful for detecting cuts and fades to/from black), and `detect-content` (compares each frame sequentially looking for changes in content, useful for detecting fast cuts between video scenes, although slower to process).  Each mode has slightly different parameters, and is described in detail below.
 
 In general, use `detect-threshold` mode if you want to detect scene boundaries using fades/cuts in/out to black.  If the video uses a lot of fast cuts between content, and has no well-defined scene boundaries, you should use the `detect-content` mode.  Once you know what detection mode to use, you can try the parameters recommended below, or generate a statistics file (using the `-s` / `--statsfile` flag) in order to determine the correct paramters - specifically, the proper threshold value.
 
 For help or other issues, you can join [the official PySceneDetect Discord Server](https://discord.gg/H83HbJngk7), submit an issue/bug report [here on Github](https://github.com/Breakthrough/PySceneDetect/issues), or contact me via [my website](http://www.bcastell.com/about/).
 
 
 Usage
 ----------------------------------------------------------
 
  - [Basic Usage](https://scenedetect.com/en/latest/examples/usage/)
  - [PySceneDetect Manual](https://manual.scenedetect.com/io/en/latest/), covers `scenedetect` command and Python API
- - [Example: Detecting and Splitting Scenes in Movie Clip](https://scenedetect.com/examples/usage-example/)
+ - [Example: Detecting and Splitting Scenes in Movie Clip](https://scenedetect.com/en/v0.6/examples/usage-example/)
 
 
 Features & Roadmap
 ----------------------------------------------------------
 
 You can [view the latest features and version roadmap on Readthedocs](http://pyscenedetect.readthedocs.org/en/latest/features/).
 See [`docs/changelog.md`](https://github.com/Breakthrough/PySceneDetect/blob/master/docs/changelog.md) for a list of changes in each version, or visit [the Releases page](https://github.com/Breakthrough/PySceneDetect/releases) to download a specific version.  Feel free to submit any bugs/issues or feature requests to [the Issue Tracker](https://github.com/Breakthrough/PySceneDetect/issues).
```

### Comparing `scenedetect-0.6.dev3/docs/changelog.md` & `scenedetect-0.6rc0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 PySceneDetect Releases
 ==========================================================
 
 ## PySceneDetect 0.6
 
-### 0.6-dev3 (March 11, 2022)
+### 0.6-rc0 (April 24, 2022)
 
 #### Release Notes
 
 **This is a pre-release of the upcoming PySceneDetect v0.6.**
 
 PySceneDetect v0.6 is a **major breaking change** including better performance, configuration file support, and a more ergonomic API.  The new **minimum Python version is now 3.6**. See the [Migration Guide](https://manual.scenedetect.com/en/v0.6/api/migration_guide.html) for information on how to port existing applications to the new API.  Most users will see performance improvements after updating, and changes to the command-line are not expected to break most workflows.
 
@@ -21,21 +21,35 @@
  * Support for Python 2.7 has been dropped, minimum supported Python version is 3.6
  * Support for OpenCV 2.x has been dropped, minimum OpenCV version is 3.x
  * Decoding now runs in parallel with detection resulting in significant performance improvements
  * Adds support for configuration file via command line or in user settings folder
  * Adds support for multiple video backends, PyAV is now supported in addition to OpenCV
  * Breaking API changes to `VideoManager` (replaced with `VideoStream`), `StatsManager`, and `save_images()`
     * See the [Migration Guide](https://manual.scenedetect.com/en/v0.6/api/migration_guide.html) for details on how to update from v0.5.x
+    * A backwards compatibility layer has been added to prevent most applications from breaking - this layer will be removed in a future release
 
 **Command-Line Changes:**
 
+*v0.6-rc0*:
+ * Using `--backend pyav` no longer causes the application to occasionally hang once processing is complete
+ * `save-images` now supports image sequences
+ * `-s`/`--stats` is now only used to write stats files, previously would load existing contents if any
+    * Previous behavior can be obtained by merging stats files from multiple runs and setting the start/end times accordingly
+ * Using `--backend opencv` is now more robust to frame decode failures
+ * Add global option `--merge-last-scene` to merge final scene if it is shorter than `--min-scene-len`
+ * Frame numbers are now 1-based, and there is no longer any overlap between the start/end frame numbers of adjacent scenes
+     * This also applies to the frame numbers in a statsfile (`-s`/`--stats`) and those provided by `list-scenes`
+     * The output via the CLI now matches `ffmpeg` in all cases
+ * The default backend has been changed back to `opencv`
+     * To enable the `pyav` backend, either specify `-b pyav` via the command line, or set `backend = pyav` under `[global]` in your [config file](http://scenedetect.com/projects/Manual/en/v0.6/cli/config_file.html)
+
 *v0.6-dev3*:
 
- * `pyav` backend (the `av` package) will be used by default for video decoding, if installed
- * Specifying `-b pyav` / `--backend pyav` now uses faster multithreaded decoding
+ * The `pyav` backend (the `av` package) will be used by default
+ * The `pyav` backend now uses faster multithreaded decoding
  * [v0.6-only] Fix progress bar stuck at 0 when video duration was not available
  * [v0.6-only] Fix slow seeking with `pyav` backend
 
 *v0.6-dev2*:
 
  * Configuration files are now supported via `-c`/`--config` or from a user config folder ([see documentation for details](https://scenedetect.com/en/v0.6/reference/config))
  * `-i`/`--input` may no longer be specified multiple times (use an external tool like `ffmpeg` to perform concatenation first)
@@ -50,39 +64,47 @@
      * Default threshold `-t`/`--threshold` lowered to 27 to be more sensitive to shot changes ([#246](https://github.com/Breakthrough/PySceneDetect/issues/246))
      * Add override for global `-m`/`--min-scene-len` option
  * `detect-threshold` command:
      * `-p`/`--min-percent` and `-b`/`--block-size` have been removed
      * Add override for global `-m`/`--min-scene-len` option
  * `split-video` command:
      * Long name for `-a` has been changed to `--args` (from `--override-args`)
-     * `-c`/`--copy` now uses `ffmpeg` instead of `mkvmerge`
-     * New `-m`/`--mkvmerge` flag can be set to use `mkvmerge` instead of `ffmpeg`
+     * `-c`/`--copy` now uses `ffmpeg` instead of `mkvmerge` ([#77](https://github.com/Breakthrough/PySceneDetect/issues/77), [#236](https://github.com/Breakthrough/PySceneDetect/issues/236))
+     * New `-m`/`--mkvmerge` flag can be set to use `mkvmerge` instead of `ffmpeg` ([#77](https://github.com/Breakthrough/PySceneDetect/issues/77))
 
 **API Changes:**
 
+*v0.6-rc0*:
+
+ * Add some backwards compatibility with v0.5 to avoid breaking most applications on release while still allowing performance improvements
+ * Changes to `StatsManager`:
+    * The `load_from_csv` method is now deprecated and will be removed in v1.0
+ * [v0.6-only] `VideoStreamAv`: Many fixes around `threading_mode` and documentation regarding application lockups
+ * [v0.6-only] Moved `open_video` function from `scenedetect.backends` to `scenedetect` module
+ * Changes to `FrameTimecode`:
+    * Values in the form of seconds (float) or timecodes (str) are now rounded to the nearest frame, rather than truncated ([#268](https://github.com/Breakthrough/PySceneDetect/issues/268)), allowing correct round-trip conversion
+
 *v0.6-dev3*:
 
  * [v0.6-only] `VideoStreamAv`:
     * Allow specifying `threading_mode`, default is now to use multithreaded decoding
     * Allow specifying `framerate`
     * Fix incorrect duration calculation
  * Changes to `FrameTimecode`:
     * `FrameTimecode` objects can now perform arithmetic with formatted strings, e.g. `'HH:MM:SS.nnn'`
  * Changes to `StatsManager`:
-    * The `load_from_csv`/`save_to_csv` methods now accept a path or an open file handle
     * The `base_timecode` argument has been removed from `save_to_csv` (it is no longer required)
- * When calling `scenedetect.backends.open_video`, `VideoStreamAv` will now be used as the preferred backend instead of `VideoStreamCv2`
+ * When calling `scenedetect.open_video`, `VideoStreamAv` will now be used as the preferred backend instead of `VideoStreamCv2`
 
 *v0.6-dev2*:
 
  * New high-level `detect` function in `scenedetect` module that only has two required arguments: the path to a video (`path`) and a detector (`detector`), [see example here](http://manual.scenedetect.com/en/v0.6/api.html#quickstart)
  * New `VideoStream` replaces `VideoManager` and supports both OpenCV (`VideoStreamCv2`) and PyAV (`VideoStreamAv`) backends ([#213](https://github.com/Breakthrough/PySceneDetect/issues/213))
     * Improves video seeking invariants, especially around defining what frames 0 and 1 mean for different time properties (`frame_number` is 1-based whereas `position` is 0-based to align with PTS)
     * See `test_time_invariants` in `tests/test_video_stream.py` as a reference for specific behaviours of these properties, and a test video detailing visually what is expected
-    * Both command-line and public-facing API outputs still retain 0-based frame numbers (this will be changed in v1.0)
  * Changes to `SceneManager`:
     * `SceneManager` is now responsible for frame downscaling (see the `downscale` and `auto_downscale` properties)
     * `detect_scenes()` now performs video decoding in a background thread which greatly improves performance in many cases
     * `clear()` now also clears any
     * `detect_scenes()` no longer displays a progress bar by default (set `show_progress=True` to restore the previous behaviour)detectors, as detectors are stateful
     * `get_scene_list()` now returns an empty list if there are no detected cuts (previously one scene with the duration of the video was returned)
         * To restore the previous behaviour, specify `start_in_scene=True`
```

### Comparing `scenedetect-0.6.dev3/docs/contributing.md` & `scenedetect-0.6rc0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/download.md` & `scenedetect-0.6rc0/docs/download.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 </div>
 
 PySceneDetect is available via `pip` as [the `scenedetect` package](https://pypi.org/project/scenedetect/).  See below for instructions on installing a non-pip version of OpenCV.  To ensure you have all the requirements installed, open a `python` interpreter, and ensure you can run `import cv2` without any errors.
 
 ### Windows Build (64-bit Only) &nbsp; <span class="wy-text-neutral"><span class="fa fa-windows"></span></span>
 
 <div class="important">
-<h3 class="wy-text-neutral"><span class="fa fa-forward wy-text-info"></span> Latest Release: <b class="wy-text-neutral">v0.6-dev2</b></h3>
-<h4 class="wy-text-neutral"><span class="fa fa-calendar wy-text-info"></span>&nbsp; Release Date:&nbsp; <b>March 6, 2022</b></h4>
+<h3 class="wy-text-neutral"><span class="fa fa-forward wy-text-info"></span> Latest Release: <b class="wy-text-neutral">v0.6-rc0</b></h3>
+<h4 class="wy-text-neutral"><span class="fa fa-calendar wy-text-info"></span>&nbsp; Release Date:&nbsp; <b>April 24, 2022</b></h4>
 <a href="https://github.com/Breakthrough/PySceneDetect/releases/download/v0.6-dev2/PySceneDetect-0.6-dev2-win64-portable.zip" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Portable .zip</b></a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="../examples/usage/" class="btn btn-success" style="margin-bottom:8px;" role="button"><span class="fa fa-book"></span>&nbsp; <b>Getting Started</b></a>
 </div>
 
 ### Python Installer (All Platforms) &nbsp; <span class="wy-text-neutral"><span class="fa fa-windows"></span> &nbsp; <span class="fa fa-linux"></span> &nbsp; <span class="fa fa-apple"></span></span></h3>
 
 <div class="important">
-<h4 class="wy-text-neutral"><span class="fa fa-forward wy-text-info"></span> Latest Release: <b class="wy-text-neutral">v0.6-dev2</b></h4>
-<h4 class="wy-text-neutral"><span class="fa fa-calendar wy-text-info"></span>&nbsp; Release Date:&nbsp; <b>March 6, 2022</b></h4>
-<a href="https://github.com/Breakthrough/PySceneDetect/archive/v0.6-dev2.zip" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Source</b>&nbsp;&nbsp;.zip</a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="https://github.com/Breakthrough/PySceneDetect/archive/v0.6-dev2.tar.gz" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Source</b>&nbsp;&nbsp;.tar.gz</a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="../examples/usage/" class="btn btn-success" style="margin-bottom:8px;" role="button"><span class="fa fa-book"></span>&nbsp; <b>Getting Started</b></a>
+<h4 class="wy-text-neutral"><span class="fa fa-forward wy-text-info"></span> Latest Release: <b class="wy-text-neutral">v0.6-rc0</b></h4>
+<h4 class="wy-text-neutral"><span class="fa fa-calendar wy-text-info"></span>&nbsp; Release Date:&nbsp; <b>April 24, 2022</b></h4>
+<a href="https://github.com/Breakthrough/PySceneDetect/archive/v0.6-rc0.zip" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Source</b>&nbsp;&nbsp;.zip</a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="https://github.com/Breakthrough/PySceneDetect/archive/v0.6-rc0.tar.gz" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Source</b>&nbsp;&nbsp;.tar.gz</a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="../examples/usage/" class="btn btn-success" style="margin-bottom:8px;" role="button"><span class="fa fa-book"></span>&nbsp; <b>Getting Started</b></a>
 </div>
 
 To install from source, download and extract the latest release to a location of your choice, and make sure you have the appropriate [system requirements](#dependencies) installed before continuing.  PySceneDetect can be installed by running the following command in the location of the extracted files (don't forget `sudo` if you're installing system-wide):
 
 ```md
 python setup.py install
 ```
@@ -49,15 +49,15 @@
 
 ## Dependencies
 
 ### Python Packages
 
 PySceneDetect requires [Python 3](https://www.python.org/) and the following packages:
 
- - [OpenCV](http://opencv.org/) (compatible with 2/3), can install via `pip install opencv-python`. Used for video I/O.
+ - [OpenCV](http://opencv.org/) (compatible with 3/4), can install via `pip install opencv-python`. Used for video I/O.
  - [Numpy](https://numpy.org/), can install via `pip install numpy`. Used for frame processing.
  - [Click](https://click.palletsprojects.com), can install via `pip install Click`. Used for command line interface.
  - [tqdm](https://github.com/tqdm/tqdm), can install via `pip install tqdm`. Used to show progress bar and estimated time remaining.
  - [appdirs](https://github.com/ActiveState/appdirs), can install via `pip install appdirs`. Used to obtain path correct configuration file path for each platform.
 
 ### Video Splitting Tools
```

#### html2text {}

```diff
@@ -9,20 +9,20 @@
 *** Including Headless OpenCV : ***
 **** pip install --pre scenedetect[opencv-headless] ****
 PySceneDetect is available via `pip` as [the `scenedetect` package](https://
 pypi.org/project/scenedetect/). See below for instructions on installing a non-
 pip version of OpenCV. To ensure you have all the requirements installed, open
 a `python` interpreter, and ensure you can run `import cv2` without any errors.
 ### Windows Build (64-bit Only)  
-**** Latest Release: v0.6-dev2 ****
-***   Release Date:  March 6, 2022 ***
+**** Latest Release: v0.6-rc0 ****
+***   Release Date:  April 24, 2022 ***
  _Portable_.zip       _Getting_Started
 ### Python Installer (All Platforms)        
-*** Latest Release: v0.6-dev2 ***
-***   Release Date:  March 6, 2022 ***
+*** Latest Release: v0.6-rc0 ***
+***   Release Date:  April 24, 2022 ***
  _Source  .zip       _Source  .tar.gz       _Getting_Started
 To install from source, download and extract the latest release to a location
 of your choice, and make sure you have the appropriate [system requirements]
 (#dependencies) installed before continuing. PySceneDetect can be installed by
 running the following command in the location of the extracted files (don't
 forget `sudo` if you're installing system-wide): ```md python setup.py install
 ``` ### Post Installation After installation, you can call PySceneDetect from
@@ -34,15 +34,15 @@
 listed in the System Requirements section above (you should be able to `import
 numpy` and `import cv2`). If you encounter any issues or want to make a feature
 request, feel free to [report any bugs or share some feature requests/ideas]
 (contributing.md) on the [issue tracker](https://github.com/Breakthrough/
 PySceneDetect/issues) and help make PySceneDetect even better. ## Dependencies
 ### Python Packages PySceneDetect requires [Python 3](https://www.python.org/
 ) and the following packages: - [OpenCV](http://opencv.org/) (compatible with
-2/3), can install via `pip install opencv-python`. Used for video I/O. -
+3/4), can install via `pip install opencv-python`. Used for video I/O. -
 [Numpy](https://numpy.org/), can install via `pip install numpy`. Used for
 frame processing. - [Click](https://click.palletsprojects.com), can install via
 `pip install Click`. Used for command line interface. - [tqdm](https://
 github.com/tqdm/tqdm), can install via `pip install tqdm`. Used to show
 progress bar and estimated time remaining. - [appdirs](https://github.com/
 ActiveState/appdirs), can install via `pip install appdirs`. Used to obtain
 path correct configuration file path for each platform. ### Video Splitting
```

### Comparing `scenedetect-0.6.dev3/docs/examples/usage.md` & `scenedetect-0.6rc0/docs/examples/usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 You can also print the usage/help manual of PySceneDetect with the `help` command:
 
 ```rst
 scenedetect help
 ```
 
 <div class="important">
-The complete PySceneDetect Command-Line Interface (CLI) Reference <span class="fa fa-book"> can be found in the <a href="http://manual.scenedetect.com/en/v0.6/" alt="Manual Link">PySceneDetect Manual</a>, located at <a href="http://manual.scenedetect.com/0.6-dev2/" alt="Manual Link">manual.scenedetect.com/0.6-dev2/</a>.
+The complete PySceneDetect Command-Line Interface (CLI) Reference <span class="fa fa-book"> can be found in the <a href="http://manual.scenedetect.com/en/v0.6/" alt="Manual Link">PySceneDetect Manual</a>, located at <a href="http://manual.scenedetect.com/en/v0.6/" alt="Manual Link">manual.scenedetect.com/en/v0.6/</a>.
 </div>
 
 
 ## Quick Example
 
 
 Split the input video wherever a new scene is detected:
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
  # PySceneDetect Command-Line Usage This page outlines the most commonly used
 command-line options for using PySceneDetect. Basic usage of PySceneDetect
 (`scenedetect`) is: ```rst scenedetect [global options] [commands + command
 options] ``` You can also print the usage/help manual of PySceneDetect with the
 `help` command: ```rst scenedetect help ```
 The complete PySceneDetect Command-Line Interface (CLI) Reference  can be found
-in the PySceneDetect_Manual, located at manual.scenedetect.com/0.6-dev2/.
+in the PySceneDetect_Manual, located at manual.scenedetect.com/en/v0.6/.
 ## Quick Example Split the input video wherever a new scene is detected: ```rst
 scenedetect -i video.mp4 detect-content split-video ``` Print a table of
 detected scenes to the terminal, and save an image at the start, middle, and
 end frame of each scene: ```rst scenedetect -i video.mp4 detect-content list-
 scenes -n save-images ``` Skip the first 10 seconds of the input video: ```rst
 scenedetect -i video.mp4 time -s 10s detect-content ``` There are many other
 options and commands. To show a summary of available options/arguments, and a
```

### Comparing `scenedetect-0.6.dev3/docs/faq.md` & `scenedetect-0.6rc0/docs/faq.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 Unlike calling `pip install opencv-python`, the above commands will download and install the correct OpenCV version based on the Python version you are running.
 
 
 #### How can I enable video splitting support?
 
-To enable video splitting support, you will also need to have `mkvmerge` or `ffmpeg` installed on your system. See the documentation on [Video Splitting Support](https://scenedetect.com/examples/video-splitting/) after installation for details.
+To enable video splitting support, you will also need to have `mkvmerge` or `ffmpeg` installed on your system. See the documentation on [Video Splitting Support](https://scenedetect.com/en/v0.6/examples/video-splitting/) after installation for details.
 
 
 #### How can I fix the error `Cannot split video due to too many scenes`?
 
 This error occurs on Windows platforms specifically when the number of detected scenes is too large.  This is because PySceneDetect internally invokes other commands, such as those used for the `split-video` command.
 
 You can get around this issue by simply invoking those tools manually, using a smaller sub-set of scenes (or splitting the scene list into multiple parts).  You can obtain a comma-separated list of timecodes by using the `list-scenes` command.
```

### Comparing `scenedetect-0.6.dev3/docs/features.md` & `scenedetect-0.6rc0/docs/features.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/img/goldeneye-stats.png` & `scenedetect-0.6rc0/docs/img/goldeneye-stats.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/img/params.png` & `scenedetect-0.6rc0/docs/img/params.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/img/pyscenedetect_logo.png` & `scenedetect-0.6rc0/docs/img/pyscenedetect_logo.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/img/pyscenedetect_logo_small.png` & `scenedetect-0.6rc0/docs/img/pyscenedetect_logo_small.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/index.md` & `scenedetect-0.6rc0/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 <img alt="PySceneDetect" src="img/pyscenedetect_logo_small.png" />
 <h4 class="wy-text-info">Intelligent scene cut detection and video splitting tool.</h4>
 
 <div class="important">
-<h3 class="wy-text-neutral"><span class="fa fa-info-circle wy-text-info"></span>&nbsp; Latest Release: <b>v0.6-dev2</b> (March 6, 2022)</h3>
+<h3 class="wy-text-neutral"><span class="fa fa-info-circle wy-text-info"></span>&nbsp; Latest Release: <b>v0.6-rc0</b> (April 24, 2022)</h3>
 <a href="download/" class="btn btn-success" style="margin-bottom:8px;" role="button"><span class="fa fa-download"></span>&nbsp; <b>Download</b></a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="changelog/" class="btn btn-info" style="margin-bottom:8px;" role="button"><span class="fa fa-reorder"></span>&nbsp; <b>Changelog</b></a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="http://pyscenedetect-manual.readthedocs.io/en/v0.6/" class="btn btn-warning" style="margin-bottom:8px;" role="button"><span class="fa fa-gear"></span>&nbsp; <b>Manual</b></a> &nbsp;&nbsp;&nbsp;&nbsp; <a href="examples/usage-example/" class="btn btn-danger" style="margin-bottom:8px;" role="button"><span class="fa fa-book"></span>&nbsp; <b>Getting Started</b></a>
 <br/>
 See the changelog for the latest release notes and known issues.
 </div>
 
 **PySceneDetect** is a command-line application and a Python library for **detecting shot changes in videos** ([example](examples/usage-example.md)), and **automatically splitting the video into separate clips**.  Not only is it free and open-source software (FOSS), but there are several detection methods available ([see Features](features.md)), from simple threshold-based fade in/out detection, to advanced content aware fast-cut detection of each shot.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
  [PySceneDetect]
 *** Intelligent scene cut detection and video splitting tool. ***
-****   Latest Release: v0.6-dev2 (March 6, 2022) ****
+****   Latest Release: v0.6-rc0 (April 24, 2022) ****
  _Download       _Changelog       _Manual       _Getting_Started
 See the changelog for the latest release notes and known issues.
 **PySceneDetect** is a command-line application and a Python library for
 **detecting shot changes in videos** ([example](examples/usage-example.md)),
 and **automatically splitting the video into separate clips**. Not only is it
 free and open-source software (FOSS), but there are several detection methods
 available ([see Features](features.md)), from simple threshold-based fade in/
```

### Comparing `scenedetect-0.6.dev3/docs/other/copyright.md` & `scenedetect-0.6rc0/docs/other/copyright.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/other/literature.md` & `scenedetect-0.6rc0/docs/other/literature.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/other/similar.md` & `scenedetect-0.6rc0/docs/other/similar.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/reference/config.md` & `scenedetect-0.6rc0/docs/reference/config.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/reference/detection-methods.md` & `scenedetect-0.6rc0/docs/reference/detection-methods.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/reference/video-splitting.md` & `scenedetect-0.6rc0/docs/reference/video-splitting.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/docs/supporting.md` & `scenedetect-0.6rc0/docs/supporting.md`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/Makefile` & `scenedetect-0.6rc0/manual/Makefile`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/_static/pyscenedetect_logo.png` & `scenedetect-0.6rc0/manual/_static/pyscenedetect_logo.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/_static/pyscenedetect_logo_small.png` & `scenedetect-0.6rc0/manual/_static/pyscenedetect_logo_small.png`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/api/backends.rst` & `scenedetect-0.6rc0/manual/api/backends.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 .. _scenedetect-backends:
 
 ----------------------------------------
-VideoStream Backends
+Backends
 ----------------------------------------
 
 .. automodule:: scenedetect.backends
    :members:
    :undoc-members:
 
 
@@ -22,8 +22,7 @@
 =========================================
 PyAV
 =========================================
 
 .. automodule:: scenedetect.backends.pyav
    :members:
    :undoc-members:
-
```

### Comparing `scenedetect-0.6.dev3/manual/api/detectors.rst` & `scenedetect-0.6rc0/manual/api/detectors.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/api/frame_timecode.rst` & `scenedetect-0.6rc0/manual/api/frame_timecode.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/api/migration_guide.rst` & `scenedetect-0.6rc0/manual/api/migration_guide.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 
 .. _scenedetect-migration_guide:
 
 ---------------------------------------------------------------
 Migration Guide
 ---------------------------------------------------------------
 
-This page details how to transition a program written using PySceneDetect v0.5 to the new v0.6 API. It is recommended to review the new :ref:`Quickstart <scenedetect-quickstart>` and :ref:`Example <scenedetect-detailed_example>` sections first, as they should cover the majority of use cases. Also see `tests/test_api.py <https://github.com/Breakthrough/PySceneDetect/blob/v0.6/tests/test_api.py>` for a set of demonstrations covering many high level use cases.
+This page details how to transition a program written using PySceneDetect v0.5 to the new v0.6 API. It is recommended to review the new :ref:`Quickstart <scenedetect-quickstart>` and :ref:`Example <scenedetect-detailed_example>` sections first, as they should cover the majority of use cases. Also see `tests/test_api.py <https://github.com/Breakthrough/PySceneDetect/blob/v0.6/tests/test_api.py>`_ for a set of demonstrations covering many high level use cases.
 
-PySceneDetect v0.6 is a major step towards a more stable and simplified API.  The biggest change to most existing workflows is how video input is handled, and that Python 3.6 or above is now required.
+PySceneDetect v0.6 is a major step towards a more stable and simplified API.  The biggest change to existing workflows is how video input is handled, and that Python 3.6 or above is now required.
 
-This page covers the most commonly used APIs which require updates to work with v0.6.  Note that this page is not an exhaustive set of changes.  For a complete list of breaking API changes, see `the changelog <https://scenedetect.com/changelog/>`_.
+This page covers commonly used APIs which require updates to work with v0.6.  Note that this page is not an exhaustive set of changes.  For a complete list of breaking API changes, see `the changelog <https://scenedetect.com/changelog/>`_.
+
+In some places, a backwards compatibility layer has been added to avoid breaking most applications upon release. This should not be relied upon, and will be removed in the future. You can call ``scenedetect.platform.init_logger(show_stdout=True)`` or attach a custom log handler to the ``'pyscenedetect'`` logger to help find these cases.
 
 
 ===============================================================
 `VideoManager` Class
 ===============================================================
 
-`VideoManager` has been removed and placed with :py:mod:`scenedetect.backends`.  For most applications, the easiest way to update this is to use the :py:func:`open_video <scenedetect.backends.open_video>` function:
+`VideoManager` has been deprecated and replaced with :py:mod:`scenedetect.backends`.  For most applications, the :py:func:`open_video <scenedetect.open_video>` function should be used instead:
 
 .. code:: python
 
     from scenedetect import open_video
     video = open_video(video.mp4')
 
 The resulting object can then be passed to a :py:class:`SceneManager <scenedetect.scene_manager.SceneManager>` when calling :py:meth:`detect_scenes <scenedetect.scene_manager.SceneManager.detect_scenes>`, or any other function/method that used to take a `VideoManager`, e.g.:
@@ -30,15 +32,15 @@
     from scenedetect import open_video, SceneManager, ContentDetector
     video = open_video('video.mp4')
     scene_manager = SceneManager()
     scene_manager.add_detector(ContentDetector(threshold=threshold))
     scene_manager.detect_scenes(video)
     print(scene_manager.get_scene_list())
 
-See :py:mod:`scenedetect.backends` for examples of how to create specific backends. Note that where previously a list of paths was accepted, now only a single string should be provided.
+See :py:mod:`scenedetect.backends` for examples of how to create specific backends.  Where previously a list of paths was accepted, now only a single string should be provided.
 
 
 Seeking and Start/End Times
 ===============================================================
 
 Instead of setting the start time via the `VideoManager`, now :py:meth:`seek <scenedetect.video_stream.VideoStream.seek>` to the starting time on the :py:class:`VideoStream <scenedetect.video_stream.VideoStream>` object.
 
@@ -76,15 +78,15 @@
 The `downscale_factor` parameter has been removed from :py:func:`save_images <scenedetect.scene_manager.save_images>` (use the `scale` parameter instead). To achieve the same result as the previous version, set `scale` to `1.0 / downscale_factor`.
 
 
 ===============================================================
 `split_video_*` Functions
 ===============================================================
 
-The the :py:mod:`scenedetect.video_splitter` functions :py:func:`split_video_ffmpeg <scenedetect.video_splitter.split_video_ffmpeg>` and :py:func:`split_video_mkvmerge <scenedetect.video_splitter.split_video_mkvmerge>` now only accept a single path as the input (first) argument, where previously it was required to be a list.
+The the :py:mod:`scenedetect.video_splitter` functions :py:func:`split_video_ffmpeg <scenedetect.video_splitter.split_video_ffmpeg>` and :py:func:`split_video_mkvmerge <scenedetect.video_splitter.split_video_mkvmerge>` now only accept a single path as the input (first) argument.
 
 The `suppress_output` and `hide_progress` arguments to the :py:func:`split_video_ffmpeg <scenedetect.video_splitter.split_video_ffmpeg>` and :py:func:`split_video_mkvmerge <scenedetect.video_splitter.split_video_mkvmerge>` have been removed, and two new options have been added:
 
  * `suppress_output` is now `show_output`, default is `False`
  * `hide_progress` is now `show_progress`, default is `False`
 
 This makes the API consistent with that of :py:class:`SceneManager <scenedetect.scene_manager.SceneManager>`.
```

### Comparing `scenedetect-0.6.dev3/manual/api/scene_manager.rst` & `scenedetect-0.6rc0/manual/api/scene_manager.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 =======================================================================
 Usage Example
 =======================================================================
 
 In the code example below, we create a function ``find_scenes()`` which performs the following actions:
 
- * loads a video file by path (`str`) using :py:func:`scenedetect.backends.open_video`
+ * loads a video file by path (`str`) using :py:func:`scenedetect.open_video`
  * loads/saves a stats file for the video to ``{video_path}.stats.csv`` using a :py:class:`StatsManager <scenedetect.stats_manager.StatsManager>`
  * performs content-aware scene detection on the video using a :py:class:`ContentDetector <scenedetect.detectors.content_detector.ContentDetector>` bound to a :py:class:`SceneManager`
  * ``print()`` out a table of detected scenes to the terminal/console
  * returns a list of tuples of :py:class:`FrameTimecode <scenedetect.frame_timecode.FrameTimecode>` objects of the start and end times for each detected scene
 
 This example is a modified version of `the api_test.py file <https://github.com/Breakthrough/PySceneDetect/blob/master/tests/test_api.py>`_, and shows complete usage of a :py:class:`SceneManager <scenedetect.scene_manager.SceneManager>` object to perform content-aware scene detection using the :py:class:`ContentDetector <scenedetect.detectors.content_detector.ContentDetector>`, printing a list of scenes, then saving the calculated per-frame metrics to disk:
 
@@ -29,15 +29,15 @@
     import os
 
     from scenedetect import open_video, ContentDetector, SceneManager, StatsManager
 
     def find_scenes(video_path):
         # type: (str) -> List[Tuple[FrameTimecode, FrameTimecode]]
 
-        video_stream = open_video(path=video_path)
+        video_stream = open_video(video_path)
         stats_manager = StatsManager()
         # Construct our SceneManager and pass it our StatsManager.
         scene_manager = SceneManager(stats_manager)
 
         # Add ContentDetector algorithm (each detector's constructor
         # takes various options, e.g. threshold).
         scene_manager.add_detector(ContentDetector())
@@ -52,15 +52,15 @@
             print(
                 'Scene %2d: Start %s / Frame %d, End %s / Frame %d' % (
                 i+1,
                 scene[0].get_timecode(), scene[0].get_frames(),
                 scene[1].get_timecode(), scene[1].get_frames(),))
 
         # Store the frame metrics we calculated for the next time the program runs.
-        stats_manager.save_to_csv(path=stats_file_path, base_timecode=base_timecode)
+        stats_manager.save_to_csv(csv_file=stats_file_path, base_timecode=base_timecode)
 
         return scene_list
 
 The statsfile can be used to find a better threshold for certain inputs, or perform further statistical analysis.  The use of a :py:class:`StatsManager <scenedetect.stats_manager.StatsManager>` also allows certain detectors to operate faster on subsequent passes by caching calculations.  Statsfiles can be persisted on disk and loaded again, which helps avoid unnecessary calculations in applications where multiple passes are expected (e.g. interactively selecting a threshold).
 
 
 =======================================================================
```

### Comparing `scenedetect-0.6.dev3/manual/api/stats_manager.rst` & `scenedetect-0.6rc0/manual/api/stats_manager.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/api/video_stream.rst` & `scenedetect-0.6rc0/manual/api/video_stream.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/api.rst` & `scenedetect-0.6rc0/manual/api.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
       class for storing, converting, and performing arithmetic on timecodes
       with frame-accurate precision.
 
     * :ref:`scenedetect.scene_detector 🌐 <scenedetect-scene_detector>`: Contains :py:class:`SceneDetector <scenedetect.scene_detector.SceneDetector>` base class for implementing scene detection algorithms.
 
     * :ref:`scenedetect.stats_manager 🧮 <scenedetect-stats_manager>`: Contains :py:class:`StatsManager <scenedetect.stats_manager.StatsManager>` class for caching frame metrics and loading/saving them to disk in CSV format for analysis. Also used as a persistent cache to make multiple passes on the same video significantly faster.
 
+    * :ref:`scenedetect.platform 🐱‍💻 <scenedetect-platform>`: Logging and utility functions.
+
 
 Most types/functions are also available directly from the `scenedetect` package to make imports simpler.
 
 .. note::
 
     The PySceneDetect API is still under development. It is recommended that you pin the `scenedetect` version in your requirements to below the next major release:
 
@@ -76,15 +78,17 @@
 
 .. code:: python
 
     from scenedetect import detect, ContentDetector, split_video_ffmpeg
     scene_list = detect('my_video.mp4', ContentDetector())
     split_video_ffmpeg('my_video.mp4', scene_list)
 
-This is just a small snippet of what PySceneDetect offers. The library is very modular, and can integrate with most application workflows easily. In the next example, we show how the various library components can be used to create a more customizable scene cut/shot detection pipeline.  In addition, demonstrations of common use cases can be found in the `tests/test_api.py <https://github.com/Breakthrough/PySceneDetect/blob/v0.6/tests/test_api.py>`_ file.
+This is just a small snippet of what PySceneDetect offers. The library is very modular, and can integrate with most application workflows easily.
+
+In the next example, we show how the library components can be used to create a more customizable scene cut/shot detection pipeline.  Additional demonstrations/recipes can be found in the `tests/test_api.py <https://github.com/Breakthrough/PySceneDetect/blob/v0.6/tests/test_api.py>`_ file.
 
 
 .. _scenedetect-detailed_example:
 
 =======================================================================
 Example
 =======================================================================
@@ -120,8 +124,23 @@
 PySceneDetect v0.6 introduces several breaking changes which are incompatible with v0.5. See :ref:`Migration Guide <scenedetect-migration_guide>` for details on how to update your application. In addition, demonstrations of common use cases can be found in the `tests/test_api.py <https://github.com/Breakthrough/PySceneDetect/blob/v0.6/tests/test_api.py>`_ file.
 
 
 =======================================================================
 Module-Level Functions
 =======================================================================
 
+
+`detect`
+===============================================================
+
 .. autofunction:: scenedetect.detect
+
+`open_video`
+===============================================================
+.. autofunction:: scenedetect.open_video
+
+
+=======================================================================
+Logging
+=======================================================================
+
+PySceneDetect outputs messages to a logger named ``pyscenedetect`` which does not have any default handlers. You can use :py:func:`scenedetect.init_logger <scenedetect.platform.init_logger>` with ``show_stdout=True`` or specify a log file (verbosity can also be specified) to attach some common handlers, or use ``logging.getLogger('pyscenedetect')`` and attach log handlers manually.
```

### Comparing `scenedetect-0.6.dev3/manual/cli/commands.rst` & `scenedetect-0.6rc0/manual/cli/commands.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/cli/config_file.rst` & `scenedetect-0.6rc0/manual/cli/config_file.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,144 @@
-00000000: 0d0a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ..**************
-00000010: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000020: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000000: 0d0a 2e2e 205f 7363 656e 6564 6574 6563  .... _scenedetec
+00000010: 745f 636c 692d 636f 6e66 6967 5f66 696c  t_cli-config_fil
+00000020: 653a 0d0a 0d0a 2a2a 2a2a 2a2a 2a2a 2a2a  e:....**********
 00000030: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000040: 2a2a 2a2a 2a2a 2a2a 2a0d 0a43 6f6e 6669  *********..Confi
-00000050: 6775 7261 7469 6f6e 2046 696c 650d 0a2a  guration File..*
-00000060: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000070: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-00000080: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000040: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000050: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+00000060: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0d 0a43  *************..C
+00000070: 6f6e 6669 6775 7261 7469 6f6e 2046 696c  onfiguration Fil
+00000080: 650d 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  e..*************
 00000090: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
-000000a0: 2a2a 2a2a 2a2a 0d0a 0d0a 4d6f 7374 2063  ******....Most c
-000000b0: 6f6d 6d61 6e64 206c 696e 6520 7061 7261  ommand line para
-000000c0: 6d65 7465 7273 2063 616e 2062 6520 7365  meters can be se
-000000d0: 7420 7573 696e 6720 6120 636f 6e66 6967  t using a config
-000000e0: 7572 6174 696f 6e20 6669 6c65 2e20 6043  uration file. `C
-000000f0: 6c69 636b 2068 6572 6520 746f 2064 6f77  lick here to dow
-00000100: 6e6c 6f61 6420 6120 7363 656e 6564 6574  nload a scenedet
-00000110: 6563 742e 6366 6720 6669 6c65 2074 656d  ect.cfg file tem
-00000120: 706c 6174 6520 3c68 7474 7073 3a2f 2f72  plate <https://r
-00000130: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000140: 7465 6e74 2e63 6f6d 2f42 7265 616b 7468  tent.com/Breakth
-00000150: 726f 7567 682f 5079 5363 656e 6544 6574  rough/PySceneDet
-00000160: 6563 742f 7630 2e36 2f73 6365 6e65 6465  ect/v0.6/scenede
-00000170: 7465 6374 2e63 6667 3e60 5f20 636f 6e74  tect.cfg>`_ cont
-00000180: 6169 6e69 6e67 2065 7665 7279 2070 6f73  aining every pos
-00000190: 7369 626c 6520 6f70 7469 6f6e 2c20 616c  sible option, al
-000001a0: 6f6e 6720 7769 7468 2063 6f6d 6d65 6e74  ong with comment
-000001b0: 7320 7468 6174 2064 6573 6372 6962 6520  s that describe 
-000001c0: 6561 6368 206f 6e65 2c20 6f72 2073 6565  each one, or see
-000001d0: 2074 6865 2063 6f6d 706c 6574 6520 636f   the complete co
-000001e0: 6e66 6967 206f 7074 696f 6e20 6c69 7374  nfig option list
-000001f0: 696e 6720 6265 6c6f 772e 204e 6f74 6520  ing below. Note 
-00000200: 7468 6174 206c 696e 6573 2073 7461 7274  that lines start
-00000210: 696e 6720 7769 7468 2061 2060 6023 6060  ing with a ``#``
-00000220: 2061 7265 2063 6f6d 6d65 6e74 7320 616e   are comments an
-00000230: 6420 7769 6c6c 2062 6520 6967 6e6f 7265  d will be ignore
-00000240: 642e 2020 5468 6520 7363 656e 6564 6574  d.  The scenedet
-00000250: 6563 742e 6366 6720 7465 6d70 6c61 7465  ect.cfg template
-00000260: 2066 696c 6520 6973 2061 6c73 6f20 6176   file is also av
-00000270: 6169 6c61 626c 6520 696e 2074 6865 2066  ailable in the f
-00000280: 6f6c 6465 7220 7768 6572 6520 5079 5363  older where PySc
-00000290: 656e 6544 6574 6563 7420 6973 2069 6e73  eneDetect is ins
-000002a0: 7461 6c6c 6564 2e0d 0a0d 0a41 2063 6f6e  talled.....A con
-000002b0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-000002c0: 7061 7468 2063 616e 2062 6520 7370 6563  path can be spec
-000002d0: 6966 6965 6420 7573 696e 6720 7468 6520  ified using the 
-000002e0: 6060 2d63 6060 2f60 602d 2d63 6f6e 6669  ``-c``/``--confi
-000002f0: 6760 6020 6172 6775 6d65 6e74 2e20 5079  g`` argument. Py
-00000300: 5363 656e 6544 6574 6563 7420 616c 736f  SceneDetect also
-00000310: 206c 6f6f 6b73 2066 6f72 2061 2063 6f6e   looks for a con
-00000320: 6669 6720 6669 6c65 206e 616d 6564 2073  fig file named s
-00000330: 6365 6e65 6465 7465 6374 2e63 6667 2069  cenedetect.cfg i
-00000340: 6e20 6f6e 6520 6f66 2074 6865 2066 6f6c  n one of the fol
-00000350: 6c6f 7769 6e67 206c 6f63 6174 696f 6e73  lowing locations
-00000360: 3a0d 0a0d 0a20 2a20 5769 6e64 6f77 733a  :.... * Windows:
-00000370: 0d0a 2020 2020 202a 2060 6043 3a2f 5573  ..     * ``C:/Us
-00000380: 6572 732f 2555 5345 524e 414d 4525 2f41  ers/%USERNAME%/A
-00000390: 7070 4461 7461 2f4c 6f63 616c 2f50 7953  ppData/Local/PyS
-000003a0: 6365 6e65 4465 7465 6374 2f73 6365 6e65  ceneDetect/scene
-000003b0: 6465 7465 6374 2e63 6667 6060 0d0a 0d0a  detect.cfg``....
-000003c0: 202a 204c 696e 7578 3a0d 0a20 2020 2020   * Linux:..     
-000003d0: 2a20 6060 7e2f 2e63 6f6e 6669 672f 5079  * ``~/.config/Py
-000003e0: 5363 656e 6544 6574 6563 742f 7363 656e  SceneDetect/scen
-000003f0: 6564 6574 6563 742e 6366 6760 600d 0a20  edetect.cfg``.. 
-00000400: 2020 2020 2a20 6060 2458 4447 5f43 4f4e      * ``$XDG_CON
-00000410: 4649 475f 484f 4d45 2f73 6365 6e65 6465  FIG_HOME/scenede
-00000420: 7465 6374 2e63 6667 6060 0d0a 0d0a 202a  tect.cfg``.... *
-00000430: 204d 6163 3a0d 0a20 2020 2020 2a20 6060   Mac:..     * ``
-00000440: 7e2f 4c69 6272 6172 792f 5072 6566 6572  ~/Library/Prefer
-00000450: 656e 6365 732f 5079 5363 656e 6544 6574  ences/PySceneDet
-00000460: 6563 742f 7363 656e 6564 6574 6563 742e  ect/scenedetect.
-00000470: 6366 6760 600d 0a0d 0a52 756e 2060 7363  cfg``....Run `sc
-00000480: 656e 6564 6574 6563 7420 6865 6c70 6020  enedetect help` 
-00000490: 746f 2073 6565 2074 6865 2065 7861 6374  to see the exact
-000004a0: 2070 6174 6820 6f6e 2079 6f75 7220 7379   path on your sy
-000004b0: 7374 656d 2077 6869 6368 2077 696c 6c20  stem which will 
-000004c0: 6265 2075 7365 6420 2869 7420 7769 6c6c  be used (it will
-000004d0: 2062 6520 6c69 7374 6564 2075 6e64 6572   be listed under
-000004e0: 2074 6865 2068 656c 7020 7465 7874 2066   the help text f
-000004f0: 6f72 2074 6865 2060 602d 6360 602f 6060  or the ``-c``/``
-00000500: 2d2d 636f 6e66 6967 6060 206f 7074 696f  --config`` optio
-00000510: 6e29 2e20 596f 7520 6361 6e20 7269 6768  n). You can righ
-00000520: 742d 636c 6963 6b20 616e 6420 7361 7665  t-click and save
-00000530: 2074 6865 2061 626f 7665 2073 6365 6e65   the above scene
-00000540: 6465 7465 6374 2e63 6667 2074 656d 706c  detect.cfg templ
-00000550: 6174 6520 696e 746f 206f 6e65 206f 6620  ate into one of 
-00000560: 7468 6573 6520 6c6f 6361 7469 6f6e 7320  these locations 
-00000570: 746f 2067 6574 2073 7461 7274 6564 2e0d  to get started..
-00000580: 0a0d 0a53 7065 6369 6679 696e 6720 6120  ...Specifying a 
-00000590: 636f 6e66 6967 2066 696c 6520 7061 7468  config file path
-000005a0: 2075 7369 6e67 2060 602d 6360 602f 6060   using ``-c``/``
-000005b0: 2d2d 636f 6e66 6967 6060 206f 7665 7272  --config`` overr
-000005c0: 6964 6573 2074 6865 2075 7365 7220 636f  ides the user co
-000005d0: 6e66 6967 2066 696c 652e 2053 7065 6369  nfig file. Speci
-000005e0: 6679 696e 6720 7661 6c75 6573 206f 6e20  fying values on 
-000005f0: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
-00000600: 2077 696c 6c20 6f76 6572 7269 6465 2074   will override t
-00000610: 686f 7365 2076 616c 7565 7320 696e 2074  hose values in t
-00000620: 6865 2063 6f6e 6669 6720 6669 6c65 2e0d  he config file..
-00000630: 0a0d 0a54 6865 2073 796e 7461 7820 6f66  ...The syntax of
-00000640: 2061 2063 6f6e 6669 6775 7261 7469 6f6e   a configuration
-00000650: 2066 696c 6520 6973 3a0d 0a0d 0a2e 2e20   file is:...... 
-00000660: 636f 6465 3a3a 2069 6e69 0d0a 0d0a 2020  code:: ini....  
-00000670: 2020 5b63 6f6d 6d61 6e64 5d0d 0a20 2020    [command]..   
-00000680: 206f 7074 696f 6e5f 6120 3d20 7661 6c75   option_a = valu
-00000690: 650d 0a20 2020 2023 636f 6d6d 656e 740d  e..    #comment.
-000006a0: 0a20 2020 206f 7074 696f 6e5f 6220 3d20  .    option_b = 
-000006b0: 310d 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  1....===========
-000006c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000006f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 4578  ============..Ex
-00000700: 616d 706c 650d 0a3d 3d3d 3d3d 3d3d 3d3d  ample..=========
-00000710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000000a0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000000b0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000000c0: 2a2a 2a2a 2a2a 2a2a 2a2a 0d0a 0d0a 4d6f  **********....Mo
+000000d0: 7374 2063 6f6d 6d61 6e64 206c 696e 6520  st command line 
+000000e0: 7061 7261 6d65 7465 7273 2063 616e 2062  parameters can b
+000000f0: 6520 7365 7420 7573 696e 6720 6120 636f  e set using a co
+00000100: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00000110: 2e20 5365 6520 7468 6520 3a72 6566 3a60  . See the :ref:`
+00000120: 5465 6d70 6c61 7465 203c 636f 6e66 6967  Template <config
+00000130: 5f66 696c 6520 5465 6d70 6c61 7465 3e60  _file Template>`
+00000140: 2062 656c 6f77 2066 6f72 2061 6e20 6578   below for an ex
+00000150: 616d 706c 6520 6060 7363 656e 6564 6574  ample ``scenedet
+00000160: 6563 742e 6366 6760 6020 6669 6c65 2063  ect.cfg`` file c
+00000170: 6f6e 7461 696e 696e 6720 6576 6572 7920  ontaining every 
+00000180: 706f 7373 6962 6c65 206f 7074 696f 6e2c  possible option,
+00000190: 2061 6c6f 6e67 2077 6974 6820 636f 6d6d   along with comm
+000001a0: 656e 7473 2074 6861 7420 6465 7363 7269  ents that descri
+000001b0: 6265 2065 6163 6820 6f6e 652e 2020 4e6f  be each one.  No
+000001c0: 7465 2074 6861 7420 6c69 6e65 7320 7374  te that lines st
+000001d0: 6172 7469 6e67 2077 6974 6820 6120 6060  arting with a ``
+000001e0: 2360 6020 6172 6520 636f 6d6d 656e 7473  #`` are comments
+000001f0: 2061 6e64 2077 696c 6c20 6265 2069 676e   and will be ign
+00000200: 6f72 6564 2e0d 0a0d 0a50 7953 6365 6e65  ored.....PyScene
+00000210: 4465 7465 6374 206c 6f6f 6b73 2066 6f72  Detect looks for
+00000220: 2061 2066 696c 6520 6e61 6d65 6420 6060   a file named ``
+00000230: 7363 656e 6564 6574 6563 742e 6366 6760  scenedetect.cfg`
+00000240: 6020 696e 206f 6e65 206f 6620 7468 6520  ` in one of the 
+00000250: 666f 6c6c 6f77 696e 6720 6c6f 6361 7469  following locati
+00000260: 6f6e 733a 0d0a 0d0a 202a 2057 696e 646f  ons:.... * Windo
+00000270: 7773 3a0d 0a20 2020 2020 2a20 6060 433a  ws:..     * ``C:
+00000280: 2f55 7365 7273 2f25 5553 4552 4e41 4d45  /Users/%USERNAME
+00000290: 252f 4170 7044 6174 612f 4c6f 6361 6c2f  %/AppData/Local/
+000002a0: 5079 5363 656e 6544 6574 6563 742f 7363  PySceneDetect/sc
+000002b0: 656e 6564 6574 6563 742e 6366 6760 600d  enedetect.cfg``.
+000002c0: 0a0d 0a20 2a20 4c69 6e75 783a 0d0a 2020  ... * Linux:..  
+000002d0: 2020 202a 2060 607e 2f2e 636f 6e66 6967     * ``~/.config
+000002e0: 2f50 7953 6365 6e65 4465 7465 6374 2f73  /PySceneDetect/s
+000002f0: 6365 6e65 6465 7465 6374 2e63 6667 6060  cenedetect.cfg``
+00000300: 0d0a 2020 2020 202a 2060 6024 5844 475f  ..     * ``$XDG_
+00000310: 434f 4e46 4947 5f48 4f4d 452f 7363 656e  CONFIG_HOME/scen
+00000320: 6564 6574 6563 742e 6366 6760 600d 0a0d  edetect.cfg``...
+00000330: 0a20 2a20 4d61 633a 0d0a 2020 2020 202a  . * Mac:..     *
+00000340: 2060 607e 2f4c 6962 7261 7279 2f50 7265   ``~/Library/Pre
+00000350: 6665 7265 6e63 6573 2f50 7953 6365 6e65  ferences/PyScene
+00000360: 4465 7465 6374 2f73 6365 6e65 6465 7465  Detect/scenedete
+00000370: 6374 2e63 6667 6060 0d0a 0d0a 5275 6e20  ct.cfg``....Run 
+00000380: 6073 6365 6e65 6465 7465 6374 2068 656c  `scenedetect hel
+00000390: 7060 2074 6f20 7365 6520 7468 6520 6578  p` to see the ex
+000003a0: 6163 7420 7061 7468 206f 6e20 796f 7572  act path on your
+000003b0: 2073 7973 7465 6d20 7768 6963 6820 7769   system which wi
+000003c0: 6c6c 2062 6520 7573 6564 2e20 596f 7520  ll be used. You 
+000003d0: 6361 6e20 616c 736f 2073 7065 6369 6679  can also specify
+000003e0: 2074 6865 2064 6972 6563 7420 7061 7468   the direct path
+000003f0: 2074 6f20 6120 636f 6e66 6967 2066 696c   to a config fil
+00000400: 6520 7573 696e 6720 7468 6520 6060 2d63  e using the ``-c
+00000410: 6060 2f60 602d 2d63 6f6e 6669 6760 6020  ``/``--config`` 
+00000420: 6172 6775 6d65 6e74 2e20 5661 6c75 6573  argument. Values
+00000430: 2073 6574 206f 6e20 7468 6520 636f 6d6d   set on the comm
+00000440: 616e 6420 6c69 6e65 2074 616b 6520 7072  and line take pr
+00000450: 6563 6564 656e 6365 206f 7665 7220 7468  ecedence over th
+00000460: 6f73 6520 7365 7420 696e 2074 6865 2063  ose set in the c
+00000470: 6f6e 6669 6720 6669 6c65 2e0d 0a0d 0a54  onfig file.....T
+00000480: 6865 2073 796e 7461 7820 6f66 2061 2063  he syntax of a c
+00000490: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+000004a0: 6520 6973 3a0d 0a0d 0a2e 2e20 636f 6465  e is:...... code
+000004b0: 3a3a 2069 6e69 0d0a 0d0a 2020 2020 5b63  :: ini....    [c
+000004c0: 6f6d 6d61 6e64 5d0d 0a20 2020 206f 7074  ommand]..    opt
+000004d0: 696f 6e5f 6120 3d20 7661 6c75 650d 0a20  ion_a = value.. 
+000004e0: 2020 2023 636f 6d6d 656e 740d 0a20 2020     #comment..   
+000004f0: 206f 7074 696f 6e5f 6220 3d20 310d 0a0d   option_b = 1...
+00000500: 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...=============
+00000510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000540: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 4578 616d  ==========..Exam
+00000550: 706c 650d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  ple..===========
+00000560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a  ============....
+000005a0: 2e2e 2063 6f64 653a 3a20 696e 690d 0a0d  .. code:: ini...
+000005b0: 0a20 2020 205b 676c 6f62 616c 5d0d 0a20  .    [global].. 
+000005c0: 2020 206d 696e 2d73 6365 6e65 2d6c 656e     min-scene-len
+000005d0: 203d 2030 2e38 730d 0a0d 0a20 2020 205b   = 0.8s....    [
+000005e0: 6465 7465 6374 2d63 6f6e 7465 6e74 5d0d  detect-content].
+000005f0: 0a20 2020 2074 6872 6573 686f 6c64 203d  .    threshold =
+00000600: 2032 360d 0a0d 0a20 2020 205b 7370 6c69   26....    [spli
+00000610: 742d 7669 6465 6f5d 0d0a 2020 2020 7072  t-video]..    pr
+00000620: 6573 6574 203d 2073 6c6f 770d 0a20 2020  eset = slow..   
+00000630: 2072 6174 652d 6661 6374 6f72 203d 2031   rate-factor = 1
+00000640: 370d 0a20 2020 2023 2044 6f6e 2774 206e  7..    # Don't n
+00000650: 6565 6420 746f 2075 7365 2071 756f 7465  eed to use quote
+00000660: 7320 6576 656e 2069 6620 6669 6c65 6e61  s even if filena
+00000670: 6d65 2063 6f6e 7461 696e 7320 7370 6163  me contains spac
+00000680: 6573 0d0a 2020 2020 6669 6c65 6e61 6d65  es..    filename
+00000690: 203d 2024 5649 4445 4f5f 4e41 4d45 2d43   = $VIDEO_NAME-C
+000006a0: 6c69 702d 2453 4345 4e45 5f4e 554d 4245  lip-$SCENE_NUMBE
+000006b0: 520d 0a0d 0a20 2020 205b 7361 7665 2d69  R....    [save-i
+000006c0: 6d61 6765 735d 0d0a 2020 2020 666f 726d  mages]..    form
+000006d0: 6174 203d 206a 7065 670d 0a20 2020 2071  at = jpeg..    q
+000006e0: 7561 6c69 7479 203d 2038 300d 0a20 2020  uality = 80..   
+000006f0: 206e 756d 2d69 6d61 6765 7320 3d20 330d   num-images = 3.
+00000700: 0a0d 0a0d 0a2e 2e20 5f63 6f6e 6669 675f  ....... _config_
+00000710: 6669 6c65 2054 656d 706c 6174 653a 0d0a  file Template:..
+00000720: 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ..==============
 00000730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
-00000750: 0d0a 2e2e 2063 6f64 653a 3a20 696e 690d  .... code:: ini.
-00000760: 0a0d 0a20 2020 205b 676c 6f62 616c 5d0d  ...    [global].
-00000770: 0a20 2020 206d 696e 2d73 6365 6e65 2d6c  .    min-scene-l
-00000780: 656e 203d 2030 2e38 730d 0a0d 0a20 2020  en = 0.8s....   
-00000790: 205b 6465 7465 6374 2d63 6f6e 7465 6e74   [detect-content
-000007a0: 5d0d 0a20 2020 2074 6872 6573 686f 6c64  ]..    threshold
-000007b0: 203d 2032 360d 0a0d 0a20 2020 205b 7370   = 26....    [sp
-000007c0: 6c69 742d 7669 6465 6f5d 0d0a 2020 2020  lit-video]..    
-000007d0: 7072 6573 6574 203d 2073 6c6f 770d 0a20  preset = slow.. 
-000007e0: 2020 2072 6174 652d 6661 6374 6f72 203d     rate-factor =
-000007f0: 2031 370d 0a20 2020 2023 2044 6f6e 2774   17..    # Don't
-00000800: 206e 6565 6420 746f 2075 7365 2071 756f   need to use quo
-00000810: 7465 7320 6576 656e 2069 6620 6669 6c65  tes even if file
-00000820: 6e61 6d65 2063 6f6e 7461 696e 7320 7370  name contains sp
-00000830: 6163 6573 0d0a 2020 2020 6669 6c65 6e61  aces..    filena
-00000840: 6d65 203d 2024 5649 4445 4f5f 4e41 4d45  me = $VIDEO_NAME
-00000850: 2d43 6c69 702d 2453 4345 4e45 5f4e 554d  -Clip-$SCENE_NUM
-00000860: 4245 520d 0a0d 0a20 2020 205b 7361 7665  BER....    [save
-00000870: 2d69 6d61 6765 735d 0d0a 2020 2020 666f  -images]..    fo
-00000880: 726d 6174 203d 206a 7065 670d 0a20 2020  rmat = jpeg..   
-00000890: 2071 7561 6c69 7479 203d 2038 300d 0a20   quality = 80.. 
-000008a0: 2020 206e 756d 2d69 6d61 6765 7320 3d20     num-images = 
-000008b0: 330d 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  3....===========
-000008c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000008d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000008e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000008f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 5465  ============..Te
-00000900: 6d70 6c61 7465 0d0a 3d3d 3d3d 3d3d 3d3d  mplate..========
-00000910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000940: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
-00000950: 0a0d 0a2e 2e20 6c69 7465 7261 6c69 6e63  ..... literalinc
-00000960: 6c75 6465 3a3a 202e 2e2f 2e2e 2f73 6365  lude:: ../../sce
-00000970: 6e65 6465 7465 6374 2e63 6667 0d0a 2020  nedetect.cfg..  
-00000980: 203a 6c61 6e67 7561 6765 3a20 696e 690d   :language: ini.
-00000990: 0a                                       .
+00000740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000750: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000760: 3d3d 3d3d 3d3d 3d3d 3d0d 0a54 656d 706c  =========..Templ
+00000770: 6174 650d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  ate..===========
+00000780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000007a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000007b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a  ============....
+000007c0: 5468 6973 2074 656d 706c 6174 6520 7368  This template sh
+000007d0: 6f77 7320 6576 6572 7920 706f 7373 6962  ows every possib
+000007e0: 6c65 2063 6f6e 6669 6775 7261 7469 6f6e  le configuration
+000007f0: 206f 7074 696f 6e20 616e 6420 6465 6661   option and defa
+00000800: 756c 7420 7661 6c75 6573 2e20 4974 2063  ult values. It c
+00000810: 616e 2062 6520 7573 6564 2061 7320 6120  an be used as a 
+00000820: 6060 7363 656e 6564 6574 6563 742e 6366  ``scenedetect.cf
+00000830: 6760 6020 6669 6c65 2e20 596f 7520 6361  g`` file. You ca
+00000840: 6e20 616c 736f 2060 646f 776e 6c6f 6164  n also `download
+00000850: 2069 7420 6672 6f6d 2047 6974 6875 6220   it from Github 
+00000860: 3c68 7474 7073 3a2f 2f72 6177 2e67 6974  <https://raw.git
+00000870: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000880: 6f6d 2f42 7265 616b 7468 726f 7567 682f  om/Breakthrough/
+00000890: 5079 5363 656e 6544 6574 6563 742f 7630  PySceneDetect/v0
+000008a0: 2e36 2f73 6365 6e65 6465 7465 6374 2e63  .6/scenedetect.c
+000008b0: 6667 3e60 5f2e 0d0a 0d0a 2e2e 206c 6974  fg>`_....... lit
+000008c0: 6572 616c 696e 636c 7564 653a 3a20 2e2e  eralinclude:: ..
+000008d0: 2f2e 2e2f 7363 656e 6564 6574 6563 742e  /../scenedetect.
+000008e0: 6366 670d 0a20 2020 3a6c 616e 6775 6167  cfg..   :languag
+000008f0: 653a 2069 6e69 0d0a                      e: ini..
```

### Comparing `scenedetect-0.6.dev3/manual/cli/detectors.rst` & `scenedetect-0.6rc0/manual/cli/detectors.rst`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/manual/cli/global_options.rst` & `scenedetect-0.6rc0/manual/cli/global_options.rst`

 * *Files 2% similar despite different names*

```diff
@@ -240,130 +240,138 @@
 00000ef0: 6365 6e65 7320 7368 6f72 7465 7220 7468  cenes shorter th
 00000f00: 616e 2060 6d69 6e2d 7363 656e 652d 6c65  an `min-scene-le
 00000f10: 6e60 0d0a 2020 2020 2020 2020 2020 2020  n`..            
 00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000f30: 2020 2020 696e 7374 6561 6420 6f66 2063      instead of c
 00000f40: 6f6d 6269 6e69 6e67 2074 6865 6d20 7769  ombining them wi
 00000f50: 7468 206e 6569 6768 626f 7273 2e0d 0a0d  th neighbors....
-00000f60: 0a20 202d 732c 202d 2d73 7461 7473 2043  .  -s, --stats C
-00000f70: 5356 2020 2020 2020 2020 2020 2020 2020  SV              
-00000f80: 2050 6174 6820 746f 2073 7461 7473 2066   Path to stats f
-00000f90: 696c 6520 282e 6373 7629 2066 6f72 2077  ile (.csv) for w
-00000fa0: 7269 7469 6e67 2066 7261 6d65 0d0a 2020  riting frame..  
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00000fd0: 7472 6963 7320 746f 2e20 4966 2074 6865  trics to. If the
-00000fe0: 2066 696c 6520 6578 6973 7473 2c20 616e   file exists, an
-00000ff0: 7920 6d65 7472 6963 730d 0a20 2020 2020  y metrics..     
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
-00001020: 6265 2070 726f 6365 7373 6564 2c20 6f74  be processed, ot
-00001030: 6865 7277 6973 6520 6120 6e65 7720 6669  herwise a new fi
-00001040: 6c65 2077 696c 6c0d 0a20 2020 2020 2020  le will..       
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 2020 2020 2020 2020 2062 6520 6372 6561           be crea
-00001070: 7465 642e 2043 616e 2062 6520 7573 6564  ted. Can be used
-00001080: 2074 6f20 6465 7465 726d 696e 6520 6f70   to determine op
-00001090: 7469 6d61 6c0d 0a20 2020 2020 2020 2020  timal..         
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2020 2076 616c 7565 7320 666f         values fo
-000010c0: 7220 7661 7269 6f75 7320 7363 656e 6520  r various scene 
-000010d0: 6465 7465 6374 6f72 206f 7074 696f 6e73  detector options
-000010e0: 2c20 616e 640d 0a20 2020 2020 2020 2020  , and..         
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 2074 6f20 6361 6368 6520         to cache 
-00001110: 6672 616d 6520 6361 6c63 756c 6174 696f  frame calculatio
-00001120: 6e73 2069 6e20 6f72 6465 7220 746f 2073  ns in order to s
-00001130: 7065 6564 0d0a 2020 2020 2020 2020 2020  peed..          
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 2020 2020 2020 7570 206d 756c 7469 706c        up multipl
-00001160: 6520 6465 7465 6374 696f 6e20 7275 6e73  e detection runs
-00001170: 2e0d 0a0d 0a20 202d 762c 202d 2d76 6572  .....  -v, --ver
-00001180: 626f 7369 7479 204c 4556 454c 2020 2020  bosity LEVEL    
-00001190: 2020 2020 204c 6576 656c 206f 6620 6465       Level of de
-000011a0: 6275 672f 696e 666f 2f65 7272 6f72 2069  bug/info/error i
-000011b0: 6e66 6f72 6d61 7469 6f6e 2074 6f20 7368  nformation to sh
-000011c0: 6f77 2e0d 0a20 2020 2020 2020 2020 2020  ow...           
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 2020 204d 7573 7420 6265 206f 6e65       Must be one
-000011f0: 206f 663a 2064 6562 7567 2c20 696e 666f   of: debug, info
-00001200: 2c20 7761 726e 696e 672c 2065 7272 6f72  , warning, error
-00001210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 206e 6f6e 652e 204f 7665 7272 6964     none. Overrid
-00001240: 6573 2060 2d71 602f 602d 2d71 7569 6574  es `-q`/`--quiet
-00001250: 602e 2055 7365 2060 2d76 2064 6562 7567  `. Use `-v debug
-00001260: 600d 0a20 2020 2020 2020 2020 2020 2020  `..             
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2066 6f72 2062 7567 2072 6570 6f72     for bug repor
-00001290: 7473 2e20 5b64 6566 6175 6c74 3a20 696e  ts. [default: in
-000012a0: 666f 5d0d 0a0d 0a20 202d 6c2c 202d 2d6c  fo]....  -l, --l
-000012b0: 6f67 6669 6c65 204c 4f47 2020 2020 2020  ogfile LOG      
-000012c0: 2020 2020 2020 2050 6174 6820 746f 206c         Path to l
-000012d0: 6f67 2066 696c 6520 666f 7220 7772 6974  og file for writ
-000012e0: 696e 6720 6170 706c 6963 6174 696f 6e0d  ing application.
-000012f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 206c 6f67 6769 6e67 2069 6e66 6f72 6d61   logging informa
-00001320: 7469 6f6e 2c20 6d61 696e 6c79 2066 6f72  tion, mainly for
-00001330: 2064 6562 7567 6769 6e67 2e20 5365 740d   debugging. Set.
-00001340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2060 2d76 2064 6562 7567 6020 6173 2077   `-v debug` as w
-00001370: 656c 6c20 6966 2079 6f75 2061 7265 2073  ell if you are s
-00001380: 7562 6d69 7474 696e 6720 6120 6275 670d  ubmitting a bug.
-00001390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2072 6570 6f72 742e 2049 6620 7665 7262   report. If verb
-000013c0: 6f73 6974 7920 6973 206e 6f6e 652c 206c  osity is none, l
-000013d0: 6f67 6669 6c65 2069 7320 7374 696c 6c0d  ogfile is still.
-000013e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 2062 6520 6765 6e65 7261 7465 6420 7769   be generated wi
-00001410: 7468 2069 6e66 6f2d 6c65 7665 6c20 7665  th info-level ve
-00001420: 7262 6f73 6974 792e 0d0a 0d0a 2020 2d71  rbosity.....  -q
-00001430: 2c20 2d2d 7175 6965 7420 2020 2020 2020  , --quiet       
-00001440: 2020 2020 2020 2020 2020 2020 5375 7070              Supp
-00001450: 7265 7373 6573 2061 6c6c 206f 7574 7075  resses all outpu
-00001460: 7420 6f66 2050 7953 6365 6e65 4465 7465  t of PySceneDete
-00001470: 6374 2074 6f20 7468 650d 0a20 2020 2020  ct to the..     
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 2020 2020 2074 6572 6d69             termi
-000014a0: 6e61 6c2f 7374 646f 7574 2e20 4571 7569  nal/stdout. Equi
-000014b0: 7661 6c65 6e74 2074 6f20 602d 7620 6e6f  valent to `-v no
-000014c0: 6e65 602e 0d0a 0d0a 2020 2d62 2c20 2d2d  ne`.....  -b, --
-000014d0: 6261 636b 656e 6420 4241 434b 454e 4420  backend BACKEND 
-000014e0: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
-000014f0: 6261 636b 656e 6420 746f 2075 7365 2066  backend to use f
-00001500: 6f72 2076 6964 656f 2069 6e70 7574 2e0d  or video input..
-00001510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2042 6163 6b65 6e64 7320 6176 6169 6c61   Backends availa
-00001540: 626c 6520 6f6e 2074 6869 7320 7379 7374  ble on this syst
-00001550: 656d 3a0d 0a20 2020 2020 2020 2020 2020  em:..           
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2020 2020 2064 6963 745f 6b65 7973 285b       dict_keys([
-00001580: 276f 7065 6e63 7627 2c20 2770 7961 7627  'opencv', 'pyav'
-00001590: 5d29 205b 6465 6661 756c 743a 0d0a 2020  ]) [default:..  
+00000f60: 0a20 202d 2d6d 6572 6765 2d6c 6173 742d  .  --merge-last-
+00000f70: 7363 656e 6520 2020 2020 2020 2020 2020  scene           
+00000f80: 204d 6572 6765 206c 6173 7420 7363 656e   Merge last scen
+00000f90: 6520 7769 7468 2070 7265 7669 6f75 7320  e with previous 
+00000fa0: 6966 2073 686f 7274 6572 2074 6861 6e0d  if shorter than.
+00000fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 206d 696e 2d73 6365 6e65 2d6c 656e 2e0d   min-scene-len..
+00000fe0: 0a0d 0a20 202d 732c 202d 2d73 7461 7473  ...  -s, --stats
+00000ff0: 2043 5356 2020 2020 2020 2020 2020 2020   CSV            
+00001000: 2020 2050 6174 6820 746f 2073 7461 7473     Path to stats
+00001010: 2066 696c 6520 282e 6373 7629 2066 6f72   file (.csv) for
+00001020: 2077 7269 7469 6e67 2066 7261 6d65 0d0a   writing frame..
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 6d65 7472 6963 7320 746f 2e20 4966 2074  metrics to. If t
+00001060: 6865 2066 696c 6520 6578 6973 7473 2c20  he file exists, 
+00001070: 616e 7920 6d65 7472 6963 730d 0a20 2020  any metrics..   
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 2020 2020 2020 2020 2020 2020 2077 696c               wil
+000010a0: 6c20 6265 2070 726f 6365 7373 6564 2c20  l be processed, 
+000010b0: 6f74 6865 7277 6973 6520 6120 6e65 7720  otherwise a new 
+000010c0: 6669 6c65 2077 696c 6c0d 0a20 2020 2020  file will..     
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2020 2020 2020 2020 2062 6520 6372             be cr
+000010f0: 6561 7465 642e 2043 616e 2062 6520 7573  eated. Can be us
+00001100: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
+00001110: 6f70 7469 6d61 6c0d 0a20 2020 2020 2020  optimal..       
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2020 2020 2020 2020 2076 616c 7565 7320           values 
+00001140: 666f 7220 7661 7269 6f75 7320 7363 656e  for various scen
+00001150: 6520 6465 7465 6374 6f72 206f 7074 696f  e detector optio
+00001160: 6e73 2c20 616e 640d 0a20 2020 2020 2020  ns, and..       
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 2074 6f20 6361 6368           to cach
+00001190: 6520 6672 616d 6520 6361 6c63 756c 6174  e frame calculat
+000011a0: 696f 6e73 2069 6e20 6f72 6465 7220 746f  ions in order to
+000011b0: 2073 7065 6564 0d0a 2020 2020 2020 2020   speed..        
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2020 2020 2020 2020 7570 206d 756c 7469          up multi
+000011e0: 706c 6520 6465 7465 6374 696f 6e20 7275  ple detection ru
+000011f0: 6e73 2e0d 0a0d 0a20 202d 762c 202d 2d76  ns.....  -v, --v
+00001200: 6572 626f 7369 7479 204c 4556 454c 2020  erbosity LEVEL  
+00001210: 2020 2020 2020 204c 6576 656c 206f 6620         Level of 
+00001220: 6465 6275 672f 696e 666f 2f65 7272 6f72  debug/info/error
+00001230: 2069 6e66 6f72 6d61 7469 6f6e 2074 6f20   information to 
+00001240: 7368 6f77 2e0d 0a20 2020 2020 2020 2020  show...         
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 204d 7573 7420 6265 206f         Must be o
+00001270: 6e65 206f 663a 2064 6562 7567 2c20 696e  ne of: debug, in
+00001280: 666f 2c20 7761 726e 696e 672c 2065 7272  fo, warning, err
+00001290: 6f72 2c0d 0a20 2020 2020 2020 2020 2020  or,..           
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2020 2020 206e 6f6e 652e 204f 7665 7272       none. Overr
+000012c0: 6964 6573 2060 2d71 602f 602d 2d71 7569  ides `-q`/`--qui
+000012d0: 6574 602e 2055 7365 2060 2d76 2064 6562  et`. Use `-v deb
+000012e0: 7567 600d 0a20 2020 2020 2020 2020 2020  ug`..           
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 2020 2066 6f72 2062 7567 2072 6570       for bug rep
+00001310: 6f72 7473 2e20 5b64 6566 6175 6c74 3a20  orts. [default: 
+00001320: 696e 666f 5d0d 0a0d 0a20 202d 6c2c 202d  info]....  -l, -
+00001330: 2d6c 6f67 6669 6c65 204c 4f47 2020 2020  -logfile LOG    
+00001340: 2020 2020 2020 2020 2050 6174 6820 746f           Path to
+00001350: 206c 6f67 2066 696c 6520 666f 7220 7772   log file for wr
+00001360: 6974 696e 6720 6170 706c 6963 6174 696f  iting applicatio
+00001370: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 206c 6f67 6769 6e67 2069 6e66 6f72     logging infor
+000013a0: 6d61 7469 6f6e 2c20 6d61 696e 6c79 2066  mation, mainly f
+000013b0: 6f72 2064 6562 7567 6769 6e67 2e20 5365  or debugging. Se
+000013c0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2060 2d76 2064 6562 7567 6020 6173     `-v debug` as
+000013f0: 2077 656c 6c20 6966 2079 6f75 2061 7265   well if you are
+00001400: 2073 7562 6d69 7474 696e 6720 6120 6275   submitting a bu
+00001410: 670d 0a20 2020 2020 2020 2020 2020 2020  g..             
+00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001430: 2020 2072 6570 6f72 742e 2049 6620 7665     report. If ve
+00001440: 7262 6f73 6974 7920 6973 206e 6f6e 652c  rbosity is none,
+00001450: 206c 6f67 6669 6c65 2069 7320 7374 696c   logfile is stil
+00001460: 6c0d 0a20 2020 2020 2020 2020 2020 2020  l..             
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2062 6520 6765 6e65 7261 7465 6420     be generated 
+00001490: 7769 7468 2069 6e66 6f2d 6c65 7665 6c20  with info-level 
+000014a0: 7665 7262 6f73 6974 792e 0d0a 0d0a 2020  verbosity.....  
+000014b0: 2d71 2c20 2d2d 7175 6965 7420 2020 2020  -q, --quiet     
+000014c0: 2020 2020 2020 2020 2020 2020 2020 5375                Su
+000014d0: 7070 7265 7373 6573 2061 6c6c 206f 7574  ppresses all out
+000014e0: 7075 7420 6f66 2050 7953 6365 6e65 4465  put of PySceneDe
+000014f0: 7465 6374 2074 6f20 7468 650d 0a20 2020  tect to the..   
+00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001510: 2020 2020 2020 2020 2020 2020 2074 6572               ter
+00001520: 6d69 6e61 6c2f 7374 646f 7574 2e20 4571  minal/stdout. Eq
+00001530: 7569 7661 6c65 6e74 2074 6f20 602d 7620  uivalent to `-v 
+00001540: 6e6f 6e65 602e 0d0a 0d0a 2020 2d62 2c20  none`.....  -b, 
+00001550: 2d2d 6261 636b 656e 6420 4241 434b 454e  --backend BACKEN
+00001560: 4420 2020 2020 2020 2020 4e61 6d65 206f  D         Name o
+00001570: 6620 6261 636b 656e 6420 746f 2075 7365  f backend to use
+00001580: 2066 6f72 2076 6964 656f 2069 6e70 7574   for video input
+00001590: 2e0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-000015c0: 656e 6376 5d0d 0a0d 0a20 202d 632c 202d  encv]....  -c, -
-000015d0: 2d63 6f6e 6669 6720 4649 4c45 2020 2020  -config FILE    
-000015e0: 2020 2020 2020 2020 2050 6174 6820 746f           Path to
-000015f0: 2063 6f6e 6669 6720 6669 6c65 2e20 4966   config file. If
-00001600: 206e 6f74 2073 6574 2c20 7472 6965 7320   not set, tries 
-00001610: 746f 206c 6f61 640d 0a20 2020 2020 2020  to load..       
+000015b0: 2020 2042 6163 6b65 6e64 7320 6176 6169     Backends avai
+000015c0: 6c61 626c 6520 6f6e 2074 6869 7320 7379  lable on this sy
+000015d0: 7374 656d 3a0d 0a20 2020 2020 2020 2020  stem:..         
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2020 2020 2020 2064 6963 745f 6b65 7973         dict_keys
+00001600: 285b 276f 7065 6e63 7627 2c20 2770 7961  (['opencv', 'pya
+00001610: 7627 5d29 205b 6465 6661 756c 743a 0d0a  v']) [default:..
 00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 206f 6e65 2066 726f           one fro
-00001640: 6d20 6120 6c6f 6361 7469 6f6e 2062 6173  m a location bas
-00001650: 6564 206f 6e20 796f 7572 206f 7065 7261  ed on your opera
-00001660: 7469 6e67 2073 7973 7465 6d2e 0d0a 2020  ting system...  
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 5479                Ty
-00001690: 7065 2060 7363 656e 6564 6574 6563 7420  pe `scenedetect 
-000016a0: 6865 6c70 6020 616e 6420 7468 6973 206f  help` and this o
-000016b0: 7074 696f 6e20 7769 6c6c 2073 686f 770d  ption will show.
-000016c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2074 6865 2063 6f72 7265 6374 2070 6174   the correct pat
-000016f0: 6820 6f6e 2079 6f75 7220 7379 7374 656d  h on your system
-00001700: 2e0d 0a                                  ...
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 6f70 656e 6376 5d0d 0a0d 0a20 202d 632c  opencv]....  -c,
+00001650: 202d 2d63 6f6e 6669 6720 4649 4c45 2020   --config FILE  
+00001660: 2020 2020 2020 2020 2020 2050 6174 6820             Path 
+00001670: 746f 2063 6f6e 6669 6720 6669 6c65 2e20  to config file. 
+00001680: 4966 206e 6f74 2073 6574 2c20 7472 6965  If not set, trie
+00001690: 7320 746f 206c 6f61 640d 0a20 2020 2020  s to load..     
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 2020 2020 2020 2020 2020 206f 6e65 2066             one f
+000016c0: 726f 6d20 6120 6c6f 6361 7469 6f6e 2062  rom a location b
+000016d0: 6173 6564 206f 6e20 796f 7572 206f 7065  ased on your ope
+000016e0: 7261 7469 6e67 2073 7973 7465 6d2e 0d0a  rating system...
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 5479 7065 2060 7363 656e 6564 6574 6563  Type `scenedetec
+00001720: 7420 6865 6c70 6020 616e 6420 7468 6973  t help` and this
+00001730: 206f 7074 696f 6e20 7769 6c6c 2073 686f   option will sho
+00001740: 770d 0a20 2020 2020 2020 2020 2020 2020  w..             
+00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001760: 2020 2074 6865 2063 6f72 7265 6374 2070     the correct p
+00001770: 6174 6820 6f6e 2079 6f75 7220 7379 7374  ath on your syst
+00001780: 656d 2e0d 0a                             em...
```

### Comparing `scenedetect-0.6.dev3/manual/conf.py` & `scenedetect-0.6rc0/manual/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 project = 'PySceneDetect'
 copyright = '2014-2022, Brandon Castellano'
 author = 'Brandon Castellano'
 
 # The short X.Y version
 version = '0.6'
 # The full version, including alpha/beta/rc tags
-release = 'v0.6-dev3'
+release = 'v0.6-rc0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `scenedetect-0.6.dev3/manual/index.rst` & `scenedetect-0.6rc0/manual/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     :caption: Command-Line Interface [CLI]:
     :name: clitoc
 
     cli/global_options
     cli/commands
     cli/detectors
     cli/config_file
+    cli/backends
 
 
 =======================================================================
 ``scenedetect`` Python Module 🐍
 =======================================================================
 
 .. toctree::
@@ -48,14 +49,15 @@
     api/detectors
     api/video_stream
     api/backends
     api/video_splitter
     api/frame_timecode
     api/scene_detector
     api/stats_manager
+    api/platform
     api/migration_guide
 
 =======================================================================
 Indices and Tables
 =======================================================================
 
 * :ref:`genindex`
```

### Comparing `scenedetect-0.6.dev3/manual/make.bat` & `scenedetect-0.6rc0/manual/make.bat`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/mkdocs.yml` & `scenedetect-0.6rc0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/package-info.rst` & `scenedetect-0.6rc0/dist/package-info.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
    :target: http://pyscenedetect.readthedocs.org/en/latest/copyright/
 
 .. image:: https://img.shields.io/github/stars/Breakthrough/PySceneDetect.svg?style=social&label=View%20on%20Github
    :target: https://github.com/Breakthrough/PySceneDetect
 
 ----------------------------------------------------------
 
-Website: http://py.scenedetect.com/
+Website: http://scenedetect.com/
 
 Documentation: http://manual.scenedetect.com/
 
 Github Repo: https://github.com/Breakthrough/PySceneDetect/
 
 ----------------------------------------------------------
```

### Comparing `scenedetect-0.6.dev3/scenedetect/__main__.py` & `scenedetect-0.6rc0/scenedetect/__main__.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/backends/__init__.py` & `scenedetect-0.6rc0/tests/test_scene_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,136 +6,164 @@
 #     [  Docs:   http://manual.scenedetect.scenedetect.com/      ]
 #     [  Github: https://github.com/Breakthrough/PySceneDetect/  ]
 #
 # Copyright (C) 2014-2022 Brandon Castellano <http://www.bcastell.com>.
 # PySceneDetect is licensed under the BSD 3-Clause License; see the
 # included LICENSE file, or visit one of the above pages for details.
 #
-""" ``scenedetect.backends`` Module
+"""PySceneDetect scenedetect.scene_manager Tests
 
-This module contains concrete :py:class:`VideoStream <scenedetect.video_stream.VideoStream>`
-implementations. For video files, the :py:data:`open_video` function can be used to open a
-video with any available backend (or a string hinting which backend is preferred).
+This file includes unit tests for the scenedetect.scene_manager.SceneManager class,
+which applies SceneDetector algorithms on VideoStream backends.
+"""
 
-Backends available on the current system can be found via :py:data:`AVAILABLE_BACKENDS`.
+# Standard project pylint disables for unit tests using pytest.
+# pylint: disable=protected-access, invalid-name, unused-argument, redefined-outer-name
 
-===============================================================
-Usage Example
-===============================================================
+import glob
+import os
+import os.path
+from typing import Iterable, Tuple
 
-Assuming we have a file `video.mp4` in our working directory, we can load it and iterate through
-all of the frames:
+import pytest
 
-.. code:: python
+from scenedetect.backends.opencv import VideoStreamCv2
+from scenedetect.detectors import ContentDetector
+from scenedetect.frame_timecode import FrameTimecode
+from scenedetect.scene_manager import SceneManager, save_images
 
-    from scenedetect.backends import open_video
-    video = open_video(path='video.mp4')
-    while True:
-        frame = video.read()
-        if frame is False:
-            break
-    print("Read %d frames" % video.frame_number)
 
-If we want to use a specific backend from :py:data:`AVAILABLE_BACKENDS`, we can pass it to
-:py:func:`open_video`:
+def test_scene_list(test_video_file):
+    """ Test SceneManager get_scene_list method with VideoStreamCv2/ContentDetector. """
+    video = VideoStreamCv2(test_video_file)
+    sm = SceneManager()
+    sm.add_detector(ContentDetector())
 
-.. code:: python
+    video_fps = video.frame_rate
+    start_time = FrameTimecode('00:00:05', video_fps)
+    end_time = FrameTimecode('00:00:15', video_fps)
 
-    # Specifying a backend via `open_video`:
-    from scenedetect.backends import open_video
-    video = open_video(path='video.mp4', backend='opencv')
+    assert end_time.get_frames() > start_time.get_frames()
 
-Or we can import and use specific backend directly:
+    video.seek(start_time)
+    sm.auto_downscale = True
 
-.. code:: python
+    num_frames = sm.detect_scenes(video=video, end_time=end_time)
 
-    # Manually importing and constructing a backend:
-    from scenedetect.backends.opencv import VideoStreamCv2
-    video = VideoStreamCv2(path_or_device='video.mp4')
+    assert num_frames == (1 + end_time.get_frames() - start_time.get_frames())
 
-The ``'opencv'`` backend (:py:class:`VideoStreamCv2 <scenedetect.backends.opencv.VideoStreamCv2>`)
-is guaranteed to be available.
-"""
+    scene_list = sm.get_scene_list()
+    assert scene_list
+    # Each scene is in the format (Start Timecode, End Timecode)
+    assert len(scene_list[0]) == 2
 
-# TODO(v1.0): Consider removing and making this a namespace package so that additional backends can
-# be dynamically added. The preferred approach for this should probably be:
-# https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-namespace-packages
+    for i, _ in enumerate(scene_list):
+        assert scene_list[i][0].get_frames() < scene_list[i][1].get_frames()
+        if i > 0:
+            # Ensure frame list is sorted (i.e. end time frame of
+            # one scene is equal to the start time of the next).
+            assert scene_list[i-1][1] == scene_list[i][0]
 
-# TODO: Future VideoStream implementations under consideration:
-#  - Nvidia VPF: https://developer.nvidia.com/blog/vpf-hardware-accelerated-video-processing-framework-in-python/
 
-from logging import getLogger
-from typing import Dict, List, Optional, Type
 
-# VideoStreamCv2 must be available at minimum.
-from scenedetect.backends.opencv import VideoStreamCv2
-from scenedetect.video_stream import VideoStream, VideoOpenFailure
+def test_save_images(test_video_file):
+    """ Test scenedetect.scene_manager.save_images function.  """
+    video = VideoStreamCv2(test_video_file)
+    sm = SceneManager()
+    sm.add_detector(ContentDetector())
 
-try:
-    from scenedetect.backends.pyav import VideoStreamAv
-except ImportError:
-    VideoStreamAv = None
-
-logger = getLogger('pyscenedetect')
-
-AVAILABLE_BACKENDS: Dict[str, Type] = {
-    backend.BACKEND_NAME: backend for backend in filter(None, [
-        VideoStreamCv2,
-        VideoStreamAv,
-    ])
-}
-"""All available backends that :py:func:`open_video` can consider for the `preferred_backend`
-parameter. These backends must support construction with the following signature:
+    image_name_glob = 'scenedetect.tempfile.*.jpg'
+    image_name_template = 'scenedetect.tempfile.$SCENE_NUMBER.$IMAGE_NUMBER'
 
-    BackendType(path: str, framerate: Optional[float])
-"""
+    try:
+        video_fps = video.frame_rate
+        start_time = FrameTimecode('00:00:05', video_fps)
+        end_time = FrameTimecode('00:00:15', video_fps)
+
+        video.seek(start_time)
+        sm.auto_downscale = True
+
+        sm.detect_scenes(video=video, end_time=end_time)
+
+        scene_list = sm.get_scene_list()
+        assert scene_list
+
+        image_filenames = save_images(
+            scene_list=scene_list,
+            video=video,
+            num_images=3,
+            image_extension='jpg',
+            image_name_template=image_name_template)
+
+        # Ensure images got created, and the proper number got created.
+        total_images = 0
+        for scene_number in image_filenames:
+            for path in image_filenames[scene_number]:
+                assert os.path.exists(path)
+                total_images += 1
+
+        assert total_images == len(glob.glob(image_name_glob))
+
+    finally:
+        for path in glob.glob(image_name_glob):
+            os.remove(path)
+
+
+class FakeCallback(object):
+    """ Fake callback used for testing purposes only. Currently just stores
+    the number of times the callback was invoked."""
+
+    def __init__(self):
+        self.num_invoked: int = 0
+
+    def get_callback_lambda(self):
+        """Returns a callback which consumes a frame image and timecode. The `num_invoked` property
+        is incremented each time the callback is invoked."""
+        return lambda image, frame_num: self._callback(image, frame_num)
+
+    def get_callback_func(self):
+        """Returns a callback which consumes a frame image and timecode. The `num_invoked` property
+        is incremented each time the callback is invoked."""
+
+        def callback(image, frame_num):
+            nonlocal self
+            self._callback(image, frame_num)
+
+        return callback
+
+    def _callback(self, image, frame_num):
+        self.num_invoked += 1
 
-PREFERRED_BACKENDS: List[str] = ['pyav', 'opencv']
-"""List of backend names to try, in order, when using :py:func:`open_video`."""
 
+def test_detect_scenes_callback(test_video_file):
+    """ Test SceneManager detect_scenes method with a callback function.
 
-def open_video(path: str,
-               framerate: Optional[float] = None,
-               backend: Optional[str] = None) -> VideoStream:
-    """Opens a video at the given path.
-
-    Arguments:
-        path: Path to video file to open.
-        framerate: Overrides detected framerate if set.
-        backend: Name of specific to use if possible. See :py:data:`AVAILABLE_BACKENDS` for
-            available backends. If the specified backend is unavailable (or `backend` is not
-            specified), the values in :py:data:`PREFERRED_BACKENDS` will be used in order.
-
-    Returns:
-        VideoStream backend object created with the specified video path.
-
-    Raises:
-        :py:class:`VideoOpenFailure`: Constructing the VideoStream fails. If multiple backends have
-            been attempted, the error from the first backend will be returned.
+    Note that the API signature of the callback will undergo breaking changes in v1.0.
     """
-    # Try to open the video with the specified backend.
-    last_error = None
-    if backend is not None:
-        if backend in AVAILABLE_BACKENDS:
-            try:
-                logger.debug('Opening video with %s...', AVAILABLE_BACKENDS[backend].__name__)
-                return AVAILABLE_BACKENDS[backend](path, framerate)
-            except VideoOpenFailure as ex:
-                logger.debug('Failed to open video: %s', str(ex))
-                logger.debug('Trying preferred backends...')
-                last_error = ex
-        else:
-            logger.debug('Backend %s not available. Trying preferred backends...', backend)
-    # Try to open the video with the preferred backends in order.
-    for backend_type in PREFERRED_BACKENDS:
-        if not backend_type in AVAILABLE_BACKENDS:
-            continue
-        try:
-            backend = AVAILABLE_BACKENDS[backend_type]
-            logger.debug('Opening video with %s...', backend.__name__)
-            return backend(path, framerate)
-        except VideoOpenFailure as ex:
-            logger.debug('Failed to open video: %s', str(ex))
-            if last_error is None:
-                last_error = ex
-    assert last_error is not None
-    raise last_error
+    video = VideoStreamCv2(test_video_file)
+    sm = SceneManager()
+    sm.add_detector(ContentDetector())
+
+    fake_callback = FakeCallback()
+
+    video_fps = video.frame_rate
+    start_time = FrameTimecode('00:00:05', video_fps)
+    end_time = FrameTimecode('00:00:15', video_fps)
+    video.seek(start_time)
+    sm.auto_downscale = True
+
+    _ = sm.detect_scenes(
+        video=video, end_time=end_time, callback=fake_callback.get_callback_lambda())
+    scene_list = sm.get_scene_list()
+    assert scene_list
+    assert fake_callback.num_invoked == (len(sm.get_scene_list()) - 1)
+
+    # Perform same test using callback function instead of lambda.
+    sm.clear()
+    sm.add_detector(ContentDetector())
+    fake_callback.num_invoked = 0
+    video.seek(start_time)
+
+    _ = sm.detect_scenes(video=video, end_time=end_time, callback=fake_callback.get_callback_func())
+    scene_list = sm.get_scene_list()
+    assert scene_list
+    assert fake_callback.num_invoked == (len(sm.get_scene_list()) - 1)
```

### Comparing `scenedetect-0.6.dev3/scenedetect/backends/opencv.py` & `scenedetect-0.6rc0/scenedetect/backends/opencv.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,59 +11,75 @@
 # included LICENSE file, or visit one of the above pages for details.
 #
 """:py:class:`VideoStreamCv2` provides an adapter for the OpenCV cv2.VideoCapture object.
 
 Uses string identifier ``'opencv'``.
 """
 
-import logging
+from logging import getLogger
 import math
 from typing import Tuple, Union, Optional
 import os.path
 
 import cv2
 from numpy import ndarray
 
 from scenedetect.frame_timecode import FrameTimecode, MAX_FPS_DELTA
 from scenedetect.platform import get_aspect_ratio, get_file_name
 from scenedetect.video_stream import VideoStream, SeekError, VideoOpenFailure, FrameRateUnavailable
 
-logger = logging.getLogger('pyscenedetect')
+logger = getLogger('pyscenedetect')
 
 
 class VideoStreamCv2(VideoStream):
     """OpenCV `cv2.VideoCapture` backend."""
 
-    def __init__(self, path_or_device: Union[bytes, str, int], framerate: Optional[float] = None):
+    def __init__(
+        self,
+        path_or_device: Union[bytes, str, int],
+        framerate: Optional[float] = None,
+        max_decode_attempts: int = 5,
+    ):
         """Open a video or device.
 
         Arguments:
             path_or_device: Path to video, or device ID as integer.
             framerate: If set, overrides the detected framerate.
+            max_decode_attempts: Number of attempts to continue decoding the video
+                after a frame fails to decode. This allows processing videos that
+                have a few corrupted frames or metadata (in which case accuracy
+                of detection algorithms may be lower). Once this limit is passed,
+                decoding will stop and emit an error.
 
         Raises:
             OSError: file could not be found or access was denied
             VideoOpenFailure: video could not be opened (may be corrupted)
             ValueError: specified framerate is invalid
         """
         super().__init__()
 
         if framerate is not None and framerate < MAX_FPS_DELTA:
             raise ValueError('Specified framerate (%f) is invalid!' % framerate)
+        if max_decode_attempts < 0:
+            raise ValueError('Maximum decode attempts must be >= 0!')
 
         self._path_or_device = path_or_device
         self._is_device = isinstance(self._path_or_device, int)
 
         # Initialized in _open_capture:
-        self._cap = None # Reference to underlying cv2.VideoCapture object.
-        self._frame_rate = None
+        self._cap: Optional[
+            cv2.VideoCapture] = None # Reference to underlying cv2.VideoCapture object.
+        self._frame_rate: Optional[float] = None
 
         # VideoCapture state
         self._has_seeked = False
         self._has_grabbed = False
+        self._max_decode_attempts = max_decode_attempts
+        self._decode_failures = 0
+        self._warning_displayed = False
 
         self._open_capture(framerate)
 
     #
     # Backend-Specific Methods/Properties
     #
 
@@ -71,41 +87,49 @@
     def capture(self) -> cv2.VideoCapture:
         """Returns reference to underlying VideoCapture object. Use with caution.
 
         Prefer to use this property only to take ownership of the underlying cv2.VideoCapture object
         backing this object. Seeking or using the read/grab methods through this property are
         unsupported and will leave this object in an inconsistent state.
         """
+        assert self._cap
         return self._cap
 
     #
     # VideoStream Methods/Properties
     #
 
     BACKEND_NAME = 'opencv'
     """Unique name used to identify this backend."""
 
     @property
     def frame_rate(self) -> float:
         """Framerate in frames/sec."""
+        assert self._frame_rate
         return self._frame_rate
 
     @property
     def path(self) -> Union[bytes, str]:
         """Video or device path."""
         if self._is_device:
+            assert isinstance(self._path_or_device, (int))
             return "Device %d" % self._path_or_device
+        assert isinstance(self._path_or_device, (bytes, str))
         return self._path_or_device
 
     @property
     def name(self) -> Union[bytes, str]:
         """Name of the video, without extension, or device."""
         if self._is_device:
             return self.path
-        return get_file_name(self.path, include_extension=False)
+        file_name: str = get_file_name(self.path, include_extension=False)
+        if '%' in file_name:
+            # file_name is an image sequence, trim everything including/after the %.
+            file_name = file_name[:file_name.rfind('%')]
+        return file_name
 
     @property
     def is_seekable(self) -> bool:
         """True if seek() is allowed, False otherwise.
 
         Always False if opening a device/webcam."""
         return not self._is_device
@@ -214,14 +238,26 @@
             If decode = False, a boolean indicating if the next frame was advanced to or not is
             returned.
         """
         if not self._cap.isOpened():
             return False
         if advance:
             self._has_grabbed = self._cap.grab()
+            if not self._has_grabbed:
+                if self.duration > 0 and self.position < (self.duration - 1):
+                    for _ in range(self._max_decode_attempts):
+                        self._has_grabbed = self._cap.grab()
+                        if self._has_grabbed:
+                            break
+                # Report previous failure in debug mode.
+                if self._has_grabbed:
+                    self._decode_failures += 1
+                    logger.debug('Frame failed to decode.')
+                    if not self._warning_displayed and self._decode_failures > 1:
+                        logger.warning('Failed to decode some frames, results may be inaccurate.')
             self._has_seeked = False
         if decode and self._has_grabbed:
             _, frame = self._cap.retrieve()
             return frame
         return self._has_grabbed
 
     #
@@ -242,15 +278,17 @@
         cap = cv2.VideoCapture(self._path_or_device)
         if not cap.isOpened():
             raise VideoOpenFailure(
                 'VideoCapture.isOpened() returned False. Ensure the input file is a valid video,'
                 ' and check that OpenCV is installed correctly.\n')
 
         # Display a warning if the video codec type seems unsupported (#86).
-        if not self._is_device and int(abs(cap.get(cv2.CAP_PROP_FOURCC))) == 0:
+        # We don't do the check if this is a webcam/video capture device or an image sequence.
+        if not (self._is_device or '%' in self._path_or_device) and int(
+                abs(cap.get(cv2.CAP_PROP_FOURCC))) == 0:
             logger.error(
                 'Video codec detection failed, output may be incorrect.\nThis could be caused'
                 ' by using an outdated version of OpenCV, or using codecs that currently are'
                 ' not well supported (e.g. VP9).\n'
                 'As a workaround, consider re-encoding the source material before processing.\n'
                 'For details, see https://github.com/Breakthrough/PySceneDetect/issues/86')
```

### Comparing `scenedetect-0.6.dev3/scenedetect/backends/pyav.py` & `scenedetect-0.6rc0/scenedetect/backends/pyav.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,79 +14,110 @@
 
 Uses string identifier ``'pyav'``.
 """
 
 from logging import getLogger
 from typing import AnyStr, BinaryIO, Optional, Tuple, Union
 
+#pylint: disable=c-extension-no-member
 import av
 from numpy import ndarray
 
 from scenedetect.frame_timecode import FrameTimecode, MAX_FPS_DELTA
 from scenedetect.platform import get_file_name
 from scenedetect.video_stream import VideoStream, VideoOpenFailure, FrameRateUnavailable
 
 logger = getLogger('pyscenedetect')
 
+VALID_THREAD_MODES = [
+    av.codec.context.ThreadType.NONE,
+    av.codec.context.ThreadType.SLICE,
+    av.codec.context.ThreadType.FRAME,
+    av.codec.context.ThreadType.AUTO,
+]
 
-#pylint: disable=c-extension-no-member
 class VideoStreamAv(VideoStream):
     """PyAV `av.InputContainer` backend."""
 
-    # TODO(v0.6.1): Add config file option for threading mode.
-    # TODO(v0.6.1): Add `accurate_duration` option (default to False) to config file.
+    # TODO: Investigate adding an accurate_duration option to backends to calculate the duration
+    # with higher precision. Sometimes it doesn't exactly match what the codec or VLC reports,
+    # but we can try to seek to the end of the video first to determine it. Investigate how VLC
+    # calculates the end time.
     def __init__(
         self,
         path_or_io: Union[AnyStr, BinaryIO],
         framerate: Optional[float] = None,
         name: Optional[str] = None,
-        threading_mode: str = 'AUTO',
+        threading_mode: Optional[str] = None,
+        suppress_output: bool = False,
     ):
         """Open a video by path.
 
+        .. warning::
+
+            Using `threading_mode` with `suppress_output = True` can cause lockups in your
+            application. See the PyAV documentation for details:
+            https://pyav.org/docs/stable/overview/caveats.html#sub-interpeters
+
         Arguments:
             path_or_io: Path to the video, or a file-like object.
             framerate: If set, overrides the detected framerate.
             name: Overrides the `name` property derived from the video path. Should be set if
                 `path_or_io` is a file-like object.
             threading_mode: The PyAV video stream `thread_type`. See av.codec.context.ThreadType
                 for valid threading modes ('AUTO', 'FRAME', 'NONE', and 'SLICE'). If this mode is
                 'AUTO' or 'FRAME' and not all frames have been decoded, the video will be reopened
-                if it is seekable, and the remaining frames will be decoded in single-threaded mode.
-                Default is 'AUTO' for performance (there will be a slight pause near the end).
+                if seekable, and the remaining frames decoded in single-threaded mode.
+            suppress_output: If False, ffmpeg output will be sent to stdout/stderr by calling
+                `av.logging.restore_default_callback()` before any other library calls. If True
+                the application may deadlock if threading_mode is set. See the PyAV documentation
+                for details: https://pyav.org/docs/stable/overview/caveats.html#sub-interpeters
 
         Raises:
             OSError: file could not be found or access was denied
             VideoOpenFailure: video could not be opened (may be corrupted)
             ValueError: specified framerate is invalid
         """
+        self._container = None
+
         # TODO(#258): See what self._container.discard_corrupt = True does with corrupt videos.
         super().__init__()
 
         # Ensure specified framerate is valid if set.
         if framerate is not None and framerate < MAX_FPS_DELTA:
             raise ValueError('Specified framerate (%f) is invalid!' % framerate)
 
-        self._name: Union[str, bytes] = '' if name is None else name
+        self._name = '' if name is None else name
+        self._path = ''
         self._frame = None
         self._reopened = True
 
+        if threading_mode:
+            threading_mode = threading_mode.upper()
+            if not threading_mode in VALID_THREAD_MODES:
+                raise ValueError('Invalid threading mode! Must be one of: %s' % VALID_THREAD_MODES)
+
+        if not suppress_output:
+            logger.debug('Restoring default ffmpeg log callbacks.')
+            av.logging.restore_default_callback()
+
         try:
             if isinstance(path_or_io, (str, bytes)):
                 self._path = path_or_io
                 self._io = open(path_or_io, 'rb')
                 if not self._name:
                     self._name = get_file_name(self.path, include_extension=False)
             else:
                 self._io = path_or_io
 
             self._container = av.open(self._io)
             if threading_mode is not None:
                 self._video_stream.thread_type = threading_mode
                 self._reopened = False
+                logger.debug('Threading mode set: %s', threading_mode)
         except OSError:
             raise
         except Exception as ex:
             raise VideoOpenFailure(str(ex)) from ex
 
         if framerate is None:
             # Calculate framerate from video container.
@@ -100,14 +131,18 @@
         else:
             assert framerate >= MAX_FPS_DELTA
             self._frame_rate: float = framerate
 
         # Calculate duration after we have set the framerate.
         self._duration_frames = self._get_duration()
 
+    def __del__(self):
+        if self._container is not None:
+            self._container.close()
+
     #
     # VideoStream Methods/Properties
     #
 
     BACKEND_NAME = 'pyav'
     """Unique name used to identify this backend."""
 
@@ -292,21 +327,23 @@
     def _handle_eof(self):
         """Fix for issue where if thread_type is 'AUTO' the whole video is not decoded.
 
         Re-open video if the threading mode is AUTO and we didn't decode all of the frames."""
         # Don't re-open the video if we already did, or if we already decoded all the frames.
         if self._reopened or self.frame_number >= self.duration:
             return False
+        self._reopened = True
         # Don't re-open the video if we can't seek or aren't in AUTO/FRAME thread_type mode.
         if not self.is_seekable or not self._video_stream.thread_type in ('AUTO', 'FRAME'):
             return False
         last_frame = self.frame_number
         orig_pos = self._io.tell()
         try:
             self._io.seek(0)
             container = av.open(self._io)
         except:
             self._io.seek(orig_pos)
             raise
+        self._container.close()
         self._container = container
         self.seek(last_frame)
         return True
```

### Comparing `scenedetect-0.6.dev3/scenedetect/cli/__init__.py` & `scenedetect-0.6rc0/scenedetect/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,21 @@
     '--drop-short-scenes',
     is_flag=True,
     flag_value=True,
     help='Drop scenes shorter than `min-scene-len` instead of combining them with neighbors.%s' %
     (USER_CONFIG.get_help_string('global', 'drop-short-scenes')),
 )
 @click.option(
+    '--merge-last-scene',
+    is_flag=True,
+    flag_value=True,
+    help='Merge last scene with previous if shorter than min-scene-len.%s' %
+    (USER_CONFIG.get_help_string('global', 'merge-last-scene')),
+)
+@click.option(
     '--stats',
     '-s',
     metavar='CSV',
     type=click.Path(exists=False, file_okay=True, writable=True, resolve_path=False),
     help='Path to stats file (.csv) for writing frame metrics to. If the file exists, any'
     ' metrics will be processed, otherwise a new file will be created. Can be used to determine'
     ' optimal values for various scene detector options, and to cache frame calculations in order'
@@ -213,15 +220,16 @@
 )
 @click.option(
     '--backend',
     '-b',
     metavar='BACKEND',
     type=click.Choice(CHOICE_MAP["global"]["backend"]),
     default=None,
-    help='Name of backend to use for video input. Backends available on this system: %s.%s' %
+    help='Backend to use for video input. Backends can be configured using -c/--config. Backends'
+    ' available on this system: %s.%s.' %
     (', '.join(AVAILABLE_BACKENDS.keys()), USER_CONFIG.get_help_string("global", "backend")),
 )
 @click.option(
     '--config',
     '-c',
     metavar='FILE',
     type=click.Path(exists=True, file_okay=True, readable=True, resolve_path=False),
@@ -234,14 +242,15 @@
     input: Optional[AnyStr],
     output: Optional[AnyStr],
     framerate: Optional[float],
     downscale: Optional[int],
     frame_skip: Optional[int],
     min_scene_len: Optional[str],
     drop_short_scenes: bool,
+    merge_last_scene: bool,
     stats: Optional[AnyStr],
     verbosity: Optional[str],
     logfile: Optional[AnyStr],
     quiet: bool,
     backend: Optional[str],
     config: Optional[AnyStr],
 ):
@@ -262,14 +271,15 @@
         output=output,
         framerate=framerate,
         stats_file=stats,
         downscale=downscale,
         frame_skip=frame_skip,
         min_scene_len=min_scene_len,
         drop_short_scenes=drop_short_scenes,
+        merge_last_scene=merge_last_scene,
         backend=backend,
         quiet=quiet,
         logfile=logfile,
         config=config,
         stats=stats,
         verbosity=verbosity,
     )
```

### Comparing `scenedetect-0.6.dev3/scenedetect/cli/config.py` & `scenedetect-0.6rc0/scenedetect/cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 
 Handles loading configuration files from disk and validating each section. Only validation
 of the config file schema and data types are performed. Constants/defaults are also defined
 here where possible and re-used by the CLI so that there is one source of truth.
 """
 
 import logging
+import os
 import os.path
 from configparser import ConfigParser
 from typing import AnyStr, Dict, List, Optional, Tuple, Union
 
 from appdirs import user_config_dir
 
-from scenedetect.backends import PREFERRED_BACKENDS
+from scenedetect.backends.pyav import VALID_THREAD_MODES
 from scenedetect.frame_timecode import FrameTimecode
 
 
 class TimecodeValue:
 
     def __init__(self, value: Union[int, str]):
         self.value = value
@@ -64,18 +65,22 @@
 ConfigDict = Dict[str, Dict[str, ConfigValue]]
 
 _CONFIG_FILE_NAME: AnyStr = 'scenedetect.cfg'
 _CONFIG_FILE_DIR: AnyStr = user_config_dir("PySceneDetect", False)
 
 CONFIG_FILE_PATH: AnyStr = os.path.join(_CONFIG_FILE_DIR, _CONFIG_FILE_NAME)
 
-_DEFAULT_BACKENDS: str = 'try %s in order' % ', '.join(
-    backend_type for backend_type in PREFERRED_BACKENDS)
-
 CONFIG_MAP: ConfigDict = {
+    'backend-opencv': {
+        'max-decode-attempts': 5,
+    },
+    'backend-pyav': {
+        'suppress-output': False,
+        'threading-mode': 'auto',
+    },
     'detect-adaptive': {
         'frame-window': 2,
         'luma-only': False,
         'min-delta-hsv': RangeValue(15.0, min_val=0.0, max_val=255.0),
         'min-scene-len': TimecodeValue(0),
         'threshold': RangeValue(3.0, min_val=0.0, max_val=255.0),
     },
@@ -100,41 +105,43 @@
         'output': '',
         'filename': '$VIDEO_NAME-Scenes.csv',
         'no-output-file': False,
         'quiet': False,
         'skip-cuts': False,
     },
     'global': {
-        'backend': _DEFAULT_BACKENDS,
+        'backend': 'opencv',
         'downscale': 0,
         'drop-short-scenes': False,
         'frame-skip': 0,
+        'merge-last-scene': False,
         'min-scene-len': TimecodeValue('0.6s'),
         'output': '',
         'verbosity': 'info',
     },
     'save-images': {
         'output': '',
         'filename': '$VIDEO_NAME-Scene-$SCENE_NUMBER-$IMAGE_NUMBER',
         'num-images': 3,
         'format': 'jpeg',
-        'quality': RangeValue(95, 0, 100),
-        'compression': RangeValue(3, 0, 9),
+        # Default value of quality is unused as it depends on the format.
+        'quality': RangeValue(0, min_val=0, max_val=100),
+        'compression': RangeValue(3, min_val=0, max_val=9),
         'frame-margin': 1,
         'scale': 1.0,
         'height': 0,
         'width': 0,
     },
     'split-video': {
         'args': "-c:v libx264 -preset veryfast -crf 22 -c:a aac",
         'copy': False,
         'filename': '$VIDEO_NAME-Scene-$SCENE_NUMBER',
         'high-quality': False,
         'mkvmerge': False,
-        'output': '/usr/tmp/encoded',
+        'output': '',
         'preset': 'veryfast',
         'quiet': False,
         'rate-factor': RangeValue(22, min_val=0, max_val=100),
     },
 }
 """Mapping of valid configuration file parameters and their default values or placeholders.
 The types of these values are used when decoding the configuration file. Valid choices for
@@ -149,18 +156,22 @@
         'preset': [
             'ultrafast', 'superfast', 'veryfast', 'faster', 'fast', 'medium', 'slow', 'slower',
             'veryslow'
         ],
     },
     'save-images': {
         'format': ['jpeg', 'png', 'webp'],
-    }
+    },
+    'backend-pyav': {
+        'threading_mode': [str(mode).lower() for mode in VALID_THREAD_MODES],
+    },
 }
 """Mapping of string options which can only be of a particular set of values. We use a list instead
-of a set to preserve order when generating error contexts."""
+of a set to preserve order when generating error contexts. Values are case-insensitive, and must be
+in lowercase in this map."""
 
 
 def _validate_structure(config: ConfigParser) -> List[str]:
     """Validates the layout of the section/option mapping.
 
     Returns:
         List of any parsing errors in human-readable form.
```

### Comparing `scenedetect-0.6.dev3/scenedetect/cli/context.py` & `scenedetect-0.6rc0/scenedetect/cli/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,54 +18,57 @@
 from __future__ import print_function
 import logging
 import os
 from typing import AnyStr, Optional, Union
 
 import click
 
-from scenedetect.backends import open_video, AVAILABLE_BACKENDS
+from scenedetect import open_video, AVAILABLE_BACKENDS
 from scenedetect.cli.config import ConfigRegistry, ConfigLoadFailure, CHOICE_MAP
 from scenedetect.frame_timecode import FrameTimecode, MAX_FPS_DELTA
 import scenedetect.detectors
 from scenedetect.platform import get_and_create_path, get_cv2_imwrite_params, init_logger
 from scenedetect.scene_manager import SceneManager
-from scenedetect.stats_manager import StatsManager, StatsFileCorrupt
+from scenedetect.stats_manager import StatsManager
 from scenedetect.video_stream import VideoStream, VideoOpenFailure, FrameRateUnavailable
 from scenedetect.video_splitter import is_mkvmerge_available, is_ffmpeg_available
 
 logger = logging.getLogger('pyscenedetect')
 
 USER_CONFIG = ConfigRegistry()
 
 
-def parse_timecode(value: Union[str, int, FrameTimecode], frame_rate: float) -> FrameTimecode:
+def parse_timecode(value: str, frame_rate: float, first_index_is_one: bool = False) -> FrameTimecode:
     """Parses a user input string into a FrameTimecode assuming the given framerate.
 
     If value is None, None will be returned instead of processing the value.
 
     Raises:
         click.BadParameter
      """
     if value is None:
         return None
     try:
+        if first_index_is_one and value.isdigit():
+            value = int(value)
+            if value >= 1:
+                value -= 1
         return FrameTimecode(timecode=value, fps=frame_rate)
     except ValueError as ex:
         raise click.BadParameter(
             'timecode must be in frames (1234), seconds (123.4s), or HH:MM:SS (00:02:03.400)'
         ) from ex
 
 
 def contains_sequence_or_url(video_path: str) -> bool:
     """Checks if the video path is a URL or image sequence."""
     return '%' in video_path or '://' in video_path
 
 
 def check_split_video_requirements(use_mkvmerge: bool) -> None:
-    # type: (bool) -> None
     """ Validates that the proper tool is available on the system to perform the
     `split-video` command.
 
     Arguments:
         use_mkvmerge: True if mkvmerge (-m), False otherwise.
 
     Raises: click.BadParameter if the proper video splitting tool cannot be found.
@@ -108,14 +111,15 @@
         self.stats_manager: StatsManager = None
 
         # Main `scenedetect` Options
         self.output_directory: str = None        # -o/--output
         self.quiet_mode: bool = None             # -q/--quiet or -v/--verbosity quiet
         self.stats_file_path: str = None         # -s/--stats
         self.drop_short_scenes: bool = None      # --drop-short-scenes
+        self.merge_last_scene: bool = None       # --merge-last-scene
         self.min_scene_len: FrameTimecode = None # -m/--min-scene-len
         self.frame_skip: int = None              # -fs/--frame-skip
 
         # `time` Command Options
         self.time: bool = False
         self.start_time: FrameTimecode = None # time -s/--start
         self.end_time: FrameTimecode = None   # time -e/--end
@@ -170,14 +174,15 @@
         output: Optional[AnyStr],
         framerate: float,
         stats_file: Optional[AnyStr],
         downscale: Optional[int],
         frame_skip: int,
         min_scene_len: str,
         drop_short_scenes: bool,
+        merge_last_scene: bool,
         backend: Optional[str],
         quiet: bool,
         logfile: Optional[AnyStr],
         config: Optional[AnyStr],
         stats: Optional[AnyStr],
         verbosity: Optional[str],
     ):
@@ -212,16 +217,16 @@
                 if log_level >= logging.ERROR:
                     init_failure = True
             if init_failure:
                 logger.critical("Error processing configuration file.")
                 raise click.Abort()
 
         logger.debug("Current configuration:\n%s", str(self.config.config_dict))
-        logger.debug('Parsing program options.')
 
+        logger.debug('Parsing program options.')
         if stats is not None and frame_skip:
             error_strs = [
                 'Unable to detect scenes with stats file if frame skip is not 0.',
                 '  Either remove the -fs/--frame-skip option, or the -s/--stats file.\n'
             ]
             logger.error('\n'.join(error_strs))
             raise click.BadParameter(
@@ -243,19 +248,22 @@
             logger.info('Output directory set:\n  %s', self.output_directory)
 
         self.min_scene_len = parse_timecode(
             min_scene_len if min_scene_len is not None else self.config.get_value(
                 "global", "min-scene-len"), self.video_stream.frame_rate)
         self.drop_short_scenes = drop_short_scenes or self.config.get_value(
             "global", "drop-short-scenes")
+        self.merge_last_scene = merge_last_scene or self.config.get_value(
+            "global", "merge-last-scene")
         self.frame_skip = self.config.get_value("global", "frame-skip", frame_skip)
 
-        # Open StatsManager if --stats is specified.
+        # Create StatsManager if --stats is specified.
         if stats_file:
-            self._open_stats_file(file_path=stats_file)
+            self.stats_file_path = get_and_create_path(stats_file, self.output_directory)
+            self.stats_manager = StatsManager()
 
         logger.debug('Initializing SceneManager.')
         self.scene_manager = SceneManager(self.stats_manager)
         if downscale is None and self.config.is_default("global", "downscale"):
             self.scene_manager.auto_downscale = True
         else:
             try:
@@ -364,15 +372,15 @@
                     min_scene_len = self.min_scene_len.frame_num
                 else:
                     min_scene_len = self.config.get_value("detect-threshold", "min-scene-len")
             min_scene_len = parse_timecode(min_scene_len, self.video_stream.frame_rate).frame_num
 
         threshold = self.config.get_value("detect-threshold", "threshold", threshold)
         fade_bias = self.config.get_value("detect-threshold", "fade-bias", fade_bias)
-        # TODO: This cannot be disabled right now.
+        # TODO(v1.0): This cannot be disabled right now.
         add_last_scene = add_last_scene or self.config.get_value("detect-threshold",
                                                                  "add-last-scene")
 
         logger.debug(
             'Adding detector: ThresholdDetector(threshold=%f, fade_bias=%f,'
             ' min_scene_len=%d, add_last_scene=%s)', threshold, fade_bias, min_scene_len,
             add_last_scene)
@@ -527,17 +535,14 @@
             logger.info('Using mkvmerge for video splitting.')
             self.options_processed = options_processed_orig
             return
 
         ##
         ## ffmpeg-Specific Arguments/Options
         ##
-        # TODO: Should add some validation of the name format to ensure it contains at
-        # least one variable, otherwise the output will just keep getting overwritten.
-
         if copy:
             args = '-c:v copy -c:a copy'
         elif not args:
             if rate_factor is None:
                 rate_factor = 22 if not high_quality else 17
             if preset is None:
                 preset = 'veryfast' if not high_quality else 'slow'
@@ -569,16 +574,16 @@
         """Handle `save-images` command options."""
         self._check_input_open()
         if self.save_images:
             self._on_duplicate_command('save-images')
         options_processed_orig = self.options_processed
         self.options_processed = False
 
-        if contains_sequence_or_url(self.video_stream.path):
-            error_str = '\nThe save-images command is incompatible with image sequences/URLs.'
+        if '://' in self.video_stream.path:
+            error_str = '\nThe save-images command is incompatible with URLs.'
             logger.error(error_str)
             raise click.BadParameter(error_str, param_hint='save-images')
 
         num_flags = sum([1 if flag else 0 for flag in [jpeg, webp, png]])
         if num_flags > 1:
             logger.error('Multiple image type flags set for save-images command.')
             raise click.BadParameter(
@@ -596,15 +601,19 @@
             self.height = self.config.get_value('save-images', 'height')
             self.width = self.config.get_value('save-images', 'width')
         else:
             self.scale = scale
             self.height = height
             self.width = width
 
-        quality = self.config.get_value('save-images', 'quality', 100 if webp else 95)
+        default_quality = 100 if webp else 95
+        quality = (
+            default_quality if self.config.is_default('save-images', 'quality') else
+            self.config.get_value('save-images', 'quality'))
+
         compression = self.config.get_value('save-images', 'compression', compression)
         self.image_param = compression if png else quality
 
         self.image_extension = 'jpg' if jpeg else 'png' if png else 'webp'
         valid_params = get_cv2_imwrite_params()
         if not self.image_extension in valid_params or valid_params[self.image_extension] is None:
             error_strs = [
@@ -646,17 +655,17 @@
             raise click.BadParameter(
                 'Only one of --duration/-d or --end/-e can be specified, not both.',
                 param_hint='time')
 
         logger.debug('Setting video time:\n    start: %s, duration: %s, end: %s', start, duration,
                      end)
 
-        self.start_time = parse_timecode(start, self.video_stream.frame_rate)
-        self.end_time = parse_timecode(end, self.video_stream.frame_rate)
-        self.duration = parse_timecode(duration, self.video_stream.frame_rate)
+        self.start_time = parse_timecode(start, self.video_stream.frame_rate, first_index_is_one=True)
+        self.end_time = parse_timecode(end, self.video_stream.frame_rate, first_index_is_one=True)
+        self.duration = parse_timecode(duration, self.video_stream.frame_rate, first_index_is_one=True)
         self.time = True
 
         self.options_processed = options_processed_orig
 
     #
     # Private Methods
     #
@@ -730,63 +739,66 @@
                 logger.error('Error: No input video (-i/--input) was specified.')
             self._check_input_open_failed = True
             self.options_processed = False
             raise click.Abort()
 
     def _open_video_stream(self, input_path: AnyStr, framerate: Optional[float],
                            backend: Optional[str]):
+        if '%' in input_path and backend != 'opencv':
+            raise click.BadParameter(
+                'The OpenCV backend (`--backend opencv`) must be used to process image sequences.',
+                param_hint='-i/--input')
         if framerate is not None and framerate < MAX_FPS_DELTA:
             raise click.BadParameter('Invalid framerate specified!', param_hint='-f/--framerate')
         try:
-            if backend is not None:
+            if backend is None:
+                backend = self.config.get_value('global', 'backend')
+            else:
                 if not backend in AVAILABLE_BACKENDS:
                     raise click.BadParameter(
                         'Specified backend %s is not available on this system!' % backend,
                         param_hint='-b/--backend')
-                self.video_stream = AVAILABLE_BACKENDS[backend](input_path, framerate)
+            # Open the video with the specified backend, loading any required config settings.
+            if backend == 'pyav':
+                self.video_stream = open_video(
+                    path=input_path,
+                    framerate=framerate,
+                    backend=backend,
+                    threading_mode=self.config.get_value('backend-pyav', 'threading-mode'),
+                    suppress_output=self.config.get_value('backend-pyav', 'suppress-output'),
+                )
+            elif backend == 'opencv':
+                self.video_stream = open_video(
+                    path=input_path,
+                    framerate=framerate,
+                    backend=backend,
+                    max_decode_attempts=self.config.get_value('backend-opencv',
+                                                              'max-decode-attempts'),
+                )
+            # Handle backends without any config options.
             else:
-                self.video_stream = open_video(path=input_path, framerate=framerate)
+                self.video_stream = open_video(
+                    path=input_path,
+                    framerate=framerate,
+                    backend=backend,
+                )
             logger.debug('Video opened using backend %s', type(self.video_stream).__name__)
         except FrameRateUnavailable as ex:
             raise click.BadParameter(
                 'Failed to obtain framerate for input video. Manually specify framerate with the'
                 ' -f/--framerate option, or try re-encoding the file.',
                 param_hint='-i/--input') from ex
         except VideoOpenFailure as ex:
             raise click.BadParameter(
                 'Failed to open input video%s: %s' %
                 (' using %s backend' % backend if backend else '', str(ex)),
                 param_hint='-i/--input') from ex
         except OSError as ex:
             raise click.BadParameter('Input error:\n\n\t%s\n' % str(ex), param_hint='-i/--input')
 
-    def _open_stats_file(self, file_path: str):
-        """Initializes this object's StatsManager, loading any existing stats from disk.
-        If the file does not already exist, all directories leading up to it's eventual
-        location will be created here."""
-        self.stats_file_path = get_and_create_path(file_path, self.output_directory)
-        self.stats_manager = StatsManager()
-
-        logger.info('Loading frame metrics from stats file: %s',
-                    os.path.basename(self.stats_file_path))
-        try:
-            self.stats_manager.load_from_csv(self.stats_file_path)
-        except StatsFileCorrupt:
-            error_info = (
-                'Could not load frame metrics from stats file - file is either corrupt,'
-                ' or not a valid PySceneDetect stats file. If the file exists, ensure that'
-                ' it is a valid stats file CSV, otherwise delete it and run PySceneDetect'
-                ' again to re-generate the stats file.')
-            error_strs = ['Could not load stats file.', 'Failed to parse stats file:', error_info]
-            logger.error('\n'.join(error_strs))
-            # pylint: disable=raise-missing-from
-            raise click.BadParameter(
-                '\n  Could not load given stats file, see above output for details.',
-                param_hint='input stats file')
-
     def _on_duplicate_command(self, command: str) -> None:
         """Called when a command is duplicated to stop parsing and raise an error.
 
         Arguments:
             command: Command that was duplicated for error context.
 
         Raises:
```

### Comparing `scenedetect-0.6.dev3/scenedetect/cli/controller.py` & `scenedetect-0.6rc0/scenedetect/cli/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 This file contains the implementation of the PySceneDetect command-line logic.
 """
 
 import logging
 import os
 from string import Template
 import time
+import threading
 from typing import Dict, List, Tuple, Optional
 
-import cv2
-
-from scenedetect.backends import VideoStreamCv2
 from scenedetect.cli.context import CliContext, check_split_video_requirements
 from scenedetect.frame_timecode import FrameTimecode
 from scenedetect.platform import get_and_create_path
 from scenedetect.scene_manager import save_images, write_scene_list, write_scene_list_html
 from scenedetect.video_splitter import split_video_mkvmerge, split_video_ffmpeg
 
 logger = logging.getLogger('pyscenedetect')
@@ -47,39 +45,29 @@
         logger.debug('CLI options were not parsed successfully.')
         return
     if context.scene_manager.get_num_detectors() == 0:
         logger.error('No scene detectors specified (detect-content, detect-threshold, etc...),\n'
                      ' or failed to process all command line arguments.')
         return
 
-    # Display a warning if the video codec type seems unsupported (#86).
-    if isinstance(context.video_stream, VideoStreamCv2):
-        if int(abs(context.video_stream.capture.get(cv2.CAP_PROP_FOURCC))) == 0:
-            logger.error(
-                'Video codec detection failed, output may be incorrect.\nThis could be caused'
-                ' by using an outdated version of OpenCV, or using codecs that currently are'
-                ' not well supported (e.g. VP9).\n'
-                'As a workaround, consider re-encoding the source material before processing.\n'
-                'For details, see https://github.com/Breakthrough/PySceneDetect/issues/86')
-
     perf_start_time = time.time()
     if context.start_time is not None:
         logger.debug('Seeking to start time...')
         context.video_stream.seek(target=context.start_time)
 
     logger.info('Detecting scenes...')
     num_frames = context.scene_manager.detect_scenes(
         video=context.video_stream,
         duration=context.duration,
         end_time=context.end_time,
         frame_skip=context.frame_skip,
         show_progress=not context.quiet_mode)
 
     # Handle case where video failure is most likely due to multiple audio tracks (#179).
-    if num_frames <= 0:
+    if num_frames <= 0 and context.video_stream.BACKEND_NAME == 'opencv':
         logger.critical(
             'Failed to read any frames from video file. This could be caused by the video'
             ' having multiple audio tracks. If so, try installing the PyAV backend:\n'
             '      pip install av\n'
             'Or remove the audio tracks by running either:\n'
             '      ffmpeg -i input.mp4 -c copy -an output.mp4\n'
             '      mkvmerge -o output.mkv input.mp4\n'
@@ -95,14 +83,20 @@
     _save_stats(context)
 
     # Get list of detected cuts/scenes from the SceneManager to generate the required output
     # files, based on the given commands (list-scenes, split-video, save-images, etc...).
     cut_list = context.scene_manager.get_cut_list()
     scene_list = context.scene_manager.get_scene_list(start_in_scene=True)
 
+    # Handle --merge-last-scene.
+    if context.merge_last_scene and context.min_scene_len is not None and context.min_scene_len > 0:
+        if len(scene_list) > 1 and (scene_list[-1][1] - scene_list[-1][0]) < context.min_scene_len:
+            new_last_scene = (scene_list[-2][0], scene_list[-1][1])
+            scene_list = scene_list[:-2] + [new_last_scene]
+
     # Handle --drop-short-scenes.
     if context.drop_short_scenes and context.min_scene_len > 0:
         scene_list = [s for s in scene_list if (s[1] - s[0]) >= context.min_scene_len]
 
     # Ensure we don't divide by zero.
     if scene_list:
         logger.info(
@@ -128,15 +122,15 @@
 def _save_stats(context: CliContext) -> None:
     """Handles saving the statsfile if -s/--stats was specified."""
     if context.stats_file_path is not None:
         # We check if the save is required in order to reduce unnecessary log messages.
         if context.stats_manager.is_save_required():
             logger.info('Saving frame metrics to stats file: %s',
                         os.path.basename(context.stats_file_path))
-            context.stats_manager.save_to_csv(path=context.stats_file_path)
+            context.stats_manager.save_to_csv(csv_file=context.stats_file_path)
         else:
             logger.debug('No frame metrics updated, skipping update of the stats file.')
 
 
 def _list_scenes(context: CliContext, scene_list: List[Tuple[FrameTimecode, FrameTimecode]],
                  cut_list: List[FrameTimecode]) -> None:
     """Handles the `list-scenes` command."""
@@ -162,16 +156,17 @@
 -----------------------------------------------------------------------
  | Scene # | Start Frame |  Start Time  |  End Frame  |   End Time   |
 -----------------------------------------------------------------------
 %s
 -----------------------------------------------------------------------
 """, '\n'.join([
                 ' |  %5d  | %11d | %s | %11d | %s |' %
-                (i + 1, start_time.get_frames(), start_time.get_timecode(), end_time.get_frames(),
-                 end_time.get_timecode()) for i, (start_time, end_time) in enumerate(scene_list)
+                (i + 1, start_time.get_frames() + 1, start_time.get_timecode(),
+                 end_time.get_frames(), end_time.get_timecode())
+                for i, (start_time, end_time) in enumerate(scene_list)
             ]))
 
     if cut_list:
         logger.info('Comma-separated timecode list:\n  %s',
                     ','.join([cut.get_timecode() for cut in cut_list]))
```

### Comparing `scenedetect-0.6.dev3/scenedetect/detectors/__init__.py` & `scenedetect-0.6rc0/scenedetect/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/detectors/adaptive_detector.py` & `scenedetect-0.6rc0/scenedetect/detectors/adaptive_detector.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,32 +14,52 @@
 similar to `ContentDetector` except the threshold isn't fixed, but is a rolling average of
 adjacent frame changes. This can help mitigate false detections in situations such as fast
 camera motions.
 
 This detector is available from the command-line as the `detect-adaptive` command.
 """
 
+from logging import getLogger
+
 # PySceneDetect Library Imports
 from scenedetect.detectors import ContentDetector
 
+logger = getLogger('pyscenedetect')
 
 class AdaptiveDetector(ContentDetector):
     """Detects cuts using HSV changes similar to ContentDetector, but with a
     rolling average that can help mitigate false detections in situations such
     as camera moves.
     """
 
     ADAPTIVE_RATIO_KEY_TEMPLATE = "adaptive_ratio{luma_only} (w={window_width})"
 
     def __init__(self,
                  adaptive_threshold=3.0,
                  luma_only=False,
                  min_scene_len=15,
                  min_delta_hsv=15.0,
-                 window_width=2):
+                 window_width=2,
+                 video_manager=None):
+        """
+        Arguments:
+            adaptive_threshold: Threshold value (float) that the calculated frame score must exceed to
+                trigger a new scene (see frame metric adaptive_ratio in stats file).
+            luma_only: Only consider luma/brightness channel (useful for greyscale videos).
+            min_scene_len: Minimum length of any scene.
+            min_delta_hsv: Minimum threshold (float) that the content_val must exceed in order to register as a new'
+                scene. This is calculated the same way that `detect-content` calculates frame score.
+            window_width: Size of window (number of frames) before and after each frame to average together in'
+                order to detect deviations from the mean.
+            video_manager: [DEPRECATED] DO NOT USE. For backwards compatibility only.
+        """
+        # TODO: Remove `video_manager`.
+        if video_manager is not None:
+            logger.error('video_manager is deprecated, use video instead.')
+
         super().__init__()
         self.min_scene_len = min_scene_len                                              # minimum length of any given scene, in frames (int) or FrameTimecode
         self.adaptive_threshold = adaptive_threshold
         self.min_delta_hsv = min_delta_hsv
         self.window_width = window_width
         self._luma_only = luma_only
         self._adaptive_ratio_key = AdaptiveDetector.ADAPTIVE_RATIO_KEY_TEMPLATE.format(
```

### Comparing `scenedetect-0.6.dev3/scenedetect/detectors/content_detector.py` & `scenedetect-0.6rc0/scenedetect/detectors/content_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,22 @@
     """
 
     FRAME_SCORE_KEY = 'content_val'
     DELTA_H_KEY, DELTA_S_KEY, DELTA_V_KEY = ('delta_hue', 'delta_sat', 'delta_lum')
     METRIC_KEYS = [FRAME_SCORE_KEY, DELTA_H_KEY, DELTA_S_KEY, DELTA_V_KEY]
 
     def __init__(self, threshold: float = 27.0, min_scene_len: int = 15, luma_only: bool = False):
-        """Construct a `ContentDetector`.
-
+        """
         Arguments:
             threshold: Threshold the average change in pixel intensity must exceed to trigger a cut.
             min_scene_len: Once a cut is detected, this many frames must pass before a new one can
                 be added to the scene list.
             luma_only: If True, only considers changes in the luminance channel of the video. The
                 default is False, which considers changes in hue, saturation, and luma.
         """
-        #
-        #  type: (float, Union[int, FrameTimecode]) -> None
         super().__init__()
         self.threshold = threshold
         # Minimum length of any given scene, in frames (int) or FrameTimecode
         self.min_scene_len = min_scene_len
         self.luma_only = luma_only
         self.last_frame = None
         self.last_scene_cut = None
@@ -120,15 +117,14 @@
                 detection on. Can be None *only* if the self.is_processing_required() method
                 (inhereted from the base SceneDetector class) returns True.
 
         Returns:
             List of frames where scene cuts have been detected. There may be 0
             or more frames in the list, and not necessarily the same as frame_num.
         """
-
         cut_list = []
         _unused = ''
 
         # Initialize last scene cut point at the beginning of the frames of interest.
         if self.last_scene_cut is None:
             self.last_scene_cut = frame_num
 
@@ -168,13 +164,14 @@
                 and self.stats_manager.metrics_exist(frame_num + 1, self.get_metrics())):
             self.last_frame = _unused
         else:
             self.last_frame = frame_img.copy()
 
         return cut_list
 
+    # TODO(#250): Based on the parameters passed to the ContentDetector constructor,
+    # ensure that the last scene meets the minimum length requirement, otherwise it
+    # should be merged with the previous scene.
+
     #def post_process(self, frame_num):
-    #    """ TODO: Based on the parameters passed to the ContentDetector constructor,
-    #        ensure that the last scene meets the minimum length requirement,
-    #        otherwise it should be merged with the previous scene.
     #    """
     #    return []
```

### Comparing `scenedetect-0.6.dev3/scenedetect/detectors/motion_detector.py` & `scenedetect-0.6rc0/scenedetect/detectors/motion_detector.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/detectors/threshold_detector.py` & `scenedetect-0.6rc0/scenedetect/detectors/threshold_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 #
 """:py:class:`ThresholdDetector` uses a set intensity as a threshold to detect cuts, which
 are triggered when the average pixel intensity exceeds or falls below this threshold.
 
 This detector is available from the command-line as the `detect-threshold` command.
 """
 
+from logging import getLogger
 from typing import List
 
 import numpy
 
 from scenedetect.scene_detector import SceneDetector
 
+logger = getLogger('pyscenedetect')
+
 ##
 ## ThresholdDetector Helper Functions
 ##
 
 
 def compute_frame_average(frame: numpy.ndarray) -> float:
     """Computes the average pixel value/intensity for all pixels in a frame.
@@ -54,33 +57,41 @@
 
     Detects both fast cuts and slow fades so long as an appropriate threshold
     is chosen (especially taking into account the minimum grey/black level).
     """
 
     THRESHOLD_VALUE_KEY = 'delta_rgb'
 
-    def __init__(self,
-                 threshold: float = 12,
-                 min_scene_len: int = 15,
-                 fade_bias: float = 0.0,
-                 add_final_scene: bool = False):
-        """Construct a `ThresholdDetector`.
-
+    def __init__(
+        self,
+        threshold: float = 12,
+        min_scene_len: int = 15,
+        fade_bias: float = 0.0,
+        add_final_scene: bool = False,
+        block_size=None,
+    ):
+        """
         Arguments:
             threshold:  8-bit intensity value that each pixel value (R, G, and B)
                 must be <= to in order to trigger a fade in/out.
             min_scene_len:  FrameTimecode object or integer greater than 0 of the
                 minimum length, in frames, of a scene (or subsequent scene cut).
             fade_bias:  Float between -1.0 and +1.0 representing the percentage of
                 timecode skew for the start of a scene (-1.0 causing a cut at the
                 fade-to-black, 0.0 in the middle, and +1.0 causing the cut to be
                 right at the position where the threshold is passed).
             add_final_scene:  Boolean indicating if the video ends on a fade-out to
                 generate an additional scene at this timecode.
+            block_size: [DEPRECATED] DO NOT USE. For backwards compatibility.
         """
+        # TODO: Remove `block_size`.
+        if block_size is not None:
+            logger.error('block_size is deprecated.')
+
+
         super().__init__()
         self.threshold = int(threshold)
         self.fade_bias = fade_bias
         self.min_scene_len = min_scene_len
         self.processed_frame = False
         self.last_scene_cut = None
         # Whether to add an additional scene or not when ending on a fade out
```

### Comparing `scenedetect-0.6.dev3/scenedetect/frame_timecode.py` & `scenedetect-0.6rc0/scenedetect/frame_timecode.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         If using to compare a :py:class:`FrameTimecode` with a frame number,
         you can do so directly against the object (e.g. ``FrameTimecode(10, 10.0) <= 10``).
 
         Returns:
             int: The current time in frames (the current frame number).
         """
-        return int(self.frame_num)
+        return self.frame_num
 
     # TODO(v1.0): Add a `framerate` property to replace the existing one and deprecate this getter.
     def get_framerate(self) -> float:
         """Get Framerate: Returns the framerate used by the FrameTimecode object.
 
         Returns:
             float: Framerate of the current FrameTimecode object, in frames per second.
@@ -177,15 +177,15 @@
         """Convert the passed value seconds to the nearest number of frames using
         the current FrameTimecode object's FPS (self.framerate).
 
         Returns:
             Integer number of frames the passed number of seconds represents using
             the current FrameTimecode's framerate property.
         """
-        return int(seconds * self.framerate)
+        return round(seconds * self.framerate)
 
     def _parse_timecode_number(self, timecode: Union[int, float]) -> int:
         """ Parse a timecode number, storing it as the exact number of frames.
         Can be passed as frame number (int), seconds (float)
 
         Raises:
             TypeError, ValueError
@@ -227,15 +227,15 @@
         if timecode_string.endswith('s'):
             secs = timecode_string[:-1]
             if not secs.replace('.', '').isdigit():
                 raise ValueError('All characters in timecode seconds string must be digits.')
             secs = float(secs)
             if secs < 0.0:
                 raise ValueError('Timecode seconds value must be positive.')
-            return int(secs * self.framerate)
+            return self._seconds_to_frames(secs)
         # Exact number of frames N
         elif timecode_string.isdigit():
             timecode = int(timecode_string)
             if timecode < 0:
                 raise ValueError('Timecode frame number must be positive.')
             return timecode
         # Standard timecode in string format 'HH:MM:SS[.nnn]'
@@ -245,15 +245,15 @@
                     and tc_val[2].replace('.', '').isdigit()):
                 raise ValueError('Unrecognized or improperly formatted timecode string.')
             hrs, mins = int(tc_val[0]), int(tc_val[1])
             secs = float(tc_val[2]) if '.' in tc_val[2] else int(tc_val[2])
             if not (hrs >= 0 and mins >= 0 and secs >= 0 and mins < 60 and secs < 60):
                 raise ValueError('Invalid timecode range (values outside allowed range).')
             secs += (((hrs * 60.0) + mins) * 60.0)
-            return int(secs * self.framerate)
+            return self._seconds_to_frames(secs)
 
     def __iadd__(self, other: Union[int, float, str, 'FrameTimecode']) -> 'FrameTimecode':
         if isinstance(other, int):
             self.frame_num += other
         elif isinstance(other, FrameTimecode):
             if self.equal_framerate(other.framerate):
                 self.frame_num += other.frame_num
```

### Comparing `scenedetect-0.6.dev3/scenedetect/platform.py` & `scenedetect-0.6rc0/scenedetect/platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,17 @@
 DLLs on Windows and getting uniform line-terminating csv reader/writer objects
 are also included in this module.
 """
 
 import logging
 import os
 import os.path
-import platform
-import struct
 import subprocess
 import sys
-from typing import AnyStr, Dict, List, Optional, TextIO, Tuple, Union
+from typing import AnyStr, Dict, List, Optional, Union
 
 import cv2
 
 ##
 ## tqdm Library (`scenedetect.platform.tqdm`` will be tqdm object type or None)
 ##
 
@@ -41,14 +39,15 @@
     from tqdm import tqdm
 except ModuleNotFoundError:
     tqdm = None
 # pylint: enable=unused-import
 # pylint: enable=invalid-name
 
 
+# TODO: Move this into scenedetect.backends.opencv.
 def get_aspect_ratio(cap: cv2.VideoCapture, epsilon: float = 0.01) -> float:
     """ Compatibility fix for OpenCV < v3.4.1 to get the aspect ratio
     of a video. For older versions, this function always returns 1.0.
 
     Arguments:
         cap: cv2.VideoCapture object. Must be opened and in valid state.
         epsilon: Used to compare numerator/denominator to zero.
@@ -69,14 +68,15 @@
 
 
 ##
 ## OpenCV imwrite Supported Image Types & Quality/Compression Parameters
 ##
 
 
+# TODO: Move this into scene_manager.
 def get_cv2_imwrite_params() -> Dict[str, Union[int, None]]:
     """ Get OpenCV imwrite Params: Returns a dict of supported image formats and
     their associated quality/compression parameter index, or None if that format
     is not supported.
 
     Returns:
         Dictionary of supported image formats/extensions ('jpg', 'png', etc...) mapped to the
@@ -101,19 +101,19 @@
 
 
 ##
 ## File I/O
 ##
 
 
-def get_file_name(file_path: AnyStr, include_extension=True) -> AnyStr:
+def get_file_name(file_path: AnyStr, include_extension=True) -> str:
     """Return the file name that `file_path` refers to, optionally removing the extension.
 
     E.g. /tmp/foo.bar -> foo"""
-    file_name = os.path.basename(file_path)
+    file_name = str(os.path.basename(file_path))
     if not include_extension:
         last_dot_pos = file_name.rfind('.')
         if last_dot_pos >= 0:
             file_name = file_name[:last_dot_pos]
     return file_name
 
 
@@ -154,15 +154,16 @@
                 show_stdout: bool = False,
                 log_file: Optional[str] = None):
     """Initializes logging for PySceneDetect. The logger instance used is named 'pyscenedetect'.
     By default the logger has no handlers to suppress output. All existing log handlers are replaced
     every time this function is invoked.
 
     Arguments:
-        log_level: Verbosity of log messages.
+        log_level: Verbosity of log messages. Should be one of [logging.INFO, logging.DEBUG,
+            logging.WARNING, logging.ERROR, logging.CRITICAL].
         show_stdout: If True, add handler to show log messages on stdout (default: False).
         log_file: If set, add handler to dump log messages to given file path.
     """
     # Format of log messages depends on verbosity.
     format_str = '[PySceneDetect] %(message)s'
     if log_level == logging.DEBUG:
         format_str = '%(levelname)s: %(module)s.%(funcName)s(): %(message)s'
```

### Comparing `scenedetect-0.6.dev3/scenedetect/scene_detector.py` & `scenedetect-0.6rc0/scenedetect/scene_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,16 +39,19 @@
     to get an idea of how a particular detector can be created.
     """
 
     stats_manager: Optional[StatsManager] = None
     """Optional :py:class:`StatsManager <scenedetect.stats_manager.StatsManager>` to
     use for caching frame metrics to and from."""
 
+    # TODO(v1.0): Remove - this is a rarely used case for what is now a neglegible performance gain.
     def is_processing_required(self, frame_num: int) -> bool:
-        """Is Processing Required: Test if all calculations for a given frame are already done.
+        """[DEPRECATED] DO NOT USE
+
+        Test if all calculations for a given frame are already done.
 
         Returns:
             False if the SceneDetector has assigned _metric_keys, and the
             stats_manager property is set to a valid StatsManager object containing
             the required frame metrics/calculations for the given frame - thus, not
             needing the frame to perform scene detection.
```

### Comparing `scenedetect-0.6.dev3/scenedetect/scene_manager.py` & `scenedetect-0.6rc0/scenedetect/scene_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         "End Timecode", "End Time (seconds)", "Length (frames)", "Length (timecode)",
         "Length (seconds)"
     ])
     for i, (start, end) in enumerate(scene_list):
         duration = end - start
         csv_writer.writerow([
             '%d' % (i + 1),
-            '%d' % start.get_frames(),
+            '%d' % (start.get_frames() + 1),
             start.get_timecode(),
             '%.3f' % start.get_seconds(),
             '%d' % end.get_frames(),
             end.get_timecode(),
             '%.3f' % end.get_seconds(),
             '%d' % duration.get_frames(),
             duration.get_timecode(),
@@ -246,15 +246,15 @@
         "Length (seconds)"
     ]
     for i, (start, end) in enumerate(scene_list):
         duration = end - start
 
         row = SimpleTableRow([
             '%d' % (i + 1),
-            '%d' % start.get_frames(),
+            '%d' % (start.get_frames() + 1),
             start.get_timecode(),
             '%.3f' % start.get_seconds(),
             '%d' % end.get_frames(),
             end.get_timecode(),
             '%.3f' % end.get_seconds(),
             '%d' % duration.get_frames(),
             duration.get_timecode(),
@@ -291,16 +291,18 @@
                 image_extension: str = 'jpg',
                 encoder_param: int = 95,
                 image_name_template: str = '$VIDEO_NAME-Scene-$SCENE_NUMBER-$IMAGE_NUMBER',
                 output_dir: Optional[str] = None,
                 show_progress: Optional[bool] = False,
                 scale: Optional[float] = None,
                 height: Optional[int] = None,
-                width: Optional[int] = None) -> Dict[int, List[str]]:
-    """ Saves a set number of images from each scene, given a list of scenes
+                width: Optional[int] = None,
+                video_manager = None,
+                ) -> Dict[int, List[str]]:
+    """Save a set number of images from each scene, given a list of scenes
     and the associated video/frame source.
 
     Arguments:
         scene_list: A list of scenes (pairs of FrameTimecode objects) returned
             from calling a SceneManager's detect_scenes() method.
         video: A VideoStream object corresponding to the scene list.
             Note that the video will be closed/re-opened and seeked through.
@@ -327,24 +329,29 @@
             and width will resize images to an exact size, regardless of aspect ratio.
             Specifying only height will rescale the image to that number of pixels in height
             while preserving the aspect ratio.
         width: Optional value for the width of the saved images. Specifying both the width
             and height will resize images to an exact size, regardless of aspect ratio.
             Specifying only width will rescale the image to that number of pixels wide
             while preserving the aspect ratio.
+        video_manager: [DEPRECATED] DO NOT USE. For backwards compatibility only.
 
     Returns:
         Dictionary of the format { scene_num : [image_paths] }, where scene_num is the
         number of the scene in scene_list (starting from 1), and image_paths is a list of
         the paths to the newly saved/created images.
 
     Raises:
         ValueError: Raised if any arguments are invalid or out of range (e.g.
         if num_images is negative).
     """
+    # TODO: Remove `video_manager`.
+    if video_manager is not None:
+        logger.error('video_manager is deprecated, use video instead.')
+        video = video_manager
 
     if not scene_list:
         return {}
     if num_images <= 0 or frame_margin < 0:
         raise ValueError()
 
     # TODO: Validate that encoder_param is within the proper range.
@@ -477,15 +484,15 @@
         """
         self._cutting_list = []
         self._event_list = []
         self._detector_list = []
         self._sparse_detector_list = []
         # TODO(v1.0): This class should own a StatsManager instead of taking an optional one.
         # Expose a new `stats_manager` @property from the SceneManager, and either change the
-        # `stats_manager` argument to to `store_stats: bool=False``, or lazy-init one.
+        # `stats_manager` argument to to `store_stats: bool=False`, or lazy-init one.
 
         # TODO(v1.0): This class should own a VideoStream as well, instead of passing one
         # to the detect_scenes method. If concatenation is required, it can be implemented as
         # a generic VideoStream wrapper.
         self._stats_manager: Optional[StatsManager] = stats_manager
 
         # Position of video that was first passed to detect_scenes.
@@ -582,15 +589,16 @@
     def clear_detectors(self) -> None:
         """ Removes all scene detectors added to the SceneManager via add_detector(). """
         self._detector_list.clear()
         self._sparse_detector_list.clear()
 
     def get_scene_list(self,
                        base_timecode: Optional[FrameTimecode] = None,
-                       start_in_scene: bool = False) -> List[Tuple[FrameTimecode, FrameTimecode]]:
+                       start_in_scene: bool = False,
+                       ) -> List[Tuple[FrameTimecode, FrameTimecode]]:
         """ Returns a list of tuples of start/end FrameTimecodes for each detected scene.
 
         The scene list is generated by combining the results of all sparse detectors with
         those from dense ones (i.e. combining the results of :py:meth:`get_cut_list`
         and :py:meth:`get_event_list`).
 
         Returns:
@@ -681,63 +689,70 @@
 
     def _post_process(self, frame_num: int) -> None:
         """ Adds any remaining cuts to the cutting list after processing the last frame. """
         for detector in self._detector_list:
             self._cutting_list += detector.post_process(frame_num)
 
     def detect_scenes(self,
-                      video: VideoStream,
+                      video: VideoStream = None,
                       duration: Optional[FrameTimecode] = None,
                       end_time: Optional[FrameTimecode] = None,
                       frame_skip: int = 0,
                       show_progress: bool = False,
-                      callback: Optional[Callable[[np.ndarray, int], None]] = None):
+                      callback: Optional[Callable[[np.ndarray, int], None]] = None,
+                      frame_source: Optional[VideoStream] = None) -> int:
         """ Perform scene detection on the given video using the added SceneDetectors.
 
         Blocks until all frames in the video have been processed. Results can
         be obtained by calling either the get_scene_list() or get_cut_list() methods.
         Video decoding is performed in a background thread to allow scene detection and
         frame decoding to happen in parallel.
 
         Arguments:
-            video: A VideoStream object pointing.
+            video: VideoStream obtained from either `scenedetect.open_video`, or by creating
+                one directly (e.g. `scenedetect.backends.opencv.VideoStreamCv2`).
             duration: Maximum amount of frames to detect. If not specified,
                 stream will be processed until end. Cannot be specified if `end_time` is set.
             end_time: Last frame number to process. If not specified,
                 stream will be processed until end. Cannot be specified if `duration` is set.
             frame_skip: Not recommended except for extremely high framerate videos.
                 Number of frames to skip (i.e. process every 1 in N+1 frames,
                 where N is frame_skip, processing only 1/N+1 percent of the video,
                 speeding up the detection time at the expense of accuracy).
                 `frame_skip` **must** be 0 (the default) when using a StatsManager.
             show_progress: If True, and the ``tqdm`` module is available, displays
                 a progress bar with the progress, framerate, and expected time to
                 complete processing the video frame source.
             callback: If set, called after each scene/event detected.
-                TODO(v1.0): Update signature.
+            frame_source: [DEPRECATED] DO NOT USE. For compatibility with previous version.
         Returns:
             int: Number of frames read and processed from the frame source.
         Raises:
             ValueError: `frame_skip` **must** be 0 (the default) if the SceneManager
                 was constructed with a StatsManager object.
         """
-
-        #
+        # Compatibility for v0.5 API.
+        # TODO: Remove default value for `video`` when removing `frame_source`.
+        if frame_source is not None:
+            video = frame_source
+        if video is None:
+            raise TypeError("detect_scenes() missing 1 required positional argument: 'video'")
 
         if frame_skip > 0 and self.stats_manager is not None:
             raise ValueError('frame_skip must be 0 when using a StatsManager.')
         if duration is not None and end_time is not None:
             raise ValueError('duration and end_time cannot be set at the same time!')
         if duration is not None and duration < 0:
             raise ValueError('duration must be greater than or equal to 0!')
         if end_time is not None and end_time < 0:
             raise ValueError('end_time must be greater than or equal to 0!')
 
         self._base_timecode = video.base_timecode
-        # TODO: Fix this properly.
+        # TODO(v1.0): Fix this properly by making SceneManager create and own a StatsManager,
+        # and requiring the framerate to be passed to the StatsManager the constructor.
         if self._stats_manager is not None:
             self._stats_manager._base_timecode = self._base_timecode
         start_frame_num: int = video.frame_number
 
         if duration is not None:
             end_time = duration + start_frame_num
 
@@ -797,14 +812,16 @@
     def _decode_thread(self, video, frame_skip, downscale_factor, end_time, out_queue):
         try:
             while True:
                 frame_im = None
                 # We don't do any kind of locking here since the worst-case of this being wrong
                 # is that we do some extra work, and this function should never mutate any data
                 # (all of which should be modified under the GIL).
+                # TODO(v1.0): This optimization should be removed as it is rarely used and
+                # simplifies the implementation of detection algorithms.
                 if (self._is_processing_required(video.position.frame_num)):
                     frame_im = video.read()
                     if frame_im is False:
                         break
                     if downscale_factor > 1:
                         frame_im = frame_im[::downscale_factor, ::downscale_factor, :]
                 else:
```

### Comparing `scenedetect-0.6.dev3/scenedetect/stats_manager.py` & `scenedetect-0.6rc0/scenedetect/stats_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,21 @@
 for each :py:class:`SceneDetector <scenedetect.scene_detector.SceneDetector>` to read/write
 the metrics calculated for each frame. The :py:class:`StatsManager` must be registered to a
 :py:class:`SceneManager <scenedetect.scene_manager.SceneManager>` by passing it to the
 :py:class:`SceneManager constructor <scenedetect.scene_manager.SceneManager>` as the
 `stats_manager` argument.
 
 The entire :py:class:`StatsManager` can be :py:meth:`saved to <StatsManager.save_to_csv>`
-and :py:meth:`loaded from <StatsManager.load_from_csv>` a human-readable CSV
-file, also allowing both precise determination of the threshold or other optimal values
-for video files.  See the :py:meth:`save_to_csv <StatsManager.save_to_csv>` and
-:py:meth:`load_from_csv <StatsManager.load_from_csv>` methods for more information.
-
-The :py:class:`StatsManager` can also be used to cache the calculation results of the scene
-detectors being used, speeding up subsequent scene detection runs using the same pair of
-:py:class:`SceneManager<scenedetect.scene_manager.SceneManager>`/:py:class:`StatsManager` objects.
+a human-readable CSV file, also allowing both precise determination of the threshold or
+other optimal values for video files.
 """
 
 import csv
 from logging import getLogger
-from typing import Any, Dict, Iterable, List, Optional, TextIO
+from typing import Any, Dict, Iterable, List, Optional, Set, TextIO, Union
 import os.path
 
 from scenedetect.frame_timecode import FrameTimecode
 
 logger = getLogger('pyscenedetect')
 
 ##
@@ -87,42 +81,41 @@
 ##
 ## StatsManager Class Implementation
 ##
 
 
 class StatsManager:
     """Provides a key-value store for frame metrics/calculations which can be used
-    as a cache to speed up subsequent calls to a SceneManager's detect_scenes(...)
-    method. The statistics can be saved to a CSV file, and loaded from disk.
+    for two-pass detection algorithms, as well as saving stats to a CSV file.
 
     Analyzing a statistics CSV file is also very useful for finding the optimal
     algorithm parameters for certain detection methods. Additionally, the data
     may be plotted by a graphing module (e.g. matplotlib) by obtaining the
     metric of interest for a series of frames by iteratively calling get_metrics(),
     after having called the detect_scenes(...) method on the SceneManager object
     which owns the given StatsManager instance.
 
     Only metrics consisting of `float` or `int` should be used currently. All metrics loaded
     from disk are treated as `float`.
     """
 
-    def __init__(self, base_timecode: FrameTimecode=None):
+    def __init__(self, base_timecode: FrameTimecode = None):
         """Initialize a new StatsManager.
 
         Arguments:
             base_timecode: Timecode associated with this object. Must not be None (default value
-                will be removed in v1.0).
+                will be removed in a future release).
         """
         # Frame metrics is a dict of frame (int): metric_dict (Dict[str, float])
         # of each frame metric key and the value it represents (usually float).
-        self._frame_metrics = dict()     # Dict[FrameTimecode, Dict[str, float]]
-        self._registered_metrics = set() # Set of frame metric keys.
-        self._loaded_metrics = set()     # Metric keys loaded from stats file.
-        self._metrics_updated = False    # Flag indicating if metrics require saving.
-        self._base_timecode = base_timecode     # Used for timing calculations.
+        self._frame_metrics: Dict[FrameTimecode, Dict[str, float]] = dict()
+        self._registered_metrics: Set[str] = set()                   # Set of frame metric keys.
+        self._loaded_metrics: Set[str] = set()                       # Metric keys loaded from stats file.
+        self._metrics_updated: bool = False                          # Flag indicating if metrics require saving.
+        self._base_timecode: Optional[FrameTimecode] = base_timecode # Used for timing calculations.
 
     def register_metrics(self, metric_keys: Iterable[str]) -> None:
         """Register a list of metric keys that will be used by the detector.
 
         Used to ensure that multiple detector keys don't overlap.
 
         Raises:
@@ -178,57 +171,55 @@
         Returns:
             bool: True if there are frame metrics/statistics not yet written to disk,
             False otherwise.
         """
         return self._metrics_updated
 
     def save_to_csv(self,
-                    path: str = None,
-                    file: TextIO = None,
+                    csv_file: Union[str, bytes, TextIO],
+                    base_timecode: Optional[FrameTimecode] = None,
                     force_save=True) -> None:
         """ Save To CSV: Saves all frame metrics stored in the StatsManager to a CSV file.
 
         Arguments:
-            path: Path to destination file. Use `file` to pass a file handle instead.
-            file: A file handle opened in write mode (e.g. open('...', 'w')).
-            base_timecode: [DEPRECATED] The base_timecode to use. Not required in v0.6.
+            csv_file: A file handle opened in write mode (e.g. open('...', 'w')) or a path as str.
+            base_timecode: [DEPRECATED] DO NOT USE. For backwards compatibility.
             force_save: If True, writes metrics out even if an update is not required.
 
         Raises:
-            ValueError: If both path and file are specified.
             OSError: If `path` cannot be opened or a write failure occurs.
         """
-
-        if path is not None and file is not None:
-            raise ValueError("Only one of path or file can be specified")
+        # TODO: Remove `base_timecode`.
+        if base_timecode is not None:
+            logger.error('base_timecode is deprecated.')
 
         # Ensure we need to write to the file, and that we have data to do so with.
         if not ((self.is_save_required() or force_save) and self._registered_metrics
                 and self._frame_metrics):
             logger.info("No metrics to save.")
             return
 
         assert self._base_timecode is not None
 
         # If we get a path instead of an open file handle, recursively call ourselves
         # again but with file handle instead of path.
-        if path is not None:
-            with open(path, 'w') as file:
-                return self.save_to_csv(file=file, force_save=force_save)
-        csv_writer = csv.writer(file, lineterminator='\n')
+        if isinstance(csv_file, (str, bytes)):
+            with open(csv_file, 'w') as file:
+                return self.save_to_csv(csv_file=file, force_save=force_save)
+        csv_writer = csv.writer(csv_file, lineterminator='\n')
 
         # Header rows.
         metric_keys = sorted(list(self._registered_metrics.union(self._loaded_metrics)))
         csv_writer.writerow([COLUMN_NAME_FRAME_NUMBER, COLUMN_NAME_TIMECODE] + metric_keys)
         frame_keys = sorted(self._frame_metrics.keys())
         logger.info("Writing %d frames to CSV...", len(frame_keys))
         for frame_key in frame_keys:
             frame_timecode = self._base_timecode + frame_key
             csv_writer.writerow(
-                [frame_timecode.get_frames(),
+                [frame_timecode.get_frames() + 1,
                  frame_timecode.get_timecode()] +
                 [str(metric) for metric in self.get_metrics(frame_key, metric_keys)])
 
     @staticmethod
     def valid_header(row: List[str]) -> bool:
         """Check that the given CSV row is a valid header for a statsfile.
 
@@ -240,41 +231,46 @@
         """
         if not row or not len(row) >= 2:
             return False
         if row[0] != COLUMN_NAME_FRAME_NUMBER or row[1] != COLUMN_NAME_TIMECODE:
             return False
         return True
 
-    def load_from_csv(self, path: str = None, file: TextIO = None) -> Optional[int]:
-        """Load all metrics stored in a CSV file into the StatsManager instance.
+    # TODO(v1.0): Remove.
+    def load_from_csv(self, csv_file: Union[str, bytes, TextIO]) -> Optional[int]:
+        """[DEPRECATED] DO NOT USE
+
+        Load all metrics stored in a CSV file into the StatsManager instance. Will be removed in a
+        future release after becoming a no-op.
 
         Arguments:
             csv_file: A file handle opened in read mode (e.g. open('...', 'r')) or a path as str.
 
         Returns:
             int or None: Number of frames/rows read from the CSV file, or None if the
             input file was blank or could not be found.
 
         Raises:
             StatsFileCorrupt: Stats file is corrupt and can't be loaded, or wrong file
                 was specified.
         """
-        if path is not None and file is not None:
-            raise ValueError("Only one of path or file can be specified")
+        # TODO: Make this an error, then make load_from_csv() a no-op, and finally, remove it.
+        logger.warning("load_from_csv() is deprecated and will be removed in a future release.")
+
         # If we get a path instead of an open file handle, check that it exists, and if so,
         # recursively call ourselves again but with file set instead of path.
-        if path is not None:
-            if os.path.exists(path):
-                with open(path, 'r') as file:
-                    return self.load_from_csv(file=file)
+        if isinstance(csv_file, (str, bytes)):
+            if os.path.exists(csv_file):
+                with open(csv_file, 'r') as file:
+                    return self.load_from_csv(csv_file=file)
             # Path doesn't exist.
-            return
+            return None
 
         # If we get here, file is a valid file handle in read-only text mode.
-        csv_reader = csv.reader(file, lineterminator='\n')
+        csv_reader = csv.reader(csv_file, lineterminator='\n')
         num_cols = None
         num_metrics = None
         num_frames = None
         # First Row: Frame Num, Timecode, [metrics...]
         try:
             row = next(csv_reader)
             # Backwards compatibility for previous versions of statsfile
@@ -299,15 +295,19 @@
             for i, metric_str in enumerate(row[2:]):
                 if metric_str and metric_str != 'None':
                     try:
                         metric_dict[self._loaded_metrics[i]] = float(metric_str)
                     except ValueError:
                         raise StatsFileCorrupt('Corrupted value in stats file: %s' %
                                                metric_str) from ValueError
-            self.set_metrics(int(row[0]), metric_dict)
+            frame_number = int(row[0])
+            # Switch from 1-based to 0-based frame numbers.
+            if frame_number > 0:
+                frame_number -= 1
+            self.set_metrics(frame_number, metric_dict)
             num_frames += 1
         logger.info('Loaded %d metrics for %d frames.', num_metrics, num_frames)
         self._metrics_updated = False
         return num_frames
 
     def _get_metric(self, frame_number: int, metric_key: str) -> Optional[Any]:
         if self._metric_exists(frame_number, metric_key):
```

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-CLICK` & `scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-CLICK`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-NUMPY` & `scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-NUMPY`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-OPENCV` & `scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-OPENCV`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-PYTEST` & `scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-PYTEST`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/LICENSE-TQDM` & `scenedetect-0.6rc0/scenedetect/thirdparty/LICENSE-TQDM`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/__init__.py` & `scenedetect-0.6rc0/scenedetect/thirdparty/__init__.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/thirdparty/simpletable.py` & `scenedetect-0.6rc0/scenedetect/thirdparty/simpletable.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/scenedetect/video_splitter.py` & `scenedetect-0.6rc0/scenedetect/video_splitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 import time
 from typing import Iterable, Optional, Tuple
 from string import Template
 
 from scenedetect.frame_timecode import FrameTimecode
 from scenedetect.platform import tqdm, invoke_command, CommandTooLong, get_file_name
 
-
 logger = logging.getLogger('pyscenedetect')
 
 FrameTimecodePair = Tuple[FrameTimecode, FrameTimecode]
 
 COMMAND_TOO_LONG_STRING = '''
 Cannot split video due to too many scenes (resulting command
 is too large to process). To work around this issue, you can
@@ -66,15 +65,15 @@
 
 
 def is_mkvmerge_available():
     # type: () -> bool
     """ Is mkvmerge Available: Gracefully checks if mkvmerge command is available.
 
     Returns:
-        (bool) True if the mkvmerge command is available, False otherwise.
+        True if `mkvmerge` can be invoked, False otherwise.
     """
     ret_val = None
     try:
         ret_val = subprocess.call(['mkvmerge', '--quiet'])
     except OSError:
         return False
     if ret_val is not None and ret_val != 2:
@@ -83,15 +82,15 @@
 
 
 def is_ffmpeg_available():
     # type: () -> bool
     """ Is ffmpeg Available: Gracefully checks if ffmpeg command is available.
 
     Returns:
-        (bool) True if the ffmpeg command is available, False otherwise.
+        True if `ffmpeg` can be invoked, False otherwise.
     """
     ret_val = None
     try:
         ret_val = subprocess.call(['ffmpeg', '-v', 'quiet'])
     except OSError:
         return False
     if ret_val is not None and ret_val != 1:
@@ -100,35 +99,47 @@
 
 
 ##
 ## Split Video Functions
 ##
 
 
-def split_video_mkvmerge(input_video_path: str,
-                         scene_list: Iterable[FrameTimecodePair],
-                         output_file_template: str = '$VIDEO_NAME.mkv',
-                         video_name: Optional[str] = None,
-                         show_output: bool = False):
+def split_video_mkvmerge(
+    input_video_path: str,
+    scene_list: Iterable[FrameTimecodePair],
+    output_file_template: str = '$VIDEO_NAME.mkv',
+    video_name: Optional[str] = None,
+    show_output: bool = False,
+    suppress_output=None,
+):
     """ Calls the mkvmerge command on the input video, splitting it at the
     passed timecodes, where each scene is written in sequence from 001.
 
     Arguments:
         input_video_path: Path to the video to be split.
         scene_list : List of scenes as pairs of FrameTimecodes denoting the start/end times.
         output_file_template: Template to use for output files. Mkvmerge always adds the suffix
             "-$SCENE_NUMBER". Can use $VIDEO_NAME as a template parameter (e.g. "$VIDEO_NAME.mkv").
         video_name (str): Name of the video to be substituted in output_file_template for
             $VIDEO_NAME. If not specified, will be obtained from the filename.
-        show_output: If False, adds the --quiet flag when invoking `mkvmerge`.
-
+        show_output: If False, adds the --quiet flag when invoking `mkvmerge`..
+        suppress_output: [DEPRECATED] DO NOT USE. For backwards compatibility only.
     Returns:
         Return code of invoking mkvmerge (0 on success). If scene_list is empty, will
         still return 0, but no commands will be invoked.
     """
+    # Handle backwards compatibility with v0.5 API.
+    if isinstance(input_video_path, list):
+        logger.error('Using a list of paths is deprecated. Pass a single path instead.')
+        if len(input_video_path) > 1:
+            raise ValueError('Concatenating multiple input videos is not supported.')
+        input_video_path = input_video_path[0]
+    if suppress_output is not None:
+        logger.error('suppress_output is deprecated, use show_output instead.')
+        show_output = not suppress_output
 
     if not scene_list:
         return 0
 
     logger.info('Splitting input video using mkvmerge, output path template:\n  %s',
                 output_file_template)
 
@@ -164,21 +175,25 @@
         logger.error('mkvmerge could not be found on the system.'
                      ' Please install mkvmerge to enable video output support.')
     if ret_val != 0:
         logger.error('Error splitting video (mkvmerge returned %d).', ret_val)
     return ret_val
 
 
-def split_video_ffmpeg(input_video_path: str,
-                       scene_list: Iterable[FrameTimecodePair],
-                       output_file_template: str = '$VIDEO_NAME-Scene-$SCENE_NUMBER.mp4',
-                       video_name: Optional[str] = None,
-                       arg_override: str = '-c:v libx264 -preset fast -crf 21 -c:a aac',
-                       show_progress: bool = False,
-                       show_output: bool = False):
+def split_video_ffmpeg(
+    input_video_path: str,
+    scene_list: Iterable[FrameTimecodePair],
+    output_file_template: str = '$VIDEO_NAME-Scene-$SCENE_NUMBER.mp4',
+    video_name: Optional[str] = None,
+    arg_override: str = '-c:v libx264 -preset fast -crf 21 -c:a aac',
+    show_progress: bool = False,
+    show_output: bool = False,
+    suppress_output=None,
+    hide_progress=None,
+):
     """ Calls the ffmpeg command on the input video, generating a new video for
     each scene based on the start/end timecodes.
 
     Arguments:
         input_video_path: Path to the video to be split.
         scene_list (List[Tuple[FrameTimecode, FrameTimecode]]): List of scenes
             (pairs of FrameTimecodes) denoting the start/end frames of each scene.
@@ -186,19 +201,33 @@
             Can use $VIDEO_NAME and $SCENE_NUMBER in this format, for example:
             `$VIDEO_NAME - Scene $SCENE_NUMBER.mp4`
         video_name (str): Name of the video to be substituted in output_file_template. If not
             passed will be calculated from input_video_path automatically.
         arg_override (str): Allows overriding the arguments passed to ffmpeg for encoding.
         show_progress (bool): If True, will show progress bar provided by tqdm (if installed).
         show_output (bool): If True, will show output from ffmpeg for first split.
+        suppress_output: [DEPRECATED] DO NOT USE. For backwards compatibility only.
+        hide_progress: [DEPRECATED] DO NOT USE. For backwards compatibility only.
 
     Returns:
         Return code of invoking ffmpeg (0 on success). If scene_list is empty, will
         still return 0, but no commands will be invoked.
     """
+    # Handle backwards compatibility with v0.5 API.
+    if isinstance(input_video_path, list):
+        logger.error('Using a list of paths is deprecated. Pass a single path instead.')
+        if len(input_video_path) > 1:
+            raise ValueError('Concatenating multiple input videos is not supported.')
+        input_video_path = input_video_path[0]
+    if suppress_output is not None:
+        logger.error('suppress_output is deprecated, use show_output instead.')
+        show_output = not suppress_output
+    if hide_progress is not None:
+        logger.error('hide_progress is deprecated, use show_progress instead.')
+        show_progress = not hide_progress
 
     if not scene_list:
         return 0
 
     logger.info('Splitting input video using ffmpeg, output path template:\n  %s',
                 output_file_template)
```

### Comparing `scenedetect-0.6.dev3/scenedetect/video_stream.py` & `scenedetect-0.6rc0/scenedetect/video_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 # Copyright (C) 2014-2022 Brandon Castellano <http://www.bcastell.com>.
 # PySceneDetect is licensed under the BSD 3-Clause License; see the
 # included LICENSE file, or visit one of the above pages for details.
 #
 """ ``scenedetect.video_stream`` Module
 
 This module contains the :py:class:`VideoStream` class, which provides a library agnostic
-interface for video input.  See :py:mod:`scenedetect.backends` for supported backends.
-
-To open a video by path, either construct one of the available backends directly, or use
-the :py:func:`scenedetect.backends.open_video` function:
+interface for video input. To open a video by path, use :py:func:`scenedetect.open_video`:
 
 .. code:: python
 
     from scenedetect import open_video
-    video = open_video(path='video.mp4')
+    video = open_video('video.mp4')
 
-See :py:mod:`scenedetect.backends` for a more detailed example example.
+You can also optionally specify a framerate and a specific backend library to use. Unless specified,
+OpenCV will be used as the video backend. See :py:mod:`scenedetect.backends` for a detailed example.
 
 New :py:class:`VideoStream <scenedetect.video_stream.VideoStream>` implementations can be
 tested by adding it to the test suite in `tests/test_video_stream.py`.
 """
 
 from abc import ABC, abstractmethod
 from typing import Tuple, Optional, Union
@@ -45,14 +43,15 @@
     """Either an unrecoverable error happened while attempting to seek, or the underlying
     stream is not seekable (additional information will be provided when possible)."""
 
 
 class VideoOpenFailure(Exception):
     """Raised by a backend if opening a video fails."""
 
+    # pylint: disable=useless-super-delegation
     def __init__(self, message: str = "Unknown backend error."):
         super().__init__(message)
 
 
 class FrameRateUnavailable(VideoOpenFailure):
     """Exception instance to provide consistent error messaging across backends when the video frame
     rate is unavailable or cannot be calculated. Subclass of VideoOpenFailure."""
@@ -115,15 +114,15 @@
     #
 
     @staticmethod
     @abstractmethod
     def BACKEND_NAME() -> str:
         """Unique name used to identify this backend. Should be a static property in derived
         classes (`BACKEND_NAME = 'backend_identifier'`)."""
-        return NotImplementedError
+        raise NotImplementedError
 
     #
     # Abstract Properties
     #
 
     @property
     @abstractmethod
```

### Comparing `scenedetect-0.6.dev3/scenedetect.cfg` & `scenedetect-0.6rc0/scenedetect.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -15,39 +15,51 @@
 #   Mac:     ~/Library/Preferences/PySceneDetect/scenedetect.cfg
 #
 # Run `scenedetect help` to see the exact path on your system which will be
 # used (it will be listed under the help text for the -c/--config option).
 # Specifying a config file path using -c/--config overrides the user config.
 #
 
+
+#
+# GLOBAL OPTIONS
+#
+
 [global]
 # Output directory for written files. If unset, defaults to working directory.
 #output = /usr/tmp/scenedetect/
 
 # Video backend interface, must be one of: opencv, pyav.
 #backend = opencv
 
 # Downscale frame using sub-sampling ratio of N. Set to 1 for no downscaling.
 # If unset, applied automatically based on input video resolution.
 #downscale = 1
 
 # Minimum length of a given scene (shorter scenes will be merged).
 #min-scene-len = 0.6s
 
-# Drop scenes shorter than min-scene-len instead of merging them (yes/no)
+# Merge last scene if it is shorter than min-scene-len (yes/no)
+#merge-last-scene = no
+
+# Drop scenes shorter than min-scene-len instead of merging (yes/no)
 #drop-short-scenes = no
 
 # Verbosity of console output (debug, info, warning, error, or none).
 # Set to none for the same behavior as specifying -q/--quiet.
 #verbosity = debug
 
 # Amount of frames to skip between performing scene detection. Not recommended.
 #frame-skip = 0
 
 
+#
+# DETECTOR OPTIONS
+#
+
 [detect-content]
 # Sensitivity threshold from 0 to 255. Lower values are more sensitive.
 #threshold = 27
 
 # Discard colour information and only use luminance (yes/no).
 #luma-only = no
 
@@ -86,14 +98,18 @@
 # Discard colour information and only use luminance (yes/no).
 #luma-only = no
 
 # Minimum length of a given scene (overrides [global] option).
 #min-scene-len = 0.6s
 
 
+#
+# COMMAND OPTIONS
+#
+
 [split-video]
 # Folder to output videos. Overrides [global] output option.
 #output = /usr/tmp/encoded
 
 # Filename template to use as output.
 #filename = $VIDEO_NAME-Scene-$SCENE_NUMBER
 
@@ -160,14 +176,15 @@
 # Override <img> element width/height.
 #image-height = 0
 #image-width = 0
 
 # Do not generate <img> elements in resulting table (yes/no).
 #no-images = no
 
+
 [list-scenes]
 # Folder to output scene list. Overrides [global] output option.
 #output = /usr/tmp/images
 
 # Filename format of created scene list. Can use $VIDEO_NAME in the name.
 #filename = $VIDEO_NAME-Scenes.csv
 
@@ -176,7 +193,30 @@
 #skip-cuts = no
 
 # Output only to command-line, don't write file (yes/no).
 #no-output-file = no
 
 # Suppress printing of scene list.
 #quiet = no
+
+
+#
+# BACKEND OPTIONS
+#
+
+[backend-opencv]
+# Number of times to keep reading frames after one fails to decode.
+# If set to 0, processing will stop on the first decode failure.
+#max-decode-attempts = 5
+
+
+[backend-pyav]
+# Threading mode to use: [none, slice, frame, auto]. Slice mode is the
+# PyAV default, and auto/frame are the fastest.
+#threading-mode = auto
+
+# Suppress ffmpeg log output. Default is `no`.
+#
+# WARNING: When threading-mode is set to auto/frame, setting
+# `suppress-output = yes` can cause the the program to not exit properly
+# on Linux/OSX (press Ctrl+C to quit if this occurs).
+#suppress-output = no
```

### Comparing `scenedetect-0.6.dev3/scenedetect.egg-info/PKG-INFO` & `scenedetect-0.6rc0/scenedetect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenedetect
-Version: 0.6.dev3
+Version: 0.6rc0
 Summary: Video scene cut/shot detection program and Python library.
 Home-page: https://github.com/Breakthrough/PySceneDetect
 Author: Brandon Castellano
 Author-email: brandon248@gmail.com
 License: BSD 3-Clause
 Project-URL: Homepage, https://pyscenedetect.readthedocs.io/
 Project-URL: Manual, https://manual.scenedetect.com/en/v0.6/
@@ -30,15 +30,15 @@
            :target: http://pyscenedetect.readthedocs.org/en/latest/copyright/
         
         .. image:: https://img.shields.io/github/stars/Breakthrough/PySceneDetect.svg?style=social&label=View%20on%20Github
            :target: https://github.com/Breakthrough/PySceneDetect
         
         ----------------------------------------------------------
         
-        Website: http://py.scenedetect.com/
+        Website: http://scenedetect.com/
         
         Documentation: http://manual.scenedetect.com/
         
         Github Repo: https://github.com/Breakthrough/PySceneDetect/
         
         ----------------------------------------------------------
```

### Comparing `scenedetect-0.6.dev3/scenedetect.egg-info/SOURCES.txt` & `scenedetect-0.6rc0/scenedetect.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 .gitignore
 .style.yapf
 .travis.yml
 LICENSE
 MANIFEST.in
 README.md
+appveyor.yml
 mkdocs.yml
-package-info.rst
 requirements.txt
+requirements_headless.txt
 scenedetect.cfg
 scenedetect.py
-scenedetect.spec
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/blank-template.md
 .github/ISSUE_TEMPLATE/bug-or-issue-report.md
 .github/ISSUE_TEMPLATE/feature-or-enhancement-request.md
+dist/.version_info
+dist/cleanup_dependencies.py
+dist/package-info.rst
+dist/requirements_windows.txt
+dist/scenedetect.spec
 docs/changelog.md
 docs/contributing.md
 docs/download.md
 docs/faq.md
 docs/features.md
 docs/index.md
 docs/requirements.txt
@@ -45,40 +50,42 @@
 manual/requirements.txt
 manual/_static/pyscenedetect_logo.png
 manual/_static/pyscenedetect_logo_small.png
 manual/api/backends.rst
 manual/api/detectors.rst
 manual/api/frame_timecode.rst
 manual/api/migration_guide.rst
+manual/api/platform.rst
 manual/api/scene_detector.rst
 manual/api/scene_manager.rst
 manual/api/stats_manager.rst
 manual/api/video_splitter.rst
 manual/api/video_stream.rst
+manual/cli/backends.rst
 manual/cli/commands.rst
 manual/cli/config_file.rst
 manual/cli/detectors.rst
 manual/cli/global_options.rst
 scenedetect/__init__.py
 scenedetect/__main__.py
 scenedetect/frame_timecode.py
 scenedetect/platform.py
 scenedetect/scene_detector.py
 scenedetect/scene_manager.py
 scenedetect/stats_manager.py
+scenedetect/video_manager.py
 scenedetect/video_splitter.py
 scenedetect/video_stream.py
 scenedetect.egg-info/PKG-INFO
 scenedetect.egg-info/SOURCES.txt
 scenedetect.egg-info/dependency_links.txt
 scenedetect.egg-info/entry_points.txt
 scenedetect.egg-info/requires.txt
 scenedetect.egg-info/top_level.txt
 scenedetect/../LICENSE
-scenedetect/../package-info.rst
 scenedetect/backends/__init__.py
 scenedetect/backends/opencv.py
 scenedetect/backends/pyav.py
 scenedetect/cli/__init__.py
 scenedetect/cli/config.py
 scenedetect/cli/context.py
 scenedetect/cli/controller.py
@@ -94,14 +101,15 @@
 scenedetect/thirdparty/LICENSE-TQDM
 scenedetect/thirdparty/__init__.py
 scenedetect/thirdparty/simpletable.py
 tests/__init__.py
 tests/conftest.py
 tests/test_api.py
 tests/test_backend_pyav.py
+tests/test_backwards_compat.py
 tests/test_cli.py
 tests/test_detectors.py
 tests/test_frame_timecode.py
 tests/test_platform.py
 tests/test_scene_manager.py
 tests/test_stats_manager.py
 tests/test_video_stream.py
```

### Comparing `scenedetect-0.6.dev3/scenedetect.py` & `scenedetect-0.6rc0/scenedetect.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/setup.py` & `scenedetect-0.6rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         'opencv': ['opencv-python'],
         'opencv-headless': ['opencv-python-headless'],
     }
 
 
 setup(
     name='scenedetect',
-    version='0.6-dev3',
+    version='0.6-rc0',
     description='Video scene cut/shot detection program and Python library.',
-    long_description=open('package-info.rst').read(),
+    long_description=open('dist/package-info.rst').read(),
     author='Brandon Castellano',
     author_email='brandon248@gmail.com',
     url='https://github.com/Breakthrough/PySceneDetect',
     license="BSD 3-Clause",
     keywords="video computer-vision analysis",
     install_requires=get_requires(),
     extras_require=get_extra_requires(),
```

### Comparing `scenedetect-0.6.dev3/tests/__init__.py` & `scenedetect-0.6rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/tests/conftest.py` & `scenedetect-0.6rc0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,24 +45,23 @@
                                 relative_path)
     return abs_path
 
 
 #
 # Test Case Fixtures
 #
-@pytest.fixture
-def test_video_file():
-    # type: () -> str
-    """ Fixture for test video file path (ensures file exists).
 
-    Access in test case by adding a test_video_file argument to obtain the path.
-    """
+@pytest.fixture
+def test_video_file() -> str:
+    """Simple test video containing both fast cuts and fades/dissolves."""
     return get_absolute_path("resources/testvideo.mp4")
 
 @pytest.fixture
-def test_movie_clip():
-    # type: () -> str
-    """ Fixture for test movie clip path (ensures file exists).
-
-    Access in test case by adding a test_movie_clip argument to obtain the path.
-    """
+def test_movie_clip() -> str:
+    """Movie clip containing fast cuts."""
     return get_absolute_path("resources/goldeneye.mp4")
+
+
+@pytest.fixture
+def corrupt_video_file() -> str:
+    """Video containing a corrupted frame causing a decode failure."""
+    return get_absolute_path("resources/corrupt_frame.mp4")
```

### Comparing `scenedetect-0.6.dev3/tests/test_api.py` & `scenedetect-0.6rc0/tests/test_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,66 +13,75 @@
 """PySceneDetect API Tests
 
 Demonstrates high-level usage of the PySceneDetect API.
 """
 
 from typing import List, Tuple
 
-from scenedetect import open_video, ContentDetector, FrameTimecode, SceneManager, StatsManager
+from scenedetect import detect, open_video
+from scenedetect import ContentDetector, FrameTimecode, SceneManager, StatsManager
 from scenedetect.backends import VideoStreamCv2
 
 STATS_FILE_PATH = 'api_test_statsfile.csv'
 
 
 def print_scenes(scene_list: List[Tuple[FrameTimecode, FrameTimecode]]):
-    """Iterate over a scene list and print it to the terminal."""
+    """Helper function to print a list of scenes to the terminal."""
     print('Scene List:')
     for i, scene in enumerate(scene_list):
         print('  Scene %2d: Start %s / Frame %d, End %s / Frame %d' % (
             i + 1,
             scene[0].get_timecode(),
             scene[0].get_frames(),
             scene[1].get_timecode(),
             scene[1].get_frames(),
         ))
 
 
+def test_api_detect(test_video_file: str):
+    """Demonstrate basic usage of the `detect` function to process a complete video."""
+    scene_list = detect(test_video_file, ContentDetector())
+    print_scenes(scene_list=scene_list)
+
+
 def test_api_start_end_time(test_video_file: str):
     """Demonstrate processing a subsection of a video based on a starting/ending time."""
     video = open_video(test_video_file)
     scene_manager = SceneManager()
     scene_manager.add_detector(ContentDetector())
-    # See FrameTimecode docs or test_api_timecode_types for all
-    # supported timecode formats.
+    # See test_api_timecode_types below for all supported timecode formats.
     start_time = 20 # Start at frame (int) 20
     end_time = 15.0 # End at 15 seconds (float)
     video.seek(start_time)
 
-    # Can specify `duration` instead of `end_time`.
+    # Can also specify `duration` instead of `end_time`.
     scene_manager.detect_scenes(video=video, end_time=end_time)
     scene_list = scene_manager.get_scene_list()
     print_scenes(scene_list=scene_list)
 
 
 def test_api_stats_manager(test_video_file: str):
-    """Demonstrate using a StatsManager to save and optionally load stats from disk."""
+    """Demonstrate using a StatsManager to save per-frame statistics to disk."""
     video = open_video(test_video_file)
     scene_manager = SceneManager(stats_manager=StatsManager())
     scene_manager.add_detector(ContentDetector())
     # Loading from disk is optional.
-    scene_manager.stats_manager.load_from_csv(path=STATS_FILE_PATH)
+    scene_manager.stats_manager.load_from_csv(csv_file=STATS_FILE_PATH)
     scene_manager.detect_scenes(video=video)
     scene_list = scene_manager.get_scene_list()
     print_scenes(scene_list=scene_list)
     # Save per-frame statistics to disk.
-    scene_manager.stats_manager.save_to_csv(path=STATS_FILE_PATH)
+    scene_manager.stats_manager.save_to_csv(csv_file=STATS_FILE_PATH)
 
 
 def test_api_video_stream_opencv(test_video_file: str):
-    """Demonstrate constructing and using a VideoStream backend."""
+    """Demonstrate constructing and using a VideoStream backend directly, instead of
+    using the `open_video` function. Only VideoStreamCv2 is guaranteed to be available.
+    Applications that do not require a specific backend library should use `open_video`.
+    """
     video = VideoStreamCv2(test_video_file)
     scene_manager = SceneManager()
     scene_manager.add_detector(ContentDetector())
     scene_manager.detect_scenes(video=video)
     scene_list = scene_manager.get_scene_list()
     print_scenes(scene_list=scene_list)
```

### Comparing `scenedetect-0.6.dev3/tests/test_backend_pyav.py` & `scenedetect-0.6rc0/tests/test_backend_pyav.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 
 from scenedetect.backends.pyav import VideoStreamAv
 
 def test_video_stream_pyav_bytesio(test_video_file: str):
     """Test that VideoStreamAv works with a BytesIO input in addition to a path."""
     # Mode must be binary!
     video_file = open(test_video_file, mode='rb')
-    stream = VideoStreamAv(path_or_io=video_file)
+    stream = VideoStreamAv(path_or_io=video_file, threading_mode=None)
     assert stream.is_seekable
     stream.seek(50)
     for _ in range(10):
         assert stream.read() is not False
```

### Comparing `scenedetect-0.6.dev3/tests/test_detectors.py` & `scenedetect-0.6rc0/tests/test_detectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from scenedetect.backends.opencv import VideoStreamCv2
 
 # TODO(v1.0): Parameterize these tests like VideoStreams are.
 # Current test output cannot be used for profiling cases which iterate over multiple detectors.
 
 # TODO(v1.0): Add new test video.
 
-TEST_MOVIE_CLIP_GROUND_TRUTH_CONTENT = [(30, [1198, 1226, 1260, 1281, 1334, 1365, 1697, 1871]),
-                                        (27, [1198, 1226, 1260, 1281, 1334, 1365, 1590, 1697,
+TEST_MOVIE_CLIP_GROUND_TRUTH_CONTENT = [(30, [1199, 1226, 1260, 1281, 1334, 1365, 1697, 1871]),
+                                        (27, [1199, 1226, 1260, 1281, 1334, 1365, 1590, 1697,
                                               1871])]
 """Ground truth for `test_movie_clip` with ContentDetector as (threshold, [scene start frame])."""
 
 TEST_VIDEO_FILE_GROUND_TRUTH_THRESHOLD = [0, 15, 198, 376]
 """Results for `test_video_file` with default ThresholdDetector values."""
```

### Comparing `scenedetect-0.6.dev3/tests/test_frame_timecode.py` & `scenedetect-0.6rc0/tests/test_frame_timecode.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #     [  Docs:   http://manual.scenedetect.scenedetect.com/      ]
 #     [  Github: https://github.com/Breakthrough/PySceneDetect/  ]
 #
 # Copyright (C) 2014-2022 Brandon Castellano <http://www.bcastell.com>.
 # PySceneDetect is licensed under the BSD 3-Clause License; see the
 # included LICENSE file, or visit one of the above pages for details.
 #
-
 """ PySceneDetect scenedetect.timecode Tests
 
 This file includes unit tests for the scenedetect.timecode module (specifically, the
 FrameTimecode object, used for representing frame-accurate timestamps and time values).
 
 These unit tests test the FrameTimecode object with respect to object construction,
 testing argument format/limits, operators (addition/subtraction), and conversion
@@ -23,69 +22,90 @@
 """
 
 # Standard project pylint disables for unit tests using pytest.
 # pylint: disable=no-self-use, protected-access, multiple-statements, invalid-name
 # pylint: disable=redefined-outer-name, pointless-statement, expression-not-assigned
 # pylint: disable=unneeded-not
 
-
 # Third-Party Library Imports
 import pytest
 
 # Standard Library Imports
 from scenedetect.frame_timecode import FrameTimecode
 from scenedetect.frame_timecode import MAX_FPS_DELTA
 
 
 def test_framerate():
     ''' Test FrameTimecode constructor argument "fps". '''
     # Not passing fps results in TypeError.
-    with pytest.raises(TypeError): FrameTimecode()
-    with pytest.raises(TypeError): FrameTimecode(timecode=0, fps=None)
+    with pytest.raises(TypeError):
+        FrameTimecode()
+    with pytest.raises(TypeError):
+        FrameTimecode(timecode=0, fps=None)
     with pytest.raises(TypeError):
         FrameTimecode(timecode=None, fps=FrameTimecode(timecode=0, fps=None))
     # Test zero FPS/negative.
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=0)
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=-1)
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=-100)
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=0.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=-1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode=0, fps=-1000.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=-1)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=-100)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=0.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=-1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=0, fps=-1000.0)
     with pytest.raises(ValueError):
         FrameTimecode(timecode=0, fps=MAX_FPS_DELTA / 2)
     # Test positive framerates.
     assert FrameTimecode(timecode=0, fps=1).frame_num == 0
     assert FrameTimecode(timecode=0, fps=MAX_FPS_DELTA).frame_num == 0
     assert FrameTimecode(timecode=0, fps=10).frame_num == 0
     assert FrameTimecode(timecode=0, fps=MAX_FPS_DELTA * 2).frame_num == 0
     assert FrameTimecode(timecode=0, fps=1000).frame_num == 0
     assert FrameTimecode(timecode=0, fps=1000.0).frame_num == 0
 
+
 def test_timecode_numeric():
     ''' Test FrameTimecode constructor argument "timecode" with numeric arguments. '''
-    with pytest.raises(ValueError): FrameTimecode(timecode=-1, fps=1)
-    with pytest.raises(ValueError): FrameTimecode(timecode=-1.0, fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode=-0.1, fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode=-1.0/1000, fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=-1, fps=1)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=-1.0, fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=-0.1, fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode=-1.0 / 1000, fps=1.0)
     assert FrameTimecode(timecode=0, fps=1).frame_num == 0
     assert FrameTimecode(timecode=1, fps=1).frame_num == 1
     assert FrameTimecode(timecode=0.0, fps=1.0).frame_num == 0
     assert FrameTimecode(timecode=1.0, fps=1.0).frame_num == 1
 
+
 def test_timecode_string():
     ''' Test FrameTimecode constructor argument "timecode" with string arguments. '''
     # Invalid strings:
-    with pytest.raises(ValueError): FrameTimecode(timecode='-1', fps=1)
-    with pytest.raises(ValueError): FrameTimecode(timecode='-1.0', fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode='-0.1', fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode='1.0', fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode='1.9x', fps=1)
-    with pytest.raises(ValueError): FrameTimecode(timecode='1x', fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode='1.9.9', fps=1.0)
-    with pytest.raises(ValueError): FrameTimecode(timecode='1.0-', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='-1', fps=1)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='-1.0', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='-0.1', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='1.0', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='1.9x', fps=1)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='1x', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='1.9.9', fps=1.0)
+    with pytest.raises(ValueError):
+        FrameTimecode(timecode='1.0-', fps=1.0)
 
     # Frame number integer [int->str] ('%d', integer number as string)
     assert FrameTimecode(timecode='0', fps=1).frame_num == 0
     assert FrameTimecode(timecode='1', fps=1).frame_num == 1
     assert FrameTimecode(timecode='10', fps=1.0).frame_num == 10
 
     # Seconds format [float->str] ('%fs', number as string followed by 's' for seconds)
@@ -95,124 +115,139 @@
     assert FrameTimecode(timecode='10.0s', fps=1.0).frame_num == 10
     assert FrameTimecode(timecode='10.0000000000s', fps=1.0).frame_num == 10
     assert FrameTimecode(timecode='10.100s', fps=1.0).frame_num == 10
     assert FrameTimecode(timecode='1.100s', fps=10.0).frame_num == 11
 
     # Standard timecode format [timecode->str] ('HH:MM:SS[.nnn]', where [.nnn] is optional)
     assert FrameTimecode(timecode='00:00:01', fps=1).frame_num == 1
-    assert FrameTimecode(timecode='00:00:01.9999', fps=1).frame_num == 1
+    assert FrameTimecode(timecode='00:00:01.9999', fps=1).frame_num == 2
     assert FrameTimecode(timecode='00:00:02.0000', fps=1).frame_num == 2
     assert FrameTimecode(timecode='00:00:02.0001', fps=1).frame_num == 2
 
     assert FrameTimecode(timecode='00:00:01', fps=10).frame_num == 10
     assert FrameTimecode(timecode='00:00:00.5', fps=10).frame_num == 5
     assert FrameTimecode(timecode='00:00:00.100', fps=10).frame_num == 1
     assert FrameTimecode(timecode='00:00:00.001', fps=1000).frame_num == 1
 
-    assert FrameTimecode(timecode='00:00:59.999', fps=1).frame_num == 59
+    assert FrameTimecode(timecode='00:00:59.999', fps=1).frame_num == 60
     assert FrameTimecode(timecode='00:01:00.000', fps=1).frame_num == 60
     assert FrameTimecode(timecode='00:01:00.001', fps=1).frame_num == 60
 
-    assert FrameTimecode(timecode='00:59:59.999', fps=1).frame_num == 3599
+    assert FrameTimecode(timecode='00:59:59.999', fps=1).frame_num == 3600
     assert FrameTimecode(timecode='01:00:00.000', fps=1).frame_num == 3600
     assert FrameTimecode(timecode='01:00:00.001', fps=1).frame_num == 3600
 
+
 def test_get_frames():
     ''' Test FrameTimecode get_frames() method. '''
     assert FrameTimecode(timecode=1, fps=1.0).get_frames(), 1
     assert FrameTimecode(timecode=1000, fps=60.0).get_frames(), 1000
     assert FrameTimecode(timecode=1000000000, fps=29.97).get_frames(), 1000000000
 
-    assert FrameTimecode(timecode=1.0, fps=1.0).get_frames(), int(1.0/1.0)
-    assert FrameTimecode(timecode=1000.0, fps=60.0).get_frames(), int(1000.0*60.0)
-    assert FrameTimecode(timecode=1000000000.0, fps=29.97).get_frames(), int(1000000000.0*29.97)
+    assert FrameTimecode(timecode=1.0, fps=1.0).get_frames(), int(1.0 / 1.0)
+    assert FrameTimecode(timecode=1000.0, fps=60.0).get_frames(), int(1000.0 * 60.0)
+    assert FrameTimecode(timecode=1000000000.0, fps=29.97).get_frames(), int(1000000000.0 * 29.97)
 
     assert FrameTimecode(timecode='00:00:02.0000', fps=1).get_frames(), 2
     assert FrameTimecode(timecode='00:00:00.5', fps=10).get_frames(), 5
     assert FrameTimecode(timecode='00:00:01', fps=10).get_frames(), 10
     assert FrameTimecode(timecode='00:01:00.000', fps=1).get_frames(), 60
 
+
 def test_get_seconds():
     ''' Test FrameTimecode get_seconds() method. '''
-    assert FrameTimecode(timecode=1, fps=1.0).get_seconds(), pytest.approx(1.0/1.0)
-    assert FrameTimecode(timecode=1000, fps=60.0).get_seconds(), pytest.approx(1000/60.0)
+    assert FrameTimecode(timecode=1, fps=1.0).get_seconds(), pytest.approx(1.0 / 1.0)
+    assert FrameTimecode(timecode=1000, fps=60.0).get_seconds(), pytest.approx(1000 / 60.0)
     assert FrameTimecode(
-        timecode=1000000000, fps=29.97).get_seconds(), pytest.approx(1000000000/29.97)
+        timecode=1000000000, fps=29.97).get_seconds(), pytest.approx(1000000000 / 29.97)
 
     assert FrameTimecode(timecode=1.0, fps=1.0).get_seconds(), pytest.approx(1.0)
     assert FrameTimecode(timecode=1000.0, fps=60.0).get_seconds(), pytest.approx(1000.0)
     assert FrameTimecode(
         timecode=1000000000.0, fps=29.97).get_seconds(), pytest.approx(1000000000.0)
 
     assert FrameTimecode(timecode='00:00:02.0000', fps=1).get_seconds(), pytest.approx(2.0)
     assert FrameTimecode(timecode='00:00:00.5', fps=10).get_seconds(), pytest.approx(0.5)
     assert FrameTimecode(timecode='00:00:01', fps=10).get_seconds(), pytest.approx(1.0)
     assert FrameTimecode(timecode='00:01:00.000', fps=1).get_seconds(), pytest.approx(60.0)
 
+
 def test_get_timecode():
     ''' Test FrameTimecode get_timecode() method. '''
     assert FrameTimecode(timecode=1.0, fps=1.0).get_timecode() == '00:00:01.000'
     assert FrameTimecode(timecode=60.117, fps=60.0).get_timecode() == '00:01:00.117'
     assert FrameTimecode(timecode=3600.234, fps=29.97).get_timecode() == '01:00:00.234'
 
     assert FrameTimecode(timecode='00:00:02.0000', fps=1).get_timecode() == '00:00:02.000'
     assert FrameTimecode(timecode='00:00:00.5', fps=10).get_timecode() == '00:00:00.500'
     assert FrameTimecode(timecode='00:00:01.501', fps=10).get_timecode() == '00:00:01.500'
     assert FrameTimecode(timecode='00:01:00.000', fps=1).get_timecode() == '00:01:00.000'
 
+
 def test_equality():
     ''' Test FrameTimecode equality (==, __eq__) operator. '''
     x = FrameTimecode(timecode=1.0, fps=10.0)
     assert x == x
     assert x == FrameTimecode(timecode=1.0, fps=10.0)
     assert not x != FrameTimecode(timecode=1.0, fps=10.0)
     assert x != FrameTimecode(timecode=10.0, fps=10.0)
     assert not x == FrameTimecode(timecode=10.0, fps=10.0)
     # Comparing FrameTimecodes with different framerates raises a TypeError.
-    with pytest.raises(TypeError): x == FrameTimecode(timecode=1.0, fps=100.0)
-    with pytest.raises(TypeError): x == FrameTimecode(timecode=1.0, fps=10.1)
+    with pytest.raises(TypeError):
+        x == FrameTimecode(timecode=1.0, fps=100.0)
+    with pytest.raises(TypeError):
+        x == FrameTimecode(timecode=1.0, fps=10.1)
 
     assert x == FrameTimecode(x)
     assert x == FrameTimecode(1.0, x)
     assert x == FrameTimecode(10, x)
     assert x == '00:00:01'
     assert x == '00:00:01.0'
     assert x == '00:00:01.00'
     assert x == '00:00:01.000'
     assert x == '00:00:01.0000'
     assert x == '00:00:01.00000'
     assert x == 10
     assert x == 1.0
 
-    with pytest.raises(ValueError): x == '0x'
-    with pytest.raises(ValueError): x == 'x00:00:00.000'
-    with pytest.raises(TypeError): x == [0]
-    with pytest.raises(TypeError): x == (0,)
-    with pytest.raises(TypeError): x == [0, 1, 2, 3]
-    with pytest.raises(TypeError): x == {0:0}
+    with pytest.raises(ValueError):
+        x == '0x'
+    with pytest.raises(ValueError):
+        x == 'x00:00:00.000'
+    with pytest.raises(TypeError):
+        x == [0]
+    with pytest.raises(TypeError):
+        x == (0,)
+    with pytest.raises(TypeError):
+        x == [0, 1, 2, 3]
+    with pytest.raises(TypeError):
+        x == {0: 0}
 
     assert FrameTimecode(timecode='00:00:00.5', fps=10) == '00:00:00.500'
     assert FrameTimecode(timecode='00:00:01.500', fps=10) == '00:00:01.500'
     assert FrameTimecode(timecode='00:00:01.500', fps=10) == '00:00:01.501'
     assert FrameTimecode(timecode='00:00:01.500', fps=10) == '00:00:01.502'
     assert FrameTimecode(timecode='00:00:01.500', fps=10) == '00:00:01.508'
     assert FrameTimecode(timecode='00:00:01.500', fps=10) == '00:00:01.509'
     assert FrameTimecode(timecode='00:00:01.519', fps=10) == '00:00:01.510'
 
+
 def test_addition():
     ''' Test FrameTimecode addition (+/+=, __add__/__iadd__) operator. '''
     x = FrameTimecode(timecode=1.0, fps=10.0)
     assert x + 1 == FrameTimecode(timecode=1.1, fps=10.0)
     assert x + 1 == FrameTimecode(1.1, x)
     assert x + 10 == 20
     assert x + 10 == 2.0
 
     assert x + 10 == '00:00:02.000'
 
-    with pytest.raises(TypeError): FrameTimecode('00:00:02.000', fps=20.0) == x + 10
+    with pytest.raises(TypeError):
+        FrameTimecode('00:00:02.000', fps=20.0) == x + 10
+
 
 def test_subtraction():
     ''' Test FrameTimecode subtraction (-/-=, __sub__) operator. '''
     x = FrameTimecode(timecode=1.0, fps=10.0)
     assert (x - 1) == FrameTimecode(timecode=0.9, fps=10.0)
     assert x - 2 == FrameTimecode(0.8, x)
     assert x - 10 == FrameTimecode(0.0, x)
@@ -221,9 +256,19 @@
     assert x - 100 == FrameTimecode(0.0, x)
 
     assert x - 1.0 == FrameTimecode(0.0, x)
     assert x - 100.0 == FrameTimecode(0.0, x)
 
     assert x - 1 == FrameTimecode(timecode=0.9, fps=10.0)
 
-    with pytest.raises(TypeError): FrameTimecode('00:00:02.000', fps=20.0) == x - 10
+    with pytest.raises(TypeError):
+        FrameTimecode('00:00:02.000', fps=20.0) == x - 10
+
 
+@pytest.mark.parametrize("frame_num,fps", [(1, 1), (61, 14), (29, 25), (126, 24000 / 1001.0)])
+def test_identity(frame_num, fps):
+    ''' Test FrameTimecode values, when used in init return the same values '''
+    frame_time_code = FrameTimecode(frame_num, fps=fps)
+    assert FrameTimecode(frame_time_code) == frame_time_code
+    assert FrameTimecode(frame_time_code.get_frames(), fps=fps) == frame_time_code
+    assert FrameTimecode(frame_time_code.get_seconds(), fps=fps) == frame_time_code
+    assert FrameTimecode(frame_time_code.get_timecode(), fps=fps) == frame_time_code
```

### Comparing `scenedetect-0.6.dev3/tests/test_platform.py` & `scenedetect-0.6rc0/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `scenedetect-0.6.dev3/tests/test_stats_manager.py` & `scenedetect-0.6rc0/tests/test_stats_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """ PySceneDetect scenedetect.stats_manager Tests
 
 This file includes unit tests for the scenedetect.stats_manager module (specifically,
 the StatsManager object, used to coordinate caching of frame metrics to/from a CSV
 file to speed up subsequent calls to detect_scenes on a SceneManager.
 
-These tests rely on the SceneManager, VideoStreamCv2, and ContentDetector classes.
+These tests rely on the SceneManager, VifdeoStreamCv2, and ContentDetector classes.
 
 These tests also require the testvideo.mp4 (see test_scene_manager.py for download
 instructions), however any other valid video file can be used as well by modifying
 the fixture test_video_file in conftest.py.
 
 Additionally, these tests will create, write to, and read from files which use names
 TEST_STATS_FILE_XXXXXXXXXXXX.csv, where the X's will be replaced with random digits.
@@ -133,15 +133,15 @@
 def test_load_empty_stats():
     """ Test loading an empty stats file, ensuring it results in no errors. """
     open(TEST_STATS_FILES[0], 'w').close()
     stats_manager = StatsManager()
     stats_manager.load_from_csv(TEST_STATS_FILES[0])
 
 
-def test__save_no_detect_scenes():
+def test_save_no_detect_scenes():
     """Test saving without calling detect_scenes."""
     stats_manager = StatsManager()
     stats_manager.save_to_csv(TEST_STATS_FILES[0])
 
 
 def test_load_hardcoded_file():
     """ Test loading a stats file with some hard-coded data generated by this test case. """
@@ -157,60 +157,23 @@
         base_timecode = FrameTimecode(0, 29.97)
         some_frame_timecode = base_timecode + some_frame_key
 
         # Write out a valid file.
         stats_writer.writerow(
             [COLUMN_NAME_FRAME_NUMBER, COLUMN_NAME_TIMECODE, some_metric_key])
         stats_writer.writerow(
-            [some_frame_key, some_frame_timecode.get_timecode(), str(some_metric_value)])
-
-
-    stats_manager.load_from_csv(TEST_STATS_FILES[0])
-
-    # Check that we decoded the correct values.
-    assert stats_manager.metrics_exist(some_frame_key, [some_metric_key])
-    assert stats_manager.get_metrics(
-        some_frame_key, [some_metric_key])[0] == pytest.approx(some_metric_value)
-
-
-
-def test_load_hardcoded_file_backwards_compat():
-    """ Test loading a stats file with some hard-coded data generated by this test case.
-
-    Ensures backwards compatibility with old statsfiles which included an addional header.
-    """
-
-    stats_manager = StatsManager()
-    with open(TEST_STATS_FILES[0], 'w') as stats_file:
-        stats_writer = csv.writer(stats_file, lineterminator='\n')
-
-        some_metric_key = 'some_metric'
-        some_metric_value = 1.2
-        some_frame_key = 100
-        base_timecode = FrameTimecode(0, 29.97)
-        some_frame_timecode = base_timecode + some_frame_key
-
-        # Write out a valid file as per PySceneDetect v0.5.4 and prior.
-        stats_writer.writerow(
-            ['Video Framerate', '23.976'])
-        stats_writer.writerow(
-            [COLUMN_NAME_FRAME_NUMBER, COLUMN_NAME_TIMECODE, some_metric_key])
-        stats_writer.writerow(
-            [some_frame_key, some_frame_timecode.get_timecode(), str(some_metric_value)])
-
-        stats_file.close()
+            [some_frame_key + 1, some_frame_timecode.get_timecode(), str(some_metric_value)])
 
     stats_manager.load_from_csv(TEST_STATS_FILES[0])
 
     # Check that we decoded the correct values.
     assert stats_manager.metrics_exist(some_frame_key, [some_metric_key])
     assert stats_manager.get_metrics(
         some_frame_key, [some_metric_key])[0] == pytest.approx(some_metric_value)
 
-
 def test_save_load_from_video(test_video_file):
     """ Test generating and saving some frame metrics from TEST_VIDEO_FILE to a file on disk, and
     loading the file back to ensure the loaded frame metrics agree with those that were saved.
     """
     video = VideoStreamCv2(test_video_file)
     stats_manager = StatsManager()
     scene_manager = SceneManager(stats_manager)
@@ -219,15 +182,15 @@
 
     video_fps = video.frame_rate
     duration = FrameTimecode('00:00:20', video_fps)
 
     scene_manager.auto_downscale = True
     scene_manager.detect_scenes(video, duration=duration)
 
-    stats_manager.save_to_csv(path=TEST_STATS_FILES[0])
+    stats_manager.save_to_csv(csv_file=TEST_STATS_FILES[0])
 
     stats_manager_new = StatsManager()
 
     stats_manager_new.load_from_csv(TEST_STATS_FILES[0])
 
     # Choose the first available frame key and compare all metrics in both.
     frame_key = min(stats_manager._frame_metrics.keys())
```

### Comparing `scenedetect-0.6.dev3/tests/test_video_stream.py` & `scenedetect-0.6rc0/tests/test_video_stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,32 +26,21 @@
 # Third-Party Library Imports
 import numpy
 import pytest
 
 from scenedetect.video_stream import VideoStream
 from scenedetect.backends.opencv import VideoStreamCv2
 from scenedetect.backends.pyav import VideoStreamAv
+# Compatibility w/ v0.5.
+from scenedetect.video_manager import VideoManager
 
-## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
-## List of Required/TBD Test Cases
-## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
-
-# TODO: End of video read()/seek behaviour!
-
-# TODO: Add checks that frame was decoded properly - compare against
-# a set of hand-picked frames? Or just a few colour samples?
-
-# TODO: Add test using image sequence.
-
-# TODO: Create a test case which opens both a corrupted video (set random bytes in the header
-# to zeroes until one fails with all backends?).  Can create dynamically by just opening
-# the path to a good video, copying it to a temp location, and modifying it in place.
-
-## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
-
+# TODO(v0.6): End of video read/seek behaviour, seek to very large offset, etc.
+# TODO(v0.6): Add test using image sequence (use counter.mp4 frames).
+# TODO(#258): Create a test case which opens a corrupted video. Copy one of the ground truth
+# files and see if a frame decode failure can be triggered.
 
 # Accuracy a framerate is checked to for testing purposes.
 FRAMERATE_TOLERANCE = 0.001
 # Accuracy a time in milliseconds is checked to for testing purposes.
 TIME_TOLERANCE_MS = 0.1
 
 
@@ -59,15 +48,15 @@
     if roi:
         assert False # TODO
     assert frame_a.shape == frame_b.shape
     num_pixels = frame_a.shape[0] * frame_a.shape[1]
     return numpy.sum(numpy.abs(frame_b - frame_a)) / num_pixels
 
 
-# TODO: Need to reduce code duplication here and in `conftest.py`
+# TODO: Reduce code duplication here and in `conftest.py`
 def get_absolute_path(relative_path: str) -> str:
     # type: (str) -> str
     """ Returns the absolute path to a (relative) path of a file that
     should exist within the tests/ directory.
 
     Throws FileNotFoundError if the file could not be found.
     """
@@ -82,18 +71,18 @@
 
     def __init__(self, path: str, height: int, width: int, frame_rate: float, total_frames: int):
         self.path = path
         self.height = height
         self.width = width
         self.frame_rate = frame_rate
         self.total_frames = total_frames
-        # TODO: Aspect ratio.
+        # TODO(v0.6): Test aspect ratio.
 
 
-# TODO: Need to reduce duplicated paths here and in `conftest.py`
+# TODO: Reduce duplicated paths here and in `conftest.py`
 def get_test_video_params():
     # type: () -> str
     """Fixture for parameters of all videos."""
     return [
         VideoParameters(
             path=get_absolute_path("resources/testvideo.mp4"),
             width=1280,
@@ -105,21 +94,22 @@
             width=1280,
             height=544,
             frame_rate=23.976,
             total_frames=1980),
     ]
 
 
-pytestmark = pytest.mark.parametrize("vs_type", [VideoStreamCv2, VideoStreamAv])
+pytestmark = pytest.mark.parametrize("vs_type", [VideoStreamCv2, VideoStreamAv, VideoManager])
 
 
 @pytest.mark.parametrize("test_video", get_test_video_params())
 class TestVideoStream:
 
     def test_basic_params(self, vs_type: Type[VideoStream], test_video: VideoParameters):
+        """Validate getting basic video parameters: frame size, frame rate, duration, etc."""
         stream = vs_type(test_video.path)
         assert stream.frame_size == (test_video.width, test_video.height)
         assert stream.frame_rate == pytest.approx(test_video.frame_rate, FRAMERATE_TOLERANCE)
         assert stream.duration.get_frames() == test_video.total_frames
         file_name = os.path.basename(test_video.path)
         last_dot_pos = file_name.rfind('.')
         assert stream.name == file_name[:last_dot_pos]
@@ -162,29 +152,28 @@
         assert stream.read() is not False
         # After the first frame has been decoded, position is still at 0 (PTS),
         # but frame_number is 1.
         assert stream.position == stream.base_timecode
         assert stream.position_ms == pytest.approx(0.0, abs=TIME_TOLERANCE_MS)
         assert stream.frame_number == 1
 
-
         stream.reset()
         # After resetting the stream, we should be back in the initial time state.
         assert stream.position == stream.base_timecode
         assert stream.position_ms == pytest.approx(0.0, abs=TIME_TOLERANCE_MS)
         assert stream.frame_number == 0
 
         # Test invariants over the first 100 frames.
         stream.reset()
 
         for i in range(1, 100 + 1):
             assert stream.read() is not False
             assert stream.position == stream.base_timecode + (i - 1)
-            assert stream.position_ms == pytest.approx(1000.0 * (i - 1) / float(stream.frame_rate),
-                                                       abs=TIME_TOLERANCE_MS)
+            assert stream.position_ms == pytest.approx(
+                1000.0 * (i - 1) / float(stream.frame_rate), abs=TIME_TOLERANCE_MS)
             assert stream.frame_number == i
         stream.reset()
 
     def test_seek(self, vs_type: Type[VideoStream], test_video: VideoParameters):
         """Validate seeking behaviour."""
         #
         # Basic timecode "identities".
@@ -201,37 +190,37 @@
         # FrameTimecode is currently one "behind" the frame_number since it
         # starts counting from zero. This should eventually be changed.
         assert stream.position == stream.base_timecode
         assert stream.position_ms == pytest.approx(0.0, abs=TIME_TOLERANCE_MS)
 
         stream.seek(2.0)
         stream.read()
-        assert stream.frame_number == 1 + int(stream.frame_rate * 2.0)
+        assert stream.frame_number == 1 + round(stream.frame_rate * 2.0)
         # FrameTimecode is currently one "behind" the frame_number since it
         # starts counting from zero. This should eventually be changed.
         assert stream.position == stream.base_timecode + 2.0
         assert stream.position_ms == pytest.approx(2000.0, abs=1000.0 / stream.frame_rate)
 
         # Seek to given FrameTimecode.
         stream.seek(stream.base_timecode)
         assert stream.frame_number == 0
         assert stream.position == stream.base_timecode
         assert stream.position_ms == pytest.approx(0.0, abs=TIME_TOLERANCE_MS)
 
         # Seek to a given frame number.
         stream.seek(200)
         assert stream.position == stream.base_timecode + 199
-        assert stream.position_ms == pytest.approx(1000.0 * (199.0 / float(stream.frame_rate)),
-                                                   abs=TIME_TOLERANCE_MS)
+        assert stream.position_ms == pytest.approx(
+            1000.0 * (199.0 / float(stream.frame_rate)), abs=TIME_TOLERANCE_MS)
         assert stream.frame_number == 200
         stream.read()
         assert stream.frame_number == 201
         assert stream.position == stream.base_timecode + 200
-        assert stream.position_ms == pytest.approx(1000.0 * (200.0 / float(stream.frame_rate)),
-                                                   abs=TIME_TOLERANCE_MS)
+        assert stream.position_ms == pytest.approx(
+            1000.0 * (200.0 / float(stream.frame_rate)), abs=TIME_TOLERANCE_MS)
 
         # Seek to given time in seconds.
         stream.seek(0)
         assert stream.frame_number == 0
         # FrameTimecode is currently one "behind" the frame_number since it
         # starts counting from zero. This should eventually be changed.
         assert stream.position == stream.base_timecode
@@ -246,14 +235,15 @@
         assert stream.frame_number == 2
 
 
 #
 # Tests which only use a single video file
 #
 
+
 def test_invalid_path(vs_type: Type[VideoStream]):
     """Ensure correct exception is thrown if the path does not exist."""
     with pytest.raises(OSError):
         _ = vs_type('this_path_should_not_exist.mp4')
 
 
 def test_seek_invalid(vs_type: Type[VideoStream], test_video_file: str):
@@ -263,22 +253,31 @@
     with pytest.raises(ValueError):
         stream.seek(-1)
 
     with pytest.raises(ValueError):
         stream.seek(-0.1)
 
 
-
 def test_reset(vs_type: Type[VideoStream], test_video_file: str):
     """Test `reset()` functions as expected."""
     stream = vs_type(test_video_file)
 
     for _ in range(3):
         stream.read()
     assert stream.frame_number > 0
     stream.reset()
     assert stream.frame_number == 0
     assert stream.position == 0
     assert stream.position_ms == pytest.approx(0, abs=TIME_TOLERANCE_MS)
 
 
-
+def test_corrupt_video(vs_type: Type[VideoStream], corrupt_video_file: str):
+    """Test that backend handles video with corrupt frame gracefully with defaults."""
+    if vs_type == VideoManager:
+        pytest.skip(msg='VideoManager does not support handling corrupt videos.')
+
+    stream = vs_type(corrupt_video_file)
+
+    # OpenCV usually fails to read the video at frame 45, so we make sure all backends can
+    # get to 100 without reporting a failure.
+    for frame in range(100):
+        assert stream.read() is not False, "Failed on frame %d!" % frame
```

