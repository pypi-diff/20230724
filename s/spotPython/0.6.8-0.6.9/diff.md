# Comparing `tmp/spotPython-0.6.8.tar.gz` & `tmp/spotPython-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.6.8.tar", last modified: Sun Jul 23 21:39:14 2023, max compression
+gzip compressed data, was "spotPython-0.6.9.tar", last modified: Mon Jul 24 09:27:35 2023, max compression
```

## Comparing `spotPython-0.6.8.tar` & `spotPython-0.6.9.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.984879 spotPython-0.6.8/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.954779 spotPython-0.6.8/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.958699 spotPython-0.6.8/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.6.8/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    17867 2023-07-04 14:15:14.000000 spotPython-0.6.8/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.6.8/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.964192 spotPython-0.6.8/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.6.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.6.8/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.6.8/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-23 21:39:14.984708 spotPython-0.6.8/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-08 16:18:46.000000 spotPython-0.6.8/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.965068 spotPython-0.6.8/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2022-10-31 16:48:05.000000 spotPython-0.6.8/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-12 23:09:54.000000 spotPython-0.6.8/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-16 08:32:11.000000 spotPython-0.6.8/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2022-10-31 16:48:05.000000 spotPython-0.6.8/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-14 22:03:54.000000 spotPython-0.6.8/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.965337 spotPython-0.6.8/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.8/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.8/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-15 18:25:23.000000 spotPython-0.6.8/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.965586 spotPython-0.6.8/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 05:52:18.000000 spotPython-0.6.8/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.6.8/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-07-15 09:35:47.000000 spotPython-0.6.8/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)     1822 2023-07-23 20:44:39.000000 spotPython-0.6.8/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.966482 spotPython-0.6.8/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-15 20:49:26.000000 spotPython-0.6.8/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   953519 2023-07-04 14:15:14.000000 spotPython-0.6.8/notebooks/31_spot_lightning_csv.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.955493 spotPython-0.6.8/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.966606 spotPython-0.6.8/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.6.8/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.6.8/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.972498 spotPython-0.6.8/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-07 17:28:19.000000 spotPython-0.6.8/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-08 12:22:25.000000 spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-08 12:22:25.000000 spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-08 12:22:25.000000 spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-07 11:49:47.000000 spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-07 11:04:53.000000 spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-07 11:10:20.000000 spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
--rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-07 11:11:28.000000 spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
--rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-24 19:48:27.000000 spotPython-0.6.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-24 19:48:27.000000 spotPython-0.6.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-07 05:09:22.000000 spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-06 21:13:57.000000 spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-07 06:30:18.000000 spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-06 21:13:56.000000 spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.6.8/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.6.8/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.6.8/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-07 06:48:45.000000 spotPython-0.6.8/notebooks/figures/tensorboard_0.png
--rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-07 06:46:35.000000 spotPython-0.6.8/notebooks/figures/tensorboard_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-07 06:51:03.000000 spotPython-0.6.8/notebooks/figures/tensorboard_hdparams.png
--rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-07 06:53:15.000000 spotPython-0.6.8/notebooks/figures/tensorboard_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)     1507 2023-07-23 20:48:02.000000 spotPython-0.6.8/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-07-23 21:39:14.984922 spotPython-0.6.8/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.955880 spotPython-0.6.8/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.956995 spotPython-0.6.8/src/spotPython/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.974392 spotPython-0.6.8/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     3888 2023-07-23 20:55:05.000000 spotPython-0.6.8/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.974674 spotPython-0.6.8/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    55582 2023-07-23 21:27:59.000000 spotPython-0.6.8/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.6.8/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.975925 spotPython-0.6.8/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.6.8/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    23267 2023-07-17 19:56:10.000000 spotPython-0.6.8/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     6159 2023-07-18 19:53:58.000000 spotPython-0.6.8/src/spotPython/data/light_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     1036 2023-07-17 20:01:02.000000 spotPython-0.6.8/src/spotPython/data/light_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.6.8/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     1282 2023-07-17 20:05:39.000000 spotPython-0.6.8/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-06 20:04:52.000000 spotPython-0.6.8/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)     1262 2023-07-17 20:07:25.000000 spotPython-0.6.8/src/spotPython/data/torch_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     1471 2023-07-17 20:09:39.000000 spotPython-0.6.8/src/spotPython/data/torchdata.py
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-07-17 20:14:22.000000 spotPython-0.6.8/src/spotPython/data/vbdp.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.976302 spotPython-0.6.8/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)     1223 2023-07-17 22:31:41.000000 spotPython-0.6.8/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)     1299 2023-07-23 21:35:33.000000 spotPython-0.6.8/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2227 2023-07-23 21:36:02.000000 spotPython-0.6.8/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.976762 spotPython-0.6.8/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     4647 2023-07-23 21:36:25.000000 spotPython-0.6.8/src/spotPython/fun/hyperlight.py
--rw-r--r--   0 bartz      (501) staff       (20)     5720 2023-07-18 05:26:06.000000 spotPython-0.6.8/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     7435 2023-07-17 20:59:08.000000 spotPython-0.6.8/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    26824 2023-07-15 21:02:46.000000 spotPython-0.6.8/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.977118 spotPython-0.6.8/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4856 2023-07-23 21:37:39.000000 spotPython-0.6.8/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     5113 2023-07-17 21:02:24.000000 spotPython-0.6.8/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    34602 2023-07-17 21:26:45.000000 spotPython-0.6.8/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.978817 spotPython-0.6.8/src/spotPython/light/
--rw-r--r--   0 bartz      (501) staff       (20)     3426 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/cifar10datamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     4882 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/crossvalidationdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     4120 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/csvdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     3313 2023-07-17 21:43:36.000000 spotPython-0.6.8/src/spotPython/light/csvdataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     5546 2023-07-17 21:54:43.000000 spotPython-0.6.8/src/spotPython/light/litmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-25 16:06:47.000000 spotPython-0.6.8/src/spotPython/light/mnistdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)    12288 2023-07-18 19:40:25.000000 spotPython-0.6.8/src/spotPython/light/netlightbase.py
--rw-r--r--   0 bartz      (501) staff       (20)    13445 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/netlinearbase.py
--rw-r--r--   0 bartz      (501) staff       (20)    11119 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/traintest.py
--rw-r--r--   0 bartz      (501) staff       (20)    11435 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/traintest_NEW.py
--rw-r--r--   0 bartz      (501) staff       (20)    11131 2023-07-20 07:13:47.000000 spotPython-0.6.8/src/spotPython/light/traintest_OLD.py
--rw-r--r--   0 bartz      (501) staff       (20)      255 2023-07-02 17:23:44.000000 spotPython-0.6.8/src/spotPython/light/utils.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.979033 spotPython-0.6.8/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1708 2023-07-23 21:37:57.000000 spotPython-0.6.8/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     5949 2023-07-15 21:05:52.000000 spotPython-0.6.8/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.979150 spotPython-0.6.8/src/spotPython/sklearn/
--rw-r--r--   0 bartz      (501) staff       (20)     3715 2023-06-07 16:26:19.000000 spotPython-0.6.8/src/spotPython/sklearn/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.979267 spotPython-0.6.8/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    39594 2023-07-15 20:52:28.000000 spotPython-0.6.8/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.980500 spotPython-0.6.8/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-23 13:29:53.000000 spotPython-0.6.8/src/spotPython/torch/activation.py
--rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.6.8/src/spotPython/torch/dataframedataset.py
--rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 22:26:23.000000 spotPython-0.6.8/src/spotPython/torch/initialization.py
--rw-r--r--   0 bartz      (501) staff       (20)     4570 2023-07-15 20:49:35.000000 spotPython-0.6.8/src/spotPython/torch/mapk.py
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.6.8/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.6.8/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.6.8/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-06 19:59:34.000000 spotPython-0.6.8/src/spotPython/torch/netregression.py
--rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.6.8/src/spotPython/torch/netvbdp.py
--rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-20 05:35:32.000000 spotPython-0.6.8/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.981839 spotPython-0.6.8/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2019 2023-07-23 21:38:32.000000 spotPython-0.6.8/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.6.8/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1484 2023-07-23 21:33:07.000000 spotPython-0.6.8/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     3764 2023-07-15 20:51:00.000000 spotPython-0.6.8/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      628 2023-07-15 21:01:58.000000 spotPython-0.6.8/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     9289 2023-07-15 20:33:18.000000 spotPython-0.6.8/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)     3299 2023-07-15 20:40:43.000000 spotPython-0.6.8/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     5846 2023-07-15 20:53:33.000000 spotPython-0.6.8/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.6.8/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.6.8/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1381 2023-07-23 21:38:50.000000 spotPython-0.6.8/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     6826 2023-07-15 20:54:18.000000 spotPython-0.6.8/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.974252 spotPython-0.6.8/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-23 21:39:14.000000 spotPython-0.6.8/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     8273 2023-07-23 21:39:14.000000 spotPython-0.6.8/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-07-23 21:39:14.000000 spotPython-0.6.8/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      216 2023-07-23 21:39:14.000000 spotPython-0.6.8/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-07-23 21:39:14.000000 spotPython-0.6.8/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-23 21:39:14.984480 spotPython-0.6.8/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.6.8/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.6.8/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.6.8/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.6.8/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.6.8/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.253973 spotPython-0.6.9/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.130687 spotPython-0.6.9/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.137294 spotPython-0.6.9/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-05 01:17:02.000000 spotPython-0.6.9/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    17867 2023-07-04 13:42:00.000000 spotPython-0.6.9/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 20:25:57.000000 spotPython-0.6.9/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.158503 spotPython-0.6.9/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 21:46:16.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-08 15:19:19.000000 spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-07 19:44:11.000000 spotPython-0.6.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-01-30 12:58:45.000000 spotPython-0.6.9/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-23 10:59:22.000000 spotPython-0.6.9/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-24 09:27:35.253569 spotPython-0.6.9/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-09 14:13:36.000000 spotPython-0.6.9/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.161785 spotPython-0.6.9/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2023-07-13 14:40:46.000000 spotPython-0.6.9/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-13 14:40:46.000000 spotPython-0.6.9/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-17 08:56:18.000000 spotPython-0.6.9/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2023-07-13 14:40:46.000000 spotPython-0.6.9/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-17 08:56:18.000000 spotPython-0.6.9/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.162546 spotPython-0.6.9/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 14:40:46.000000 spotPython-0.6.9/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 14:40:46.000000 spotPython-0.6.9/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-17 08:56:18.000000 spotPython-0.6.9/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.163350 spotPython-0.6.9/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-17 08:56:18.000000 spotPython-0.6.9/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-06-09 14:13:36.000000 spotPython-0.6.9/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-07-17 08:56:18.000000 spotPython-0.6.9/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     1822 2023-07-24 08:17:37.000000 spotPython-0.6.9/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.168566 spotPython-0.6.9/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-17 08:56:18.000000 spotPython-0.6.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   953519 2023-07-04 13:42:01.000000 spotPython-0.6.9/notebooks/31_spot_lightning_csv.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.131611 spotPython-0.6.9/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.169112 spotPython-0.6.9/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-15 06:42:12.000000 spotPython-0.6.9/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-25 23:35:15.000000 spotPython-0.6.9/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.206392 spotPython-0.6.9/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
+-rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
+-rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-26 10:36:37.000000 spotPython-0.6.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-26 10:36:37.000000 spotPython-0.6.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-27 21:08:47.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 04:57:10.000000 spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-01-30 12:58:45.000000 spotPython-0.6.9/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-01-30 12:58:45.000000 spotPython-0.6.9/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-01-30 12:58:45.000000 spotPython-0.6.9/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/tensorboard_0.png
+-rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/tensorboard_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/tensorboard_hdparams.png
+-rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-09 14:13:36.000000 spotPython-0.6.9/notebooks/figures/tensorboard_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1507 2023-07-24 08:35:31.000000 spotPython-0.6.9/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-07-24 09:27:35.254068 spotPython-0.6.9/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.132088 spotPython-0.6.9/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.133637 spotPython-0.6.9/src/spotPython/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.214012 spotPython-0.6.9/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     3888 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.214706 spotPython-0.6.9/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    55582 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-01-30 12:58:45.000000 spotPython-0.6.9/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.220708 spotPython-0.6.9/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-23 10:59:22.000000 spotPython-0.6.9/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    23267 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6159 2023-07-19 07:52:35.000000 spotPython-0.6.9/src/spotPython/data/light_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1036 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/light_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 11:46:53.000000 spotPython-0.6.9/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1282 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-09 14:13:36.000000 spotPython-0.6.9/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1262 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/torch_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1471 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/torchdata.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/data/vbdp.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.222035 spotPython-0.6.9/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)     1223 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1299 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2227 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.223983 spotPython-0.6.9/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     4647 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/fun/hyperlight.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5720 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7435 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26824 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.225436 spotPython-0.6.9/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4856 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5113 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    34602 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.232556 spotPython-0.6.9/src/spotPython/light/
+-rw-r--r--   0 bartz      (501) staff       (20)     3426 2023-07-19 08:08:13.000000 spotPython-0.6.9/src/spotPython/light/cifar10datamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4882 2023-07-19 11:01:58.000000 spotPython-0.6.9/src/spotPython/light/crossvalidationdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4120 2023-07-19 10:30:12.000000 spotPython-0.6.9/src/spotPython/light/csvdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3313 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/light/csvdataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5546 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/light/litmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-26 10:36:37.000000 spotPython-0.6.9/src/spotPython/light/mnistdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)    12288 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/light/netlightbase.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13445 2023-07-19 09:48:01.000000 spotPython-0.6.9/src/spotPython/light/netlinearbase.py
+-rw-r--r--   0 bartz      (501) staff       (20)    11119 2023-07-19 10:54:19.000000 spotPython-0.6.9/src/spotPython/light/traintest.py
+-rw-r--r--   0 bartz      (501) staff       (20)    11435 2023-07-19 08:08:09.000000 spotPython-0.6.9/src/spotPython/light/traintest_NEW.py
+-rw-r--r--   0 bartz      (501) staff       (20)    11131 2023-07-18 07:18:07.000000 spotPython-0.6.9/src/spotPython/light/traintest_OLD.py
+-rw-r--r--   0 bartz      (501) staff       (20)      255 2023-07-02 19:29:48.000000 spotPython-0.6.9/src/spotPython/light/utils.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.233425 spotPython-0.6.9/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1708 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5949 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.234075 spotPython-0.6.9/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3715 2023-06-09 14:13:36.000000 spotPython-0.6.9/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.234701 spotPython-0.6.9/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    39594 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.241359 spotPython-0.6.9/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-26 10:36:37.000000 spotPython-0.6.9/src/spotPython/torch/activation.py
+-rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 23:03:53.000000 spotPython-0.6.9/src/spotPython/torch/dataframedataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 23:06:07.000000 spotPython-0.6.9/src/spotPython/torch/initialization.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5191 2023-07-24 08:34:12.000000 spotPython-0.6.9/src/spotPython/torch/mapk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 21:08:47.000000 spotPython-0.6.9/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 21:08:47.000000 spotPython-0.6.9/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 21:08:47.000000 spotPython-0.6.9/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-09 14:13:36.000000 spotPython-0.6.9/src/spotPython/torch/netregression.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-02 14:39:41.000000 spotPython-0.6.9/src/spotPython/torch/netvbdp.py
+-rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-18 09:30:24.000000 spotPython-0.6.9/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.247117 spotPython-0.6.9/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2019 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-14 07:02:46.000000 spotPython-0.6.9/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1484 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3764 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      628 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9289 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3299 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5846 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-06-26 11:21:46.000000 spotPython-0.6.9/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-02 14:39:41.000000 spotPython-0.6.9/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1381 2023-07-24 08:17:37.000000 spotPython-0.6.9/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6826 2023-07-17 08:56:18.000000 spotPython-0.6.9/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.213669 spotPython-0.6.9/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-24 09:27:35.000000 spotPython-0.6.9/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     8273 2023-07-24 09:27:35.000000 spotPython-0.6.9/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-07-24 09:27:35.000000 spotPython-0.6.9/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      216 2023-07-24 09:27:35.000000 spotPython-0.6.9/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-07-24 09:27:35.000000 spotPython-0.6.9/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-24 09:27:35.252984 spotPython-0.6.9/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-11 06:36:10.000000 spotPython-0.6.9/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-11 06:36:10.000000 spotPython-0.6.9/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-11 06:36:10.000000 spotPython-0.6.9/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-01-30 12:58:45.000000 spotPython-0.6.9/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 13:13:30.000000 spotPython-0.6.9/tox.ini
```

### Comparing `spotPython-0.6.8/.github/workflows/test.yml` & `spotPython-0.6.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/.gitignore` & `spotPython-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.6.9/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.6.9/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.6.9/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.6.9/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/LICENSE.txt` & `spotPython-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/PKG-INFO` & `spotPython-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.6.8
+Version: 0.6.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.6.8/README.md` & `spotPython-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/docs/about.md` & `spotPython-0.6.9/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/docs/examples.md` & `spotPython-0.6.9/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/docs/gen_ref_pages.py` & `spotPython-0.6.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/docs/images/favicon.png` & `spotPython-0.6.9/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/docs/images/spotlogo.png` & `spotPython-0.6.9/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/img/favicon.png` & `spotPython-0.6.9/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/img/spotLogo.png` & `spotPython-0.6.9/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/mkdocs.yml` & `spotPython-0.6.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb` & `spotPython-0.6.9/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/31_spot_lightning_csv.ipynb` & `spotPython-0.6.9/notebooks/31_spot_lightning_csv.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.6.9/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png` & `spotPython-0.6.9/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png` & `spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png` & `spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png` & `spotPython-0.6.9/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png` & `spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png` & `spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png` & `spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png` & `spotPython-0.6.9/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png` & `spotPython-0.6.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png` & `spotPython-0.6.9/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.6.9/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png` & `spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png` & `spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png` & `spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png` & `spotPython-0.6.9/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/spotModel.graffle` & `spotPython-0.6.9/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/spotModel.pdf` & `spotPython-0.6.9/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/spotModel.png` & `spotPython-0.6.9/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/tensorboard_0.png` & `spotPython-0.6.9/notebooks/figures/tensorboard_0.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/tensorboard_1.png` & `spotPython-0.6.9/notebooks/figures/tensorboard_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/tensorboard_hdparams.png` & `spotPython-0.6.9/notebooks/figures/tensorboard_hdparams.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/notebooks/figures/tensorboard_parallel.png` & `spotPython-0.6.9/notebooks/figures/tensorboard_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/pyproject.toml` & `spotPython-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.6.8/src/spotPython/budget/ocba.py` & `spotPython-0.6.9/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/build/kriging.py` & `spotPython-0.6.9/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/base.py` & `spotPython-0.6.9/src/spotPython/data/base.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/light_hyper_dict.json` & `spotPython-0.6.9/src/spotPython/data/light_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/light_hyper_dict.py` & `spotPython-0.6.9/src/spotPython/data/light_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.6.9/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/sklearn_hyper_dict.py` & `spotPython-0.6.9/src/spotPython/data/sklearn_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.6.9/src/spotPython/data/torch_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/torch_hyper_dict.py` & `spotPython-0.6.9/src/spotPython/data/torch_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/torchdata.py` & `spotPython-0.6.9/src/spotPython/data/torchdata.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/data/vbdp.py` & `spotPython-0.6.9/src/spotPython/data/vbdp.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/design/designs.py` & `spotPython-0.6.9/src/spotPython/design/designs.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/design/factorial.py` & `spotPython-0.6.9/src/spotPython/design/factorial.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/design/spacefilling.py` & `spotPython-0.6.9/src/spotPython/design/spacefilling.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/fun/hyperlight.py` & `spotPython-0.6.9/src/spotPython/fun/hyperlight.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/fun/hypersklearn.py` & `spotPython-0.6.9/src/spotPython/fun/hypersklearn.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/fun/hypertorch.py` & `spotPython-0.6.9/src/spotPython/fun/hypertorch.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.6.9/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.6.9/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.6.9/src/spotPython/hyperparameters/optimizer.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/hyperparameters/values.py` & `spotPython-0.6.9/src/spotPython/hyperparameters/values.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/cifar10datamodule.py` & `spotPython-0.6.9/src/spotPython/light/cifar10datamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/crossvalidationdatamodule.py` & `spotPython-0.6.9/src/spotPython/light/crossvalidationdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/csvdatamodule.py` & `spotPython-0.6.9/src/spotPython/light/csvdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/csvdataset.py` & `spotPython-0.6.9/src/spotPython/light/csvdataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/litmodel.py` & `spotPython-0.6.9/src/spotPython/light/litmodel.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/mnistdatamodule.py` & `spotPython-0.6.9/src/spotPython/light/mnistdatamodule.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/netlightbase.py` & `spotPython-0.6.9/src/spotPython/light/netlightbase.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/netlinearbase.py` & `spotPython-0.6.9/src/spotPython/light/netlinearbase.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/traintest.py` & `spotPython-0.6.9/src/spotPython/light/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/traintest_NEW.py` & `spotPython-0.6.9/src/spotPython/light/traintest_NEW.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/light/traintest_OLD.py` & `spotPython-0.6.9/src/spotPython/light/traintest_OLD.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/plot/contour.py` & `spotPython-0.6.9/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/plot/validation.py` & `spotPython-0.6.9/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/sklearn/traintest.py` & `spotPython-0.6.9/src/spotPython/sklearn/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/spot/spot.py` & `spotPython-0.6.9/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/activation.py` & `spotPython-0.6.9/src/spotPython/torch/activation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/dataframedataset.py` & `spotPython-0.6.9/src/spotPython/torch/dataframedataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/initialization.py` & `spotPython-0.6.9/src/spotPython/torch/initialization.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/mapk.py` & `spotPython-0.6.9/src/spotPython/torch/mapk.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,18 +53,34 @@
             predicted (torch.Tensor):
                 A 2D tensor containing the predicted scores for each class.
             actual (torch.Tensor):
                 A 1D tensor containing the ground truth labels.
         Returns:
             (NoneType): None
 
+        Examples:
+            >>> from spotPython.torch.mapk import MAPK
+            >>> import torch
+            >>> mapk = MAPK(k=2)
+            >>> target = torch.tensor([0, 1, 2, 2])
+            >>> preds = torch.tensor(
+            ...     [
+            ...         [0.5, 0.2, 0.2],  # 0 is in top 2
+            ...         [0.3, 0.4, 0.2],  # 1 is in top 2
+            ...         [0.2, 0.4, 0.3],  # 2 is in top 2
+            ...         [0.7, 0.2, 0.1],  # 2 isn't in top 2
+            ...     ]
+            ... )
+            >>> mapk.update(preds, target)
+            >>> print(mapk.compute()) # tensor(0.6250)
+
         Raises:
-            AssertionError:
-                If `actual` is not a 1D tensor or if `predicted` is not a 2D tensor
-                or if `actual` and `predicted` do not have the same number of elements.
+            AssertionError: If the actual tensor is not 1D or the predicted tensor is not 2D.
+            AssertionError: If the number of elements in the actual and predicted tensors are not equal.
+
         """
         assert len(actual.shape) == 1, "actual must be a 1D tensor"
         assert len(predicted.shape) == 2, "predicted must be a 2D tensor"
         assert actual.shape[0] == predicted.shape[0], "actual and predicted must have the same number of elements"
 
         # Convert actual to list of lists
         actual = actual.tolist()
```

### Comparing `spotPython-0.6.8/src/spotPython/torch/netcifar10.py` & `spotPython-0.6.9/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.6.9/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/netregression.py` & `spotPython-0.6.9/src/spotPython/torch/netregression.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/netvbdp.py` & `spotPython-0.6.9/src/spotPython/torch/netvbdp.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/torch/traintest.py` & `spotPython-0.6.9/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/aggregate.py` & `spotPython-0.6.9/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/compare.py` & `spotPython-0.6.9/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/convert.py` & `spotPython-0.6.9/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/device.py` & `spotPython-0.6.9/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/eda.py` & `spotPython-0.6.9/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/file.py` & `spotPython-0.6.9/src/spotPython/utils/file.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/init.py` & `spotPython-0.6.9/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/metrics.py` & `spotPython-0.6.9/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/progress.py` & `spotPython-0.6.9/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/repair.py` & `spotPython-0.6.9/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython/utils/transform.py` & `spotPython-0.6.9/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.6.9/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.6.8
+Version: 0.6.9
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.6.8/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.6.9/src/spotPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_aggregate_mean_var.py` & `spotPython-0.6.9/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_build_Psi.py` & `spotPython-0.6.9/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_build_U.py` & `spotPython-0.6.9/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_build_psi_vec.py` & `spotPython-0.6.9/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_evaluate_new_X.py` & `spotPython-0.6.9/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_evaluate_new_solutions.py` & `spotPython-0.6.9/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_extract_from_bounds.py` & `spotPython-0.6.9/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_generate_design.py` & `spotPython-0.6.9/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_infill.py` & `spotPython-0.6.9/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_nat_to_cod.py` & `spotPython-0.6.9/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_nat_to_cod_init.py` & `spotPython-0.6.9/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_ocba.py` & `spotPython-0.6.9/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_repair_non_numeric.py` & `spotPython-0.6.9/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_set_de_bounds.py` & `spotPython-0.6.9/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_show_progress.py` & `spotPython-0.6.9/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_suggest_new_X.py` & `spotPython-0.6.9/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.8/test/test_update_surrogate.py` & `spotPython-0.6.9/test/test_update_surrogate.py`

 * *Files identical despite different names*

