# Comparing `tmp/nuclear-1.4.2.tar.gz` & `tmp/nuclear-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclear-1.4.2.tar", last modified: Thu Jul  6 10:51:27 2023, max compression
+gzip compressed data, was "nuclear-1.4.3.tar", last modified: Mon Jul 24 08:07:56 2023, max compression
```

## Comparing `nuclear-1.4.2.tar` & `nuclear-1.4.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.2/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-06 10:51:27.382318 nuclear-1.4.2/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18082 2023-07-06 10:51:27.000000 nuclear-1.4.2/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      564 2023-04-07 09:00:07.000000 nuclear-1.4.2/nuclear/__init__.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/args/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/args_que.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/container.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/autocomplete/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/autocomplete/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/autocomplete/autocomplete.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.2/nuclear/autocomplete/install.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/builder/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/builder/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.2/nuclear/builder/builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.2/nuclear/builder/decorator_builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/builder/rule.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.2/nuclear/builder/rule_factory.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/builder/typedef.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/completers/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/completers/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/completers/file.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/help/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/help/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.2/nuclear/help/help.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/inspection/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.2/nuclear/inspection/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    12596 2023-07-06 10:47:26.000000 nuclear-1.4.2/nuclear/inspection/inspection.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/parser/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/context.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/error.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/parser/inject.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/internal_vars.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/keyword.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/matcher.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.2/nuclear/parser/parser.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/transform.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/parser/validate.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.2/nuclear/parser/value.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/shell/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.2/nuclear/shell/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.2/nuclear/shell/background_cmd.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.2/nuclear/shell/shell_utils.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/sublog/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.2/nuclear/sublog/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.2/nuclear/sublog/catch.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.2/nuclear/sublog/context_logger.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.2/nuclear/sublog/wrap_error.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/types/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/boolean.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/filesystem.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/time.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/utils/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.2/nuclear/utils/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.2/nuclear/utils/files.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/input.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.2/nuclear/utils/regex.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.2/nuclear/utils/shell.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/strings.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/time.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-07-06 10:50:19.000000 nuclear-1.4.2/nuclear/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear.egg-info/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-07-06 10:51:27.382318 nuclear-1.4.2/setup.cfg
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.2/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.3/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-24 08:07:56.484101 nuclear-1.4.3/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18082 2023-07-24 08:07:56.000000 nuclear-1.4.3/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.476101 nuclear-1.4.3/nuclear/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      564 2023-07-24 08:01:33.000000 nuclear-1.4.3/nuclear/__init__.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/args/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/args/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/args/args_que.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/args/container.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/autocomplete/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/autocomplete/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/autocomplete/autocomplete.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.3/nuclear/autocomplete/install.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/builder/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/builder/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.3/nuclear/builder/builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.3/nuclear/builder/decorator_builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.3/nuclear/builder/rule.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.3/nuclear/builder/rule_factory.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/builder/typedef.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/completers/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/completers/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/completers/file.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/help/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/help/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.3/nuclear/help/help.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear/inspection/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.3/nuclear/inspection/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    12673 2023-07-24 08:01:17.000000 nuclear-1.4.3/nuclear/inspection/inspection.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/nuclear/parser/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/context.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/error.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.3/nuclear/parser/inject.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/internal_vars.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/keyword.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/matcher.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.3/nuclear/parser/parser.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/parser/transform.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.3/nuclear/parser/validate.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.3/nuclear/parser/value.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/nuclear/shell/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.3/nuclear/shell/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.3/nuclear/shell/background_cmd.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.3/nuclear/shell/shell_utils.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/nuclear/sublog/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.3/nuclear/sublog/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.3/nuclear/sublog/catch.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.3/nuclear/sublog/context_logger.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.3/nuclear/sublog/wrap_error.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/nuclear/types/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/types/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/types/boolean.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/types/filesystem.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/types/time.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.484101 nuclear-1.4.3/nuclear/utils/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.3/nuclear/utils/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.3/nuclear/utils/files.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/utils/input.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.3/nuclear/utils/regex.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.3/nuclear/utils/shell.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/utils/strings.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.3/nuclear/utils/time.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-07-24 08:00:20.000000 nuclear-1.4.3/nuclear/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-24 08:07:56.480101 nuclear-1.4.3/nuclear.egg-info/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-24 08:07:56.000000 nuclear-1.4.3/nuclear.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-07-24 08:07:56.000000 nuclear-1.4.3/nuclear.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-07-24 08:07:56.000000 nuclear-1.4.3/nuclear.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-07-24 08:07:56.000000 nuclear-1.4.3/nuclear.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-07-24 08:07:56.000000 nuclear-1.4.3/nuclear.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-07-24 08:07:56.484101 nuclear-1.4.3/setup.cfg
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.3/setup.py
```

### Comparing `nuclear-1.4.2/LICENSE` & `nuclear-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/PKG-INFO` & `nuclear-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.2
+Version: 1.4.3
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nuclear-1.4.2/README.md` & `nuclear-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/__init__.py` & `nuclear-1.4.3/nuclear/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .builder.rule_factory import subcommand, flag, dictionary, parameter, primary_option, argument, arguments, \
     default_action
 from .shell.shell_utils import shell, shell_error_code, shell_output, CommandError
 from .shell.background_cmd import BackgroundCommand
 from .sublog.catch import logerr, ContextError, log_exception
 from .sublog.context_logger import log
 from .sublog.wrap_error import wrap_context
-from .inspection.inspection import inspect, wat, ins, insp
+from .inspection.inspection import inspect, ins, wat, wats
 
 from .version import __version__
 
 name = "nuclear"
```

### Comparing `nuclear-1.4.2/nuclear/args/args_que.py` & `nuclear-1.4.3/nuclear/args/args_que.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/autocomplete/autocomplete.py` & `nuclear-1.4.3/nuclear/autocomplete/autocomplete.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/autocomplete/install.py` & `nuclear-1.4.3/nuclear/autocomplete/install.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/builder/builder.py` & `nuclear-1.4.3/nuclear/builder/builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/builder/decorator_builder.py` & `nuclear-1.4.3/nuclear/builder/decorator_builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/builder/rule.py` & `nuclear-1.4.3/nuclear/builder/rule.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/builder/rule_factory.py` & `nuclear-1.4.3/nuclear/builder/rule_factory.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/completers/file.py` & `nuclear-1.4.3/nuclear/completers/file.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/help/help.py` & `nuclear-1.4.3/nuclear/help/help.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/inspection/inspection.py` & `nuclear-1.4.3/nuclear/inspection/inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,19 +49,14 @@
     :param all: whether to include all information
     """
     print(inspect_format(
         obj, short=short, dunder=dunder or all, long=long or all, docs=docs or all, code=code or all
     ))
 
 
-def insp(obj: Any, **kwargs):
-    """Inspect object's attributes (variables and methods)"""
-    inspect(obj, **kwargs)
-
-
 def ins(obj: Any, **kwargs):
     """Inspect object's short, elementary data: value, type, signature"""
     inspect(obj, short=True, **kwargs)
 
 
 def inspect_format(
     obj: Any,
@@ -76,14 +71,17 @@
 
     str_value = _format_value(obj)
     str_type = _format_type(type(obj))
     output: List[str] = [
         f'{STYLE_BRIGHT_BLUE}value:{RESET} {str_value}',
         f'{STYLE_BRIGHT_BLUE}type:{RESET} {STYLE_BRIGHT_YELLOW}{str_type}{RESET}',
     ]
+
+    if isinstance(obj, (list, dict, str, bytes, bytearray, tuple, set, frozenset, range)):
+        output.append(f'{STYLE_BRIGHT_BLUE}len:{RESET} {_format_value(len(obj))}')
  
     if callable(obj):
         name = getattr(obj, '__name__', '…')
         signature = _get_callable_signature(name, obj)
         output.append(f'{STYLE_BRIGHT_BLUE}signature:{RESET} {signature}')
 
     doc = _get_doc(obj, long=True)
@@ -353,14 +351,15 @@
     def __truediv__(self, other: Any): return self._react_with(other) # /
     def __lshift__(self, other: Any): return self._react_with(other)  # <<
     def __rshift__(self, other: Any): return self._react_with(other)  # >>
     def __or__(self, other: Any): return self._react_with(other)  # |
     def __lt__(self, other: Any): return self._react_with(other)  # <
 
 wat = Wat()
+wats = Wat(short=True)
 
 
 def _strip_color(text: str) -> str:
     return re.sub(r'\x1b\[\d+(;\d+)?m', '', text)
 
 
 RESET ='\033[0m'
```

### Comparing `nuclear-1.4.2/nuclear/parser/inject.py` & `nuclear-1.4.3/nuclear/parser/inject.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/parser/keyword.py` & `nuclear-1.4.3/nuclear/parser/keyword.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/parser/matcher.py` & `nuclear-1.4.3/nuclear/parser/matcher.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/parser/parser.py` & `nuclear-1.4.3/nuclear/parser/parser.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/parser/validate.py` & `nuclear-1.4.3/nuclear/parser/validate.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/parser/value.py` & `nuclear-1.4.3/nuclear/parser/value.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/shell/background_cmd.py` & `nuclear-1.4.3/nuclear/shell/background_cmd.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/shell/shell_utils.py` & `nuclear-1.4.3/nuclear/shell/shell_utils.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/sublog/catch.py` & `nuclear-1.4.3/nuclear/sublog/catch.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/sublog/context_logger.py` & `nuclear-1.4.3/nuclear/sublog/context_logger.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/sublog/wrap_error.py` & `nuclear-1.4.3/nuclear/sublog/wrap_error.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/types/time.py` & `nuclear-1.4.3/nuclear/types/time.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/utils/regex.py` & `nuclear-1.4.3/nuclear/utils/regex.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear/utils/strings.py` & `nuclear-1.4.3/nuclear/utils/strings.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/nuclear.egg-info/PKG-INFO` & `nuclear-1.4.3/nuclear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.2
+Version: 1.4.3
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nuclear-1.4.2/nuclear.egg-info/SOURCES.txt` & `nuclear-1.4.3/nuclear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.2/setup.py` & `nuclear-1.4.3/setup.py`

 * *Files identical despite different names*

