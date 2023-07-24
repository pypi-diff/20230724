# Comparing `tmp/ytdl-sub-2023.7.24.post1.tar.gz` & `tmp/ytdl-sub-2023.7.24.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.7.24.post1.tar", last modified: Mon Jul 24 17:17:09 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.7.24.post2.tar", last modified: Mon Jul 24 17:23:41 2023, max compression
```

## Comparing `ytdl-sub-2023.7.24.post1.tar` & `ytdl-sub-2023.7.24.post2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.711863 ytdl-sub-2023.7.24.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:17:09.711863 ytdl-sub-2023.7.24.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 17:17:09.711863 ytdl-sub-2023.7.24.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.687862 ytdl-sub-2023.7.24.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.691862 ytdl-sub-2023.7.24.post1/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.691862 ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.691862 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.695863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.695863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.695863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.695863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.699863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.703863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.707863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.707863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.707863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.711863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.711863 ytdl-sub-2023.7.24.post1/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-24 17:16:42.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:17:09.691862 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 17:17:09.000000 ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 17:23:41.100891 ytdl-sub-2023.7.24.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.056890 ytdl-sub-2023.7.24.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.060890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.064890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.068890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.072890 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.080891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.084891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.088891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.088891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.092891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.096891 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-07-24 17:23:17.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:23:41.060890 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 17:23:41.000000 ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.7.24.post1/LICENSE` & `ytdl-sub-2023.7.24.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/PKG-INFO` & `ytdl-sub-2023.7.24.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.24.post1
+Version: 2023.7.24.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.24.post1/README.md` & `ytdl-sub-2023.7.24.post2/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/pyproject.toml` & `ytdl-sub-2023.7.24.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/setup.cfg` & `ytdl-sub-2023.7.24.post2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from typing import Union
 
 from mergedeep import mergedeep
 
 from ytdl_sub.config.config_validator import ConfigValidator
 from ytdl_sub.config.preset_class_mappings import DownloadStrategyMapping
 from ytdl_sub.config.preset_class_mappings import PluginMapping
+from ytdl_sub.config.preset_options import OptionsValidator
 from ytdl_sub.config.preset_options import OutputOptions
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.config.preset_options import YTDLOptions
 from ytdl_sub.downloaders.base_downloader import BaseDownloader
 from ytdl_sub.downloaders.base_downloader import BaseDownloaderValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginOptionsT
 from ytdl_sub.prebuilt_presets import PREBUILT_PRESET_NAMES
 from ytdl_sub.prebuilt_presets import PUBLISHED_PRESET_NAMES
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.yaml import dump_yaml
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
@@ -63,25 +63,25 @@
         f"Your presets: {', '.join(sorted(user_defined_presets))}",
     )
 
 
 class PresetPlugins:
     def __init__(self):
         self.plugin_types: List[Type[Plugin]] = []
-        self.plugin_options: List[PluginOptions] = []
+        self.plugin_options: List[OptionsValidator] = []
 
-    def add(self, plugin_type: Type[Plugin], plugin_options: PluginOptions) -> "PresetPlugins":
+    def add(self, plugin_type: Type[Plugin], plugin_options: OptionsValidator) -> "PresetPlugins":
         """
         Add a pair of plugin type and options to the list
         """
         self.plugin_types.append(plugin_type)
         self.plugin_options.append(plugin_options)
         return self
 
-    def zipped(self) -> Iterable[Tuple[Type[Plugin], PluginOptions]]:
+    def zipped(self) -> Iterable[Tuple[Type[Plugin], OptionsValidator]]:
         """
         Returns
         -------
         Plugin and PluginOptions zipped
         """
         return zip(self.plugin_types, self.plugin_options)
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/config/preset_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_datetime import StringDatetimeValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import OverridesStringFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 from ytdl_sub.validators.validators import LiteralDictValidator
+from ytdl_sub.validators.validators import Validator
 
 
 # pylint: disable=no-self-use
 # pylint: disable=unused-argument
-class OptionsValidator(StrictDictValidator, ABC):
+class OptionsValidator(Validator, ABC):
     """
     Abstract class that validates options for preset sections (plugins, downloaders)
     """
 
     def validation_exception(
         self,
         error_message: str | Exception,
@@ -66,14 +67,18 @@
             Available source variables when running the plugin
         override_variables
             Available override variables when running the plugin
         """
         return None
 
 
+class OptionsDictValidator(StrictDictValidator, OptionsValidator, ABC):
+    pass
+
+
 # pylint: enable=no-self-use
 # pylint: enable=unused-argument
 
 
 class YTDLOptions(LiteralDictValidator):
     """
     Optional. This section allows you to add any ytdl argument to ytdl-sub's downloader.
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from abc import ABC
 from typing import Generic
 from typing import Iterable
 from typing import List
 from typing import Type
 from typing import TypeVar
 
-from ytdl_sub.config.preset_options import OptionsValidator
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
-BaseDownloaderValidator = OptionsValidator
+BaseDownloaderValidator = OptionsDictValidator
 BaseDownloaderOptionsT = TypeVar("BaseDownloaderOptionsT", bound=BaseDownloaderValidator)
 
 
 class BaseDownloaderPlugin(Plugin[BaseDownloaderOptionsT], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/url/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
-from ytdl_sub.config.preset_options import OptionsValidator
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import OverridesStringFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 from ytdl_sub.validators.validators import ListValidator
 
@@ -168,15 +168,15 @@
 
             # see if this collection is missing any added vars (if so, inherit from the top)
             for var in added_variables.keys():
                 if var not in collection_variables.keys():
                     collection_variables[var] = added_variables[var]
 
 
-class MultiUrlValidator(OptionsValidator):
+class MultiUrlValidator(OptionsDictValidator):
     """
     Downloads from multiple URLs. If an entry is returned from more than one URL, it will
     resolve to the bottom-most URL settings.
     """
 
     _required_keys = {"urls"}
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/main.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/audio_extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os.path
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.exceptions import FileNotDownloadedException
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_TYPES_EXTENSION_MAPPING
 from ytdl_sub.validators.audo_codec_validator import AudioTypeValidator
 from ytdl_sub.validators.validators import FloatValidator
 
 
-class AudioExtractOptions(PluginOptions):
+class AudioExtractOptions(OptionsDictValidator):
     """
     Extracts audio from a video file.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/chapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import collections
 import re
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import COMMENTS
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_CUSTOM_CHAPTERS
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.chapters import Chapters
 from ytdl_sub.utils.ffmpeg import set_ffmpeg_metadata_chapters
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
 from ytdl_sub.validators.validators import BoolValidator
 from ytdl_sub.validators.validators import ListValidator
@@ -54,15 +54,15 @@
 
 
 class SponsorBlockCategoryListValidator(ListValidator[SponsorBlockCategoriesValidator]):
     _expected_value_type_name = "sponsorblock category"
     _inner_list_type = SponsorBlockCategoriesValidator
 
 
-class ChaptersOptions(PluginOptions):
+class ChaptersOptions(OptionsDictValidator):
     """
     Embeds chapters to video files if they are present. Additional options to add SponsorBlock
     chapters and remove specific ones. Can also remove chapters using regex.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/date_range.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.datetime import to_date_range
 from ytdl_sub.validators.string_datetime import StringDatetimeValidator
 
 
-class DateRangeOptions(PluginOptions):
+class DateRangeOptions(OptionsDictValidator):
     """
     Only download files uploaded within the specified date range.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/file_convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import EXT
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import FileNotDownloadedException
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.validators.audo_codec_validator import FileTypeValidator
@@ -18,15 +18,15 @@
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
 
 
 class FileConvertWithValidator(StringSelectValidator):
     _select_values = {"yt-dlp", "ffmpeg"}
 
 
-class FileConvertOptions(PluginOptions):
+class FileConvertOptions(OptionsDictValidator):
     """
     Converts video files from one extension to another.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/internal/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.config.preset_options import Overrides
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.output_directory_nfo_tags import OutputDirectoryNfoTagsOptions
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
-class ViewOptions(PluginOptions):
+class ViewOptions(OptionsDictValidator):
     """
     INTERNAL PLUGIN. Do not expose in documentation
     """
 
     _optional_keys = {"_placeholder"}
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/match_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp import match_filter_func
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_MATCH_FILTER_REJECT
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.validators import StringListValidator
 
 logger = Logger.get("match_filters")
 
 
-class MatchFiltersOptions(PluginOptions):
+class MatchFiltersOptions(OptionsDictValidator):
     """
     Set ``--match-filters``` to pass into yt-dlp to filter entries from being downloaded.
     Uses the same syntax as yt-dlp.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/music_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict
 from typing import Any
 from typing import Dict
 from typing import List
 
 import mediafile
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.validators.audo_codec_validator import AUDIO_CODEC_EXTS
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import ListFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
@@ -41,15 +41,15 @@
         Returns
         -------
         Tag formatter(s) as a list
         """
         return self._tags
 
 
-class MusicTagsOptions(PluginOptions):
+class MusicTagsOptions(OptionsDictValidator):
     """
     Adds tags to every download audio file using
     `MediaFile <https://mediafile.readthedocs.io/en/latest/>`_,
     the same audio file tagging package used by
     `beets <https://beets.readthedocs.io/en/stable/>`_.
     It supports basic tags like ``title``, ``album``, ``artist`` and ``albumartist``. You can find
     a full list of tags for various file types in MediaFile's
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.xml import XmlElement
 from ytdl_sub.utils.xml import to_max_3_byte_utf8_dict
 from ytdl_sub.utils.xml import to_max_3_byte_utf8_string
 from ytdl_sub.utils.xml import to_xml
 from ytdl_sub.validators.file_path_validators import StringFormatterFileNameValidator
 from ytdl_sub.validators.nfo_validators import NfoTagsValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.validators import BoolValidator
 
 
-class SharedNfoTagsOptions(PluginOptions):
+class SharedNfoTagsOptions(OptionsDictValidator):
     """
     Shared code between NFO tags and Ouptut Directory NFO Tags
     """
 
     _required_keys = {"nfo_name", "nfo_root", "tags"}
     _optional_keys = {"kodi_safe"}
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         Returns
         -------
         True if the plugin should modify an entry after a potential split. False otherwise.
         """
         return self.modify_entry >= PluginPriority.MODIFY_ENTRY_AFTER_SPLIT
 
 
-PluginOptions = OptionsValidator
-PluginOptionsT = TypeVar("PluginOptionsT", bound=PluginOptions)
+PluginOptionsT = TypeVar("PluginOptionsT", bound=OptionsValidator)
 
 
 class Plugin(DownloadArchiver, Generic[PluginOptionsT], ABC):
     """
     Class to define the new plugin functionality
     """
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp.utils import sanitize_filename
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import YTDL_SUB_REGEX_SOURCE_VARS
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.plugins.plugin import PluginPriority
 from ytdl_sub.utils.exceptions import RegexNoMatchException
 from ytdl_sub.utils.exceptions import StringFormattingVariableNotFoundException
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.validators.regex_validator import RegexListValidator
 from ytdl_sub.validators.source_variable_validator import SourceVariableNameListValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
@@ -117,15 +117,15 @@
     def __init__(self, name, value):
         super().__init__(name, value)
         self.variable_capture_dict: Dict[str, VariableRegex] = {
             key: self._validate_key(key=key, validator=VariableRegex) for key in self._keys
         }
 
 
-class RegexOptions(PluginOptions):
+class RegexOptions(OptionsDictValidator):
     r"""
     Performs regex matching on an entry's source or override variables. Regex can be used to filter
     entries from proceeding with download or capture groups to create new source variables. NOTE to
     use backslashes anywhere in your regex, i.e. ``\d``, you must add another backslash escape. This
     means ``\d`` should be written as ``\\d``. This is because YAML requires an escape for any
     backslash usage.
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 from yt_dlp.utils import sanitize_filename
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import CHAPTERS
 from ytdl_sub.entries.variables.kwargs import SPLIT_BY_CHAPTERS_PARENT_ENTRY
 from ytdl_sub.entries.variables.kwargs import SPONSORBLOCK_CHAPTERS
 from ytdl_sub.entries.variables.kwargs import UID
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.chapters import Chapters
 from ytdl_sub.utils.chapters import Timestamp
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.utils.ffmpeg import FFMPEG
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
@@ -43,15 +43,15 @@
 
 
 class WhenNoChaptersValidator(StringSelectValidator):
     _expected_value_type_name = "when no chapters option"
     _select_values = {"pass", "drop", "error"}
 
 
-class SplitByChaptersOptions(PluginOptions):
+class SplitByChaptersOptions(OptionsDictValidator):
     """
     Splits a file by chapters into multiple files. Each file becomes its own entry with the
     new source variables ``chapter_title``, ``chapter_title_sanitized``, ``chapter_index``,
     ``chapter_index_padded``, ``chapter_count``.
 
     If a file has no chapters, and ``when_no_chapters`` is set to "pass", then ``chapter_title`` is
     set to the entry's title and ``chapter_index``, ``chapter_count`` are both set to 1.
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/subtitles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Optional
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.subtitles import SUBTITLE_EXTENSIONS
 from ytdl_sub.validators.file_path_validators import StringFormatterFileNameValidator
 from ytdl_sub.validators.string_formatter_validators import StringFormatterValidator
 from ytdl_sub.validators.string_select_validator import StringSelectValidator
@@ -21,15 +21,15 @@
 
 
 class SubtitlesTypeValidator(StringSelectValidator):
     _expected_value_type_name = "subtitles type"
     _select_values = SUBTITLE_EXTENSIONS
 
 
-class SubtitleOptions(PluginOptions):
+class SubtitleOptions(OptionsDictValidator):
     """
     Defines how to download and store subtitles. Using this plugin creates two new variables:
     ``lang`` and ``subtitles_ext``. ``lang`` is dynamic since you can download multiple subtitles.
     It will set the respective language to the correct subtitle file.
 
     Usage:
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/plugins/video_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any
 from typing import Dict
 
+from ytdl_sub.config.preset_options import OptionsDictValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.plugins.plugin import Plugin
-from ytdl_sub.plugins.plugin import PluginOptions
 from ytdl_sub.utils.ffmpeg import add_ffmpeg_metadata_key_values
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
 
 
-class VideoTagsOptions(PluginOptions):
+class VideoTagsOptions(OptionsDictValidator):
     """
     Adds tags to every downloaded video file using ffmpeg ``-metadata key=value`` args.
 
     Usage:
 
     .. code-block:: yaml
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.7.24.post1
+Version: 2023.7.24.post2
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.7.24.post1/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.7.24.post2/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

