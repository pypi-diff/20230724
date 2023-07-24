# Comparing `tmp/ytdl-sub-2023.7.24.post2.tar.gz` & `tmp/ytdl-sub-2023.7.24.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.24.post2.tar", last modified: Mon Jul 24 17:23:41 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.24.post3.tar", last modified: Mon Jul 24 19:08:51 2023, max compression
```

## Comparing `ytdl-sub-2023.7.24.post2.tar` & `ytdl-sub-2023.7.24.post3.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 17:23:41.100891 ytdl-sub-2023.7.24.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.056890 ytdl-sub-2023.7.24.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.060890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.064890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.084891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.088891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.088891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.092891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.060890 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.094166 ytdl-sub-2023.7.24.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 19:08:51.094166 ytdl-sub-2023.7.24.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 19:08:51.094166 ytdl-sub-2023.7.24.post3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.078166 ytdl-sub-2023.7.24.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.082166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.082166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.082166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.082166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.086166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.090166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.090166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.090166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.090166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.090166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.094166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.094166 ytdl-sub-2023.7.24.post3/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-24 19:08:31.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:08:51.082166 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 19:08:51.000000 ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.24.post2/LICENSE` & `ytdl-sub-2023.7.24.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/PKG-INFO` & `ytdl-sub-2023.7.24.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.24.post2
+Version: 2023.7.24.post3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.24.post2/README.md` & `ytdl-sub-2023.7.24.post3/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/pyproject.toml` & `ytdl-sub-2023.7.24.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/setup.cfg` & `ytdl-sub-2023.7.24.post3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.url.multi_url import MultiUrlDownloader
 from ytdl_sub.downloaders.url.url import UrlDownloader
 from ytdl_sub.plugins.audio_extract import AudioExtractPlugin
 from ytdl_sub.plugins.chapters import ChaptersPlugin
 from ytdl_sub.plugins.date_range import DateRangePlugin
+from ytdl_sub.plugins.embed_thumbnail import EmbedThumbnailPlugin
 from ytdl_sub.plugins.file_convert import FileConvertPlugin
 from ytdl_sub.plugins.internal.view import ViewPlugin
 from ytdl_sub.plugins.match_filters import MatchFiltersPlugin
 from ytdl_sub.plugins.music_tags import MusicTagsPlugin
 from ytdl_sub.plugins.nfo_tags import NfoTagsPlugin
 from ytdl_sub.plugins.output_directory_nfo_tags import OutputDirectoryNfoTagsPlugin
 from ytdl_sub.plugins.plugin import Plugin
@@ -103,14 +104,15 @@
     Maps plugins defined in the preset to its respective plugin class
     """
 
     _MAPPING: Dict[str, Type[Plugin]] = {
         "_view": ViewPlugin,
         "audio_extract": AudioExtractPlugin,
         "date_range": DateRangePlugin,
+        "embed_thumbnail": EmbedThumbnailPlugin,
         "file_convert": FileConvertPlugin,
         "match_filters": MatchFiltersPlugin,
         "music_tags": MusicTagsPlugin,
         "video_tags": VideoTagsPlugin,
         "nfo_tags": NfoTagsPlugin,
         "output_directory_nfo_tags": OutputDirectoryNfoTagsPlugin,
         "regex": RegexPlugin,
```

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/music_tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,16 +66,14 @@
                artist: "{artist}"
                album: "{album}"
                genre: "ytdl-sub"
                # Supports id3v2.4 multi-tags
                albumartists:
                  - "{artist}"
                  - "ytdl-sub"
-             # Optional
-             embed_thumbnail: False
     """
 
     _required_keys = {"tags"}
     _optional_keys = {"embed_thumbnail"}
 
     @classmethod
     def partial_validate(cls, name: str, value: Any) -> None:
@@ -145,14 +143,19 @@
                             "Music tag '%s' does not support lists. "
                             "Only setting the first element",
                             tag_name,
                         )
                     setattr(audio_file, tag_name, tag_value[0])
 
             if self.plugin_options.embed_thumbnail:
+                logger.warning(
+                    "music_tags.embed_thumbnail is now deprecated. Use the dedicated "
+                    "embed_thumbnail plugin instead. This will be removed in October of 2023."
+                )
+
                 # convert the entry thumbnail so it is embedded as jpg
                 convert_download_thumbnail(entry=entry)
 
                 with open(entry.get_download_thumbnail_path(), "rb") as thumb:
                     mediafile_img = mediafile.Image(
                         data=thumb.read(), desc="cover", type=mediafile.ImageType.front
                     )
```

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     """
     Defines priority for plugins, 0 is highest priority
     """
 
     # If modify_entry priority is >= to this value, run after split
     MODIFY_ENTRY_AFTER_SPLIT = 10
 
+    # if post_process is >= to this value, run after file_convert
+    POST_PROCESS_AFTER_FILE_CONVERT = 10
+
     MODIFY_ENTRY_FIRST = 0
 
     def __init__(self, modify_entry: int = 5, post_process: int = 5):
         self.modify_entry = modify_entry
         self.post_process = post_process
 
     @property
```

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.24.post2
+Version: 2023.7.24.post3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.24.post3/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 src/ytdl_sub/entries/variables/__init__.py
 src/ytdl_sub/entries/variables/entry_variables.py
 src/ytdl_sub/entries/variables/kwargs.py
 src/ytdl_sub/plugins/__init__.py
 src/ytdl_sub/plugins/audio_extract.py
 src/ytdl_sub/plugins/chapters.py
 src/ytdl_sub/plugins/date_range.py
+src/ytdl_sub/plugins/embed_thumbnail.py
 src/ytdl_sub/plugins/file_convert.py
 src/ytdl_sub/plugins/match_filters.py
 src/ytdl_sub/plugins/music_tags.py
 src/ytdl_sub/plugins/nfo_tags.py
 src/ytdl_sub/plugins/output_directory_nfo_tags.py
 src/ytdl_sub/plugins/plugin.py
 src/ytdl_sub/plugins/regex.py
```

