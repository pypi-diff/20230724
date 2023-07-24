# Comparing `tmp/figaro-1.2.0.tar.gz` & `tmp/figaro-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.2.0.tar", last modified: Thu Jul 20 14:26:07 2023, max compression
+gzip compressed data, was "figaro-1.2.1.tar", last modified: Mon Jul 24 09:27:01 2023, max compression
```

## Comparing `figaro-1.2.0.tar` & `figaro-1.2.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.168753 figaro-1.2.0/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.2.0/LICENSE
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 09:07:00.000000 figaro-1.2.0/MANIFEST.in
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-20 14:26:07.168138 figaro-1.2.0/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.2.0/README.md
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.085645 figaro-1.2.0/docs/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       55 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/modules.rst
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.104630 figaro-1.2.0/docs/source/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      429 2023-07-16 06:22:36.000000 figaro-1.2.0/docs/source/api.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      142 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.coordinates.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.cosmology.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      159 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.cumulative.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.decorators.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.exceptions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.likelihood.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.load.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.marginal.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      130 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.mixture.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.plot.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      150 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.plot_settings.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      404 2023-07-16 06:21:48.000000 figaro-1.2.0/docs/source/figaro.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.threeDvolume.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.transform.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      124 2023-07-15 19:25:01.000000 figaro-1.2.0/docs/source/figaro.utils.rst
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.123449 figaro-1.2.0/docs/source/generated/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      306 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.coordinates.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      207 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      363 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      231 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      263 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      397 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      278 2023-07-16 06:23:23.000000 figaro-1.2.0/docs/source/generated/figaro.exceptions.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      407 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.likelihood.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      267 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.load.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      211 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      225 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      201 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      357 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      140 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.plot_settings.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      332 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.threeDvolume.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      385 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      320 2023-07-16 06:23:24.000000 figaro-1.2.0/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      996 2023-07-16 06:43:04.000000 figaro-1.2.0/docs/source/index.rst
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.151912 figaro-1.2.0/figaro/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.2.0/figaro/__init__.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2465 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/coordinates.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000320 2023-07-15 09:07:35.000000 figaro-1.2.0/figaro/cosmology.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-15 09:06:46.000000 figaro-1.2.0/figaro/cosmology.pxd
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.2.0/figaro/cosmology.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7604 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/credible_regions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.2.0/figaro/cumulative.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.2.0/figaro/cumulative.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.2.0/figaro/decorators.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8492 2023-07-19 18:35:03.000000 figaro-1.2.0/figaro/diagnostic.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.2.0/figaro/exceptions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5262 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/likelihood.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26408 2023-07-20 13:59:57.000000 figaro-1.2.0/figaro/load.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5953 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/marginal.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    40334 2023-07-20 14:22:33.000000 figaro-1.2.0/figaro/mixture.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2604 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/montecarlo.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.166823 figaro-1.2.0/figaro/pipelines/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.2.0/figaro/pipelines/create_glade.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.2.0/figaro/pipelines/entropy.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.2.0/figaro/pipelines/gen_mock_data.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.2.0/figaro/pipelines/hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.2.0/figaro/pipelines/par_hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.2.0/figaro/pipelines/par_probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.2.0/figaro/pipelines/ppplot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.2.0/figaro/pipelines/probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    38113 2023-07-19 13:23:48.000000 figaro-1.2.0/figaro/plot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.2.0/figaro/plot_settings.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39731 2023-07-15 08:17:11.000000 figaro-1.2.0/figaro/threeDvolume.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2230 2023-07-14 19:38:56.000000 figaro-1.2.0/figaro/transform.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12606 2023-07-20 14:22:33.000000 figaro-1.2.0/figaro/utils.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-20 14:26:07.156752 figaro-1.2.0/figaro.egg-info/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    24809 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/entry_points.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      115 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/requires.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-20 14:26:06.000000 figaro-1.2.0/figaro.egg-info/top_level.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 13:47:26.000000 figaro-1.2.0/pyproject.toml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      114 2023-07-16 06:52:54.000000 figaro-1.2.0/requirements.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-20 14:26:07.168925 figaro-1.2.0/setup.cfg
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4092 2023-07-20 14:25:34.000000 figaro-1.2.0/setup.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.315804 figaro-1.2.1/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.2.1/LICENSE
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 09:07:00.000000 figaro-1.2.1/MANIFEST.in
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-24 09:27:01.315380 figaro-1.2.1/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.2.1/README.md
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.264539 figaro-1.2.1/docs/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       55 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/modules.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.276192 figaro-1.2.1/docs/source/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      429 2023-07-16 06:22:36.000000 figaro-1.2.1/docs/source/api.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      142 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.coordinates.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      159 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.decorators.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.exceptions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.likelihood.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.load.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.marginal.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      130 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.mixture.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.plot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      150 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.plot_settings.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      404 2023-07-16 06:21:48.000000 figaro-1.2.1/docs/source/figaro.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.threeDvolume.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.transform.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      124 2023-07-15 19:25:01.000000 figaro-1.2.1/docs/source/figaro.utils.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.288015 figaro-1.2.1/docs/source/generated/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      306 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.coordinates.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      207 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      363 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      231 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      263 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      397 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      278 2023-07-16 06:23:23.000000 figaro-1.2.1/docs/source/generated/figaro.exceptions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      407 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.likelihood.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      267 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      211 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      225 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      201 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      357 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      140 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.plot_settings.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      332 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.threeDvolume.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      385 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      320 2023-07-16 06:23:24.000000 figaro-1.2.1/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      996 2023-07-16 06:43:04.000000 figaro-1.2.1/docs/source/index.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.305079 figaro-1.2.1/figaro/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.2.1/figaro/__init__.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2465 2023-07-15 08:17:11.000000 figaro-1.2.1/figaro/coordinates.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000320 2023-07-15 09:07:35.000000 figaro-1.2.1/figaro/cosmology.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-15 09:06:46.000000 figaro-1.2.1/figaro/cosmology.pxd
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.2.1/figaro/cosmology.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7604 2023-07-15 08:17:11.000000 figaro-1.2.1/figaro/credible_regions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.2.1/figaro/cumulative.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.2.1/figaro/cumulative.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.2.1/figaro/decorators.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8492 2023-07-19 18:35:03.000000 figaro-1.2.1/figaro/diagnostic.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.2.1/figaro/exceptions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5262 2023-07-24 09:13:19.000000 figaro-1.2.1/figaro/likelihood.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26408 2023-07-21 08:58:08.000000 figaro-1.2.1/figaro/load.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5953 2023-07-15 08:17:11.000000 figaro-1.2.1/figaro/marginal.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    40352 2023-07-24 09:20:22.000000 figaro-1.2.1/figaro/mixture.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2604 2023-07-15 08:17:11.000000 figaro-1.2.1/figaro/montecarlo.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.314844 figaro-1.2.1/figaro/pipelines/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.2.1/figaro/pipelines/create_glade.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.2.1/figaro/pipelines/entropy.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.2.1/figaro/pipelines/gen_mock_data.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.2.1/figaro/pipelines/hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.2.1/figaro/pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.2.1/figaro/pipelines/par_probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.2.1/figaro/pipelines/ppplot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.2.1/figaro/pipelines/probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    38113 2023-07-19 13:23:48.000000 figaro-1.2.1/figaro/plot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.2.1/figaro/plot_settings.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39731 2023-07-15 08:17:11.000000 figaro-1.2.1/figaro/threeDvolume.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2230 2023-07-14 19:38:56.000000 figaro-1.2.1/figaro/transform.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    13373 2023-07-24 09:20:22.000000 figaro-1.2.1/figaro/utils.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-24 09:27:01.309418 figaro-1.2.1/figaro.egg-info/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    24809 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      115 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/requires.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-24 09:27:01.000000 figaro-1.2.1/figaro.egg-info/top_level.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 13:47:26.000000 figaro-1.2.1/pyproject.toml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      114 2023-07-16 06:52:54.000000 figaro-1.2.1/requirements.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-24 09:27:01.315901 figaro-1.2.1/setup.cfg
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4092 2023-07-24 09:26:40.000000 figaro-1.2.1/setup.py
```

### Comparing `figaro-1.2.0/LICENSE` & `figaro-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/PKG-INFO` & `figaro-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.2.0
+Version: 1.2.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.2.0/README.md` & `figaro-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/docs/source/index.rst` & `figaro-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/coordinates.py` & `figaro-1.2.1/figaro/coordinates.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/cosmology.c` & `figaro-1.2.1/figaro/cosmology.c`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/cosmology.pxd` & `figaro-1.2.1/figaro/cosmology.pxd`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/cosmology.pyx` & `figaro-1.2.1/figaro/cosmology.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/credible_regions.py` & `figaro-1.2.1/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/cumulative.c` & `figaro-1.2.1/figaro/cumulative.c`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/cumulative.pyx` & `figaro-1.2.1/figaro/cumulative.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/decorators.py` & `figaro-1.2.1/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/diagnostic.py` & `figaro-1.2.1/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/exceptions.py` & `figaro-1.2.1/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/likelihood.py` & `figaro-1.2.1/figaro/likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/load.py` & `figaro-1.2.1/figaro/load.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/marginal.py` & `figaro-1.2.1/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/mixture.py` & `figaro-1.2.1/figaro/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import dill
 
 from collections import Counter
 from pathlib import Path
 
 from scipy.special import gammaln, logsumexp
 from scipy.stats import multivariate_normal as mn
-from scipy.stats import invwishart, norm, invgamma, dirichlet
+from scipy.stats import invwishart, norm, invgamma, dirichlet, gamma
 
 from figaro.decorators import *
 from figaro.transform import *
 from figaro.likelihood import evaluate_mixture_MC_draws, evaluate_mixture_MC_draws_1d, logsumexp_jit, log_norm, inv_jit
 from figaro.exceptions import except_hook, FIGAROException
-from figaro.utils import get_priors
+from figaro.utils import get_priors, _rescale_matrix
 from figaro.marginal import _condition, _marginalise
 
 from numba import njit, prange
 from numba.extending import get_cython_function_address
 import ctypes
 
 #-----------#
@@ -92,18 +92,18 @@
     
     Returns:
         double: new concentration parameter value
     """
     a_old = alpha
     n_draws = burnin+np.random.randint(100)
     for i in prange(n_draws):
-        a_new = a_old + (np.random.random() - 0.5)
+        a_new = a_old + (np.random.random() - 0.5)*0.1
         if a_new > 0.:
-            logP_old = _numba_gammaln(a_old) - _numba_gammaln(a_old + n) + K * np.log(a_old) - 1./a_old
-            logP_new = _numba_gammaln(a_new) - _numba_gammaln(a_new + n) + K * np.log(a_new) - 1./a_new
+            logP_old = _numba_gammaln(a_old) - _numba_gammaln(a_old + n) + K * np.log(a_old) - a_old
+            logP_new = _numba_gammaln(a_new) - _numba_gammaln(a_new + n) + K * np.log(a_new) - a_new
             if logP_new - logP_old > np.log(np.random.random()):
                 a_old = a_new
     return a_old
 
 @njit
 def _compute_t_pars(nu, L, mean, S, N, dim):
     """
@@ -122,15 +122,15 @@
         np.ndarray: scale matrix for student-t
         np.ndarray: mean for student-t
     """
     # Update hyperparameters
     nu_n, L_n = _compute_hyperpars(nu, L, mean, S, N)
     # Update t-parameters
     t_df    = nu_n - dim + 1
-    t_shape = L_n/t_df
+    t_shape = _rescale_matrix(L_n, t_df)
     return t_df, t_shape, mean
 
 @njit
 def _compute_hyperpars(nu, L, mean, S, N):
     """
     Update hyperparameters for Normal Inverse Gamma/Wishart (NIG/NIW).
     See https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf
@@ -167,18 +167,18 @@
         np.ndarray: updated mean
         np.ndarray: updated covariance
         int:        updated number of samples
         np.ndarray: mean (maximum a posteriori)
         np.ndarray: covariance (maximum a posteriori)
     """
     new_mean  = (mean*N+x)/(N+1)
-    new_S     = (S + N*mean.T@mean + x.T@x) - new_mean.T@new_mean*(N+1)
+    new_S     = (S + _rescale_matrix(np.outer(mean,mean), 1./N) + np.outer(x,x)) - _rescale_matrix(np.outer(new_mean, new_mean), 1./(N+1))
     new_N     = N+1
     new_mu    = new_mean
-    new_sigma = (p_L + new_S)/(p_nu + new_N - x.shape[-1] - 1)
+    new_sigma = _rescale_matrix(p_L + new_S, p_nu + new_N - x.shape[-1] - 1)
     
     return new_mean, new_S, new_N, new_mu, new_sigma
 
 #-------------------#
 # Auxiliary classes #
 #-------------------#
 
@@ -194,15 +194,15 @@
         np.ndarray L:    Wishart scale matrix
     
     Returns:
         prior: instance of prior class
     """
     def __init__(self, L, nu):
         self.nu  = np.max([nu, L.shape[-1]+2])
-        self.L   = L*(self.nu-L.shape[-1]-1)
+        self.L   = _rescale_matrix(L, (self.nu-L.shape[-1]-1))
 
 class _component:
     """
     Class to store the relevant informations for each component in the mixture.
     
     Arguments:
         np.ndarray x: sample added to the new component
@@ -211,16 +211,16 @@
     Returns:
         component: instance of component class
     """
     def __init__(self, x, prior):
         self.N     = 1
         self.mean  = x
         self.S     = np.identity(x.shape[-1])*0.
-        self.mu    = np.atleast_2d(self.mean).astype(np.float64)[0]
-        self.sigma = np.identity(x.shape[-1]).astype(np.float64)*prior.L/(prior.nu - x.shape[-1] - 1)
+        self.mu    = self.mean
+        self.sigma = _rescale_matrix(prior.L, (prior.nu - x.shape[-1] - 1))
 
 class _component_h:
     """
     Class to store the relevant informations for each component in the mixture.
     To be used in hierarchical inference.
     
     Arguments:
@@ -797,15 +797,18 @@
         
         Returns:
             double: log Likelihood
         """
         if ss is None:
             return -self.log_V
         t_df, t_shape, mu_n = _compute_t_pars(self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
-        return _student_t(df = t_df, t = x, mu = mu_n, sigma = t_shape, dim = self.dim)
+        try:
+            return _student_t(df = t_df, t = x, mu = mu_n, sigma = t_shape, dim = self.dim)
+        except np.linalg.LinAlgError:
+            return -np.inf
 
     def _cluster_assignment_distribution(self, x):
         """
         Compute the marginal distribution of cluster assignment for each cluster.
         
         Arguments:
             np.ndarray x: sample
@@ -887,18 +890,15 @@
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
         means     = np.zeros((self.n_cl, self.dim))
         variances = np.zeros((self.n_cl, self.dim, self.dim))
         for i, ss in enumerate(self.mixture):
             nu_n, L_n = _compute_hyperpars(self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
             variances[i] = invwishart(df = nu_n, scale = L_n).rvs()
-            if ss.N == 1:
-                means[i] = mn(mean = ss.mean[0], cov = L_n/(nu_n - self.dim + 1), allow_singular = True).rvs()
-            else:
-                means[i] = mn(mean = ss.mean[0], cov = ss.S/ss.N**2, allow_singular = True).rvs()
+            means[i] = mn(mean = ss.mean[0], cov = _rescale_matrix(ss.sigma, ss.N), allow_singular = True).rvs()
         w = dirichlet(self.w*self.n_pts+self.alpha/self.n_cl).rvs()[0]
         return mixture(means, variances, w, self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
 
     # Methods to overwrite density methods
     def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
```

### Comparing `figaro-1.2.0/figaro/montecarlo.py` & `figaro-1.2.1/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/create_glade.py` & `figaro-1.2.1/figaro/pipelines/create_glade.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/entropy.py` & `figaro-1.2.1/figaro/pipelines/entropy.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/gen_mock_data.py` & `figaro-1.2.1/figaro/pipelines/gen_mock_data.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/hierarchical_inference.py` & `figaro-1.2.1/figaro/pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/par_hierarchical_inference.py` & `figaro-1.2.1/figaro/pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/par_probability_density.py` & `figaro-1.2.1/figaro/pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/ppplot.py` & `figaro-1.2.1/figaro/pipelines/ppplot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/pipelines/probability_density.py` & `figaro-1.2.1/figaro/pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/plot.py` & `figaro-1.2.1/figaro/plot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/plot_settings.py` & `figaro-1.2.1/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/threeDvolume.py` & `figaro-1.2.1/figaro/threeDvolume.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/transform.py` & `figaro-1.2.1/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/figaro/utils.py` & `figaro-1.2.1/figaro/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import numpy as np
 import warnings
 import dill
 import configparser
 
 from pathlib import Path
 from tqdm import tqdm
+from numba import njit
 from typing import cast
 from collections import Counter
 from scipy.stats import multivariate_normal as mn
 
 from figaro.transform import transform_to_probit, transform_from_probit
 from figaro.exceptions import FIGAROException
 
 #-–––––––––-#
 # Utilities #
 #-----------#
 
+@njit
+def _rescale_matrix(S, n):
+    std = np.sqrt(np.diag(S))
+    rho = np.divide(S, np.outer(std,std))
+    return rho * np.outer(std/np.sqrt(n), std/np.sqrt(n))
+
 def recursive_grid(bounds, n_pts, get_1d = False):
     """
     Recursively generates the n-dimensional grid points (extremes are excluded).
     
     Arguments:
         list-of-lists bounds: extremes for each dimension (excluded)
         int n_pts:            number of points for each dimension
@@ -78,33 +85,37 @@
         probs = f(pts)*selfunc(pts)
         h     = np.random.uniform(0, top, size = n_draws)
         samples.extend(pts[np.where(h < probs)])
     return np.array(samples).flatten()[:n_draws]
 
 def get_priors(bounds, samples = None, mean = None, std = None, cov = None, df = None, k = None, a = None, scale = None, probit = True, hierarchical = False):
     """
-    This method takes the prior parameters for the Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
+    This method takes the prior parameters for the Normal-Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
 
-    Two parameters are returned:
+    Four parameters are returned:
         * df, is the number of degrees of freedom for the Inverse Wishart distribution,. It must be greater than D+1. If this parameter is None or does not satisfy the condition df > D+1, the default value D+2 is used;
+        * k is the scale parameter for the multivariate Normal distribution. Suggested values are  k <~ 1e-1. If None, the default value 1e-2 is used.
+        * mu is the mean of the multivariate Normal distribution. It can be either estimated from the available samples or passed directly as a 1D array with length D (the keyword argument mean overrides the samples). If None, the default value 0 (corresponding to the parameter space center) is used.
         * L is the expected value for the Inverse Wishart distribution. This parameter can be either (in descending priority order):
             * passed as 2D array with shape (D,D), the covariance matrix - keyword cov;
             * passed as 1D array with shape (D,) or double: vector of standard deviations (if double, it assumes that the same std has to be used for all dimensions) - keyword std;
             * estimated from samples - keyword samples.
        
-    The order in which they are returned is (L,df).
+    The order in which they are returned is (k,L,df,mu).
     
     Arguments:
         np.ndarray bounds:              boundaries for probit transformation
         np.ndarray samples:             2D [DPGMM] or 3D [(H)DPGMM] array with samples
+        double or np.ndarray mean:      mean [DPGMM]
         double or np.ndarray std:       expected standard deviation (if double, the same std is used for all dimensions, if np.ndarray must match the number of dimensions) [DPGMM and (H)DPGMM]
         np.ndarray cov:                 covariance matrix [DPGMM]
-        int df:                         degrees of freedom for Inverse Gamma/Inverse Wishart distribution [DPGMM]
+        int df:                         degrees of freedom for Inverse Wishart distribution [DPGMM]
+        double k:                       scale parameter for Normal distribution [DPGMM]
         double a:                       shape parameter for the Inverse Gamma distribution [(H)DPGMM]
-        double scale:                   fraction of samples std [DPGMM and (H)DPGMM]
+        double scale:                   fraction of samples std [DPGMM]
         bool probit:                    whether the probit transformation will be applied or not
         bool hierarchical:              returns the prior pars for (H)DPGMM rather than for DPGMM
         
     Returns:
         tuple: prior parameters ordered as in (H)/DPGMM
     """
     bounds = np.atleast_2d(bounds)
```

### Comparing `figaro-1.2.0/figaro.egg-info/PKG-INFO` & `figaro-1.2.1/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.2.0
+Version: 1.2.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.2.0/figaro.egg-info/SOURCES.txt` & `figaro-1.2.1/figaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figaro-1.2.0/setup.py` & `figaro-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     include_dirs = ['figaro', numpy.get_include()],
     setup_requires=['numpy', 'cython'],
     package_data={"": ['*.c', '*.pyx', '*.pxd']},
     ext_modules=ext_modules,
     entry_points = {
         'console_scripts': scripts,
         },
-    version='1.2.0',
+    version='1.2.1',
     long_description=long_description,
     long_description_content_type='text/markdown',
     cmdclass = {
             "build_ext": build_ext
             }
     )
```

