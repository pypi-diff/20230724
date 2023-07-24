# Comparing `tmp/pyft-0.1.8.tar.gz` & `tmp/pyft-0.1.9.tar.gz`

## Comparing `pyft-0.1.8.tar` & `pyft-0.1.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/bamlift/Cargo.toml
--rw-r--r--   0      501       20    11043 2023-07-23 00:01:50.000000 pyft-0.1.8/local_dependencies/bamlift/src/lib.rs
--rw-r--r--   0      501       20     1043 2023-07-22 20:22:41.000000 pyft-0.1.8/local_dependencies/bamlift/tests/test-liftover.rs
--rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.toml
--rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.cargo/config
--rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.dockerignore
--rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/CI.yml
--rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/release.yml
--rw-r--r--   0      501       20      211 2023-07-22 20:39:35.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.gitignore
--rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.pre-commit-config.yaml
--rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.8/local_dependencies/fibertools-rs/.readthedocs.yaml
--rw-------   0      501       20   122462 2023-07-21 08:31:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/CHANGELOG.md
--rw-r--r--   0      501       20    63353 2023-07-22 22:51:02.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.lock
--rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.8/local_dependencies/fibertools-rs/Dockerfile
--rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.8/local_dependencies/fibertools-rs/INSTALL.md
--rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/NOTES.md
--rw-r--r--   0      501       20     4471 2023-07-21 07:53:23.000000 pyft-0.1.8/local_dependencies/fibertools-rs/README.md
--rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/_config.yml
--rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/center.png
--rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
--rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
--rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
--rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/logo.png
--rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.8/local_dependencies/fibertools-rs/build.rs
--rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft--help.md
--rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
--rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-all-columns.md
--rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-center-help.md
--rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
--rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-extract-help.md
--rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
--rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
--rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/docs/make_help_docs.sh
--rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.8/local_dependencies/fibertools-rs/env.yaml
--rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
--rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_torch.pt
--rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
--rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
--rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_torch.pt
--rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
--rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
--rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
--rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
--rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
--rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
--rw-r--r--   0      501       20    17495 2023-07-24 04:21:23.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/basemods/mod.rs
--rw-r--r--   0      501       20    11897 2023-07-24 05:46:36.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/center.rs
--rw-r--r--   0      501       20    10971 2023-07-22 19:51:25.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/cli.rs
--rw-r--r--   0      501       20     3441 2023-07-24 05:11:49.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/extract.rs
--rw-r--r--   0      501       20    19184 2023-07-24 05:42:15.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/fiber.rs
--rw-r--r--   0      501       20     4182 2023-07-24 05:09:19.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/lib.rs
--rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/main.rs
--rw-r--r--   0      501       20    12930 2023-07-24 05:13:33.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/nucleosomes.rs
--rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
--rw-r--r--   0      501       20    18361 2023-07-21 00:03:41.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
--rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
--rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.8/local_dependencies/fibertools-rs/src/strip_basemods.rs
--rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam
--rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam.bai
--rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam
--rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam.bai
--rw-r--r--   0      501       20     3349 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bed
--rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
--rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/test.txt
--rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/test.txt.gz
--rw-r--r--   0      501       20     1776 2023-07-24 05:14:05.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/extract_test.rs
--rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.8/local_dependencies/fibertools-rs/tests/run_test.rs
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.8/local_dependencies/bio-io/Cargo.toml
--rw-r--r--   0      501       20    10927 2023-07-21 23:45:13.000000 pyft-0.1.8/local_dependencies/bio-io/src/lib.rs
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pyft-0.1.8/Cargo.toml
--rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.8/.github/workflows/CI.yml
--rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.8/.gitignore
--rw-r--r--   0      501       20      382 2023-07-23 16:19:13.000000 pyft-0.1.8/README.md
--rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.8/docs/Makefile
--rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.8/docs/_static/css/rtd_dark.css
--rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.8/docs/_static/img/fiber_tools_grey.png
--rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.8/docs/_templates/layout.html
--rw-r--r--   0      501       20     1699 2023-07-23 22:44:19.000000 pyft-0.1.8/docs/conf.py
--rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.8/docs/environment.yml
--rw-r--r--   0      501       20     1277 2023-07-23 16:17:21.000000 pyft-0.1.8/docs/index.rst
--rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.8/docs/make.bat
--rw-r--r--   0      501       20      120 2023-07-24 03:07:50.000000 pyft-0.1.8/docs/requirements.txt
--rw-r--r--   0      501       20      896 2023-07-24 05:50:12.000000 pyft-0.1.8/example.py
--rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.8/pyproject.toml
--rw-r--r--   0      501       20    11880 2023-07-24 05:50:35.000000 pyft-0.1.8/src/fiberdata.rs
--rw-r--r--   0      501       20      700 2023-07-23 20:56:35.000000 pyft-0.1.8/src/lib.rs
--rw-r--r--   0      501       20    49806 2023-07-24 05:50:16.000000 pyft-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 pyft-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pyft-0.1.9/local_dependencies/fibertools-rs/Cargo.toml
+-rw-r--r--   0      501       20      231 2022-10-14 01:13:49.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.cargo/config
+-rw-r--r--   0      501       20      210 2023-06-29 17:34:56.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.dockerignore
+-rw-r--r--   0      501       20      467 2022-08-31 04:23:38.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20     1366 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     5839 2023-02-01 23:24:35.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.github/workflows/release.yml
+-rw-r--r--   0      501       20      211 2023-07-22 20:39:35.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.gitignore
+-rw-r--r--   0      501       20      475 2023-07-19 02:39:46.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      383 2023-07-20 16:48:33.000000 pyft-0.1.9/local_dependencies/fibertools-rs/.readthedocs.yaml
+-rw-------   0      501       20   127941 2023-07-24 16:55:29.000000 pyft-0.1.9/local_dependencies/fibertools-rs/CHANGELOG.md
+-rw-r--r--   0      501       20    63353 2023-07-22 22:51:02.000000 pyft-0.1.9/local_dependencies/fibertools-rs/Cargo.lock
+-rw-r--r--   0      501       20     1216 2023-07-03 16:43:59.000000 pyft-0.1.9/local_dependencies/fibertools-rs/Dockerfile
+-rw-r--r--   0      501       20     1486 2023-06-14 05:56:02.000000 pyft-0.1.9/local_dependencies/fibertools-rs/INSTALL.md
+-rw-r--r--   0      501       20      146 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/NOTES.md
+-rw-r--r--   0      501       20     4714 2023-07-24 15:33:17.000000 pyft-0.1.9/local_dependencies/fibertools-rs/README.md
+-rw-r--r--   0      501       20      297 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/_config.yml
+-rw-r--r--   0      501       20   670134 2022-12-09 17:50:21.000000 pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/center.png
+-rw-r--r--   0      501       20   160734 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20   159267 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png
+-rw-r--r--   0      501       20   220557 2022-12-09 17:50:21.000000 pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png
+-rw-r--r--   0      501       20   303252 2022-12-09 17:50:21.000000 pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/logo.png
+-rw-r--r--   0      501       20      761 2023-05-08 02:36:47.000000 pyft-0.1.9/local_dependencies/fibertools-rs/build.rs
+-rw-r--r--   0      501       20     1181 2023-07-19 02:49:54.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft--help.md
+-rw-r--r--   0      501       20     1035 2023-07-19 02:50:05.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md
+-rw-r--r--   0      501       20      323 2023-07-19 02:50:14.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-all-columns.md
+-rw-r--r--   0      501       20     1697 2023-07-19 02:50:00.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-center-help.md
+-rw-r--r--   0      501       20      488 2023-07-19 02:50:08.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-clear-kinetics-help.md
+-rw-r--r--   0      501       20     1436 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-extract-help.md
+-rw-r--r--   0      501       20     2234 2023-07-19 02:50:03.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md
+-rw-r--r--   0      501       20      627 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md
+-rwxr-xr-x   0      501       20      675 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/docs/make_help_docs.sh
+-rw-r--r--   0      501       20      294 2023-06-18 22:24:56.000000 pyft-0.1.9/local_dependencies/fibertools-rs/env.yaml
+-rw-r--r--   0      501       20     5008 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_semi_torch.json
+-rw-r--r--   0      501       20    26890 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-10-20 20:35:37.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_torch.pt
+-rw-r--r--   0      501       20     8502 2023-02-27 20:16:15.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_semi_torch.json
+-rw-r--r--   0      501       20    27030 2023-01-13 07:54:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt
+-rw-r--r--   0      501       20    26136 2022-12-20 16:24:36.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_torch.pt
+-rw-r--r--   0      501       20    15472 2023-04-25 19:19:04.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/3.2_semi_torch.json
+-rw-r--r--   0      501       20    26130 2023-03-14 17:30:11.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt
+-rw-r--r--   0      501       20     4491 2023-05-02 16:35:59.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/Revio_semi_torch.json
+-rw-r--r--   0      501       20    32320 2023-05-02 16:35:43.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt
+-rw-r--r--   0      501       20  2589234 2022-11-17 21:59:57.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json
+-rw-r--r--   0      501       20  2579653 2022-11-17 21:59:57.000000 pyft-0.1.9/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json
+-rw-r--r--   0      501       20    15592 2023-07-24 19:04:54.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/basemods/mod.rs
+-rw-r--r--   0      501       20    12338 2023-07-24 19:03:39.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/center.rs
+-rw-r--r--   0      501       20    10971 2023-07-22 19:51:25.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/cli.rs
+-rw-r--r--   0      501       20     3441 2023-07-24 17:14:31.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/extract.rs
+-rw-r--r--   0      501       20    18472 2023-07-24 19:08:10.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/fiber.rs
+-rw-r--r--   0      501       20     4475 2023-07-24 19:07:27.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/lib.rs
+-rw-r--r--   0      501       20     9233 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/main.rs
+-rw-r--r--   0      501       20    12930 2023-07-24 05:13:33.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/nucleosomes.rs
+-rw-r--r--   0      501       20     3476 2023-06-18 04:21:08.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs
+-rw-r--r--   0      501       20    18361 2023-07-21 00:03:41.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs
+-rw-r--r--   0      501       20     1684 2023-03-10 15:54:29.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs
+-rw-r--r--   0      501       20     1588 2023-06-29 17:25:52.000000 pyft-0.1.9/local_dependencies/fibertools-rs/src/strip_basemods.rs
+-rw-r--r--   0      501       20  1529300 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/all.bam
+-rw-r--r--   0      501       20     1792 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/all.bam.bai
+-rw-r--r--   0      501       20  4202969 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bam
+-rw-r--r--   0      501       20   758264 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bam.bai
+-rw-r--r--   0      501       20     3315 2023-07-24 14:59:44.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bed
+-rw-r--r--   0      501       20    17525 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam
+-rw-r--r--   0      501       20       13 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/test.txt
+-rw-r--r--   0      501       20       72 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/test.txt.gz
+-rw-r--r--   0      501       20     1892 2023-07-24 19:11:50.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/extract_test.rs
+-rw-r--r--   0      501       20     2216 2023-07-19 18:23:20.000000 pyft-0.1.9/local_dependencies/fibertools-rs/tests/run_test.rs
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 pyft-0.1.9/local_dependencies/bio-io/Cargo.toml
+-rw-r--r--   0      501       20    10927 2023-07-21 23:45:13.000000 pyft-0.1.9/local_dependencies/bio-io/src/lib.rs
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 pyft-0.1.9/local_dependencies/bamlift/Cargo.toml
+-rw-r--r--   0      501       20    11508 2023-07-24 19:24:06.000000 pyft-0.1.9/local_dependencies/bamlift/src/lib.rs
+-rw-r--r--   0      501       20     1112 2023-07-24 19:13:10.000000 pyft-0.1.9/local_dependencies/bamlift/tests/test-liftover.rs
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 pyft-0.1.9/Cargo.toml
+-rw-r--r--   0      501       20     2807 2023-07-19 21:04:05.000000 pyft-0.1.9/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      692 2023-07-19 21:52:50.000000 pyft-0.1.9/.gitignore
+-rw-r--r--   0      501       20      382 2023-07-23 16:19:13.000000 pyft-0.1.9/README.md
+-rw-r--r--   0      501       20      634 2023-07-20 03:00:42.000000 pyft-0.1.9/docs/Makefile
+-rw-r--r--   0      501       20     2216 2023-07-20 18:11:44.000000 pyft-0.1.9/docs/_static/css/rtd_dark.css
+-rw-r--r--   0      501       20   160734 2023-07-20 16:45:23.000000 pyft-0.1.9/docs/_static/img/fiber_tools_grey.png
+-rw-r--r--   0      501       20      294 2023-07-20 17:07:50.000000 pyft-0.1.9/docs/_templates/layout.html
+-rw-r--r--   0      501       20     1706 2023-07-24 16:39:12.000000 pyft-0.1.9/docs/conf.py
+-rw-r--r--   0      501       20       76 2023-07-20 18:49:05.000000 pyft-0.1.9/docs/environment.yml
+-rw-r--r--   0      501       20     1277 2023-07-23 16:17:21.000000 pyft-0.1.9/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-07-20 03:00:42.000000 pyft-0.1.9/docs/make.bat
+-rw-r--r--   0      501       20      120 2023-07-24 03:07:50.000000 pyft-0.1.9/docs/requirements.txt
+-rw-r--r--   0      501       20      806 2023-07-24 19:52:20.000000 pyft-0.1.9/example.py
+-rw-r--r--   0      501       20      357 2023-07-20 17:34:33.000000 pyft-0.1.9/pyproject.toml
+-rw-r--r--   0      501       20    11726 2023-07-24 19:53:14.000000 pyft-0.1.9/src/fiberdata.rs
+-rw-r--r--   0      501       20      700 2023-07-23 20:56:35.000000 pyft-0.1.9/src/lib.rs
+-rw-r--r--   0      501       20    49806 2023-07-24 19:52:53.000000 pyft-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 pyft-0.1.9/PKG-INFO
```

### Comparing `pyft-0.1.8/local_dependencies/bamlift/src/lib.rs` & `pyft-0.1.9/local_dependencies/bamlift/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -146,27 +146,31 @@
             a_idx += 1;
         }
     }
     log::trace!("search_sorted: {:?}\n{:?}", v, indexes);
     indexes
 }
 
+//
+// CLOSEST LIFTOVER FUNCTIONS
+//
+
 /// this is a helper function for liftover_closest that should only be called from there
 /// The exception for this is test cases, where it should be easier to test this function
 /// directly.
 fn liftover_closest(
     positions: &[i64],
     aligned_block_pairs: &Vec<([i64; 2], [i64; 2])>,
-) -> Vec<i64> {
+) -> Vec<Option<i64>> {
     // skip empty
     if positions.is_empty() {
         return vec![];
     }
     if aligned_block_pairs.is_empty() {
-        return positions.iter().map(|_x| -1).collect();
+        return positions.iter().map(|_x| None).collect();
     }
     assert!(
         is_sorted(positions),
         "Positions must be sorted before calling liftover!"
     );
 
     // find the closest position for every position
@@ -207,45 +211,49 @@
                 starting_block = current_block;
             }
             current_block += 1;
         }
     }
     let mut rtn = vec![];
     for q_pos in positions {
-        let (r_pos, _diff) = pos_mapping.get(q_pos).unwrap();
-        rtn.push(*r_pos);
+        let (r_pos, diff) = pos_mapping.get(q_pos).unwrap();
+        if *r_pos == -1 && *diff == i64::MAX {
+            rtn.push(None);
+        } else {
+            rtn.push(Some(*r_pos));
+        }
     }
     assert_eq!(rtn.len(), positions.len());
     rtn
 }
 
 /// find the closest reference positions for a list of query positions
 pub fn lift_reference_positions(
     aligned_block_pairs: &Vec<([i64; 2], [i64; 2])>,
     query_positions: &[i64],
-) -> Vec<i64> {
+) -> Vec<Option<i64>> {
     liftover_closest(query_positions, aligned_block_pairs)
 }
 
 /// find the closest query positions for a list of reference positions
 pub fn lift_query_positions(
     aligned_block_pairs: &Vec<([i64; 2], [i64; 2])>,
     reference_positions: &[i64],
-) -> Vec<i64> {
+) -> Vec<Option<i64>> {
     // if lifting to the query, we need to reverse the pairs
     let aligned_block_pairs = aligned_block_pairs.iter().map(|(q, r)| (*r, *q)).collect();
     liftover_closest(reference_positions, &aligned_block_pairs)
 }
 
-pub fn lift_range(
+fn lift_range(
     aligned_block_pairs: &Vec<([i64; 2], [i64; 2])>,
     starts: &[i64],
     ends: &[i64],
     lift_reference_to_query: bool,
-) -> (Vec<i64>, Vec<i64>, Vec<i64>) {
+) -> (Vec<Option<i64>>, Vec<Option<i64>>, Vec<Option<i64>>) {
     assert_eq!(starts.len(), ends.len());
     let (ref_starts, ref_ends) = if !lift_reference_to_query {
         (
             lift_reference_positions(aligned_block_pairs, starts),
             lift_reference_positions(aligned_block_pairs, ends),
         )
     } else {
@@ -254,42 +262,49 @@
             lift_query_positions(aligned_block_pairs, ends),
         )
     };
     assert_eq!(ref_starts.len(), ref_ends.len());
     let rtn = ref_starts
         .into_iter()
         .zip(ref_ends.into_iter())
-        .map(|(start, end)| {
-            if end <= start {
-                (-1, -1, -1)
-            } else {
-                (start, end, end - start)
+        .map(|(start, end)| match (start, end) {
+            (Some(start), Some(end)) => {
+                if start == end {
+                    (None, None, None)
+                } else {
+                    (Some(start), Some(end), Some(end - start))
+                }
             }
+            _ => (None, None, None),
         })
         .collect::<Vec<_>>();
     multiunzip(rtn)
 }
 
 /// Find the closest range but hopefully better
 pub fn lift_query_range(
     record: &bam::Record,
     starts: &[i64],
     ends: &[i64],
-) -> (Vec<i64>, Vec<i64>, Vec<i64>) {
+) -> (Vec<Option<i64>>, Vec<Option<i64>>, Vec<Option<i64>>) {
     // get the aligned block pairs
     let aligned_block_pairs: Vec<([i64; 2], [i64; 2])> = record.aligned_block_pairs().collect();
     lift_range(&aligned_block_pairs, starts, ends, false)
 }
 
+//
+// EXACT LIFTOVER FUNCTIONS
+//
+
 /// liftover positions using the cigar string
-pub fn liftover_exact(
+fn liftover_exact(
     aligned_block_pairs: &Vec<([i64; 2], [i64; 2])>,
     positions: &[i64],
     lift_reference_to_query: bool,
-) -> Vec<i64> {
+) -> Vec<Option<i64>> {
     assert!(
         is_sorted(positions),
         "Positions must be sorted before calling liftover!"
     );
 
     // find the shared positions in the reference
     let mut return_positions = vec![];
@@ -311,45 +326,51 @@
             if cur_pos >= *st {
                 let dist_from_start = cur_pos - st;
                 let rtn_pos = if !lift_reference_to_query {
                     r_st + dist_from_start
                 } else {
                     q_st + dist_from_start
                 };
-                return_positions.push(rtn_pos);
+                return_positions.push(Some(rtn_pos));
             } else {
-                return_positions.push(-1);
+                return_positions.push(None);
             }
             // reset current position
             cur_idx += 1;
             if cur_idx == positions.len() {
                 break;
             }
             cur_pos = positions[cur_idx];
         }
     }
 
     // add values for things that won't lift at the end
     while positions.len() > return_positions.len() {
-        return_positions.push(-1);
+        return_positions.push(None);
     }
     assert_eq!(positions.len(), return_positions.len());
     return_positions
 }
 
-pub fn lift_reference_positions_exact(record: &bam::Record, query_positions: &[i64]) -> Vec<i64> {
+pub fn lift_reference_positions_exact(
+    record: &bam::Record,
+    query_positions: &[i64],
+) -> Vec<Option<i64>> {
     if record.is_unmapped() {
-        query_positions.iter().map(|_x| -1).collect()
+        query_positions.iter().map(|_x| None).collect()
     } else {
         let aligned_block_pairs: Vec<([i64; 2], [i64; 2])> = record.aligned_block_pairs().collect();
         liftover_exact(&aligned_block_pairs, query_positions, false)
     }
 }
 
-pub fn lift_query_positions_exact(record: &bam::Record, reference_positions: &[i64]) -> Vec<i64> {
+pub fn lift_query_positions_exact(
+    record: &bam::Record,
+    reference_positions: &[i64],
+) -> Vec<Option<i64>> {
     if record.is_unmapped() {
-        reference_positions.iter().map(|_x| -1).collect()
+        reference_positions.iter().map(|_x| None).collect()
     } else {
         let aligned_block_pairs: Vec<([i64; 2], [i64; 2])> = record.aligned_block_pairs().collect();
         liftover_exact(&aligned_block_pairs, reference_positions, true)
     }
 }
```

### Comparing `pyft-0.1.8/local_dependencies/bamlift/tests/test-liftover.rs` & `pyft-0.1.9/local_dependencies/bamlift/tests/test-liftover.rs`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     let aligned_block_pairs = vec![
         ([0, 4], [40, 44]),
         ([7, 8], [50, 51]),
         ([9, 20], [59, 70]),
         ([20, 21], [70, 71]),
     ];
     let positions = vec![1, 2, 3, 4, 5, 6, 7, 8, 9];
-    let expected_result = vec![41, 42, 43, 44, 44, 50, 50, 51, 59];
+    let expected_result = vec![41, 42, 43, 44, 44, 50, 50, 51, 59]
+        .into_iter()
+        .map(Some)
+        .collect::<Vec<_>>();
     let result = lift_reference_positions(&aligned_block_pairs, &positions);
     assert_eq!(result, expected_result);
 }
 
 ///```
 /// use rust_htslib::{bam, bam::Read};
 /// use bamlift::*;
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.toml` & `pyft-0.1.9/local_dependencies/fibertools-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/CI.yml` & `pyft-0.1.9/local_dependencies/fibertools-rs/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/.github/workflows/release.yml` & `pyft-0.1.9/local_dependencies/fibertools-rs/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/CHANGELOG.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,98 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and the project tries but probably doesn't to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## Unreleased
+
+### Chore
+
+ - <csr-id-6fe2beb91b2552292563fdae391c5ce026eded1d/> simplifed center with new api.
+ - <csr-id-df3ffba3aafa8403cdc95b6e0c31de07ac0a8114/> refactor a large part of the code base to reduce redudance. TODO simplify center and basemods with this new api.
+ - <csr-id-96b4fc0638e991ec6c29dffbb1678b99ffc00b1d/> improve docs
+ - <csr-id-1436dbfb05c542aa1f4c862d46113e43d0b396d8/> drop darkmode
+ - <csr-id-04b1e9b02059718fea91b0aef71efc0d9d86f744/> fix docs and fetch
+ - <csr-id-f73a36a716023835e16da50838752d74a2768843/> regex update
+ - <csr-id-168c9517b5137dbd58950f341d96a420c7d50935/> readme
+ - <csr-id-9f711585d39c66ff45598d85dbf3783aca6ee44c/> clippy
+ - <csr-id-a80fe514ff3d4bf860dedbf7130a21d97b9537ab/> hide more deps under features for pyft
+ - <csr-id-c55fcc59749216e0f65c3d9c07efc14f32fb5fdf/> example py-ft
+ - <csr-id-2e1fe93f48b357fbb3459f5206fc5a994325d7a4/> unify api anming for liftover, optimize for inclusion in pyft
+ - <csr-id-3e6aa945cb643e5d0559fac59b14a649e0de34b1/> reduce number of copies for nuc and msp.
+ - <csr-id-eea28d57a9eac79e3e3e0d9d16ede6dce51d242e/> move nuc and msp logic out of extract into ranges struct and simplify. We ran on a whole genome ft extract to confirm results dont change.
+### New Features
+
+ - <csr-id-b9f4950f2839c5d8df61593ec58997e439fc5c6a/> add qual to ft cetner, and clean the ft center code more
+ - <csr-id-96f251b7f370f68e729357f52d3f2b6400d1af33/> adding ft center to the python module!
+ - <csr-id-9da4fa3b27e991250185463de48ba0ebea866bce/> Reorganize pyft api and docs
+ - <csr-id-248bf4e56c5b10c2dd4613888818a995e6f75529/> adding liftover to pyft
+ - <csr-id-6a695ec7a71e5002709d5496c8aade541e737514/> very large improvment in speed of lifting over ranges, some liftover results differ from before by 1bp but it is rare.
+
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 40 commits contributed to the release over the course of 2 calendar days.
+ - 3 days passed between releases.
+ - 28 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Readme ([`6595c36`](https://github.com/fiberseq/fibertools-rs/commit/6595c3696dda1288f0f763fdc54d7311dfb790c9))
+    - Add qual to ft cetner, and clean the ft center code more ([`b9f4950`](https://github.com/fiberseq/fibertools-rs/commit/b9f4950f2839c5d8df61593ec58997e439fc5c6a))
+    - Docs ([`1a1f260`](https://github.com/fiberseq/fibertools-rs/commit/1a1f260323e262772ce7ecfaed2df52ab2597b5d))
+    - Docs ([`2ab1645`](https://github.com/fiberseq/fibertools-rs/commit/2ab16455268ef311fbc60a17a7831e05b2f2cf8a))
+    - Simplifed center with new api. ([`6fe2beb`](https://github.com/fiberseq/fibertools-rs/commit/6fe2beb91b2552292563fdae391c5ce026eded1d))
+    - Refactor a large part of the code base to reduce redudance. TODO simplify center and basemods with this new api. ([`df3ffba`](https://github.com/fiberseq/fibertools-rs/commit/df3ffba3aafa8403cdc95b6e0c31de07ac0a8114))
+    - Improve docs ([`96b4fc0`](https://github.com/fiberseq/fibertools-rs/commit/96b4fc0638e991ec6c29dffbb1678b99ffc00b1d))
+    - Adding ft center to the python module! ([`96f251b`](https://github.com/fiberseq/fibertools-rs/commit/96f251b7f370f68e729357f52d3f2b6400d1af33))
+    - Drop darkmode ([`1436dbf`](https://github.com/fiberseq/fibertools-rs/commit/1436dbfb05c542aa1f4c862d46113e43d0b396d8))
+    - Fix docs and fetch ([`04b1e9b`](https://github.com/fiberseq/fibertools-rs/commit/04b1e9b02059718fea91b0aef71efc0d9d86f744))
+    - Clean ([`1d5872d`](https://github.com/fiberseq/fibertools-rs/commit/1d5872dc510a370c065076e533af1913ccbc764f))
+    - Reorganize pyft api and docs ([`9da4fa3`](https://github.com/fiberseq/fibertools-rs/commit/9da4fa3b27e991250185463de48ba0ebea866bce))
+    - Check for sorted ([`8fbdc7c`](https://github.com/fiberseq/fibertools-rs/commit/8fbdc7c1a4af7039e62f249c49a4ca226023eefb))
+    - Check for sorted ([`624dd33`](https://github.com/fiberseq/fibertools-rs/commit/624dd3317814594b47835be120a8d4bcadc775f6))
+    - Block index ([`ab59d1d`](https://github.com/fiberseq/fibertools-rs/commit/ab59d1d3a650530c75d50b507a594ee7cc74eddc))
+    - Regex update ([`f73a36a`](https://github.com/fiberseq/fibertools-rs/commit/f73a36a716023835e16da50838752d74a2768843))
+    - Readme ([`8bf2168`](https://github.com/fiberseq/fibertools-rs/commit/8bf2168969acf67fa5069fb578f94941bd01e3f4))
+    - Readme ([`15d535a`](https://github.com/fiberseq/fibertools-rs/commit/15d535ae7dc90f86bec99a18015a22376c195788))
+    - Readme ([`aba1d75`](https://github.com/fiberseq/fibertools-rs/commit/aba1d7572a6109bb2e7d2acffea5f5e5c4f1ced6))
+    - Readme ([`9ea0b5f`](https://github.com/fiberseq/fibertools-rs/commit/9ea0b5f04f21cf74ab40a0ff1097eac996cc5b8b))
+    - Readme ([`69d87ea`](https://github.com/fiberseq/fibertools-rs/commit/69d87ea41febf0bd88380708cacea4232ae57f24))
+    - Readme ([`970c41f`](https://github.com/fiberseq/fibertools-rs/commit/970c41f9ba4a8c26bf980f0ce87f635dd4f68bd3))
+    - Readme ([`49180bc`](https://github.com/fiberseq/fibertools-rs/commit/49180bccd2dffdc49313e0b259dcdd0e80682bba))
+    - Readme ([`c8a2ab4`](https://github.com/fiberseq/fibertools-rs/commit/c8a2ab45cbff913c41bde48903c129b6e4d2f70a))
+    - Readme ([`168c951`](https://github.com/fiberseq/fibertools-rs/commit/168c9517b5137dbd58950f341d96a420c7d50935))
+    - Readme ([`f5a65a6`](https://github.com/fiberseq/fibertools-rs/commit/f5a65a612b8978f9742dab6990a8d52c6df7645a))
+    - Clippy ([`9f71158`](https://github.com/fiberseq/fibertools-rs/commit/9f711585d39c66ff45598d85dbf3783aca6ee44c))
+    - Clippy ([`b4278e4`](https://github.com/fiberseq/fibertools-rs/commit/b4278e4599a6634f37f05874a7e2e860c0b6a45a))
+    - Adding liftover to pyft ([`248bf4e`](https://github.com/fiberseq/fibertools-rs/commit/248bf4e56c5b10c2dd4613888818a995e6f75529))
+    - Unify api anming for liftover, optimize for inclusion in pyft ([`2e1fe93`](https://github.com/fiberseq/fibertools-rs/commit/2e1fe93f48b357fbb3459f5206fc5a994325d7a4))
+    - Unify api anming for liftover, optimize for inclusion in pyft ([`1c32392`](https://github.com/fiberseq/fibertools-rs/commit/1c32392c0bb24adfb3dc4bc78ab290e5405e2a62))
+    - Clean ([`0e2a574`](https://github.com/fiberseq/fibertools-rs/commit/0e2a574cfd8e1b832a3f157b51c22a60713039a9))
+    - Speed up and clean up approximate liftover and add a real test ([`c1ac44e`](https://github.com/fiberseq/fibertools-rs/commit/c1ac44e0a188a77900f9bf1dfef2dfbc42b3fdb9))
+    - Update with ranges ([`cae1a41`](https://github.com/fiberseq/fibertools-rs/commit/cae1a415a2dac4aca1558d14a50eaa0cba258b09))
+    - Very large improvment in speed of lifting over ranges, some liftover results differ from before by 1bp but it is rare. ([`6a695ec`](https://github.com/fiberseq/fibertools-rs/commit/6a695ec7a71e5002709d5496c8aade541e737514))
+    - Hide more deps under features for pyft ([`a80fe51`](https://github.com/fiberseq/fibertools-rs/commit/a80fe514ff3d4bf860dedbf7130a21d97b9537ab))
+    - Clean writes in center. ([`0d19ac1`](https://github.com/fiberseq/fibertools-rs/commit/0d19ac12281dd7fef0b571a745a3e6240bc771a3))
+    - Reduce number of copies for nuc and msp. ([`3e6aa94`](https://github.com/fiberseq/fibertools-rs/commit/3e6aa945cb643e5d0559fac59b14a649e0de34b1))
+    - Move nuc and msp logic out of extract into ranges struct and simplify. We ran on a whole genome ft extract to confirm results dont change. ([`eea28d5`](https://github.com/fiberseq/fibertools-rs/commit/eea28d57a9eac79e3e3e0d9d16ede6dce51d242e))
+    - Example py-ft ([`c55fcc5`](https://github.com/fiberseq/fibertools-rs/commit/c55fcc59749216e0f65c3d9c07efc14f32fb5fdf))
+</details>
+
 ## 0.2.6 (2023-07-21)
 
 <csr-id-66b98f9f3c2644e79bf72de2ed070fba75b2ba38/>
 <csr-id-9e8cda2fb47eff101eb3d458cf4599543e7d05a2/>
 <csr-id-23e6b12a7601afb4aa21454048a53d803ca1bcdf/>
 <csr-id-b03df77d99a8f28ecd6d43509a43ff92fb300329/>
 <csr-id-6e8cd6f9f25dcabc15ef2a25595b3a3ee86de241/>
@@ -60,75 +144,37 @@
 ### New Features
 
  - <csr-id-3ea32b01fda3e12f0cacae90d5a52495cec0b6bd/> add cpg to python modele and make easier access in the rust basemod api
  - <csr-id-1f6fea3cf07e1e798649df45d944a5396bf82902/> I have a minimal working python package yay!
 
 ### Chore
 
- - <csr-id-66b98f9f3c2644e79bf72de2ed070fba75b2ba38/> rename iterator
- - <csr-id-9e8cda2fb47eff101eb3d458cf4599543e7d05a2/> rename iterator
- - <csr-id-23e6b12a7601afb4aa21454048a53d803ca1bcdf/> rename iterator
  - <csr-id-b03df77d99a8f28ecd6d43509a43ff92fb300329/> rename iterator
  - <csr-id-6e8cd6f9f25dcabc15ef2a25595b3a3ee86de241/> docs
- - <csr-id-79ca845b0e72e832cdc57b1e1b58090a09417936/> docs
- - <csr-id-41bcd27e9de8654fd46bfb50d3c7efabad59a17e/> docs
- - <csr-id-66338fd576a66ee230aa4234d072a93b3a3b21d5/> docs
- - <csr-id-6f910c53a4e0cb7be411b724385e540517f21306/> docs
- - <csr-id-85d471df45a0c88567857427725852c491c041ff/> docs
- - <csr-id-c5eb60a8d42616eacfafb871cf4f46fb2fa924c8/> docs
- - <csr-id-5bd6803c346a409150daea7713878af46995e836/> docs
- - <csr-id-a59f41d0b2d4b97b277b738f04b23010be8d6449/> docs
- - <csr-id-7a633d71272a9425ae276d9b846fcda38f6526e5/> docs
- - <csr-id-8d16055edc4bf9bc5f94d5be42b86b2a2df712c8/> docs
- - <csr-id-467072ae6419b3ece8329f587467d0d0bf316911/> docs
- - <csr-id-09994bdbdd3949186d44ecef36199a8d228ea280/> docs
- - <csr-id-8ea9fb1efc4897e191468ee10aa66500456fa0fc/> docs
- - <csr-id-82399e6e702033acbb455ef6aea3a9935338d77f/> docs
- - <csr-id-fd115b7fdb6754d6f6885e901bc34d7364bfc7df/> docs
- - <csr-id-1d25caf7e8c19f97d39dec8eb69de7219e85621b/> docs
- - <csr-id-e73e00c849726e4577344ec8e964b3eda93ddbc6/> docs
- - <csr-id-a3f29cd798fcbeb071fce7ea7041c4e71a98f8f6/> docs
- - <csr-id-e85afd963f513fe578b2d0f3e368a7ae56b59d84/> docs
- - <csr-id-580968a9da3c2a66740d01dfcc0d8c574bfd46c8/> docs
- - <csr-id-6b1e714ccda049aef3199563c03d6f5ec1df9dfa/> docs
- - <csr-id-c8502ac7cf87d375a5aa9fcf3494a3cf8f43105c/> docs
- - <csr-id-b9274c2a7064cd615b079b3cc0b44d9e2f4b5e50/> docs
- - <csr-id-eb44bdaf8280689eb06e536266b64802f509a7b3/> docs
- - <csr-id-b98edf9f855ae24f81389a5ea481bf0b16dcd794/> python docs
- - <csr-id-32f01826bbf06ac726464d59eee2769dfe80b138/> python docs
- - <csr-id-94dfd521a3f637df47c996fd046d1de3cde85776/> python docs
- - <csr-id-b3fa1c3b218379a3290fbed2382572b5e1c3e091/> python docs
- - <csr-id-d4b75b1a569d694495bc1e87de651c1bb4e63778/> python docs
- - <csr-id-73c918f9344fe362f602fa5356b11c9574c5ffec/> python docs
- - <csr-id-5f635e04085c012d39d8afa362416ca3642fc7c5/> python docs
- - <csr-id-c86cc585993506c55bd0243936767afe4a5f671c/> python docs
- - <csr-id-15b825ed80a4b099c9ea9f21f64f1b695e20554a/> python docs
- - <csr-id-26ef86389490b3161546271bea194e4c8a4a8b7f/> python docs
- - <csr-id-d953400d9c7f676fea70fee51264c331ba7e1067/> python docs
  - <csr-id-10bf0df63acca5812e3d2d3ad5134bc75abe73b4/> python docs
  - <csr-id-cdde18e3b119ef36d57feed2f4740b7bde30c011/> readme
  - <csr-id-ac1987d33daf7fb7395ed1cf15b311390a15e60c/> add to changelog
- - <csr-id-2f7c08e2b24a07054d547088ac2c96463a6229d3/> add to changelog
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 78 commits contributed to the release over the course of 2 calendar days.
+ - 79 commits contributed to the release over the course of 2 calendar days.
  - 2 days passed between releases.
  - 48 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release fibertools-rs v0.2.6 ([`3beecf6`](https://github.com/fiberseq/fibertools-rs/commit/3beecf697eafa9707abf5be30a2b773479125069))
     - Release fibertools-rs v0.2.6 ([`e973f17`](https://github.com/fiberseq/fibertools-rs/commit/e973f17def31e7c4731ae10143e6c5be5e01425a))
     - Release fibertools-rs v0.2.6 ([`ba8df9b`](https://github.com/fiberseq/fibertools-rs/commit/ba8df9b8e918be85beef13411cb3aab588634056))
     - Release fibertools-rs v0.2.6 ([`1b5dcfa`](https://github.com/fiberseq/fibertools-rs/commit/1b5dcfa18eef69a8e4a3f7e3e514bb5d5ae87b7f))
     - Release fibertools-rs v0.2.6 ([`5aa1908`](https://github.com/fiberseq/fibertools-rs/commit/5aa19089b0cf0614a7a8d0b4f8dc477d6e808ea5))
     - Release fibertools-rs v0.2.6 ([`656682a`](https://github.com/fiberseq/fibertools-rs/commit/656682a1b70871df4ca52484351d8296755cbe02))
     - Release fibertools-rs v0.2.6 ([`2d2f0f9`](https://github.com/fiberseq/fibertools-rs/commit/2d2f0f96800779088138f6671ab81acfb61cdacc))
     - Release fibertools-rs v0.2.6 ([`b80d856`](https://github.com/fiberseq/fibertools-rs/commit/b80d8567ee7ee899734fa5d2c5fd2b6604d45c78))
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/Cargo.lock` & `pyft-0.1.9/local_dependencies/fibertools-rs/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/Dockerfile` & `pyft-0.1.9/local_dependencies/fibertools-rs/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/INSTALL.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/README.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 ### `ft extract --all`
 The extract all option is a special option that tries to extract all the fiberseq data into a tabular format. The following is an image of the output. Note that the [column names](/docs/ft-all-columns.md) will be preserved across different software versions (unless otherwise noted); however, the order may change and new columns may be added. Therefore, when loading the data (with `pandas` e.g.) be sure to use the column names as opposed to indexes for manipulation.
 ![ft-extract all](/assets/img/ft-extract-all.png)
 ## `ft center`
 Center fiberseq reads (bam) around reference position(s). [Help page for center](/docs/ft-center-help.md).
 ![Center](/assets/img/center.png)
 
+# Python API (`pyft`)
+The python API is still in development and not stable; however, you can find the current code progress in the [py-ft](/py-ft) folder. More information available at [readthedocs](https://py-ft.readthedocs.io/en/latest/).
+
 # Cite
 **Jha, A.**, **Bohaczuk, S. C.**, Mao, Y., Ranchalis, J., Mallory, B. J., Min, A. T., Hamm, M. O., Swanson, E., Finkbeiner, C., Li, T., Whittington, D., Stergachis, A. B., & **Vollger, M. R.** (2023). Fibertools: fast and accurate DNA-m6A calling using single-molecule long-read sequencing. *bioRxiv*. https://doi.org/10.1101/2023.04.20.537673
 
 # Read the fibertools library docs
 You can find the docs for the latest release here:
 [https://docs.rs/fibertools-rs/latest/fibertools_rs/](https://docs.rs/fibertools-rs/latest/fibertools_rs/)
 or download from source and run:
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/center.png` & `pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/center.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png` & `pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png` & `pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/fiber_tools_teal.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png` & `pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/ft-extract-all.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/assets/img/logo.png` & `pyft-0.1.9/local_dependencies/fibertools-rs/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/build.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/build.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft--help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft--help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-add-nucleosomes-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-center-help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-center-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-extract-help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-extract-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-predict-m6a-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/ft-strip-basemods-help.md`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/docs/make_help_docs.sh` & `pyft-0.1.9/local_dependencies/fibertools-rs/docs/make_help_docs.sh`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.0_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.0_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/2.2_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/2.2_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/3.2_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/3.2_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/Revio_semi_torch.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/Revio_semi_torch.pt`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.0.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json` & `pyft-0.1.9/local_dependencies/fibertools-rs/models/gbdt_0.81_p2.2.json`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/basemods/mod.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/basemods/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,29 @@
     bam,
     bam::record::{Aux, AuxArray},
 };
 use std::collections::HashMap;
 
 use std::convert::TryFrom;
 
+pub enum FiberModTypes {
+    M6A,
+    CPG,
+}
+
 #[derive(Eq, PartialEq, Debug, PartialOrd, Ord, Clone)]
 pub struct BaseMod {
     pub modified_base: u8,
     pub strand: char,
     pub modification_type: char,
     record_is_reverse: bool,
     modified_bases: Vec<i64>,
     modified_bases_forward: Vec<i64>,
     modified_probabilities: Vec<u8>,
-    reference_positions: Vec<i64>,
+    reference_positions: Vec<Option<i64>>,
 }
 
 impl BaseMod {
     pub fn new(
         record: &bam::Record,
         modified_base: u8,
         strand: char,
@@ -54,15 +59,15 @@
             modified_bases,
             modified_bases_forward,
             modified_probabilities,
             reference_positions,
         }
     }
 
-    pub fn get_reference_positions(&self) -> Vec<i64> {
+    pub fn get_reference_positions(&self) -> Vec<Option<i64>> {
         self.reference_positions.clone()
     }
 
     pub fn get_modified_bases(&self) -> Vec<i64> {
         self.modified_bases.clone()
     }
 
@@ -282,129 +287,67 @@
     }
 
     /// remove cpg/5mc base mods from the struct
     pub fn drop_cpg(&mut self) {
         self.base_mods.retain(|bm| !bm.is_cpg());
     }
 
-    pub fn m6a_positions(&self, reference: bool) -> Vec<i64> {
-        let m6a: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_m6a()).collect();
-        // skip if no m6a
-        if m6a.is_empty() {
-            return vec![];
-        }
-        // if we only have one of the two mod types
-        if m6a.len() == 1 {
-            if reference {
-                return m6a[0].get_reference_positions();
-            } else {
-                return m6a[0].get_modified_bases();
-            }
-        }
-        // get positions of m6a if we have both A+a and T-a
-        if reference {
-            merge_two_lists(
-                &m6a[0].get_reference_positions(),
-                &m6a[1].get_reference_positions(),
-            )
-        } else {
-            merge_two_lists(&m6a[0].get_modified_bases(), &m6a[1].get_modified_bases())
-        }
-    }
+    fn helper_get_basemods(
+        &self,
+        forward: bool,
+        fiber_mod_type: FiberModTypes,
+    ) -> (Vec<i64>, Vec<Option<i64>>, Vec<u8>) {
+        let bm: Vec<&BaseMod> = match fiber_mod_type {
+            FiberModTypes::M6A => self.base_mods.iter().filter(|x| x.is_m6a()).collect(),
+            FiberModTypes::CPG => self.base_mods.iter().filter(|x| x.is_cpg()).collect(),
+        };
 
-    fn helper_get_m6a(&self, forward: bool) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        let m6a: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_m6a()).collect();
-        // skip if no m6a
-        if m6a.is_empty() {
+        // skip if no basemods
+        if bm.is_empty() {
             return (vec![], vec![], vec![]);
         }
 
-        let m6a_pos: Vec<i64> = if forward {
-            m6a.iter()
+        let bm_pos: Vec<i64> = if forward {
+            bm.iter()
                 .flat_map(|x| x.get_modified_bases_forward())
                 .collect()
         } else {
-            m6a.iter().flat_map(|x| x.get_modified_bases()).collect()
+            bm.iter().flat_map(|x| x.get_modified_bases()).collect()
         };
 
-        let m6a_ref: Vec<i64> = m6a
+        let bm_ref: Vec<Option<i64>> = bm
             .iter()
             .flat_map(|x| x.get_reference_positions())
             .collect();
-        let m6a_qual: Vec<u8> = m6a
+        let bm_qual: Vec<u8> = bm
             .iter()
             .flat_map(|x| x.get_modified_probabilities())
             .collect();
 
-        assert_eq!(m6a_pos.len(), m6a_ref.len());
-        assert_eq!(m6a_ref.len(), m6a_qual.len());
-        let mut z: Vec<(i64, i64, u8)> = izip!(m6a_pos, m6a_ref, m6a_qual).collect();
+        assert_eq!(bm_pos.len(), bm_ref.len());
+        assert_eq!(bm_ref.len(), bm_qual.len());
+        let mut z: Vec<(i64, Option<i64>, u8)> = izip!(bm_pos, bm_ref, bm_qual).collect();
         z.sort_by_key(|(p, _r, _q)| *p);
         multiunzip(z)
     }
 
-    pub fn m6a(&self) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        self.helper_get_m6a(false)
+    pub fn m6a(&self) -> (Vec<i64>, Vec<Option<i64>>, Vec<u8>) {
+        self.helper_get_basemods(false, FiberModTypes::M6A)
     }
 
-    pub fn forward_m6a(&self) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        self.helper_get_m6a(true)
-    }
-
-    pub fn cpg_positions(&self, reference: bool) -> Vec<i64> {
-        let cpg: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_cpg()).collect();
-        // skip if no cpg
-        if cpg.is_empty() {
-            return vec![];
-        }
-        // get positions of cpg
-        if reference {
-            cpg[0].get_reference_positions()
-        } else {
-            cpg[0].get_modified_bases()
-        }
-    }
-
-    fn helper_get_cpg(&self, forward: bool) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        let cpg: Vec<&BaseMod> = self.base_mods.iter().filter(|x| x.is_cpg()).collect();
-        // skip if no m6a
-        if cpg.is_empty() {
-            return (vec![], vec![], vec![]);
-        }
-
-        let cpg_pos: Vec<i64> = if forward {
-            cpg.iter()
-                .flat_map(|x| x.get_modified_bases_forward())
-                .collect()
-        } else {
-            cpg.iter().flat_map(|x| x.get_modified_bases()).collect()
-        };
-
-        let cpg_ref: Vec<i64> = cpg
-            .iter()
-            .flat_map(|x| x.get_reference_positions())
-            .collect();
-        let cpg_qual: Vec<u8> = cpg
-            .iter()
-            .flat_map(|x| x.get_modified_probabilities())
-            .collect();
-
-        assert_eq!(cpg_pos.len(), cpg_ref.len());
-        assert_eq!(cpg_ref.len(), cpg_qual.len());
-        let mut z: Vec<(i64, i64, u8)> = izip!(cpg_pos, cpg_ref, cpg_qual).collect();
-        z.sort_by_key(|(p, _r, _q)| *p);
-        multiunzip(z)
+    pub fn forward_m6a(&self) -> (Vec<i64>, Vec<Option<i64>>, Vec<u8>) {
+        self.helper_get_basemods(true, FiberModTypes::M6A)
     }
 
-    pub fn cpg(&self) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        self.helper_get_cpg(false)
+    pub fn cpg(&self) -> (Vec<i64>, Vec<Option<i64>>, Vec<u8>) {
+        self.helper_get_basemods(false, FiberModTypes::CPG)
     }
 
-    pub fn forward_cpg(&self) -> (Vec<i64>, Vec<i64>, Vec<u8>) {
-        self.helper_get_cpg(true)
+    pub fn forward_cpg(&self) -> (Vec<i64>, Vec<Option<i64>>, Vec<u8>) {
+        self.helper_get_basemods(true, FiberModTypes::CPG)
     }
 
     /// Example MM tag: MM:Z:C+m,11,6,10;A+a,0,0,0;
     /// Example ML tag: ML:B:C,157,30,2,164,118,255
     pub fn add_mm_and_ml_tags(&self, record: &mut bam::Record) {
         // init the mm and ml tag to be populated
         let mut ml_tag: Vec<u8> = vec![];
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/center.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/center.rs`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         (ref_offset, mol_offset)
     }
 
     /// find the query position that corresponds to the central reference position
     pub fn find_offset(record: &bam::Record, reference_position: i64) -> Option<i64> {
         let read_center: Vec<i64> = lift_query_positions_exact(record, &[reference_position])
             .into_iter()
-            .filter(|&x| x >= 0)
+            .flatten()
             .collect();
         log::debug!(
             "{}, {}, {}, {:?}",
             reference_position,
             record.reference_start(),
             record.reference_end(),
             read_center
@@ -90,54 +90,14 @@
         if self.center_position.strand == '-' {
             out_seq = revcomp(out_seq);
         }
         //assert_eq!(out_seq.len() as i64, dist * 2 + 1);
         String::from_utf8_lossy(&out_seq).to_string()
     }
 
-    pub fn m6a_positions(&self) -> Vec<i64> {
-        self.fiber.m6a_positions(self.reference).to_vec()
-    }
-
-    pub fn cpg_positions(&self) -> Vec<i64> {
-        self.fiber.cpg_positions(self.reference).to_vec()
-    }
-
-    pub fn nuc_positions(&self) -> Vec<(i64, i64)> {
-        let (starts, ends) = if self.reference {
-            (
-                &self.fiber.nuc.reference_starts,
-                &self.fiber.nuc.reference_ends,
-            )
-        } else {
-            (&self.fiber.nuc.starts, &self.fiber.nuc.ends)
-        };
-        starts
-            .clone()
-            .into_iter()
-            .zip(ends.clone().into_iter())
-            .collect()
-    }
-
-    pub fn msp_positions(&self) -> Vec<(i64, i64)> {
-        let (starts, ends) = if self.reference {
-            (
-                &self.fiber.msp.reference_starts,
-                &self.fiber.msp.reference_ends,
-            )
-        } else {
-            (&self.fiber.msp.starts, &self.fiber.msp.ends)
-        };
-        starts
-            .clone()
-            .into_iter()
-            .zip(ends.clone().into_iter())
-            .collect()
-    }
-
     pub fn get_sequence(&self) -> String {
         let forward_bases = if self.center_position.strand == '+' {
             self.fiber.record.seq().as_bytes()
         } else {
             revcomp(self.fiber.record.seq().as_bytes())
         };
         String::from_utf8_lossy(&forward_bases).to_string()
@@ -156,28 +116,65 @@
             self.fiber.rg,
             -self.offset,
             self.fiber.record.seq_len() as i64 - self.offset,
             self.fiber.record.seq_len()
         )
     }
 
+    #[allow(clippy::type_complexity)]
+    fn grab_data(
+        &self,
+    ) -> (
+        &[Option<i64>],
+        &[u8],
+        &[Option<i64>],
+        &[u8],
+        &[Option<i64>],
+        &[Option<i64>],
+        &[Option<i64>],
+        &[Option<i64>],
+    ) {
+        if self.reference {
+            (
+                &self.fiber.m6a.reference_starts,
+                &self.fiber.m6a.ml,
+                &self.fiber.cpg.reference_starts,
+                &self.fiber.cpg.ml,
+                &self.fiber.nuc.reference_starts,
+                &self.fiber.nuc.reference_ends,
+                &self.fiber.msp.reference_starts,
+                &self.fiber.msp.reference_ends,
+            )
+        } else {
+            (
+                &self.fiber.m6a.starts,
+                &self.fiber.m6a.ml,
+                &self.fiber.cpg.starts,
+                &self.fiber.cpg.ml,
+                &self.fiber.nuc.starts,
+                &self.fiber.nuc.ends,
+                &self.fiber.msp.starts,
+                &self.fiber.msp.ends,
+            )
+        }
+    }
+
     pub fn write(&self) -> String {
-        let m6a = join_by_str(self.m6a_positions(), ",");
-        let cpg = join_by_str(self.cpg_positions(), ",");
-        let (nuc_st, nuc_en) = unzip_to_vectors(self.nuc_positions());
-        let (msp_st, msp_en) = unzip_to_vectors(self.msp_positions());
+        let (m6a, m6a_qual, cpg, cpg_qual, nuc_st, nuc_en, msp_st, msp_en) = self.grab_data();
         format!(
-            "{}{}\t{}\t{}\t{}\t{}\t{}\t{}\n",
+            "{}{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\n",
             self.leading_columns(),
-            m6a,
-            cpg,
-            join_by_str(nuc_st, ","),
-            join_by_str(nuc_en, ","),
-            join_by_str(msp_st, ","),
-            join_by_str(msp_en, ","),
+            join_by_str_option(m6a, ""),
+            join_by_str(m6a_qual, ","),
+            join_by_str_option(cpg, ""),
+            join_by_str(cpg_qual, ","),
+            join_by_str_option(nuc_st, ","),
+            join_by_str_option(nuc_en, ","),
+            join_by_str_option(msp_st, ","),
+            join_by_str_option(msp_en, ","),
             self.get_sequence(),
         )
     }
 
     pub fn leading_header() -> String {
         format!(
             "{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t",
@@ -192,66 +189,82 @@
             "centered_query_start",
             "centered_query_end",
             "query_length",
         )
     }
     pub fn header() -> String {
         format!(
-            "{}{}\t{}\t{}\t{}\t{}\t{}\t{}\n",
+            "{}{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\n",
             CenteredFiberData::leading_header(),
             "centered_m6a_positions",
+            "m6a_qual",
             "centered_5mC_positions",
+            "5mC_qual",
             "centered_nuc_starts",
             "centered_nuc_ends",
             "centered_msp_starts",
             "centered_msp_ends",
             "query_sequence"
         )
     }
 
     pub fn long_header() -> String {
         format!(
-            "{}{}\t{}\t{}\n",
+            "{}{}\t{}\t{}\t{}\n",
             CenteredFiberData::leading_header(),
             "centered_position_type",
             "centered_start",
             "centered_end",
+            "centered_qual",
         )
     }
 
     pub fn write_long(&self) -> String {
-        let m6a = self.m6a_positions();
-        let cpg = self.cpg_positions();
-        let (nuc_st, nuc_en) = unzip_to_vectors(self.nuc_positions());
-        let (msp_st, msp_en) = unzip_to_vectors(self.msp_positions());
         let mut rtn = String::new();
+        let (m6a, m6a_qual, cpg, cpg_qual, nuc_st, nuc_en, msp_st, msp_en) = self.grab_data();
         for (t, vals) in [
-            ("m6a", (m6a, None)),
-            ("5mC", (cpg, None)),
-            ("nuc", (nuc_st, Some(nuc_en))),
-            ("msp", (msp_st, Some(msp_en))),
+            ("m6a", (m6a, None, Some(m6a_qual))),
+            ("5mC", (cpg, None, Some(cpg_qual))),
+            ("nuc", (nuc_st, Some(nuc_en), None)),
+            ("msp", (msp_st, Some(msp_en), None)),
         ] {
-            let starts = vals.0;
-            let ends = match vals.1 {
-                Some(ends) => ends,
-                None => starts.iter().map(|&st| st + 1).collect(),
+            let starts = vals.0.iter().collect::<Vec<_>>();
+            let ends: Vec<Option<i64>> = match vals.1 {
+                Some(ends) => ends.to_vec(),
+                None => vec![None; starts.len()],
             };
-            for (&st, &en) in starts.iter().zip(ends.iter()) {
+            let quals = match vals.2 {
+                Some(quals) => quals.to_vec(),
+                None => vec![0; starts.len()],
+            };
+
+            for ((&st, &en), &qual) in starts.iter().zip(ends.iter()).zip(quals.iter()) {
+                let Some(st) = st else {
+                    continue;
+                };
+                let st = *st;
+                let en = en.unwrap_or(st + 1);
+
                 let mut write = true;
                 if let Some(dist) = self.dist {
                     // skip writing if we are outside the motif range
                     if en <= -dist || st > dist {
                         write = false;
                     }
                 };
                 if write {
                     // add the leading data
                     rtn.push_str(&self.leading_columns());
                     // add the long form data
-                    write!(&mut rtn, "{}", format_args!("{}\t{}\t{}\n", t, st, en)).unwrap();
+                    write!(
+                        &mut rtn,
+                        "{}",
+                        format_args!("{}\t{}\t{}\t{}\n", t, st, en, qual)
+                    )
+                    .unwrap();
                 }
             }
         }
 
         rtn
     }
 }
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/cli.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/cli.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/extract.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/extract.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/fiber.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/fiber.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 use rayon::prelude::*;
 use rust_htslib::{bam, bam::ext::BamRecordExtensions, bam::record::Aux, bam::HeaderView};
 use std::collections::HashMap;
 use std::fmt::Write;
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct FiberMods {
-    pub starts: Vec<i64>,
-    pub reference_starts: Vec<i64>,
+    pub starts: Vec<Option<i64>>,
+    pub reference_starts: Vec<Option<i64>>,
     pub ml: Vec<u8>,
 }
 
 impl FiberMods {
     pub fn new(all_basemods: &BaseMods) -> (Self, Self) {
         let (starts, reference_starts, ml) = all_basemods.m6a();
         let m6a = Self {
-            starts,
+            starts: starts.into_iter().map(Some).collect(),
             reference_starts,
             ml,
         };
         let (starts, reference_starts, ml) = all_basemods.cpg();
         let cpg = Self {
-            starts,
+            starts: starts.into_iter().map(Some).collect(),
             reference_starts,
             ml,
         };
         (m6a, cpg)
     }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct Ranges {
-    pub starts: Vec<i64>,
-    pub ends: Vec<i64>,
-    pub lengths: Vec<i64>,
-    pub reference_starts: Vec<i64>,
-    pub reference_ends: Vec<i64>,
-    pub reference_lengths: Vec<i64>,
+    pub starts: Vec<Option<i64>>,
+    pub ends: Vec<Option<i64>>,
+    pub lengths: Vec<Option<i64>>,
+    pub reference_starts: Vec<Option<i64>>,
+    pub reference_ends: Vec<Option<i64>>,
+    pub reference_lengths: Vec<Option<i64>>,
 }
 
 impl Ranges {
     pub fn new(
         record: &bam::Record,
         mut starts: Vec<i64>,
         ends: Option<Vec<i64>>,
@@ -70,22 +70,22 @@
         if record.is_reverse() {
             std::mem::swap(&mut starts, &mut ends);
         }
         // get lengths
         let lengths = starts
             .iter()
             .zip(ends.iter())
-            .map(|(&x, &y)| y - x)
+            .map(|(&x, &y)| Some(y - x))
             .collect::<Vec<_>>();
 
         let (reference_starts, reference_ends, reference_lengths) =
             lift_query_range(record, &starts, &ends);
         Ranges {
-            starts,
-            ends,
+            starts: starts.into_iter().map(Some).collect(),
+            ends: ends.into_iter().map(Some).collect(),
             lengths,
             reference_starts,
             reference_ends,
             reference_lengths,
         }
     }
 }
@@ -203,65 +203,21 @@
         if let Ok(Aux::U8(f)) = self.record.aux(b"HP") {
             format!("H{f}")
         } else {
             "UNK".to_string()
         }
     }
 
-    pub fn get_nuc(&self, reference: bool, get_starts: bool) -> Vec<i64> {
-        if reference {
-            if get_starts {
-                self.nuc.reference_starts.clone()
-            } else {
-                self.nuc.reference_lengths.clone()
-            }
-        } else if get_starts {
-            self.nuc.starts.clone()
-        } else {
-            self.nuc.lengths.clone()
-        }
-    }
-
-    pub fn get_msp(&self, reference: bool, get_starts: bool) -> Vec<i64> {
-        if reference {
-            if get_starts {
-                self.msp.reference_starts.clone()
-            } else {
-                self.msp.reference_lengths.clone()
-            }
-        } else if get_starts {
-            self.msp.starts.clone()
-        } else {
-            self.msp.lengths.clone()
-        }
-    }
-
-    pub fn m6a_positions(&self, reference: bool) -> &[i64] {
-        if reference {
-            &self.m6a.reference_starts
-        } else {
-            &self.m6a.starts
-        }
-    }
-
-    pub fn cpg_positions(&self, reference: bool) -> &[i64] {
-        if reference {
-            &self.cpg.reference_starts
-        } else {
-            &self.cpg.starts
-        }
-    }
-
     //
     //  CENTERING FUNCTIONS
     //
 
     /// Center positions on the read around the reference position.
-    fn apply_offset(positions: &mut [i64], offset: i64, strand: char) {
-        for pos in positions.iter_mut() {
+    fn apply_offset(positions: &mut [Option<i64>], offset: i64, strand: char) {
+        for pos in positions.iter_mut().flatten() {
             // bp is unaligned
             if *pos == -1 {
                 *pos = i64::MIN;
                 continue;
             }
             // else
             *pos -= offset;
@@ -271,15 +227,20 @@
         }
         if strand == '-' {
             positions.reverse();
         }
     }
 
     /// Center ranges on the read around the reference position.
-    fn offset_range(starts: &mut [i64], ends: &mut [i64], offset: i64, strand: char) {
+    fn offset_range(
+        starts: &mut [Option<i64>],
+        ends: &mut [Option<i64>],
+        offset: i64,
+        strand: char,
+    ) {
         FiberseqData::apply_offset(starts, offset, strand);
         FiberseqData::apply_offset(ends, offset, strand);
         for (start, end) in starts.iter_mut().zip(ends.iter_mut()) {
             if start > end {
                 std::mem::swap(start, end);
             }
         }
@@ -345,59 +306,72 @@
     }
 
     //
     //  WRITE BED12 FUNCTIONS
     //
     pub fn write_msp(&self, reference: bool) -> String {
         let color = "255,0,255";
-        let starts = self.get_msp(reference, true);
-        let lengths = self.get_msp(reference, false);
-        if starts.is_empty() {
-            return "".to_string();
-        }
-        self.to_bed12(reference, &starts, &lengths, color)
+        let (starts, _ends, lengths) = if reference {
+            (
+                &self.msp.reference_starts,
+                &self.msp.reference_ends,
+                &self.msp.reference_lengths,
+            )
+        } else {
+            (&self.msp.starts, &self.msp.ends, &self.msp.lengths)
+        };
+        self.to_bed12(reference, starts, lengths, color)
     }
 
     pub fn write_nuc(&self, reference: bool) -> String {
         let color = "169,169,169";
-        let starts = self.get_nuc(reference, true);
-        let lengths = self.get_nuc(reference, false);
-        if starts.is_empty() {
-            return "".to_string();
-        }
-        self.to_bed12(reference, &starts, &lengths, color)
+        let (starts, _ends, lengths) = if reference {
+            (
+                &self.nuc.reference_starts,
+                &self.nuc.reference_ends,
+                &self.nuc.reference_lengths,
+            )
+        } else {
+            (&self.nuc.starts, &self.nuc.ends, &self.nuc.lengths)
+        };
+        self.to_bed12(reference, starts, lengths, color)
     }
 
     pub fn write_m6a(&self, reference: bool) -> String {
         let color = "128,0,128";
-        let starts = self.m6a_positions(reference);
-        if starts.is_empty() {
-            return "".to_string();
-        }
-        let lengths = vec![1; starts.len()];
+        let starts = if reference {
+            &self.m6a.reference_starts
+        } else {
+            &self.m6a.starts
+        };
+        let lengths = vec![Some(1); starts.len()];
         self.to_bed12(reference, starts, &lengths, color)
     }
 
     pub fn write_cpg(&self, reference: bool) -> String {
         let color = "139,69,19";
-        let starts = self.cpg_positions(reference);
-        if starts.is_empty() {
-            return "".to_string();
-        }
-        let lengths = vec![1; starts.len()];
+        let starts = if reference {
+            &self.cpg.reference_starts
+        } else {
+            &self.cpg.starts
+        };
+        let lengths = vec![Some(1); starts.len()];
         self.to_bed12(reference, starts, &lengths, color)
     }
 
     pub fn to_bed12(
         &self,
         reference: bool,
-        starts: &[i64],
-        lengths: &[i64],
+        starts: &[Option<i64>],
+        lengths: &[Option<i64>],
         color: &str,
     ) -> String {
+        if starts.is_empty() {
+            return "".to_string();
+        }
         // skip if no alignments are here
         if self.record.is_unmapped() && reference {
             return "".to_string();
         }
 
         let ct;
         let start;
@@ -414,16 +388,16 @@
             end = self.record.seq_len() as i64;
         }
         let score = self.ec.round() as i64;
         let strand = if self.record.is_reverse() { '-' } else { '+' };
         // filter out positions that do not have an exact liftover
         let (filtered_starts, filtered_lengths): (Vec<i64>, Vec<i64>) = starts
             .iter()
-            .zip(lengths.iter())
-            .filter(|(&st, &ln)| st >= 0 && ln >= 0)
+            .flatten()
+            .zip(lengths.iter().flatten())
             .unzip();
         // skip empty ones
         if filtered_lengths.is_empty() || filtered_starts.is_empty() {
             return "".to_string();
         }
         let b_ct = filtered_starts.len() + 2;
         let b_ln: String = filtered_lengths
@@ -529,38 +503,27 @@
             start = self.record.reference_start();
             end = self.record.reference_end();
             strand = if self.record.is_reverse() { '-' } else { '+' };
         }
         let sam_flag = self.record.flags();
         let hp = self.get_hp();
 
-        // fiber features
-        let nuc_starts = self.get_nuc(false, true);
-        let nuc_lengths = self.get_nuc(false, false);
-        let ref_nuc_starts = self.get_nuc(true, true);
-        let ref_nuc_lengths = self.get_nuc(true, false);
-
-        let msp_starts = self.get_msp(false, true);
-        let msp_lengths = self.get_msp(false, false);
-        let ref_msp_starts = self.get_msp(true, true);
-        let ref_msp_lengths = self.get_msp(true, false);
-
         let at_count = self
             .record
             .seq()
             .as_bytes()
             .iter()
             .filter(|&x| *x == b'A' || *x == b'T')
             .count() as i64;
 
         // get the info
         let m6a_count = self.m6a.starts.len();
-        let m6a_qual: Vec<i64> = self.m6a.ml.iter().map(|a| *a as i64).collect();
+        let m6a_qual = self.m6a.ml.iter().map(|a| Some(*a as i64)).collect();
         let cpg_count = self.cpg.starts.len();
-        let cpg_qual: Vec<i64> = self.cpg.ml.iter().map(|a| *a as i64).collect();
+        let cpg_qual = self.cpg.ml.iter().map(|a| Some(*a as i64)).collect();
 
         // write the features
         let mut rtn = String::with_capacity(0);
         // add first things 7
         rtn.write_fmt(format_args!(
             "{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t",
             ct, start, end, name, score, strand, sam_flag, hp, self.rg, q_len
@@ -586,43 +549,50 @@
                         .map(|x| x + 33)
                         .collect::<Vec<u8>>()
                 ),
             ))
             .unwrap();
         }
         // add PB features
-        let total_nuc_bp = nuc_lengths.iter().sum::<i64>();
-        let total_msp_bp = msp_lengths.iter().sum::<i64>();
+        let total_nuc_bp = self.nuc.lengths.iter().flatten().sum::<i64>();
+        let total_msp_bp = self.msp.lengths.iter().flatten().sum::<i64>();
         rtn.write_fmt(format_args!(
             "{}\t{}\t{}\t{}\t{}\t{}\t{}\t",
             self.ec, rq, at_count, m6a_count, total_nuc_bp, total_msp_bp, cpg_count
         ))
         .unwrap();
         // add fiber features
         for vec in &[
-            &nuc_starts,
-            &nuc_lengths,
-            &ref_nuc_starts,
-            &ref_nuc_lengths,
-            &msp_starts,
-            &msp_lengths,
-            &ref_msp_starts,
-            &ref_msp_lengths,
+            &self.nuc.starts,
+            &self.nuc.lengths,
+            &self.nuc.reference_starts,
+            &self.nuc.reference_lengths,
+            &self.msp.starts,
+            &self.msp.lengths,
+            &self.msp.reference_starts,
+            &self.msp.reference_lengths,
             &self.m6a.starts,
             &self.m6a.reference_starts,
             &m6a_qual,
             &self.cpg.starts,
             &self.cpg.reference_starts,
             &cpg_qual,
         ] {
             if vec.is_empty() {
                 rtn.push('.');
                 rtn.push('\t');
             } else {
-                let z: String = vec.iter().map(|&x| x.to_string() + ",").collect();
+                let z: String = vec
+                    .iter()
+                    .map(|x| match x {
+                        Some(y) => *y,
+                        None => -1,
+                    })
+                    .map(|x| x.to_string() + ",")
+                    .collect();
                 rtn.write_fmt(format_args!("{}\t", z)).unwrap();
             }
         }
         // replace the last tab with a newline
         let len = rtn.len();
         rtn.replace_range(len - 1..len, "\n");
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/lib.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,25 @@
 where
     I: IntoIterator<Item = Z>,
     Z: ToString + 'a,
 {
     vals.into_iter().map(|v| v.to_string() + sep).collect()
 }
 
+/// join a vector with commas
+pub fn join_by_str_option(vals: &[Option<i64>], sep: &str) -> String {
+    vals.iter()
+        .map(|v| match v {
+            Some(v) => v.to_string() + sep,
+            None => String::from("NA") + sep,
+        })
+        .map(|v| v + sep)
+        .collect()
+}
+
 pub struct FiberOut {
     pub m6a: Option<Box<dyn Write>>,
     pub cpg: Option<Box<dyn Write>>,
     pub msp: Option<Box<dyn Write>>,
     pub nuc: Option<Box<dyn Write>>,
     pub all: Option<Box<dyn Write>>,
     pub reference: bool,
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/main.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/nucleosomes.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/nucleosomes.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/cnn.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/mod.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/predict_m6a/xgb.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/src/strip_basemods.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/src/strip_basemods.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/all.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/all.bam.bai` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/all.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bam.bai` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bam.bai`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/center.bed` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/center.bed`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 chr1	41417257	41417292	CTCF_XL	3.160000e-11	-	CAGCAGTTTCTGCCGCATGCCACCAGAGGGCACCA
 chr11	44286466	44286501	CTCF_XL	9.450000e-11	+	CTGCAGTTGTGCATGCTGGCCACCAGGAGGCACTG
 chr15	74054174	74054209	CTCF_XL	3.870000e-11	+	AAGCAGTTCCCCCATGTAACCTGCAGGTGGCACCA
 chr13	78121669	78121704	CTCF_XL	2.330000e-11	-	CTGCACTTCTTGTTTGCTGCCAGCAGGGGGAGGTG
 chr1	15323698	15323733	CTCF_XL	4.970000e-11	+	CTGCAGGGTCCTGTAATGGCCAGCAGAGGGCAGCA
 chr1	153568701	153568736	CTCF_XL	4.680000e-11	-	CTGCAATGACACGCCTTAGCCACCAGAGGGCACGA
-#chr7	131689283	131689318	CTCF_XL	8.620000e-11	+	ATGCACTGCTGGGATCTGTCCACCAGAGGGCAGGA
-#chr1	32876798	32876833	CTCF_XL	6.370000e-11	+	CTGCACAGCCTGGGCACAGCCAGCAGAGGGCGCCA
-#chr8	42692645	42692680	CTCF_XL	4.890000e-11	+	CTGCAGTGTGAGGAGTGAGCCACCAGAGGGCACCC
-#chr15	75802259	75802294	CTCF_XL	8.000000e-11	-	AAGCAGTTCCCCCATATAACCTGCAGGTGGCACCA
-#chr15	38440420	38440455	CTCF_XL	9.810000e-12	+	ATGCAGTTCCATCTACAGGCCAGTAGATGGCGCTG
-#chr22	36301453	36301488	CTCF_XL	1.100000e-11	+	ATGCCGTGCCTACCGATGGCCAGCAGGTGGCAGCA
-#chr11	19077152	19077187	CTCF_XL	4.970000e-11	+	CTGCAGTGCTAGGCCTCCTCCACAAGAGGGCGCAC
-#chr4	54234421	54234456	CTCF_XL	8.620000e-11	-	CAGTAGTTCTTACGAGTGGCCAGCAGATGGCAGTG
-#chr14	104896837	104896872	CTCF_XL	9.760000e-11	+	CTGCAATTCAGAGATGCTGCCACCAGGAGGCGGCC
-#chr4	37603163	37603198	CTCF_XL	1.180000e-12	+	GTGCAGTTCTCCGATTCGGCCAGCAGAGGGAGCGA
-#chrX	140766189	140766224	CTCF_XL	1.710000e-11	+	TAGCTGTTCCACGCTGTAGCCAGCAGAGGGCACTG
-#chr3	126522437	126522472	CTCF_XL	5.370000e-11	+	ATGTTATTCCCAACTTTGGCCACCAGGTGGCAGCA
-#chr1	46477574	46477609	CTCF_XL	2.000000e-12	+	GTGCAGTTCTGAGAGCCAGACAGCAGGGGGCGGCC
-#chr22	26360575	26360610	CTCF_XL	4.520000e-11	-	CTGCAGTGCAGAAAAATGACCAGCAGGTGGCAGTG
-#chr10	30392653	30392688	CTCF_XL	4.680000e-11	+	AAGCAGTTCCCCCACATAACCTGCAGGTGGCACCA
-#chr17	60638915	60638950	CTCF_XL	5.750000e-12	-	ATGCAATTCCAGCAGGCAGCCACTAGAGGGCACCT
-#chr1	30719373	30719408	CTCF_XL	4.490000e-14	+	GTGCAGTTCTGCGCTTTGGCCACCAGATGGCAGCC
-#chr12	64802374	64802409	CTCF_XL	4.150000e-11	+	CTGCTGTTACCCGAGATGGCCAGCAGAGGGCAGGC
-#chr13	75695980	75696015	CTCF_XL	6.100000e-12	+	CTGCAGTACTCAGAATGTGCCAGCAGGTGGCAGCA
-#chr17	21280152	21280187	CTCF_XL	6.370000e-11	+	GAGCACTGCCGGGCCCTGGTCACCAGAGGGCGCTG
-#chr1	5510035	5510070	CTCF_XL	2.740000e-11	+	CTGCAGTGTGCAGAACTGGCCACCAGGTGGCAGCA
-#chr15	77959535	77959570	CTCF_XL	8.000000e-11	+	AAGCAGTTCCCCCATATAACCTGCAGGTGGCACCA
-#chr7	19709134	19709169	CTCF_XL	9.760000e-11	+	CTGCATTACGCAGCCCTGACCAGCAGGGGGAACCG
-#chr21	43646828	43646863	CTCF_XL	6.000000e-11	-	CAGCAATGCTCCCATCTGGCCACAAGGTGGCGGCC
-#chr8	22137534	22137569	CTCF_XL	5.950000e-11	-	TTGCACCTCTGAGGAGTGGCCACGAGAGGGCAGCA
-#chr11	15650153	15650188	CTCF_XL	5.560000e-11	+	CTGCAGTTCTCCGCTGCGGACGGTAGGTGGCAGCG
-#chr10	101836140	101836175	CTCF_XL	6.760000e-11	+	CTGCAGTTCTATACAGCCACCACCGGGGGGCACGC
-#chr15	89358745	89358780	CTCF_XL	6.320000e-11	+	CTGCATCTCCCCGGAACGCCCACCAGAGGGCGCTG
-#chr1	27300950	27300985	CTCF_XL	1.370000e-11	+	GTGCAGTTGCACTCTGTGCCCAGCAGAGGGCAGCC
-#chr2	238970654	238970689	CTCF_XL	3.930000e-11	-	CAGCAGTTTCAGGGGTTGGCCACTAGGTGGCAGAG
-#chr2	26469278	26469313	CTCF_XL	2.760000e-11	-	CTGCAATTTTCACAGACTGCCACCAGGTGGCGGTG
-#chr19	18388551	18388586	CTCF_XL	5.240000e-11	+	TTGCACTTGCGGCCGCAAGCCGCCAGGGGGCGCCG
-#chr1	27097569	27097604	CTCF_XL	8.660000e-12	-	GTGCATTTCCTGGATCCAACCACCAGAGGGCAGTG
-#chr10	116788234	116788269	CTCF_XL	3.830000e-11	-	GCGCAGTTCACCAGCTCCACCACCAGAGGGCGGCG
+chr7	131689283	131689318	CTCF_XL	8.620000e-11	+	ATGCACTGCTGGGATCTGTCCACCAGAGGGCAGGA
+chr1	32876798	32876833	CTCF_XL	6.370000e-11	+	CTGCACAGCCTGGGCACAGCCAGCAGAGGGCGCCA
+chr8	42692645	42692680	CTCF_XL	4.890000e-11	+	CTGCAGTGTGAGGAGTGAGCCACCAGAGGGCACCC
+chr15	75802259	75802294	CTCF_XL	8.000000e-11	-	AAGCAGTTCCCCCATATAACCTGCAGGTGGCACCA
+chr15	38440420	38440455	CTCF_XL	9.810000e-12	+	ATGCAGTTCCATCTACAGGCCAGTAGATGGCGCTG
+chr22	36301453	36301488	CTCF_XL	1.100000e-11	+	ATGCCGTGCCTACCGATGGCCAGCAGGTGGCAGCA
+chr11	19077152	19077187	CTCF_XL	4.970000e-11	+	CTGCAGTGCTAGGCCTCCTCCACAAGAGGGCGCAC
+chr4	54234421	54234456	CTCF_XL	8.620000e-11	-	CAGTAGTTCTTACGAGTGGCCAGCAGATGGCAGTG
+chr14	104896837	104896872	CTCF_XL	9.760000e-11	+	CTGCAATTCAGAGATGCTGCCACCAGGAGGCGGCC
+chr4	37603163	37603198	CTCF_XL	1.180000e-12	+	GTGCAGTTCTCCGATTCGGCCAGCAGAGGGAGCGA
+chrX	140766189	140766224	CTCF_XL	1.710000e-11	+	TAGCTGTTCCACGCTGTAGCCAGCAGAGGGCACTG
+chr3	126522437	126522472	CTCF_XL	5.370000e-11	+	ATGTTATTCCCAACTTTGGCCACCAGGTGGCAGCA
+chr1	46477574	46477609	CTCF_XL	2.000000e-12	+	GTGCAGTTCTGAGAGCCAGACAGCAGGGGGCGGCC
+chr22	26360575	26360610	CTCF_XL	4.520000e-11	-	CTGCAGTGCAGAAAAATGACCAGCAGGTGGCAGTG
+chr10	30392653	30392688	CTCF_XL	4.680000e-11	+	AAGCAGTTCCCCCACATAACCTGCAGGTGGCACCA
+chr17	60638915	60638950	CTCF_XL	5.750000e-12	-	ATGCAATTCCAGCAGGCAGCCACTAGAGGGCACCT
+chr1	30719373	30719408	CTCF_XL	4.490000e-14	+	GTGCAGTTCTGCGCTTTGGCCACCAGATGGCAGCC
+chr12	64802374	64802409	CTCF_XL	4.150000e-11	+	CTGCTGTTACCCGAGATGGCCAGCAGAGGGCAGGC
+chr13	75695980	75696015	CTCF_XL	6.100000e-12	+	CTGCAGTACTCAGAATGTGCCAGCAGGTGGCAGCA
+chr17	21280152	21280187	CTCF_XL	6.370000e-11	+	GAGCACTGCCGGGCCCTGGTCACCAGAGGGCGCTG
+chr1	5510035	5510070	CTCF_XL	2.740000e-11	+	CTGCAGTGTGCAGAACTGGCCACCAGGTGGCAGCA
+chr15	77959535	77959570	CTCF_XL	8.000000e-11	+	AAGCAGTTCCCCCATATAACCTGCAGGTGGCACCA
+chr7	19709134	19709169	CTCF_XL	9.760000e-11	+	CTGCATTACGCAGCCCTGACCAGCAGGGGGAACCG
+chr21	43646828	43646863	CTCF_XL	6.000000e-11	-	CAGCAATGCTCCCATCTGGCCACAAGGTGGCGGCC
+chr8	22137534	22137569	CTCF_XL	5.950000e-11	-	TTGCACCTCTGAGGAGTGGCCACGAGAGGGCAGCA
+chr11	15650153	15650188	CTCF_XL	5.560000e-11	+	CTGCAGTTCTCCGCTGCGGACGGTAGGTGGCAGCG
+chr10	101836140	101836175	CTCF_XL	6.760000e-11	+	CTGCAGTTCTATACAGCCACCACCGGGGGGCACGC
+chr15	89358745	89358780	CTCF_XL	6.320000e-11	+	CTGCATCTCCCCGGAACGCCCACCAGAGGGCGCTG
+chr1	27300950	27300985	CTCF_XL	1.370000e-11	+	GTGCAGTTGCACTCTGTGCCCAGCAGAGGGCAGCC
+chr2	238970654	238970689	CTCF_XL	3.930000e-11	-	CAGCAGTTTCAGGGGTTGGCCACTAGGTGGCAGAG
+chr2	26469278	26469313	CTCF_XL	2.760000e-11	-	CTGCAATTTTCACAGACTGCCACCAGGTGGCGGTG
+chr19	18388551	18388586	CTCF_XL	5.240000e-11	+	TTGCACTTGCGGCCGCAAGCCGCCAGGGGGCGCCG
+chr1	27097569	27097604	CTCF_XL	8.660000e-12	-	GTGCATTTCCTGGATCCAACCACCAGAGGGCAGTG
+chr10	116788234	116788269	CTCF_XL	3.830000e-11	-	GCGCAGTTCACCAGCTCCACCACCAGAGGGCGGCG
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/data/msp_nuc.bam`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/extract_test.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/extract_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,47 +9,51 @@
             fiber_data
         })
         .collect::<Vec<_>>()
 }
 
 #[test]
 fn test_msp_extract() -> Result<(), Box<dyn std::error::Error>> {
-    let expected_msp_starts = vec![
+    let expected_msp_starts: Vec<Option<i64>> = vec![
         141, 376, 789, 977, 1112, 1316, 1453, 1691, 1974, 2134, 2283, 2455, 2677, 2784, 2920, 3057,
         3205, 3508, 3729, 4157, 4318, 4583, 4891, 5109, 5322, 5568, 5719, 5901, 6066, 6217, 6383,
         6583, 6727, 6921, 7090, 7276,
-    ];
+    ]
+    .into_iter()
+    .map(Some)
+    .collect();
     let fiber_records = get_fiber_data_from_test_bam("tests/data/msp_nuc.bam");
     assert!(fiber_records.len() == 1);
     let fiber_data = &fiber_records[0];
     assert_eq!(fiber_data.msp.starts, expected_msp_starts);
     Ok(())
 }
 
 #[test]
 fn test_many_msps() {
     let fiber_records = get_fiber_data_from_test_bam("tests/data/all.bam");
     for fiber_data in fiber_records {
-        let m6a = fiber_data.base_mods.m6a_positions(false);
+        let m6a = fiber_data.m6a.starts.iter().flatten().collect::<Vec<_>>();
         if m6a.is_empty() {
             continue;
         }
 
         let msps = fiber_data
             .msp
             .starts
             .iter()
+            .flatten()
             .map(|&x| x)
-            .chain(fiber_data.msp.ends.iter().map(|&x| x - 1))
+            .chain(fiber_data.msp.ends.iter().flatten().map(|&x| x - 1))
             .collect::<Vec<_>>();
         eprintln!("m6a: {:?}", m6a);
         eprintln!("msp: {:?}", msps);
         eprintln!(
             "strand: {:?}\t{:?}",
             fiber_data.record.strand(),
             fiber_data.record.seq_len()
         );
         for msp in msps {
-            assert!(m6a.contains(&msp), "{}", msp);
+            assert!(m6a.contains(&&msp), "{}", msp);
         }
     }
 }
```

### Comparing `pyft-0.1.8/local_dependencies/fibertools-rs/tests/run_test.rs` & `pyft-0.1.9/local_dependencies/fibertools-rs/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/bio-io/Cargo.toml` & `pyft-0.1.9/local_dependencies/bio-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/local_dependencies/bio-io/src/lib.rs` & `pyft-0.1.9/local_dependencies/bio-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/Cargo.toml` & `pyft-0.1.9/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 edition = "2021"
 name = "pyft"
-version = "0.1.8"
+version = "0.1.9"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib"]
 name = "pyft"
 
 [dependencies]
```

### Comparing `pyft-0.1.8/.github/workflows/CI.yml` & `pyft-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/.gitignore` & `pyft-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/docs/Makefile` & `pyft-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/docs/_static/css/rtd_dark.css` & `pyft-0.1.9/docs/_static/css/rtd_dark.css`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/docs/_static/img/fiber_tools_grey.png` & `pyft-0.1.9/docs/_static/img/fiber_tools_grey.png`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/docs/conf.py` & `pyft-0.1.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "sphinx_rtd_theme",
     "sphinx.ext.intersphinx",
     #"edit_on_github",
     "m2r2",
 ]
 
 # source_suffix = '.rst'
-source_suffix = [".rst", ".md"]
+source_suffix = [".rst", ".md", ".py"]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `pyft-0.1.8/docs/index.rst` & `pyft-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/docs/make.bat` & `pyft-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/example.py` & `pyft-0.1.9/example.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,13 +10,12 @@
     fiber.msp.starts
     # print the nuc reference starts
     fiber.nuc.reference_starts
     # lift query (fiber) positions to reference positions
     fiber.lift_query_positions([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
     # lift reference positions to query (fiber) positions
     fiber.lift_reference_positions([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
-    # aligned blocks between query (fiber) and reference 
-    fiber.get_aligned_blocks_as_ranges()
+ 
 
 for fiber in fiberbam.center("chr20", start=20_000_000, end=20_000_001, strand="-"):
-    # returns the same fiber object as above; however, all the positions have been modified to be relative to the region be fetched
-    print(fiber.msp.starts)
+    # returns the same fiber object as above; however, all the positions have been modified to be relative to the region fetched
+    print(fiber.msp.reference_starts)
```

### Comparing `pyft-0.1.8/src/fiberdata.rs` & `pyft-0.1.9/src/fiberdata.rs`

 * *Files 7% similar despite different names*

```diff
@@ -81,33 +81,22 @@
 
     /// return the length of the sequence
     pub fn get_seq_length(&self) -> usize {
         self.seq.len()
     }
 
     /// liftover query (fiber) positions to the reference
-    pub fn lift_query_positions(&self, positions: Vec<i64>) -> Vec<i64> {
+    pub fn lift_query_positions(&self, positions: Vec<i64>) -> Vec<Option<i64>> {
         bamlift::lift_query_positions(&self.aligned_block_pairs, &positions)
     }
 
     /// liftover reference positions to the query (fiber)
-    pub fn lift_reference_positions(&self, positions: Vec<i64>) -> Vec<i64> {
+    pub fn lift_reference_positions(&self, positions: Vec<i64>) -> Vec<Option<i64>> {
         bamlift::lift_reference_positions(&self.aligned_block_pairs, &positions)
     }
-
-    /// Return a :class:`~pyft.Ranges` object for the continuous aligned regions of the fiber
-    pub fn get_aligned_blocks_as_ranges(&self) -> Ranges {
-        let (fiber, genome): (Vec<[i64; 2]>, Vec<[i64; 2]>) =
-            self.aligned_block_pairs.iter().cloned().unzip();
-        let starts = fiber.iter().map(|x| x[0]).collect();
-        let lengths = fiber.iter().map(|x| x[1] - x[0]).collect();
-        let reference_starts = genome.iter().map(|x| x[0]).collect();
-        let reference_lengths = genome.iter().map(|x| x[1] - x[0]).collect();
-        Ranges::new(starts, lengths, reference_starts, reference_lengths)
-    }
 }
 
 impl Fiberdata {
     fn new(fiber: FiberseqData, offset: Option<i64>) -> Self {
         // PB features
         let ec = fiber.ec.round() as i64;
 
@@ -135,18 +124,16 @@
             log::trace!("{f}");
             f
         } else {
             "."
         };
 
         // fiberseq features
-        let m6a = fiber.base_mods.m6a();
-        let m6a = Basemods::new(m6a.0, m6a.1, m6a.2);
-        let cpg = fiber.base_mods.cpg();
-        let cpg = Basemods::new(cpg.0, cpg.1, cpg.2);
+        let m6a = Basemods::new(fiber.m6a.starts, fiber.m6a.reference_starts, fiber.m6a.ml);
+        let cpg = Basemods::new(fiber.cpg.starts, fiber.cpg.reference_starts, fiber.cpg.ml);
 
         let nuc = Ranges {
             starts: fiber.nuc.starts,
             ends: fiber.nuc.ends,
             lengths: fiber.nuc.lengths,
             reference_starts: fiber.nuc.reference_starts,
             reference_ends: fiber.nuc.reference_ends,
@@ -258,19 +245,24 @@
         let position = if strand == '-' { end - 1 } else { start };
         let center_position = fibertools_rs::center::CenterPosition {
             chrom: chrom.to_string(),
             position,
             strand,
         };
         let fiberdata = self._fetch_helper(chrom, Some(position), Some(position + 1));
-        let fibderdata: Vec<FiberseqData> = fiberdata
+        let fiberdata: Vec<FiberseqData> = fiberdata
             .into_iter()
             .filter_map(|fiber| fiber.center(&center_position))
             .collect();
-        Fiberiter::build_fiberdata_iter(fibderdata)
+        log::info!(
+            "Fiberdata centered for {} records in {:.2}s",
+            fiberdata.len(),
+            self._time_from_last()
+        );
+        Fiberiter::build_fiberdata_iter(fiberdata)
     }
 
     fn _time_from_last(&mut self) -> f64 {
         let elapsed = self.start.elapsed().as_secs_f64();
         self.start = time::Instant::now();
         elapsed
     }
@@ -320,27 +312,27 @@
 /// Class for describing base modifications within fiberseq data.
 /// For example, m6a and 5mC (cpg) features.
 #[pyclass]
 #[derive(Clone)]
 pub struct Basemods {
     /// Basemod starts
     #[pyo3(get, set)]
-    pub starts: Vec<i64>,
+    pub starts: Vec<Option<i64>>,
     /// Basemod reference starts
     #[pyo3(get, set)]
-    pub reference_starts: Vec<i64>,
+    pub reference_starts: Vec<Option<i64>>,
     /// Basemod ML
     #[pyo3(get, set)]
     pub ml: Vec<u8>,
 }
 
 #[pymethods]
 impl Basemods {
     #[new]
-    pub fn new(starts: Vec<i64>, reference_starts: Vec<i64>, ml: Vec<u8>) -> Self {
+    pub fn new(starts: Vec<Option<i64>>, reference_starts: Vec<Option<i64>>, ml: Vec<u8>) -> Self {
         Self {
             starts,
             reference_starts,
             ml,
         }
     }
 }
@@ -348,50 +340,56 @@
 /// Class for describing ranges within fiberseq data.
 /// For example, nucleosomes and msp features.
 #[pyclass]
 #[derive(Clone)]
 pub struct Ranges {
     /// Range starts
     #[pyo3(get, set)]
-    pub starts: Vec<i64>,
+    pub starts: Vec<Option<i64>>,
     /// Range ends
     #[pyo3(get, set)]
-    pub ends: Vec<i64>,
+    pub ends: Vec<Option<i64>>,
     /// Range lengths
     #[pyo3(get, set)]
-    pub lengths: Vec<i64>,
+    pub lengths: Vec<Option<i64>>,
     /// Reference starts
     #[pyo3(get, set)]
-    pub reference_starts: Vec<i64>,
+    pub reference_starts: Vec<Option<i64>>,
     /// Reference ends
     #[pyo3(get, set)]
-    pub reference_ends: Vec<i64>,
+    pub reference_ends: Vec<Option<i64>>,
     /// Reference lengths
     #[pyo3(get, set)]
-    pub reference_lengths: Vec<i64>,
+    pub reference_lengths: Vec<Option<i64>>,
 }
 
 #[pymethods]
 impl Ranges {
     #[new]
     pub fn new(
-        starts: Vec<i64>,
-        lengths: Vec<i64>,
-        reference_starts: Vec<i64>,
-        reference_lengths: Vec<i64>,
+        starts: Vec<Option<i64>>,
+        lengths: Vec<Option<i64>>,
+        reference_starts: Vec<Option<i64>>,
+        reference_lengths: Vec<Option<i64>>,
     ) -> Self {
         let ends = starts
             .iter()
             .zip(lengths.iter())
-            .map(|(s, l)| s + l)
+            .map(|(s, l)| match (s, l) {
+                (Some(s), Some(l)) => Some(s + l),
+                _ => None,
+            })
             .collect();
         let reference_ends = reference_starts
             .iter()
             .zip(reference_lengths.iter())
-            .map(|(s, l)| s + l)
+            .map(|(s, l)| match (s, l) {
+                (Some(s), Some(l)) => Some(s + l),
+                _ => None,
+            })
             .collect();
         Self {
             starts,
             ends,
             lengths,
             reference_starts,
             reference_ends,
```

### Comparing `pyft-0.1.8/src/lib.rs` & `pyft-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyft-0.1.8/Cargo.lock` & `pyft-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1198,15 +1198,15 @@
 checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyft"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anyhow",
  "bamlift",
  "bio-io",
  "colored",
  "env_logger 0.10.0",
  "fibertools-rs",
```

### Comparing `pyft-0.1.8/PKG-INFO` & `pyft-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyft
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # pyft: python bindings for fibertools-rs
```

