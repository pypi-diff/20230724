# Comparing `tmp/mgtron-2.20.0.tar.gz` & `tmp/mgtron-2.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.20.0.tar", last modified: Thu Jul 13 17:43:10 2023, max compression
+gzip compressed data, was "mgtron-2.21.0.tar", last modified: Mon Jul 24 17:47:27 2023, max compression
```

## Comparing `mgtron-2.20.0.tar` & `mgtron-2.21.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.724422 mgtron-2.20.0/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.20.0/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.20.0/.github/workflows/pypi_action.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      409 2023-07-13 17:42:32.000000 mgtron-2.20.0/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9474 2023-07-13 17:42:32.000000 mgtron-2.20.0/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.20.0/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-13 17:43:10.724422 mgtron-2.20.0/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.20.0/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.20.0/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.20.0/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.701088 mgtron-2.20.0/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2376 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-13 17:43:10.000000 mgtron-2.20.0/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.20.0/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.20.0/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-13 17:43:10.724422 mgtron-2.20.0/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.701088 mgtron-2.20.0/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.20.0/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.707754 mgtron-2.20.0/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/CA_subheading.png
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)   141680 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/assets/MGTron Command Description.pdf
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/init_cellantenna.sh
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/log_read
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/assets/network-wireless.ico
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/assets/wifi_rs
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.714421 mgtron-2.20.0/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/ble/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.20.0/src/ble/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10863 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/db/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-13 17:23:31.000000 mgtron-2.20.0/src/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9064 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/globals/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/globals/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/globals/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.717755 mgtron-2.20.0/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.20.0/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    51305 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10946 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43803 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.20.0/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19802 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.721088 mgtron-2.20.0/src/wifi/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.20.0/src/wifi/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.20.0/src/wifi/chasing.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17393 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/wifi/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9518 2023-07-13 17:42:32.000000 mgtron-2.20.0/src/wifi/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.697754 mgtron-2.20.0/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 17:43:10.724422 mgtron-2.20.0/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.20.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.398000 mgtron-2.21.0/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.371333 mgtron-2.21.0/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.371333 mgtron-2.21.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.21.0/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.21.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.371333 mgtron-2.21.0/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.21.0/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      834 2023-07-24 14:32:37.000000 mgtron-2.21.0/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      409 2023-07-13 17:42:32.000000 mgtron-2.21.0/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9474 2023-07-13 17:42:32.000000 mgtron-2.21.0/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.21.0/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4223 2023-07-24 17:47:27.398000 mgtron-2.21.0/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3724 2023-07-18 14:31:35.000000 mgtron-2.21.0/README.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      315 2023-07-18 14:31:35.000000 mgtron-2.21.0/SECURITY.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.371333 mgtron-2.21.0/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.21.0/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.21.0/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.374667 mgtron-2.21.0/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4223 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2388 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-24 17:47:27.000000 mgtron-2.21.0/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.21.0/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-18 14:31:35.000000 mgtron-2.21.0/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-24 17:47:27.398000 mgtron-2.21.0/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.374667 mgtron-2.21.0/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.21.0/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.381333 mgtron-2.21.0/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/CA_subheading.png
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)   141680 2023-07-13 17:42:32.000000 mgtron-2.21.0/src/assets/MGTron Command Description.pdf
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.21.0/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/init_cellantenna.sh
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.21.0/src/assets/log_read
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/assets/network-wireless.ico
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.21.0/src/assets/wifi_rs
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.388000 mgtron-2.21.0/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3503 2023-07-24 17:46:16.000000 mgtron-2.21.0/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8408 2023-07-24 17:46:16.000000 mgtron-2.21.0/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.21.0/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.391334 mgtron-2.21.0/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10863 2023-07-13 17:42:32.000000 mgtron-2.21.0/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-13 17:23:31.000000 mgtron-2.21.0/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9064 2023-07-13 17:42:32.000000 mgtron-2.21.0/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.391334 mgtron-2.21.0/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-19 18:13:09.000000 mgtron-2.21.0/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.391334 mgtron-2.21.0/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.391334 mgtron-2.21.0/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      147 2023-07-24 14:03:49.000000 mgtron-2.21.0/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.394667 mgtron-2.21.0/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    51305 2023-07-24 17:46:13.000000 mgtron-2.21.0/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10946 2023-07-24 17:46:13.000000 mgtron-2.21.0/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43813 2023-07-24 17:46:16.000000 mgtron-2.21.0/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.394667 mgtron-2.21.0/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.21.0/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19802 2023-07-14 18:23:12.000000 mgtron-2.21.0/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.394667 mgtron-2.21.0/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.21.0/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.21.0/src/wifi/chasing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17393 2023-07-24 14:32:37.000000 mgtron-2.21.0/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9518 2023-07-24 14:32:37.000000 mgtron-2.21.0/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.371333 mgtron-2.21.0/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-24 17:47:27.398000 mgtron-2.21.0/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.21.0/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.21.0/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.21.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/.github/workflows/black_actions.yml` & `mgtron-2.21.0/.github/workflows/black_actions.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/.github/workflows/pypi_action.yml` & `mgtron-2.21.0/.github/workflows/pypi_action.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,13 @@
       - name: "Build and publish"
         run: |
           python -m build
       - name: "Publish to PyPI"
         uses: pypa/gh-action-pypi-publish@master
         with:
           user: __token__
-          password: ${{ secrets.PYPI_TOKEN }}
+          password: ${{ secrets.PYPI_API_TOKEN }}
           url: https://pypi.org/project/mgtron/
```

### Comparing `mgtron-2.20.0/CHANGELOG.md` & `mgtron-2.21.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/LICENSE.rst` & `mgtron-2.21.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/PKG-INFO` & `mgtron-2.21.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.20.0
+Version: 2.21.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -37,14 +37,21 @@
 
 ## Visualization
 
 ![mgtron_demo](https://user-images.githubusercontent.com/25860608/174464184-1511b551-a6ca-4b74-84f8-aeec5d31d9a4.gif)
 
 ## Installation
 
+### Permissions
+- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
+* `sudo chmod 777 /dev/ttyACM*` - temporary and **UNSAFE** fix
+* `sudo usermod -a -G dialout $USER` - permanent fix; **reboot required**
+* `sudo usermod -a -G uucp $USER` - permanent fix; **reboot required**
+
+
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
@@ -54,19 +61,14 @@
 
 `pip install mgtron`
 
 `mgtron`
 
 ## Known Issues
 
-### Permissions
-- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
-* `sudo chmod 777 /dev/ttyACM*` - temporary fix
-* `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
-* `sudo usermod -a -G uucp $USER` - permanent fix; reboot required
 
 * Version
   * `Update to Python3.10`
 
 ### GUI never launches
 * The Teensy is not properly initialized. This appears to happen randomly in testing.  The solution is to power cycle the Teensy.  This can be done by unplugging the USB cable from the Teensy and plugging it back in.  The Teensy will then be recognized by the linux operating system and the GUI will launch.
 * There is no Teensy
```

### Comparing `mgtron-2.20.0/README.md` & `mgtron-2.21.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 
 ## Visualization
 
 ![mgtron_demo](https://user-images.githubusercontent.com/25860608/174464184-1511b551-a6ca-4b74-84f8-aeec5d31d9a4.gif)
 
 ## Installation
 
+### Permissions
+- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
+* `sudo chmod 777 /dev/ttyACM*` - temporary and **UNSAFE** fix
+* `sudo usermod -a -G dialout $USER` - permanent fix; **reboot required**
+* `sudo usermod -a -G uucp $USER` - permanent fix; **reboot required**
+
+
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
@@ -40,19 +47,14 @@
 
 `pip install mgtron`
 
 `mgtron`
 
 ## Known Issues
 
-### Permissions
-- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
-* `sudo chmod 777 /dev/ttyACM*` - temporary fix
-* `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
-* `sudo usermod -a -G uucp $USER` - permanent fix; reboot required
 
 * Version
   * `Update to Python3.10`
 
 ### GUI never launches
 * The Teensy is not properly initialized. This appears to happen randomly in testing.  The solution is to power cycle the Teensy.  This can be done by unplugging the USB cable from the Teensy and plugging it back in.  The Teensy will then be recognized by the linux operating system and the GUI will launch.
 * There is no Teensy
```

### Comparing `mgtron-2.20.0/docs/MGTron Command Description.docx` & `mgtron-2.21.0/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/docs/MGTron Function Descriptions.docx` & `mgtron-2.21.0/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/mgtron.egg-info/PKG-INFO` & `mgtron-2.21.0/mgtron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.20.0
+Version: 2.21.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -37,14 +37,21 @@
 
 ## Visualization
 
 ![mgtron_demo](https://user-images.githubusercontent.com/25860608/174464184-1511b551-a6ca-4b74-84f8-aeec5d31d9a4.gif)
 
 ## Installation
 
+### Permissions
+- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
+* `sudo chmod 777 /dev/ttyACM*` - temporary and **UNSAFE** fix
+* `sudo usermod -a -G dialout $USER` - permanent fix; **reboot required**
+* `sudo usermod -a -G uucp $USER` - permanent fix; **reboot required**
+
+
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
@@ -54,19 +61,14 @@
 
 `pip install mgtron`
 
 `mgtron`
 
 ## Known Issues
 
-### Permissions
-- Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
-* `sudo chmod 777 /dev/ttyACM*` - temporary fix
-* `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
-* `sudo usermod -a -G uucp $USER` - permanent fix; reboot required
 
 * Version
   * `Update to Python3.10`
 
 ### GUI never launches
 * The Teensy is not properly initialized. This appears to happen randomly in testing.  The solution is to power cycle the Teensy.  This can be done by unplugging the USB cable from the Teensy and plugging it back in.  The Teensy will then be recognized by the linux operating system and the GUI will launch.
 * There is no Teensy
```

### Comparing `mgtron-2.20.0/mgtron.egg-info/SOURCES.txt` & `mgtron-2.21.0/mgtron.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 CHANGELOG.md
 LICENSE.rst
 README.md
+SECURITY.md
 pyproject.toml
 requirements.txt
 .github/ISSUE_TEMPLATE/mgtron--.md
 .github/ISSUE_TEMPLATE/mgtron_issue.yml
 .github/workflows/black_actions.yml
 .github/workflows/pypi_action.yml
 docs/MGTron Command Description.docx
```

### Comparing `mgtron-2.20.0/mgtron.egg-info/requires.txt` & `mgtron-2.21.0/mgtron.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
-cryptography==41.0.1
+cryptography==41.0.2
 dearpygui==1.9.1
 debugpy==1.6.7
 dill==0.3.6
 distlib==0.3.6
 docstring-to-markdown==0.12
 docutils==0.20.1
 editables==0.3
```

### Comparing `mgtron-2.20.0/pyproject.toml` & `mgtron-2.21.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/requirements.txt` & `mgtron-2.21.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
-cryptography==41.0.1
+cryptography==41.0.2
 dearpygui==1.9.1
 debugpy==1.6.7
 dill==0.3.6
 distlib==0.3.6
 docstring-to-markdown==0.12
 docutils==0.20.1
 editables==0.3
```

### Comparing `mgtron-2.20.0/src/assets/CA logo without subtext.JPG` & `mgtron-2.21.0/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/CA_subheading.png` & `mgtron-2.21.0/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/MGTron Command Description.pdf` & `mgtron-2.21.0/src/assets/MGTron Command Description.pdf`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/blueio_rs` & `mgtron-2.21.0/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/init_cellantenna.sh` & `mgtron-2.21.0/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/log_read` & `mgtron-2.21.0/src/assets/log_read`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/mgtron.svg` & `mgtron-2.21.0/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/network-wireless.ico` & `mgtron-2.21.0/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/assets/wifi_rs` & `mgtron-2.21.0/src/assets/wifi_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/ble/ble_data.py` & `mgtron-2.21.0/src/ble/ble_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,50 +53,64 @@
     """Scan for BLE signals and frequencies in a thread."""
     loggei.debug(msg=f"{threaded_scan.__name__}()")
 
     dpg.configure_item(
         item="12",
         modal=True,
     )
-
-    dpg.add_text(
-        tag="scan_text",
-        default_value="Scanning"
+    dpg.configure_item(
+        item="ble_list",
+        width=880,
+        height=680,
     )
 
     dpg.add_text(
-        tag="scan_text_",
-        default_value='-' * 89
+        tag="scan_text",
+        default_value="SCANNING",
+        pos=(400, 265)
     )
 
     ble = ThreadWithReturnValue(
         target=ble_data,
         args=(company[0],)
     )
     ble.start()
 
     ble_rssi = ThreadWithReturnValue(
         target=ble_data,
         args=(company[1],)
     )
+    sleep_delay: float = 0.5
 
-    for i in range(1, 7):
-        time.sleep(1)
+    count = 0
+
+    while ble.is_alive():
+        time.sleep(sleep_delay)
+        count += 1
         dpg.configure_item(
             item="scan_text",
-            default_value="Scanning" + "." * i
+            default_value="SCANNING" + "." * count
         )
+        count = 0 if count > 3 else count
+    count = 0
 
     ble_rssi.start()
 
+    while ble_rssi.is_alive():
+        time.sleep(sleep_delay)
+        count += 1
+        dpg.configure_item(
+            item="scan_text",
+            default_value="SCANNING" + "." * count
+        )
+        count = 0 if count > 3 else count
     ble = ble.join()
     ble_rssi = ble_rssi.join()
 
     dpg.delete_item(item="scan_text")
-    dpg.delete_item(item="scan_text_")
 
     dpg.configure_item(
         item="12",
         modal=False,
     )
 
     return ble, ble_rssi
```

### Comparing `mgtron-2.20.0/src/ble/helpers.py` & `mgtron-2.21.0/src/ble/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Make remote API calls to find Bluetooth device names."""
 
 
+from ..globals.helpers import BLE_BTNS_LIST
+from ..globals.helpers import enable_select_btns
+from ..globals.helpers import disble_select_btns
+from .ble_data import ble_data_complete
+import dearpygui.dearpygui as dpg
+from colorama import Fore as F
+from decouple import config
 from datetime import datetime
 from typing import Callable
 
 import json
 import time
 import logging
 import requests
-import tabulate 
+import tabulate
 tabulate.PRESERVE_WHITESPACE = True
-from decouple import config
-
-from colorama import Fore as F
-
-import dearpygui.dearpygui as dpg
-
-from .ble_data import ble_data_complete
-from ..globals.helpers import disble_select_btns
-
-from ..globals.helpers import enable_select_btns
-from ..globals.helpers import BLE_BTNS_LIST
 
 
 loggei = logging.getLogger(name=__name__)
 
 R = F.RESET
 
 
@@ -75,15 +71,15 @@
             dpg.bind_item_theme(
                 item="mssn_bluetooth_scan",
                 theme=blue_btn_theme,
             )
 
             dpg.configure_item(
                 item=sender,
-                label="  BLUETOOTH\n   SCAN",
+                label=" TRACKER \n   TAG",
             )
             loggei.debug(msg="Bluetooth scan button disabled")
 
             # Delete the open bluetooth scan window
             dpg.delete_item(item="12")
             loggei.debug(msg="Bluetooth scan window deleted")
 
@@ -95,47 +91,30 @@
             # Launch the window that will show the bluetooth information
             dpg.bind_item_theme(
                 item=sender,
                 theme=orng_btn_theme,
             )
             dpg.configure_item(
                 item=sender,
-                label="  BLUETOOTH\n   SCAN",
+                label=" TRACKER \n   TAG",
             )
             loggei.debug(msg="Bluetooth scan button enabled")
 
             with dpg.window(
                 tag="12",
                 no_scrollbar=True,
                 no_collapse=True,
                 no_resize=True,
                 no_title_bar=True,
                 no_move=True,
                 pos=(0, 0),
                 width=880,
-                height=735,
+                height=720,
             ):
                 with dpg.child_window(
-                    tag="ble_labels",
-                    pos=(0, 0),
-                    width=880,
-                    height=715,
-                ):
-                    dpg.add_text(
-                        default_value=" " * 7 + "MAC" + " " * 7 + "|" +
-                        " " * 4 +
-                        "MANUFACTURER" + " " * 3 + "|" + " " +
-                        "RSSI" + " "  + "|" + " " * 2 + "DATE",
-                        label="BLUETOOTH LIST",
-                    )
-                    dpg.add_text(
-                        default_value='-'*89
-                    )
-
-                with dpg.child_window(
                     tag="ble_list",
                     no_scrollbar=False,
                     pos=(0, 60),
                     width=880,
                     height=680,
                 ):
 
@@ -157,19 +136,32 @@
                             i[0] += " " * mac_diff
                         dpg.add_text(
                             # tag=i[1],  # Causes issue on re-scan
                             default_value=tabulate.tabulate(
                                 [i],
                                 stralign="left",
                                 tablefmt="plain",
-                                ),
+                            ),
                         )
                         dpg.add_text(
                             default_value=" "
                         )
+                with dpg.child_window(
+                    tag="ble_labels",
+                    pos=(0, 0),
+                    width=880,
+                    height=55,
+                ):
+                    dpg.add_text(
+                        default_value=" " * 7 + "MAC" + " " * 7 + "|" +
+                        " " * 4 +
+                        "MANUFACTURER" + " " * 3 + "|" + " " +
+                        "RSSI" + " " + "|" + " " * 2 + "DATE",
+                        label="BLUETOOTH LIST",
+                    )
 
     except SystemError:
         loggei.error(msg="Bluetooth scan window not found")
         return
 
 
 def bluetooth_defeat(callstack_helper: Callable[[int,], None]) -> None:
```

### Comparing `mgtron-2.20.0/src/ble/scanning.py` & `mgtron-2.21.0/src/ble/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/helpers.py` & `mgtron-2.21.0/src/db/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/init_db.sql` & `mgtron-2.21.0/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/long_save.json` & `mgtron-2.21.0/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/mgtron_db.db` & `mgtron-2.21.0/src/db/mgtron_db.db`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/models.py` & `mgtron-2.21.0/src/db/models.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/db/quick_save.json` & `mgtron-2.21.0/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/globals/helpers.py` & `mgtron-2.21.0/src/globals/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.21.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.21.0/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.21.0/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/gui/helpers.py` & `mgtron-2.21.0/src/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/gui/interface.py` & `mgtron-2.21.0/src/gui/interface.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/main.py` & `mgtron-2.21.0/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,15 +941,15 @@
                     ###############
                     # Tracker Tag #
                     ###############
                     logger.info(msg="Bluetooth scan button initialized")
                     mission_golf_button = dpg.add_button(
                         tag="mssn_bluetooth_scan",
                         callback=bluetooth_scan_jam,
-                        label="BLE TAG",
+                        label=" TRACKER \n   TAG",
                         height=70,
                         width=BUTTON_WIDTH,
                         pos=(
                             (
                                 dpg.get_item_width(item="big_buttons") - 285) /
                             DIVISOR,
                             (
```

### Comparing `mgtron-2.20.0/src/tests/test_configfiles.py` & `mgtron-2.21.0/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/tests/test_helpers.py` & `mgtron-2.21.0/src/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/wifi/helpers.py` & `mgtron-2.21.0/src/wifi/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/src/wifi/scanning.py` & `mgtron-2.21.0/src/wifi/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2html.py` & `mgtron-2.21.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2html4.py` & `mgtron-2.21.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2html5.py` & `mgtron-2.21.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2latex.py` & `mgtron-2.21.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2man.py` & `mgtron-2.21.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2odt.py` & `mgtron-2.21.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.21.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2pseudoxml.py` & `mgtron-2.21.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2s5.py` & `mgtron-2.21.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2xetex.py` & `mgtron-2.21.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rst2xml.py` & `mgtron-2.21.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.20.0/venv/bin/rstpep2html.py` & `mgtron-2.21.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

