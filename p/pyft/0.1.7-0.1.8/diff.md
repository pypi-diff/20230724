# Comparing `tmp/pyft-0.1.7.tar.gz` & `tmp/pyft-0.1.8.tar.gz`

## Comparing `pyft-0.1.7.tar` & `pyft-0.1.8.tar`

### file list

```diff
@@ -1,91 +1,90 @@
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pyft-0.1.7/local_dependencies/bamlift/Cargo.toml
--rw-r--r--   0      501       20    11043 2023-07-23 00:01:50.000000 pyft-0.1.7/local_dependencies/bamlift/src/lib.rs
--rw-r--r--   0      501       20     1043 2023-07-22 20:22:41.000000 pyft-0.1.7/local_dependencies/bamlift/tests/test-liftover.rs
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.7/local_dependencies/bio-io/Cargo.toml
--rw-r--r--   0      501       20    10927 2023-07-21 23:45:13.000000 pyft-0.1.7/local_dependencies/bio-io/src/lib.rs
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pyft-0.1.7/local_dependencies/fibertools-rs/Cargo.toml
--rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.cargo/config
--rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.dockerignore
--rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.github/workflows/CI.yml
--rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.github/workflows/release.yml
--rw-r--r--   0      501       20      211 2023-07-22 20:39:35.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.gitignore
--rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.pre-commit-config.yaml
--rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.7/local_dependencies/fibertools-rs/.readthedocs.yaml
--rw-------   0      501       20   122462 2023-07-21 08:31:15.000000 pyft-0.1.7/local_dependencies/fibertools-rs/CHANGELOG.md
--rw-r--r--   0      501       20    63353 2023-07-22 22:51:02.000000 pyft-0.1.7/local_dependencies/fibertools-rs/Cargo.lock
--rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.7/local_dependencies/fibertools-rs/Dockerfile
--rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.7/local_dependencies/fibertools-rs/INSTALL.md
--rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/NOTES.md
--rw-r--r--   0      501       20     4471 2023-07-21 07:53:23.000000 pyft-0.1.7/local_dependencies/fibertools-rs/README.md
--rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/_config.yml
--rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/center.png
--rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
--rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
--rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
--rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/logo.png
--rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.7/local_dependencies/fibertools-rs/build.rs
--rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft--help.md
--rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
--rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-all-columns.md
--rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-center-help.md
--rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
--rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-extract-help.md
--rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
--rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
--rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/docs/make_help_docs.sh
--rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.7/local_dependencies/fibertools-rs/env.yaml
--rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
--rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_torch.pt
--rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
--rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_torch.pt
--rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
--rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
--rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
--rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
--rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
--rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.7/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
--rw-r--r--   0      501       20    18323 2023-07-22 22:54:01.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/basemods/mod.rs
--rw-r--r--   0      501       20    12588 2023-07-22 20:33:30.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/center.rs
--rw-r--r--   0      501       20    10971 2023-07-22 19:51:25.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/cli.rs
--rw-r--r--   0      501       20    18362 2023-07-22 20:40:22.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/extract.rs
--rw-r--r--   0      501       20     4129 2023-07-22 01:59:45.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/lib.rs
--rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/main.rs
--rw-r--r--   0      501       20    12907 2023-07-21 05:47:41.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/nucleosomes.rs
--rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
--rw-r--r--   0      501       20    18361 2023-07-21 00:03:41.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
--rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
--rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.7/local_dependencies/fibertools-rs/src/strip_basemods.rs
--rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/all.bam
--rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/all.bam.bai
--rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bam
--rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bam.bai
--rw-r--r--   0      501       20     3349 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bed
--rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
--rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/test.txt
--rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/test.txt.gz
--rw-r--r--   0      501       20     1780 2023-07-21 22:42:46.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/extract_test.rs
--rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.7/local_dependencies/fibertools-rs/tests/run_test.rs
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pyft-0.1.7/Cargo.toml
--rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.7/.github/workflows/CI.yml
--rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.7/.gitignore
--rw-r--r--   0      501       20      382 2023-07-23 16:19:13.000000 pyft-0.1.7/README.md
--rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.7/docs/Makefile
--rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.7/docs/_static/css/rtd_dark.css
--rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.7/docs/_static/img/fiber_tools_grey.png
--rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.7/docs/_templates/layout.html
--rw-r--r--   0      501       20     1695 2023-07-23 14:42:32.000000 pyft-0.1.7/docs/conf.py
--rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.7/docs/environment.yml
--rw-r--r--   0      501       20     1277 2023-07-23 16:17:21.000000 pyft-0.1.7/docs/index.rst
--rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.7/docs/make.bat
--rw-r--r--   0      501       20       46 2023-07-20 17:01:46.000000 pyft-0.1.7/docs/modules.rst
--rw-r--r--   0      501       20      141 2023-07-20 17:44:28.000000 pyft-0.1.7/docs/pyft.rst
--rw-r--r--   0      501       20      113 2023-07-23 14:43:25.000000 pyft-0.1.7/docs/requirements.txt
--rw-r--r--   0      501       20      651 2023-07-23 17:34:01.000000 pyft-0.1.7/example.py
--rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.7/pyproject.toml
--rw-r--r--   0      501       20    10263 2023-07-23 17:46:37.000000 pyft-0.1.7/src/fiberdata.rs
--rw-r--r--   0      501       20      700 2023-07-23 17:48:37.000000 pyft-0.1.7/src/lib.rs
--rw-r--r--   0      501       20    49806 2023-07-23 17:46:30.000000 pyft-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 pyft-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/bamlift/Cargo.toml
+-rw-r--r--   0      501       20    11043 2023-07-23 00:01:50.000000 pyft-0.1.8/local_dependencies/bamlift/src/lib.rs
+-rw-r--r--   0      501       20     1043 2023-07-22 20:22:41.000000 pyft-0.1.8/local_dependencies/bamlift/tests/test-liftover.rs
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.toml
+-rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.cargo/config
+-rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.dockerignore
+-rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/release.yml
+-rw-r--r--   0      501       20      211 2023-07-22 20:39:35.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.gitignore
+-rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.readthedocs.yaml
+-rw-------   0      501       20   122462 2023-07-21 08:31:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/CHANGELOG.md
+-rw-r--r--   0      501       20    63353 2023-07-22 22:51:02.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.lock
+-rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Dockerfile
+-rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.8/local_dependencies/fibertools-rs/INSTALL.md
+-rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/NOTES.md
+-rw-r--r--   0      501       20     4471 2023-07-21 07:53:23.000000 pyft-0.1.8/local_dependencies/fibertools-rs/README.md
+-rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/_config.yml
+-rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/center.png
+-rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
+-rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
+-rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/logo.png
+-rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.8/local_dependencies/fibertools-rs/build.rs
+-rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft--help.md
+-rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
+-rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-all-columns.md
+-rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-center-help.md
+-rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
+-rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-extract-help.md
+-rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
+-rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
+-rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/make_help_docs.sh
+-rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.8/local_dependencies/fibertools-rs/env.yaml
+-rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
+-rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_torch.pt
+-rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
+-rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_torch.pt
+-rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
+-rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
+-rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
+-rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
+-rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
+-rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
+-rw-r--r--   0      501       20    17495 2023-07-24 04:21:23.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/basemods/mod.rs
+-rw-r--r--   0      501       20    11897 2023-07-24 05:46:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/center.rs
+-rw-r--r--   0      501       20    10971 2023-07-22 19:51:25.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/cli.rs
+-rw-r--r--   0      501       20     3441 2023-07-24 05:11:49.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/extract.rs
+-rw-r--r--   0      501       20    19184 2023-07-24 05:42:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/fiber.rs
+-rw-r--r--   0      501       20     4182 2023-07-24 05:09:19.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/lib.rs
+-rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/main.rs
+-rw-r--r--   0      501       20    12930 2023-07-24 05:13:33.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/nucleosomes.rs
+-rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
+-rw-r--r--   0      501       20    18361 2023-07-21 00:03:41.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
+-rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
+-rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/strip_basemods.rs
+-rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam
+-rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam.bai
+-rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam
+-rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam.bai
+-rw-r--r--   0      501       20     3349 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bed
+-rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
+-rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/test.txt
+-rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/test.txt.gz
+-rw-r--r--   0      501       20     1776 2023-07-24 05:14:05.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/extract_test.rs
+-rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/run_test.rs
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/bio-io/Cargo.toml
+-rw-r--r--   0      501       20    10927 2023-07-21 23:45:13.000000 pyft-0.1.8/local_dependencies/bio-io/src/lib.rs
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pyft-0.1.8/Cargo.toml
+-rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.8/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.8/.gitignore
+-rw-r--r--   0      501       20      382 2023-07-23 16:19:13.000000 pyft-0.1.8/README.md
+-rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.8/docs/Makefile
+-rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.8/docs/_static/css/rtd_dark.css
+-rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.8/docs/_static/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.8/docs/_templates/layout.html
+-rw-r--r--   0      501       20     1699 2023-07-23 22:44:19.000000 pyft-0.1.8/docs/conf.py
+-rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.8/docs/environment.yml
+-rw-r--r--   0      501       20     1277 2023-07-23 16:17:21.000000 pyft-0.1.8/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.8/docs/make.bat
+-rw-r--r--   0      501       20      120 2023-07-24 03:07:50.000000 pyft-0.1.8/docs/requirements.txt
+-rw-r--r--   0      501       20      896 2023-07-24 05:50:12.000000 pyft-0.1.8/example.py
+-rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.8/pyproject.toml
+-rw-r--r--   0      501       20    11880 2023-07-24 05:50:35.000000 pyft-0.1.8/src/fiberdata.rs
+-rw-r--r--   0      501       20      700 2023-07-23 20:56:35.000000 pyft-0.1.8/src/lib.rs
+-rw-r--r--   0      501       20    49806 2023-07-24 05:50:16.000000 pyft-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 pyft-0.1.8/PKG-INFO
```

### Comparing `pyft-0.1.7/local_dependencies/bamlift/src/lib.rs` & `pyft-0.1.8/local_dependencies/bamlift/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/bamlift/tests/test-liftover.rs` & `pyft-0.1.8/local_dependencies/bamlift/tests/test-liftover.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/bio-io/Cargo.toml` & `pyft-0.1.8/local_dependencies/bio-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/bio-io/src/lib.rs` & `pyft-0.1.8/local_dependencies/bio-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/Cargo.toml` & `pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/.github/workflows/CI.yml` & `pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/.github/workflows/release.yml` & `pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/CHANGELOG.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/Cargo.lock` & `pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/Dockerfile` & `pyft-0.1.8/local_dependencies/fibertools-rs/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/INSTALL.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/README.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/README.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/center.png` & `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/center.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png` & `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png` & `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png` & `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/assets/img/logo.png` & `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/build.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/build.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft--help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft--help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-center-help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-center-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-extract-help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-extract-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/docs/make_help_docs.sh` & `pyft-0.1.8/local_dependencies/fibertools-rs/docs/make_help_docs.sh`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_semi_torch.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.0_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_semi_torch.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/2.2_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/3.2_semi_torch.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/Revio_semi_torch.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json` & `pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/basemods/mod.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/basemods/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     bam,
     bam::record::{Aux, AuxArray},
 };
 use std::collections::HashMap;
 
 use std::convert::TryFrom;
 
-#[derive(Eq, PartialEq, Debug, PartialOrd, Ord)]
+#[derive(Eq, PartialEq, Debug, PartialOrd, Ord, Clone)]
 pub struct BaseMod {
     pub modified_base: u8,
     pub strand: char,
     pub modification_type: char,
     record_is_reverse: bool,
     modified_bases: Vec<i64>,
     modified_bases_forward: Vec<i64>,
@@ -87,15 +87,15 @@
     }
 
     pub fn is_cpg(&self) -> bool {
         self.modification_type == 'm'
     }
 }
 
-#[derive(Eq, PartialEq, Debug)]
+#[derive(Eq, PartialEq, Debug, Clone)]
 pub struct BaseMods {
     pub base_mods: Vec<BaseMod>,
 }
 
 impl BaseMods {
     pub fn new(record: &bam::Record, min_ml_score: u8) -> BaseMods {
         // my basemod parser is ~25% faster than rust_htslib's
@@ -307,35 +307,14 @@
                 &m6a[1].get_reference_positions(),
             )
         } else {
             merge_two_lists(&m6a[0].get_modified_bases(), &m6a[1].get_modified_bases())
         }
     }
 
-    pub fn m6a_full_probabilities(&self, record: &bam::Record) -> Vec<(i64, f32)> {
-        let mp = get_f32_tag(record, b"mp");
-        let m6a: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_m6a()).collect();
-        // skip if no mp or m6a
-        if m6a.is_empty() || mp.is_empty() {
-            return vec![];
-        }
-        let m6a: Vec<i64> = m6a.iter().flat_map(|x| x.get_modified_bases()).collect();
-        // skip if not equal
-        if m6a.len() != mp.len() {
-            log::warn!(
-                "In {} m6A mods ({}) not equal to number of predictions ({}), returning nothing for this read.",
-                String::from_utf8_lossy(record.qname()),
-                m6a.len(),
-                mp.len()
-            );
-            return vec![];
-        }
-        m6a.into_iter().zip(mp.into_iter()).collect()
-    }
-
     fn helper_get_m6a(&self, forward: bool) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
         let m6a: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_m6a()).collect();
         // skip if no m6a
         if m6a.is_empty() {
             return (vec![], vec![], vec![]);
         }
```

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/center.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/center.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-use super::extract::*;
+use super::fiber::FiberseqData;
 use super::*;
 use bamlift::*;
 use bio::alphabets::dna::revcomp;
 use bio_io;
 use indicatif::{style, ProgressBar};
 use rayon::prelude::*;
 use rust_htslib::bam::Read;
 use rust_htslib::{bam, bam::ext::BamRecordExtensions};
 use std::fmt::Write;
 use std::io::{self, prelude::*};
 
-#[derive(Clone)]
+#[derive(Clone, Debug, PartialEq, Eq)]
 pub struct CenterPosition {
     pub chrom: String,
     pub position: i64,
     pub strand: char,
 }
 pub struct CenteredFiberData {
     fiber: FiberseqData,
-    rg: String,
-    offset: i64,
     pub dist: Option<i64>,
     center_position: CenterPosition,
+    pub offset: i64,
     pub reference: bool,
 }
 
 impl CenteredFiberData {
     pub fn new(
         fiber: FiberseqData,
         center_position: CenterPosition,
         dist: Option<i64>,
         reference: bool,
     ) -> Option<Self> {
-        let offset = if reference {
-            Some(center_position.position)
-        } else {
-            CenteredFiberData::find_offset(&fiber.record, center_position.position)
-        };
-        // get RG
-        let rg = if let Ok(bam::record::Aux::String(f)) = fiber.record.aux(b"RG") {
-            f
-        } else {
-            "."
-        }
-        .to_string();
+        let (ref_offset, mol_offset) =
+            CenteredFiberData::find_offsets(&fiber.record, &center_position);
+        let offset = if reference { ref_offset } else { mol_offset };
+
+        let fiber = fiber.center(&center_position)?;
 
-        offset.map(|offset| CenteredFiberData {
+        Some(CenteredFiberData {
             fiber,
-            rg,
-            offset,
             dist,
             center_position,
+            offset,
             reference,
         })
     }
-
-    pub fn get_centering_position(&self) -> i64 {
-        self.center_position.position
+    /// find both the ref and mol offsets
+    pub fn find_offsets(record: &bam::Record, center_position: &CenterPosition) -> (i64, i64) {
+        let ref_offset = center_position.position;
+        let mol_offset =
+            CenteredFiberData::find_offset(record, center_position.position).unwrap_or(0);
+        (ref_offset, mol_offset)
     }
 
     /// find the query position that corresponds to the central reference position
-    fn find_offset(record: &bam::Record, reference_position: i64) -> Option<i64> {
+    pub fn find_offset(record: &bam::Record, reference_position: i64) -> Option<i64> {
         let read_center: Vec<i64> = lift_query_positions_exact(record, &[reference_position])
             .into_iter()
             .filter(|&x| x >= 0)
             .collect();
         log::debug!(
             "{}, {}, {}, {:?}",
             reference_position,
@@ -75,24 +69,14 @@
         if read_center.is_empty() {
             None
         } else {
             Some(read_center[0])
         }
     }
 
-    /// Center positions on the read around the reference position.
-    fn apply_offset(&self, positions: &[i64]) -> Vec<i64> {
-        let out = positions.iter().map(|&p| p - self.offset).collect();
-        if self.center_position.strand == '+' {
-            out
-        } else {
-            out.iter().rev().map(|&p| -p).collect()
-        }
-    }
-
     /// Get the sequence
     pub fn subset_sequence(&self) -> String {
         let dist = if let Some(dist) = self.dist { dist } else { 0 };
         let seq = self.fiber.record.seq().as_bytes();
 
         let mut out_seq: Vec<u8> = vec![];
         let st = self.offset - dist; //(self.offset - dist)
@@ -107,62 +91,51 @@
             out_seq = revcomp(out_seq);
         }
         //assert_eq!(out_seq.len() as i64, dist * 2 + 1);
         String::from_utf8_lossy(&out_seq).to_string()
     }
 
     pub fn m6a_positions(&self) -> Vec<i64> {
-        self.apply_offset(&self.fiber.base_mods.m6a_positions(self.reference))
+        self.fiber.m6a_positions(self.reference).to_vec()
     }
 
     pub fn cpg_positions(&self) -> Vec<i64> {
-        self.apply_offset(&self.fiber.base_mods.cpg_positions(self.reference))
-    }
-
-    fn get_start_end_positions(&self, starts: &[i64], ends: &[i64]) -> Vec<(i64, i64)> {
-        let starts = self.apply_offset(starts);
-        let ends = self.apply_offset(ends);
-        starts
-            .into_iter()
-            .zip(ends)
-            .map(|(s, e)| {
-                if e - s > 300 || s - e > 300 {
-                    log::trace!("{}, {}, {}", s, e, e - s);
-                }
-                if s < e {
-                    (s, e)
-                } else {
-                    (e, s)
-                }
-            })
-            .collect()
+        self.fiber.cpg_positions(self.reference).to_vec()
     }
 
     pub fn nuc_positions(&self) -> Vec<(i64, i64)> {
         let (starts, ends) = if self.reference {
             (
                 &self.fiber.nuc.reference_starts,
                 &self.fiber.nuc.reference_ends,
             )
         } else {
             (&self.fiber.nuc.starts, &self.fiber.nuc.ends)
         };
-        self.get_start_end_positions(starts, ends)
+        starts
+            .clone()
+            .into_iter()
+            .zip(ends.clone().into_iter())
+            .collect()
     }
 
     pub fn msp_positions(&self) -> Vec<(i64, i64)> {
         let (starts, ends) = if self.reference {
             (
                 &self.fiber.msp.reference_starts,
                 &self.fiber.msp.reference_ends,
             )
         } else {
             (&self.fiber.msp.starts, &self.fiber.msp.ends)
         };
-        self.get_start_end_positions(starts, ends)
+        starts
+            .clone()
+            .into_iter()
+            .zip(ends.clone().into_iter())
+            .collect()
     }
 
     pub fn get_sequence(&self) -> String {
         let forward_bases = if self.center_position.strand == '+' {
             self.fiber.record.seq().as_bytes()
         } else {
             revcomp(self.fiber.record.seq().as_bytes())
@@ -176,15 +149,15 @@
             self.center_position.chrom,
             self.center_position.position,
             self.center_position.strand,
             self.subset_sequence(),
             self.fiber.record.reference_start(),
             self.fiber.record.reference_end(),
             std::str::from_utf8(self.fiber.record.qname()).unwrap(),
-            self.rg,
+            self.fiber.rg,
             -self.offset,
             self.fiber.record.seq_len() as i64 - self.offset,
             self.fiber.record.seq_len()
         )
     }
 
     pub fn write(&self) -> String {
```

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/cli.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/cli.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/lib.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+/// Data structure for fiberseq data
+pub mod fiber;
+
 /// Add and remove base modifications from a bam record
 pub mod basemods;
 /// Center fiberseq information around a reference position
 pub mod center;
 #[cfg(feature = "cli")]
 /// Command line interface for fibertools-rs.
 pub mod cli;
```

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/main.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/nucleosomes.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/nucleosomes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use super::fiber::FiberseqData;
 use super::*;
 use indicatif::{style, ParallelProgressIterator};
 use rayon::current_num_threads;
 use rayon::iter::ParallelIterator;
 use rayon::prelude::IntoParallelRefMutIterator;
 use rust_htslib::{
     bam,
@@ -314,15 +315,15 @@
             .progress_chars("##-");
 
         // add nuc calls
         let records: Vec<&mut Record> = chunk
             .par_iter_mut()
             .progress_with_style(style)
             .map(|record| {
-                let fd = extract::FiberseqData::new(record.clone(), None, 0);
+                let fd = FiberseqData::new(record.clone(), None, 0);
                 let m6a = fd.base_mods.forward_m6a();
                 add_nucleosomes_to_record(record, &m6a.0, &options);
                 record
             })
             .collect();
 
         records
```

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/src/strip_basemods.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/src/strip_basemods.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/all.bam` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/all.bam.bai` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bam` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bam.bai` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/center.bed` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bed`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/extract_test.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/extract_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use rust_htslib::bam::Read;
 
-fn get_fiber_data_from_test_bam(bam_file: &str) -> Vec<fibertools_rs::extract::FiberseqData> {
+fn get_fiber_data_from_test_bam(bam_file: &str) -> Vec<fibertools_rs::fiber::FiberseqData> {
     let mut bam = bio_io::bam_reader(bam_file, 1);
     bam.records()
         .map(|r| {
             let record = r.unwrap();
-            let fiber_data = fibertools_rs::extract::FiberseqData::new(record, None, 0);
+            let fiber_data = fibertools_rs::fiber::FiberseqData::new(record, None, 0);
             fiber_data
         })
         .collect::<Vec<_>>()
 }
 
 #[test]
 fn test_msp_extract() -> Result<(), Box<dyn std::error::Error>> {
```

### Comparing `pyft-0.1.7/local_dependencies/fibertools-rs/tests/run_test.rs` & `pyft-0.1.8/local_dependencies/fibertools-rs/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/Cargo.toml` & `pyft-0.1.8/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "pyft"
-version = "0.1.7"
+version = "0.1.8"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "pyft"
 
 [dependencies]
```

### Comparing `pyft-0.1.7/.github/workflows/CI.yml` & `pyft-0.1.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/.gitignore` & `pyft-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/docs/Makefile` & `pyft-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/docs/_static/css/rtd_dark.css` & `pyft-0.1.8/docs/_static/css/rtd_dark.css`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/docs/_static/img/fiber_tools_grey.png` & `pyft-0.1.8/docs/_static/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/docs/conf.py` & `pyft-0.1.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
-    "sphinx_autodoc_typehints",
+    #"sphinx_autodoc_typehints",
     "sphinx.ext.viewcode",
     #"sphinx.ext.napoleon",
     "sphinx_rtd_theme",
     "sphinx.ext.intersphinx",
     #"edit_on_github",
     "m2r2",
 ]
@@ -45,16 +45,16 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 #html_theme = "alabaster"
 html_theme = "sphinx_rtd_theme"
 #html_permalinks_icon = '<span>#</span>'
 #html_theme = 'sphinxawesome_theme'
 html_static_path = ["_static"]
-html_css_files = [
-    "css/rtd_dark.css",
-]
+#html_css_files = [
+    #"css/rtd_dark.css",
+#]
 html_logo = "_static/img/fiber_tools_grey.png"
 
 
 # other options
 autodoc_member_order = 'bysource'
```

### Comparing `pyft-0.1.7/docs/index.rst` & `pyft-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/docs/make.bat` & `pyft-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/src/fiberdata.rs` & `pyft-0.1.8/src/fiberdata.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-use fibertools_rs::extract::FiberseqData;
+use fibertools_rs::fiber::FiberseqData;
 use pyo3::iter::IterNextOutput;
 use pyo3::prelude::*;
 use rust_htslib::{bam, bam::ext::BamRecordExtensions, bam::record::Aux, bam::Read};
 use std::time;
 use std::vec::IntoIter;
 
 #[pyclass]
-/// Record class for fiberseq data, corresponding to a single bam record
+/// Class for fiberseq data. This class corresponds to a single record in the bam file.
 pub struct Fiberdata {
     /// Number of ccs passes
     #[pyo3(get, set)]
     pub ec: i64,
     /// Name of the read
     #[pyo3(get, set)]
     pub qname: String,
@@ -52,14 +52,17 @@
     pub msp: Ranges,
     /// :class:`~pyft.Ranges` object for nuc features
     #[pyo3(get, set)]
     pub nuc: Ranges,
     /// Aligned block pairs from the bam record
     #[pyo3(get)]
     pub aligned_block_pairs: Vec<([i64; 2], [i64; 2])>,
+    /// offset for centering the fiber
+    #[pyo3(get, set)]
+    offset: Option<i64>,
 }
 #[pymethods]
 impl Fiberdata {
     pub fn __str__(&self) -> String {
         format!(
             "fiber: {}\t\
             chrom: {}\tstart: {}\tend {}\t\
@@ -99,97 +102,132 @@
         let lengths = fiber.iter().map(|x| x[1] - x[0]).collect();
         let reference_starts = genome.iter().map(|x| x[0]).collect();
         let reference_lengths = genome.iter().map(|x| x[1] - x[0]).collect();
         Ranges::new(starts, lengths, reference_starts, reference_lengths)
     }
 }
 
-fn new_py_fiberdata(fiber: FiberseqData) -> Fiberdata {
-    // PB features
-    let ec = fiber.ec.round() as i64;
-
-    // record features
-    let qname = std::str::from_utf8(fiber.record.qname()).unwrap();
-    let sam_flag = fiber.record.flags();
-    let rq = match fiber.get_rq() {
-        Some(x) => format!("{}", x),
-        None => ".".to_string(),
-    };
-    let hp = fiber.get_hp();
-    let seq = String::from_utf8_lossy(&fiber.record.seq().as_bytes()).to_string();
-    let (chrom, start, end, strand): (&str, i64, i64, char) = if fiber.record.is_unmapped() {
-        (".", 0, 0, '.')
-    } else {
-        let strand = if fiber.record.is_reverse() { '-' } else { '+' };
-        (
-            &fiber.target_name,
-            fiber.record.reference_start(),
-            fiber.record.reference_end(),
+impl Fiberdata {
+    fn new(fiber: FiberseqData, offset: Option<i64>) -> Self {
+        // PB features
+        let ec = fiber.ec.round() as i64;
+
+        // record features
+        let qname = std::str::from_utf8(fiber.record.qname()).unwrap();
+        let sam_flag = fiber.record.flags();
+        let rq = match fiber.get_rq() {
+            Some(x) => format!("{}", x),
+            None => ".".to_string(),
+        };
+        let hp = fiber.get_hp();
+        let seq = String::from_utf8_lossy(&fiber.record.seq().as_bytes()).to_string();
+        let (chrom, start, end, strand): (&str, i64, i64, char) = if fiber.record.is_unmapped() {
+            (".", 0, 0, '.')
+        } else {
+            let strand = if fiber.record.is_reverse() { '-' } else { '+' };
+            (
+                &fiber.target_name,
+                fiber.record.reference_start(),
+                fiber.record.reference_end(),
+                strand,
+            )
+        };
+        let rg = if let Ok(Aux::String(f)) = fiber.record.aux(b"RG") {
+            log::trace!("{f}");
+            f
+        } else {
+            "."
+        };
+
+        // fiberseq features
+        let m6a = fiber.base_mods.m6a();
+        let m6a = Basemods::new(m6a.0, m6a.1, m6a.2);
+        let cpg = fiber.base_mods.cpg();
+        let cpg = Basemods::new(cpg.0, cpg.1, cpg.2);
+
+        let nuc = Ranges {
+            starts: fiber.nuc.starts,
+            ends: fiber.nuc.ends,
+            lengths: fiber.nuc.lengths,
+            reference_starts: fiber.nuc.reference_starts,
+            reference_ends: fiber.nuc.reference_ends,
+            reference_lengths: fiber.nuc.reference_lengths,
+        };
+        let msp = Ranges {
+            starts: fiber.msp.starts,
+            ends: fiber.msp.ends,
+            lengths: fiber.msp.lengths,
+            reference_starts: fiber.msp.reference_starts,
+            reference_ends: fiber.msp.reference_ends,
+            reference_lengths: fiber.msp.reference_lengths,
+        };
+
+        let aligned_block_pairs = fiber.record.aligned_block_pairs().collect();
+        Self {
+            ec,
+            qname: qname.to_string(),
+            sam_flag,
+            rq,
+            hp,
+            seq,
+            chrom: chrom.to_string(),
+            start,
+            end,
             strand,
-        )
-    };
-    let rg = if let Ok(Aux::String(f)) = fiber.record.aux(b"RG") {
-        log::trace!("{f}");
-        f
-    } else {
-        "."
-    };
-
-    // fiberseq features
-    let m6a = fiber.base_mods.m6a();
-    let m6a = Basemods::new(m6a.0, m6a.1, m6a.2);
-    let cpg = fiber.base_mods.cpg();
-    let cpg = Basemods::new(cpg.0, cpg.1, cpg.2);
-
-    let nuc = Ranges {
-        starts: fiber.nuc.starts,
-        ends: fiber.nuc.ends,
-        lengths: fiber.nuc.lengths,
-        reference_starts: fiber.nuc.reference_starts,
-        reference_ends: fiber.nuc.reference_ends,
-        reference_lengths: fiber.nuc.reference_lengths,
-    };
-    let msp = Ranges {
-        starts: fiber.msp.starts,
-        ends: fiber.msp.ends,
-        lengths: fiber.msp.lengths,
-        reference_starts: fiber.msp.reference_starts,
-        reference_ends: fiber.msp.reference_ends,
-        reference_lengths: fiber.msp.reference_lengths,
-    };
-
-    let aligned_block_pairs = fiber.record.aligned_block_pairs().collect();
-    Fiberdata {
-        ec,
-        qname: qname.to_string(),
-        sam_flag,
-        rq,
-        hp,
-        seq,
-        chrom: chrom.to_string(),
-        start,
-        end,
-        strand,
-        rg: rg.to_string(),
-        m6a,
-        cpg,
-        msp,
-        nuc,
-        aligned_block_pairs,
+            rg: rg.to_string(),
+            m6a,
+            cpg,
+            msp,
+            nuc,
+            aligned_block_pairs,
+            offset,
+        }
     }
 }
 
 #[pyclass]
 /// Open a fiberseq bam file. Must have an index.
 pub struct Fiberbam {
     bam: bam::IndexedReader,
     header: bam::Header,
     start: time::Instant,
 }
 
+/// pure rust functions for Fiberbam
+impl Fiberbam {
+    fn _fetch_helper(
+        &mut self,
+        chrom: &str,
+        start: Option<i64>,
+        end: Option<i64>,
+    ) -> Vec<FiberseqData> {
+        let fetch_args = match (start, end) {
+            (Some(start), Some(end)) => bam::FetchDefinition::from((chrom, start, end)),
+            _ => bam::FetchDefinition::from(chrom),
+        };
+
+        let head_view = bam::HeaderView::from_header(&self.header);
+        self.bam.fetch(fetch_args).expect("unable to fetch region");
+        let records: Vec<bam::Record> = self.bam.records().map(|r| r.unwrap()).collect();
+
+        log::info!(
+            "{} records fetched in {:.2}s",
+            records.len(),
+            self._time_from_last()
+        );
+        let fiberdata = FiberseqData::from_records(records, &head_view, 0);
+        log::info!(
+            "Fiberdata made for {} records in {:.2}s",
+            fiberdata.len(),
+            self._time_from_last()
+        );
+        fiberdata
+    }
+}
+
 #[pymethods]
 impl Fiberbam {
     #[new]
     #[pyo3(signature = (bam_file, threads = 8))]
     fn new(bam_file: &str, threads: usize) -> Self {
         let mut bam =
             bam::IndexedReader::from_path(bam_file).expect("unable to open indexed bam file");
@@ -207,65 +245,65 @@
     ///     fiberdata.fetch("chr1", start=100, end=200)
     ///
     ///     fiberdata.fetch("chr1:100-200")
     ///
     ///     fiberdata.fetch("chr1")
     #[pyo3(signature = (chrom, start = None, end=None))]
     pub fn fetch(&mut self, chrom: &str, start: Option<i64>, end: Option<i64>) -> Fiberiter {
-        let fetch_args = if start.is_none() || end.is_none() {
-            bam::FetchDefinition::from(chrom)
-        } else {
-            bam::FetchDefinition::from((chrom, start.unwrap(), end.unwrap()))
-        };
-        let head_view = bam::HeaderView::from_header(&self.header);
-        self.bam.fetch(fetch_args).expect("unable to fetch region");
-        let records: Vec<bam::Record> = self.bam.records().map(|r| r.unwrap()).collect();
+        Fiberiter::build_fiberdata_iter(self._fetch_helper(chrom, start, end))
+    }
 
-        log::info!(
-            "{} records fetched in {:.2}s",
-            records.len(),
-            self._time_from_last()
-        );
-        let fiberdata = FiberseqData::from_records(records, &head_view, 0);
-        log::info!(
-            "Fiberdata made for {} records in {:.2}s",
-            fiberdata.len(),
-            self._time_from_last()
-        );
-        build_fiberdata_iter(fiberdata)
+    /// Returns an iterator over :class:`~pyft.Fiberdata` objects; however, the data is centered around the region that has been fetched (`should` work the same as **ft center**).
+    #[pyo3(signature = (chrom, start, end, strand = '+'))]
+    pub fn center(&mut self, chrom: &str, start: i64, end: i64, strand: char) -> Fiberiter {
+        let position = if strand == '-' { end - 1 } else { start };
+        let center_position = fibertools_rs::center::CenterPosition {
+            chrom: chrom.to_string(),
+            position,
+            strand,
+        };
+        let fiberdata = self._fetch_helper(chrom, Some(position), Some(position + 1));
+        let fibderdata: Vec<FiberseqData> = fiberdata
+            .into_iter()
+            .filter_map(|fiber| fiber.center(&center_position))
+            .collect();
+        Fiberiter::build_fiberdata_iter(fibderdata)
     }
 
     fn _time_from_last(&mut self) -> f64 {
         let elapsed = self.start.elapsed().as_secs_f64();
         self.start = time::Instant::now();
         elapsed
     }
 }
 
-fn build_fiberdata_iter(fiberdata: Vec<FiberseqData>) -> Fiberiter {
-    let length = fiberdata.len();
-    Fiberiter {
-        fiberdata: fiberdata.into_iter(),
-        length,
-    }
-}
-
 #[pyclass]
 /// An iterator over :class:`~pyft.Fiberdata` objects.
 pub struct Fiberiter {
     fiberdata: IntoIter<FiberseqData>,
     length: usize,
 }
 
+/// rust only functions for Fiberiter
+impl Fiberiter {
+    fn build_fiberdata_iter(fiberdata: Vec<FiberseqData>) -> Self {
+        let length = fiberdata.len();
+        Self {
+            fiberdata: fiberdata.into_iter(),
+            length,
+        }
+    }
+}
+
 #[pymethods]
 impl Fiberiter {
     fn __next__(&mut self) -> IterNextOutput<Fiberdata, &'static str> {
         let data = self.fiberdata.next();
         match data {
-            Some(fiber) => IterNextOutput::Yield(new_py_fiberdata(fiber)),
+            Some(fiber) => IterNextOutput::Yield(Fiberdata::new(fiber, None)),
             None => IterNextOutput::Return("Ended"),
         }
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
```

### Comparing `pyft-0.1.7/src/lib.rs` & `pyft-0.1.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.7/Cargo.lock` & `pyft-0.1.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1198,15 +1198,15 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyft"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "anyhow",
  "bamlift",
  "bio-io",
  "colored",
  "env_logger 0.10.0",
  "fibertools-rs",
```

### Comparing `pyft-0.1.7/PKG-INFO` & `pyft-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyft
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # pyft: python bindings for fibertools-rs
```

