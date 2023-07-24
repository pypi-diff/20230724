# Comparing `tmp/Cactool-0.6.0.tar.gz` & `tmp/Cactool-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cactool-0.6.0.tar", last modified: Sat Jul  1 00:15:11 2023, max compression
+gzip compressed data, was "Cactool-0.6.1.tar", last modified: Mon Jul 24 00:18:46 2023, max compression
```

## Comparing `Cactool-0.6.0.tar` & `Cactool-0.6.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.745362 Cactool-0.6.0/Cactool.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     6047 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       44 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      142 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        8 2023-07-01 00:15:11.000000 Cactool-0.6.0/Cactool.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)     1093 2022-05-11 16:09:13.000000 Cactool-0.6.0/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-01 00:15:11.785363 Cactool-0.6.0/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     6821 2023-06-30 00:04:08.000000 Cactool-0.6.0/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.748696 Cactool-0.6.0/cactool/
--rw-r--r--   0 sam       (1000) sam       (1000)     4631 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       91 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)    11482 2023-01-13 15:13:46.000000 Cactool-0.6.0/cactool/database.py
--rw-r--r--   0 sam       (1000) sam       (1000)      102 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/dates.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.748696 Cactool-0.6.0/cactool/defaults/
--rw-r--r--   0 sam       (1000) sam       (1000)      365 2023-03-01 20:55:20.000000 Cactool-0.6.0/cactool/defaults/config.json
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.752029 Cactool-0.6.0/cactool/migrations/
--rw-r--r--   0 sam       (1000) sam       (1000)       41 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/migrations/README
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.752029 Cactool-0.6.0/cactool/migrations/__pycache__/
--rw-r--r--   0 sam       (1000) sam       (1000)     2254 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     4001 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      832 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/alembic.ini
--rw-r--r--   0 sam       (1000) sam       (1000)     2745 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/env.py
--rw-r--r--   0 sam       (1000) sam       (1000)      494 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/migrations/script.py.mako
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.755362 Cactool-0.6.0/cactool/migrations/versions/
--rw-r--r--   0 sam       (1000) sam       (1000)      592 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/07c0c9849f18_store_user_otp_secret.py
--rw-r--r--   0 sam       (1000) sam       (1000)      952 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/versions/07d73859b99c_add_show_data_type.py
--rw-r--r--   0 sam       (1000) sam       (1000)      822 2022-12-19 20:19:53.000000 Cactool-0.6.0/cactool/migrations/versions/16942fdb0f18_add_relative_column_priorities.py
--rw-r--r--   0 sam       (1000) sam       (1000)      709 2023-01-13 15:21:55.000000 Cactool-0.6.0/cactool/migrations/versions/19d06323ddd6_store_dataset_access_ranes.py
--rw-r--r--   0 sam       (1000) sam       (1000)      763 2023-01-12 00:42:42.000000 Cactool-0.6.0/cactool/migrations/versions/28e8811a530d_support_dataset_file_storage.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1269 2023-01-02 05:22:05.000000 Cactool-0.6.0/cactool/migrations/versions/51ed49d3ed75_support_user_email_verification.py
--rw-r--r--   0 sam       (1000) sam       (1000)      938 2022-12-19 20:19:53.000000 Cactool-0.6.0/cactool/migrations/versions/5e7f3be664d5_rename_priority_column_to_order.py
--rw-r--r--   0 sam       (1000) sam       (1000)      380 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/migrations/versions/6286ef6698f9_merge_heads.py
--rw-r--r--   0 sam       (1000) sam       (1000)      885 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.768696 Cactool-0.6.0/cactool/migrations/versions/__pycache__/
--rw-r--r--   0 sam       (1000) sam       (1000)     1064 2022-11-12 14:02:05.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/072331977abf_store_user_emails.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      966 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1133 2022-11-17 22:52:32.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1026 2023-01-10 17:45:24.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/0f3a32ab3b24_support_dataset_files.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      946 2022-12-11 16:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      993 2023-01-01 23:29:37.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1644 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1005 2023-01-13 14:54:14.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1051 2023-01-22 14:51:47.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1888 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1092 2023-01-10 17:39:40.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/25345a0b177f_make_datasetfile_file_names_part_of_the_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1032 2023-01-13 14:54:14.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1594 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1299 2023-01-07 09:30:57.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     2396 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      922 2022-11-12 13:57:50.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5ab489444dcc_store_user_emails.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      986 2023-01-01 23:29:37.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1882 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      686 2022-11-13 17:44:58.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      695 2022-11-17 22:52:32.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1124 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1579 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      937 2022-11-12 15:14:52.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/727b95af4b5f_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1242 2023-01-02 05:07:03.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c0ed5c0ee030_.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      972 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1628 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1154 2023-01-10 10:50:03.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     3000 2022-11-13 17:39:31.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-310.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)     8379 2023-06-30 00:02:56.000000 Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-311.pyc
--rw-r--r--   0 sam       (1000) sam       (1000)      587 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/c12d86b089b8_store_user_emails.py
--rw-r--r--   0 sam       (1000) sam       (1000)      982 2023-01-07 10:01:34.000000 Cactool-0.6.0/cactool/migrations/versions/ce5fc447a2e8_add_image_display_type.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5807 2022-11-13 17:39:27.000000 Cactool-0.6.0/cactool/migrations/versions/d1b66364eeb3_initial_migration.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.768696 Cactool-0.6.0/cactool/scripts/
--rwxr-xr-x   0 sam       (1000) sam       (1000)       50 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/debug.sh
--rwxr-xr-x   0 sam       (1000) sam       (1000)       92 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/delete-database.sh
--rw-r--r--   0 sam       (1000) sam       (1000)      209 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/get-port.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)      323 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/scripts/update.sh
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.745362 Cactool-0.6.0/cactool/static/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.772029 Cactool-0.6.0/cactool/static/assets/
--rw-r--r--   0 sam       (1000) sam       (1000)   162190 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/static/assets/404Error.png
--rw-r--r--   0 sam       (1000) sam       (1000)   161280 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/static/assets/StrangeError.png
--rw-r--r--   0 sam       (1000) sam       (1000)    96984 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/assets/cactool-large.png
--rw-r--r--   0 sam       (1000) sam       (1000)    15406 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/assets/favicon.ico
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.772029 Cactool-0.6.0/cactool/static/bin/
--rw-r--r--   0 sam       (1000) sam       (1000)    15593 2022-05-14 10:36:35.000000 Cactool-0.6.0/cactool/static/bin/instagram_embed.js
--rw-r--r--   0 sam       (1000) sam       (1000)    47547 2023-01-07 09:19:40.000000 Cactool-0.6.0/cactool/static/bin/tiktok_embed.js
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.775363 Cactool-0.6.0/cactool/static/css/
--rw-r--r--   0 sam       (1000) sam       (1000)    95609 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/bootstrap-icons.css
--rw-r--r--   0 sam       (1000) sam       (1000)   194901 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/bootstrap.css
--rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-02-28 15:07:32.000000 Cactool-0.6.0/cactool/static/css/cactool.css
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.775363 Cactool-0.6.0/cactool/static/css/fonts/
--rw-r--r--   0 sam       (1000) sam       (1000)   121296 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 sam       (1000) sam       (1000)     1508 2022-12-20 02:32:09.000000 Cactool-0.6.0/cactool/static/css/login.css
--rw-r--r--   0 sam       (1000) sam       (1000)      130 2022-12-20 02:57:30.000000 Cactool-0.6.0/cactool/static/css/projects.css
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.778696 Cactool-0.6.0/cactool/static/js/
--rw-r--r--   0 sam       (1000) sam       (1000)    80496 2022-11-17 22:51:58.000000 Cactool-0.6.0/cactool/static/js/bootstrap.js
--rw-r--r--   0 sam       (1000) sam       (1000)    10545 2023-01-17 13:21:52.000000 Cactool-0.6.0/cactool/static/js/code.js
--rw-r--r--   0 sam       (1000) sam       (1000)      428 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/static/js/twitter.js
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/cactool/templates/
--rw-r--r--   0 sam       (1000) sam       (1000)      838 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/templates/404.html
--rw-r--r--   0 sam       (1000) sam       (1000)     3113 2022-12-20 03:07:40.000000 Cactool-0.6.0/cactool/templates/add_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)      445 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/templates/card.html
--rw-r--r--   0 sam       (1000) sam       (1000)     4581 2023-02-28 15:09:22.000000 Cactool-0.6.0/cactool/templates/code_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2121 2023-01-02 14:21:53.000000 Cactool-0.6.0/cactool/templates/coding_interface.html
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/contact.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1491 2022-12-20 02:57:47.000000 Cactool-0.6.0/cactool/templates/create_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2727 2022-12-20 02:38:15.000000 Cactool-0.6.0/cactool/templates/dashboard.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1583 2022-12-20 02:42:07.000000 Cactool-0.6.0/cactool/templates/delete_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1463 2022-12-20 03:06:04.000000 Cactool-0.6.0/cactool/templates/delete_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1268 2023-06-30 00:04:08.000000 Cactool-0.6.0/cactool/templates/error.html
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/faq.html
--rw-r--r--   0 sam       (1000) sam       (1000)      615 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/templates/flash.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2067 2022-12-20 02:39:33.000000 Cactool-0.6.0/cactool/templates/import_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2349 2022-12-20 03:04:09.000000 Cactool-0.6.0/cactool/templates/index.html
--rw-r--r--   0 sam       (1000) sam       (1000)     6812 2022-05-28 12:15:27.000000 Cactool-0.6.0/cactool/templates/instagram_embed.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1947 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/login.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1847 2023-01-10 12:22:56.000000 Cactool-0.6.0/cactool/templates/macros.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2046 2022-12-19 20:19:56.000000 Cactool-0.6.0/cactool/templates/navigation.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1541 2022-12-20 02:59:07.000000 Cactool-0.6.0/cactool/templates/setup_2fa.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1634 2022-12-20 03:07:12.000000 Cactool-0.6.0/cactool/templates/show_datasets.html
--rw-r--r--   0 sam       (1000) sam       (1000)     4580 2022-12-20 02:59:18.000000 Cactool-0.6.0/cactool/templates/signup.html
--rw-r--r--   0 sam       (1000) sam       (1000)      209 2023-01-07 09:19:00.000000 Cactool-0.6.0/cactool/templates/tiktok_embed.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1545 2023-01-12 01:15:17.000000 Cactool-0.6.0/cactool/templates/upload_images.html
--rw-r--r--   0 sam       (1000) sam       (1000)     1488 2022-12-20 03:08:13.000000 Cactool-0.6.0/cactool/templates/verify_2fa.html
--rw-r--r--   0 sam       (1000) sam       (1000)     6815 2023-02-28 15:19:51.000000 Cactool-0.6.0/cactool/templates/view_dataset.html
--rw-r--r--   0 sam       (1000) sam       (1000)     2401 2022-12-20 03:07:59.000000 Cactool-0.6.0/cactool/templates/view_project.html
--rw-r--r--   0 sam       (1000) sam       (1000)      847 2023-01-07 09:58:35.000000 Cactool-0.6.0/cactool/types.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-01 00:15:11.785363 Cactool-0.6.0/cactool/views/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-05-11 16:09:13.000000 Cactool-0.6.0/cactool/views/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8334 2023-01-22 15:00:13.000000 Cactool-0.6.0/cactool/views/authentication.py
--rw-r--r--   0 sam       (1000) sam       (1000)    19277 2023-01-22 15:00:13.000000 Cactool-0.6.0/cactool/views/datasets.py
--rw-r--r--   0 sam       (1000) sam       (1000)      558 2022-05-28 11:37:55.000000 Cactool-0.6.0/cactool/views/home.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3152 2022-05-28 11:37:55.000000 Cactool-0.6.0/cactool/views/projects.py
--rw-r--r--   0 sam       (1000) sam       (1000)      425 2023-01-22 14:59:50.000000 Cactool-0.6.0/cactool/views/site.py
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2022-07-06 17:45:09.000000 Cactool-0.6.0/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)     1028 2023-07-01 00:15:11.785363 Cactool-0.6.0/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.882981 Cactool-0.6.1/
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.842981 Cactool-0.6.1/Cactool.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     6047 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       44 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      142 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        8 2023-07-24 00:18:46.000000 Cactool-0.6.1/Cactool.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)     1093 2022-05-11 16:09:13.000000 Cactool-0.6.1/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     7367 2023-07-24 00:18:46.882981 Cactool-0.6.1/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     6821 2023-06-30 00:04:08.000000 Cactool-0.6.1/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.846315 Cactool-0.6.1/cactool/
+-rw-r--r--   0 sam       (1000) sam       (1000)     4631 2023-06-30 00:04:08.000000 Cactool-0.6.1/cactool/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       91 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    11482 2023-01-13 15:13:46.000000 Cactool-0.6.1/cactool/database.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      102 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/dates.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.846315 Cactool-0.6.1/cactool/defaults/
+-rw-r--r--   0 sam       (1000) sam       (1000)      365 2023-03-01 20:55:20.000000 Cactool-0.6.1/cactool/defaults/config.json
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.846315 Cactool-0.6.1/cactool/migrations/
+-rw-r--r--   0 sam       (1000) sam       (1000)       41 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/migrations/README
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.846315 Cactool-0.6.1/cactool/migrations/__pycache__/
+-rw-r--r--   0 sam       (1000) sam       (1000)     2254 2022-11-13 17:39:31.000000 Cactool-0.6.1/cactool/migrations/__pycache__/env.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     4001 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      832 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/migrations/alembic.ini
+-rw-r--r--   0 sam       (1000) sam       (1000)     2745 2022-11-13 17:39:27.000000 Cactool-0.6.1/cactool/migrations/env.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      494 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/migrations/script.py.mako
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.849648 Cactool-0.6.1/cactool/migrations/versions/
+-rw-r--r--   0 sam       (1000) sam       (1000)      592 2022-11-13 17:39:27.000000 Cactool-0.6.1/cactool/migrations/versions/07c0c9849f18_store_user_otp_secret.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      952 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/migrations/versions/07d73859b99c_add_show_data_type.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      822 2022-12-19 20:19:53.000000 Cactool-0.6.1/cactool/migrations/versions/16942fdb0f18_add_relative_column_priorities.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      709 2023-01-13 15:21:55.000000 Cactool-0.6.1/cactool/migrations/versions/19d06323ddd6_store_dataset_access_ranes.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      763 2023-01-12 00:42:42.000000 Cactool-0.6.1/cactool/migrations/versions/28e8811a530d_support_dataset_file_storage.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1269 2023-01-02 05:22:05.000000 Cactool-0.6.1/cactool/migrations/versions/51ed49d3ed75_support_user_email_verification.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      938 2022-12-19 20:19:53.000000 Cactool-0.6.1/cactool/migrations/versions/5e7f3be664d5_rename_priority_column_to_order.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      380 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/migrations/versions/6286ef6698f9_merge_heads.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      885 2022-11-13 17:39:27.000000 Cactool-0.6.1/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.859648 Cactool-0.6.1/cactool/migrations/versions/__pycache__/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1064 2022-11-12 14:02:05.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/072331977abf_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      966 2022-11-13 17:39:31.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1133 2022-11-17 22:52:32.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1592 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1026 2023-01-10 17:45:24.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/0f3a32ab3b24_support_dataset_files.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      946 2022-12-11 16:39:27.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      993 2023-01-01 23:29:37.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1644 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1005 2023-01-13 14:54:14.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1051 2023-01-22 14:51:47.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1888 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1092 2023-01-10 17:39:40.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/25345a0b177f_make_datasetfile_file_names_part_of_the_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1032 2023-01-13 14:54:14.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1594 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1299 2023-01-07 09:30:57.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     2396 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      922 2022-11-12 13:57:50.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/5ab489444dcc_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      986 2023-01-01 23:29:37.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1882 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      686 2022-11-13 17:44:58.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      695 2022-11-17 22:52:32.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1124 2022-11-13 17:39:31.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1579 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      937 2022-11-12 15:14:52.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/727b95af4b5f_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1242 2023-01-02 05:07:03.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/c0ed5c0ee030_.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      972 2022-11-13 17:39:31.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1628 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1154 2023-01-10 10:50:03.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     1615 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     3000 2022-11-13 17:39:31.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-310.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)     8379 2023-06-30 00:02:56.000000 Cactool-0.6.1/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-311.pyc
+-rw-r--r--   0 sam       (1000) sam       (1000)      587 2022-11-13 17:39:27.000000 Cactool-0.6.1/cactool/migrations/versions/c12d86b089b8_store_user_emails.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      982 2023-01-07 10:01:34.000000 Cactool-0.6.1/cactool/migrations/versions/ce5fc447a2e8_add_image_display_type.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5807 2022-11-13 17:39:27.000000 Cactool-0.6.1/cactool/migrations/versions/d1b66364eeb3_initial_migration.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.862981 Cactool-0.6.1/cactool/scripts/
+-rwxr-xr-x   0 sam       (1000) sam       (1000)       50 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/scripts/debug.sh
+-rwxr-xr-x   0 sam       (1000) sam       (1000)       92 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/scripts/delete-database.sh
+-rw-r--r--   0 sam       (1000) sam       (1000)      209 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/scripts/get-port.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)      323 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/scripts/update.sh
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.842981 Cactool-0.6.1/cactool/static/
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.866315 Cactool-0.6.1/cactool/static/assets/
+-rw-r--r--   0 sam       (1000) sam       (1000)   162190 2023-06-30 00:04:08.000000 Cactool-0.6.1/cactool/static/assets/404Error.png
+-rw-r--r--   0 sam       (1000) sam       (1000)   161280 2023-06-30 00:04:08.000000 Cactool-0.6.1/cactool/static/assets/StrangeError.png
+-rw-r--r--   0 sam       (1000) sam       (1000)    96984 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/static/assets/cactool-large.png
+-rw-r--r--   0 sam       (1000) sam       (1000)    15406 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/static/assets/favicon.ico
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.866315 Cactool-0.6.1/cactool/static/bin/
+-rw-r--r--   0 sam       (1000) sam       (1000)    15593 2022-05-14 10:36:35.000000 Cactool-0.6.1/cactool/static/bin/instagram_embed.js
+-rw-r--r--   0 sam       (1000) sam       (1000)    47547 2023-01-07 09:19:40.000000 Cactool-0.6.1/cactool/static/bin/tiktok_embed.js
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.869648 Cactool-0.6.1/cactool/static/css/
+-rw-r--r--   0 sam       (1000) sam       (1000)    95609 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/static/css/bootstrap-icons.css
+-rw-r--r--   0 sam       (1000) sam       (1000)   194901 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/static/css/bootstrap.css
+-rw-r--r--   0 sam       (1000) sam       (1000)      790 2023-02-28 15:07:32.000000 Cactool-0.6.1/cactool/static/css/cactool.css
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.869648 Cactool-0.6.1/cactool/static/css/fonts/
+-rw-r--r--   0 sam       (1000) sam       (1000)   121296 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 sam       (1000) sam       (1000)     1508 2022-12-20 02:32:09.000000 Cactool-0.6.1/cactool/static/css/login.css
+-rw-r--r--   0 sam       (1000) sam       (1000)      130 2022-12-20 02:57:30.000000 Cactool-0.6.1/cactool/static/css/projects.css
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.872981 Cactool-0.6.1/cactool/static/js/
+-rw-r--r--   0 sam       (1000) sam       (1000)    80496 2022-11-17 22:51:58.000000 Cactool-0.6.1/cactool/static/js/bootstrap.js
+-rw-r--r--   0 sam       (1000) sam       (1000)    10622 2023-07-23 12:16:46.000000 Cactool-0.6.1/cactool/static/js/code.js
+-rw-r--r--   0 sam       (1000) sam       (1000)      428 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/static/js/twitter.js
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.879648 Cactool-0.6.1/cactool/templates/
+-rw-r--r--   0 sam       (1000) sam       (1000)      838 2023-06-30 00:04:08.000000 Cactool-0.6.1/cactool/templates/404.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     3113 2022-12-20 03:07:40.000000 Cactool-0.6.1/cactool/templates/add_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      445 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/templates/card.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     4581 2023-02-28 15:09:22.000000 Cactool-0.6.1/cactool/templates/code_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2121 2023-01-02 14:21:53.000000 Cactool-0.6.1/cactool/templates/coding_interface.html
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.1/cactool/templates/contact.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1491 2022-12-20 02:57:47.000000 Cactool-0.6.1/cactool/templates/create_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2727 2022-12-20 02:38:15.000000 Cactool-0.6.1/cactool/templates/dashboard.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1583 2022-12-20 02:42:07.000000 Cactool-0.6.1/cactool/templates/delete_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1463 2022-12-20 03:06:04.000000 Cactool-0.6.1/cactool/templates/delete_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1268 2023-06-30 00:04:08.000000 Cactool-0.6.1/cactool/templates/error.html
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-12-19 20:19:56.000000 Cactool-0.6.1/cactool/templates/faq.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      615 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/templates/flash.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2067 2022-12-20 02:39:33.000000 Cactool-0.6.1/cactool/templates/import_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2349 2022-12-20 03:04:09.000000 Cactool-0.6.1/cactool/templates/index.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     6812 2022-05-28 12:15:27.000000 Cactool-0.6.1/cactool/templates/instagram_embed.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1947 2022-12-19 20:19:56.000000 Cactool-0.6.1/cactool/templates/login.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1847 2023-01-10 12:22:56.000000 Cactool-0.6.1/cactool/templates/macros.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2046 2022-12-19 20:19:56.000000 Cactool-0.6.1/cactool/templates/navigation.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1541 2022-12-20 02:59:07.000000 Cactool-0.6.1/cactool/templates/setup_2fa.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1634 2022-12-20 03:07:12.000000 Cactool-0.6.1/cactool/templates/show_datasets.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     4581 2023-07-23 12:03:50.000000 Cactool-0.6.1/cactool/templates/signup.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      209 2023-01-07 09:19:00.000000 Cactool-0.6.1/cactool/templates/tiktok_embed.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1545 2023-01-12 01:15:17.000000 Cactool-0.6.1/cactool/templates/upload_images.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     1488 2022-12-20 03:08:13.000000 Cactool-0.6.1/cactool/templates/verify_2fa.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     6815 2023-02-28 15:19:51.000000 Cactool-0.6.1/cactool/templates/view_dataset.html
+-rw-r--r--   0 sam       (1000) sam       (1000)     2401 2022-12-20 03:07:59.000000 Cactool-0.6.1/cactool/templates/view_project.html
+-rw-r--r--   0 sam       (1000) sam       (1000)      847 2023-01-07 09:58:35.000000 Cactool-0.6.1/cactool/types.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-07-24 00:18:46.882981 Cactool-0.6.1/cactool/views/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2022-05-11 16:09:13.000000 Cactool-0.6.1/cactool/views/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8318 2023-07-23 22:40:53.000000 Cactool-0.6.1/cactool/views/authentication.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    19238 2023-07-23 22:40:53.000000 Cactool-0.6.1/cactool/views/datasets.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      558 2022-05-28 11:37:55.000000 Cactool-0.6.1/cactool/views/home.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3152 2022-05-28 11:37:55.000000 Cactool-0.6.1/cactool/views/projects.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      425 2023-01-22 14:59:50.000000 Cactool-0.6.1/cactool/views/site.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2022-07-06 17:45:09.000000 Cactool-0.6.1/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)     1028 2023-07-24 00:18:46.882981 Cactool-0.6.1/setup.cfg
```

### Comparing `Cactool-0.6.0/Cactool.egg-info/PKG-INFO` & `Cactool-0.6.1/Cactool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cactool
-Version: 0.6.0
+Version: 0.6.1
 Summary: An easy way to collaboratively code social media posts for manual content and discourse analysis
 Home-page: https://cactool.github.io
 Author: Sam Ezeh
 Author-email: sam.z.ezeh@gmail.com
 Project-URL: Bug Tracker, https://github.com/cactool/cactool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Cactool Version: 0.6.0 Summary: An easy way to
+Metadata-Version: 2.1 Name: Cactool Version: 0.6.1 Summary: An easy way to
 collaboratively code social media posts for manual content and discourse
 analysis Home-page: https://cactool.github.io Author: Sam Ezeh Author-email:
 sam.z.ezeh@gmail.com Project-URL: Bug Tracker, https://github.com/cactool/
 cactool/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE ![Cactool](https://i.imgur.com/XooF3N8.png) # Cactool
```

### Comparing `Cactool-0.6.0/Cactool.egg-info/SOURCES.txt` & `Cactool-0.6.1/Cactool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/LICENSE` & `Cactool-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/PKG-INFO` & `Cactool-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cactool
-Version: 0.6.0
+Version: 0.6.1
 Summary: An easy way to collaboratively code social media posts for manual content and discourse analysis
 Home-page: https://cactool.github.io
 Author: Sam Ezeh
 Author-email: sam.z.ezeh@gmail.com
 Project-URL: Bug Tracker, https://github.com/cactool/cactool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Cactool Version: 0.6.0 Summary: An easy way to
+Metadata-Version: 2.1 Name: Cactool Version: 0.6.1 Summary: An easy way to
 collaboratively code social media posts for manual content and discourse
 analysis Home-page: https://cactool.github.io Author: Sam Ezeh Author-email:
 sam.z.ezeh@gmail.com Project-URL: Bug Tracker, https://github.com/cactool/
 cactool/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE ![Cactool](https://i.imgur.com/XooF3N8.png) # Cactool
```

### Comparing `Cactool-0.6.0/README.md` & `Cactool-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/__init__.py` & `Cactool-0.6.1/cactool/__init__.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/database.py` & `Cactool-0.6.1/cactool/database.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/__pycache__/env.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/__pycache__/env.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/alembic.ini` & `Cactool-0.6.1/cactool/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/env.py` & `Cactool-0.6.1/cactool/migrations/env.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/07c0c9849f18_store_user_otp_secret.py` & `Cactool-0.6.1/cactool/migrations/versions/07c0c9849f18_store_user_otp_secret.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/07d73859b99c_add_show_data_type.py` & `Cactool-0.6.1/cactool/migrations/versions/07d73859b99c_add_show_data_type.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/16942fdb0f18_add_relative_column_priorities.py` & `Cactool-0.6.1/cactool/migrations/versions/16942fdb0f18_add_relative_column_priorities.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/19d06323ddd6_store_dataset_access_ranes.py` & `Cactool-0.6.1/cactool/migrations/versions/19d06323ddd6_store_dataset_access_ranes.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/28e8811a530d_support_dataset_file_storage.py` & `Cactool-0.6.1/cactool/migrations/versions/28e8811a530d_support_dataset_file_storage.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/51ed49d3ed75_support_user_email_verification.py` & `Cactool-0.6.1/cactool/migrations/versions/51ed49d3ed75_support_user_email_verification.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/5e7f3be664d5_rename_priority_column_to_order.py` & `Cactool-0.6.1/cactool/migrations/versions/5e7f3be664d5_rename_priority_column_to_order.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py` & `Cactool-0.6.1/cactool/migrations/versions/7226d855d8ec_add_more_ordinal_data_types.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/072331977abf_store_user_emails.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/072331977abf_store_user_emails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/07c0c9849f18_store_user_otp_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/07d73859b99c_add_show_data_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/0f3a32ab3b24_support_dataset_files.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/0f3a32ab3b24_support_dataset_files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/16942fdb0f18_add_relative_column_priorities.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/19d06323ddd6_store_dataset_access_ranes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/25345a0b177f_make_datasetfile_file_names_part_of_the_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/25345a0b177f_make_datasetfile_file_names_part_of_the_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/28e8811a530d_support_dataset_file_storage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/51ed49d3ed75_support_user_email_verification.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/5ab489444dcc_store_user_emails.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/5ab489444dcc_store_user_emails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/5e7f3be664d5_rename_priority_column_to_order.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/6286ef6698f9_merge_heads.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/7226d855d8ec_add_more_ordinal_data_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/727b95af4b5f_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/727b95af4b5f_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/c0ed5c0ee030_.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/c0ed5c0ee030_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/c12d86b089b8_store_user_emails.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/ce5fc447a2e8_add_image_display_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-310.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-311.pyc` & `Cactool-0.6.1/cactool/migrations/versions/__pycache__/d1b66364eeb3_initial_migration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/c12d86b089b8_store_user_emails.py` & `Cactool-0.6.1/cactool/migrations/versions/c12d86b089b8_store_user_emails.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/ce5fc447a2e8_add_image_display_type.py` & `Cactool-0.6.1/cactool/migrations/versions/ce5fc447a2e8_add_image_display_type.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/migrations/versions/d1b66364eeb3_initial_migration.py` & `Cactool-0.6.1/cactool/migrations/versions/d1b66364eeb3_initial_migration.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/assets/404Error.png` & `Cactool-0.6.1/cactool/static/assets/404Error.png`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/assets/StrangeError.png` & `Cactool-0.6.1/cactool/static/assets/StrangeError.png`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/assets/cactool-large.png` & `Cactool-0.6.1/cactool/static/assets/cactool-large.png`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/assets/favicon.ico` & `Cactool-0.6.1/cactool/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/bin/instagram_embed.js` & `Cactool-0.6.1/cactool/static/bin/instagram_embed.js`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/bin/tiktok_embed.js` & `Cactool-0.6.1/cactool/static/bin/tiktok_embed.js`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/css/bootstrap-icons.css` & `Cactool-0.6.1/cactool/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/css/bootstrap.css` & `Cactool-0.6.1/cactool/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/css/cactool.css` & `Cactool-0.6.1/cactool/static/css/cactool.css`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/css/fonts/bootstrap-icons.woff2` & `Cactool-0.6.1/cactool/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/css/login.css` & `Cactool-0.6.1/cactool/static/css/login.css`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/js/bootstrap.js` & `Cactool-0.6.1/cactool/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/static/js/code.js` & `Cactool-0.6.1/cactool/static/js/code.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -106,15 +106,19 @@
     data = {
         dataset_id: window.dataset_id,
         row_number: window.row_number,
         values: {}
     }
 
     for (column of window.columns) {
-        if (column.type === SOCIAL_MEDIA || column.type === HIDDEN || column.type === IMAGE) {
+        if (
+            column.type === SOCIAL_MEDIA ||
+            column.type === HIDDEN ||
+            column.type === IMAGE ||
+            column.type === DISPLAY) {
             continue
         } else if (
             column.type == LIKERT ||
             column.type == ONE_TO_THREE ||
             column.type == ONE_TO_FIVE ||
             column.type == ONE_TO_SEVEN) {
             const selected = document.querySelector(`input[name="options-${column.name}"]:checked`);
```

### Comparing `Cactool-0.6.0/cactool/templates/404.html` & `Cactool-0.6.1/cactool/templates/404.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/add_dataset.html` & `Cactool-0.6.1/cactool/templates/add_dataset.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/code_dataset.html` & `Cactool-0.6.1/cactool/templates/code_dataset.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/coding_interface.html` & `Cactool-0.6.1/cactool/templates/coding_interface.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/create_project.html` & `Cactool-0.6.1/cactool/templates/create_project.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/dashboard.html` & `Cactool-0.6.1/cactool/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/delete_dataset.html` & `Cactool-0.6.1/cactool/templates/delete_dataset.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/delete_project.html` & `Cactool-0.6.1/cactool/templates/delete_project.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/error.html` & `Cactool-0.6.1/cactool/templates/error.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/flash.html` & `Cactool-0.6.1/cactool/templates/flash.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/import_dataset.html` & `Cactool-0.6.1/cactool/templates/import_dataset.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/index.html` & `Cactool-0.6.1/cactool/templates/index.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/instagram_embed.html` & `Cactool-0.6.1/cactool/templates/instagram_embed.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/login.html` & `Cactool-0.6.1/cactool/templates/login.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/macros.html` & `Cactool-0.6.1/cactool/templates/macros.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/navigation.html` & `Cactool-0.6.1/cactool/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/setup_2fa.html` & `Cactool-0.6.1/cactool/templates/setup_2fa.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/show_datasets.html` & `Cactool-0.6.1/cactool/templates/show_datasets.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/signup.html` & `Cactool-0.6.1/cactool/templates/signup.html`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                         <input name=username class=form-control />
                         <br>
                         <h3>
                             Password
                             {{
                               tooltip(
                                 "Passwords must have 8 or more
-                                chracters and must contain a number
+                                characters and must contain a number
                                 and a letter"
                               )
                             }}
                         </h3>
                         <input name=password type=password class=form-control />
                         <br>
                         {% if config['signup-code'] %}
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_syxhg6pc_/tmp_dod1ewk_TarContainer/0/121.html", line 53, column 34: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_syxhg6pc_/tmp_dod1ewk_TarContainer/0/121.html", line 53, column 34: Levels of opening and closing headings don't match*

```diff
@@ -19,15 +19,15 @@
 emails with the following domains: " + ', '.join(config['email-domains']) ) }}
 {% endif %} ****
 {% if config['require-email'] %} [Unknown INPUT type] {% else %}
 ***** optional *****
 [email               ] {% endif %} {% endif %}
 **** Username ****
 [username            ]
-**** Password {{ tooltip( "Passwords must have 8 or more chracters and must
+**** Password {{ tooltip( "Passwords must have 8 or more characters and must
 contain a number and a letter" ) }} ****
 [********************]
 {% if config['signup-code'] %}
 **** Sign up code {{ tooltip( "This instance requires a code to sign up. Please
 contact the system administrator." ) }} ****
 [                    ]
 {% endif %} [Sign up]
```

### Comparing `Cactool-0.6.0/cactool/templates/upload_images.html` & `Cactool-0.6.1/cactool/templates/upload_images.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/verify_2fa.html` & `Cactool-0.6.1/cactool/templates/verify_2fa.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/view_dataset.html` & `Cactool-0.6.1/cactool/templates/view_dataset.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/templates/view_project.html` & `Cactool-0.6.1/cactool/templates/view_project.html`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/types.py` & `Cactool-0.6.1/cactool/types.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/views/authentication.py` & `Cactool-0.6.1/cactool/views/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,16 @@
 import smtplib
 import ssl
 import time
 
 import pyotp
 import qrcode
 import qrcode.image.svg
-from flask import (
-    Blueprint,
-    current_app,
-    flash,
-    redirect,
-    render_template,
-    request,
-    session,
-    url_for,
-)
+from flask import (Blueprint, current_app, flash, redirect, render_template,
+                   request, session, url_for)
 from flask_login import login_user, logout_user
 from passlib.hash import pbkdf2_sha256
 
 from ..database import User, UserEmailVerification, db
 
 authentication = Blueprint("authentication", __name__)
```

### Comparing `Cactool-0.6.0/cactool/views/datasets.py` & `Cactool-0.6.1/cactool/views/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,41 +6,22 @@
 import tempfile
 import uuid
 import zipfile
 from pathlib import Path
 
 import requests
 from bs4 import BeautifulSoup
-from flask import (
-    Blueprint,
-    Response,
-    abort,
-    current_app,
-    flash,
-    jsonify,
-    redirect,
-    render_template,
-    request,
-    send_file,
-    url_for,
-)
+from flask import (Blueprint, Response, abort, current_app, flash, jsonify,
+                   redirect, render_template, request, send_file, url_for)
 from flask_login import current_user
 from sqlalchemy import select
 from werkzeug.utils import secure_filename
 
-from ..database import (
-    AccessLevel,
-    Dataset,
-    DatasetAccess,
-    DatasetFile,
-    DatasetRow,
-    DatasetRowValue,
-    Project,
-    db,
-)
+from ..database import (AccessLevel, Dataset, DatasetAccess, DatasetFile,
+                        DatasetRow, DatasetRowValue, Project, db)
 from ..dates import date_string
 from ..types import Type
 
 datasets = Blueprint("datasets", __name__)
 
 
 def process_row(row_data):
```

### Comparing `Cactool-0.6.0/cactool/views/home.py` & `Cactool-0.6.1/cactool/views/home.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/cactool/views/projects.py` & `Cactool-0.6.1/cactool/views/projects.py`

 * *Files identical despite different names*

### Comparing `Cactool-0.6.0/setup.cfg` & `Cactool-0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Cactool
-version = 0.6.0
+version = 0.6.1
 description = An easy way to collaboratively code social media posts for manual content and discourse analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Sam Ezeh
 author_email = sam.z.ezeh@gmail.com
 url = https://cactool.github.io
 project_urls =
```

