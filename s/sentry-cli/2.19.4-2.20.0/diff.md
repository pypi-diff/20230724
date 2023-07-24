# Comparing `tmp/sentry_cli-2.19.4.tar.gz` & `tmp/sentry_cli-2.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.19.4.tar", last modified: Tue Jun 27 12:56:23 2023, max compression
+gzip compressed data, was "sentry_cli-2.20.0.tar", last modified: Fri Jul 21 10:48:14 2023, max compression
```

## Comparing `sentry_cli-2.19.4.tar` & `sentry_cli-2.20.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/
--rw-r--r--   0 runner    (1001) docker     (123)    80979 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.824067 sentry_cli-2.19.4/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-27 12:56:23.000000 sentry_cli-2.19.4/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-27 12:56:23.000000 sentry_cli-2.19.4/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:56:23.000000 sentry_cli-2.19.4/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:56:23.000000 sentry_cli-2.19.4/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.824067 sentry_cli-2.19.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87371 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.824067 sentry_cli-2.19.4/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.828067 sentry_cli-2.19.4/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.832068 sentry_cli-2.19.4/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.832068 sentry_cli-2.19.4/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.832068 sentry_cli-2.19.4/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:56:23.836068 sentry_cli-2.19.4/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-27 12:56:07.000000 sentry_cli-2.19.4/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.458107 sentry_cli-2.20.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    80991 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-21 10:48:14.458107 sentry_cli-2.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.442107 sentry_cli-2.20.0/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-21 10:48:14.000000 sentry_cli-2.20.0/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-21 10:48:14.000000 sentry_cli-2.20.0/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:48:14.000000 sentry_cli-2.20.0/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:48:14.000000 sentry_cli-2.20.0/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 10:48:14.462108 sentry_cli-2.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.442107 sentry_cli-2.20.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    90307 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.442107 sentry_cli-2.20.0/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.446107 sentry_cli-2.20.0/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.446107 sentry_cli-2.20.0/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.446107 sentry_cli-2.20.0/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.446107 sentry_cli-2.20.0/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.446107 sentry_cli-2.20.0/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/issues/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.450107 sentry_cli-2.20.0/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.454107 sentry_cli-2.20.0/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    24715 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.458107 sentry_cli-2.20.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.458107 sentry_cli-2.20.0/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:48:14.458107 sentry_cli-2.20.0/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    40019 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-21 10:47:49.000000 sentry_cli-2.20.0/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.19.4/Cargo.lock` & `sentry_cli-2.20.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2185,15 +2185,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.19.4"
+version = "2.20.0"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
@@ -2464,19 +2464,20 @@
 dependencies = [
  "libc",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "sourcemap"
-version = "6.2.3"
+version = "6.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eed16231c92d0a6f0388f56e0ab2be24ecff1173f8e22f0ea5e074d0525631cb"
+checksum = "e8df03d85f2767c45e61b4453eb6144153c80399e4fdd6407a6d16cb87cc0347"
 dependencies = [
  "data-encoding",
+ "debugid",
  "if_chain",
  "rustc_version 0.2.3",
  "scroll 0.10.2",
  "serde",
  "serde_json",
  "unicode-id",
  "url",
```

### Comparing `sentry_cli-2.19.4/Cargo.toml` & `sentry_cli-2.20.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.19.4"
+version = "2.20.0"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -61,15 +61,15 @@
   "anyhow",
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
-sourcemap = { version = "6.2.3", features = ["ram_bundle"] }
+sourcemap = { version = "6.3.0", features = ["ram_bundle"] }
 symbolic = { version = "12.1.5", features = ["debuginfo-serde", "il2cpp"] }
 thiserror = "1.0.38"
 url = "2.3.1"
 username = "0.2.0"
 uuid = { version = "1.3.0", features = ["v4", "serde"] }
 walkdir = "2.3.2"
 which = "4.4.0"
```

### Comparing `sentry_cli-2.19.4/LICENSE` & `sentry_cli-2.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/PKG-INFO` & `sentry_cli-2.20.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.19.4
+Version: 2.20.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.4 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.20.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.4/README.md` & `sentry_cli-2.20.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/build.rs` & `sentry_cli-2.20.0/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.20.0/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.19.4
+Version: 2.20.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.4 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.20.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.19.4/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.20.0/sentry_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 src/commands/deploys/new.rs
 src/commands/events/list.rs
 src/commands/events/mod.rs
 src/commands/files/delete.rs
 src/commands/files/list.rs
 src/commands/files/mod.rs
 src/commands/files/upload.rs
+src/commands/issues/list.rs
 src/commands/issues/mod.rs
 src/commands/issues/mute.rs
 src/commands/issues/resolve.rs
 src/commands/issues/unresolve.rs
 src/commands/monitors/list.rs
 src/commands/monitors/mod.rs
 src/commands/monitors/run.rs
```

### Comparing `sentry_cli-2.19.4/setup.cfg` & `sentry_cli-2.20.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/setup.py` & `sentry_cli-2.20.0/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/api.rs` & `sentry_cli-2.20.0/src/api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -552,16 +552,23 @@
                     "/organizations/{}/releases/{}/files/?cursor={}",
                     PathArg(org),
                     PathArg(release),
                     QueryArg(&cursor),
                 )
             };
 
+            let mut checkums_qs = String::new();
             for checksum in checksums.iter() {
-                path.push_str(&format!("&checksum={}", QueryArg(checksum)));
+                checkums_qs.push_str(&format!("&checksum={}", QueryArg(checksum)));
+            }
+            // We have a 16kb buffer for reach request configured in nginx,
+            // so do not even bother trying if it's too long.
+            // (16_384 limit still leaves us with 384 bytes for the url itself).
+            if !checkums_qs.is_empty() && checkums_qs.len() <= 16_000 {
+                path.push_str(&checkums_qs);
             }
 
             let resp = self.get(&path)?;
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ReleaseNotFound.into());
                 } else {
@@ -1350,14 +1357,38 @@
                 app_id: manifest.package().to_string(),
                 version: manifest.version_name().to_string(),
                 build: Some(manifest.version_code().to_string()),
             },
         )
     }
 
+    pub fn associate_proguard_mappings(
+        &self,
+        org: &str,
+        project: &str,
+        data: &AssociateProguard,
+    ) -> ApiResult<()> {
+        let path = format!(
+            "/projects/{}/{}/files/proguard-artifact-releases",
+            PathArg(org),
+            PathArg(project)
+        );
+        let resp: ApiResponse = self
+            .request(Method::Post, &path)?
+            .with_json_body(data)?
+            .send()?;
+        if resp.status() == 201 {
+            Ok(())
+        } else if resp.status() == 404 {
+            return Err(ApiErrorKind::ResourceNotFound.into());
+        } else {
+            resp.convert()
+        }
+    }
+
     /// Associate arbitrary debug symbols with a build
     pub fn associate_dsyms(
         &self,
         org: &str,
         project: &str,
         data: &AssociateDsyms,
     ) -> ApiResult<Option<AssociateDsymsResponse>> {
@@ -1561,14 +1592,67 @@
                 break;
             }
         }
 
         Ok(rv)
     }
 
+    /// List all issues associated with an organization and a project
+    pub fn list_organization_project_issues(
+        &self,
+        org: &str,
+        project: &str,
+        max_pages: usize,
+        query: Option<String>,
+    ) -> ApiResult<Vec<Issue>> {
+        let mut rv = vec![];
+        let mut cursor = "".to_string();
+        let mut requests_no = 0;
+
+        let url = if let Some(query) = query {
+            format!(
+                "/projects/{}/{}/issues/?query={}&",
+                PathArg(org),
+                PathArg(project),
+                QueryArg(&query),
+            )
+        } else {
+            format!("/projects/{}/{}/issues/?", PathArg(org), PathArg(project),)
+        };
+
+        loop {
+            requests_no += 1;
+
+            let resp = self.get(&format!("{}cursor={}", url, QueryArg(&cursor)))?;
+
+            if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
+                if rv.is_empty() {
+                    return Err(ApiErrorKind::OrganizationNotFound.into());
+                } else {
+                    break;
+                }
+            }
+
+            let pagination = resp.pagination();
+            rv.extend(resp.convert::<Vec<Issue>>()?.into_iter());
+
+            if requests_no == max_pages {
+                break;
+            }
+
+            if let Some(next) = pagination.into_next_cursor() {
+                cursor = next;
+            } else {
+                break;
+            }
+        }
+
+        Ok(rv)
+    }
+
     /// List all repos associated with an organization
     pub fn list_organization_repos(&self, org: &str) -> ApiResult<Vec<Repo>> {
         let mut rv = vec![];
         let mut cursor = "".to_string();
         loop {
             let path = format!(
                 "/organizations/{}/repos/?cursor={}",
@@ -2340,19 +2424,36 @@
     pub name: String,
     #[serde(rename = "appId")]
     pub app_id: String,
     pub version: String,
     pub build: Option<String>,
 }
 
+#[derive(Debug, Serialize)]
+pub struct AssociateProguard {
+    pub release_name: String,
+    pub proguard_uuid: String,
+}
+
 #[derive(Deserialize)]
 struct MissingChecksumsResponse {
     missing: HashSet<Digest>,
 }
 
+#[derive(Clone, Debug, Deserialize)]
+#[serde(rename_all = "camelCase")]
+pub struct Issue {
+    pub id: String,
+    pub short_id: String,
+    pub title: String,
+    pub last_seen: String,
+    pub status: String,
+    pub level: String,
+}
+
 /// Change information for issue bulk updates.
 #[derive(Serialize, Default)]
 pub struct IssueChanges {
     #[serde(rename = "status")]
     pub new_status: Option<String>,
     #[serde(rename = "snoozeDuration")]
     pub snooze_duration: Option<i64>,
```

### Comparing `sentry_cli-2.19.4/src/bashsupport.sh` & `sentry_cli-2.20.0/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/bash_hook.rs` & `sentry_cli-2.20.0/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.20.0/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.20.0/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/check.rs` & `sentry_cli-2.20.0/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/find.rs` & `sentry_cli-2.20.0/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/mod.rs` & `sentry_cli-2.20.0/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.20.0/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/debug_files/upload.rs` & `sentry_cli-2.20.0/src/commands/debug_files/upload.rs`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,15 @@
             "elf" => upload.filter_format(DifFormat::Object(FileFormat::Elf)),
             "breakpad" => upload.filter_format(DifFormat::Object(FileFormat::Breakpad)),
             "pdb" => upload.filter_format(DifFormat::Object(FileFormat::Pdb)),
             "pe" => upload.filter_format(DifFormat::Object(FileFormat::Pe)),
             "sourcebundle" => upload.filter_format(DifFormat::Object(FileFormat::SourceBundle)),
             "portablepdb" => upload.filter_format(DifFormat::Object(FileFormat::PortablePdb)),
             "jvm" => upload.filter_format(DifFormat::Object(FileFormat::SourceBundle)),
+            "wasm" => upload.filter_format(DifFormat::Object(FileFormat::Wasm)),
             "bcsymbolmap" => {
                 upload.filter_format(DifFormat::BcSymbolMap);
                 upload.filter_format(DifFormat::PList)
             }
             other => bail!("Unsupported type: {}", other),
         };
     }
```

### Comparing `sentry_cli-2.19.4/src/commands/deploys/list.rs` & `sentry_cli-2.20.0/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/deploys/mod.rs` & `sentry_cli-2.20.0/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/deploys/new.rs` & `sentry_cli-2.20.0/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/events/list.rs` & `sentry_cli-2.20.0/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/events/mod.rs` & `sentry_cli-2.20.0/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/files/delete.rs` & `sentry_cli-2.20.0/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/files/list.rs` & `sentry_cli-2.20.0/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/files/mod.rs` & `sentry_cli-2.20.0/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/files/upload.rs` & `sentry_cli-2.20.0/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/info.rs` & `sentry_cli-2.20.0/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/issues/mod.rs` & `sentry_cli-2.20.0/src/commands/issues/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 use anyhow::Result;
 use clap::{Arg, ArgAction, ArgMatches, Command};
 
 use crate::utils::args::ArgExt;
 
+pub mod list;
 pub mod mute;
 pub mod resolve;
 pub mod unresolve;
 
 macro_rules! each_subcommand {
     ($mac:ident) => {
+        $mac!(list);
         $mac!(mute);
         $mac!(resolve);
         $mac!(unresolve);
     };
 }
 
 pub fn make_command(mut command: Command) -> Command {
```

### Comparing `sentry_cli-2.19.4/src/commands/issues/mute.rs` & `sentry_cli-2.20.0/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/issues/resolve.rs` & `sentry_cli-2.20.0/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/issues/unresolve.rs` & `sentry_cli-2.20.0/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/login.rs` & `sentry_cli-2.20.0/src/commands/login.rs`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             .action(ArgAction::SetTrue)
             .help("Store authentication token globally rather than locally."),
     )
 }
 
 fn update_config(config: &Config, token: &str) -> Result<()> {
     let mut new_cfg = config.clone();
-    new_cfg.set_auth(Auth::Token(token.to_string()));
+    new_cfg.set_auth(Auth::Token(token.to_string()))?;
     new_cfg.save()?;
     Ok(())
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     let config = Config::current();
     let token_url = format!("{}/api/", config.get_base_url()?);
@@ -61,15 +61,15 @@
         token = if let Some(token) = predefined_token {
             token.to_string()
         } else {
             prompt("Enter your token")?
         };
 
         let test_cfg = config.make_copy(|cfg| {
-            cfg.set_auth(Auth::Token(token.to_string()));
+            cfg.set_auth(Auth::Token(token.to_string()))?;
             Ok(())
         })?;
         match Api::with_config(test_cfg).get_auth_info() {
             Ok(info) => {
                 // we can unwrap here somewhat safely because we do not permit
                 // signing in with legacy non user bound api keys here.
                 println!("Valid token for user {}", info.user.unwrap().email);
```

### Comparing `sentry_cli-2.19.4/src/commands/mod.rs` & `sentry_cli-2.20.0/src/commands/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -93,29 +93,29 @@
     #[cfg(not(target_os = "macos"))]
     fn sentry_react_native_xcode_wrap() -> Result<bool> {
         Ok(false)
     }
 }
 
 fn configure_args(config: &mut Config, matches: &ArgMatches) -> Result<()> {
-    if let Some(url) = matches.get_one::<String>("url") {
-        config.set_base_url(url);
+    if let Some(api_key) = matches.get_one::<String>("api_key") {
+        config.set_auth(Auth::Key(api_key.to_owned()))?;
     }
 
-    if let Some(headers) = matches.get_many::<String>("headers") {
-        let headers = headers.map(|h| h.to_owned()).collect();
-        config.set_headers(headers);
+    if let Some(auth_token) = matches.get_one::<String>("auth_token") {
+        config.set_auth(Auth::Token(auth_token.to_owned()))?;
     }
 
-    if let Some(api_key) = matches.get_one::<String>("api_key") {
-        config.set_auth(Auth::Key(api_key.to_owned()));
+    if let Some(url) = matches.get_one::<String>("url") {
+        config.set_base_url(url)?;
     }
 
-    if let Some(auth_token) = matches.get_one::<String>("auth_token") {
-        config.set_auth(Auth::Token(auth_token.to_owned()));
+    if let Some(headers) = matches.get_many::<String>("headers") {
+        let headers = headers.map(|h| h.to_owned()).collect();
+        config.set_headers(headers);
     }
 
     if let Some(level_str) = matches.get_one::<String>("log_level") {
         match level_str.parse() {
             Ok(level) => {
                 config.set_log_level(level);
             }
```

### Comparing `sentry_cli-2.19.4/src/commands/monitors/list.rs` & `sentry_cli-2.20.0/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/monitors/mod.rs` & `sentry_cli-2.20.0/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/monitors/run.rs` & `sentry_cli-2.20.0/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/organizations/list.rs` & `sentry_cli-2.20.0/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/organizations/mod.rs` & `sentry_cli-2.20.0/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/projects/list.rs` & `sentry_cli-2.20.0/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/projects/mod.rs` & `sentry_cli-2.20.0/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/react_native/appcenter.rs` & `sentry_cli-2.20.0/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/react_native/gradle.rs` & `sentry_cli-2.20.0/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/react_native/mod.rs` & `sentry_cli-2.20.0/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/react_native/xcode.rs` & `sentry_cli-2.20.0/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/archive.rs` & `sentry_cli-2.20.0/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/delete.rs` & `sentry_cli-2.20.0/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/finalize.rs` & `sentry_cli-2.20.0/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/info.rs` & `sentry_cli-2.20.0/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/list.rs` & `sentry_cli-2.20.0/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/mod.rs` & `sentry_cli-2.20.0/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/new.rs` & `sentry_cli-2.20.0/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/restore.rs` & `sentry_cli-2.20.0/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/releases/set_commits.rs` & `sentry_cli-2.20.0/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/repos/list.rs` & `sentry_cli-2.20.0/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/repos/mod.rs` & `sentry_cli-2.20.0/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/send_envelope.rs` & `sentry_cli-2.20.0/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/send_event.rs` & `sentry_cli-2.20.0/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.20.0/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.20.0/src/commands/sourcemaps/inject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             If the referenced sourcemap already contains a debug id, \
             that id is used instead.",
         )
         .arg(
             Arg::new("paths")
                 .value_name("PATHS")
                 .num_args(1..)
+                .required(true)
                 .action(ArgAction::Append)
                 .help(
                     "A path to recursively search for javascript files that should be processed.",
                 ),
         )
         .arg(
             Arg::new("ignore")
```

### Comparing `sentry_cli-2.19.4/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.20.0/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.20.0/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.20.0/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/uninstall.rs` & `sentry_cli-2.20.0/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/update.rs` & `sentry_cli-2.20.0/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/commands/upload_proguard.rs` & `sentry_cli-2.20.0/src/commands/upload_proguard.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 use clap::{Arg, ArgMatches, Command};
 use console::style;
 use log::{debug, info};
 use proguard::ProguardMapping;
 use symbolic::common::ByteView;
 use uuid::Uuid;
 
-use crate::api::{Api, AssociateDsyms};
+use crate::api::Api;
+use crate::api::AssociateProguard;
 use crate::config::Config;
 use crate::utils::android::{dump_proguard_uuids_as_properties, AndroidManifest};
 use crate::utils::args::ArgExt;
 use crate::utils::fs::{get_sha1_checksum, TempFile};
 use crate::utils::system::QuietExit;
 use crate::utils::ui::{copy_with_progress, make_byte_progress_bar};
 
@@ -212,15 +213,14 @@
         return Err(QuietExit(1).into());
     }
 
     println!("{} compressing mappings", style(">").dim());
     let tf = TempFile::create()?;
     {
         let mut zip = zip::ZipWriter::new(tf.open()?);
-
         for mapping in &mappings {
             let pb = make_byte_progress_bar(mapping.size);
             zip.start_file(
                 format!("proguard/{}.txt", mapping.uuid),
                 zip::write::FileOptions::default(),
             )?;
             copy_with_progress(&pb, &mut fs::File::open(&mapping.path)?, &mut zip)?;
@@ -263,30 +263,37 @@
 
     // update the uuids
     if let Some(android_manifest) = android_manifest {
         api.associate_android_proguard_mappings(&org, &project, &android_manifest, all_checksums)?;
 
     // if values are given associate
     } else if let Some(app_id) = matches.get_one::<String>("app_id") {
-        api.associate_dsyms(
-            &org,
-            &project,
-            &AssociateDsyms {
-                platform: matches
-                    .get_one::<String>("platform")
-                    .map(String::as_str)
-                    .unwrap_or("android")
-                    .to_string(),
-                checksums: all_checksums,
-                name: app_id.to_string(),
-                app_id: app_id.to_string(),
-                version: matches.get_one::<String>("version").unwrap().to_owned(),
-                build: matches.get_one::<String>("version_code").cloned(),
-            },
-        )?;
+        let version = matches.get_one::<String>("version").unwrap().to_owned();
+        let build: Option<String> = matches.get_one::<String>("version_code").cloned();
+
+        let mut release_name = app_id.to_owned();
+        release_name.push('@');
+        release_name.push_str(&version);
+
+        if let Some(build_str) = build {
+            release_name.push('+');
+            release_name.push_str(&build_str);
+        }
+
+        for mapping in &mappings {
+            let uuid = forced_uuid.unwrap_or(&mapping.uuid);
+            api.associate_proguard_mappings(
+                &org,
+                &project,
+                &AssociateProguard {
+                    release_name: release_name.to_owned(),
+                    proguard_uuid: uuid.to_string(),
+                },
+            )?;
+        }
     }
 
     // If wanted trigger reprocessing
     if !matches.get_flag("no_reprocessing") && !matches.get_flag("no_upload") {
         if !api.trigger_reprocessing(&org, &project)? {
             println!(
                 "{} Server does not support reprocessing. Not triggering.",
```

### Comparing `sentry_cli-2.19.4/src/config.rs` & `sentry_cli-2.20.0/src/config.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,61 +9,122 @@
 use anyhow::{bail, format_err, Context, Error, Result};
 use clap::ArgMatches;
 use ini::Ini;
 use lazy_static::lazy_static;
 use log::{debug, info, set_max_level, warn};
 use parking_lot::Mutex;
 use sentry::types::Dsn;
+use serde::Deserialize;
 
 use crate::constants::DEFAULT_MAX_DIF_ITEM_SIZE;
 use crate::constants::DEFAULT_MAX_DIF_UPLOAD_SIZE;
 use crate::constants::{CONFIG_RC_FILE_NAME, DEFAULT_RETRIES, DEFAULT_URL};
 use crate::utils::http::is_absolute_url;
 
 /// Represents the auth information
 #[derive(Debug, Clone)]
 pub enum Auth {
     Key(String),
     Token(String),
 }
 
+/// Data parsed from an "org auth token".
+#[derive(Debug, Clone, Deserialize, PartialEq, Eq)]
+struct TokenData {
+    /// An org slug.
+    org: String,
+    /// A base Sentry URL.
+    url: String,
+}
+
+impl TokenData {
+    /// Attempt to extract data from an "org auth token".
+    ///
+    /// Org auth tokens start with `sntrys` and contain BASE64-encoded
+    /// data between two underscores.
+    ///
+    /// Attempting to decode a valid org auth token results in `Ok(Some(data))`.
+    /// Attempting to decode an org auth token that contains invalid data returns an error.
+    /// Attempting to decode any other token returns Ok(None).
+    fn decode(token: &str) -> Result<Option<Self>> {
+        const ORG_TOKEN_PREFIX: &str = "sntrys_";
+
+        let Some(rest) = token.strip_prefix(ORG_TOKEN_PREFIX) else {
+            return Ok(None);
+        };
+
+        let Some((encoded, _)) = rest.split_once('_') else {
+            bail!("no closing _");
+        };
+
+        let json = data_encoding::BASE64
+            .decode(encoded.as_bytes())
+            .context("invalid base64 data")?;
+
+        Ok(serde_json::from_slice(&json)?)
+    }
+}
+
 lazy_static! {
     static ref CONFIG: Mutex<Option<Arc<Config>>> = Mutex::new(None);
 }
 
 /// Represents the `sentry-cli` config.
 pub struct Config {
     filename: PathBuf,
     process_bound: bool,
     ini: Ini,
     cached_auth: Option<Auth>,
     cached_base_url: String,
     cached_headers: Option<Vec<String>>,
     cached_log_level: log::LevelFilter,
     cached_vcs_remote: String,
+    cached_token_data: Option<TokenData>,
 }
 
 impl Config {
     /// Loads the CLI config from the default location and returns it.
     pub fn from_cli_config() -> Result<Config> {
         let (filename, ini) = load_cli_config()?;
         Config::from_file(filename, ini)
     }
 
     /// Creates Config based on provided config file.
     pub fn from_file(filename: PathBuf, ini: Ini) -> Result<Config> {
+        let auth = get_default_auth(&ini);
+        let token_embedded_data = match auth {
+            Some(Auth::Token(ref token)) => {
+                TokenData::decode(token).context("Failed to parse org auth token {token}")?
+            }
+            _ => None,
+        };
+
+        let mut url = get_default_url(&ini);
+
+        if let Some(ref token_embedded_data) = token_embedded_data {
+            if url == DEFAULT_URL || url.is_empty() {
+                url = token_embedded_data.url.clone();
+            } else if url != token_embedded_data.url {
+                bail!(
+                    "Two different url values supplied: `{}` (from token), `{url}`.",
+                    token_embedded_data.url,
+                );
+            }
+        }
+
         Ok(Config {
             filename,
             process_bound: false,
-            cached_auth: get_default_auth(&ini),
-            cached_base_url: get_default_url(&ini),
+            cached_auth: auth,
+            cached_base_url: url,
             cached_headers: get_default_headers(&ini),
             cached_log_level: get_default_log_level(&ini),
             cached_vcs_remote: get_default_vcs_remote(&ini),
             ini,
+            cached_token_data: token_embedded_data,
         })
     }
 
     /// Makes this config the process bound one that can be
     /// fetched from anywhere.
     pub fn bind_to_process(mut self) -> Arc<Config> {
         self.process_bound = true;
@@ -135,30 +196,39 @@
 
     /// Returns the auth info
     pub fn get_auth(&self) -> Option<&Auth> {
         self.cached_auth.as_ref()
     }
 
     /// Updates the auth info
-    pub fn set_auth(&mut self, auth: Auth) {
+    pub fn set_auth(&mut self, auth: Auth) -> Result<()> {
         self.cached_auth = Some(auth);
 
         self.ini.delete_from(Some("auth"), "api_key");
         self.ini.delete_from(Some("auth"), "token");
         match self.cached_auth {
             Some(Auth::Token(ref val)) => {
+                self.cached_token_data =
+                    TokenData::decode(val).context("Failed to parse org auth token {token}")?;
+
+                if let Some(ref data) = self.cached_token_data {
+                    self.cached_base_url = data.url.clone();
+                }
+
                 self.ini
                     .set_to(Some("auth"), "token".into(), val.to_string());
             }
             Some(Auth::Key(ref val)) => {
                 self.ini
                     .set_to(Some("auth"), "api_key".into(), val.to_string());
             }
             None => {}
         }
+
+        Ok(())
     }
 
     /// Returns the base url (without trailing slashes)
     pub fn get_base_url(&self) -> Result<&str> {
         let base = self.cached_base_url.trim_end_matches('/');
         if !is_absolute_url(base) {
             bail!("bad sentry url: unknown scheme ({})", base);
@@ -166,18 +236,27 @@
         if base.matches('/').count() != 2 {
             bail!("bad sentry url: not on URL root ({})", base);
         }
         Ok(base)
     }
 
     /// Sets the URL
-    pub fn set_base_url(&mut self, url: &str) {
+    pub fn set_base_url(&mut self, url: &str) -> Result<()> {
+        if let Some(ref org_token) = self.cached_token_data {
+            if url != org_token.url {
+                bail!(
+                    "Two different url values supplied: `{}` (from token), `{url}`.",
+                    org_token.url,
+                );
+            }
+        }
         self.cached_base_url = url.to_owned();
         self.ini
             .set_to(Some("defaults"), "url".into(), self.cached_base_url.clone());
+        Ok(())
     }
 
     /// Sets headers that should be attached to all requests
     pub fn set_headers(&mut self, headers: Vec<String>) {
         self.cached_headers = Some(headers);
     }
 
@@ -269,24 +348,43 @@
             None => true,
             Some(val) => val == "true",
         }
     }
 
     /// Given a match object from clap, this returns the org from it.
     pub fn get_org(&self, matches: &ArgMatches) -> Result<String> {
-        matches
+        let org_from_token = self.cached_token_data.as_ref().map(|t| &t.org);
+
+        let org_from_cli = matches
             .get_one::<String>("org")
             .cloned()
-            .or_else(|| env::var("SENTRY_ORG").ok())
-            .or_else(|| {
-                self.ini
-                    .get_from(Some("defaults"), "org")
-                    .map(str::to_owned)
-            })
-            .ok_or_else(|| format_err!("An organization slug is required (provide with --org)"))
+            .or_else(|| env::var("SENTRY_ORG").ok());
+
+        match (org_from_token, org_from_cli) {
+            (None, None) => self
+                .ini
+                .get_from(Some("defaults"), "org")
+                .map(str::to_owned)
+                .ok_or_else(|| {
+                    format_err!("An organization slug is required (provide with --org)")
+                }),
+            (None, Some(cli_org)) => Ok(cli_org),
+            (Some(token_org), None) => Ok(token_org.to_string()),
+            (Some(token_org), Some(cli_org)) => {
+                if cli_org.is_empty() {
+                    return Ok(token_org.to_owned());
+                }
+                if cli_org != *token_org {
+                    return Err(format_err!(
+                        "Two different org values supplied: `{token_org}` (from token), `{cli_org}`."
+                    ));
+                }
+                Ok(cli_org)
+            }
+        }
     }
 
     /// Given a match object from clap, this returns the release from it.
     pub fn get_release(&self, matches: &ArgMatches) -> Result<String> {
         matches
             .get_one::<String>("release")
             .cloned()
@@ -570,14 +668,15 @@
             process_bound: false,
             ini: self.ini.clone(),
             cached_auth: self.cached_auth.clone(),
             cached_base_url: self.cached_base_url.clone(),
             cached_headers: self.cached_headers.clone(),
             cached_log_level: self.cached_log_level,
             cached_vcs_remote: self.cached_vcs_remote.clone(),
+            cached_token_data: self.cached_token_data.clone(),
         }
     }
 }
 
 #[allow(clippy::manual_map)]
 fn get_default_auth(ini: &Ini) -> Option<Auth> {
     if let Ok(val) = env::var("SENTRY_AUTH_TOKEN") {
@@ -637,7 +736,25 @@
         remote
     } else if let Some(remote) = ini.get_from(Some("defaults"), "vcs_remote") {
         remote.to_string()
     } else {
         "origin".to_string()
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_decode_token_data() {
+        let token = "sntrys_eyJ1cmwiOiJodHRwczovL3NlbnRyeS5pbyIsIm9yZyI6InRlc3Qtb3JnIn0=_foobarthisdoesntmatter";
+
+        assert_eq!(
+            TokenData::decode(token).unwrap().unwrap(),
+            TokenData {
+                org: "test-org".to_string(),
+                url: "https://sentry.io".to_string(),
+            }
+        );
+    }
+}
```

### Comparing `sentry_cli-2.19.4/src/constants.rs` & `sentry_cli-2.20.0/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/android.rs` & `sentry_cli-2.20.0/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/appcenter.rs` & `sentry_cli-2.20.0/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/args.rs` & `sentry_cli-2.20.0/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/chunks.rs` & `sentry_cli-2.20.0/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/codepush.rs` & `sentry_cli-2.20.0/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/cordova.rs` & `sentry_cli-2.20.0/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/dif.rs` & `sentry_cli-2.20.0/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/dif_upload.rs` & `sentry_cli-2.20.0/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/enc.rs` & `sentry_cli-2.20.0/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/event.rs` & `sentry_cli-2.20.0/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/file_search.rs` & `sentry_cli-2.20.0/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/file_upload.rs` & `sentry_cli-2.20.0/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/formatting.rs` & `sentry_cli-2.20.0/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/fs.rs` & `sentry_cli-2.20.0/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/http.rs` & `sentry_cli-2.20.0/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/logging.rs` & `sentry_cli-2.20.0/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/progress.rs` & `sentry_cli-2.20.0/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/releases.rs` & `sentry_cli-2.20.0/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/retry.rs` & `sentry_cli-2.20.0/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.20.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.20.0/src/utils/sourcemaps/inject.rs`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 use regex::Regex;
 use symbolic::common::{clean_path, join_path};
 
 use std::fmt;
 use std::io::{BufRead, Write};
 use std::path::PathBuf;
 
-use anyhow::{bail, Result};
+use anyhow::{bail, Context, Result};
 use lazy_static::lazy_static;
 use log::debug;
 use sentry::types::DebugId;
 use serde_json::Value;
 
 const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}();"#;
 const DEBUGID_PLACEHOLDER: &str = "__SENTRY_DEBUG_ID__";
-const SOURCEMAP_DEBUGID_KEY: &str = "debug_id";
 const DEBUGID_COMMENT_PREFIX: &str = "//# debugId";
 
 lazy_static! {
-    static ref USE_PRAGMA_RE: Regex = Regex::new(r#""use \w+";|'use \w+';"#).unwrap();
+    static ref USE_PRAGMA_RE: Regex = Regex::new(r#"^"use \w+";|^'use \w+';"#).unwrap();
 }
 
 fn print_section_with_debugid(
     f: &mut fmt::Formatter<'_>,
     title: &str,
     data: &[(PathBuf, DebugId)],
 ) -> fmt::Result {
@@ -299,35 +298,43 @@
 /// Fixes up a sourcemap file with a debug id.
 ///
 /// If the file already contains a debug id under the `debug_id` key, it is left unmodified.
 /// Otherwise, a fresh debug id is inserted under that key.
 ///
 /// In either case, the value of the `debug_id` key is returned.
 pub fn fixup_sourcemap(sourcemap_contents: &mut Vec<u8>) -> Result<(DebugId, bool)> {
-    let mut sourcemap: Value = serde_json::from_slice(sourcemap_contents)?;
-
-    let Some(map) = sourcemap.as_object_mut() else {
-        bail!("Invalid sourcemap");
-    };
-
-    match map.get(SOURCEMAP_DEBUGID_KEY) {
-        Some(id) => {
-            let debug_id = serde_json::from_value(id.clone())?;
-            debug!("Sourcemap already has a debug id");
-            Ok((debug_id, false))
+    match sourcemap::decode_slice(sourcemap_contents).context("Invalid sourcemap")? {
+        sourcemap::DecodedMap::Regular(mut sm) => {
+            if let Some(debug_id) = sm.get_debug_id() {
+                debug!("Sourcemap already has a debug id");
+                Ok((debug_id, false))
+            } else {
+                let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
+                sm.set_debug_id(Some(debug_id));
+
+                sourcemap_contents.clear();
+                sm.to_writer(sourcemap_contents)?;
+                Ok((debug_id, true))
+            }
         }
-
-        None => {
-            let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
-            let id = serde_json::to_value(debug_id)?;
-            map.insert(SOURCEMAP_DEBUGID_KEY.to_string(), id);
-
-            sourcemap_contents.clear();
-            serde_json::to_writer(sourcemap_contents, &sourcemap)?;
-            Ok((debug_id, true))
+        sourcemap::DecodedMap::Hermes(mut smh) => {
+            if let Some(debug_id) = smh.get_debug_id() {
+                debug!("Sourcemap already has a debug id");
+                Ok((debug_id, false))
+            } else {
+                let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
+                smh.set_debug_id(Some(debug_id));
+
+                sourcemap_contents.clear();
+                smh.to_writer(sourcemap_contents)?;
+                Ok((debug_id, true))
+            }
+        }
+        sourcemap::DecodedMap::Index(_) => {
+            bail!("DebugId injection is not supported for sourcemap indexes")
         }
     }
 }
 
 /// This adds an empty mapping at the start of a sourcemap.
 ///
 /// This is used to adjust a sourcemap when the corresponding source file has a
@@ -374,23 +381,77 @@
     while joined[cutoff..].starts_with("./") {
         cutoff += 2;
     }
 
     format!("{}{}", &joined[..cutoff], clean_path(&joined[cutoff..]))
 }
 
+/// Returns a list of those paths among `candidate_paths` that differ from `expected_path` in
+/// at most one segment (modulo `.` segments).
+///
+/// The differing segment cannot be the last one (i.e., the filename).
+///
+/// If `expected_path` occurs among the `candidate_paths`, no other paths will be returned since
+/// that is considered a unique best match.
+///
+/// The intended usecase is finding sourcemaps even if they reside in a different directory; see
+/// the `test_find_matching_paths_sourcemaps` test for a minimal example.
+pub fn find_matching_paths(candidate_paths: &[String], expected_path: &str) -> Vec<String> {
+    let mut matches = Vec::new();
+    for candidate in candidate_paths {
+        let mut expected_segments = expected_path
+            .split('/')
+            .filter(|&segment| segment != ".")
+            .peekable();
+        let mut candidate_segments = candidate
+            .split('/')
+            .filter(|&segment| segment != ".")
+            .peekable();
+
+        // If there is a candidate that is exactly equal to the goal path,
+        // return only that one.
+        if Iterator::eq(candidate_segments.clone(), expected_segments.clone()) {
+            return vec![candidate.clone()];
+        }
+
+        // Iterate through both paths and discard segments so long as they are equal.
+        while candidate_segments
+            .peek()
+            .zip(expected_segments.peek())
+            .map_or(false, |(x, y)| x == y)
+        {
+            candidate_segments.next();
+            expected_segments.next();
+        }
+
+        // The next segments (if there are any left) must be where the paths disagree.
+        candidate_segments.next();
+        expected_segments.next();
+
+        // The rest of both paths must agree and be nonempty, so at least the filenames definitely
+        // must agree.
+        if candidate_segments.peek().is_some()
+            && Iterator::eq(candidate_segments, expected_segments)
+        {
+            matches.push(candidate.clone());
+        }
+    }
+
+    matches
+}
+
 #[cfg(test)]
 mod tests {
     use std::io::Write;
 
     use sentry::types::DebugId;
 
     use crate::utils::fs::TempFile;
 
-    use super::{fixup_js_file, fixup_sourcemap, normalize_sourcemap_url, replace_sourcemap_url};
+    use super::*;
 
     #[test]
     fn test_fixup_sourcemap() {
         for sourcemap_path in &[
             "server/chunks/1.js.map",
             "server/edge-runtime-webpack.js.map",
             "server/pages/_document.js.map",
@@ -512,15 +573,15 @@
 
     #[test]
     fn test_fixup_js_file_use_strict() {
         let source = r#"#!/bin/node
 //# sourceMappingURL=fake1
 
   // some other comment
- "use strict"; rest of the line
+"use strict"; rest of the line
 'use strict';
 some line
 //# sourceMappingURL=fake2
 //# sourceMappingURL=real
 something else"#;
 
         let debug_id = DebugId::default();
@@ -529,28 +590,64 @@
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"#!/bin/node
 //# sourceMappingURL=fake1
 
   // some other comment
- "use strict"; rest of the line
+"use strict"; rest of the line
 'use strict';
 !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
 some line
 //# sourceMappingURL=fake2
 something else
 //# debugId=00000000-0000-0000-0000-000000000000
 //# sourceMappingURL=real
 "#;
 
         assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
     }
 
     #[test]
+    fn test_fixup_js_file_fake_use_strict() {
+        let source = r#"#!/bin/node
+//# sourceMappingURL=fake1
+
+  // some other comment
+"use strict"; rest of the line
+(this.foo=this.bar||[]).push([[2],[function(e,t,n){"use strict"; […] }
+some line
+//# sourceMappingURL=fake2
+//# sourceMappingURL=real
+something else"#;
+
+        let debug_id = DebugId::default();
+
+        let mut source = Vec::from(source);
+
+        fixup_js_file(&mut source, debug_id).unwrap();
+
+        let expected = r#"#!/bin/node
+//# sourceMappingURL=fake1
+
+  // some other comment
+"use strict"; rest of the line
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}();
+(this.foo=this.bar||[]).push([[2],[function(e,t,n){"use strict"; […] }
+some line
+//# sourceMappingURL=fake2
+something else
+//# debugId=00000000-0000-0000-0000-000000000000
+//# sourceMappingURL=real
+"#;
+
+        assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
+    }
+
+    #[test]
     fn test_normalize_sourcemap_url() {
         assert_eq!(
             normalize_sourcemap_url("foo/bar/baz.js", "baz.js.map"),
             "foo/bar/baz.js.map"
         );
 
         assert_eq!(
@@ -597,8 +694,73 @@
 some text
 //@ sourceMappingURL=not this one either
 //# sourceMappingURL=new url
 more text
 "#;
         assert_eq!(std::str::from_utf8(&js_contents).unwrap(), expected);
     }
+
+    #[test]
+    fn test_find_matching_paths_unique() {
+        let expected = "./foo/bar/baz/quux";
+        let candidates = &[
+            "./foo/baz/quux".to_string(),
+            "foo/baar/baz/quux".to_string(),
+        ];
+
+        assert_eq!(
+            find_matching_paths(candidates, expected),
+            vec!["foo/baar/baz/quux"]
+        );
+
+        let candidates = &[
+            "./foo/baz/quux".to_string(),
+            "foo/baar/baz/quux".to_string(),
+            "./foo/bar/baz/quux".to_string(),
+        ];
+
+        assert_eq!(find_matching_paths(candidates, expected), vec![expected]);
+    }
+
+    #[test]
+    fn test_find_matching_paths_ambiguous() {
+        let expected = "./foo/bar/baz/quux";
+        let candidates = &[
+            "./foo/bar/baaz/quux".to_string(),
+            "foo/baar/baz/quux".to_string(),
+        ];
+
+        assert_eq!(find_matching_paths(candidates, expected), candidates,);
+    }
+
+    #[test]
+    fn test_find_matching_paths_filename() {
+        let expected = "./foo/bar/baz/quux";
+        let candidates = &[
+            "./foo/bar/baz/nop".to_string(),
+            "foo/baar/baz/quux".to_string(),
+        ];
+
+        assert_eq!(
+            find_matching_paths(candidates, expected),
+            ["foo/baar/baz/quux".to_string()]
+        );
+    }
+
+    #[test]
+    fn test_find_matching_paths_sourcemaps() {
+        let candidates = &[
+            "./project/maps/index.js.map".to_string(),
+            "./project/maps/page/index.js.map".to_string(),
+        ];
+
+        assert_eq!(
+            find_matching_paths(candidates, "project/code/index.js.map"),
+            &["./project/maps/index.js.map"]
+        );
+
+        assert_eq!(
+            find_matching_paths(candidates, "project/code/page/index.js.map"),
+            &["./project/maps/page/index.js.map"]
+        );
+    }
 }
```

### Comparing `sentry_cli-2.19.4/src/utils/sourcemaps.rs` & `sentry_cli-2.20.0/src/utils/sourcemaps.rs`

 * *Files 2% similar despite different names*

```diff
@@ -680,15 +680,15 @@
             &sources_checksums,
         ) {
             let already_uploaded_checksums: HashSet<_> = artifacts
                 .into_iter()
                 .filter_map(|artifact| Digest::from_str(&artifact.sha1).ok())
                 .collect();
 
-            for mut source in self.sources.values_mut() {
+            for source in self.sources.values_mut() {
                 if let Ok(checksum) = source.checksum() {
                     if already_uploaded_checksums.contains(&checksum) {
                         source.already_uploaded = true;
                         files_needing_upload -= 1;
                     }
                 }
             }
@@ -762,14 +762,21 @@
     /// for JavaScript files.
     pub fn inject_debug_ids(&mut self, dry_run: bool, js_extensions: &[&str]) -> Result<()> {
         self.flush_pending_sources();
         println!("{} Injecting debug ids", style(">").dim());
 
         let mut report = InjectReport::default();
 
+        let mut sourcemaps = self
+            .sources
+            .values()
+            .filter_map(|s| (s.ty == SourceFileType::SourceMap).then_some(s.url.clone()))
+            .collect::<Vec<_>>();
+        sourcemaps.sort();
+
         for (source_url, sourcemap_url) in self.sourcemap_references.iter_mut() {
             // We only allow injection into files that match the extension
             if !url_matches_extension(source_url, js_extensions) {
                 debug!(
                     "skipping potential js file {} because it does not match extension",
                     source_url
                 );
@@ -822,16 +829,30 @@
                             )?;
                             *sourcemap_url = new_sourcemap_url;
 
                             (debug_id, true)
                         } else {
                             // Handle external sourcemaps
 
-                            let sourcemap_url =
+                            let normalized =
                                 inject::normalize_sourcemap_url(source_url, sourcemap_url);
+                            let matches = inject::find_matching_paths(&sourcemaps, &normalized);
+
+                            let sourcemap_url = match &matches[..] {
+                                [] => normalized,
+                                [x] => x.to_string(),
+                                _ => {
+                                    warn!("Ambiguous matches for sourcemap path {normalized}:");
+                                    for path in matches {
+                                        warn!("{path}");
+                                    }
+                                    normalized
+                                }
+                            };
+
                             match self.sources.get_mut(&sourcemap_url) {
                                 None => {
                                     debug!("Sourcemap file {} not found", sourcemap_url);
                                     // source map cannot be found, fall back to hashing the contents if
                                     // available.  The v4 fallback should not happen.
                                     let debug_id = self
                                         .sources
@@ -975,58 +996,63 @@
 
 impl Default for SourceMapProcessor {
     fn default() -> Self {
         SourceMapProcessor::new()
     }
 }
 
-#[test]
-fn test_split_url() {
-    assert_eq!(split_url("/foo.js"), (Some(""), "foo", Some("js")));
-    assert_eq!(split_url("foo.js"), (None, "foo", Some("js")));
-    assert_eq!(split_url("foo"), (None, "foo", None));
-    assert_eq!(split_url("/foo"), (Some(""), "foo", None));
-    assert_eq!(
-        split_url("/foo.deadbeef0123.js"),
-        (Some(""), "foo", Some("deadbeef0123.js"))
-    );
-    assert_eq!(
-        split_url("/foo/bar/baz.js"),
-        (Some("/foo/bar"), "baz", Some("js"))
-    );
-}
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_split_url() {
+        assert_eq!(split_url("/foo.js"), (Some(""), "foo", Some("js")));
+        assert_eq!(split_url("foo.js"), (None, "foo", Some("js")));
+        assert_eq!(split_url("foo"), (None, "foo", None));
+        assert_eq!(split_url("/foo"), (Some(""), "foo", None));
+        assert_eq!(
+            split_url("/foo.deadbeef0123.js"),
+            (Some(""), "foo", Some("deadbeef0123.js"))
+        );
+        assert_eq!(
+            split_url("/foo/bar/baz.js"),
+            (Some("/foo/bar"), "baz", Some("js"))
+        );
+    }
 
-#[test]
-fn test_unsplit_url() {
-    assert_eq!(&unsplit_url(Some(""), "foo", Some("js")), "/foo.js");
-    assert_eq!(&unsplit_url(None, "foo", Some("js")), "foo.js");
-    assert_eq!(&unsplit_url(None, "foo", None), "foo");
-    assert_eq!(&unsplit_url(Some(""), "foo", None), "/foo");
-}
+    #[test]
+    fn test_unsplit_url() {
+        assert_eq!(&unsplit_url(Some(""), "foo", Some("js")), "/foo.js");
+        assert_eq!(&unsplit_url(None, "foo", Some("js")), "foo.js");
+        assert_eq!(&unsplit_url(None, "foo", None), "foo");
+        assert_eq!(&unsplit_url(Some(""), "foo", None), "/foo");
+    }
 
-#[test]
-fn test_join() {
-    assert_eq!(&join_url("app:///", "foo.html").unwrap(), "app:///foo.html");
-    assert_eq!(&join_url("app://", "foo.html").unwrap(), "app:///foo.html");
-    assert_eq!(&join_url("~/", "foo.html").unwrap(), "~/foo.html");
-    assert_eq!(
-        &join_url("app:///", "/foo.html").unwrap(),
-        "app:///foo.html"
-    );
-    assert_eq!(&join_url("app://", "/foo.html").unwrap(), "app:///foo.html");
-    assert_eq!(
-        &join_url("https:///example.com/", "foo.html").unwrap(),
-        "https://example.com/foo.html"
-    );
-    assert_eq!(
-        &join_url("https://example.com/", "foo.html").unwrap(),
-        "https://example.com/foo.html"
-    );
-}
+    #[test]
+    fn test_join() {
+        assert_eq!(&join_url("app:///", "foo.html").unwrap(), "app:///foo.html");
+        assert_eq!(&join_url("app://", "foo.html").unwrap(), "app:///foo.html");
+        assert_eq!(&join_url("~/", "foo.html").unwrap(), "~/foo.html");
+        assert_eq!(
+            &join_url("app:///", "/foo.html").unwrap(),
+            "app:///foo.html"
+        );
+        assert_eq!(&join_url("app://", "/foo.html").unwrap(), "app:///foo.html");
+        assert_eq!(
+            &join_url("https:///example.com/", "foo.html").unwrap(),
+            "https://example.com/foo.html"
+        );
+        assert_eq!(
+            &join_url("https://example.com/", "foo.html").unwrap(),
+            "https://example.com/foo.html"
+        );
+    }
 
-#[test]
-fn test_url_matches_extension() {
-    assert!(url_matches_extension("foo.js", &["js"][..]));
-    assert!(!url_matches_extension("foo.mjs", &["js"][..]));
-    assert!(url_matches_extension("foo.mjs", &["js", "mjs"][..]));
-    assert!(!url_matches_extension("js", &["js"][..]));
+    #[test]
+    fn test_url_matches_extension() {
+        assert!(url_matches_extension("foo.js", &["js"][..]));
+        assert!(!url_matches_extension("foo.mjs", &["js"][..]));
+        assert!(url_matches_extension("foo.mjs", &["js", "mjs"][..]));
+        assert!(!url_matches_extension("js", &["js"][..]));
+    }
 }
```

### Comparing `sentry_cli-2.19.4/src/utils/system.rs` & `sentry_cli-2.20.0/src/utils/system.rs`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,17 @@
     }
 
     eprintln!("{} {}", style("error:").red(), err);
     err.chain()
         .skip(1)
         .for_each(|cause| eprintln!("  {} {}", style("caused by:").dim(), cause));
 
-    if Config::current().get_log_level() < log::LevelFilter::Info {
+    if Config::current_opt().map_or(true, |config| {
+        config.get_log_level() < log::LevelFilter::Info
+    }) {
         eprintln!();
         eprintln!("{}", style("Add --log-level=[info|debug] or export SENTRY_LOG_LEVEL=[info|debug] to see more output.").dim());
         eprintln!(
             "{}",
             style("Please attach the full debug log to all bug reports.").dim()
         );
     }
```

### Comparing `sentry_cli-2.19.4/src/utils/ui.rs` & `sentry_cli-2.20.0/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/update.rs` & `sentry_cli-2.20.0/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/vcs.rs` & `sentry_cli-2.20.0/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.19.4/src/utils/xcode.rs` & `sentry_cli-2.20.0/src/utils/xcode.rs`

 * *Files identical despite different names*

