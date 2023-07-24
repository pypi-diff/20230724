# Comparing `tmp/codechecker-6.22.1.tar.gz` & `tmp/codechecker-6.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codechecker-6.22.1.tar", last modified: Wed Apr 19 13:51:05 2023, max compression
+gzip compressed data, was "codechecker-6.22.2.tar", last modified: Thu Jul 13 15:52:45 2023, max compression
```

## Comparing `codechecker-6.22.1.tar` & `codechecker-6.22.2.tar`

### file list

```diff
@@ -1,573 +1,572 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/
--rw-r--r--   0 runner    (1001) docker     (122)    12262 2023-04-19 13:47:50.000000 codechecker-6.22.1/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-19 13:47:50.000000 codechecker-6.22.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    28188 2023-04-19 13:51:05.140489 codechecker-6.22.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.052488 codechecker-6.22.1/analyzer/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.044488 codechecker-6.22.1/analyzer/tools/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.044488 codechecker-6.22.1/analyzer/tools/build-logger/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.052488 codechecker-6.22.1/analyzer/tools/build-logger/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-hooks.c
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-hooks.h
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-logger.c
--rw-r--r--   0 runner    (1001) docker     (122)    15010 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool-gcc.c
--rw-r--r--   0 runner    (1001) docker     (122)     7949 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool-javac.c
--rw-r--r--   0 runner    (1001) docker     (122)     3898 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool.c
--rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool.h
--rw-r--r--   0 runner    (1001) docker     (122)    13629 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-util.c
--rw-r--r--   0 runner    (1001) docker     (122)     8851 2023-04-19 13:47:50.000000 codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-util.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.044488 codechecker-6.22.1/build_dist/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.048488 codechecker-6.22.1/build_dist/CodeChecker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.052488 codechecker-6.22.1/build_dist/CodeChecker/config/
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/analyzer_version.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/commands.json
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/config.json
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/config.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.052488 codechecker-6.22.1/build_dist/CodeChecker/config/config_files/
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/config_files/codechecker.json
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/config_files/codechecker.yml
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/git_commit_urls.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.052488 codechecker-6.22.1/build_dist/CodeChecker/config/labels/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.056488 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/asan.json
--rw-r--r--   0 runner    (1001) docker     (122)   246133 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/clang-tidy.json
--rw-r--r--   0 runner    (1001) docker     (122)    34768 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/clangsa.json
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/coccinelle.json
--rw-r--r--   0 runner    (1001) docker     (122)    26460 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/cppcheck.json
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/golint.json
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/kernel-doc.json
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/lsan.json
--rw-r--r--   0 runner    (1001) docker     (122)     6776 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/mdl.json
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/msan.json
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/pyflakes.json
--rw-r--r--   0 runner    (1001) docker     (122)    23053 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/pylint.json
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/smatch.json
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/sparse.json
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/sphinx.json
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/tsan.json
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/ubsan.json
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/labels/descriptions.json
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/logger.conf
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/package_layout.json
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/server_config.json
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/session_client.json
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/system_comment_kinds.json
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/config/web_version.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.044488 codechecker-6.22.1/build_dist/CodeChecker/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.048488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.056488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/bazel_compile_commands/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/bazel_compile_commands/__init__.py
--rwxr--r--   0 runner    (1001) docker     (122)     8862 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/bazel_compile_commands/bazel_compile_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.056488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28188 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    36821 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-19 13:51:04.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.056488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    31150 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    12959 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10256 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.060488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5421 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8926 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.060488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18529 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5225 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/clang_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_autodetection.py
--rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_triple_arch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/statistics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2907 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.060488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20559 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2658 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    11079 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/config_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.060488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14806 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/flag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6629 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/result_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4781 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.060488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_action.py
--rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/host_check.py
--rw-r--r--   0 runner    (1001) docker     (122)    48779 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/log_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/checkers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    52765 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4020 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzer_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     8234 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzers.py
--rw-r--r--   0 runner    (1001) docker     (122)    45984 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/check.py
--rw-r--r--   0 runner    (1001) docker     (122)    21094 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/checkers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15470 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/fixit.py
--rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/log.py
--rw-r--r--   0 runner    (1001) docker     (122)    18063 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     7379 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/compilation_database.py
--rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/env.py
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/gcc_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/host_check.py
--rw-r--r--   0 runner    (1001) docker     (122)    13211 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/makefile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7902 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/pre_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5010 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   115795 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/codeCheckerAuthentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20342 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14120 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/configurationService.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57448 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/codeCheckerProductService.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    22012 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.064488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/serverInfoService.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.068488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   538314 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/codeCheckerDBAccess.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)   183676 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.068488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api_shared/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api_shared/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-03-01 14:14:21.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api_shared/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.068488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4064 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/blame_info.py
--rw-r--r--   0 runner    (1001) docker     (122)    10046 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.068488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    69073 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)    31639 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line.py
--rw-r--r--   0 runner    (1001) docker     (122)    59220 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/credential_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/product.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/results.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/permission_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/product.py
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/product_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/report_type_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/source_component_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/suppress_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/thrift_call.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/token_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/arg.py
--rw-r--r--   0 runner    (1001) docker     (122)    10733 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/checker_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8646 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3696 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6186 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/output/
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/skiplist_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/__init__.py
--rwxr--r--   0 runner    (1001) docker     (122)     2573 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3158 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/merge_clang_extdef_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5803 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.072488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      871 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     5567 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1905 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.076488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4341 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/analyzer_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6000 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/analyzer_result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.080489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/analyzer_result.py
--rwxr--r--   0 runner    (1001) docker     (122)     9318 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/
--rw-r--r--   0 runner    (1001) docker     (122)    18196 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/checker_labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     7100 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/baseline.py
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/codeclimate.py
--rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/gerrit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    19532 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/html.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/buglist.css
--rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/bugview.css
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/icon.css
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/statistics.css
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/table.css
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/browsersupport.js
--rw-r--r--   0 runner    (1001) docker     (122)     4505 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/buglist.js
--rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/bugviewer.js
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/layout.html
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/statistics.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.048488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/
--rw-r--r--   0 runner    (1001) docker     (122)    18240 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/clike.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   166305 2023-04-19 13:48:18.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     6673 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/plaintext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.084488 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23989 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/plist.py
--rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/report_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/statistics.py
--rw-r--r--   0 runner    (1001) docker     (122)    12533 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/source_code_comment_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5869 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/twodim.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16040 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2865 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    56436 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/mass_store_run.py
--rw-r--r--   0 runner    (1001) docker     (122)    25999 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/product_server.py
--rw-r--r--   0 runner    (1001) docker     (122)   148077 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/report_server.py
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/server_info_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/thrift_enum_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16154 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_ldap.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_pam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    40187 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5339 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/config_db_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    22520 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/database.py
--rw-r--r--   0 runner    (1001) docker     (122)     9646 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/db_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (122)    18645 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/run_db_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/instance_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     8900 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.088489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.092489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/env.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.092489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/126fa3f55e4b_added_permission_for_product_view.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/150800b30447_share_sessions_through_the_database.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/302693c76eb8_remove_db_version_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      980 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/3335ff7593cc_disable_review_status_change.py
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4964142b58d2_authentication_session_tokens.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4db450cf38af_add_extra_product_detail_columns.py
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/6b9f832d0b20_add_user_name_and_group_to_session.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/7829789fc19c_global_permission_to_get_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/8268fc7ca7f4_initial_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/bb5278995f41_run_limitation_for_products.py
--rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/cf025b6d7998_add_confidentiality.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/dec6feb991e6_new_table_for_server_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.092489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/env.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/080349e895d7_add_check_command_to_run_history.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/101a9cb747de_add_bug_event_and_point_report_index.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/2185167f8568_content_hash_index_for_files.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3793e361a752_source_components.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/39f9e96071c0_analyzer_statistics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3e91d0612422_off_and_unavailable_detection_statuses.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/4b38fa14c27b_file_id_index_for_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/5f8a443a51e5_add_description_for_run_history.py
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/6cb6a3a41967_system_comments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/75ae226b5d88_review_status_for_each_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/82ca43f05c10_initial_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9987aa593ca7_add_codechecker_version_to_run_history.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9d956a0fae8d_report_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a24461972d2e_add_index_for_report_and_history_id_columns.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a79677f54e48_remove_db_version_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/ad2a567e513a_git_blame_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/af5d8a21c1e4_add_analyzer_name_for_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/c042e02cca99_extended_report_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dabc6998b8f0_analysis_info_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dd9c97ead24_share_the_locking_of_runs.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/e89887e7d3f0_add_bug_path_length.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/f8291ab1d6be_fix_setting_analysis_info_id_seq.py
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/fb356f0eefed_cleanup_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)    27198 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/profiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/routing.py
--rw-r--r--   0 runner    (1001) docker     (122)    43638 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    29582 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/__init__.py
--rwxr--r--   0 runner    (1001) docker     (122)     3962 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/return_value.py
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/special_return_value.py
--rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-04-19 13:48:19.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/post_process_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4503 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/web_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/database_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/env.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/host_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/pgpass.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7448 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/webserver_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.096489 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/tu_collector/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/tu_collector/__init__.py
--rwxr--r--   0 runner    (1001) docker     (122)    23361 2023-04-19 13:47:50.000000 codechecker-6.22.1/build_dist/CodeChecker/lib/python3/tu_collector/tu_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.120489 codechecker-6.22.1/build_dist/CodeChecker/www/
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/07c4c8ad1e67dd03142f8a3f10cf0c1d.png
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/198.71b517a7d103c8182680.js
--rw-r--r--   0 runner    (1001) docker     (122)    43824 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/204.48d4cf3235458f4f48b8.js
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/257.2fb64e335d3132937e67.js
--rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/287.0bc0c02a80fc6fec452e.js
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/291.5a3df2fbabd931cce421.js
--rw-r--r--   0 runner    (1001) docker     (122)   273189 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/2d39422cd3aa08e2c9d27844e52cf651.png
--rw-r--r--   0 runner    (1001) docker     (122)    30271 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/3408d5e44bc83a8a65abfaab3db59b34.png
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/343.e2548aa08e829c446317.js
--rw-r--r--   0 runner    (1001) docker     (122)    83388 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/437c4ff8b03d221ca7112e93dd271271.png
--rw-r--r--   0 runner    (1001) docker     (122)    87663 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/452.49b8e5bc5792d6509d2d.js
--rw-r--r--   0 runner    (1001) docker     (122)    17700 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/455.0a5796cf6fe665353148.js
--rw-r--r--   0 runner    (1001) docker     (122)   105730 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/5857a166c7017a15b8caedeed9b85c88.png
--rw-r--r--   0 runner    (1001) docker     (122)    21843 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/608.57f5c652f7cf87d221c0.js
--rw-r--r--   0 runner    (1001) docker     (122)    59238 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/60b2da9aea5224169d569c59129b6aea.png
--rw-r--r--   0 runner    (1001) docker     (122)    29433 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/680.fd2ce6a69f228ec1a2d0.js
--rw-r--r--   0 runner    (1001) docker     (122)    70005 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/72d28790afb57a543ab3215b7fcff696.png
--rw-r--r--   0 runner    (1001) docker     (122)     4798 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/771.a2b39dd451456852d62a.js
--rw-r--r--   0 runner    (1001) docker     (122)    18465 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/77db62d20f442ca57ed2fba2bb8bdf0d.png
--rw-r--r--   0 runner    (1001) docker     (122)    36957 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/808.1a0aee7cc43bc809830d.js
--rw-r--r--   0 runner    (1001) docker     (122)    39055 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/820.ef2aa58b90057d1d858f.js
--rw-r--r--   0 runner    (1001) docker     (122)    35010 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/83e0246ba1dc6bed1c4c6ef2bb708e6d.png
--rw-r--r--   0 runner    (1001) docker     (122)    16631 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/840.3f6ddcfae65b29844150.js
--rw-r--r--   0 runner    (1001) docker     (122)    10709 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/8b0b574430b7d19d0afcaf576a964c21.png
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/91.f30e841add2c06736bcc.js
--rw-r--r--   0 runner    (1001) docker     (122)    68487 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/960.69e3e9a01225afeb6d5a.js
--rw-r--r--   0 runner    (1001) docker     (122)    40817 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/bc9b37bfe8ed72f234a5972c2c45239c.png
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/browsersupport.js
--rw-r--r--   0 runner    (1001) docker     (122)    19283 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/d7ffbebc7a4edf70373bbc18d3ca66cf.png
--rw-r--r--   0 runner    (1001) docker     (122)    32519 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/e528e8e6e67ca7bdcbb707be99615dba.png
--rw-r--r--   0 runner    (1001) docker     (122)   225798 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/efdadec91f4d830906939a930fc180aa.png
--rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.048488 codechecker-6.22.1/build_dist/CodeChecker/www/images/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.048488 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.120489 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.10.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10709 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.10.0/bug_path_length_filter.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.120489 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.17.0/
--rw-r--r--   0 runner    (1001) docker     (122)   273189 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.17.0/git_blame.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.120489 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    70005 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.7.0/component_filter.png
--rw-r--r--   0 runner    (1001) docker     (122)   225798 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.7.0/plist_to_html_index.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.124489 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)    83388 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.8.0/analysis_statistics.png
--rw-r--r--   0 runner    (1001) docker     (122)    59238 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.8.0/report_hash_filter.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.124489 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)    30271 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.9.1/macro_expansion.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.128489 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/
--rw-r--r--   0 runner    (1001) docker     (122)    14363 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/confidentiality.png
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/disable_review_status_change.png
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/edit_announcement_btn.png
--rw-r--r--   0 runner    (1001) docker     (122)    51288 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/edit_product.png
--rw-r--r--   0 runner    (1001) docker     (122)    35938 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/new_product.png
--rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/no_permission.png
--rw-r--r--   0 runner    (1001) docker     (122)     9497 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/notificaiton_dialog.png
--rw-r--r--   0 runner    (1001) docker     (122)    10540 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/notification.png
--rw-r--r--   0 runner    (1001) docker     (122)    31194 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/product_permissions.png
--rw-r--r--   0 runner    (1001) docker     (122)   110551 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/products.png
--rw-r--r--   0 runner    (1001) docker     (122)    25550 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/products/remove_product.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.132489 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/
--rw-r--r--   0 runner    (1001) docker     (122)   118986 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/bug_path.png
--rw-r--r--   0 runner    (1001) docker     (122)    19414 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/button_pane.png
--rw-r--r--   0 runner    (1001) docker     (122)    40847 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/checker_documentation.png
--rw-r--r--   0 runner    (1001) docker     (122)    41255 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/comment.png
--rw-r--r--   0 runner    (1001) docker     (122)    53754 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/report_navigation_tree.png
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_change.png
--rw-r--r--   0 runner    (1001) docker     (122)     9725 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_message.png
--rw-r--r--   0 runner    (1001) docker     (122)    11572 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_unreviewed.png
--rw-r--r--   0 runner    (1001) docker     (122)    11274 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/report/same_reports.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.136489 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/
--rw-r--r--   0 runner    (1001) docker     (122)    29002 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/assign_report_to_cleanup_plan.png
--rw-r--r--   0 runner    (1001) docker     (122)    40817 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/assign_reports_to_cleanup_plan.png
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/cleanup_plan_filter.png
--rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/clear_all_filters.png
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/clear_report_filters.png
--rw-r--r--   0 runner    (1001) docker     (122)    34503 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/compare_runs.png
--rw-r--r--   0 runner    (1001) docker     (122)    35010 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/compare_tags.png
--rw-r--r--   0 runner    (1001) docker     (122)    74119 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.png
--rw-r--r--   0 runner    (1001) docker     (122)    50119 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.svg
--rw-r--r--   0 runner    (1001) docker     (122)     6883 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_statuses.png
--rw-r--r--   0 runner    (1001) docker     (122)    25289 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/filter_runs.png
--rw-r--r--   0 runner    (1001) docker     (122)    64739 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/filters.png
--rw-r--r--   0 runner    (1001) docker     (122)    32519 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/list_of_cleanup_plans.png
--rw-r--r--   0 runner    (1001) docker     (122)    19283 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/list_of_source_components.png
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/manage_source_components.png
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/remove_filtered_reports.png
--rw-r--r--   0 runner    (1001) docker     (122)   405260 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/reports.png
--rw-r--r--   0 runner    (1001) docker     (122)     7296 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/review_statuses.png
--rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/severity_levels.png
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/unqiue_reports.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.136489 codechecker-6.22.1/build_dist/CodeChecker/www/images/review_status_rules/
--rw-r--r--   0 runner    (1001) docker     (122)    55319 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/review_status_rules/review_status.rules.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/
--rw-r--r--   0 runner    (1001) docker     (122)   127483 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/analyzer_statistics.png
--rw-r--r--   0 runner    (1001) docker     (122)    18301 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/check_command.png
--rw-r--r--   0 runner    (1001) docker     (122)    64219 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/compare_runs.png
--rw-r--r--   0 runner    (1001) docker     (122)    40814 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/delete_runs.png
--rw-r--r--   0 runner    (1001) docker     (122)    52678 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/filter_run_history_events.png
--rw-r--r--   0 runner    (1001) docker     (122)    15735 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/filter_runs.png
--rw-r--r--   0 runner    (1001) docker     (122)   100697 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/runs.png
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_analyzer_statistics_btn.png
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_check_command_btn.png
--rw-r--r--   0 runner    (1001) docker     (122)    12000 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_description.png
--rw-r--r--   0 runner    (1001) docker     (122)    63857 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_run_history.png
--rw-r--r--   0 runner    (1001) docker     (122)     4156 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/sort_runs.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/
--rw-r--r--   0 runner    (1001) docker     (122)   105730 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/checker_statistics.png
--rw-r--r--   0 runner    (1001) docker     (122)    43632 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/component_statistics.png
--rw-r--r--   0 runner    (1001) docker     (122)   137141 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/component_statistics_expanded.png
--rw-r--r--   0 runner    (1001) docker     (122)   177254 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/product_overview.png
--rw-r--r--   0 runner    (1001) docker     (122)    49552 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/severity_statistics.png
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/index.html
--rw-r--r--   0 runner    (1001) docker     (122)   266698 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/main.176c47b086909cc3937b.js
--rw-r--r--   0 runner    (1001) docker     (122)  1147844 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.5d42b4e.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   521080 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.5dff34d.woff
--rw-r--r--   0 runner    (1001) docker     (122)   361384 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.606b164.woff2
--rw-r--r--   0 runner    (1001) docker     (122)  1148064 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.e044ed2.eot
--rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/runtime.78a99b5041c202c0a7ed.js
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/static.js
--rw-r--r--   0 runner    (1001) docker     (122)  3324916 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-04-19 13:51:02.000000 codechecker-6.22.1/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    23459 2023-04-19 13:47:50.000000 codechecker-6.22.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1607 2023-04-19 13:47:50.000000 codechecker-6.22.1/scripts/gerrit_changed_files_to_skipfile.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 13:51:05.140489 codechecker-6.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-04-19 13:48:16.000000 codechecker-6.22.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 13:51:05.140489 codechecker-6.22.1/web/
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-04-19 13:47:50.000000 codechecker-6.22.1/web/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    12262 2023-07-13 15:48:35.000000 codechecker-6.22.2/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-13 15:48:35.000000 codechecker-6.22.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    28188 2023-07-13 15:52:45.874900 codechecker-6.22.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.782900 codechecker-6.22.2/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.774900 codechecker-6.22.2/analyzer/tools/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.774900 codechecker-6.22.2/analyzer/tools/build-logger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.786900 codechecker-6.22.2/analyzer/tools/build-logger/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     5614 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-hooks.c
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-hooks.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-logger.c
+-rw-r--r--   0 runner    (1001) docker     (122)    15010 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool-gcc.c
+-rw-r--r--   0 runner    (1001) docker     (122)     7949 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool-javac.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3898 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool.h
+-rw-r--r--   0 runner    (1001) docker     (122)    13629 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-util.c
+-rw-r--r--   0 runner    (1001) docker     (122)     8851 2023-07-13 15:48:35.000000 codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-util.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.774900 codechecker-6.22.2/build_dist/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.782900 codechecker-6.22.2/build_dist/CodeChecker/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.786900 codechecker-6.22.2/build_dist/CodeChecker/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/analyzer_version.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/commands.json
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/config.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/config.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.786900 codechecker-6.22.2/build_dist/CodeChecker/config/config_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/config_files/codechecker.json
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/config_files/codechecker.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/git_commit_urls.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.786900 codechecker-6.22.2/build_dist/CodeChecker/config/labels/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.790900 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/asan.json
+-rw-r--r--   0 runner    (1001) docker     (122)   254681 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/clang-tidy.json
+-rw-r--r--   0 runner    (1001) docker     (122)    34768 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/clangsa.json
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/coccinelle.json
+-rw-r--r--   0 runner    (1001) docker     (122)    26435 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/cppcheck.json
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/golint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/kernel-doc.json
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/lsan.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6776 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/mdl.json
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/msan.json
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/pyflakes.json
+-rw-r--r--   0 runner    (1001) docker     (122)    23053 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/smatch.json
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/sparse.json
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/sphinx.json
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/tsan.json
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/ubsan.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/labels/descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/logger.conf
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/package_layout.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/server_config.json
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/session_client.json
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/system_comment_kinds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/config/web_version.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.774900 codechecker-6.22.2/build_dist/CodeChecker/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.782900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.790900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/bazel_compile_commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/bazel_compile_commands/__init__.py
+-rwxr--r--   0 runner    (1001) docker     (122)     8862 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/bazel_compile_commands/bazel_compile_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.790900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28188 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    36730 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.794900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31311 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12938 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10551 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.794900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8554 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.794900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22537 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7573 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_autodetection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8353 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_triple_arch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2907 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.794900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22223 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2658 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10163 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/config_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.798900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15513 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6629 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/result_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4781 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.798900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6232 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2438 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/host_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48983 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/checkers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.798900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52765 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4020 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzer_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8063 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45984 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20909 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15470 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/fixit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18063 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7379 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/compilation_database.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/gcc_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/host_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13142 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7928 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/pre_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5010 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.798900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.798900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   115795 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/codeCheckerAuthentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20342 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.802900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14120 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/configurationService.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.802900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57448 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/codeCheckerProductService.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22012 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.802900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/serverInfoService.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.802900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   538314 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/codeCheckerDBAccess.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)   183676 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.802900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api_shared/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api_shared/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-13 15:52:45.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api_shared/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.806900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4064 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/blame_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10046 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.806900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69073 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31639 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59578 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/credential_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.806900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/product.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/permission_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/product.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/product_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/report_type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/source_component_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/suppress_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4490 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/thrift_call.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/token_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/arg.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10733 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/checker_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8646 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3696 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6186 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/output/
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/skiplist_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:49:11.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/__init__.py
+-rwxr--r--   0 runner    (1001) docker     (122)     2573 2023-07-13 15:49:11.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3158 2023-07-13 15:49:11.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/merge_clang_extdef_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5894 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5567 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.810900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1905 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1786 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.814900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/analyzer_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.818900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6017 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/analyzer_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/analyzer_result.py
+-rwxr--r--   0 runner    (1001) docker     (122)    10872 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/
+-rw-r--r--   0 runner    (1001) docker     (122)    18990 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/checker_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7310 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/codeclimate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/gerrit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19532 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/html.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.822900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/buglist.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2781 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/bugview.css
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/icon.css
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/statistics.css
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.826900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/browsersupport.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4505 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/buglist.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/bugviewer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/layout.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/statistics.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.778900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.826900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/
+-rw-r--r--   0 runner    (1001) docker     (122)    18240 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/clike.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   166305 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6673 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/plaintext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.826900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24271 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/plist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/report_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12533 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/source_code_comment_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5869 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/twodim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.826900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16040 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2865 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56629 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/mass_store_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25999 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/product_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)   148083 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/report_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/server_info_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/thrift_enum_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16154 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_pam.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40187 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5339 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/config_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22520 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9646 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/db_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18645 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/run_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/instance_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8900 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.830900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/env.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.834900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/126fa3f55e4b_added_permission_for_product_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/150800b30447_share_sessions_through_the_database.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/302693c76eb8_remove_db_version_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/3335ff7593cc_disable_review_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4964142b58d2_authentication_session_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4db450cf38af_add_extra_product_detail_columns.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/6b9f832d0b20_add_user_name_and_group_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/7829789fc19c_global_permission_to_get_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/8268fc7ca7f4_initial_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/bb5278995f41_run_limitation_for_products.py
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/cf025b6d7998_add_confidentiality.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/dec6feb991e6_new_table_for_server_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.834900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/env.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/080349e895d7_add_check_command_to_run_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/101a9cb747de_add_bug_event_and_point_report_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/2185167f8568_content_hash_index_for_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3793e361a752_source_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/39f9e96071c0_analyzer_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3e91d0612422_off_and_unavailable_detection_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/4b38fa14c27b_file_id_index_for_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/5f8a443a51e5_add_description_for_run_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/6cb6a3a41967_system_comments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/75ae226b5d88_review_status_for_each_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/82ca43f05c10_initial_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9987aa593ca7_add_codechecker_version_to_run_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9d956a0fae8d_report_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a24461972d2e_add_index_for_report_and_history_id_columns.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a79677f54e48_remove_db_version_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/ad2a567e513a_git_blame_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/af5d8a21c1e4_add_analyzer_name_for_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/c042e02cca99_extended_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dabc6998b8f0_analysis_info_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dd9c97ead24_share_the_locking_of_runs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/e89887e7d3f0_add_bug_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/f8291ab1d6be_fix_setting_analysis_info_id_seq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/fb356f0eefed_cleanup_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27198 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4474 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43638 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29582 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/__init__.py
+-rwxr--r--   0 runner    (1001) docker     (122)     3962 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/return_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/special_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2988 2023-07-13 15:49:12.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/post_process_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4503 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/web_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/database_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3223 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/host_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/pgpass.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7448 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/webserver_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.838900 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/tu_collector/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/tu_collector/__init__.py
+-rwxr--r--   0 runner    (1001) docker     (122)    23361 2023-07-13 15:48:35.000000 codechecker-6.22.2/build_dist/CodeChecker/lib/python3/tu_collector/tu_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/07c4c8ad1e67dd03142f8a3f10cf0c1d.png
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/198.71b517a7d103c8182680.js
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/257.2fb64e335d3132937e67.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/287.0bc0c02a80fc6fec452e.js
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/291.5a3df2fbabd931cce421.js
+-rw-r--r--   0 runner    (1001) docker     (122)   273189 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/2d39422cd3aa08e2c9d27844e52cf651.png
+-rw-r--r--   0 runner    (1001) docker     (122)    44465 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/324.780b5ed89944be295f22.js
+-rw-r--r--   0 runner    (1001) docker     (122)    30271 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/3408d5e44bc83a8a65abfaab3db59b34.png
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/343.e2548aa08e829c446317.js
+-rw-r--r--   0 runner    (1001) docker     (122)    83388 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/437c4ff8b03d221ca7112e93dd271271.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17728 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/455.f9ee007c1bcfd28541ae.js
+-rw-r--r--   0 runner    (1001) docker     (122)   105730 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/5857a166c7017a15b8caedeed9b85c88.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21843 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/608.57f5c652f7cf87d221c0.js
+-rw-r--r--   0 runner    (1001) docker     (122)    59238 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/60b2da9aea5224169d569c59129b6aea.png
+-rw-r--r--   0 runner    (1001) docker     (122)    29433 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/680.fd2ce6a69f228ec1a2d0.js
+-rw-r--r--   0 runner    (1001) docker     (122)    70005 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/72d28790afb57a543ab3215b7fcff696.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4798 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/771.a2b39dd451456852d62a.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18465 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/77db62d20f442ca57ed2fba2bb8bdf0d.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36957 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/808.1a0aee7cc43bc809830d.js
+-rw-r--r--   0 runner    (1001) docker     (122)    39055 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/820.ef2aa58b90057d1d858f.js
+-rw-r--r--   0 runner    (1001) docker     (122)    35010 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/83e0246ba1dc6bed1c4c6ef2bb708e6d.png
+-rw-r--r--   0 runner    (1001) docker     (122)    16631 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/840.3f6ddcfae65b29844150.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10709 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/8b0b574430b7d19d0afcaf576a964c21.png
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/91.f30e841add2c06736bcc.js
+-rw-r--r--   0 runner    (1001) docker     (122)    88615 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/950.87a139d7b44cf5913f38.js
+-rw-r--r--   0 runner    (1001) docker     (122)    68487 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/960.69e3e9a01225afeb6d5a.js
+-rw-r--r--   0 runner    (1001) docker     (122)    40817 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/bc9b37bfe8ed72f234a5972c2c45239c.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/browsersupport.js
+-rw-r--r--   0 runner    (1001) docker     (122)    19283 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/d7ffbebc7a4edf70373bbc18d3ca66cf.png
+-rw-r--r--   0 runner    (1001) docker     (122)    32519 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/e528e8e6e67ca7bdcbb707be99615dba.png
+-rw-r--r--   0 runner    (1001) docker     (122)   225798 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/efdadec91f4d830906939a930fc180aa.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.782900 codechecker-6.22.2/build_dist/CodeChecker/www/images/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.782900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.10.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10709 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.10.0/bug_path_length_filter.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.17.0/
+-rw-r--r--   0 runner    (1001) docker     (122)   273189 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.17.0/git_blame.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    70005 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.7.0/component_filter.png
+-rw-r--r--   0 runner    (1001) docker     (122)   225798 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.7.0/plist_to_html_index.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    83388 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.8.0/analysis_statistics.png
+-rw-r--r--   0 runner    (1001) docker     (122)    59238 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.8.0/report_hash_filter.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.858900 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    30271 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.9.1/macro_expansion.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.862900 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/
+-rw-r--r--   0 runner    (1001) docker     (122)    14363 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/confidentiality.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/disable_review_status_change.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/edit_announcement_btn.png
+-rw-r--r--   0 runner    (1001) docker     (122)    51288 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/edit_product.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35938 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/new_product.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/no_permission.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9497 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/notificaiton_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10540 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/notification.png
+-rw-r--r--   0 runner    (1001) docker     (122)    31194 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/product_permissions.png
+-rw-r--r--   0 runner    (1001) docker     (122)   110551 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/products.png
+-rw-r--r--   0 runner    (1001) docker     (122)    25550 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/products/remove_product.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.866901 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/
+-rw-r--r--   0 runner    (1001) docker     (122)   118986 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/bug_path.png
+-rw-r--r--   0 runner    (1001) docker     (122)    19414 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/button_pane.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40847 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/checker_documentation.png
+-rw-r--r--   0 runner    (1001) docker     (122)    41255 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/comment.png
+-rw-r--r--   0 runner    (1001) docker     (122)    53754 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/report_navigation_tree.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_change.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9725 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_message.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11572 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_unreviewed.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11274 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/report/same_reports.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.870900 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/
+-rw-r--r--   0 runner    (1001) docker     (122)    29002 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/assign_report_to_cleanup_plan.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40817 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/assign_reports_to_cleanup_plan.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/cleanup_plan_filter.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/clear_all_filters.png
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/clear_report_filters.png
+-rw-r--r--   0 runner    (1001) docker     (122)    34503 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/compare_runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)    35010 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/compare_tags.png
+-rw-r--r--   0 runner    (1001) docker     (122)    74119 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.png
+-rw-r--r--   0 runner    (1001) docker     (122)    50119 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     6883 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_statuses.png
+-rw-r--r--   0 runner    (1001) docker     (122)    25289 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/filter_runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)    64739 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/filters.png
+-rw-r--r--   0 runner    (1001) docker     (122)    32519 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/list_of_cleanup_plans.png
+-rw-r--r--   0 runner    (1001) docker     (122)    19283 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/list_of_source_components.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/manage_source_components.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/remove_filtered_reports.png
+-rw-r--r--   0 runner    (1001) docker     (122)   405260 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/reports.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7296 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/review_statuses.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/severity_levels.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/unqiue_reports.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.870900 codechecker-6.22.2/build_dist/CodeChecker/www/images/review_status_rules/
+-rw-r--r--   0 runner    (1001) docker     (122)    55319 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/review_status_rules/review_status.rules.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/
+-rw-r--r--   0 runner    (1001) docker     (122)   127483 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/analyzer_statistics.png
+-rw-r--r--   0 runner    (1001) docker     (122)    18301 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/check_command.png
+-rw-r--r--   0 runner    (1001) docker     (122)    64219 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/compare_runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40814 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/delete_runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)    52678 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/filter_run_history_events.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15735 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/filter_runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)   100697 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/runs.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4851 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_analyzer_statistics_btn.png
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_check_command_btn.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12000 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_description.png
+-rw-r--r--   0 runner    (1001) docker     (122)    63857 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_run_history.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4156 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/sort_runs.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/
+-rw-r--r--   0 runner    (1001) docker     (122)   105730 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/checker_statistics.png
+-rw-r--r--   0 runner    (1001) docker     (122)    43632 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/component_statistics.png
+-rw-r--r--   0 runner    (1001) docker     (122)   137141 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/component_statistics_expanded.png
+-rw-r--r--   0 runner    (1001) docker     (122)   177254 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/product_overview.png
+-rw-r--r--   0 runner    (1001) docker     (122)    49552 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/severity_statistics.png
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)   266697 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/main.42489517cdf5af8e5e0e.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1147844 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.5d42b4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   521080 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.5dff34d.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   361384 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.606b164.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)  1148064 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.e044ed2.eot
+-rw-r--r--   0 runner    (1001) docker     (122)     3222 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/runtime.e1b8e20cfbd50bdd0fef.js
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/static.js
+-rw-r--r--   0 runner    (1001) docker     (122)  3324916 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-13 15:52:38.000000 codechecker-6.22.2/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    23459 2023-07-13 15:48:35.000000 codechecker-6.22.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1607 2023-07-13 15:48:35.000000 codechecker-6.22.2/scripts/gerrit_changed_files_to_skipfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-13 15:52:45.874900 codechecker-6.22.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-07-13 15:49:08.000000 codechecker-6.22.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 15:52:45.874900 codechecker-6.22.2/web/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-13 15:48:35.000000 codechecker-6.22.2/web/requirements.txt
```

### Comparing `codechecker-6.22.1/LICENSE.TXT` & `codechecker-6.22.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/PKG-INFO` & `codechecker-6.22.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechecker
-Version: 6.22.1
+Version: 6.22.2
 Summary: CodeChecker is an analyzer tooling, defect database and viewer extension
 Home-page: https://github.com/Ericsson/CodeChecker
 Author: CodeChecker Team (Ericsson)
 Author-email: codechecker-tool@googlegroups.com
 License: Apache-2.0 WITH LLVM-exception
 Project-URL: Documentation, http://codechecker.readthedocs.io
 Project-URL: Issue Tracker, http://github.com/Ericsson/CodeChecker/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codechecker Version: 6.22.1 Summary: CodeChecker is
+Metadata-Version: 2.1 Name: codechecker Version: 6.22.2 Summary: CodeChecker is
 an analyzer tooling, defect database and viewer extension Home-page: https://
 github.com/Ericsson/CodeChecker Author: CodeChecker Team (Ericsson) Author-
 email: codechecker-tool@googlegroups.com License: Apache-2.0 WITH LLVM-
 exception Project-URL: Documentation, http://codechecker.readthedocs.io
 Project-URL: Issue Tracker, http://github.com/Ericsson/CodeChecker/issues
 Description:
                                     ******
```

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-logger.c` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-logger.c`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool-gcc.c` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool-gcc.c`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool-javac.c` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool-javac.c`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool.c` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool.c`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-tool.h` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-tool.h`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-util.c` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-util.c`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/analyzer/tools/build-logger/src/ldlogger-util.h` & `codechecker-6.22.2/analyzer/tools/build-logger/src/ldlogger-util.h`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/commands.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/commands.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/config.md` & `codechecker-6.22.2/build_dist/CodeChecker/config/config.md`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/config_files/codechecker.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/config_files/codechecker.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/config_files/codechecker.yml` & `codechecker-6.22.2/build_dist/CodeChecker/config/config_files/codechecker.yml`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/clang-tidy.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/clang-tidy.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909877433309301%*

 * *Differences: {"'labels'": "{'clang-diagnostic-always-inline-coroutine': "*

 * *             "['doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#walways-inline-coroutine', "*

 * *             "'severity:MEDIUM'], 'clang-diagnostic-array-parameter': "*

 * *             "['doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#warray-parameter', "*

 * *             "'severity:MEDIUM'], 'clang-diagnostic-atomic-access': "*

 * *             "['doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#watomic-access', "*

 * *       […]*

```diff
@@ -1064,14 +1064,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#walloca",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-alloca-with-align-alignof": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#walloca-with-align-alignof",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-always-inline-coroutine": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#walways-inline-coroutine",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-ambiguous-delete": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wambiguous-delete",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-ambiguous-ellipsis": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wambiguous-ellipsis",
             "severity:MEDIUM"
@@ -1144,14 +1148,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#warray-bounds",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-array-bounds-pointer-arithmetic": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#warray-bounds-pointer-arithmetic",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-array-parameter": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#warray-parameter",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-asm": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wasm",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-asm-operand-widths": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wasm-operand-widths",
             "severity:MEDIUM"
@@ -1168,14 +1176,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wat-protocol",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-atimport-in-framework-header": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#watimport-in-framework-header",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-atomic-access": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#watomic-access",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-atomic-alignment": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#watomic-alignment",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-atomic-implicit-seq-cst": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#watomic-implicit-seq-cst",
             "severity:MEDIUM"
@@ -1248,14 +1260,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbind-to-temporary-copy",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-binding-in-condition": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbinding-in-condition",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-bit-int-extension": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbit-int-extension",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-bitfield-constant-conversion": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbitfield-constant-conversion",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-bitfield-enum-conversion": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbitfield-enum-conversion",
             "severity:MEDIUM"
@@ -1292,14 +1308,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbool-operation",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-braced-scalar-init": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbraced-scalar-init",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-branch-protection": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbranch-protection",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-bridge-cast": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbridge-cast",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-builtin-assume-aligned-alignment": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wbuiltin-assume-aligned-alignment",
             "severity:MEDIUM"
@@ -1536,14 +1556,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcast-calling-convention",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-cast-function-type": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcast-function-type",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-cast-function-type-strict": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcast-function-type-strict",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-cast-of-sel-type": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcast-of-sel-type",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-cast-qual": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcast-qual",
             "severity:MEDIUM"
@@ -1660,14 +1684,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wconversion",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-conversion-null": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wconversion-null",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-coro-non-aligned-allocation-function": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcoro-non-aligned-allocation-function",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-coroutine": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcoroutine",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-coroutine-missing-unhandled-exception": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wcoroutine-missing-unhandled-exception",
             "severity:MEDIUM"
@@ -1772,14 +1800,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdelete-non-virtual-dtor",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-delimited-escape-sequence-extension": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdelimited-escape-sequence-extension",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecate-lax-vec-conv-all": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecate-lax-vec-conv-all",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-altivec-src-compat": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-altivec-src-compat",
             "severity:MEDIUM"
@@ -1792,14 +1824,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-array-compare",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-attributes": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-attributes",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecated-builtins": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-builtins",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated-comma-subscript": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-comma-subscript",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-copy": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-copy",
             "severity:MEDIUM"
@@ -1816,14 +1852,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-copy-with-user-provided-copy",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-copy-with-user-provided-dtor": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-copy-with-user-provided-dtor",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecated-coroutine": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-deprecated-coroutine",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated-declarations": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-declarations",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-dynamic-exception-spec": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-dynamic-exception-spec",
             "severity:MEDIUM"
@@ -1848,14 +1888,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-implementations",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-increment-bool": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-increment-bool",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecated-non-prototype": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-non-prototype",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated-objc-isa-usage": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-objc-isa-usage",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-objc-pointer-introspection": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-objc-pointer-introspection",
             "severity:MEDIUM"
@@ -1868,18 +1912,26 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-pragma",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-register": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-register",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecated-static-analyzer-flag": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-static-analyzer-flag",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated-this-capture": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-this-capture",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-deprecated-type": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-type",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-deprecated-volatile": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-volatile",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-deprecated-writable-strings": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdeprecated-writable-strings",
             "severity:MEDIUM"
@@ -1976,22 +2028,30 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wduplicate-method-match",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-duplicate-protocol": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wduplicate-protocol",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-dxil-validation": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdxil-validation",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-dynamic-class-memaccess": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdynamic-class-memaccess",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-dynamic-exception-spec": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wdynamic-exception-spec",
             "severity:HIGH"
         ],
+        "clang-diagnostic-eager-load-cxx-named-modules": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#weager-load-cxx-named-modules",
+            "severity:HIGH"
+        ],
         "clang-diagnostic-effc++": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#weffc",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-elaborated-enum-base": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#welaborated-enum-base",
             "severity:HIGH"
@@ -2036,14 +2096,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wenum-compare-conditional",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-enum-compare-switch": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wenum-compare-switch",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-enum-constexpr-conversion": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wenum-constexpr-conversion",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-enum-conversion": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wenum-conversion",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-enum-enum-conversion": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wenum-enum-conversion",
             "severity:MEDIUM"
@@ -2071,14 +2135,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wexit-time-destructors",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-expansion-to-defined": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wexpansion-to-defined",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-experimental-header-units": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wexperimental-header-units",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-explicit-initialize-call": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wexplicit-initialize-call",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-explicit-ownership-type": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wexplicit-ownership-type",
             "severity:MEDIUM"
@@ -2163,14 +2231,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wfor-loop-analysis",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-format": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wformat",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-format-2": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wformat-2",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-format-extra-args": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wformat-extra-args",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-format-insufficient-args": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wformat-insufficient-args",
             "severity:MEDIUM"
@@ -2247,14 +2319,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wfunction-multiversion",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-fuse-ld-path": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wfuse-ld-path",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-future-attribute-extensions": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wfuture-attribute-extensions",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-future-compat": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wfuture-compat",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-gcc-compat": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgcc-compat",
             "severity:MEDIUM"
@@ -2343,22 +2419,42 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-inline-cpp-without-extern",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-gnu-label-as-value": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-label-as-value",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-gnu-line-marker": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-line-marker",
+            "severity:MEDIUM"
+        ],
+        "clang-diagnostic-gnu-null-pointer-arithmetic": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-null-pointer-arithmetic",
+            "severity:MEDIUM"
+        ],
+        "clang-diagnostic-gnu-offsetof-extensions": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-offsetof-extensions",
+            "severity:MEDIUM"
+        ],
+        "clang-diagnostic-gnu-pointer-arith": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-pointer-arith",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-gnu-redeclared-enum": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-redeclared-enum",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-gnu-statement-expression": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-statement-expression",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-gnu-statement-expression-from-macro-expansion": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-statement-expression-from-macro-expansion",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-gnu-static-float-init": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-static-float-init",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-gnu-string-literal-operator-template": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wgnu-string-literal-operator-template",
             "severity:MEDIUM"
@@ -2387,18 +2483,26 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wheader-guard",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-header-hygiene": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wheader-hygiene",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-hip-omp-target-directives": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#whip-omp-target-directives",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-hip-only": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#whip-only",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-hlsl-extensions": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#whlsl-extensions",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-idiomatic-parentheses": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#widiomatic-parentheses",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-ignored-attributes": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wignored-attributes",
             "severity:MEDIUM"
@@ -2515,14 +2619,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wincompatible-exception-spec",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-incompatible-function-pointer-types": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wincompatible-function-pointer-types",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-incompatible-function-pointer-types-strict": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wincompatible-function-pointer-types-strict",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-incompatible-library-redeclaration": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wincompatible-library-redeclaration",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-incompatible-ms-struct": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wincompatible-ms-struct",
             "severity:HIGH"
@@ -2699,14 +2807,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#winvalid-source-encoding",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-invalid-token-paste": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#winvalid-token-paste",
             "severity:HIGH"
         ],
+        "clang-diagnostic-invalid-utf8": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#winvalid-utf8",
+            "severity:HIGH"
+        ],
         "clang-diagnostic-jump-seh-finally": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wjump-seh-finally",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-keyword-compat": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wkeyword-compat",
             "severity:MEDIUM"
@@ -2779,14 +2891,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmalformed-warning-check",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-many-braces-around-scalar-init": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmany-braces-around-scalar-init",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-mathematical-notation-identifier-extension": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmathematical-notation-identifier-extension",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-max-tokens": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmax-tokens",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-max-unsigned-zero": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmax-unsigned-zero",
             "severity:MEDIUM"
@@ -2887,14 +3003,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-inaccessible-base",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-microsoft-include": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-include",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-microsoft-init-from-predefined": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-init-from-predefined",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-microsoft-mutable-reference": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-mutable-reference",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-microsoft-pure-definition": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-pure-definition",
             "severity:MEDIUM"
@@ -2931,14 +3051,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-using-decl",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-microsoft-void-pseudo-dtor": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmicrosoft-void-pseudo-dtor",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-misexpect": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmisexpect",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-misleading-indentation": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmisleading-indentation",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-mismatched-new-delete": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmismatched-new-delete",
             "severity:MEDIUM"
@@ -3039,14 +3163,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#rmodule-import",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-module-import-in-extern-c": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmodule-import-in-extern-c",
             "severity:HIGH"
         ],
+        "clang-diagnostic-module-include-translation": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmodule-include-translation",
+            "severity:HIGH"
+        ],
         "clang-diagnostic-module-lock": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#rmodule-lock",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-modules-ambiguous-internal-linkage": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wmodules-ambiguous-internal-linkage",
             "severity:MEDIUM"
@@ -3475,14 +3603,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#woverriding-t-option",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-packed": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wpacked",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-packed-non-pod": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wpacked-non-pod",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-padded": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wpadded",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-parentheses": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wparentheses",
             "severity:MEDIUM"
@@ -3707,14 +3839,22 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wrange-loop-bind-reference",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-range-loop-construct": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wrange-loop-construct",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-read-modules-implicitly": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wread-modules-implicitly",
+            "severity:MEDIUM"
+        ],
+        "clang-diagnostic-read-only-types": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wread-only-types",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-readonly-iboutlet-property": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreadonly-iboutlet-property",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-receiver-expr": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreceiver-expr",
             "severity:MEDIUM"
@@ -3779,26 +3919,34 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreserved-identifier",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-reserved-macro-identifier": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreserved-macro-identifier",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-reserved-module-identifier": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreserved-module-identifier",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-reserved-user-defined-literal": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreserved-user-defined-literal",
             "severity:HIGH"
         ],
         "clang-diagnostic-restrict-expansion": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wrestrict-expansion",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-retained-language-linkage": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wretained-language-linkage",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-return-local-addr": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreturn-local-addr",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-return-stack-address": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreturn-stack-address",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-return-std-move": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wreturn-std-move",
             "severity:MEDIUM"
@@ -3823,14 +3971,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wrtti",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-sanitize-address": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#rsanitize-address",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-sarif-format-unstable": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsarif-format-unstable",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-search-path-usage": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#rsearch-path-usage",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-section": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsection",
             "severity:MEDIUM"
@@ -3947,14 +4099,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsigned-enum-bitfield",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-signed-unsigned-wchar": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsigned-unsigned-wchar",
             "severity:HIGH"
         ],
+        "clang-diagnostic-single-bit-bitfield-constant-conversion": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsingle-bit-bitfield-constant-conversion",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-sizeof-array-argument": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsizeof-array-argument",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-sizeof-array-decay": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsizeof-array-decay",
             "severity:MEDIUM"
@@ -3975,14 +4131,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wslash-u-filename",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-slh-asm-goto": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wslh-asm-goto",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-sloc-usage": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsloc-usage",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-sometimes-uninitialized": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsometimes-uninitialized",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-source-mgr": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsource-mgr",
             "severity:MEDIUM"
@@ -3991,14 +4151,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsource-uses-openmp",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-spir-compat": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wspir-compat",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-spirv-compat": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wspirv-compat",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-stack-exhausted": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wstack-exhausted",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-stack-protector": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wstack-protector",
             "severity:MEDIUM"
@@ -4147,22 +4311,30 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wswitch-default",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-switch-enum": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wswitch-enum",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-sync-alignment": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsync-alignment",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-sync-fetch-and-nand-semantics-changed": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsync-fetch-and-nand-semantics-changed",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-synth": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wsynth",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-target-clones-mixed-specifiers": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wtarget-clones-mixed-specifiers",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-tautological-bitwise-compare": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wtautological-bitwise-compare",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-tautological-compare": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wtautological-compare",
             "severity:MEDIUM"
@@ -4279,14 +4451,22 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wtypename-missing",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unable-to-open-stats-file": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunable-to-open-stats-file",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unaligned-access": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunaligned-access",
+            "severity:MEDIUM"
+        ],
+        "clang-diagnostic-unaligned-qualifier-implicit-cast": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunaligned-qualifier-implicit-cast",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unavailable-declarations": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunavailable-declarations",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-undeclared-selector": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wundeclared-selector",
             "severity:MEDIUM"
@@ -4379,14 +4559,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunknown-attributes",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unknown-cuda-version": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunknown-cuda-version",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unknown-directives": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunknown-directives",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unknown-escape-sequence": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunknown-escape-sequence",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unknown-pragmas": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunknown-pragmas",
             "severity:MEDIUM"
@@ -4407,14 +4591,18 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunneeded-internal-declaration",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unneeded-member-function": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunneeded-member-function",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unqualified-std-cast-call": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunqualified-std-cast-call",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unreachable-code": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unreachable-code-aggressive": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-aggressive",
             "severity:MEDIUM"
@@ -4423,26 +4611,38 @@
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-break",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unreachable-code-fallthrough": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-fallthrough",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unreachable-code-generic-assoc": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-generic-assoc",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unreachable-code-loop-increment": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-loop-increment",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unreachable-code-return": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunreachable-code-return",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unsafe-buffer-usage": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wclang-diagnostic-unsafe-buffer-usage",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unsequenced": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunsequenced",
             "severity:MEDIUM"
         ],
+        "clang-diagnostic-unsupported-abi": [
+            "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunsupported-abi",
+            "severity:MEDIUM"
+        ],
         "clang-diagnostic-unsupported-abs": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunsupported-abs",
             "severity:MEDIUM"
         ],
         "clang-diagnostic-unsupported-availability-guard": [
             "doc_url:https://clang.llvm.org/docs/DiagnosticsReference.html#wunsupported-availability-guard",
             "severity:MEDIUM"
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/clangsa.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/clangsa.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/cppcheck.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/cppcheck.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998685594111462%*

 * *Differences: {"'labels'": "{'cppcheck-preprocessorErrorDirective': {delete: [0]}}"}*

```diff
@@ -691,15 +691,14 @@
             "profile:default",
             "severity:MEDIUM"
         ],
         "cppcheck-postfixOperator": [
             "severity:LOW"
         ],
         "cppcheck-preprocessorErrorDirective": [
-            "profile:default",
             "severity:HIGH"
         ],
         "cppcheck-publicAllocationError": [
             "profile:default",
             "severity:MEDIUM"
         ],
         "cppcheck-pureVirtualCall": [
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/mdl.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/mdl.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/analyzers/pylint.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/analyzers/pylint.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/labels/descriptions.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/labels/descriptions.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/logger.conf` & `codechecker-6.22.2/build_dist/CodeChecker/config/logger.conf`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/config/server_config.json` & `codechecker-6.22.2/build_dist/CodeChecker/config/server_config.json`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/bazel_compile_commands/bazel_compile_commands.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/bazel_compile_commands/bazel_compile_commands.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/PKG-INFO` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechecker
-Version: 6.22.1
+Version: 6.22.2
 Summary: CodeChecker is an analyzer tooling, defect database and viewer extension
 Home-page: https://github.com/Ericsson/CodeChecker
 Author: CodeChecker Team (Ericsson)
 Author-email: codechecker-tool@googlegroups.com
 License: Apache-2.0 WITH LLVM-exception
 Project-URL: Documentation, http://codechecker.readthedocs.io
 Project-URL: Issue Tracker, http://github.com/Ericsson/CodeChecker/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codechecker Version: 6.22.1 Summary: CodeChecker is
+Metadata-Version: 2.1 Name: codechecker Version: 6.22.2 Summary: CodeChecker is
 an analyzer tooling, defect database and viewer extension Home-page: https://
 github.com/Ericsson/CodeChecker Author: CodeChecker Team (Ericsson) Author-
 email: codechecker-tool@googlegroups.com License: Apache-2.0 WITH LLVM-
 exception Project-URL: Documentation, http://codechecker.readthedocs.io
 Project-URL: Issue Tracker, http://github.com/Ericsson/CodeChecker/issues
 Description:
                                     ******
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker.egg-info/SOURCES.txt` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_base.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_types.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/config_handler.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/flag.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/result_handler_base.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/__init__.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/analyzer.py
-build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/clang_options.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/config_handler.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_autodetection.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_manager.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_triple_arch.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/result_handler.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/statistics.py
 build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/version.py
@@ -354,51 +353,51 @@
 build_dist/CodeChecker/lib/python3/codechecker_web/shared/pgpass.py
 build_dist/CodeChecker/lib/python3/codechecker_web/shared/version.py
 build_dist/CodeChecker/lib/python3/codechecker_web/shared/webserver_context.py
 build_dist/CodeChecker/lib/python3/tu_collector/__init__.py
 build_dist/CodeChecker/lib/python3/tu_collector/tu_collector.py
 build_dist/CodeChecker/www/07c4c8ad1e67dd03142f8a3f10cf0c1d.png
 build_dist/CodeChecker/www/198.71b517a7d103c8182680.js
-build_dist/CodeChecker/www/204.48d4cf3235458f4f48b8.js
 build_dist/CodeChecker/www/257.2fb64e335d3132937e67.js
 build_dist/CodeChecker/www/287.0bc0c02a80fc6fec452e.js
 build_dist/CodeChecker/www/291.5a3df2fbabd931cce421.js
 build_dist/CodeChecker/www/2d39422cd3aa08e2c9d27844e52cf651.png
+build_dist/CodeChecker/www/324.780b5ed89944be295f22.js
 build_dist/CodeChecker/www/3408d5e44bc83a8a65abfaab3db59b34.png
 build_dist/CodeChecker/www/343.e2548aa08e829c446317.js
 build_dist/CodeChecker/www/437c4ff8b03d221ca7112e93dd271271.png
-build_dist/CodeChecker/www/452.49b8e5bc5792d6509d2d.js
-build_dist/CodeChecker/www/455.0a5796cf6fe665353148.js
+build_dist/CodeChecker/www/455.f9ee007c1bcfd28541ae.js
 build_dist/CodeChecker/www/5857a166c7017a15b8caedeed9b85c88.png
 build_dist/CodeChecker/www/608.57f5c652f7cf87d221c0.js
 build_dist/CodeChecker/www/60b2da9aea5224169d569c59129b6aea.png
 build_dist/CodeChecker/www/680.fd2ce6a69f228ec1a2d0.js
 build_dist/CodeChecker/www/72d28790afb57a543ab3215b7fcff696.png
 build_dist/CodeChecker/www/771.a2b39dd451456852d62a.js
 build_dist/CodeChecker/www/77db62d20f442ca57ed2fba2bb8bdf0d.png
 build_dist/CodeChecker/www/808.1a0aee7cc43bc809830d.js
 build_dist/CodeChecker/www/820.ef2aa58b90057d1d858f.js
 build_dist/CodeChecker/www/83e0246ba1dc6bed1c4c6ef2bb708e6d.png
 build_dist/CodeChecker/www/840.3f6ddcfae65b29844150.js
 build_dist/CodeChecker/www/8b0b574430b7d19d0afcaf576a964c21.png
 build_dist/CodeChecker/www/91.f30e841add2c06736bcc.js
+build_dist/CodeChecker/www/950.87a139d7b44cf5913f38.js
 build_dist/CodeChecker/www/960.69e3e9a01225afeb6d5a.js
 build_dist/CodeChecker/www/bc9b37bfe8ed72f234a5972c2c45239c.png
 build_dist/CodeChecker/www/browsersupport.js
 build_dist/CodeChecker/www/d7ffbebc7a4edf70373bbc18d3ca66cf.png
 build_dist/CodeChecker/www/e528e8e6e67ca7bdcbb707be99615dba.png
 build_dist/CodeChecker/www/efdadec91f4d830906939a930fc180aa.png
 build_dist/CodeChecker/www/favicon.ico
 build_dist/CodeChecker/www/index.html
-build_dist/CodeChecker/www/main.176c47b086909cc3937b.js
+build_dist/CodeChecker/www/main.42489517cdf5af8e5e0e.js
 build_dist/CodeChecker/www/materialdesignicons-webfont.5d42b4e.ttf
 build_dist/CodeChecker/www/materialdesignicons-webfont.5dff34d.woff
 build_dist/CodeChecker/www/materialdesignicons-webfont.606b164.woff2
 build_dist/CodeChecker/www/materialdesignicons-webfont.e044ed2.eot
-build_dist/CodeChecker/www/runtime.78a99b5041c202c0a7ed.js
+build_dist/CodeChecker/www/runtime.e1b8e20cfbd50bdd0fef.js
 build_dist/CodeChecker/www/static.js
 build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js
 build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js.LICENSE.txt
 build_dist/CodeChecker/www/images/new_features/6.10.0/bug_path_length_filter.png
 build_dist/CodeChecker/www/images/new_features/6.17.0/git_blame.png
 build_dist/CodeChecker/www/images/new_features/6.7.0/component_filter.png
 build_dist/CodeChecker/www/images/new_features/6.7.0/plist_to_html_index.png
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analysis_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analysis_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,27 +725,32 @@
     For every build action there is worker which makes the analysis.
     """
 
     # Handle SIGINT to stop this script running.
     def signal_handler(signum, frame):
         try:
             pool.terminate()
+            pool.join()
             manager.shutdown()
+        except Exception as e:
+            LOG.error("Failed to clean up after the pool!:\n")
+            LOG.error(e)
+            raise
         finally:
             sys.exit(128 + signum)
 
-    signal.signal(signal.SIGINT, signal_handler)
     actions, skipped_actions = skip_cpp(actions, skip_handlers)
     # Start checking parallel.
     checked_var = multiprocessing.Value('i', 1)
     actions_num = multiprocessing.Value('i', len(actions))
     pool = multiprocessing.Pool(jobs,
                                 initializer=init_worker,
                                 initargs=(checked_var,
                                           actions_num))
+    signal.signal(signal.SIGINT, signal_handler)
 
     # If the analysis has failed, we help debugging.
     failed_dir = os.path.join(output_path, "failed")
     if not os.path.exists(failed_dir):
         os.makedirs(failed_dir)
 
     # Analysis was successful processing results.
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,17 @@
             LOG.error("stats-relevance-threshold must be"
                       " greater than 0 and smaller than 1.")
             return None
 
     return statistics_data
 
 
-def __get_ctu_data(config_map, ctu_dir):
+def __get_ctu_data(ctu_dir):
     """ Get CTU data. """
-    ctu_capability = config_map[ClangSA.ANALYZER_NAME].ctu_capability
+    ctu_capability = ClangSA.ctu_capability()
     return {'ctu_dir': ctu_dir,
             'ctu_func_map_cmd': ctu_capability.mapping_tool_path,
             'ctu_func_map_file': ctu_capability.mapping_file_name,
             'ctu_temp_fnmap_folder': 'tmpExternalFnMaps'}
 
 
 def perform_analysis(args, skip_handlers, actions, metadata_tool,
@@ -226,28 +226,29 @@
             state, _ = data
             metadata_info['checkers'].update({
                 check: state == CheckerState.enabled})
             if state == CheckerState.enabled:
                 enabled_checkers[analyzer].append(check)
 
         # TODO: cppcheck may require a different environment than clang.
-        version = config_map[analyzer].get_version(context.analyzer_env)
+        version = analyzer_types.supported_analyzers[analyzer] \
+            .get_version(context.analyzer_env)
         metadata_info['analyzer_statistics']['version'] = version
 
         metadata_tool['analyzers'][analyzer] = metadata_info
 
     LOG.info("Enabled checkers:\n%s", '\n'.join(
         k + ': ' + ', '.join(v) for k, v in enabled_checkers.items()))
 
     if 'makefile' in args and args.makefile:
         statistics_data = __get_statistics_data(args)
 
         ctu_data = None
         if ctu_collect or statistics_data:
-            ctu_data = __get_ctu_data(config_map, ctu_dir)
+            ctu_data = __get_ctu_data(ctu_dir)
 
         makefile_creator = MakeFileCreator(analyzers, args.output_path,
                                            config_map, skip_handlers,
                                            ctu_collect, statistics_data,
                                            ctu_data)
         makefile_creator.create(actions)
         return
@@ -272,15 +273,15 @@
     statistics_data = __get_statistics_data(args)
     if statistics_data:
         statistics_data = manager.dict(statistics_data)
 
     if ctu_collect or statistics_data:
         ctu_data = None
         if ctu_collect or ctu_analyze:
-            ctu_data = manager.dict(__get_ctu_data(config_map, ctu_dir))
+            ctu_data = manager.dict(__get_ctu_data(ctu_dir))
 
         pre_analyze = [a for a in actions
                        if a.analyzer_type == ClangSA.ANALYZER_NAME]
         pre_anal_skip_handlers = None
 
         # Skip list is applied only in pre-analysis
         # if --ctu-collect or --stats-collect  was called explicitly
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer_context.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzer_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 # pylint: disable=no-name-in-module
 from distutils.spawn import find_executable
 
 import os
 import sys
 
+from pathlib import Path
+
 from codechecker_common import logger
 from codechecker_common.checker_labels import CheckerLabels
 from codechecker_common.singleton import Singleton
 from codechecker_common.util import load_json
 
 from . import env
 
@@ -59,20 +61,26 @@
         self._checker_labels = CheckerLabels(labels_dir)
         self.__package_version = None
         self.__package_build_date = None
         self.__package_git_hash = None
         self.__analyzers = {}
         self.__analyzer_env = None
 
+        machine = os.uname().machine
+
         self.logger_lib_dir_path = os.path.join(
-            self._data_files_dir_path, 'ld_logger', 'lib')
+            self._data_files_dir_path, 'ld_logger', 'lib', machine)
 
         if not os.path.exists(self.logger_lib_dir_path):
             self.logger_lib_dir_path = os.path.join(
-                self._lib_dir_path, 'codechecker_analyzer', 'ld_logger', 'lib')
+                self._lib_dir_path,
+                'codechecker_analyzer',
+                'ld_logger',
+                'lib',
+                machine)
 
         self.logger_bin = None
         self.logger_file = None
         self.logger_compilers = None
 
         # Init package specific environment variables.
         self.__init_env()
@@ -227,16 +235,20 @@
         return self.env_vars['cc_logger_file']
 
     @property
     def path_logger_bin(self):
         return os.path.join(self._bin_dir_path, 'ld_logger')
 
     @property
-    def path_logger_lib(self):
-        return self.logger_lib_dir_path
+    def logger_lib_path(self):
+        """
+        Returns the absolute path to the logger library.
+        """
+        return str(Path(self.logger_lib_dir_path,
+                        self.logger_lib_name).absolute())
 
     @property
     def logger_lib_name(self):
         return 'ldlogger.so'
 
     @property
     def path_plist_to_html_dist(self):
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_base.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         except Exception as ex:
             LOG.error(ex)
             res_handler.analyzer_returncode = 1
             return res_handler
 
     @classmethod
-    def get_analyzer_checkers(cls, cfg_handler):
+    def get_analyzer_checkers(cls):
         """
         Return the checkers available in the analyzer.
         """
         raise NotImplementedError("Subclasses should implement this!")
 
     def post_analyze(self, result_handler):
         """
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_types.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/analyzer_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,40 +34,34 @@
 
 def is_ctu_capable():
     """ Detects if the current clang is CTU compatible. """
     enabled_analyzers, _ = check_supported_analyzers([ClangSA.ANALYZER_NAME])
     if not enabled_analyzers:
         return False
 
-    clangsa_cfg = ClangSA.construct_config_handler([])
-
-    return clangsa_cfg.ctu_capability.is_ctu_capable
+    return ClangSA.ctu_capability().is_ctu_capable
 
 
 def is_ctu_on_demand_available():
     """ Detects if the current clang is capable of on-demand AST loading. """
     enabled_analyzers, _ = check_supported_analyzers([ClangSA.ANALYZER_NAME])
     if not enabled_analyzers:
         return False
 
-    clangsa_cfg = ClangSA.construct_config_handler([])
-
-    return clangsa_cfg.ctu_capability.is_on_demand_ctu_available
+    return ClangSA.ctu_capability().is_on_demand_ctu_available
 
 
 def is_statistics_capable():
     """ Detects if the current clang is Statistics compatible. """
     # Resolve potentially missing binaries.
     enabled_analyzers, _ = check_supported_analyzers([ClangSA.ANALYZER_NAME])
     if not enabled_analyzers:
         return False
 
-    clangsa_cfg = ClangSA.construct_config_handler([])
-
-    checkers = ClangSA.get_analyzer_checkers(clangsa_cfg, True, True)
+    checkers = ClangSA.get_analyzer_checkers(alpha=True, debug=True)
 
     stat_checkers_pattern = re.compile(r'.+statisticscollector.+')
 
     for checker_name, _ in checkers:
         if stat_checkers_pattern.match(checker_name):
             return True
 
@@ -76,36 +70,31 @@
 
 def is_z3_capable():
     """ Detects if the current clang is Z3 compatible. """
     enabled_analyzers, _ = check_supported_analyzers([ClangSA.ANALYZER_NAME])
     if not enabled_analyzers:
         return False
 
-    analyzer_binary = analyzer_context.get_context() \
-        .analyzer_binaries.get(ClangSA.ANALYZER_NAME)
-
-    return host_check.has_analyzer_option(analyzer_binary,
+    return host_check.has_analyzer_option(ClangSA.analyzer_binary(),
                                           ['-Xclang',
                                            '-analyzer-constraints=z3'])
 
 
 def is_z3_refutation_capable():
     """ Detects if the current clang is Z3 refutation compatible. """
 
     # This function basically checks whether the corresponding analyzer config
     # option exists i.e. it is visible on analyzer config option help page.
     # However, it doesn't mean that Clang itself is compiled with Z3.
     if not is_z3_capable():
         return False
 
     check_supported_analyzers([ClangSA.ANALYZER_NAME])
-    analyzer_binary = analyzer_context.get_context() \
-        .analyzer_binaries.get(ClangSA.ANALYZER_NAME)
 
-    return host_check.has_analyzer_config_option(analyzer_binary,
+    return host_check.has_analyzer_config_option(ClangSA.analyzer_binary(),
                                                  'crosscheck-with-z3')
 
 
 def is_ignore_conflict_supported():
     """
     Detects if clang-apply-replacements supports --ignore-insert-conflict flag.
     """
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/analyzer.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/analyzer.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,502 +2,423 @@
 #
 #  Part of the CodeChecker project, under the Apache License v2.0 with
 #  LLVM Exceptions. See LICENSE for license information.
 #  SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 #
 # -------------------------------------------------------------------------
 """
-Clang Static Analyzer related functions.
+Cppcheck related functions.
 """
 
+from collections import defaultdict
+# TODO distutils will be removed in python3.12
+from distutils.version import StrictVersion
+from pathlib import Path
 import os
+import pickle
 import re
-import shlex
+import shutil
 import subprocess
-
-from typing import List
+import xml.etree.ElementTree as ET
 
 from codechecker_common.logger import get_logger
 
-from codechecker_analyzer import analyzer_context, env
+from codechecker_analyzer import analyzer_context
+from codechecker_analyzer.env import get_binary_in_path
 
 from .. import analyzer_base
-from ..config_handler import CheckerState
-from ..flag import has_flag
-from ..flag import prepend_all
-
-from . import clang_options
-from . import config_handler
-from . import ctu_triple_arch
-from . import version
-from .result_handler import ClangSAResultHandler
-
-LOG = get_logger('analyzer')
-
-
-def parse_clang_help_page(
-    command: List[str],
-    start_label: str
-) -> List[str]:
-    """
-    Parse the clang help page starting from a specific label.
-    Returns a list of (flag, description) tuples.
-    """
-    try:
-        help_page = subprocess.check_output(
-            command,
-            stderr=subprocess.STDOUT,
-            env=analyzer_context.get_context().analyzer_env,
-            universal_newlines=True,
-            encoding="utf-8",
-            errors="ignore")
-    except (subprocess.CalledProcessError, OSError):
-        LOG.debug("Failed to run '%s' command!", command)
-        return []
-
-    try:
-        help_page = help_page[help_page.index(start_label) + len(start_label):]
-    except ValueError:
-        return []
 
-    # This regex will match lines which contain only a flag or a flag and a
-    # description: '  <flag>', '  <flag> <description>'.
-    start_new_option_rgx = \
-        re.compile(r"^\s{2}(?P<flag>\S+)(\s(?P<desc>[^\n]+))?$")
-
-    # This regex will match lines which contain description for the previous
-    # flag: '     <description>'
-    prev_help_desc_rgx = \
-        re.compile(r"^\s{3,}(?P<desc>[^\n]+)$")
-
-    res = []
-
-    flag = None
-    desc = []
-    for line in help_page.splitlines():
-        m = start_new_option_rgx.match(line)
-        if m:
-            if flag and desc:
-                res.append((flag, ' '.join(desc)))
-                flag = None
-                desc = []
-
-            flag = m.group("flag")
-        else:
-            m = prev_help_desc_rgx.match(line)
-
-        if m and m.group("desc"):
-            desc.append(m.group("desc").strip())
+from .config_handler import CppcheckConfigHandler
+from .result_handler import CppcheckResultHandler
 
-    if flag and desc:
-        res.append((flag, ' '.join(desc)))
+from ..config_handler import CheckerState
 
-    return res
+LOG = get_logger('analyzer.cppcheck')
 
 
-class ClangSA(analyzer_base.SourceAnalyzer):
+def parse_checkers(cppcheck_output):
     """
-    Constructs clang static analyzer commands.
+    Parse cppcheck checkers list given by '--errorlist' flag. Return a list of
+    (checker_name, description) pairs.
     """
-    ANALYZER_NAME = 'clangsa'
+    checkers = []
 
-    def __init__(self, cfg_handler, buildaction):
-        super(ClangSA, self).__init__(cfg_handler, buildaction)
-        self.__disable_ctu = False
-        self.__checker_configs = []
+    tree = ET.ElementTree(ET.fromstring(cppcheck_output))
+    root = tree.getroot()
+    errors = root.find('errors')
+    for error in errors.findall('error'):
+        name = error.attrib.get('id')
+        if name:
+            name = "cppcheck-" + name
+        msg = str(error.attrib.get('msg') or '')
+        # TODO: Check severity handling in cppcheck
+        # severity = error.attrib.get('severity')
 
-    def is_ctu_available(self):
-        """
-        Check if ctu is available for the analyzer.
-        If the ctu_dir is set in the config, the analyzer is capable to
-        run ctu analysis.
-        """
-        return bool(self.config_handler.ctu_dir)
+        # checkers.append((name, msg, severity))
+        checkers.append((name, msg))
 
-    def is_ctu_enabled(self):
-        """
-        Check if ctu is enabled for the analyzer.
-        """
-        return not self.__disable_ctu
+    return checkers
 
-    def disable_ctu(self):
-        """
-        Disable ctu even if ctu is available.
-        By default it is enabled if available.
-        """
-        self.__disable_ctu = True
 
-    def enable_ctu(self):
-        self.__disable_ctu = False
+def parse_version(cppcheck_output):
+    """
+    Parse cppcheck version output and return the version number.
+    """
+    version_re = re.compile(r'^Cppcheck (?P<version>[\d\.]+)')
+    match = version_re.match(cppcheck_output)
+    if match:
+        return StrictVersion(match.group('version'))
 
-    def add_checker_config(self, checker_cfg):
-        """
-        Add configuration options to specific checkers.
-        checker_cfg should be a list of arguments in case of
-        Clang Static Analyzer like this:
-        ['-Xclang', '-analyzer-config', '-Xclang', 'checker_option=some_value']
-        """
 
-        self.__checker_configs.append(checker_cfg)
+class Cppcheck(analyzer_base.SourceAnalyzer):
+    """
+    Constructs the Cppcheck analyzer commands.
+    """
 
-    @classmethod
-    def get_analyzer_checkers(
-        cls,
-        cfg_handler: config_handler.ClangSAConfigHandler,
-        alpha: bool = True,
-        debug: bool = False
-    ) -> List[str]:
-        """Return the list of the supported checkers."""
-        checker_list_args = clang_options.get_analyzer_checkers_cmd(
-            cfg_handler,
-            alpha=alpha,
-            debug=debug)
-        return parse_clang_help_page(checker_list_args, 'CHECKERS:')
+    ANALYZER_NAME = 'cppcheck'
 
     @classmethod
-    def get_checker_config(
-        cls,
-        cfg_handler: config_handler.ClangSAConfigHandler
-    ) -> List[str]:
-        """Return the list of checker config options."""
-        checker_config_args = clang_options.get_checker_config_cmd(
-            cfg_handler,
-            alpha=True)
-        return parse_clang_help_page(checker_config_args, 'OPTIONS:')
+    def analyzer_binary(cls):
+        return analyzer_context.get_context() \
+            .analyzer_binaries[cls.ANALYZER_NAME]
 
     @classmethod
-    def get_analyzer_config(
-        cls,
-        cfg_handler: config_handler.ClangSAConfigHandler
-    ) -> List[str]:
-        """Return the list of analyzer config options."""
-        analyzer_config_args = clang_options.get_analyzer_config_cmd(
-            cfg_handler)
-        return parse_clang_help_page(analyzer_config_args, 'OPTIONS:')
+    def get_version(cls, env=None):
+        """ Get analyzer version information. """
+        version = [cls.analyzer_binary(), '--version']
+        try:
+            output = subprocess.check_output(version,
+                                             env=env,
+                                             universal_newlines=True,
+                                             encoding="utf-8",
+                                             errors="ignore")
+            return output
+        except (subprocess.CalledProcessError, OSError) as oerr:
+            LOG.warning("Failed to get analyzer version: %s",
+                        ' '.join(version))
+            LOG.warning(oerr)
+
+        return None
+
+    def add_checker_config(self, checker_cfg):
+        LOG.error("Checker configuration for Cppcheck is not implemented yet")
+
+    def get_analyzer_mentioned_files(self, output):
+        """
+        Return a collection of files that were mentioned by the analyzer in
+        its standard outputs, which should be analyzer_stdout or
+        analyzer_stderr from a result handler.
+        """
+        pass
+
+    def parse_analyzer_config(self):
+        """
+        Parses a set of a white listed compiler flags.
+        Cppcheck can only use a subset of the parametes
+        found in compilation commands.
+        These are:
+        * -I: flag for specifing include directories
+        * -D: for build time defines
+        * -U: for undefining names
+        * -std: The languange standard
+        Any other parameter different from the above list will be dropped.
+        """
+        params = []
+        interesting_option = re.compile("-[IUD].*")
+        # the std flag is different. the following are all valid flags:
+        # * --std c99
+        # * -std=c99
+        # * --std=c99
+        # BUT NOT:
+        # * -std c99
+        # * -stdlib=libc++
+        std_regex = re.compile("-(-std$|-?std=.*)")
+        for i, analyzer_option in enumerate(self.buildaction.analyzer_options):
+            if interesting_option.match(analyzer_option):
+                params.extend([analyzer_option])
+                # The above extend() won't properly insert the analyzer_option
+                # in case of the following format -I <path/to/include>.
+                # The below check will add the next item in the
+                # analyzer_options list if the parameter is specified with a
+                # space, as that should be actual path to the include.
+                if interesting_option.match(analyzer_option).span() == (0, 2):
+                    params.extend(
+                        [self.buildaction.analyzer_options[i+1]]
+                    )
+            elif std_regex.match(analyzer_option):
+                standard = ""
+                if "=" in analyzer_option:
+                    standard = analyzer_option.split("=")[-1]
+                # Handle space separated parameter
+                # The else clause is never executed until a log parser
+                # limitation is addressed, as only this "-std=xxx" version
+                # of the paramter is forwareded in the analyzer_option list.
+                else:
+                    standard = self.buildaction.analyzer_options[i+1]
+                standard = standard.lower().replace("gnu", "c")
+                params.extend(["--std=" + standard])
+        return params
 
     def construct_analyzer_cmd(self, result_handler):
         """
-        Called by the analyzer method.
-        Construct the analyzer command.
+        Construct analyzer command for cppcheck.
         """
         try:
-            # Get an output file from the result handler.
-            analyzer_output_file = result_handler.analyzer_result_file
-
-            # Get the checkers list from the config_handler.
-            # Checker order matters.
             config = self.config_handler
 
-            analyzer_cmd = [config.analyzer_binary, '--analyze',
-                            # Do not warn about the unused gcc/g++ arguments.
-                            '-Qunused-arguments']
-
-            for plugin in config.analyzer_plugins:
-                analyzer_cmd.extend(["-Xclang", "-plugin",
-                                     "-Xclang", "checkercfg",
-                                     "-Xclang", "-load",
-                                     "-Xclang", plugin])
-
-            analyzer_mode = 'plist-multi-file'
-            analyzer_cmd.extend(['-Xclang',
-                                 '-analyzer-opt-analyze-headers',
-                                 '-Xclang',
-                                 '-analyzer-output=' + analyzer_mode,
-                                 '-o', analyzer_output_file])
-
-            # Expand macros in plist output on the bug path.
-            analyzer_cmd.extend(['-Xclang',
-                                 '-analyzer-config',
-                                 '-Xclang',
-                                 'expand-macros=true'])
-
-            # Checker configuration arguments needs to be set before
-            # the checkers.
-            if self.__checker_configs:
-                for cfg in self.__checker_configs:
-                    analyzer_cmd.extend(cfg)
-
-            # TODO: This object has a __checker_configs attribute and the
-            # corresponding functions to set it. Either those should be used
-            # for checker configs coming as command line argument, or those
-            # should be eliminated.
-            for cfg in config.checker_config:
-                analyzer_cmd.extend(
-                    ['-Xclang', '-analyzer-config', '-Xclang', cfg])
+            analyzer_cmd = [Cppcheck.analyzer_binary()]
+
+            # TODO implement a more granular commandline checker config
+            # Cppcheck runs with all checkers enabled for the time being
+            # the unneded checkers are passed as suppressed checkers
+            analyzer_cmd.append('--enable=all')
 
-            # Config handler stores which checkers are enabled or disabled.
-            disabled_checkers = []
-            enabled_checkers = []
             for checker_name, value in config.checks().items():
-                state, _ = value
-                if state == CheckerState.enabled:
-                    enabled_checkers.append(checker_name)
-                elif state == CheckerState.disabled:
-                    disabled_checkers.append(checker_name)
-
-            if enabled_checkers:
-                analyzer_cmd.extend(['-Xclang',
-                                     '-analyzer-checker=' +
-                                     ','.join(enabled_checkers)])
-            if disabled_checkers:
-                analyzer_cmd.extend(['-Xclang',
-                                     '-analyzer-disable-checker=' +
-                                     ','.join(disabled_checkers)])
-            # Enable aggressive-binary-operation-simplification option.
-            analyzer_cmd.extend(
-                clang_options.get_abos_options(config.version_info))
-
-            # Enable the z3 solver backend.
-            if config.enable_z3:
-                analyzer_cmd.extend(['-Xclang', '-analyzer-constraints=z3'])
-
-            if config.enable_z3_refutation and not config.enable_z3:
-                analyzer_cmd.extend(['-Xclang',
-                                     '-analyzer-config',
-                                     '-Xclang',
-                                     'crosscheck-with-z3=true'])
+                if value[0] == CheckerState.disabled:
+                    # TODO python3.9 removeprefix method would be nicer
+                    # than startswith and a hardcoded slicing
+                    if checker_name.startswith("cppcheck-"):
+                        checker_name = checker_name[9:]
+                    analyzer_cmd.append('--suppress=' + checker_name)
+
+            # unusedFunction check is for whole program analysis,
+            # which is not compatible with per source file analysis.
+            analyzer_cmd.append('--suppress=unusedFunction')
+
+            # Add extra arguments.
+            analyzer_cmd.extend(config.analyzer_extra_arguments)
+
+            # Pass whitelisted parameters
+            analyzer_cmd.extend(self.parse_analyzer_config())
+
+            # TODO fix this in a follow up patch, because it is failing
+            # the macos pypy test.
+            # analyzer_cmd.extend(["--std=" +
+            #                    self.buildaction.compiler_standard
+            #                    .split("=")[-1].lower().replace("gnu", "c")])
+
+            # By default there is no platform configuration,
+            # but a platform definition xml can be specified.
+            if 'platform' in config.analyzer_config:
+                analyzer_cmd.append(
+                        "--platform=" + config.analyzer_config['platform'][0])
+            else:
+                analyzer_cmd.append("--platform=native")
+
+            if 'inconclusive' in config.analyzer_config:
+                analyzer_cmd.append("--inconclusive")
 
-            if config.ctu_dir and not self.__disable_ctu:
+            if 'addons' in config.analyzer_config:
                 analyzer_cmd.extend(
-                    ['-Xclang', '-analyzer-config', '-Xclang',
-                     'experimental-enable-naive-ctu-analysis=true',
-                     '-Xclang', '-analyzer-config', '-Xclang',
-                     'ctu-dir=' + self.get_ctu_dir()])
-                ctu_display_progress = config.ctu_capability.display_progress
-                if ctu_display_progress:
-                    analyzer_cmd.extend(ctu_display_progress)
-
-                if config.ctu_on_demand:
-                    invocation_list_path = \
-                        os.path.join(self.get_ctu_dir(), 'invocation-list.yml')
-                    analyzer_cmd.extend(
-                        ['-Xclang', '-analyzer-config', '-Xclang',
-                         f'ctu-invocation-list={invocation_list_path}'
-                         ])
-
-            compile_lang = self.buildaction.lang
-            if not has_flag('-x', analyzer_cmd):
-                analyzer_cmd.extend(['-x', compile_lang])
-
-            if not has_flag('--target', analyzer_cmd) and \
-                    self.buildaction.target != "":
-                analyzer_cmd.append(f"--target={self.buildaction.target}")
-
-            if not has_flag('-arch', analyzer_cmd) and \
-                    self.buildaction.arch != "":
-                analyzer_cmd.extend(["-arch", self.buildaction.arch])
-
-            if not has_flag('-std', analyzer_cmd) and \
-                    self.buildaction.compiler_standard != "":
-                analyzer_cmd.append(self.buildaction.compiler_standard)
+                    f"--addon={addon}" for addon
+                    in config.analyzer_config["addons"])
 
-            analyzer_cmd.extend(config.analyzer_extra_arguments)
+            if 'libraries' in config.analyzer_config:
+                analyzer_cmd.extend(
+                    f"--library={library}" for library
+                    in config.analyzer_config["libraries"])
 
-            analyzer_cmd.extend(self.buildaction.analyzer_options)
+            # TODO Suggest a better place for this
+            # cppcheck wont create the output folders for itself
+            output_dir = Path(result_handler.workspace, "cppcheck",
+                              result_handler.buildaction_hash)
+            output_dir.mkdir(exist_ok=True)
 
-            analyzer_cmd.extend(prepend_all(
-                '-isystem',
-                self.buildaction.compiler_includes))
+            analyzer_cmd.append('--plist-output=' + str(output_dir))
 
             analyzer_cmd.append(self.source_file)
 
             return analyzer_cmd
 
         except Exception as ex:
             LOG.error(ex)
             return []
 
-    def get_ctu_dir(self):
+    @classmethod
+    def get_analyzer_checkers(cls):
         """
-        Returns the path of the ctu directory (containing the triple).
+        Return the list of the supported checkers.
         """
-        config = self.config_handler
-        triple_arch = ctu_triple_arch.get_triple_arch(self.buildaction,
-                                                      self.source_file,
-                                                      config)
-        ctu_dir = os.path.join(config.ctu_dir, triple_arch)
-        return ctu_dir
-
-    def analyzer_mentioned_file_real_path(self, mentioned_path):
-        """
-        PCH-based an On-demand-parsed CTU modes use different paths and file
-        suffixes. PCH-based mode uses ast dump files that are suffixed with
-        '.ast', and they are supposed to be under the
-        '<ctu-dir>/ast/<original-full-path>'. On-demand-parsed mode uses the
-        full paths of the original source files.
-        """
-        pch_suffix = '.ast'
-
-        # We convert the given file path to absolute path because we suppose
-        # that in the clang's output the PCH files in CTU mode are relative
-        # paths.
-        mentioned_path = os.path.join(self.get_ctu_dir(), mentioned_path)
-
-        # Detect the mode based on the path.
-        suffix_index = mentioned_path.rfind(pch_suffix)
-        # If the file does not have the suffix, the mode is On-demand-parsed.
-        # Return the original path.
-        if suffix_index == -1:
-            LOG.debug("Analyzer mentioned path path: '%s', "
-                      "corresponding source file: '%s'",
-                      mentioned_path, mentioned_path)
-            return mentioned_path
-
-        # PCH-based mode stores files with their full path structure recreated
-        # under <ctu-dir>/ast.
-        ctu_ast_dir = os.path.join(self.get_ctu_dir(), 'ast')
-
-        source_path = mentioned_path[len(ctu_ast_dir):suffix_index]
-
-        LOG.debug("Analyzer mentioned path path: '%s', "
-                  "corresponding source file: '%s'",
-                  mentioned_path, source_path)
-
-        if not mentioned_path.startswith(ctu_ast_dir):
-            LOG.error(
-                "Mentioned path '%s' ends with suffix '%s', but does "
-                "not begin with supposed ast dir '%s'.", mentioned_path,
-                pch_suffix, ctu_ast_dir)
+        command = [cls.analyzer_binary(), "--errorlist"]
 
-        # Strip the prefix ast directory and the suffix.
-        return mentioned_path[len(ctu_ast_dir):suffix_index]
+        try:
+            result = subprocess.check_output(command)
+            return parse_checkers(result)
+        except (subprocess.CalledProcessError) as e:
+            LOG.error(e.stderr)
+        except (OSError) as e:
+            LOG.error(e.errno)
+        return []
 
-    def get_analyzer_mentioned_files(self, output):
+    @classmethod
+    def get_analyzer_config(cls):
         """
-        Parse ClangSA's output to generate a list of files that were mentioned
-        in the standard output or standard error.
+        Config options for cppcheck.
         """
-        if not output:
-            return set()
-
-        regex_for_ctu_ast_load = re.compile(
-            r"CTU loaded AST file: (.*)")
+        return [("addons", "A list of cppcheck addon files."),
+                ("libraries", "A list of cppcheck library definiton files."),
+                ("platform", "The platform configuration .xml file."),
+                ("inconclusive", "Enable inconclusive reports.")
+                ]
 
-        paths = set()
+    @classmethod
+    def get_checker_config(cls):
+        """
+        TODO add config options for cppcheck checkers.
+        """
+        return []
 
-        for line in output.splitlines():
-            match = re.match(regex_for_ctu_ast_load, line)
-            if match:
-                path = match.group(1)
-                paths.add(self.analyzer_mentioned_file_real_path(path))
+    def analyze(self, analyzer_cmd, res_handler, proc_callback=None):
+        env = None
 
-        return paths
+        original_env_file = os.environ.get(
+            'CODECHECKER_ORIGINAL_BUILD_ENV')
+        if original_env_file:
+            with open(original_env_file, 'rb') as env_file:
+                env = pickle.load(env_file, encoding='utf-8')
+
+        return super().analyze(analyzer_cmd, res_handler, proc_callback, env)
+
+    def post_analyze(self, result_handler):
+        """
+        Post process the reuslts after the analysis.
+        Will copy the plist files created by cppcheck into the
+        root of the reports folder.
+        Renames the source plist files to *.plist.bak because
+        The report parsing of the Parse command is done recursively.
+
+        """
+        # Cppcheck can generate an id into the output plist file name
+        # we get "the" *.plist file from the unique output folder
+
+        cppcheck_out_folder = Path(result_handler.workspace,
+                                   "cppcheck",
+                                   result_handler.buildaction_hash)
+        cppcheck_outs = cppcheck_out_folder.glob('**/*.plist')
+
+        for cppcheck_out in list(cppcheck_outs):
+            codechecker_out = os.path.join(result_handler.workspace,
+                                           result_handler.analyzer_result_file)
+
+            # plists generated by cppcheck are still "parsable" by our plist
+            # parser. Renaming is needed to circumvent the processing of the
+            # raw files.
+            try:
+                shutil.copy2(cppcheck_out, codechecker_out)
+                Path(cppcheck_out).rename(str(cppcheck_out) + ".bak")
+            except(OSError) as e:
+                LOG.error(e.errno)
 
     @classmethod
-    def resolve_missing_binary(cls, configured_binary, environ):
+    def resolve_missing_binary(cls, configured_binary, env):
         """
         In case of the configured binary for the analyzer is not found in the
         PATH, this method is used to find a callable binary.
         """
 
-        LOG.debug("%s not found in path for ClangSA!", configured_binary)
+        LOG.debug("%s not found in path for Cppcheck!", configured_binary)
 
         if os.path.isabs(configured_binary):
             # Do not autoresolve if the path is an absolute path as there
             # is nothing we could auto-resolve that way.
             return False
 
-        # clang, clang-5.0, clang++, clang++-5.1, ...
-        clang = env.get_binary_in_path(['clang', 'clang++'],
-                                       r'^clang(\+\+)?(-\d+(\.\d+){0,2})?$',
-                                       environ)
-
-        if clang:
-            LOG.debug("Using '%s' for ClangSA!", clang)
-        return clang
+        cppcheck = get_binary_in_path(['cppcheck'],
+                                      r'^cppcheck(-\d+(\.\d+){0,2})?$',
+                                      env)
+
+        if cppcheck:
+            LOG.debug("Using '%s' for Cppcheck!", cppcheck)
+        return cppcheck
+
+    @classmethod
+    def __get_analyzer_version(cls, analyzer_binary, env):
+        """
+        Return the analyzer version.
+        """
+        command = [analyzer_binary, "--version"]
+
+        try:
+            result = subprocess.check_output(
+                    command,
+                    env=env,
+                    encoding="utf-8",
+                    errors="ignore")
+            return parse_version(result)
+        except (subprocess.CalledProcessError, OSError):
+            return []
 
     @classmethod
     def version_compatible(cls, configured_binary, environ):
         """
         Check the version compatibility of the given analyzer binary.
         """
-        return True
+        analyzer_version = \
+            cls.__get_analyzer_version(configured_binary, environ)
+
+        # The analyzer version should be above 1.80 because '--plist-output'
+        # argument was introduced in this release.
+        if analyzer_version >= StrictVersion("1.80"):
+            return True
+
+        return False
 
     def construct_result_handler(self, buildaction, report_output,
                                  skiplist_handler):
         """
         See base class for docs.
         """
-        res_handler = ClangSAResultHandler(buildaction, report_output,
-                                           self.config_handler.report_hash)
+        res_handler = CppcheckResultHandler(buildaction, report_output,
+                                            self.config_handler.report_hash)
 
         res_handler.skiplist_handler = skiplist_handler
 
         return res_handler
 
     @classmethod
     def construct_config_handler(cls, args):
-
         context = analyzer_context.get_context()
-        environ = context.analyzer_env
+        handler = CppcheckConfigHandler()
 
-        handler = config_handler.ClangSAConfigHandler(environ)
-        handler.analyzer_plugins_dir = context.checker_plugin
-        handler.analyzer_binary = context.analyzer_binaries.get(
-            cls.ANALYZER_NAME)
-        handler.version_info = version.get(handler.analyzer_binary)
-
-        handler.report_hash = args.report_hash \
-            if 'report_hash' in args else None
-
-        handler.enable_z3 = 'enable_z3' in args and args.enable_z3 == 'on'
-
-        handler.enable_z3_refutation = 'enable_z3_refutation' in args and \
-            args.enable_z3_refutation == 'on'
-
-        if 'ctu_phases' in args:
-            handler.ctu_dir = os.path.join(args.output_path,
-                                           args.ctu_dir)
-            handler.ctu_on_demand = \
-                'ctu_ast_mode' in args and \
-                args.ctu_ast_mode == 'parse-on-demand'
+        analyzer_config = defaultdict(list)
 
-        try:
-            with open(args.clangsa_args_cfg_file, 'r', encoding='utf8',
-                      errors='ignore') as sa_cfg:
-                handler.analyzer_extra_arguments = \
-                    re.sub(r'\$\((.*?)\)',
-                           env.replace_env_var(args.clangsa_args_cfg_file),
-                           sa_cfg.read().strip())
-                handler.analyzer_extra_arguments = \
-                    shlex.split(handler.analyzer_extra_arguments)
-        except IOError as ioerr:
-            LOG.debug_analyzer(ioerr)
-        except AttributeError as aerr:
-            # No clangsa arguments file was given in the command line.
-            LOG.debug_analyzer(aerr)
+        if 'analyzer_config' in args and \
+                isinstance(args.analyzer_config, list):
+            for cfg in args.analyzer_config:
+                if cfg.analyzer == cls.ANALYZER_NAME:
+                    analyzer_config[cfg.option].append(cfg.value)
+
+        handler.analyzer_config = analyzer_config
 
-        checkers = ClangSA.get_analyzer_checkers(handler)
+        check_env = context.analyzer_env
+
+        # Overwrite PATH to contain only the parent of the cppcheck binary.
+        if os.path.isabs(Cppcheck.analyzer_binary()):
+            check_env['PATH'] = os.path.dirname(Cppcheck.analyzer_binary())
+
+        checkers = cls.get_analyzer_checkers()
+
+        # Cppcheck can and will report with checks that have a different
+        # name than marked in the --errorlist xml. To be able to suppress
+        # these reports, the checkerlist needs to be extended by those found
+        # in the label file.
+        checker_labels = context.checker_labels
+        checkers_from_label = checker_labels.checkers("cppcheck")
+        parsed_set = set([data[0] for data in checkers])
+        for checker in set(checkers_from_label):
+            if checker not in parsed_set:
+                checkers.append((checker, ""))
 
         try:
             cmdline_checkers = args.ordered_checkers
         except AttributeError:
             LOG.debug_analyzer('No checkers were defined in '
-                               'the command line for %s', cls.ANALYZER_NAME)
+                               'the command line for %s',
+                               cls.ANALYZER_NAME)
             cmdline_checkers = []
 
         handler.initialize_checkers(
             checkers,
             cmdline_checkers,
             'enable_all' in args and args.enable_all)
 
-        handler.checker_config = []
-
-        # TODO: This extra "isinstance" check is needed for
-        # CodeChecker checkers --checker-config. This command also runs
-        # this function in order to construct a config handler.
-        if 'checker_config' in args and isinstance(args.checker_config, list):
-            for cfg in args.checker_config:
-                if cfg.analyzer == cls.ANALYZER_NAME:
-                    handler.checker_config.append(
-                        f"{cfg.checker}:{cfg.option}={cfg.value}")
-
-        # TODO: This extra "isinstance" check is needed for
-        # CodeChecker analyzers --analyzer-config. This command also runs
-        # this function in order to construct a config handler.
-        if 'analyzer_config' in args and \
-                isinstance(args.analyzer_config, list):
-            for cfg in args.analyzer_config:
-                if cfg.analyzer == cls.ANALYZER_NAME:
-                    handler.checker_config.append(f"{cfg.option}={cfg.value}")
-
         return handler
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/clang_options.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,158 @@
 # -------------------------------------------------------------------------
 #
 #  Part of the CodeChecker project, under the Apache License v2.0 with
 #  LLVM Exceptions. See LICENSE for license information.
 #  SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 #
 # -------------------------------------------------------------------------
-"""Clang Static analyzer version dependent arguments."""
-
 
+import logging
 import os
+import re
 
-from codechecker_common.logger import get_logger
-
-LOG = get_logger('analyzer')
-
-
-def get_analyzer_checkers_cmd(cfg_handler, alpha=True, debug=False):
-    """Return the checkers list getter command which depends on the used clang
-    version.
-
-    plugins -- A list of paths to clang plugins (so with checkers).
+from typing import Iterator, List, Optional, Tuple
 
-    Before clang9 alpha and debug checkers were printed by default.
-    Since clang9 there are extra arguments to print the additional checkers.
-    """
-    command = [cfg_handler.analyzer_binary, "-cc1"]
-
-    for plugin in cfg_handler.analyzer_plugins:
-        command.extend(["-load", plugin])
-
-    command.append("-analyzer-checker-help")
+from codechecker_report_converter.report import BugPathEvent, File, \
+    get_or_create_file, Report
 
-    # The clang compiler on OSX is a few
-    # relases older than the open source clang release.
-    # The new checker help printig flags are not available there yet.
-    # If the OSX clang will be updated to based on clang v8
-    # this early return can be removed.
-    version_info = cfg_handler.version_info
-    if not version_info or version_info.vendor != "clang":
-        return command
+from ..parser import get_next, BaseParser
 
-    if alpha and version_info.major_version > 8:
-        command.append("-analyzer-checker-help-alpha")
+LOG = logging.getLogger('report-converter')
 
-    if debug and version_info.major_version > 8:
-        command.append("-analyzer-checker-help-developer")
 
-    return command
+class SANParser(BaseParser):
+    """ Parser for Clang UndefinedBehaviourSanitizer console outputs.
 
-
-def get_checker_config_cmd(cfg_handler, alpha=True, debug=True):
-    """Return the checker config getter command which depends on the used clang
-    version.
+    Example output
+        /a/b/main.cpp:13:10: runtime error: load of value 7...
     """
-    command = [cfg_handler.analyzer_binary, "-cc1"]
-
-    for plugin in cfg_handler.analyzer_plugins:
-        command.extend(["-load", plugin])
-
-    command.append("-analyzer-checker-option-help")
-
-    if cfg_handler.version_info.vendor != "clang":
-        return command
-
-    if alpha and cfg_handler.version_info.major_version > 8:
-        command.append("-analyzer-checker-option-help-alpha")
-
-    if debug and cfg_handler.version_info.major_version > 8:
-        command.append("-analyzer-checker-option-help-developer")
-
-    return command
-
-
-def get_analyzer_config_cmd(cfg_handler):
-    """Return the analyzer config getter command which depends on the used
-    clang version.
-    """
-    command = [cfg_handler.analyzer_binary, "-cc1"]
-
-    for plugin in cfg_handler.analyzer_plugins:
-        command.extend(["-load", plugin])
 
-    command.append("-analyzer-config-help")
+    checker_name: str = ""
+    main_event_index = -1
+    line_re = re.compile(r'')
+
+    def __init__(self):
+        super(SANParser, self).__init__()
+
+        # Regex for parsing stack trace line.
+        # It has the following format:
+        #     #1 0x42a51d in main /dummy/main.cpp:24:2
+        self.stack_trace_re = re.compile(r'^\s+#\d+')
+
+        self.file_re = re.compile(
+            r'(?P<path>[\S]+?):(?P<line>\d+)(:(?P<column>\d+))?')
+
+    def parse_sanitizer_message(
+        self,
+        it: Iterator[str],
+        line: str
+    ) -> Tuple[Optional[Report], str]:
+        """ Parses ThreadSanitizer output message. """
+        match = self.line_re.match(line)
+        if not match:
+            return None, line
+
+        if getattr(self, 'skip_line_after_match', True):
+            line = get_next(it)
+        stack_traces, events, line = self.parse_stack_trace(it, line)
+
+        if not events:
+            return None, line
+
+        main_event = events[self.main_event_index]
+
+        report = self.create_report(
+            events, main_event.file, main_event.line, main_event.column,
+            match.group('message').strip(), stack_traces)
+
+        return report, line
+
+    def _parse_line(
+        self,
+        it: Iterator[str],
+        line: str
+    ) -> Tuple[List[Report], str]:
+        """ Parse the given line. """
+        report, next_line = self.parse_sanitizer_message(it, line)
+        if report:
+            return [report], next_line
+
+        return [], next(it)
+
+    def parse_stack_trace_line(self, line: str) -> Optional[BugPathEvent]:
+        """ Parse the given stack trace line.
+
+        Return an event if the file in the stack trace line exists otherwise
+        it returns None.
+        """
+        file_match = self.file_re.search(line)
+        if not file_match:
+            return None
+
+        file_path = file_match.group('path')
+        if file_path and os.path.exists(file_path):
+            col = file_match.group('column')
+            return BugPathEvent(
+                line.rstrip(),
+                get_or_create_file(
+                    os.path.abspath(file_path), self._file_cache),
+                int(file_match.group('line')),
+                int(col) if col else 0)
+
+        return None
+
+    def create_report(
+        self,
+        events: List[BugPathEvent],
+        file: File,
+        line: int,
+        column: int,
+        message: str,
+        stack_traces: List[str],
+        checker_name: Optional[str] = None
+    ) -> Report:
+        """
+        Create a report for the sanitizer output with the given data.
+        checker_name: if None then the sanitizer name will be applied.
+        """
+        # The original message should be the last part of the path. This is
+        # displayed by quick check, and this is the main event displayed by
+        # the web interface.
+        events.append(BugPathEvent(message, file, line, column))
+
+        notes = None
+        if stack_traces:
+            notes = [BugPathEvent(''.join(stack_traces), file, line, column)]
+
+        # Dynamic analyzers usually generate checker messages containing
+        # memory addresses. Since checker messages are included in the report
+        # hash, the subsequent executions of the analysis produces different
+        # reports even if they refer the same problem. For this reason the
+        # memory addresses are cut out from "static_message" for sake of
+        # stabile hash generation.
+        return Report(
+            file, line, column, message, checker_name or self.checker_name,
+            bug_path_events=events,
+            notes=notes,
+            static_message=re.sub(r'0x[0-9a-fA-F]+', '', message))
+
+    def parse_stack_trace(
+        self,
+        it: Iterator[str],
+        line: str
+    ) -> Tuple[List[str], List[BugPathEvent], str]:
+        """ Iterate over lines and parse stack traces. """
+        events: List[BugPathEvent] = []
+        stack_traces: List[str] = []
+
+        while line.strip():
+            event = self.parse_stack_trace_line(line)
+            if event:
+                events.append(event)
 
-    return command
+            stack_traces.append(line)
+            line = get_next(it)
 
+        events.reverse()
 
-def ctu_mapping(clang_version_info):
-    """Clang version dependent ctu mapping tool path and mapping file name.
-
-    The path of the mapping tool, which is assumed to be located
-    inside the installed directory of the analyzer. Certain binary
-    distributions can postfix the tool name with the major version
-    number, the number and the tool name being separated by a dash. By
-    default the shorter name is looked up, then if it is not found the
-    postfixed.
-    """
-    if not clang_version_info:
-        LOG.debug("No clang version information."
-                  "Can not detect ctu mapping tool.")
-        return None, None
-
-    old_mapping_tool_name = 'clang-func-mapping'
-    old_mapping_file_name = 'externalFnMap.txt'
-
-    new_mapping_tool_name = 'clang-extdef-mapping'
-    new_mapping_file_name = 'externalDefMap.txt'
-
-    major_version = clang_version_info.major_version
-
-    if major_version > 7:
-        tool_name = new_mapping_tool_name
-        mapping_file = new_mapping_file_name
-    else:
-        tool_name = old_mapping_tool_name
-        mapping_file = old_mapping_file_name
-
-    installed_dir = clang_version_info.installed_dir
-
-    tool_path = os.path.join(installed_dir, tool_name)
-
-    if os.path.isfile(tool_path):
-        return tool_path, mapping_file
-
-    LOG.debug(
-        "Mapping tool '%s' suggested by autodetection is not found in "
-        "directory reported by Clang '%s'. Trying with version-postfixed "
-        "filename...", tool_path, installed_dir)
-
-    postfixed_tool_path = ''.join([tool_path, '-', str(major_version)])
-
-    if os.path.isfile(postfixed_tool_path):
-        return postfixed_tool_path, mapping_file
-
-    LOG.debug(
-        "Postfixed mapping tool '%s' suggested by autodetection is not "
-        "found in directory reported by Clang '%s'.",
-        postfixed_tool_path, installed_dir)
-    return None, None
-
-
-def get_abos_options(clang_version_info):
-    """ Get options to enable aggressive-binary-operation-simplification.
-
-    Returns list of options which enables
-    aggressive-binary-operation-simplification option (which is needed for the
-    iterator checker) if the Clang version is greater then 8.
-    Otherwise returns an empty list.
-    """
-    if clang_version_info and clang_version_info.major_version >= 8:
-        return ['-Xclang',
-                '-analyzer-config',
-                '-Xclang',
-                'aggressive-binary-operation-simplification=true']
-
-    return []
+        return stack_traces, events, line
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_manager.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_triple_arch.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/ctu_triple_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 #
 # -------------------------------------------------------------------------
 """
 Helpers for determining triple arch of a compile action
 """
 
 
+from . import analyzer
 from .. import analyzer_base
 from ..flag import has_flag
 from ..flag import prepend_all
 
 
 def get_compile_command(action, config, source='', output=''):
     """ Generate a standardized and cleaned compile command serving as a base
     for other operations. """
 
-    cmd = [config.analyzer_binary]
+    cmd = [analyzer.ClangSA.analyzer_binary()]
 
     if not has_flag('--target', cmd) and action.target != "":
         cmd.append(f"--target={action.target}")
 
     cmd.append('-c')
     if not has_flag('-x', cmd):
         cmd.extend(['-x', action.lang])
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/result_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/result_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/statistics.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 
 
 def build_stat_coll_cmd(action, config, source):
     """
     Build the statistics collector analysis command.
     """
 
-    cmd = [config.analyzer_binary, '-c', '-x', action.lang, '--analyze',
+    cmd = [ClangSA.analyzer_binary(), '-c', '-x', action.lang, '--analyze',
            # Do not warn about the unused gcc/g++ arguments.
            '-Qunused-arguments',
            '--analyzer-output', 'text']
 
-    for plugin in config.analyzer_plugins:
+    for plugin in ClangSA.analyzer_plugins():
         cmd.extend(["-Xclang", "-plugin",
                     "-Xclang", "checkercfg",
                     "-Xclang", "-load",
                     "-Xclang", plugin])
 
     cmd.extend(['-Xclang',
                 '-analyzer-opt-analyze-headers'])
 
     cmd.extend(config.analyzer_extra_arguments)
     cmd.extend(action.analyzer_options)
 
     # Enable the statistics collector checkers only.
     collector_checkers = []
-    checks = ClangSA.get_analyzer_checkers(config, True, True)
+    checks = ClangSA.get_analyzer_checkers(alpha=True, debug=True)
     for checker_name, _ in checks:
         if SpecialReturnValueCollector.checker_collect in checker_name:
             collector_checkers.append(checker_name)
 
         if ReturnValueCollector.checker_collect in checker_name:
             collector_checkers.append(checker_name)
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/version.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangsa/version.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/analyzer.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import json
 import os
 import re
 import shlex
 import subprocess
 from typing import List, Tuple
 
+import yaml
+
 from codechecker_common.logger import get_logger
 
 from codechecker_analyzer import analyzer_context, env
 from codechecker_analyzer.analyzers.clangsa.analyzer import ClangSA
 
 from .. import analyzer_base
 from ..config_handler import CheckerState, CheckerType, \
@@ -51,22 +53,56 @@
             continue
         match = pattern.match(line)
         if match:
             checkers.append((match.group(0), ''))
     return checkers
 
 
+def parse_checker_config_old(config_dump):
+    """
+    Return the parsed clang-tidy config options as a list of
+    (flag, default_value) tuples. This variant works
+    for clang-tidy up to version 14.
+
+    config_dump -- clang-tidy config options YAML dump in pre-LLVM15 format.
+    """
+    reg = re.compile(r'key:\s+(\S+)\s+value:\s+([^\n]+)')
+    return re.findall(reg, config_dump)
+
+
+def parse_checker_config_new(config_dump):
+    """
+    Return the parsed clang-tidy config options as a list of
+    (flag, default_value) tuples. This variant works
+    for clang-tidy starting with version 15
+
+    config_dump -- clang-tidy config options YAML dump in post-LLVM15 format.
+    """
+    try:
+        data = yaml.safe_load(config_dump)
+        if 'CheckOptions' not in data:
+            return None
+
+        return [[key, value]
+                for (key, value) in data['CheckOptions'].items()]
+    except ImportError:
+        return None
+
+
 def parse_checker_config(config_dump):
     """
     Return the parsed clang-tidy config options as a list of
     (flag, default_value) tuples.
     config_dump -- clang-tidy config options YAML dump.
     """
-    reg = re.compile(r'key:\s+(\S+)\s+value:\s+([^\n]+)')
-    return re.findall(reg, config_dump)
+    result = parse_checker_config_old(config_dump)
+    if not result:
+        result = parse_checker_config_new(config_dump)
+
+    return result
 
 
 def parse_analyzer_config(config_dump):
     """
     Return the parsed clang-tidy analyzer options as a list of
     (flag, default_value) tuples.
     config_dump -- clang-tidy config options YAML dump.
@@ -132,26 +168,49 @@
 class ClangTidy(analyzer_base.SourceAnalyzer):
     """
     Constructs the clang tidy analyzer commands.
     """
 
     ANALYZER_NAME = 'clang-tidy'
 
+    @classmethod
+    def analyzer_binary(cls):
+        return analyzer_context.get_context() \
+            .analyzer_binaries[cls.ANALYZER_NAME]
+
+    @classmethod
+    def get_version(cls, env=None):
+        """ Get analyzer version information. """
+        version = [cls.analyzer_binary(), '--version']
+        try:
+            output = subprocess.check_output(version,
+                                             env=env,
+                                             universal_newlines=True,
+                                             encoding="utf-8",
+                                             errors="ignore")
+            return output
+        except (subprocess.CalledProcessError, OSError) as oerr:
+            LOG.warning("Failed to get analyzer version: %s",
+                        ' '.join(version))
+            LOG.warning(oerr)
+
+        return None
+
     def add_checker_config(self, checker_cfg):
         LOG.error("Not implemented yet")
 
     @classmethod
-    def get_analyzer_checkers(cls, cfg_handler):
+    def get_analyzer_checkers(cls):
         """
         Return the list of the all of the supported checkers.
         """
         try:
             environ = analyzer_context.get_context().analyzer_env
             result = subprocess.check_output(
-                [cfg_handler.analyzer_binary, "-list-checks", "-checks=*"],
+                [cls.analyzer_binary(), "-list-checks", "-checks=*"],
                 env=environ,
                 universal_newlines=True,
                 encoding="utf-8",
                 errors="ignore")
             checker_description = parse_checkers(result)
 
             checker_description.extend(
@@ -159,37 +218,37 @@
                 for warning in get_warnings(environ))
 
             return checker_description
         except (subprocess.CalledProcessError, OSError):
             return []
 
     @classmethod
-    def get_checker_config(cls, cfg_handler):
+    def get_checker_config(cls):
         """
         Return the checker configuration of the all of the supported checkers.
         """
         try:
             result = subprocess.check_output(
-                [cfg_handler.analyzer_binary, "-dump-config", "-checks=*"],
+                [cls.analyzer_binary(), "-dump-config", "-checks=*"],
                 env=analyzer_context.get_context().analyzer_env,
                 universal_newlines=True,
                 encoding="utf-8",
                 errors="ignore")
             return parse_checker_config(result)
         except (subprocess.CalledProcessError, OSError):
             return []
 
     @classmethod
-    def get_analyzer_config(cls, cfg_handler):
+    def get_analyzer_config(cls):
         """
         Return the analyzer configuration with all checkers enabled.
         """
         try:
             result = subprocess.check_output(
-                [cfg_handler.analyzer_binary, "-dump-config", "-checks=*"],
+                [cls.analyzer_binary(), "-dump-config", "-checks=*"],
                 env=analyzer_context.get_context().analyzer_env,
                 universal_newlines=True,
                 encoding="utf-8",
                 errors="ignore")
             return parse_analyzer_config(result)
         except (subprocess.CalledProcessError, OSError):
             return []
@@ -291,15 +350,15 @@
         return checkers, list(compiler_warnings)
 
     def construct_analyzer_cmd(self, result_handler):
         """ Contruct command which will be executed on analysis. """
         try:
             config = self.config_handler
 
-            analyzer_cmd = [config.analyzer_binary]
+            analyzer_cmd = [ClangTidy.analyzer_binary()]
 
             checks, compiler_warnings = self.get_checker_list(config)
 
             if checks:
                 # The invocation should end in a Popen call with shell=False,
                 # so no globbing should occur even if the checks argument
                 # contains characters that would trigger globbing in the shell.
@@ -423,18 +482,15 @@
             buildaction, report_output, report_hash)
 
         res_handler.skiplist_handler = skiplist_handler
         return res_handler
 
     @classmethod
     def construct_config_handler(cls, args):
-        context = analyzer_context.get_context()
         handler = config_handler.ClangTidyConfigHandler()
-        handler.analyzer_binary = context.analyzer_binaries.get(
-            cls.ANALYZER_NAME)
         handler.report_hash = args.report_hash \
             if 'report_hash' in args else None
 
         # FIXME We cannot get the resource dir from the clang-tidy binary,
         # therefore we get a sibling clang binary which of clang-tidy.
         # TODO Support "clang-tidy -print-resource-dir" .
         try:
@@ -515,15 +571,15 @@
         # 'take-config-from-directory' is a special option which let the user
         # to use the '.clang-tidy' config files. It will disable analyzer and
         # checker configuration options.
         if not handler.checker_config and \
                 analyzer_config.get('take-config-from-directory') != 'true':
             handler.checker_config = json.dumps(analyzer_config)
 
-        checkers = ClangTidy.get_analyzer_checkers(handler)
+        checkers = ClangTidy.get_analyzer_checkers()
 
         try:
             cmdline_checkers = args.ordered_checkers
         except AttributeError:
             LOG.debug_analyzer('No checkers were defined in '
                                'the command line for %s',
                                cls.ANALYZER_NAME)
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/config_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/config_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/result_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/clangtidy/result_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/config_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/config_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 
 
 from abc import ABCMeta
 from enum import Enum
 import collections
 import platform
-import subprocess
 
 from codechecker_analyzer import analyzer_context
 from codechecker_common.logger import get_logger
 
 LOG = get_logger('system')
 
 
@@ -68,50 +67,26 @@
 class AnalyzerConfigHandler(metaclass=ABCMeta):
     """
     Handle the checker configurations and enabled disabled checkers lists.
     """
 
     def __init__(self):
 
-        self.analyzer_binary = None
-        self.analyzer_plugins_dir = None
         self.analyzer_extra_arguments = []
         self.checker_config = ''
         self.analyzer_config = None
         self.report_hash = None
         self.enable_all = None
 
         # The key is the checker name, the value is a tuple.
         # False if disabled (should be by default).
         # True if checker is enabled.
         # (False/True, 'checker_description')
         self.__available_checkers = collections.OrderedDict()
 
-    @property
-    def analyzer_plugins(self):
-        """ Full path of the analyzer plugins. """
-        return []
-
-    def get_version(self, env=None):
-        """ Get analyzer version information. """
-        version = [self.analyzer_binary, '--version']
-        try:
-            output = subprocess.check_output(version,
-                                             env=env,
-                                             universal_newlines=True,
-                                             encoding="utf-8",
-                                             errors="ignore")
-            return output
-        except (subprocess.CalledProcessError, OSError) as oerr:
-            LOG.warning("Failed to get analyzer version: %s",
-                        ' '.join(version))
-            LOG.warning(oerr)
-
-        return None
-
     def add_checker(self, checker_name, description='',
                     state=CheckerState.default):
         """
         Add additional checker. If no state argument is given, the actual usage
         of the checker is handled by the analyzer.
         """
         self.__available_checkers[checker_name] = (state, description)
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/config_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/config_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/result_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/cppcheck/result_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/flag.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/flag.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/result_handler_base.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/analyzers/result_handler_base.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/arg.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/arg.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_action.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_action.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/build_manager.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/host_check.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/host_check.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/log_parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/buildlog/log_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     '-fno-canonical-system-headers',
     '-fno-delete-null-pointer-checks',
     '-fno-defer-pop',
     '-fno-extended-identifiers',
     '-fno-jump-table',
     '-fno-keep-inline-dllexport'
     '-fno-keep-static-consts',
+    '-fno-lifetime-dse',
     '-f(no-)?reorder-functions',
     '-fno-strength-reduce',
     '-fno-toplevel-reorder',
     '-fno-unit-at-a-time',
     '-fno-var-tracking-assignments',
     '-fobjc-link-runtime',
     '-fpartial-inlining',
@@ -155,18 +156,21 @@
     # This is not unknown but we want to preserve asserts to improve the
     # quality of analysis.
     '-DNDEBUG$',
 
     # --- IGNORED --- #
     '-save-temps',
     # Clang gives different warnings than GCC. Thus if these flags are kept,
-    # '-Werror', '-pedantic-errors' the analysis with Clang can fail even
-    # if the compilation passes with GCC.
+    # '-Werror', '-Wno-error', '-pedantic-errors' the analysis with Clang can
+    # fail even if the compilation passes with GCC.
     '-Werror',
+    '-Wno-error',
     '-pedantic-errors',
+    # Profiling flags are different or behave differently in GCC
+    '-fprofile',
     # Remove the option disabling the warnings.
     '-w',
     '-g(.+)?$',
     # Link Time Optimization:
     '-flto',
     # MicroBlaze Options:
     '-mxl',
@@ -1064,18 +1068,19 @@
     # the compiler set in gcc-toolchain. This can cause missing headers during
     # the analysis.
 
     toolchain = \
         gcc_toolchain.toolchain_in_args(details['analyzer_options'])
 
     # Store the compiler built in include paths and defines.
-    # If clang compiler is used for compilation and analysis,
-    # do not collect the implicit include paths.
-    if (not toolchain and not using_same_clang_to_compile_and_analyze) or \
-            (compiler_info_file and os.path.exists(compiler_info_file)):
+    # If clang compiler is used for compilation and analysis, or language is
+    # not recognized, do not collect the implicit include paths.
+    if ((not toolchain and not using_same_clang_to_compile_and_analyze) or
+            (compiler_info_file and os.path.exists(compiler_info_file))) and \
+            details['lang']:
         ImplicitCompilerInfo.set(details, compiler_info_file)
 
     if not keep_gcc_include_fixed:
         details['compiler_includes'] = list(filter(
             __is_not_include_fixed,
             details['compiler_includes']))
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/checkers.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/checkers.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyze.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyze.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzer_version.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzer_version.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzers.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/analyzers.py`

 * *Files 13% similar despite different names*

```diff
@@ -144,17 +144,14 @@
                             "newer.")
         elif args.dump_config == 'cppcheck':
             # TODO: Not supported by CppCheck yet!
             LOG.warning("'--dump-config cppcheck' is not supported.")
 
         return
 
-    analyzer_config_map = analyzer_types.build_config_handlers(
-        args, working_analyzers)
-
     def uglify(text):
         """
         csv and json format output contain this non human readable header
         string: no CamelCase and no space.
         """
         return text.lower().replace(' ', '_')
 
@@ -164,18 +161,17 @@
         else:
             header = ['Option']
 
         if args.output_format in ['csv', 'json']:
             header = list(map(uglify, header))
 
         analyzer = args.analyzer_config
-        config_handler = analyzer_config_map.get(analyzer)
         analyzer_class = analyzer_types.supported_analyzers[analyzer]
 
-        configs = analyzer_class.get_analyzer_config(config_handler)
+        configs = analyzer_class.get_analyzer_config()
         if not configs:
             LOG.error("Failed to get analyzer configuration options for '%s' "
                       "analyzer! Please try to upgrade your analyzer version "
                       "to use this feature.", analyzer)
             sys.exit(1)
 
         rows = [(':'.join((analyzer, c[0])), c[1]) if 'details' in args
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/check.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/check.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/checkers.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/checkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
     checker_info = defaultdict(list)
 
     for analyzer in working_analyzers:
         config_handler = analyzer_config_map.get(analyzer)
         analyzer_class = analyzer_types.supported_analyzers[analyzer]
 
-        checkers = analyzer_class.get_analyzer_checkers(config_handler)
+        checkers = analyzer_class.get_analyzer_checkers()
 
         profile_checkers = []
         if 'profile' in args:
             available_profiles = cl.get_description('profile')
 
             if args.profile not in available_profiles:
                 LOG.error("Checker profile '%s' does not exist!",
@@ -525,32 +525,28 @@
     if args.output_format == 'custom':
         args.output_format = 'rows'
 
     working_analyzers, errored = analyzer_types.check_supported_analyzers(
         args.analyzers)
     analyzer_types.check_available_analyzers(working_analyzers, errored)
 
-    analyzer_config_map = analyzer_types.build_config_handlers(
-        args, working_analyzers)
-
     if 'details' in args:
         header = ['Option', 'Description']
     else:
         header = ['Option']
 
     if args.output_format in ['csv', 'json']:
         header = list(map(__uglify, header))
 
     rows = []
     analyzer_failures = []
     for analyzer in working_analyzers:
-        config_handler = analyzer_config_map.get(analyzer)
         analyzer_class = analyzer_types.supported_analyzers[analyzer]
 
-        configs = analyzer_class.get_checker_config(config_handler)
+        configs = analyzer_class.get_checker_config()
         if not configs:
             # Checker configurations are not supported by cppcheck
             if analyzer != "cppcheck":
                 analyzer_failures.append(analyzer)
                 continue
 
         rows.extend((':'.join((analyzer, c[0])), c[1]) if 'details' in args
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/fixit.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/fixit.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/log.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/log.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/parse.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/cmd/parse.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/compilation_database.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/compilation_database.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/env.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,15 @@
     Only environment variables required for logging are changed.
     """
     context = analyzer_context.get_context()
     new_env = original_env
 
     new_env[context.env_var_cc_logger_bin] = context.path_logger_bin
 
-    new_env['LD_PRELOAD'] = context.logger_lib_name
-
-    try:
-        original_ld_library_path = new_env['LD_LIBRARY_PATH']
-        new_env['LD_LIBRARY_PATH'] = context.path_logger_lib + ':' + \
-            original_ld_library_path
-    except KeyError:
-        new_env['LD_LIBRARY_PATH'] = context.path_logger_lib
+    new_env['LD_PRELOAD'] = context.logger_lib_path
 
     # Set ld logger logfile.
     new_env[context.env_var_cc_logger_file] = logfile
 
     return new_env
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/gcc_toolchain.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/gcc_toolchain.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/host_check.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/host_check.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/makefile.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/makefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 
         self.__makefile = os.path.join(output_path, 'Makefile')
 
         self.__config = None
         self.__func_map_cmd = None
         if ClangSA.ANALYZER_NAME in config_map:
             self.__config = config_map[ClangSA.ANALYZER_NAME]
-
-            ctu_capability = config_map[ClangSA.ANALYZER_NAME].ctu_capability
-            self.__func_map_cmd = ctu_capability.mapping_tool_path
+            self.__func_map_cmd = ClangSA.ctu_capability().mapping_tool_path
 
     def __format_analyzer_type(self, analyzer_type):
         """ Format the given analyzer type. """
         return analyzer_type.replace('-', '')
 
     def __get_target_name(self, action):
         """ Get target name for the given action. """
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/pre_analysis_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/pre_analysis_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,16 @@
             # code. In case of AST-dump based analysis these sources are the
             # generated AST-dumps.
             ctu_manager.map_functions(triple_arch, action, action.source,
                                       clangsa_config, ctu_func_map_cmd,
                                       ctu_temp_fnmap_folder)
 
     except Exception as ex:
-        LOG.debug_analyzer(str(ex))
+        LOG.error("Pre-analysis failed for %s: %s", action.source, str(ex))
         traceback.print_exc(file=sys.stdout)
-        raise
 
     try:
         if statistics_data:
             LOG.debug("running statistics pre analysis")
             collect_statistics(action,
                                action.source,
                                clangsa_config,
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_file_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_file_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_analyzer/suppress_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/codeCheckerAuthentication.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/codeCheckerAuthentication.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/ttypes.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Authentication_v6/ttypes.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/configurationService.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/Configuration_v6/configurationService.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/codeCheckerProductService.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/codeCheckerProductService.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/ttypes.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ProductManagement_v6/ttypes.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/serverInfoService.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/ServerInfo_v6/serverInfoService.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/codeCheckerDBAccess.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/codeCheckerDBAccess.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/ttypes.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api/codeCheckerDBAccess_v6/ttypes.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_api_shared/ttypes.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_api_shared/ttypes.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/blame_info.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/blame_info.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/client.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/cmd.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/store.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd/store.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line_client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/cmd_line_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -175,23 +175,25 @@
             if tag:
                 run_tags.append(tag.id)
 
     return run_ids, run_names, run_tags
 
 
 def get_suppressed_reports(reports: List[Report],
-                           args: List[str]) -> List[str]:
+                           review_st: List[ttypes.ReviewStatus]) -> List[str]:
     """Returns a list of suppressed report hashes."""
     return [report.report_hash for report in reports
-            if not report.check_source_code_comments(args.review_status)]
+            if not report.check_source_code_comments(
+                [ttypes.ReviewStatus._VALUES_TO_NAMES[x]
+                 for x in review_st])]
 
 
 def get_report_dir_results(
     report_dirs: List[str],
-    args: List[str],
+    report_filter: ttypes.ReportFilter,
     checker_labels: CheckerLabels
 ) -> List[Report]:
     """Get reports from the given report directories.
 
     Absolute paths are expected to the given report directories.
     """
     all_reports = []
@@ -202,73 +204,73 @@
             # Get reports.
             reports = report_file.get_reports(file_path, checker_labels)
 
             # Skip duplicated reports.
             reports = reports_helper.skip(reports, processed_path_hashes)
 
             # Skip reports based on filter arguments.
-            reports = [
-                report for report in reports
-                if not skip_report_dir_result(report, args, checker_labels)]
+            reports = [report for report in reports
+                       if not skip_report_dir_result(
+                           report, report_filter, checker_labels)]
 
             all_reports.extend(reports)
 
     return all_reports
 
 
 def skip_report_dir_result(
     report: Report,
-    args: List[str],
+    report_filter: ttypes.ReportFilter,
     checker_labels: CheckerLabels
 ) -> bool:
     """Returns True if the report should be skipped from the results.
 
     Skipping is done based on the given filter set.
     """
-    f_severities, f_checkers, f_file_path, _, _, _ = check_filter_values(args)
 
-    if f_severities:
+    if report_filter.severity:
         severity_name = checker_labels.severity(report.checker_name)
-        if severity_name.lower() not in list(map(str.lower, f_severities)):
+        filter_severities_str = [ttypes.Severity._VALUES_TO_NAMES[x]
+                                 for x in report_filter.severity]
+        if severity_name.lower() not in \
+                list(map(str.lower, filter_severities_str)):
             return True
 
-    if f_checkers:
+    if report_filter.checkerName:
         checker_name = report.checker_name
         if not any([re.match(r'^' + c.replace("*", ".*") + '$',
                              checker_name, re.IGNORECASE)
-                    for c in f_checkers]):
+                    for c in report_filter.checkerName]):
             return True
 
-    if f_file_path:
+    if report_filter.filepath:
         if not any([re.match(r'^' + f.replace("*", ".*") + '$',
                              report.file.path, re.IGNORECASE)
-                    for f in f_file_path]):
+                    for f in report_filter.filepath]):
             return True
 
-    if 'checker_msg' in args:
+    if report_filter.checkerMsg:
         checker_msg = report.message
         if not any([re.match(r'^' + c.replace("*", ".*") + '$',
                              checker_msg, re.IGNORECASE)
-                    for c in args.checker_msg]):
+                    for c in report_filter.checkerMsg]):
             return True
 
     return False
 
 
 def get_diff_base_results(
     client,
-    args,
+    report_filter: ttypes.ReportFilter,
     baseids,
     base_hashes,
     suppressed_hashes,
     get_details: bool = True
 ):
     """Get the run results from the server."""
-    report_filter = ttypes.ReportFilter()
-    add_filter_conditions(client, report_filter, args)
     report_filter.reportHash = base_hashes + suppressed_hashes
 
     sort_mode = [(ttypes.SortMode(
         ttypes.SortType.FILENAME,
         ttypes.Order.ASC))]
 
     limit = constants.MAX_QUERY_SIZE
@@ -383,140 +385,124 @@
         offset += limit
         if len(results) < limit:
             break
 
     return all_results
 
 
-def validate_filter_values(user_values, valid_values, value_type):
+def validate_filter_values(converted_values: List[int], valid_values,
+                           value_type):
     """
     Check if the value provided by the user is a valid value.
     """
-    if not user_values:
+    # Can be None if the user provided no value to this option -- that is
+    # valid.
+    if not converted_values:
         return True
 
-    non_valid_values = [status for status in user_values
-                        if valid_values.get(status.upper(), None) is None]
+    non_valid_values = [status for status in converted_values
+                        if valid_values.get(status, None) is None]
 
     if non_valid_values:
         invalid_values = ','.join([x.lower() for x in non_valid_values])
         LOG.error('Invalid %s value(s): %s', value_type, invalid_values)
 
         valid_values = ','.join([x.lower() for x in valid_values.keys()])
         LOG.error('Valid values are: %s', valid_values)
 
         return False
 
     return True
 
 
-def check_filter_values(args):
+def parse_report_filter(client, args):
+    """
+    Parse and check attributes of the given report filter based on
+    the arguments which is provided in the command line.
+    Also, check if filter values are valid values.
+    """
+    report_filter = parse_report_filter_offline(args)
+
+    if 'tag' in args:
+        run_history_filter = ttypes.RunHistoryFilter(tagNames=args.tag)
+        run_histories = client.getRunHistory(None, None, None,
+                                             run_history_filter)
+        if run_histories:
+            report_filter.runTag = [t.id for t in run_histories]
+
+    return report_filter
+
+
+def parse_report_filter_offline(args):
     """
-    Check if filter values are valid values. Returns values which are checked
-    or exit from the interpreter.
+    Same as parse_report_filter, but will not make calls to the server.
+    As of writing this comment, this means that the 'tag' argument will be
+    ignored (as that would require a getRunHistory API call).
     """
-    severities = checkers = file_path = dt_statuses = rw_statuses = None
-    bug_path_length = None
+    report_filter = ttypes.ReportFilter()
 
     if 'severity' in args:
-        severities = args.severity
+        report_filter.severity = [
+            ttypes.Severity._NAMES_TO_VALUES[x.upper()] for x in args.severity]
 
     if 'detection_status' in args:
-        dt_statuses = args.detection_status
+        report_filter.detectionStatus = [
+            ttypes.DetectionStatus._NAMES_TO_VALUES[x.upper()] for x in
+            args.detection_status]
 
     if 'review_status' in args:
-        rw_statuses = args.review_status
+        report_filter.reviewStatus = [
+            ttypes.ReviewStatus._NAMES_TO_VALUES[x.upper()] for x in
+            args.review_status]
 
     if 'checker_name' in args:
-        checkers = args.checker_name
+        report_filter.checkerName = args.checker_name
 
     if 'file_path' in args:
-        file_path = args.file_path
+        report_filter.filepath = args.file_path
 
     if 'bug_path_length' in args:
         path_lengths = args.bug_path_length.split(':')
 
         min_bug_path_length = int(path_lengths[0]) if \
             path_lengths and path_lengths[0].isdigit() else None
 
         max_bug_path_length = int(path_lengths[1]) if \
             len(path_lengths) > 1 and path_lengths[1].isdigit() else None
 
-        bug_path_length = BugPathLengthRange(min=min_bug_path_length,
-                                             max=max_bug_path_length)
+        report_filter.bugPathLength = \
+            BugPathLengthRange(min=min_bug_path_length,
+                               max=max_bug_path_length)
 
     values_to_check = [
-        (severities, ttypes.Severity._NAMES_TO_VALUES, 'severity'),
-        (dt_statuses, ttypes.DetectionStatus._NAMES_TO_VALUES,
+        (report_filter.severity, ttypes.Severity._VALUES_TO_NAMES, 'severity'),
+        (report_filter.detectionStatus,
+         ttypes.DetectionStatus._VALUES_TO_NAMES,
          'detection status'),
-        (rw_statuses, ttypes.ReviewStatus._NAMES_TO_VALUES,
+        (report_filter.reviewStatus, ttypes.ReviewStatus._VALUES_TO_NAMES,
          'review status')]
 
     if not all(valid for valid in
                [validate_filter_values(*x) for x in values_to_check]):
         sys.exit(1)
-    return severities, checkers, file_path, dt_statuses, rw_statuses, \
-        bug_path_length
-
-
-def add_filter_conditions(client, report_filter, args):
-    """
-    This function fills some attributes of the given report filter based on
-    the arguments which is provided in the command line.
-    """
-
-    severities, checkers, file_path, dt_statuses, rw_statuses, \
-        bug_path_length = check_filter_values(args)
 
     report_filter.isUnique = args.uniqueing == 'on'
 
-    if severities:
-        report_filter.severity = [
-            ttypes.Severity._NAMES_TO_VALUES[x.upper()] for x in severities]
-
-    if dt_statuses:
-        report_filter.detectionStatus = [
-            ttypes.DetectionStatus._NAMES_TO_VALUES[x.upper()] for x in
-            dt_statuses]
-
-    if rw_statuses:
-        report_filter.reviewStatus = [
-            ttypes.ReviewStatus._NAMES_TO_VALUES[x.upper()] for x in
-            rw_statuses]
-
-    if checkers:
-        report_filter.checkerName = checkers
-
     if 'checker_msg' in args:
         report_filter.checkerMsg = args.checker_msg
 
     if 'analyzer_name' in args:
         report_filter.analyzerNames = args.analyzer_name
 
     if 'component' in args:
         report_filter.componentNames = args.component
 
     if 'report_hash' in args:
         report_filter.reportHash = args.report_hash
 
-    if file_path:
-        report_filter.filepath = file_path
-
-    if bug_path_length:
-        report_filter.bugPathLength = \
-            ttypes.BugPathLengthRange(min=bug_path_length.min,
-                                      max=bug_path_length.max)
-
-    if 'tag' in args:
-        run_history_filter = ttypes.RunHistoryFilter(tagNames=args.tag)
-        run_histories = client.getRunHistory(None, None, None,
-                                             run_history_filter)
-        if run_histories:
-            report_filter.runTag = [t.id for t in run_histories]
-
     if 'open_reports_date' in args:
         report_filter.openReportsDate = \
             int(str_to_timestamp(args.open_reports_date))
 
     if 'detected_at' in args:
         report_filter.firstDetectionDate = \
             int(str_to_timestamp(args.detected_at))
@@ -544,14 +530,15 @@
 
         if 'fixed_after' in args:
             fixed_at.after = int(str_to_timestamp(args.fixed_after))
 
     if detected_at or fixed_at:
         report_filter.date = ttypes.ReportDate(detected=detected_at,
                                                fixed=fixed_at)
+    return report_filter
 
 
 def process_run_filter_conditions(args):
     """
     This function fills some attributes of the given run filter based on
     the arguments which is provided in the command line.
     """
@@ -658,16 +645,15 @@
 
     run_data = get_run_data(client, run_filter)
     run_ids = [run.runId for run in run_data]
     if not run_ids:
         LOG.warning("No runs were found!")
         sys.exit(1)
 
-    report_filter = ttypes.ReportFilter()
-    add_filter_conditions(client, report_filter, args)
+    report_filter = parse_report_filter(client, args)
 
     query_report_details = args.details and args.output_format == 'json' \
         if 'details' in args else None
 
     all_results = get_run_results(client,
                                   run_ids,
                                   constants.MAX_QUERY_SIZE,
@@ -716,54 +702,57 @@
             rows.append((checked_file, res.checkerId, sev, msg,
                          res.bugPathLength, res.analyzerName, rw_status,
                          dt_status))
 
         print(twodim.to_str(args.output_format, header, rows))
 
 
-def handle_diff_results(args):
-    # If the given output format is not 'table', redirect logger's output to
-    # the stderr.
-    stream = None
-    if 'output_format' in args and args.output_format != 'table':
-        stream = 'stderr'
+def get_source_line_contents(
+    client,
+    reports: List[ttypes.ReportData]
+) -> Dict[int, Dict[int, str]]:
+    """
+    Get source line contents from the server for the given report data.
+    """
+    source_lines = defaultdict(set)
+    for report_data in reports:
+        source_lines[report_data.fileId].add(report_data.line)
 
-    init_logger(args.verbose if 'verbose' in args else None, stream)
+    lines_in_files_requested = []
+    for file_id in source_lines:
+        lines_in_files_requested.append(
+            ttypes.LinesInFilesRequested(fileId=file_id,
+                                         lines=source_lines[file_id]))
 
-    output_dir = args.export_dir if 'export_dir' in args else None
-    if len(args.output_format) > 1 and ('export_dir' not in args):
-        LOG.error("Export directory is required if multiple output formats "
-                  "are selected!")
-        sys.exit(1)
+    return client.getLinesInSourceFileContents(
+        lines_in_files_requested, ttypes.Encoding.BASE64)
 
-    if 'html' in args.output_format and not output_dir:
-        LOG.error("Argument --export not allowed without argument --output "
-                  "when exporting to HTML.")
-        sys.exit(1)
 
-    if 'gerrit' in args.output_format and \
-            not gerrit.mandatory_env_var_is_set():
-        sys.exit(1)
-
-    check_deprecated_arg_usage(args)
-
-    if 'clean' in args and os.path.isdir(output_dir):
-        print("Previous analysis results in '{0}' have been removed, "
-              "overwriting with current results.".format(output_dir))
-        shutil.rmtree(output_dir)
+def convert_report_data_to_report(
+    client,
+    reports_data: List[ttypes.ReportData],
+    output_formats: List[str]
+) -> List[Report]:
+    """
+    Convert the given report data list to local reports.
 
-    if output_dir and not os.path.exists(output_dir):
-        os.makedirs(output_dir)
+    If one of the given output format is HTML it will get full source file
+    contents from the server otherwise for performance reason it will
+    get only necessarry line contents.
+    """
+    reports = []
 
-    context = webserver_context.get_context()
+    if not reports_data:
+        return reports
 
-    client = None
+    source_line_contents = {}
+    if 'html' not in output_formats:
+        source_line_contents = get_source_line_contents(client, reports_data)
 
     file_cache: Dict[int, File] = {}
-    print_steps = 'print_steps' in args
 
     def cached_report_file_lookup(file_id: int, file_path: str) -> File:
         """
         It will create a file object with the given 'file_path' attribute if
         file data is not found in the cache already based on the following
         conditions:
           - if HTML output is given it will try to get source file data for the
@@ -777,423 +766,453 @@
         Finally, it returns the source file data from the cache.
         """
         nonlocal file_cache
 
         if file_id not in file_cache:
             file_cache[file_id] = File(file_path, file_id)
 
-            if 'html' in args.output_format:
+            if 'html' in output_formats:
                 source = client.getSourceFileData(
                     file_id, True, ttypes.Encoding.BASE64)
                 file_cache[file_id].content = convert.from_b64(
                     source.fileContent)
 
         return file_cache[file_id]
 
-    def get_source_line_contents(
-        reports: List[ttypes.ReportData]
-    ) -> Dict[int, Dict[int, str]]:
-        """
-        Get source line contents from the server for the given report data.
-        """
-        source_lines = defaultdict(set)
-        for report_data in reports:
-            source_lines[report_data.fileId].add(report_data.line)
-
-        lines_in_files_requested = []
-        for file_id in source_lines:
-            lines_in_files_requested.append(
-                ttypes.LinesInFilesRequested(fileId=file_id,
-                                             lines=source_lines[file_id]))
-
-        return client.getLinesInSourceFileContents(
-            lines_in_files_requested, ttypes.Encoding.BASE64)
-
-    def convert_report_data_to_report(
-        reports_data: List[ttypes.ReportData]
-    ) -> List[Report]:
-        """
-        Convert the given report data list to local reports.
+    # Convert reports data to reports.
+    for report_data in reports_data:
+        report = report_type_converter.to_report(
+            report_data, cached_report_file_lookup)
 
-        If one of the given output format is HTML it will get full source file
-        contents from the server otherwise for performance reason it will
-        get only necessarry line contents.
-        """
-        reports = []
+        report.changed_files = []
+        report.source_code_comments = []
 
-        if not reports_data:
-            return reports
+        if source_line_contents:
+            source_line = convert.from_b64(
+                source_line_contents[report_data.fileId][report_data.line])
+            report.source_line = f"{source_line}{os.linesep}"
 
-        source_line_contents = {}
-        if 'html' not in args.output_format:
-            source_line_contents = get_source_line_contents(reports_data)
+        reports.append(report)
 
-        # Convert reports data to reports.
-        for report_data in reports_data:
-            report = report_type_converter.to_report(
-                report_data, cached_report_file_lookup)
+    return reports
 
-            report.changed_files = []
-            report.source_code_comments = []
 
-            if source_line_contents:
-                source_line = convert.from_b64(
-                    source_line_contents[report_data.fileId][report_data.line])
-                report.source_line = f"{source_line}{os.linesep}"
+def get_diff_local_dir_remote_run(
+    client,
+    report_filter: ttypes.ReportFilter,
+    diff_type: ttypes.DiffType,
+    output_formats: List[str],
+    report_dirs: List[str],
+    baseline_files: List[str],
+    remote_run_names: List[str]
+) -> Tuple[List[Report], List[str], List[str]]:
+    """ Compare a local report directory with a remote run. """
+    filtered_reports = []
+    filtered_report_hashes: Set[str] = set()
 
-            reports.append(report)
+    context = webserver_context.get_context()
+    report_dir_results = get_report_dir_results(
+        report_dirs, report_filter, context.checker_labels)
 
-        return reports
+    suppressed_in_code = \
+        get_suppressed_reports(report_dir_results, report_filter.reviewStatus)
 
-    def get_diff_local_dir_remote_run(
-        client,
-        report_dirs: List[str],
-        baseline_files: List[str],
-        remote_run_names: List[str]
-    ) -> Tuple[List[Report], List[str], List[str]]:
-        """ Compare a local report directory with a remote run. """
-        filtered_reports = []
-        filtered_report_hashes: Set[str] = set()
-
-        report_dir_results = get_report_dir_results(
-            report_dirs, args, context.checker_labels)
-        suppressed_in_code = get_suppressed_reports(report_dir_results, args)
+    run_ids, run_names, tag_ids = \
+        process_run_args(client, remote_run_names)
+    local_report_hashes = set([r.report_hash for r in report_dir_results])
+
+    review_status_filter = ttypes.ReviewStatusRuleFilter()
+    review_status_filter.reportHashes = local_report_hashes
+    review_status_filter.reviewStatuses = [
+        ttypes.ReviewStatus.FALSE_POSITIVE,
+        ttypes.ReviewStatus.INTENTIONAL]
+    closed_hashes = set(
+        rule.reportHash for rule in
+        client.getReviewStatusRules(
+            review_status_filter, None, None, None))
+
+    report_dir_results = [
+        r for r in report_dir_results if
+        r.review_status not in ['false positive', 'intentional'] and
+        (r.report_hash not in closed_hashes or
+         r.review_status == 'confirmed')]
+    local_report_hashes = set(r.report_hash for r in report_dir_results)
+    local_report_hashes.update(
+        baseline.get_report_hashes(baseline_files) - closed_hashes)
 
-        diff_type = get_diff_type(args)
-        run_ids, run_names, tag_ids = \
-            process_run_args(client, remote_run_names)
-        local_report_hashes = set([r.report_hash for r in report_dir_results])
-
-        review_status_filter = ttypes.ReviewStatusRuleFilter()
-        review_status_filter.reportHashes = local_report_hashes
-        review_status_filter.reviewStatuses = [
-            ttypes.ReviewStatus.FALSE_POSITIVE,
-            ttypes.ReviewStatus.INTENTIONAL]
-        closed_hashes = set(
-            rule.reportHash for rule in
-            client.getReviewStatusRules(
-                review_status_filter, None, None, None))
-
-        report_dir_results = [
-            r for r in report_dir_results if
-            r.review_status not in ['false positive', 'intentional'] and
-            (r.report_hash not in closed_hashes or
-             r.review_status == 'confirmed')]
-        local_report_hashes = set(r.report_hash for r in report_dir_results)
-        local_report_hashes.update(
-            baseline.get_report_hashes(baseline_files) - closed_hashes)
-
-        if diff_type == ttypes.DiffType.NEW:
-            # Get report hashes which can be found only in the remote runs.
-            remote_hashes = client.getDiffResultsHash(
-                run_ids, local_report_hashes, ttypes.DiffType.RESOLVED,
-                None, tag_ids)
+    if diff_type == ttypes.DiffType.NEW:
+        # Get report hashes which can be found only in the remote runs.
+        remote_hashes = client.getDiffResultsHash(
+            run_ids, local_report_hashes, ttypes.DiffType.RESOLVED,
+            None, tag_ids)
+
+        results = get_diff_base_results(
+            client, report_filter, run_ids, remote_hashes, suppressed_in_code)
 
+        filtered_reports.extend(
+            convert_report_data_to_report(client, results, output_formats))
+    elif diff_type == ttypes.DiffType.UNRESOLVED:
+        # Get remote hashes which can be found in the remote run and in the
+        # local report directory.
+        remote_hashes = client.getDiffResultsHash(
+            run_ids, local_report_hashes, ttypes.DiffType.UNRESOLVED,
+            None, tag_ids)
+
+        filtered_report_hashes = local_report_hashes.copy()
+        for result in report_dir_results:
+            rep_h = result.report_hash
+            filtered_report_hashes.discard(rep_h)
+            if rep_h in remote_hashes and rep_h not in suppressed_in_code:
+                filtered_reports.append(result)
+        filtered_report_hashes &= set(remote_hashes)
+
+        # Try to get missing report from the server based on the report
+        # hashes.
+        if filtered_report_hashes:
             results = get_diff_base_results(
-                client, args, run_ids, remote_hashes, suppressed_in_code)
+                client, report_filter, run_ids, list(filtered_report_hashes),
+                suppressed_in_code)
 
-            filtered_reports.extend(convert_report_data_to_report(results))
-        elif diff_type == ttypes.DiffType.UNRESOLVED:
-            # Get remote hashes which can be found in the remote run and in the
-            # local report directory.
-            remote_hashes = client.getDiffResultsHash(
-                run_ids, local_report_hashes, ttypes.DiffType.UNRESOLVED,
-                None, tag_ids)
-
-            filtered_report_hashes = local_report_hashes.copy()
-            for result in report_dir_results:
-                rep_h = result.report_hash
-                filtered_report_hashes.discard(rep_h)
-                if rep_h in remote_hashes and rep_h not in suppressed_in_code:
-                    filtered_reports.append(result)
-            filtered_report_hashes &= set(remote_hashes)
-
-            # Try to get missing report from the server based on the report
-            # hashes.
-            if filtered_report_hashes:
-                results = get_diff_base_results(
-                    client, args, run_ids, list(filtered_report_hashes),
-                    suppressed_in_code)
-
-                for result in results:
-                    filtered_report_hashes.discard(result.bugHash)
-
-                filtered_reports.extend(convert_report_data_to_report(results))
-        elif diff_type == ttypes.DiffType.RESOLVED:
-            # Get remote hashes which can be found in the remote run and in the
-            # local report directory.
-            remote_hashes = client.getDiffResultsHash(
-                run_ids, local_report_hashes, ttypes.DiffType.UNRESOLVED,
-                None, tag_ids)
-
-            filtered_report_hashes = local_report_hashes.copy()
-            for result in report_dir_results:
-                filtered_report_hashes.discard(result.report_hash)
-                if result.report_hash not in remote_hashes:
-                    filtered_reports.append(result)
-            filtered_report_hashes -= set(remote_hashes)
+            for result in results:
+                filtered_report_hashes.discard(result.bugHash)
 
-        return filtered_reports, filtered_report_hashes, run_names
+            filtered_reports.extend(
+                convert_report_data_to_report(client, results, output_formats))
+    elif diff_type == ttypes.DiffType.RESOLVED:
+        # Get remote hashes which can be found in the remote run and in the
+        # local report directory.
+        remote_hashes = client.getDiffResultsHash(
+            run_ids, local_report_hashes, ttypes.DiffType.UNRESOLVED,
+            None, tag_ids)
 
-    def get_diff_remote_run_local_dir(
-        client,
-        remote_run_names: List[str],
-        report_dirs: List[str],
-        baseline_files: List[str]
-    ) -> Tuple[List[Report], List[str], List[str]]:
-        """ Compares a remote run with a local report directory. """
-        filtered_reports = []
-        filtered_report_hashes = []
-
-        report_dir_results = get_report_dir_results(
-            report_dirs, args, context.checker_labels)
-        suppressed_in_code = get_suppressed_reports(report_dir_results, args)
+        filtered_report_hashes = local_report_hashes.copy()
+        for result in report_dir_results:
+            filtered_report_hashes.discard(result.report_hash)
+            if result.report_hash not in remote_hashes:
+                filtered_reports.append(result)
+        filtered_report_hashes -= set(remote_hashes)
 
-        diff_type = get_diff_type(args)
-        run_ids, run_names, tag_ids = \
-            process_run_args(client, remote_run_names)
-        local_report_hashes = set([r.report_hash for r in report_dir_results])
-
-        review_status_filter = ttypes.ReviewStatusRuleFilter()
-        review_status_filter.reportHashes = local_report_hashes
-        review_status_filter.reviewStatuses = [
-            ttypes.ReviewStatus.FALSE_POSITIVE,
-            ttypes.ReviewStatus.INTENTIONAL]
-        closed_hashes = set(
-            rule.reportHash for rule in
-            client.getReviewStatusRules(
-                review_status_filter, None, None, None))
-
-        report_dir_results = [
-            r for r in report_dir_results if
-            r.review_status not in ['false positive', 'intentional'] and
-            (r.report_hash not in closed_hashes or
-             r.review_status == 'confirmed')]
-        local_report_hashes = set(r.report_hash for r in report_dir_results)
-        local_report_hashes.update(
-            baseline.get_report_hashes(baseline_files) - closed_hashes)
+    return filtered_reports, filtered_report_hashes, run_names
 
-        remote_hashes = client.getDiffResultsHash(
-            run_ids, local_report_hashes, diff_type, None, tag_ids)
 
-        if not remote_hashes:
-            return filtered_reports, filtered_report_hashes, run_names
+def get_diff_remote_run_local_dir(
+    client,
+    report_filter: ttypes.ReportFilter,
+    diff_type: ttypes.DiffType,
+    output_formats: List[str],
+    remote_run_names: List[str],
+    report_dirs: List[str],
+    baseline_files: List[str]
+) -> Tuple[List[Report], List[str], List[str]]:
+    """ Compares a remote run with a local report directory. """
+    filtered_reports = []
+    filtered_report_hashes = []
 
-        if diff_type in [ttypes.DiffType.NEW, ttypes.DiffType.UNRESOLVED]:
-            # Shows reports from the report dir which are not present in
-            # the baseline (NEW reports) or appear in both side (UNRESOLVED
-            # reports) and not suppressed in the code.
-            filtered_report_hashes = set(remote_hashes)
-
-            for result in report_dir_results:
-                rep_h = result.report_hash
-                filtered_report_hashes.discard(rep_h)
-                if rep_h in remote_hashes and rep_h not in suppressed_in_code:
-                    filtered_reports.append(result)
-        elif diff_type == ttypes.DiffType.RESOLVED:
-            # Show bugs in the baseline (server) which are not present in
-            # the report dir or suppressed.
-            results = get_diff_base_results(
-                client, args, run_ids, remote_hashes, suppressed_in_code)
+    context = webserver_context.get_context()
+    report_dir_results = get_report_dir_results(
+        report_dirs, report_filter, context.checker_labels)
+    suppressed_in_code = \
+        get_suppressed_reports(report_dir_results, report_filter.reviewStatus)
+
+    run_ids, run_names, tag_ids = \
+        process_run_args(client, remote_run_names)
+    local_report_hashes = set([r.report_hash for r in report_dir_results])
+
+    review_status_filter = ttypes.ReviewStatusRuleFilter()
+    review_status_filter.reportHashes = local_report_hashes
+    review_status_filter.reviewStatuses = [
+        ttypes.ReviewStatus.FALSE_POSITIVE,
+        ttypes.ReviewStatus.INTENTIONAL]
+    closed_hashes = set(
+        rule.reportHash for rule in
+        client.getReviewStatusRules(
+            review_status_filter, None, None, None))
+
+    report_dir_results = [
+        r for r in report_dir_results if
+        r.review_status not in ['false positive', 'intentional'] and
+        (r.report_hash not in closed_hashes or
+         r.review_status == 'confirmed')]
+    local_report_hashes = set(r.report_hash for r in report_dir_results)
+    local_report_hashes.update(
+        baseline.get_report_hashes(baseline_files) - closed_hashes)
 
-            filtered_reports.extend(convert_report_data_to_report(results))
+    remote_hashes = client.getDiffResultsHash(
+        run_ids, local_report_hashes, diff_type, None, tag_ids)
 
+    if not remote_hashes:
         return filtered_reports, filtered_report_hashes, run_names
 
-    def get_diff_remote_runs(
-        client,
-        remote_base_run_names: Iterable[str],
-        remote_new_run_names: Iterable[str]
-    ) -> Tuple[List[Report], List[str], List[str]]:
-        """
-        Compares two remote runs and returns the filtered results.
-        """
-        report_filter = ttypes.ReportFilter()
-        add_filter_conditions(client, report_filter, args)
+    if diff_type in [ttypes.DiffType.NEW, ttypes.DiffType.UNRESOLVED]:
+        # Shows reports from the report dir which are not present in
+        # the baseline (NEW reports) or appear in both side (UNRESOLVED
+        # reports) and not suppressed in the code.
+        filtered_report_hashes = set(remote_hashes)
+
+        for result in report_dir_results:
+            rep_h = result.report_hash
+            filtered_report_hashes.discard(rep_h)
+            if rep_h in remote_hashes and rep_h not in suppressed_in_code:
+                filtered_reports.append(result)
+    elif diff_type == ttypes.DiffType.RESOLVED:
+        # Show bugs in the baseline (server) which are not present in
+        # the report dir or suppressed.
+        results = get_diff_base_results(
+            client, report_filter, run_ids, remote_hashes, suppressed_in_code)
 
-        base_ids, base_run_names, base_run_tags = \
-            process_run_args(client, remote_base_run_names)
-        report_filter.runTag = base_run_tags
-
-        cmp_data = ttypes.CompareData()
-        cmp_data.diffType = get_diff_type(args)
-
-        new_ids, new_run_names, new_run_tags = \
-            process_run_args(client, remote_new_run_names)
-        cmp_data.runIds = new_ids
-        cmp_data.runTag = new_run_tags
-
-        # Do not show resolved bugs in compare mode new.
-        if cmp_data.diffType == ttypes.DiffType.NEW:
-            report_filter.detectionStatus = [
-                ttypes.DetectionStatus.NEW,
-                ttypes.DetectionStatus.UNRESOLVED,
-                ttypes.DetectionStatus.REOPENED]
-
-        sort_mode = [(ttypes.SortMode(
-            ttypes.SortType.FILENAME,
-            ttypes.Order.ASC))]
-
-        all_results = get_run_results(
-            client, base_ids, constants.MAX_QUERY_SIZE, 0, sort_mode,
-            report_filter, cmp_data, True)
-
-        reports = convert_report_data_to_report(all_results)
-        return reports, base_run_names, new_run_names
-
-    def get_diff_local_dirs(
-        report_dirs: List[str],
-        baseline_files: List[str],
-        new_report_dirs: List[str],
-        new_baseline_files: List[str]
-    ) -> Tuple[List[Report], List[str]]:
-        """
-        Compares two report directories and returns the filtered results.
-        """
-        filtered_reports = []
-        filtered_report_hashes = []
+        filtered_reports.extend(
+            convert_report_data_to_report(client, results, output_formats))
 
-        base_results = get_report_dir_results(
-            report_dirs, args, context.checker_labels)
-        new_results = get_report_dir_results(
-            new_report_dirs, args, context.checker_labels)
-
-        new_results = [res for res in new_results
-                       if res.check_source_code_comments(args.review_status)]
-
-        base_hashes = set([res.report_hash for res in base_results])
-        new_hashes = set([res.report_hash for res in new_results])
-
-        # Add hashes from the baseline files.
-        base_hashes.update(baseline.get_report_hashes(baseline_files))
-        new_hashes.update(baseline.get_report_hashes(new_baseline_files))
+    return filtered_reports, filtered_report_hashes, run_names
 
-        diff_type = get_diff_type(args)
-        if diff_type == ttypes.DiffType.NEW:
-            filtered_report_hashes = new_hashes.copy()
-            for res in new_results:
-                filtered_report_hashes.discard(res.report_hash)
-
-                if res.report_hash not in base_hashes:
-                    filtered_reports.append(res)
-        if diff_type == ttypes.DiffType.UNRESOLVED:
-            filtered_report_hashes = new_hashes.copy()
-            for res in new_results:
-                filtered_report_hashes.discard(res.report_hash)
-
-                if res.report_hash in base_hashes:
-                    filtered_reports.append(res)
-        elif diff_type == ttypes.DiffType.RESOLVED:
-            filtered_report_hashes = base_hashes.copy()
-            for res in base_results:
-                filtered_report_hashes.discard(res.report_hash)
-
-                if res.report_hash not in new_hashes:
-                    filtered_reports.append(res)
-
-        return filtered_reports, filtered_report_hashes
-
-    def print_reports(
-        reports: List[Report],
-        report_hashes: Iterable[str],
-        output_formats: List[str]
-    ):
-        if report_hashes:
-            LOG.info("Couldn't get local reports for the following baseline "
-                     "report hashes: %s", ', '.join(sorted(report_hashes)))
-
-        statistics = Statistics()
-        changed_files: Set[str] = set()
-        html_builder: Optional[report_to_html.HtmlBuilder] = None
-        for report in reports:
-            statistics.add_report(report)
-
-            if report.changed_files:
-                changed_files.update(report.changed_files)
-
-            repo_dir = os.environ.get('CC_REPO_DIR')
-            if repo_dir:
-                report.trim_path_prefixes([repo_dir])
-
-        processed_file_paths = set()
-        for output_format in output_formats:
-            if output_format == 'plaintext':
-                file_report_map = plaintext.get_file_report_map(reports)
-                plaintext.convert(
-                    file_report_map, processed_file_paths, print_steps)
-
-            if output_format == 'html':
-                if not html_builder:
-                    html_builder = report_to_html.HtmlBuilder(
-                        context.path_plist_to_html_dist,
-                        context.checker_labels)
-
-                file_report_map = plaintext.get_file_report_map(reports)
-
-                LOG.info("Generating HTML output files to file://%s "
-                         "directory:", output_dir)
-
-                for file_path, file_reports in file_report_map.items():
-                    file_name = os.path.basename(file_path)
-                    h = int(
-                        hashlib.md5(
-                            file_path.encode('utf-8')).hexdigest(),
-                        16) % (10 ** 8)
-
-                    output_file_path = os.path.join(
-                        output_dir, f"{file_name}_ {str(h)}.html")
-                    html_builder.create(output_file_path, file_reports)
-
-            if output_format in ['csv', 'rows', 'table']:
-                header = ['File', 'Checker', 'Severity', 'Msg', 'Source']
-                rows = []
-                for report in reports:
-                    if report.source_line is None:
-                        continue
-
-                    checked_file = f"{report.file.path}:{str(report.line)}:" \
-                                   f"{str(report.column)}"
-                    rows.append((
-                        report.severity,
-                        checked_file,
-                        report.message,
-                        report.checker_name,
-                        report.source_line.rstrip()))
-
-                print(twodim.to_str(output_format, header, rows))
-
-            if output_format == 'json':
-                data = report_to_json.convert(reports)
-
-                report_json = os.path.join(output_dir, 'reports.json') \
-                    if output_dir else None
-                dump_json_output(data, report_json)
-
-            if output_format == 'gerrit':
-                data = gerrit.convert(reports)
-
-                report_json = os.path.join(
-                    output_dir, 'gerrit_review.json') if output_dir else None
-                dump_json_output(data, report_json)
-
-            if output_format == 'codeclimate':
-                data = codeclimate.convert(reports)
-
-                report_json = os.path.join(
-                    output_dir, 'codeclimate_issues.json') \
-                    if output_dir else None
-                dump_json_output(data, report_json)
 
-        if 'html' in output_formats:
-            html_builder.finish(output_dir, statistics)
+def get_diff_remote_runs(
+    client,
+    report_filter: ttypes.ReportFilter,
+    diff_type: ttypes.DiffType,
+    output_formats: List[str],
+    remote_base_run_names: Iterable[str],
+    remote_new_run_names: Iterable[str]
+) -> Tuple[List[Report], List[str], List[str]]:
+    """
+    Compares two remote runs and returns the filtered results.
+    """
+    base_ids, base_run_names, base_run_tags = \
+        process_run_args(client, remote_base_run_names)
+    report_filter.runTag = base_run_tags
+
+    cmp_data = ttypes.CompareData()
+    cmp_data.diffType = diff_type
+
+    new_ids, new_run_names, new_run_tags = \
+        process_run_args(client, remote_new_run_names)
+    cmp_data.runIds = new_ids
+    cmp_data.runTag = new_run_tags
+
+    # Do not show resolved bugs in compare mode new.
+    if cmp_data.diffType == ttypes.DiffType.NEW:
+        report_filter.detectionStatus = [
+            ttypes.DetectionStatus.NEW,
+            ttypes.DetectionStatus.UNRESOLVED,
+            ttypes.DetectionStatus.REOPENED]
+
+    sort_mode = [(ttypes.SortMode(
+        ttypes.SortType.FILENAME,
+        ttypes.Order.ASC))]
+
+    all_results = get_run_results(
+        client, base_ids, constants.MAX_QUERY_SIZE, 0, sort_mode,
+        report_filter, cmp_data, True)
+
+    reports = \
+        convert_report_data_to_report(client, all_results, output_formats)
+    return reports, base_run_names, new_run_names
+
+
+def get_diff_local_dirs(
+    report_filter: ttypes.ReportFilter,
+    diff_type: ttypes.DiffType,
+    # TODO: No output_format argument? How come? Maybe the other functions
+    # don't need it either?
+    report_dirs: List[str],
+    baseline_files: List[str],
+    new_report_dirs: List[str],
+    new_baseline_files: List[str]
+) -> Tuple[List[Report], List[str]]:
+    """
+    Compares two report directories and returns the filtered results.
+    """
+    filtered_reports = []
+    filtered_report_hashes = []
+
+    context = webserver_context.get_context()
+    statuses_str = [ttypes.ReviewStatus._VALUES_TO_NAMES[x].lower()
+                    for x in report_filter.reviewStatus]
+
+    base_results = get_report_dir_results(
+        report_dirs, report_filter, context.checker_labels)
+    base_results = [res for res in base_results
+                    if res.check_source_code_comments(statuses_str)]
+
+    new_results = get_report_dir_results(
+        new_report_dirs, report_filter, context.checker_labels)
+    new_results = [res for res in new_results
+                   if res.check_source_code_comments(statuses_str)]
+
+    base_hashes = set([res.report_hash for res in base_results])
+    new_hashes = set([res.report_hash for res in new_results])
+
+    # Add hashes from the baseline files.
+    base_hashes.update(baseline.get_report_hashes(baseline_files))
+    new_hashes.update(baseline.get_report_hashes(new_baseline_files))
+
+    if diff_type == ttypes.DiffType.NEW:
+        filtered_report_hashes = new_hashes.copy()
+        for res in new_results:
+            filtered_report_hashes.discard(res.report_hash)
+
+            if res.report_hash not in base_hashes:
+                filtered_reports.append(res)
+    if diff_type == ttypes.DiffType.UNRESOLVED:
+        filtered_report_hashes = new_hashes.copy()
+        for res in new_results:
+            filtered_report_hashes.discard(res.report_hash)
+
+            if res.report_hash in base_hashes:
+                filtered_reports.append(res)
+    elif diff_type == ttypes.DiffType.RESOLVED:
+        filtered_report_hashes = base_hashes.copy()
+        for res in base_results:
+            filtered_report_hashes.discard(res.report_hash)
+
+            if res.report_hash not in new_hashes:
+                filtered_reports.append(res)
+
+    return filtered_reports, filtered_report_hashes
+
+
+def print_reports(
+    print_steps: bool,
+    reports: List[Report],
+    report_hashes: Iterable[str],
+    output_dir: str,
+    output_formats: List[str]
+):
+    if report_hashes:
+        LOG.info("Couldn't get local reports for the following baseline "
+                 "report hashes: %s", ', '.join(sorted(report_hashes)))
+
+    statistics = Statistics()
+    changed_files: Set[str] = set()
+    html_builder: Optional[report_to_html.HtmlBuilder] = None
+    for report in reports:
+        statistics.add_report(report)
+
+        if report.changed_files:
+            changed_files.update(report.changed_files)
+
+        repo_dir = os.environ.get('CC_REPO_DIR')
+        if repo_dir:
+            report.trim_path_prefixes([repo_dir])
+
+    processed_file_paths = set()
+    for output_format in output_formats:
+        if output_format == 'plaintext':
+            file_report_map = plaintext.get_file_report_map(reports)
+            plaintext.convert(
+                file_report_map, processed_file_paths, print_steps)
+
+        context = webserver_context.get_context()
+        if output_format == 'html':
+            if not html_builder:
+                html_builder = report_to_html.HtmlBuilder(
+                    context.path_plist_to_html_dist,
+                    context.checker_labels)
+
+            file_report_map = plaintext.get_file_report_map(reports)
+
+            LOG.info("Generating HTML output files to file://%s "
+                     "directory:", output_dir)
+
+            for file_path, file_reports in file_report_map.items():
+                file_name = os.path.basename(file_path)
+                h = int(
+                    hashlib.md5(
+                        file_path.encode('utf-8')).hexdigest(),
+                    16) % (10 ** 8)
+
+                output_file_path = os.path.join(
+                    output_dir, f"{file_name}_ {str(h)}.html")
+                html_builder.create(output_file_path, file_reports)
+
+        if output_format in ['csv', 'rows', 'table']:
+            header = ['File', 'Checker', 'Severity', 'Msg', 'Source']
+            rows = []
+            for report in reports:
+                if report.source_line is None:
+                    continue
+
+                checked_file = f"{report.file.path}:{str(report.line)}:" \
+                               f"{str(report.column)}"
+                rows.append((
+                    report.severity,
+                    checked_file,
+                    report.message,
+                    report.checker_name,
+                    report.source_line.rstrip()))
+
+            print(twodim.to_str(output_format, header, rows))
+
+        if output_format == 'json':
+            data = report_to_json.convert(reports)
+
+            report_json = os.path.join(output_dir, 'reports.json') \
+                if output_dir else None
+            dump_json_output(data, report_json)
+
+        if output_format == 'gerrit':
+            data = gerrit.convert(reports)
+
+            report_json = os.path.join(
+                output_dir, 'gerrit_review.json') if output_dir else None
+            dump_json_output(data, report_json)
+
+        if output_format == 'codeclimate':
+            data = codeclimate.convert(reports)
+
+            report_json = os.path.join(
+                output_dir, 'codeclimate_issues.json') \
+                if output_dir else None
+            dump_json_output(data, report_json)
+
+    if 'html' in output_formats:
+        html_builder.finish(output_dir, statistics)
 
-        if 'plaintext' in output_formats:
-            statistics.write()
+    if 'plaintext' in output_formats:
+        statistics.write()
 
-        reports_helper.dump_changed_files(changed_files)
+    reports_helper.dump_changed_files(changed_files)
+
+
+def handle_diff_results(args):
+    # If the given output format is not 'table', redirect logger's output to
+    # the stderr.
+    stream = None
+    output_formats = args.output_format
+    if output_formats != 'table':
+        stream = 'stderr'
+
+    init_logger(args.verbose if 'verbose' in args else None, stream)
+
+    output_dir = args.export_dir if 'export_dir' in args else None
+    if len(output_formats) > 1 and ('export_dir' not in args):
+        LOG.error("Export directory is required if multiple output formats "
+                  "are selected!")
+        sys.exit(1)
+
+    if 'html' in output_formats and not output_dir:
+        LOG.error("Argument --export not allowed without argument --output "
+                  "when exporting to HTML.")
+        sys.exit(1)
+
+    if 'gerrit' in output_formats and \
+            not gerrit.mandatory_env_var_is_set():
+        sys.exit(1)
+
+    check_deprecated_arg_usage(args)
+
+    if 'clean' in args and os.path.isdir(output_dir):
+        print("Previous analysis results in '{0}' have been removed, "
+              "overwriting with current results.".format(output_dir))
+        shutil.rmtree(output_dir)
+
+    if output_dir and not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+
+    client = None
 
     basename_local_dirs, basename_baseline_files, basename_run_names = \
         filter_local_file_remote_run(args.base_run_names)
 
     newname_local_dirs, newname_baseline_files, newname_run_names = \
         filter_local_file_remote_run(args.new_run_names)
 
@@ -1246,53 +1265,74 @@
         except SystemExit as sexit:
             LOG.error("Failed to get remote runs from server! Please "
                       "make sure that CodeChecker server is running on host "
                       "'%s' or these are valid directory paths!",
                       args.product_url)
             raise sexit
 
+    print_steps = 'print_steps' in args
     report_hashes = []
     if (basename_local_dirs or basename_baseline_files) and \
        (newname_local_dirs or newname_baseline_files):
+        report_filter = parse_report_filter_offline(args)
+        diff_type = get_diff_type(args)
+
         reports, report_hashes = get_diff_local_dirs(
+            report_filter, diff_type,
             basename_local_dirs, basename_baseline_files,
             newname_local_dirs, newname_baseline_files)
 
-        print_reports(reports, report_hashes, args.output_format)
+        print_reports(print_steps, reports, report_hashes, output_dir,
+                      output_formats)
         LOG.info("Compared the following local files / directories: %s and %s",
                  ', '.join([*basename_local_dirs, *basename_baseline_files]),
                  ', '.join([*newname_local_dirs, *newname_baseline_files]))
     elif newname_local_dirs or newname_baseline_files:
+        report_filter = parse_report_filter(client, args)
+        diff_type = get_diff_type(args)
+
         reports, report_hashes, matching_base_run_names = \
             get_diff_remote_run_local_dir(
-                client, basename_run_names,
+                client, report_filter, diff_type, output_formats,
+                basename_run_names,
                 newname_local_dirs, newname_baseline_files)
 
-        print_reports(reports, report_hashes, args.output_format)
+        print_reports(print_steps, reports, report_hashes, output_dir,
+                      output_formats)
         LOG.info("Compared remote run(s) %s (matching: %s) and local files / "
                  "report directory(s) %s",
                  ', '.join(basename_run_names),
                  ', '.join(matching_base_run_names),
                  ', '.join([*newname_local_dirs, *newname_baseline_files]))
     elif (basename_local_dirs or basename_baseline_files):
+        report_filter = parse_report_filter(client, args)
+        diff_type = get_diff_type(args)
+
         reports, report_hashes, matching_new_run_names = \
             get_diff_local_dir_remote_run(
-                client, basename_local_dirs, basename_baseline_files,
-                newname_run_names)
+                client, report_filter, diff_type, output_formats,
+                basename_local_dirs,
+                basename_baseline_files, newname_run_names)
 
-        print_reports(reports, report_hashes, args.output_format)
+        print_reports(print_steps, reports, report_hashes, output_dir,
+                      output_formats)
         LOG.info("Compared local files / report directory(s) %s and remote "
                  "run(s) %s (matching: %s).",
                  ', '.join([*basename_local_dirs, *basename_baseline_files]),
                  ', '.join(newname_run_names),
                  ', '.join(matching_new_run_names))
     else:
+        report_filter = parse_report_filter(client, args)
+        diff_type = get_diff_type(args)
+
         reports, matching_base_run_names, matching_new_run_names = \
-            get_diff_remote_runs(client, basename_run_names, newname_run_names)
-        print_reports(reports, None, args.output_format)
+            get_diff_remote_runs(
+                client, report_filter, diff_type, output_formats,
+                basename_run_names, newname_run_names)
+        print_reports(print_steps, reports, None, output_dir, output_formats)
         LOG.info("Compared multiple remote runs %s (matching: %s) and %s "
                  "(matching: %s)",
                  ', '.join(basename_run_names),
                  ', '.join(matching_base_run_names),
                  ', '.join(newname_run_names),
                  ', '.join(matching_new_run_names))
 
@@ -1307,16 +1347,15 @@
     if 'output_format' in args and args.output_format != 'table':
         stream = 'stderr'
 
     init_logger(args.verbose if 'verbose' in args else None, stream)
     check_deprecated_arg_usage(args)
 
     def get_statistics(client, run_ids, field, values):
-        report_filter = ttypes.ReportFilter()
-        add_filter_conditions(client, report_filter, args)
+        report_filter = parse_report_filter(client, args)
 
         setattr(report_filter, field, values)
         checkers = client.getCheckerCounts(run_ids,
                                            report_filter,
                                            None,
                                            None,
                                            0)
@@ -1332,16 +1371,15 @@
     if 'all_results' not in args:
         run_filter = ttypes.RunFilter(names=args.names)
         run_ids = [run.runId for run in get_run_data(client, run_filter)]
         if not run_ids:
             LOG.warning("No runs were found!")
             sys.exit(1)
 
-    all_checkers_report_filter = ttypes.ReportFilter()
-    add_filter_conditions(client, all_checkers_report_filter, args)
+    all_checkers_report_filter = parse_report_filter(client, args)
 
     all_checkers = client.getCheckerCounts(run_ids,
                                            all_checkers_report_filter,
                                            None,
                                            None,
                                            0)
     all_checkers_dict = dict((res.name, res) for res in all_checkers)
@@ -1355,16 +1393,15 @@
     false_checkers = get_statistics(client, run_ids, 'reviewStatus',
                                     [ttypes.ReviewStatus.FALSE_POSITIVE])
 
     intentional_checkers = get_statistics(client, run_ids, 'reviewStatus',
                                           [ttypes.ReviewStatus.INTENTIONAL])
 
     # Get severity counts
-    report_filter = ttypes.ReportFilter()
-    add_filter_conditions(client, report_filter, args)
+    report_filter = parse_report_filter(client, args)
 
     sev_count = client.getSeverityCounts(run_ids, report_filter, None)
 
     severities = []
     severity_total = 0
     for key, count in sorted(list(sev_count.items()),
                              reverse=True):
@@ -1439,15 +1476,17 @@
 
     client = setup_client(args.product_url)
 
     run_filter = process_run_filter_conditions(args)
     if client.removeRun(None, run_filter):
         LOG.info("Done.")
     else:
-        LOG.error("Failed to remove runs!")
+        LOG.warning(
+            "No runs were removed, check if the given criteria match existing "
+            "run names.")
 
 
 def handle_update_run(args):
     """
     Argument handler for the 'CodeChecker cmd update' subcommand.
     """
     init_logger(args.verbose if 'verbose' in args else None)
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/credential_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/credential_manager.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/authentication.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/base.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/base.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/configuration.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/configuration.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/product.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/product.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/results.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/helpers/results.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/metadata.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/metadata.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/permission_client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/permission_client.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/product.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/product.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/product_client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/product_client.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/report_type_converter.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/report_type_converter.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/source_component_client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/source_component_client.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/suppress_file_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/suppress_file_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/thrift_call.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/thrift_call.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_client/token_client.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_client/token_client.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/arg.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/arg.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/checker_labels.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/checker_labels.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cli.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cli.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/version.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd/version.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/cmd_config.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/cmd_config.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/logger.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/logger.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/singleton.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/singleton.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/skiplist_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/skiplist_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_common/util.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_common/util.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/cli.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/cli.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/merge_clang_extdef_mappings.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_merge_clang_extdef_mappings/merge_clang_extdef_mappings.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/analyzer_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 import logging
 import os
 
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 import hashlib
-from typing import Dict, List, Optional
+from typing import Dict, Iterable, List, Optional
 
 from codechecker_report_converter.report import Report, report_file
 from codechecker_report_converter.report.hash import get_report_hash, HashType
 from codechecker_report_converter.report.parser.base import AnalyzerInfo
 
 
 LOG = logging.getLogger('report-converter')
@@ -33,15 +33,15 @@
     NAME: str = ''
 
     # Link to the official analyzer website.
     URL: str = ''
 
     def transform(
         self,
-        analyzer_result_file_path: str,
+        analyzer_result_file_paths: Iterable[str],
         output_dir_path: str,
         export_type: str,
         file_name: str = "{source_file}_{analyzer}_{file_hash}",
         metadata: Optional[Dict[str, str]] = None
     ) -> bool:
         """
         Converts the given analyzer result to the output directory in the given
@@ -49,41 +49,45 @@
         """
         parser = report_file.get_parser(f".{export_type}")
         if not parser:
             LOG.error("The given output type '%s' is not supported!",
                       export_type)
             return False
 
-        analyzer_result_file_path = os.path.abspath(analyzer_result_file_path)
-        reports = self.get_reports(analyzer_result_file_path)
-        if not reports:
-            LOG.info("No '%s' results can be found in the given code analyzer "
-                     "output.", self.TOOL_NAME)
-            return False
+        all_reports = []
+
+        for file_path in analyzer_result_file_paths:
+            file_path = os.path.abspath(file_path)
+            reports = self.get_reports(file_path)
+            if not reports:
+                LOG.info("No '%s' results can be found in '%s'.",
+                         self.TOOL_NAME, file_path)
+
+            self._post_process_result(reports)
 
-        self._post_process_result(reports)
+            for report in reports:
+                report.analyzer_result_file_path = file_path
 
-        for report in reports:
-            report.analyzer_result_file_path = analyzer_result_file_path
+                if not report.checker_name:
+                    report.checker_name = self.TOOL_NAME
 
-            if not report.checker_name:
-                report.checker_name = self.TOOL_NAME
+            all_reports.extend(reports)
 
         self._write(
-            reports, output_dir_path, parser, export_type, file_name)
+            all_reports, output_dir_path, parser, export_type, file_name)
 
         if metadata:
             self._save_metadata(metadata, output_dir_path)
         else:
             LOG.warning("Use '--meta' option to provide extra information "
                         "to the CodeChecker server such as analyzer version "
                         "and analysis command when storing the results to it. "
                         "For more information see the --help.")
 
-        return True
+        return bool(all_reports)
 
     @abstractmethod
     def get_reports(self, analyzer_result_file_path: str) -> List[Report]:
         """ Get reports from the given analyzer result. """
         raise NotImplementedError("Subclasses should implement this!")
 
     def _save_metadata(self, metadata, output_dir):
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/clang_tidy/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/coccinelle/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cppcheck/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/cpplint/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/eslint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/golint/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/infer/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/kerneldoc/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/markdownlint/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pyflakes/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/pylint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/roslynator/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/address/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 from ..parser import SANParser
 
 LOG = logging.getLogger('report-converter')
 
 
 class Parser(SANParser):
-    """ Parser for Clang AddressSanitizer console outputs. """
+    """ Parser for Clang LeakSanitizer console outputs. """
 
-    checker_name = "AddressSanitizer"
+    checker_name = "LeakSanitizer"
 
-    # Regex for parsing AddressSanitizer output message.
+    # Regex for parsing MemorySanitizer output message.
     line_re = re.compile(
-            # Error code
-            r'==(?P<code>\d+)==(ERROR|WARNING): AddressSanitizer: '
-            # Checker message.
-            r'(?P<message>[\S \t]+)')
+        r'(?P<message>(Ind|D)irect leak of \d+ byte\(s\) '
+        r'in \d+ object\(s\) allocated from:)')
+
+    skip_line_after_match = False
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/leak/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 #
 #  Part of the CodeChecker project, under the Apache License v2.0 with
 #  LLVM Exceptions. See LICENSE for license information.
 #  SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 #
 # -------------------------------------------------------------------------
 
+
 import logging
 import re
 
 from ..parser import SANParser
 
+
 LOG = logging.getLogger('report-converter')
 
 
 class Parser(SANParser):
-    """ Parser for Clang LeakSanitizer console outputs. """
+    """ Parser for Clang MemorySanitizer console outputs. """
 
-    checker_name = "LeakSanitizer"
+    checker_name = "MemorySanitizer"
 
     # Regex for parsing MemorySanitizer output message.
     line_re = re.compile(
-            # Error code
-            r'==(?P<code>\d+)==(ERROR|WARNING): LeakSanitizer: '
-            # Checker message.
-            r'(?P<message>[\S \t]+)')
+        # Error code
+        r'==(?P<code>\d+)==(ERROR|WARNING): MemorySanitizer: '
+        # Checker message.
+        r'(?P<message>[\S \t]+)')
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/memory/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 #
 #  Part of the CodeChecker project, under the Apache License v2.0 with
 #  LLVM Exceptions. See LICENSE for license information.
 #  SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 #
 # -------------------------------------------------------------------------
 
-
 import logging
 import re
 
 from ..parser import SANParser
 
 
 LOG = logging.getLogger('report-converter')
 
 
 class Parser(SANParser):
-    """ Parser for Clang MemorySanitizer console outputs. """
+    """ Parser for Clang AddressSanitizer console outputs. """
 
-    checker_name = "MemorySanitizer"
+    checker_name = "ThreadSanitizer"
+    main_event_index = 0
 
-    # Regex for parsing MemorySanitizer output message.
+    # Regex for parsing ThreadSanitizer output message.
     line_re = re.compile(
         # Error code
-        r'==(?P<code>\d+)==(ERROR|WARNING): MemorySanitizer: '
+        r'==(?P<code>\d+)==(ERROR|WARNING): ThreadSanitizer: '
         # Checker message.
         r'(?P<message>[\S \t]+)')
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/thread/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sanitizers/ub/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,78 +6,98 @@
 #
 # -------------------------------------------------------------------------
 
 import logging
 import os
 import re
 
-from typing import Iterable, Optional, Tuple
+from typing import Iterator, List, Tuple
 
-from codechecker_report_converter.report import get_or_create_file, Report
-
-from ...parser import get_next
-from ..parser import SANParser
+from codechecker_report_converter.report import BugPathEvent, \
+    get_or_create_file, Report
+from ..parser import BaseParser
 
 
 LOG = logging.getLogger('report-converter')
 
 
-class Parser(SANParser):
-    """ Parser for Clang UndefinedBehaviourSanitizer console outputs.
-
-    Example output
-        /a/b/main.cpp:13:10: runtime error: load of value 7...
+class Parser(BaseParser):
+    """
+    Parser for Sparse Output
     """
 
-    checker_name = "UndefinedBehaviorSanitizer"
-
-    # Regex for parsing UndefinedBehaviorSanitizer output message.
-    line_re = re.compile(
-        # File path followed by a ':'.
-        r'^(?P<path>[\S ]+?):'
-        # Line number followed by a ':'.
-        r'(?P<line>\d+?):'
-        # Column number followed by a ':' and a space.
-        r'(?P<column>\d+?): runtime error: '
-        # Checker message.
-        r'(?P<message>[\S \t]+)')
-
-    def parse_stack_trace(self, it, line):
-        """ Iterate over lines and parse stack traces. """
-        events = []
-        stack_traces = []
-
-        while self.stack_trace_re.match(line):
-            event = self.parse_stack_trace_line(line)
-            if event:
-                events.append(event)
-
-            stack_traces.append(line)
-            line = get_next(it)
+    def __init__(self, analyzer_result):
+        super(Parser, self).__init__()
 
-        events.reverse()
+        self.analyzer_result = analyzer_result
 
-        return stack_traces, events, line
+        self.message_line_re = re.compile(
+            # File path followed by a ':'.
+            r'^(?P<path>[\S ]+?):'
+            # Line number followed by a ':'.
+            r'(?P<line>\d+?):'
+            # Column number followed by a ':'.
+            r'(?P<column>\d+?):'
+            # Message.
+            r'(?P<message>[\S \t]+)\s*')
+
+        self.note_line_re = re.compile(
+            # File path followed by a ':'.
+            r'^(?P<path>\.[\S ]+?):'
+            # Line number followed by a ':'.
+            r'(?P<line>\d+?):'
+            # Column number followed by a ':'.
+            r'(?P<column>\d+?):'
+            # Message.
+            r'(?P<message>[\S \t]+)\s*'
+        )
 
-    def parse_sanitizer_message(
+    def _parse_line(
         self,
-        it: Iterable[str],
+        it: Iterator[str],
         line: str
-    ) -> Tuple[Optional[Report], str]:
-        """ Parses UndefinedBehaviorSanitizer output message. """
-        match = self.line_re.match(line)
-        if not match:
-            return None, line
-
-        report_file = get_or_create_file(
-            os.path.abspath(match.group('path')), self._file_cache)
-        report_line = int(match.group('line'))
-        report_col = int(match.group('column'))
-
-        line = get_next(it)
-        stack_traces, events, line = self.parse_stack_trace(it, line)
-
-        report = self.create_report(
-            events, report_file, report_line, report_col,
-            match.group('message').strip(), stack_traces)
+    ) -> Tuple[List[Report], str]:
+        """ Parse the given line. """
+        match = self.message_line_re.match(line)
+
+        if (match is None):
+            return [], next(it)
+
+        file_path = os.path.normpath(
+            os.path.join(os.path.dirname(self.analyzer_result),
+                         match.group('path')))
+
+        report = Report(
+            get_or_create_file(file_path, self._file_cache),
+            int(match.group('line')),
+            int(match.group('column')),
+            match.group('message').strip(),
+            '',
+            bug_path_events=[])
+
+        line = ''
+        try:
+            line = next(it)
+            note_match = self.note_line_re.match(line)
+            while note_match:
+                file_path = os.path.normpath(
+                    os.path.join(os.path.dirname(self.analyzer_result),
+                                 note_match.group('path')))
+
+                report.bug_path_events.append(BugPathEvent(
+                    note_match.group('message').strip(),
+                    get_or_create_file(file_path, self._file_cache),
+                    int(note_match.group('line')),
+                    int(note_match.group('column'))))
+
+                line = next(it)
+                note_match = self.note_line_re.match(line)
+        except StopIteration:
+            line = ''
+        finally:
+            report.bug_path_events.append(BugPathEvent(
+                report.message,
+                report.file,
+                report.line,
+                report.column))
 
-        return report, line
+            return [report], line
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/smatch/parser.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sparse/parser.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,96 +8,58 @@
 
 import logging
 import os
 import re
 
 from typing import Iterator, List, Tuple
 
-from codechecker_report_converter.report import BugPathEvent, \
-    get_or_create_file, Report
+from codechecker_report_converter.report import get_or_create_file, Report
 from ..parser import BaseParser
 
 
 LOG = logging.getLogger('report-converter')
 
 
 class Parser(BaseParser):
     """
-    Parser for Sparse Output
+    Parser for Sphinx Output
     """
 
     def __init__(self, analyzer_result):
         super(Parser, self).__init__()
 
         self.analyzer_result = analyzer_result
 
         self.message_line_re = re.compile(
-            # File path followed by a ':'.
-            r'^(?P<path>[\S ]+?):'
+            # File path starting with '/' and followed by a ':'.
+            r'^(?P<path>\/[\S ]+?):'
             # Line number followed by a ':'.
-            r'(?P<line>\d+?):'
-            # Column number followed by a ':'.
-            r'(?P<column>\d+?):'
+            r'(?P<line>\d+?):\s'
             # Message.
             r'(?P<message>[\S \t]+)\s*')
 
-        self.note_line_re = re.compile(
-            # File path followed by a ':'.
-            r'^(?P<path>\.[\S ]+?):'
-            # Line number followed by a ':'.
-            r'(?P<line>\d+?):'
-            # Column number followed by a ':'.
-            r'(?P<column>\d+?):'
-            # Message.
-            r'(?P<message>[\S \t]+)\s*'
-        )
-
     def _parse_line(
         self,
         it: Iterator[str],
         line: str
     ) -> Tuple[List[Report], str]:
         """ Parse the given line. """
         match = self.message_line_re.match(line)
 
-        if (match is None):
+        if match is None:
             return [], next(it)
 
         file_path = os.path.normpath(
             os.path.join(os.path.dirname(self.analyzer_result),
                          match.group('path')))
 
         report = Report(
             get_or_create_file(file_path, self._file_cache),
             int(match.group('line')),
-            int(match.group('column')),
+            0,
             match.group('message').strip(),
-            '',
-            bug_path_events=[])
+            '')
 
-        line = ''
         try:
-            line = next(it)
-            note_match = self.note_line_re.match(line)
-            while note_match:
-                file_path = os.path.normpath(
-                    os.path.join(os.path.dirname(self.analyzer_result),
-                                 note_match.group('path')))
-
-                report.bug_path_events.append(BugPathEvent(
-                    note_match.group('message').strip(),
-                    get_or_create_file(file_path, self._file_cache),
-                    int(note_match.group('line')),
-                    int(note_match.group('column'))))
-
-                line = next(it)
-                note_match = self.note_line_re.match(line)
+            return [report], next(it)
         except StopIteration:
-            line = ''
-        finally:
-            report.bug_path_events.append(BugPathEvent(
-                report.message,
-                report.file,
-                report.line,
-                report.column))
-
-            return [report], line
+            return [report], ''
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/sphinx/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/spotbugs/analyzer_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,20 +46,29 @@
         for bug in root.findall('BugInstance'):
             report = self.__parse_bug(bug)
             if report:
                 reports.append(report)
 
         return reports
 
-    def __get_abs_path(self, source_path: str):
-        """ Returns full path of the given source path.
+    def __get_abs_path(self, source_line):
+        """ Returns full source path of the given source line.
 
         It will try to find the given source path in the project paths and
         returns full path if it founds.
         """
+        if source_line is None:
+            return None
+
+        source_path = source_line.attrib.get('sourcepath')
+        if source_path is None:
+            LOG.warning("No source path attribute found for class: %s",
+                        source_line.attrib.get('classname'))
+            return None
+
         if os.path.exists(source_path):
             return source_path
 
         for project_path in self.__project_paths:
             full_path = os.path.join(project_path, source_path)
             if os.path.exists(full_path):
                 return full_path
@@ -101,16 +110,15 @@
         """ Parse the given bug and create a message from them. """
         report_hash = bug.attrib.get('instanceHash')
         checker_name = bug.attrib.get('type')
 
         long_message = bug.find('LongMessage').text
 
         source_line = bug.find('SourceLine')
-        source_path = source_line.attrib.get('sourcepath')
-        source_path = self.__get_abs_path(source_path)
+        source_path = self.__get_abs_path(source_line)
         if not source_path:
             return
 
         line = source_line.attrib.get('start')
         col = 0
 
         events = []
@@ -144,19 +152,15 @@
         return report
 
     def __event_from_class(self, element) -> Optional[BugPathEvent]:
         """ Creates event from a Class element. """
         message = element.find('Message').text
 
         source_line = element.find('SourceLine')
-        if source_line is None:
-            return None
-
-        source_path = source_line.attrib.get('sourcepath')
-        source_path = self.__get_abs_path(source_path)
+        source_path = self.__get_abs_path(source_line)
         if not source_path:
             return None
 
         line = int(source_line.attrib.get('start', 0))
         col = 0
 
         return BugPathEvent(
@@ -166,19 +170,15 @@
             col)
 
     def __event_from_method(self, element) -> Optional[BugPathEvent]:
         """ Creates event from a Method element. """
         message = element.find('Message').text
 
         source_line = element.find('SourceLine')
-        if source_line is None:
-            return None
-
-        source_path = source_line.attrib.get('sourcepath')
-        source_path = self.__get_abs_path(source_path)
+        source_path = self.__get_abs_path(source_line)
         if not source_path:
             return None
 
         line = int(source_line.attrib.get('start', 0))
         col = 0
 
         return BugPathEvent(
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/analyzer_result.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/analyzers/tslint/analyzer_result.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/cli.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 #  LLVM Exceptions. See LICENSE for license information.
 #  SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 #
 # -------------------------------------------------------------------------
 
 
 import argparse
+from collections.abc import Iterable, Sequence
 import glob
 import importlib
 import logging
 import os
 import shutil
 import sys
 
-from typing import Dict, Optional, Tuple
+from typing import Any, Dict, Iterable, Optional, Sequence, Tuple, Union
 
 
 # If we run this script in an environment where 'codechecker_report_converter'
 # module is not available we should add the grandparent directory of this file
 # to the system path.
 # TODO: This section will not be needed when CodeChecker will be delivered as
 # a python package and will be installed in a virtual environment with all the
@@ -75,15 +76,15 @@
         pass
 
 
 supported_metadata_keys = ["analyzer_command", "analyzer_version"]
 
 
 def transform_output(
-    analyzer_result: str,
+    analyzer_result: Iterable[str],
     parser_type: str,
     output_dir: str,
     file_name: str,
     export_type: str,
     clean: bool = False,
     metadata: Optional[Dict[str, str]] = None
 ):
@@ -114,23 +115,65 @@
             valid_values[key] = value
         else:
             invalid_values[key] = value
 
     return valid_values, invalid_values
 
 
+class CollectFiles(argparse.Action):
+    """
+    This report-converter tool can be given a set of files and directories as
+    positional command line arguments. This action collects all files at the
+    given locations: if an argument is a file then that file is collected, if
+    it's a directory then its content is inspected recursively.
+    """
+    def __init__(
+        self,
+        option_strings: Sequence[str],
+        dest: str,
+        nargs: Union[int, str, None],
+        **kwargs
+    ) -> None:
+        if nargs != "+":
+            raise ValueError("'nargs' option for 'input' should be '+'.")
+        super().__init__(option_strings, dest, nargs, **kwargs)
+
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: Union[str, Sequence[Any], None],
+        option_string: Union[str, None] = None
+    ):
+        # Type of "values" can have any of the indicated types above. But in
+        # argument parser it is given by "nargs='+'", so it will be a list in
+        # this specific case.
+        assert isinstance(values, Sequence)
+
+        all_files = []
+
+        for path in values:
+            if os.path.isfile(path):
+                all_files.append(path)
+            else:
+                for root, _, files in os.walk(path):
+                    all_files.extend(os.path.join(root, f) for f in files)
+
+        setattr(namespace, 'input', all_files)
+
+
 def __add_arguments_to_parser(parser):
     """ Add arguments to the the given parser. """
     parser.add_argument('input',
-                        type=str,
-                        metavar='file',
+                        nargs='+',
+                        action=CollectFiles,
                         default=argparse.SUPPRESS,
-                        help="Code analyzer output result file which will be "
-                             "parsed and used to generate a CodeChecker "
-                             "report directory.")
+                        help="Code analyzer output result files or "
+                             "directories which will be parsed and used to "
+                             "generate a CodeChecker report directory.")
 
     parser.add_argument('-o', '--output',
                         dest="output_dir",
                         required=True,
                         default=argparse.SUPPRESS,
                         help="This directory will be used to generate "
                              "CodeChecker report directory files.")
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/__init__.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -288,29 +288,45 @@
         type: Optional[str] = None,
         analyzer_result_file_path: Optional[str] = None,
         source_line: Optional[str] = None,
         bug_path_events: Optional[List[BugPathEvent]] = None,
         bug_path_positions: Optional[List[BugPathPosition]] = None,
         notes: Optional[List[BugPathEvent]] = None,
         macro_expansions: Optional[List[MacroExpansion]] = None,
-        annotations: Optional[Dict[str, str]] = None
+        annotations: Optional[Dict[str, str]] = None,
+        static_message: Optional[str] = None
     ):
+        """
+        This constructor populates the members of the Report object.
+
+        static_message: hash.get_report_hash() function generates a hash value
+            based on this report object. The checker message is usually the
+            part of this hash. However, sometimes a checker message may contain
+            dynamically generated parts (e.g. sanitizers include some memory
+            addresses). This results changing hashes at every analysis
+            execution. In this case the report converter of that analyzer may
+            provide a more stable message which is used only for hash
+            generation.
+        """
         self.analyzer_result_file_path = analyzer_result_file_path
         self.file = file
         self.line = line
         self.column = column
         self.message = message
         self.checker_name = checker_name
         self.severity = severity
         self.report_hash = report_hash
         self.analyzer_name = analyzer_name
         self.category = category
         self.type = type
         self.annotations = annotations
 
+        self.static_message = \
+            message if static_message is None else static_message
+
         self.bug_path_events = bug_path_events \
             if bug_path_events is not None else \
             [BugPathEvent(self.message, self.file, self.line, self.column)]
 
         self.bug_path_positions = bug_path_positions \
             if bug_path_positions is not None else []
         self.notes = notes if notes is not None else []
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/checker_labels.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/checker_labels.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/hash.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 
 def __get_report_hash_path_sensitive(report: Report) -> List[str]:
     """ Report hash generation from the given report.
 
     High level overview of the hash content:
      * 'file_name' from the main diag section.
      * 'checker name'
-     * 'checker message'
+     * 'checker message' (Some analyzers may generate dynamic content to
+         messages, line memory addresses in case of sanitizers. The report
+         converter of these analyzers may exclude these dynamic parts.)
      * 'line content' from the source file if can be read up
      * 'column numbers' from the main diag section
      * 'range column numbers' from bug_path_positions.
     """
     try:
         event = report.bug_path_events[-1]
 
@@ -83,15 +85,15 @@
         if line_content == '' and \
                 not os.path.isfile(report.file.original_path):
             LOG.error("Failed to generate report hash. %s does not exists!",
                       report.file.original_path)
 
         hash_content = [report.file.name,
                         report.checker_name,
-                        event.message,
+                        report.static_message,
                         line_content,
                         str(from_col),
                         str(until_col)]
 
         for p in report.bug_path_positions:
             if p.range:
                 hash_content.append(str(p.range.start_col))
@@ -136,15 +138,15 @@
         if line_content == '' and \
                 not os.path.isfile(report.file.original_path):
             LOG.error("Failed to include soruce line in the report hash.")
             LOG.error('%s does not exists!', report.file.original_path)
 
         return [
             report.file.name,
-            report.message,
+            report.static_message,
             line_content,
             str(from_col),
             str(until_col)]
     except Exception as ex:
         LOG.error("Hash generation failed")
         LOG.error(ex)
         return []
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/baseline.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/baseline.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/codeclimate.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/codeclimate.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/gerrit.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/gerrit.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/cli.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/cli.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/html.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/html.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/bugview.css` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/bugview.css`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/icon.css` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/icon.css`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/style.css` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/css/style.css`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/index.html` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/index.html`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/browsersupport.js` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/browsersupport.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/buglist.js` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/buglist.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/bugviewer.js` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/js/bugviewer.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/layout.html` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/layout.html`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/statistics.html` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/statistics.html`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/clike.min.js` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/clike.min.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.LICENSE` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.LICENSE`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.css` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.js` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/html/static/vendor/codemirror/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/json.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/json.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/plaintext.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/output/plaintext.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/base.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/base.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/plist.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/parser/plist.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,23 @@
     """
     def __init__(self, dict_type=dict):
         # Since Python 3.9 plistlib._PlistParser.__init__ has changed:
         # https://github.com/python/cpython/commit/ce81a925ef
         # To be backward compatible with old interpreters we need to call this
         # function based on conditions:
         params = _PlistParser.__init__.__code__.co_varnames
+        # Before 3.9 interpreter. When a newer interpreter is used, pylint will
+        # complain that too many arguments are used to invoke __init__, but
+        # with newer interpreters, this is deadcode.
         if len(params) == 3 and "use_builtin_types" in params:
             # Before 3.9 interpreter.
+            # pylint: disable=E1121
             _PlistParser.__init__(self, True, dict_type)
         else:
+            # After 3.9 interpreter.
             _PlistParser.__init__(self, dict_type)  # pylint: disable=E1120
 
         self.event_handler = _LXMLPlistEventHandler()
         self.event_handler.start = self.handle_begin_element
         self.event_handler.end = self.handle_end_element
         self.event_handler.data = self.handle_data
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/report_file.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/report_file.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/reports.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/reports.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/statistics.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/report/statistics.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/source_code_comment_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/source_code_comment_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/twodim.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/twodim.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_report_converter/util.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_report_converter/util.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/authentication.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/authentication.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/config_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/config_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/mass_store_run.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/mass_store_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1319,18 +1319,23 @@
 
                         self.__report_server._set_run_data_for_curr_product(
                             inc_num_of_runs, run_history_time)
 
                         runtime = round(time.time() - start_time, 2)
                         zip_size_kb = round(zip_size / 1024)
 
+                        tag_desc = ""
+                        if self.__tag:
+                            tag_desc = f", under tag '{self.__tag}'"
+
                         LOG.info("'%s' stored results (%s KB "
-                                 "/decompressed/) to run '%s' (id: %d) in "
+                                 "/decompressed/) to run '%s' (id: %d) %s in "
                                  "%s seconds.", self.user_name,
-                                 zip_size_kb, self.__name, run_id, runtime)
+                                 zip_size_kb, self.__name, run_id, tag_desc,
+                                 runtime)
 
                         iso_start_time = datetime.fromtimestamp(
                             start_time).isoformat()
 
                         log_msg = f"{iso_start_time}, " +\
                                   f"{runtime}s, " +\
                                   f'"{self.__product.name}", ' +\
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/product_server.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/product_server.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/report_server.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/report_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3383,15 +3383,15 @@
         # time with a storage concurrently results foreign key constraint
         # error. An alternative solution can be adding a timestamp to file
         # entries to delay their removal. The same comment applies to
         # removeRunReports() function.
         db_cleanup.remove_unused_comments(self._Session)
         db_cleanup.remove_unused_analysis_info(self._Session)
 
-        return True
+        return bool(runs)
 
     @exc_to_thrift_reqfail
     @timeit
     def updateRunData(self, run_id, new_run_name):
         self.__require_store()
 
         if not new_run_name:
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/server_info_handler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/server_info_handler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/api/thrift_enum_helper.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/api/thrift_enum_helper.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_ldap.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_ldap.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_pam.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/auth/cc_pam.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/server.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/cmd/server.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/config_db_model.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/config_db_model.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/database.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/database.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/db_cleanup.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/db_cleanup.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/database/run_db_model.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/database/run_db_model.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/instance_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/instance_manager.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/metadata.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/metadata.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/env.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/env.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/126fa3f55e4b_added_permission_for_product_view.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/126fa3f55e4b_added_permission_for_product_view.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/150800b30447_share_sessions_through_the_database.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/150800b30447_share_sessions_through_the_database.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/302693c76eb8_remove_db_version_table.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/302693c76eb8_remove_db_version_table.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/3335ff7593cc_disable_review_status_change.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/3335ff7593cc_disable_review_status_change.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4964142b58d2_authentication_session_tokens.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4964142b58d2_authentication_session_tokens.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4db450cf38af_add_extra_product_detail_columns.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/4db450cf38af_add_extra_product_detail_columns.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/6b9f832d0b20_add_user_name_and_group_to_session.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/6b9f832d0b20_add_user_name_and_group_to_session.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/7829789fc19c_global_permission_to_get_access_controls.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/7829789fc19c_global_permission_to_get_access_controls.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/8268fc7ca7f4_initial_schema.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/8268fc7ca7f4_initial_schema.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/dec6feb991e6_new_table_for_server_config.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/config/versions/dec6feb991e6_new_table_for_server_config.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/env.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/env.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/080349e895d7_add_check_command_to_run_history.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/080349e895d7_add_check_command_to_run_history.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/101a9cb747de_add_bug_event_and_point_report_index.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/101a9cb747de_add_bug_event_and_point_report_index.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3793e361a752_source_components.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3793e361a752_source_components.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/39f9e96071c0_analyzer_statistics.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/39f9e96071c0_analyzer_statistics.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3e91d0612422_off_and_unavailable_detection_statuses.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/3e91d0612422_off_and_unavailable_detection_statuses.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/4b38fa14c27b_file_id_index_for_reports.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/4b38fa14c27b_file_id_index_for_reports.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/6cb6a3a41967_system_comments.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/6cb6a3a41967_system_comments.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/75ae226b5d88_review_status_for_each_report.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/75ae226b5d88_review_status_for_each_report.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/82ca43f05c10_initial_schema.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/82ca43f05c10_initial_schema.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9987aa593ca7_add_codechecker_version_to_run_history.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9987aa593ca7_add_codechecker_version_to_run_history.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9d956a0fae8d_report_annotations.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/9d956a0fae8d_report_annotations.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a24461972d2e_add_index_for_report_and_history_id_columns.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a24461972d2e_add_index_for_report_and_history_id_columns.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a79677f54e48_remove_db_version_table.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/a79677f54e48_remove_db_version_table.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/ad2a567e513a_git_blame_info.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/ad2a567e513a_git_blame_info.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/af5d8a21c1e4_add_analyzer_name_for_report.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/af5d8a21c1e4_add_analyzer_name_for_report.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/c042e02cca99_extended_report_data.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/c042e02cca99_extended_report_data.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dabc6998b8f0_analysis_info_table.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dabc6998b8f0_analysis_info_table.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dd9c97ead24_share_the_locking_of_runs.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/dd9c97ead24_share_the_locking_of_runs.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/e89887e7d3f0_add_bug_path_length.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/e89887e7d3f0_add_bug_path_length.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/f8291ab1d6be_fix_setting_analysis_info_id_seq.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/f8291ab1d6be_fix_setting_analysis_info_id_seq.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/fb356f0eefed_cleanup_plan.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/migrations/report/versions/fb356f0eefed_cleanup_plan.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/permissions.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/permissions.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/profiler.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/profiler.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/routing.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/routing.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/server.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/server.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/session_manager.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/session_manager.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_server/tmp.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_server/tmp.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/cli.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/cli.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/return_value.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/return_value.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/special_return_value.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/collectors/special_return_value.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/post_process_stats.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_statistics_collector/post_process_stats.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/web_version.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/cmd/web_version.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/convert.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/convert.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/database_status.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/database_status.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/env.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/env.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/host_check.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/host_check.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/pgpass.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/pgpass.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/version.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/version.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/codechecker_web/shared/webserver_context.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/codechecker_web/shared/webserver_context.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/lib/python3/tu_collector/tu_collector.py` & `codechecker-6.22.2/build_dist/CodeChecker/lib/python3/tu_collector/tu_collector.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/07c4c8ad1e67dd03142f8a3f10cf0c1d.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/07c4c8ad1e67dd03142f8a3f10cf0c1d.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/198.71b517a7d103c8182680.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/198.71b517a7d103c8182680.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/204.48d4cf3235458f4f48b8.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/324.780b5ed89944be295f22.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 (self.webpackChunkcodechecker = self.webpackChunkcodechecker || []).push([
-    [204], {
+    [324], {
         27468: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Nw: () => y,
                 QH: () => g.Z,
                 fZ: () => C
             }), n(24603), n(74916), n(39714), n(15306), n(69600), n(21249), n(23123), n(23157), n(92222);
             var r = n(99271),
-                a = n(85636);
-            const i = {
+                i = n(85636);
+            const a = {
                 name: "AnalysisInfoDialog",
                 props: {
                     value: {
                         type: Boolean,
                         default: !1
                     },
                     runId: {
@@ -75,15 +75,15 @@
                             return t.enabledCheckerRgx.test(e) ? n.push("enabled-checkers") : t.disabledCheckerRgx.test(e) ? n.push("disabled-checkers") : e.startsWith("--ctu") ? n.push("ctu") : e.startsWith("--stats") && n.push("statistics"), '<span class="'.concat(n.join(" "), '">').concat(e, "</span>")
                         })).join(" ").replace(/(?:\r\n|\r|\n)/g, "<br>")
                     },
                     getAnalysisInfo: function() {
                         var e = this;
                         if (this.dialog && (this.runId || this.runHistoryId || this.reportId)) {
                             this.analysisInfo = [];
-                            var t = new a.AnalysisInfoFilter({
+                            var t = new i.AnalysisInfoFilter({
                                 runId: this.runId,
                                 runHistoryId: this.runHistoryId,
                                 reportId: this.reportId
                             });
                             r.mv.getClient().getAnalysisInfo(t, null, 0, (0, r.nC)((function(t) {
                                 e.analysisInfo = t.map((function(t) {
                                     return e.highlightOptions(t)
@@ -100,15 +100,15 @@
                 c = n(11880),
                 u = n(74811),
                 d = n(53544),
                 p = n(19846),
                 f = n(95026),
                 v = n(13047),
                 m = n(16151),
-                h = (0, s.Z)(i, (function() {
+                h = (0, s.Z)(a, (function() {
                     var e = this,
                         t = e.$createElement,
                         n = e._self._c || t;
                     return n("v-dialog", {
                         attrs: {
                             "content-class": "analysis-info",
                             "max-width": "80%",
@@ -225,36 +225,36 @@
                 VBtn: c.Z,
                 VIcon: v.Z,
                 VTooltip: _.Z
             })
         },
         23281: (e, t, n) => {
             var r = n(8081),
-                a = n(23645)(r);
-            a.push([e.id, "[data-v-7d68540e] .analysis-info{border:1px solid gray;padding:4px}[data-v-7d68540e] .analysis-info .param{background-color:rgba(0,0,0,.15);font-weight:bold;padding-left:2px;padding-right:2px}[data-v-7d68540e] .analysis-info .enabled-checkers{background-color:rgba(0,142,0,.15)}[data-v-7d68540e] .analysis-info .disabled-checkers{background-color:rgba(142,0,0,.15)}[data-v-7d68540e] .analysis-info .ctu,[data-v-7d68540e] .analysis-info .statistics{background-color:rgba(0,0,142,.15)}", ""]), e.exports = a
+                i = n(23645)(r);
+            i.push([e.id, "[data-v-7d68540e] .analysis-info{border:1px solid gray;padding:4px}[data-v-7d68540e] .analysis-info .param{background-color:rgba(0,0,0,.15);font-weight:bold;padding-left:2px;padding-right:2px}[data-v-7d68540e] .analysis-info .enabled-checkers{background-color:rgba(0,142,0,.15)}[data-v-7d68540e] .analysis-info .disabled-checkers{background-color:rgba(142,0,0,.15)}[data-v-7d68540e] .analysis-info .ctu,[data-v-7d68540e] .analysis-info .statistics{background-color:rgba(0,0,142,.15)}", ""]), e.exports = i
         },
         85537: (e, t, n) => {
             var r = n(8081),
-                a = n(23645)(r);
-            a.push([e.id, ".analyzer-statistics{cursor:pointer}.analyzer-statistics:hover{color:var(--v-primary-base)}", ""]), e.exports = a
+                i = n(23645)(r);
+            i.push([e.id, ".analyzer-statistics{cursor:pointer}.analyzer-statistics:hover{color:var(--v-primary-base)}", ""]), e.exports = i
         },
         65814: (e, t, n) => {
             var r = n(8081),
-                a = n(23645)(r);
-            a.push([e.id, ".v-timeline-item.run-history[data-v-281491aa]:hover{background-color:#eee}", ""]), e.exports = a
+                i = n(23645)(r);
+            i.push([e.id, ".v-timeline-item.run-history[data-v-281491aa]:hover{background-color:#eee}", ""]), e.exports = i
         },
         87156: (e, t, n) => {
             var r = n(8081),
-                a = n(23645)(r);
-            a.push([e.id, ".v-list-item__title[data-v-13defd5c]{white-space:normal}", ""]), e.exports = a
+                i = n(23645)(r);
+            i.push([e.id, ".v-list-item__title[data-v-13defd5c]{white-space:normal}", ""]), e.exports = i
         },
         13720: (e, t, n) => {
             var r = n(8081),
-                a = n(23645)(r);
-            a.push([e.id, ".v-data-table[data-v-f6aa84de]  tbody tr.v-data-table__expanded__content{box-shadow:none}", ""]), e.exports = a
+                i = n(23645)(r);
+            i.push([e.id, ".v-data-table[data-v-f6aa84de]  tbody tr.v-data-table__expanded__content{box-shadow:none}", ""]), e.exports = i
         },
         93546: (e, t, n) => {
             var r = n(23281);
             r.__esModule && (r = r.default), "string" == typeof r && (r = [
                 [e.id, r, ""]
             ]), r.locals && (e.exports = r.locals), (0, n(45346).Z)("b54e9714", r, !0, {})
         },
@@ -278,22 +278,22 @@
         },
         88676: (e, t, n) => {
             var r = n(13720);
             r.__esModule && (r = r.default), "string" == typeof r && (r = [
                 [e.id, r, ""]
             ]), r.locals && (e.exports = r.locals), (0, n(45346).Z)("6fb826ae", r, !0, {})
         },
-        17204: (e, t, n) => {
+        60324: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 default: () => je
             }), n(35666), n(91058), n(66992), n(41539), n(88674), n(78783), n(33948), n(21249), n(69720), n(69826), n(74916), n(15306), n(85827), n(23123), n(68309), n(69070), n(47941), n(82526), n(57327), n(38880), n(89554), n(54747), n(49337), n(33321), n(79753), n(41817), n(32165), n(47042), n(91038);
             var r = n(20629),
-                a = n(99271),
-                i = n(85636),
+                i = n(99271),
+                a = n(85636),
                 s = n(27468);
             var o = n(51900),
                 l = n(43453),
                 c = n.n(l),
                 u = n(11880),
                 d = n(13047),
                 p = (0, o.Z)({
@@ -449,15 +449,15 @@
                 },
                 mounted: function() {
                     this.getAnalysisStatistics()
                 },
                 methods: {
                     getAnalysisStatistics: function() {
                         var e = this;
-                        (this.dialog || this.runId || this.runHistoryId) && a.mv.getClient().getAnalysisStatistics(this.runId, this.runHistoryId, (0, a.nC)((function(t) {
+                        (this.dialog || this.runId || this.runHistoryId) && i.mv.getClient().getAnalysisStatistics(this.runId, this.runHistoryId, (0, i.nC)((function(t) {
                             var n;
                             e.analyzerStatistics = t, e.activeExpansionPanels = function(e) {
                                 if (Array.isArray(e)) return b(e)
                             }(n = Array(Object.keys(t).length).keys()) || function(e) {
                                 if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                             }(n) || function(e, t) {
                                 if (e) {
@@ -470,16 +470,16 @@
                             }()
                         })))
                     }
                 }
             };
             var x = n(74811),
                 C = n(53544),
-                k = n(8857),
-                w = n(19846),
+                w = n(8857),
+                k = n(19846),
                 I = n(95026),
                 R = n(53631),
                 S = n(86416),
                 T = n(66113),
                 V = n(28814),
                 O = n(90798),
                 Z = n(16151),
@@ -589,16 +589,16 @@
             const D = A.exports;
             c()(A, {
                 VBtn: u.Z,
                 VCard: x.Z,
                 VCardActions: C.h7,
                 VCardText: C.ZB,
                 VCardTitle: C.EB,
-                VChip: k.Z,
-                VContainer: w.Z,
+                VChip: w.Z,
+                VContainer: k.Z,
                 VDialog: I.Z,
                 VDivider: h.Z,
                 VExpansionPanel: R.Z,
                 VExpansionPanelContent: S.Z,
                 VExpansionPanelHeader: T.Z,
                 VExpansionPanels: V.Z,
                 VIcon: d.Z,
@@ -622,20 +622,20 @@
                         removingInProgress: !1
                     }
                 },
                 methods: {
                     confirmDelete: function() {
                         var e = this;
                         this.removingInProgress = !0;
-                        var t = new i.RunFilter({
+                        var t = new a.RunFilter({
                             ids: this.selected.map((function(e) {
                                 return e.runId
                             }))
                         });
-                        a.mv.getClient().removeRun(null, t, (0, a.nC)((function() {
+                        i.mv.getClient().removeRun(null, t, (0, i.nC)((function() {
                             e.selected.splice(0, e.selected.length), e.dialog = !1, e.$emit("on-confirm"), e.removingInProgres = !1
                         })))
                     }
                 }
             };
             var $ = (0, o.Z)(P, (function() {
                 var e = this,
@@ -700,15 +700,15 @@
                         expression: "dialog"
                     }
                 })
             }), [], !1, null, null, null);
             const j = $.exports;
             c()($, {
                 VBtn: u.Z,
-                VChip: k.Z,
+                VChip: w.Z,
                 VIcon: d.Z
             }), n(83710);
             var B = n(56514),
                 E = n(61532),
                 z = n(42080),
                 H = n(93505);
             const q = {
@@ -783,15 +783,15 @@
                     }, [e._v("\n      mdi-tag-outline\n    ")])], 1), e._v(" "), n("span", {
                         staticClass: "grey--text text--darken-3"
                     }, [e._v("\n    " + e._s(e.value) + "\n  ")])], 1)
                 }), [], !1, null, null, null);
             const W = Q.exports;
             c()(Q, {
                 VAvatar: L.Z,
-                VChip: k.Z,
+                VChip: w.Z,
                 VIcon: d.Z
             });
             const J = {
                 name: "ExpandedRun",
                 components: {
                     AnalysisInfoBtn: f,
                     AnalyzerStatisticsBtn: g,
@@ -1030,39 +1030,39 @@
                         }
                     }, [n("v-icon", [e._v("mdi-alert-circle-outline")]), e._v(" "), n("strong", [e._v("No history events matched your search.")])], 1)
                 }), [], !1, null, "281491aa", null);
             const re = ne.exports;
             c()(ne, {
                 VCard: x.Z,
                 VCheckbox: Y.Z,
-                VChip: k.Z,
+                VChip: w.Z,
                 VCol: G.Z,
-                VContainer: w.Z,
+                VContainer: k.Z,
                 VDivider: h.Z,
                 VIcon: d.Z,
                 VListItem: K.Z,
                 VListItemContent: X.km,
                 VListItemSubtitle: X.oZ,
                 VListItemTitle: X.V9,
                 VRow: O.Z,
                 VSpacer: Z.Z,
                 VTimeline: ee.Z,
                 VTimelineItem: te.Z
             });
-            const ae = {
+            const ie = {
                 name: "RunDescription",
                 props: {
                     value: {
                         type: String,
                         required: !0
                     }
                 }
             };
-            var ie = n(92599),
-                se = (0, o.Z)(ae, (function() {
+            var ae = n(92599),
+                se = (0, o.Z)(ie, (function() {
                     var e = this,
                         t = e.$createElement,
                         n = e._self._c || t;
                     return n("v-menu", {
                         attrs: {
                             "content-class": "run-description-menu",
                             "close-on-content-click": !1,
@@ -1105,15 +1105,15 @@
                 }) : e[t] = n, e
             }
             c()(se, {
                 VCard: x.Z,
                 VCardText: C.ZB,
                 VCardTitle: C.EB,
                 VIcon: d.Z,
-                VMenu: ie.Z
+                VMenu: ae.Z
             });
             const ue = {
                 name: "RunNameColumn",
                 components: {
                     DetectionStatusIcon: v._8,
                     RunDescription: oe,
                     AnalysisInfoBtn: f,
@@ -1381,16 +1381,16 @@
                     },
                     update: function() {
                         this.$emit("update")
                     }
                 })
             };
             var Ce = n(14462),
-                ke = n(36807),
-                we = (0, o.Z)(xe, (function() {
+                we = n(36807),
+                ke = (0, o.Z)(xe, (function() {
                     var e = this,
                         t = e.$createElement,
                         n = e._self._c || t;
                     return n("v-toolbar", {
                         staticClass: "run-filter-toolbar mb-4",
                         attrs: {
                             flat: ""
@@ -1512,27 +1512,27 @@
                             to: e.diffTargetRoute,
                             disabled: e.isDiffBtnDisabled
                         }
                     }, [n("v-icon", {
                         attrs: {
                             left: ""
                         }
-                    }, [e._v("\n          mdi-select-compare\n        ")]), e._v("\n        Diff\n      ")], 1), e._v(" "), n("v-btn", {
+                    }, [e._v("\n          mdi-select-compare\n        ")]), e._v("\n        Diff\n        "), n("tooltip-help-icon", [e._v("\n          Compare the set of "), n("i", [e._v("outstanding reports")]), e._v(" in two run (or tag)\n          sets."), n("br"), e._v("\n          A report is outstanding if "), n("b", [e._v(" all of the following is true")]), e._v(":\n          "), n("ul", [n("li", [e._v("\n              its detection status is "), n("i", [e._v("new")]), e._v(", "), n("i", [e._v("reopened")]), e._v(", or\n              "), n("i", [e._v("unresolved")]), e._v(",\n            ")]), e._v(" "), n("li", [e._v("\n              its review status is "), n("i", [e._v("unreviewed")]), e._v(" or "), n("i", [e._v("confirmed")]), e._v(".\n            ")])])])], 1), e._v(" "), n("v-btn", {
                         staticClass: "reload-runs-btn",
                         attrs: {
                             icon: "",
                             title: "Reload runs",
                             color: "primary"
                         },
                         on: {
                             click: e.update
                         }
                     }, [n("v-icon", [e._v("mdi-refresh")])], 1)], 1)], 1)], 1)
                 }), [], !1, null, null, null);
-            const Ie = we.exports;
+            const Ie = ke.exports;
 
             function Re(e, t) {
                 if (e) {
                     if ("string" == typeof e) return Se(e, t);
                     var n = Object.prototype.toString.call(e).slice(8, -1);
                     return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Se(e, t) : void 0
                 }
@@ -1540,37 +1540,37 @@
 
             function Se(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                 return r
             }
 
-            function Te(e, t, n, r, a, i, s) {
+            function Te(e, t, n, r, i, a, s) {
                 try {
-                    var o = e[i](s),
+                    var o = e[a](s),
                         l = o.value
                 } catch (e) {
                     return void n(e)
                 }
-                o.done ? t(l) : Promise.resolve(l).then(r, a)
+                o.done ? t(l) : Promise.resolve(l).then(r, i)
             }
 
             function Ve(e) {
                 return function() {
                     var t = this,
                         n = arguments;
-                    return new Promise((function(r, a) {
-                        var i = e.apply(t, n);
+                    return new Promise((function(r, i) {
+                        var a = e.apply(t, n);
 
                         function s(e) {
-                            Te(i, r, a, s, o, "next", e)
+                            Te(a, r, i, s, o, "next", e)
                         }
 
                         function o(e) {
-                            Te(i, r, a, s, o, "throw", e)
+                            Te(a, r, i, s, o, "throw", e)
                         }
                         s(void 0)
                     }))
                 }
             }
 
             function Oe(e, t) {
@@ -1600,22 +1600,22 @@
                 return t in e ? Object.defineProperty(e, t, {
                     value: n,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = n, e
             }
-            c()(we, {
+            c()(ke, {
                 VBtn: u.Z,
                 VCol: G.Z,
                 VIcon: d.Z,
                 VRow: O.Z,
                 VSpacer: Z.Z,
                 VTextField: Ce.Z,
-                VToolbar: ke.Z
+                VToolbar: we.Z
             });
             const De = {
                 name: "RunList",
                 components: {
                     AnalyzerStatisticsBtn: g,
                     AnalyzerStatisticsDialog: D,
                     AnalysisInfoDialog: s.Nw,
@@ -1624,23 +1624,23 @@
                     RunFilterToolbar: Ie
                 },
                 data: function() {
                     var e = [25, 50, 100],
                         t = parseInt(this.$router.currentRoute.query.page) || 1,
                         n = parseInt(this.$router.currentRoute.query["items-per-page"]) || e[0],
                         r = this.$router.currentRoute.query["sort-by"],
-                        a = this.$router.currentRoute.query["sort-desc"];
+                        i = this.$router.currentRoute.query["sort-desc"];
                     return {
                         initialized: !1,
                         analysisInfoDialog: !1,
                         pagination: {
                             page: t,
                             itemsPerPage: n,
                             sortBy: r ? [r] : [],
-                            sortDesc: void 0 !== a ? ["true" === a] : []
+                            sortDesc: void 0 !== i ? ["true" === i] : []
                         },
                         footerProps: {
                             itemsPerPageOptions: e
                         },
                         totalItems: 0,
                         loading: !1,
                         selected: [],
@@ -1699,20 +1699,20 @@
                     pagination: {
                         handler: function() {
                             if (this.initialized) {
                                 var e = this.footerProps.itemsPerPageOptions[0],
                                     t = this.pagination.itemsPerPage === e ? void 0 : this.pagination.itemsPerPage,
                                     n = 1 === this.pagination.page ? void 0 : this.pagination.page,
                                     r = this.pagination.sortBy.length ? this.pagination.sortBy[0] : void 0,
-                                    a = this.pagination.sortDesc.length ? this.pagination.sortDesc[0] : void 0;
+                                    i = this.pagination.sortDesc.length ? this.pagination.sortDesc[0] : void 0;
                                 this.updateUrl({
                                     "items-per-page": t,
                                     page: n,
                                     "sort-by": r,
-                                    "sort-desc": a
+                                    "sort-desc": i
                                 }), this.fetchRuns()
                             }
                         },
                         deep: !0
                     }
                 },
                 mounted: function() {
@@ -1741,19 +1741,19 @@
                         var e = this;
                         return Ve(regeneratorRuntime.mark((function t() {
                             return regeneratorRuntime.wrap((function(t) {
                                 for (;;) switch (t.prev = t.next) {
                                     case 0:
                                         return e.loading = !0, t.next = 3, Promise.all(e.expanded.map(function() {
                                             var t = Ve(regeneratorRuntime.mark((function t(n) {
-                                                var r, a, i, s, o, l;
+                                                var r, i, a, s, o, l;
                                                 return regeneratorRuntime.wrap((function(t) {
                                                     for (;;) switch (t.prev = t.next) {
                                                         case 0:
-                                                            return r = n.$history, a = r.limit, i = r.offset, t.next = 3, e.getRunHistory(n.runId, a + i);
+                                                            return r = n.$history, i = r.limit, a = r.offset, t.next = 3, e.getRunHistory(n.runId, i + a);
                                                         case 3:
                                                             s = t.sent, o = s.histories, l = s.hasMore, n.$history.hasMore = l, n.$history.values = o;
                                                         case 8:
                                                         case "end":
                                                             return t.stop()
                                                     }
                                                 }), t)
@@ -1770,53 +1770,53 @@
                                 }
                             }), t)
                         })))()
                     },
                     initExpandedItems: function() {
                         var e = this;
                         return Ve(regeneratorRuntime.mark((function t() {
-                            var n, r, a, i, s;
+                            var n, r, i, a, s;
                             return regeneratorRuntime.wrap((function(t) {
                                 for (;;) switch (t.prev = t.next) {
                                     case 0:
                                         if (n = e.$router.currentRoute.query.expanded) {
                                             t.next = 3;
                                             break
                                         }
                                         return t.abrupt("return");
                                     case 3:
-                                        r = JSON.parse(n), a = regeneratorRuntime.mark((function t() {
-                                            var n, r, a, o, l, c, u, d, p, f;
+                                        r = JSON.parse(n), i = regeneratorRuntime.mark((function t() {
+                                            var n, r, i, o, l, c, u, d, p, f;
                                             return regeneratorRuntime.wrap((function(t) {
                                                 for (;;) switch (t.prev = t.next) {
                                                     case 0:
-                                                        return v = s[i], m = 2, n = function(e) {
+                                                        return v = s[a], m = 2, n = function(e) {
                                                             if (Array.isArray(e)) return e
                                                         }(v) || function(e, t) {
                                                             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                                                             if (null != n) {
-                                                                var r, a, i = [],
+                                                                var r, i, a = [],
                                                                     s = !0,
                                                                     o = !1;
                                                                 try {
-                                                                    for (n = n.call(e); !(s = (r = n.next()).done) && (i.push(r.value), !t || i.length !== t); s = !0);
+                                                                    for (n = n.call(e); !(s = (r = n.next()).done) && (a.push(r.value), !t || a.length !== t); s = !0);
                                                                 } catch (e) {
-                                                                    o = !0, a = e
+                                                                    o = !0, i = e
                                                                 } finally {
                                                                     try {
                                                                         s || null == n.return || n.return()
                                                                     } finally {
-                                                                        if (o) throw a
+                                                                        if (o) throw i
                                                                     }
                                                                 }
-                                                                return i
+                                                                return a
                                                             }
                                                         }(v, m) || Re(v, m) || function() {
                                                             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                                                        }(), r = n[0], a = n[1], o = a.limit, l = a.offset, c = +r, u = e.runs.find((function(e) {
+                                                        }(), r = n[0], i = n[1], o = i.limit, l = i.offset, c = +r, u = e.runs.find((function(e) {
                                                             return e.runId.toNumber() === c
                                                         })), t.next = 7, e.getRunHistory(c, o + l, 0);
                                                     case 7:
                                                         d = t.sent, p = d.histories, f = d.hasMore, u.$history = {
                                                             limit: o,
                                                             offset: l,
                                                             hasMore: f,
@@ -1824,23 +1824,23 @@
                                                         }, e.expanded.push(u);
                                                     case 12:
                                                     case "end":
                                                         return t.stop()
                                                 }
                                                 var v, m
                                             }), t)
-                                        })), i = 0, s = Object.entries(r);
+                                        })), a = 0, s = Object.entries(r);
                                     case 6:
-                                        if (!(i < s.length)) {
+                                        if (!(a < s.length)) {
                                             t.next = 11;
                                             break
                                         }
-                                        return t.delegateYield(a(), "t0", 8);
+                                        return t.delegateYield(i(), "t0", 8);
                                     case 8:
-                                        i++, t.next = 6;
+                                        a++, t.next = 6;
                                         break;
                                     case 11:
                                     case "end":
                                         return t.stop()
                                 }
                             }), t)
                         })))()
@@ -1860,19 +1860,19 @@
                         this.updateUrl({
                             expanded: this.expanded.length ? JSON.stringify(e) : void 0
                         })
                     },
                     loadMoreRunHistory: function(e) {
                         var t = this;
                         return Ve(regeneratorRuntime.mark((function n() {
-                            var r, a, i, s, o, l;
+                            var r, i, a, s, o, l;
                             return regeneratorRuntime.wrap((function(n) {
                                 for (;;) switch (n.prev = n.next) {
                                     case 0:
-                                        return t.loadingMoreRunHistories = !0, a = e.$history.limit, i = e.$history.offset + a, e.$history.offset = i, n.next = 6, t.getRunHistory(e.runId, a, i);
+                                        return t.loadingMoreRunHistories = !0, i = e.$history.limit, a = e.$history.offset + i, e.$history.offset = a, n.next = 6, t.getRunHistory(e.runId, i, a);
                                     case 6:
                                         s = n.sent, o = s.histories, l = s.hasMore, e.$history.hasMore = l, (r = e.$history.values).push.apply(r, function(e) {
                                             if (Array.isArray(e)) return Se(e)
                                         }(c = o) || function(e) {
                                             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                                         }(c) || Re(c) || function() {
                                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
@@ -1885,101 +1885,101 @@
                             }), n)
                         })))()
                     },
                     runExpanded: function(e) {
                         var t = arguments,
                             n = this;
                         return Ve(regeneratorRuntime.mark((function r() {
-                            var a, i, s, o, l;
+                            var i, a, s, o, l;
                             return regeneratorRuntime.wrap((function(r) {
                                 for (;;) switch (r.prev = r.next) {
                                     case 0:
-                                        if (a = t.length > 1 && void 0 !== t[1] ? t[1] : 10, i = t.length > 2 && void 0 !== t[2] ? t[2] : 0, !e.item.$history) {
+                                        if (i = t.length > 1 && void 0 !== t[1] ? t[1] : 10, a = t.length > 2 && void 0 !== t[2] ? t[2] : 0, !e.item.$history) {
                                             r.next = 4;
                                             break
                                         }
                                         return r.abrupt("return", n.$nextTick(n.updateExpandedUrlParam));
                                     case 4:
-                                        return n.loading = !0, r.next = 7, n.getRunHistory(e.item.runId, a, i);
+                                        return n.loading = !0, r.next = 7, n.getRunHistory(e.item.runId, i, a);
                                     case 7:
                                         s = r.sent, o = s.histories, l = s.hasMore, e.item.$history = {
-                                            limit: a,
-                                            offset: i,
+                                            limit: i,
+                                            offset: a,
                                             hasMore: l,
                                             values: o
                                         }, n.updateExpandedUrlParam(), n.loading = !1;
                                     case 13:
                                     case "end":
                                         return r.stop()
                                 }
                             }), r)
                         })))()
                     },
                     getRunHistory: function(e) {
                         var t = this,
                             n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 10,
                             r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
-                        return new Promise((function(i) {
-                            a.mv.getClient().getRunHistory([e], n, r, t.runHistoryFilter, (0, a.nC)((function(e) {
-                                i({
+                        return new Promise((function(a) {
+                            i.mv.getClient().getRunHistory([e], n, r, t.runHistoryFilter, (0, i.nC)((function(e) {
+                                a({
                                     hasMore: e.length === n,
                                     histories: e.map((function(e) {
                                         return Ze(Ze({}, e), {}, {
                                             $codeCheckerVersion: t.prettifyCCVersion(e.codeCheckerVersion)
                                         })
                                     }))
                                 })
                             })))
                         }))
                     },
                     getSortMode: function() {
                         var e = null;
                         switch (this.pagination.sortBy[0]) {
                             case "name":
-                                e = i.RunSortType.NAME;
+                                e = a.RunSortType.NAME;
                                 break;
                             case "resultCount":
-                                e = i.RunSortType.UNRESOLVED_REPORTS;
+                                e = a.RunSortType.UNRESOLVED_REPORTS;
                                 break;
                             case "duration":
-                                e = i.RunSortType.DURATION;
+                                e = a.RunSortType.DURATION;
                                 break;
                             case "codeCheckerVersion":
-                                e = i.RunSortType.CC_VERSION;
+                                e = a.RunSortType.CC_VERSION;
                                 break;
                             default:
-                                e = i.RunSortType.DATE
+                                e = a.RunSortType.DATE
                         }
-                        var t = !1 === this.pagination.sortDesc[0] ? i.Order.ASC : i.Order.DESC;
-                        return new i.RunSortMode({
+                        var t = !1 === this.pagination.sortDesc[0] ? a.Order.ASC : a.Order.DESC;
+                        return new a.RunSortMode({
                             type: e,
                             ord: t
                         })
                     },
                     fetchRuns: function() {
                         var e = this;
-                        this.loading = !0, a.mv.getClient().getRunCount(this.runFilter, (0, a.nC)((function(t) {
+                        this.loading = !0, i.mv.getClient().getRunCount(this.runFilter, (0, i.nC)((function(t) {
                             e.totalItems = t.toNumber()
                         })));
                         var t = this.pagination.itemsPerPage,
                             n = t * (this.pagination.page - 1),
                             r = this.getSortMode();
-                        return new Promise((function(i) {
-                            a.mv.getClient().getRunData(e.runFilter, t, n, r, (0, a.nC)((function(t) {
+                        return new Promise((function(a) {
+                            i.mv.getClient().getRunData(e.runFilter, t, n, r, (0, i.nC)((function(t) {
                                 e.runs = t.map((function(t) {
                                     var n = e.prettifyCCVersion(t.codeCheckerVersion),
                                         r = e.expanded.find((function(e) {
                                             return e.runId.toNumber() === t.runId.toNumber()
                                         }));
                                     return Ze(Ze({}, t), {}, {
                                         $history: r ? r.$history : null,
                                         $duration: e.prettifyDuration(t.duration),
                                         $codeCheckerVersion: n
                                     })
-                                })), e.loading = !1, i(e.runs)
+                                })), e.loading = !1, a(e.runs)
                             })))
                         }))
                     },
                     openAnalysisInfoDialog: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                         this.selectedRunId = e, this.selectedRunHistoryId = t, this.analysisInfoDialog = !0
                     },
@@ -2263,16 +2263,16 @@
                     })], 1)
                 }), [], !1, null, "f6aa84de", null);
             const je = $e.exports;
             c()($e, {
                 VBtn: u.Z,
                 VCard: x.Z,
                 VCheckbox: Y.Z,
-                VChip: k.Z,
-                VContainer: w.Z,
+                VChip: w.Z,
+                VContainer: k.Z,
                 VDataTable: Pe.Z,
                 VIcon: d.Z,
                 VRow: O.Z
             })
         }
     }
 ]);
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/257.2fb64e335d3132937e67.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/257.2fb64e335d3132937e67.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/287.0bc0c02a80fc6fec452e.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/287.0bc0c02a80fc6fec452e.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/2d39422cd3aa08e2c9d27844e52cf651.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/2d39422cd3aa08e2c9d27844e52cf651.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/3408d5e44bc83a8a65abfaab3db59b34.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/3408d5e44bc83a8a65abfaab3db59b34.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/343.e2548aa08e829c446317.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/343.e2548aa08e829c446317.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/437c4ff8b03d221ca7112e93dd271271.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/437c4ff8b03d221ca7112e93dd271271.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/452.49b8e5bc5792d6509d2d.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/950.87a139d7b44cf5913f38.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 (self.webpackChunkcodechecker = self.webpackChunkcodechecker || []).push([
-    [452], {
+    [950], {
         20313: (e, t, n) => {
             e.exports = n.p + "8b0b574430b7d19d0afcaf576a964c21.png"
         },
         35999: (e, t, n) => {
             e.exports = n.p + "2d39422cd3aa08e2c9d27844e52cf651.png"
         },
         74945: (e, t, n) => {
@@ -35,18 +35,18 @@
         },
         8976: (e, t, n) => {
             e.exports = n.p + "07c4c8ad1e67dd03142f8a3f10cf0c1d.png"
         },
         61413: (e, t, n) => {
             e.exports = n.p + "5857a166c7017a15b8caedeed9b85c88.png"
         },
-        19452: (e, t, n) => {
+        7950: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
-                default: () => b
+                default: () => y
             });
             const o = {
                 name: "NewFeatureItem",
                 props: {
                     color: {
                         type: String,
                         default: null
@@ -127,29 +127,56 @@
                     }
                 };
             var p = n(66897),
                 _ = n(55136),
                 f = n(90798),
                 m = n(13751),
                 g = n(17069),
-                y = (0, r.Z)(v, (function() {
+                b = (0, r.Z)(v, (function() {
                     var e = this,
                         t = e.$createElement,
                         o = e._self._c || t;
                     return o("v-container", {
                         attrs: {
                             fluid: ""
                         }
                     }, [o("v-timeline", {
                         attrs: {
                             "align-top": ""
                         }
                     }, [o("v-timeline-item", {
                         attrs: {
                             "fill-dot": "",
+                            icon: "mdi-star"
+                        }
+                    }, [o("new-release-item", {
+                        scopedSlots: e._u([{
+                            key: "title",
+                            fn: function() {
+                                return [o("a", {
+                                    staticClass: "white--text",
+                                    attrs: {
+                                        href: "https://github.com/Ericsson/codechecker/releases/tag/v6.22.2",
+                                        target: "_blank"
+                                    }
+                                }, [e._v("\n              Highlights of CodeChecker 6.22.2 release\n            ")])]
+                            },
+                            proxy: !0
+                        }])
+                    }, [e._v(" "), o("new-feature-item", {
+                        scopedSlots: e._u([{
+                            key: "title",
+                            fn: function() {
+                                return [e._v("\n              Support for Ubuntu 22.04\n            ")]
+                            },
+                            proxy: !0
+                        }])
+                    }, [e._v("\n            CodeChecker failed to build on Ubuntu 22.04 in its previous release\n            because of two issues: some of our dependencies broke with the\n            release of python3.9, and we didn't support GNU Make-s new way of\n            creating build jobs. These issues are all fixed now, so CodeChecker\n            should work with the latest version of python and GNU Make!\n          ")])], 1)], 1), e._v(" "), o("v-timeline-item", {
+                        attrs: {
+                            "fill-dot": "",
                             icon: "mdi-star",
                             color: "green lighten-1"
                         }
                     }, [o("new-release-item", {
                         attrs: {
                             color: "green lighten-1"
                         },
@@ -1517,16 +1544,16 @@
                             fn: function() {
                                 return [e._v("\n              Consistent report counting\n            ")]
                             },
                             proxy: !0
                         }])
                     }, [e._v(" "), o("ul", [o("li", [e._v("\n                Uniqueing is disabled at bug list view by default.\n              ")]), e._v(" "), o("li", [e._v("\n                Numbers on the Run page (Number of unresolved reports,\n                Detection status) are counted without uniqueing.\n              ")]), e._v(" "), o("li", [e._v("\n                Set default filter set to the following values:\n                "), o("ul", [o("li", [e._v("\n                    Review status: "), o("b", [e._v("Unreviewed")]), e._v(", "), o("b", [e._v("Confirmed")])]), e._v(" "), o("li", [e._v("\n                    Detection status: "), o("b", [e._v("New")]), e._v(", "), o("b", [e._v("Reopened")]), e._v(", "), o("b", [e._v("Unresolved")])])])])])])], 1)], 1)], 1)], 1)
                 }), [], !1, null, null, null);
-            const b = y.exports;
-            a()(y, {
+            const y = b.exports;
+            a()(b, {
                 VAlert: p.Z,
                 VCol: _.Z,
                 VContainer: l.Z,
                 VRow: f.Z,
                 VTimeline: m.Z,
                 VTimelineItem: g.Z
             })
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/455.0a5796cf6fe665353148.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/455.f9ee007c1bcfd28541ae.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -345,15 +345,15 @@
                                         bgColor: e.bgColor,
                                         icon: p.DEFAULT
                                     };
 
                                 function o(e) {
                                     if (r.startsWith(e)) return r = r.replace(e, "").replace(/'/g, ""), !0
                                 }
-                                return o("Calling ") ? (e.funcStack.push(r), e.bgColor = b[e.funcStack.length % b.length], n.icon = p.CALLING) : r.startsWith("Entered call from ") ? n.icon = p.ENTERED_CALL : o("Returning from ") ? r === e.funcStack[e.funcStack.length - 1] ? (e.funcStack.pop(), e.bgColor = b[e.funcStack.length % b.length], n.icon = p.RETURNING) : console.warn("StackError: Returned from " + r + " while the last function was " + e.funcStack[e.funcStack.length - 1]) : "Returned allocated memory" === r ? (e.funcStack.pop(), e.bgColor = b[e.funcStack.length % b], n.icon = p.RETURNING) : r.startsWith("Assuming the condition") ? n.icon = p.ASSUMING_CONDITION : r.startsWith("Assuming") ? n.icon = p.ASSUMING : "Entering loop body" == r ? n.icon = p.ENTERING_LOOP_BODY : r.startsWith("Loop body executed") ? n.icon = p.LOOP_BODY_EXECUTED : "Looping back to the head of the loop" == r && (n.icon = p.LOOP_BACK), n
+                                return o("Calling ") ? (e.funcStack.push(r), e.bgColor = b[e.funcStack.length % b.length], n.icon = p.CALLING) : r.startsWith("Entered call from ") ? n.icon = p.ENTERED_CALL : o("Returning from ") ? r === e.funcStack[e.funcStack.length - 1] ? (e.funcStack.pop(), e.bgColor = b[e.funcStack.length % b.length], n.icon = p.RETURNING) : console.warn("StackError: Returned from " + r + " while the last function was " + e.funcStack[e.funcStack.length - 1]) : "Returned allocated memory" === r || r.startsWith("Returning;") ? (e.funcStack.pop(), e.bgColor = b[e.funcStack.length % b], n.icon = p.RETURNING) : r.startsWith("Assuming the condition") ? n.icon = p.ASSUMING_CONDITION : r.startsWith("Assuming") ? n.icon = p.ASSUMING : "Entering loop body" == r ? n.icon = p.ENTERING_LOOP_BODY : r.startsWith("Loop body executed") ? n.icon = p.LOOP_BODY_EXECUTED : "Looping back to the head of the loop" == r && (n.icon = p.LOOP_BACK), n
                             }(n, o),
                             E = function(e, t, r) {
                                 return {
                                     index: t + 1,
                                     type: r ? "error" : e.msg.indexOf(" (fixit)") > -1 ? "fixit" : "info"
                                 }
                             }(o, s, c);
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/5857a166c7017a15b8caedeed9b85c88.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/5857a166c7017a15b8caedeed9b85c88.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/608.57f5c652f7cf87d221c0.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/608.57f5c652f7cf87d221c0.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/60b2da9aea5224169d569c59129b6aea.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/60b2da9aea5224169d569c59129b6aea.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/680.fd2ce6a69f228ec1a2d0.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/680.fd2ce6a69f228ec1a2d0.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/72d28790afb57a543ab3215b7fcff696.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/72d28790afb57a543ab3215b7fcff696.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/771.a2b39dd451456852d62a.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/771.a2b39dd451456852d62a.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/77db62d20f442ca57ed2fba2bb8bdf0d.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/77db62d20f442ca57ed2fba2bb8bdf0d.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/808.1a0aee7cc43bc809830d.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/808.1a0aee7cc43bc809830d.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/820.ef2aa58b90057d1d858f.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/820.ef2aa58b90057d1d858f.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/83e0246ba1dc6bed1c4c6ef2bb708e6d.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/83e0246ba1dc6bed1c4c6ef2bb708e6d.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/840.3f6ddcfae65b29844150.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/840.3f6ddcfae65b29844150.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/8b0b574430b7d19d0afcaf576a964c21.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/8b0b574430b7d19d0afcaf576a964c21.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/960.69e3e9a01225afeb6d5a.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/960.69e3e9a01225afeb6d5a.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/bc9b37bfe8ed72f234a5972c2c45239c.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/bc9b37bfe8ed72f234a5972c2c45239c.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/browsersupport.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/browsersupport.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/d7ffbebc7a4edf70373bbc18d3ca66cf.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/d7ffbebc7a4edf70373bbc18d3ca66cf.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/e528e8e6e67ca7bdcbb707be99615dba.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/e528e8e6e67ca7bdcbb707be99615dba.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/efdadec91f4d830906939a930fc180aa.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/efdadec91f4d830906939a930fc180aa.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/favicon.ico` & `codechecker-6.22.2/build_dist/CodeChecker/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.10.0/bug_path_length_filter.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.10.0/bug_path_length_filter.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.17.0/git_blame.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.17.0/git_blame.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.7.0/component_filter.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.7.0/component_filter.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.7.0/plist_to_html_index.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.7.0/plist_to_html_index.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.8.0/analysis_statistics.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.8.0/analysis_statistics.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.8.0/report_hash_filter.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.8.0/report_hash_filter.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/new_features/6.9.1/macro_expansion.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/new_features/6.9.1/macro_expansion.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/confidentiality.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/confidentiality.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/disable_review_status_change.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/disable_review_status_change.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/edit_announcement_btn.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/edit_announcement_btn.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/edit_product.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/edit_product.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/new_product.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/new_product.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/no_permission.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/no_permission.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/notificaiton_dialog.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/notificaiton_dialog.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/notification.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/notification.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/product_permissions.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/product_permissions.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/products.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/products.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/products/remove_product.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/products/remove_product.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/bug_path.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/bug_path.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/button_pane.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/button_pane.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/checker_documentation.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/checker_documentation.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/comment.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/comment.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/report_navigation_tree.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/report_navigation_tree.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_change.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_change.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_message.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_message.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/review_status_unreviewed.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/review_status_unreviewed.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/report/same_reports.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/report/same_reports.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/assign_report_to_cleanup_plan.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/assign_report_to_cleanup_plan.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/assign_reports_to_cleanup_plan.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/assign_reports_to_cleanup_plan.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/cleanup_plan_filter.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/cleanup_plan_filter.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/clear_all_filters.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/clear_all_filters.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/compare_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/compare_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/compare_tags.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/compare_tags.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.svg` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_status_flow_chart.svg`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/detection_statuses.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/detection_statuses.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/filter_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/filter_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/filters.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/filters.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/list_of_cleanup_plans.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/list_of_cleanup_plans.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/list_of_source_components.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/list_of_source_components.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/manage_source_components.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/manage_source_components.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/remove_filtered_reports.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/remove_filtered_reports.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/reports.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/reports.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/review_statuses.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/review_statuses.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/severity_levels.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/severity_levels.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/reports/unqiue_reports.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/reports/unqiue_reports.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/review_status_rules/review_status.rules.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/review_status_rules/review_status.rules.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/analyzer_statistics.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/analyzer_statistics.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/check_command.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/check_command.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/compare_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/compare_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/delete_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/delete_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/filter_run_history_events.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/filter_run_history_events.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/filter_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/filter_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_analyzer_statistics_btn.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_analyzer_statistics_btn.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_description.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_description.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/show_run_history.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/show_run_history.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/runs/sort_runs.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/runs/sort_runs.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/checker_statistics.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/checker_statistics.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/component_statistics.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/component_statistics.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/component_statistics_expanded.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/component_statistics_expanded.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/product_overview.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/product_overview.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/images/statistics/severity_statistics.png` & `codechecker-6.22.2/build_dist/CodeChecker/www/images/statistics/severity_statistics.png`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/index.html` & `codechecker-6.22.2/build_dist/CodeChecker/www/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><title>CodeChecker viewer</title><link rel="icon" href="/favicon.ico"><script defer="defer" src="/runtime.78a99b5041c202c0a7ed.js"></script><script defer="defer" src="/vendors.fdae442ee1b89ce2b7f8.js"></script><script defer="defer" src="/main.176c47b086909cc3937b.js"></script></head><body><noscript><strong>We're sorry but CodeChecker doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/browsersupport.js"></script><script src="/static.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><title>CodeChecker viewer</title><link rel="icon" href="/favicon.ico"><script defer="defer" src="/runtime.e1b8e20cfbd50bdd0fef.js"></script><script defer="defer" src="/vendors.fdae442ee1b89ce2b7f8.js"></script><script defer="defer" src="/main.42489517cdf5af8e5e0e.js"></script></head><body><noscript><strong>We're sorry but CodeChecker doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/browsersupport.js"></script><script src="/static.js"></script></body></html>
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/main.176c47b086909cc3937b.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/main.42489517cdf5af8e5e0e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9749,15 +9749,15 @@
                     component: function() {
                         return Promise.all([n.e(216), n.e(198)]).then(n.bind(n, 87198))
                     }
                 }, {
                     path: "/new-features",
                     name: "new-features",
                     component: function() {
-                        return Promise.all([n.e(216), n.e(452)]).then(n.bind(n, 19452))
+                        return Promise.all([n.e(216), n.e(950)]).then(n.bind(n, 7950))
                     }
                 }, {
                     path: "/404",
                     name: "404",
                     component: function() {
                         return n.e(343).then(n.bind(n, 84343))
                     }
@@ -9769,21 +9769,21 @@
                     component: function() {
                         return n.e(291).then(n.bind(n, 36291))
                     },
                     children: [{
                         path: "",
                         name: "main_runs",
                         component: function() {
-                            return Promise.all([n.e(216), n.e(204)]).then(n.bind(n, 17204))
+                            return Promise.all([n.e(216), n.e(324)]).then(n.bind(n, 60324))
                         }
                     }, {
                         path: "runs",
                         name: "runs",
                         component: function() {
-                            return Promise.all([n.e(216), n.e(204)]).then(n.bind(n, 17204))
+                            return Promise.all([n.e(216), n.e(324)]).then(n.bind(n, 60324))
                         }
                     }, {
                         path: "statistics",
                         component: function() {
                             return Promise.all([n.e(216), n.e(771)]).then(n.bind(n, 80771))
                         },
                         children: [{
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.5d42b4e.ttf` & `codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.5d42b4e.ttf`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.5dff34d.woff` & `codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.5dff34d.woff`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.606b164.woff2` & `codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.606b164.woff2`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/materialdesignicons-webfont.e044ed2.eot` & `codechecker-6.22.2/build_dist/CodeChecker/www/materialdesignicons-webfont.e044ed2.eot`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/runtime.78a99b5041c202c0a7ed.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/runtime.e1b8e20cfbd50bdd0fef.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -38,27 +38,27 @@
         for (var t in r) n.o(r, t) && !n.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((r, t) => (n.f[t](e, r), r)), [])), n.u = e => e + "." + {
         91: "f30e841add2c06736bcc",
         198: "71b517a7d103c8182680",
-        204: "48d4cf3235458f4f48b8",
         257: "2fb64e335d3132937e67",
         287: "0bc0c02a80fc6fec452e",
         291: "5a3df2fbabd931cce421",
+        324: "780b5ed89944be295f22",
         343: "e2548aa08e829c446317",
-        452: "49b8e5bc5792d6509d2d",
-        455: "0a5796cf6fe665353148",
+        455: "f9ee007c1bcfd28541ae",
         608: "57f5c652f7cf87d221c0",
         680: "fd2ce6a69f228ec1a2d0",
         771: "a2b39dd451456852d62a",
         808: "1a0aee7cc43bc809830d",
         820: "ef2aa58b90057d1d858f",
         840: "3f6ddcfae65b29844150",
+        950: "87a139d7b44cf5913f38",
         960: "69e3e9a01225afeb6d5a"
     } [e] + ".js", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
```

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js` & `codechecker-6.22.2/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js.LICENSE.txt` & `codechecker-6.22.2/build_dist/CodeChecker/www/vendors.fdae442ee1b89ce2b7f8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/docs/README.md` & `codechecker-6.22.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/scripts/gerrit_changed_files_to_skipfile.py` & `codechecker-6.22.2/scripts/gerrit_changed_files_to_skipfile.py`

 * *Files identical despite different names*

### Comparing `codechecker-6.22.1/setup.py` & `codechecker-6.22.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 with open(os.path.join("docs", "README.md"), "r",
           encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="codechecker",
-    version="6.22.1",
+    version="6.22.2",
     author='CodeChecker Team (Ericsson)',
     author_email='codechecker-tool@googlegroups.com',
     description="CodeChecker is an analyzer tooling, defect database and "
                 "viewer extension",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url="https://github.com/Ericsson/CodeChecker",
```

