# Comparing `tmp/jaseci-1.4.1.7.tar.gz` & `tmp/jaseci-1.4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.1.7.tar", last modified: Thu Jul 20 04:00:55 2023, max compression
+gzip compressed data, was "jaseci-1.4.1.8.tar", last modified: Mon Jul 24 16:59:09 2023, max compression
```

## Comparing `jaseci-1.4.1.7.tar` & `jaseci-1.4.1.8.tar`

### file list

```diff
@@ -1,210 +1,217 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.615107 jaseci-1.4.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-20 04:00:55.615107 jaseci-1.4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.563104 jaseci-1.4.1.7/jaseci/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.567104 jaseci-1.4.1.7/jaseci/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/cli_tools/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/cli_tools/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.567104 jaseci-1.4.1.7/jaseci/cli_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/cli_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/cli_tools/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.567104 jaseci-1.4.1.7/jaseci/extens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.571104 jaseci-1.4.1.7/jaseci/extens/act_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.575104 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/act_lib/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.583105 jaseci-1.4.1.7/jaseci/extens/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.583105 jaseci-1.4.1.7/jaseci/extens/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_uncommon.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.587105 jaseci-1.4.1.7/jaseci/extens/svc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/elastic_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/kube_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/prome_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/redis_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/stripe_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/task_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/extens/svc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.587105 jaseci-1.4.1.7/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.591106 jaseci-1.4.1.7/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    67003 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.591106 jaseci-1.4.1.7/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.591106 jaseci-1.4.1.7/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.595106 jaseci-1.4.1.7/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.595106 jaseci-1.4.1.7/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.595106 jaseci-1.4.1.7/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.595106 jaseci-1.4.1.7/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.599106 jaseci-1.4.1.7/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.599106 jaseci-1.4.1.7/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.603106 jaseci-1.4.1.7/jaseci/jsorc/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/jsorc_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/jsorc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/live_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.603106 jaseci-1.4.1.7/jaseci/jsorc/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/manifests/database.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/manifests/elastic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/manifests/prometheus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/manifests/redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.603106 jaseci-1.4.1.7/jaseci/jsorc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/jsorc/tests/test_jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.607107 jaseci-1.4.1.7/jaseci/prim/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/ability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/architype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/super_master.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/prim/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.611107 jaseci-1.4.1.7/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    25134 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.611107 jaseci-1.4.1.7/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.615107 jaseci-1.4.1.7/jaseci/utils/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/actions/actions_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/actions/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/actions/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/gprof2dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:55.563104 jaseci-1.4.1.7/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 04:00:55.000000 jaseci-1.4.1.7/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:00:55.615107 jaseci-1.4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-20 04:00:37.000000 jaseci-1.4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.148005 jaseci-1.4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 16:59:09.144005 jaseci-1.4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.116005 jaseci-1.4.1.8/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.116005 jaseci-1.4.1.8/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.116005 jaseci-1.4.1.8/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21548 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.116005 jaseci-1.4.1.8/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.120005 jaseci-1.4.1.8/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.120005 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.124005 jaseci-1.4.1.8/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_uncommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/storage_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67278 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.128005 jaseci-1.4.1.8/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.132005 jaseci-1.4.1.8/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.136005 jaseci-1.4.1.8/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.136005 jaseci-1.4.1.8/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.140005 jaseci-1.4.1.8/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.140005 jaseci-1.4.1.8/jaseci/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/svc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.144005 jaseci-1.4.1.8/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25823 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32750 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.144005 jaseci-1.4.1.8/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.144005 jaseci-1.4.1.8/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:59:09.116005 jaseci-1.4.1.8/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 16:59:09.000000 jaseci-1.4.1.8/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:59:09.148005 jaseci-1.4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 16:58:50.000000 jaseci-1.4.1.8/setup.py
```

### Comparing `jaseci-1.4.1.7/LICENSE` & `jaseci-1.4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/__init__.py` & `jaseci-1.4.1.8/jaseci/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 def load_standard():
     import jaseci.extens.act_lib.net  # noqa
     import jaseci.extens.act_lib.rand  # noqa
     import jaseci.extens.act_lib.request  # noqa
     import jaseci.extens.act_lib.std  # noqa
     import jaseci.extens.act_lib.file  # noqa
+    import jaseci.extens.act_lib.file_handler  # noqa
+    import jaseci.extens.act_lib.storage  # noqa
     import jaseci.extens.act_lib.vector  # noqa
     import jaseci.extens.act_lib.date  # noqa
     import jaseci.extens.act_lib.jaseci  # noqa
     import jaseci.extens.act_lib.mail  # noqa
     import jaseci.extens.act_lib.task  # noqa
     import jaseci.extens.act_lib.internal  # noqa
     import jaseci.extens.act_lib.zip  # noqa
```

### Comparing `jaseci-1.4.1.7/jaseci/cli_tools/book_tools.py` & `jaseci-1.4.1.8/jaseci/cli_tools/book_tools.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/cli_tools/jsctl.py` & `jaseci-1.4.1.8/jaseci/cli_tools/jsctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import requests
 from click_shell import shell
 from click.testing import CliRunner
 from jaseci import __version__
 from jaseci.prim.super_master import SuperMaster
 from jaseci.utils.utils import copy_func
 from .book_tools import Book, modifiedBook
+from jaseci.utils.file_handler import FileHandler
 from jaseci.utils.utils import logger, perf_test_start, perf_test_stop, find_first_api
 from jaseci.jsorc.jsorc import JsOrc
 from prettytable import PrettyTable
 
 session = None
 
 
@@ -98,14 +99,20 @@
     ret = method(
         session["connection"]["url"] + f"/{path}/{api_name}",
         json=payload,
         headers=session["connection"]["headers"],
     )
     if ret.status_code > 205:
         ret = f"Status Code Error {ret.status_code}\n{ret.json()}"
+    elif ret.headers.get("Content-Type", None) == "application/octet-stream":
+        file_handler = FileHandler.fromRequest(
+            ret.content, ret.headers.get("Content-Disposition")
+        )
+        session["master"]._h.add_file_handler(file_handler)
+        ret = file_handler.attr()
     else:
         ret = ret.json()
     return ret
 
 
 def resolve_none_type(kwargs):
     for i in kwargs.keys():
@@ -168,20 +175,20 @@
     if not is_cli_only and is_connected():
         out = remote_api_call(kwargs, api_name)
     elif is_public:
         out = session["master"].public_interface_to_api(kwargs, api_name)
     else:
         out = session["master"].general_interface_to_api(kwargs, api_name)
     d_out = out
-    if (
-        isinstance(out, dict)
-        and "report_custom" in out.keys()
-        and out["report_custom"] is not None
-    ):
-        out = out["report_custom"]
+    if isinstance(out, dict):
+        if "report_custom" in out.keys() and out["report_custom"] is not None:
+            out = out["report_custom"]
+        elif "report_file" in out.keys() and out["report_file"] is not None:
+            out = session["master"]._h.get_file_handler(out["report_file"]).attr()
+
     if isinstance(out, dict) or isinstance(out, list):
         out = json.dumps(out, indent=2)
     click.echo(out)
     if "output" in kwargs and kwargs["output"]:
         with open(kwargs["output"], "w") as f:
             f.write(out)
         click.echo(f'[saved to {kwargs["output"]}]')
```

### Comparing `jaseci-1.4.1.7/jaseci/cli_tools/tests/test_jsctl.py` & `jaseci-1.4.1.8/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/date.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/elastic.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/file.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/file.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/jaseci.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/jaseci.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/maths.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/maths.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/net.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/net.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/rand.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/rand.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/regex.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/request.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Built in actions for Jaseci"""
 import requests
 from jaseci.jsorc.live_actions import jaseci_action
-from base64 import b64decode, b64encode
-from io import BytesIO
 
 
 @jaseci_action()
 def get(url: str, data: dict, header: dict):
     """
     Issue request
     Param 1 - url
@@ -116,57 +114,56 @@
         ret["response"] = res.json()
     except Exception:
         ret["response"] = res.text
     return ret
 
 
 @jaseci_action()
-def multipart_base64(url: str, files: list, header: dict):
+def multipart(
+    url: str, data: dict = {}, files: list = [], header: dict = {}, meta: dict = {}
+):
     """
     Issue request
     Param 1 - url
-    Param 3 - header
-    Param 3 - file (Optional) used for single file
-    Param 4 - files (Optional) used for multiple files
-    Note - file and files can't be None at the same time
+    Param 2 - data (Optional) used for request body
+    Param 3 - files (Optional) used for request files
+    Param 4 - header
 
     Return - response object
     """
 
+    hook = meta["h"]
+
     if not files:
         return {
             "status_code": 400,
             "error": "Please include base64 using this format "
             '{"field":val,"name":val,"base64":val} '
             "using parameter `file` and `files` for array file",
         }
 
-    form_data = []
+    _files = []
+    stream_to_be_close = []
 
     if files is not None:
         for f in files:
-            form_data.append(
+            file_handler = hook.get_file_handler(f)
+            stream = file_handler.open("rb", None, True)
+            stream_to_be_close.append(stream)
+            _files.append(
                 (
-                    f["field"] if "field" in f else "file",
-                    (f["name"], BytesIO(b64decode(f["base64"]))),
+                    file_handler.field or "file",
+                    (file_handler.name, stream, file_handler.content_type),
                 )
             )
 
-    res = requests.post(url, files=form_data, headers=header)
+    res = requests.post(url, data=data, files=_files, headers=header)
     ret = {"status_code": res.status_code}
     try:
         ret["response"] = res.json()
     except Exception:
         ret["response"] = res.text
-    return ret
 
+    for stream in stream_to_be_close:
+        stream.close()
 
-@jaseci_action()
-def file_download_base64(url: str, header: dict, encoding: str = "utf-8"):
-    """Standard built in for download file from url"""
-    with requests.get(url, stream=True, headers=header) as res:
-        res.raise_for_status()
-        with BytesIO() as buffer:
-            for chunk in res.iter_content(chunk_size=8192):
-                buffer.write(chunk)
-            ret = buffer.getvalue()
-    return b64encode(ret).decode(encoding)
+    return ret
```

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/std.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/std.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,40 +107,43 @@
 @jaseci_action()
 def actload_local(filename: str, meta):
     """
     Load local actions to Jaseci
     """
     mast = master_from_meta(meta)
     if not mast.is_master(super_check=True, silent=True):
-        meta["interp"].rt_error("Only super master can load actions.")
-        return False
+        meta["interp"].rt_error(
+            "Only super master can load actions.", meta["interp"]._cur_jac_ast
+        )
     return mast.actions_load_local(file=filename)["success"]
 
 
 @jaseci_action()
 def actload_remote(url: str, meta):
     """
     Load remote actions to Jaseci
     """
     mast = master_from_meta(meta)
     if not mast.is_master(super_check=True, silent=True):
-        meta["interp"].rt_error("Only super master can load actions.")
-        return False
+        meta["interp"].rt_error(
+            "Only super master can load actions.", meta["interp"]._cur_jac_ast
+        )
     return mast.actions_load_remote(url=url)["success"]
 
 
 @jaseci_action()
 def actload_module(module: str, meta):
     """
     Load module actions to Jaseci
     """
     mast = master_from_meta(meta)
     if not mast.is_master(super_check=True, silent=True):
-        meta["interp"].rt_error("Only super master can load actions.")
-        return False
+        meta["interp"].rt_error(
+            "Only super master can load actions.", meta["interp"]._cur_jac_ast
+        )
     return mast.actions_load_module(mod=module)["success"]
 
 
 @jaseci_action()
 def destroy_global(name: str, meta):
     """Get utc date time for now in iso format"""
     mast = master_from_meta(meta)
```

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/stripe.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/std_test_code.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_date.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_elastic.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_file_lib.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_mail_lib.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_mail_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_maths.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_net_lib.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_regex.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_std.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_std_lib.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_url.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_vector.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_webtool.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/tests/test_zlib.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/url.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/vector.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/webtool.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/act_lib/zip.py` & `jaseci-1.4.1.8/jaseci/extens/act_lib/zip.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/actions_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/alias_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/alias_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/architype_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/config_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/config_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/global_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/graph_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/interface.py` & `jaseci-1.4.1.8/jaseci/extens/api/interface.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/jac_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/jac_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/jsorc_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/jsorc_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 JSORC APIs
 """
 import json
 from json import dumps
 from time import time
-from base64 import b64decode
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.jsorc.jsorc_utils import convert_yaml_manifest, ManifestType
 from jaseci.utils.utils import logger
 from jaseci.extens.svc.kube_svc import KubeService
+from jaseci.utils.file_handler import FileHandler
 from jaseci.utils.actions.actions_manager import ActionManager
 
 from jaseci.extens.api.interface import Interface
 
 
 class JsOrcApi:
     """
@@ -32,30 +32,35 @@
         """
 
         try:
             kube = JsOrc.svc("kube").poke(KubeService)
 
             res = {}
             for file in files:
+                file: FileHandler = self._h.get_file_handler(file)
+                file.open()
+
                 for kind, confs in kube.resolve_manifest(
-                    convert_yaml_manifest(b64decode(file["base64"])),
+                    convert_yaml_manifest(file.buffer),
                     ManifestType[manifest_type],
                     manual_namespace,
                 ).items():
                     for name, conf in confs.items():
                         metadata: dict = conf["metadata"]
                         kube.create(
                             kind,
                             metadata["name"],
                             conf,
                             metadata.get("namespace"),
                         )
                         if not res.get(kind):
                             res[kind] = {}
                         res[kind].update({name: conf})
+
+                file.close()
             return res
         except Exception:
             logger.exception("Error loading yaml!")
             return {"message": "load_yaml is not supported on non automated JsOrc!"}
 
     @Interface.admin_api(cli_args=["service"])
     def apply_yaml(self, service: str, file: list, unsafe_paraphrase: str = ""):
@@ -64,26 +69,31 @@
         """
         svc = JsOrc.svc(service)
 
         new_config = {}
 
         config_version = str(time())
 
-        for kind, confs in convert_yaml_manifest(b64decode(file[0]["base64"])).items():
+        file: FileHandler = self._h.get_file_handler(file[0])
+        file.open()
+
+        for kind, confs in convert_yaml_manifest(file.buffer).items():
             for name, conf in confs.items():
                 metadata = conf["metadata"]
                 labels: dict = metadata.get("labels", {})
                 if not labels.get("config_version"):
                     labels["config_version"] = config_version
                     metadata["labels"] = labels
 
                 if not new_config.get(kind):
                     new_config[kind] = {}
                 new_config[kind].update({name: conf})
 
+        file.close()
+
         if unsafe_paraphrase == JsOrc.settings("UNSAFE_PARAPHRASE"):
             new_config["__UNSAFE_PARAPHRASE__"] = unsafe_paraphrase
 
         self._h.save_glob(svc.source["manifest"], dumps(new_config))
         JsOrc.add_regeneration_queue(service)
 
         return new_config
```

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/logger_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/master_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/master_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/object_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/prometheus_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/queue_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/sentinel_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/super_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/super_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_architype_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_global_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_graph_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_logger_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_object_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_sentinel_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_uncommon.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_uncommon.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_user_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/tests/test_walker_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/tests/test_walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/user_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/walker_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/api/webhook_api.py` & `jaseci-1.4.1.8/jaseci/extens/api/webhook_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 
 class WebhookApi:
     """
     Webhook API
     """
 
     @Interface.public_api(url_args=["provider"], allowed_methods=["post"])
-    def webhook(self, provider: str, _req_ctx: dict = {}, _raw_req_ctx: str = None):
+    def webhook(self, provider: str, _req_ctx: dict = {}):
         """Handle webhook logic"""
         req_body = _req_ctx["body"]
 
         if provider == "stripe":
             stripe_service = JsOrc.svc("stripe", StripeService)
             stripe = stripe_service.poke(_stripe)
 
             # to be updated
-            stripe_service.get_event(_raw_req_ctx, _req_ctx["headers"])
+            stripe_service.get_event(
+                self._h.get_file_handler(_req_ctx["raw"]), _req_ctx["headers"]
+            )
 
             payload_obj = req_body.get("data").get("object")
             payload_meta = payload_obj.get("metadata")
 
             customer_id = payload_obj.get("customer")
             customer_meta = (
                 stripe.Customer.retrieve(id=customer_id).get("metadata")
```

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/elastic_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/elastic_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/kube_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/kube_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/mail_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/prome_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/prome_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/redis_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/redis_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/stripe_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/stripe_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/task_svc.py` & `jaseci-1.4.1.8/jaseci/extens/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/extens/svc/tasks.py` & `jaseci-1.4.1.8/jaseci/extens/svc/tasks.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.1.8/jaseci/jac/interpreter/architype_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.1.8/jaseci/jac/interpreter/interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,23 +346,27 @@
         kid = self.set_cur_ast(jac_ast)
         if kid[1].name == "COLON":
             self.run_expression(kid[4])
             if kid[2].token_text() in ["status", "status_code"]:
                 self.report_status = self.pop().value
             elif kid[2].token_text() == "custom":
                 self.report_custom = jwv(self.pop().value, serialize_mode=True)
+            elif kid[2].token_text() == "file":
+                self.report_file = self.pop().value
             elif kid[2].token_text() == "error":
                 err = self.pop().value
                 if isinstance(err, str):
                     self.runtime_errors.append(err)
                 else:
                     self.runtime_errors.append(
                         f'{err["mod"]}:{err["name"]} - line {err["line"]}, '
                         + f'col {err["col"]} - rule {err["rule"]} - {err["msg"]}'
                     )
+                    for stk in err.get("stack_trace", []):
+                        self.runtime_stack_trace.append(stk)
             else:
                 self.rt_error("Invalid report attribute to set", kid[2])
         else:
             self.run_expression(kid[1])
             report = jwv(self.pop().value, serialize_mode=True)
             if not is_jsonable(report):
                 self.rt_error(f"Report {report} not Json serializable", kid[0])
@@ -396,15 +400,15 @@
                     dest = self.run_rule(kid[0])
                     self._assign_mode = False
                     self.run_inc_assign(kid[1])
                     self.perform_increment(
                         dest, self.pop(), JsCmp[kid[1].kid[0].name], kid[0]
                     )
         except Exception as e:
-            self.jac_try_exception(e, jac_ast)
+            self.rt_error(e, jac_ast)
 
     def run_assignment(self, jac_ast):
         """
         assignment: EQ expression;
         """
         if self.attempt_bytecode(jac_ast):
             return
@@ -632,15 +636,15 @@
                     return JacValue(
                         self,
                     )
 
                 return JacValue(self, ctx=self.parent().global_vars, name=token)
 
         except Exception as e:
-            self.jac_try_exception(e, jac_ast)
+            self.rt_error(e, jac_ast)
 
     def run_atom(self, jac_ast):
         """
         atom:
             INT
             | FLOAT
             | multistring
@@ -703,15 +707,15 @@
                         ),
                     )
                 )
             else:
                 self.push(self.run_rule(kid[0]))
 
         except Exception as e:
-            self.jac_try_exception(e, jac_ast)
+            self.rt_error(e, jac_ast)
 
     def run_atom_trailer(self, jac_ast, atom_res):
         """
         atom_trailer:
             DOT built_in
             | DOT NAME
             | index_slice
@@ -749,15 +753,15 @@
             elif kid[0].name == "index_slice":
                 if not self.rt_check_type(atom_res.value, [list, str, dict], kid[0]):
                     return atom_res
                 return self.run_index_slice(kid[0], atom_res)
             elif kid[0].name == "ability_call":
                 return self.run_ability_call(kid[0], atom_res)
         except Exception as e:
-            self.jac_try_exception(e, jac_ast)
+            self.rt_error(e, jac_ast)
 
     def run_ability_call(self, jac_ast, atom_res):
         """
         ability_call:
             LPAREN param_list? RPAREN
             | ability_op NAME spawn_ctx?;
         """
@@ -765,15 +769,17 @@
 
         kid = self.set_cur_ast(jac_ast)
         if kid[0].name == "LPAREN":
             param_list = {"args": [], "kwargs": {}}
             if kid[1].name == "param_list":
                 param_list = self.run_param_list(kid[1]).value
             if isinstance(atom_res.value, Ability):
-                ret = atom_res.value.run_action(param_list, self._jac_scope, self)
+                ret = atom_res.value.run_action(
+                    param_list, self._jac_scope, self, jac_ast
+                )
                 return JacValue(self, value=ret)
             else:
                 self.rt_error("Unable to execute ability", kid[0])
         elif kid[0].name == "ability_op":
             arch = self.run_ability_op(kid[0], atom_res)
             if len(kid) > 2:
                 self.run_spawn_ctx(kid[2], atom_res.value)
@@ -792,15 +798,15 @@
         base_arch = atom_res.value.get_architype()
         if len(kid) > 1:
             kind = atom_res.value.kind
             name = kid[1].token_text()
             if name in base_arch.derived_types():
                 return self.parent().arch_ids.get_obj_by_name(name=name, kind=kind)
             else:
-                self.rt_error(f"{name} is not a super arch of {base_arch.name}")
+                self.rt_error(f"{name} is not a super arch of {base_arch.name}", kid[1])
                 return None
         else:
             return base_arch
 
     def run_ref(self, jac_ast):
         """
         ref: '&' atom;
@@ -1001,15 +1007,15 @@
                         result = JacValue(self, value=atom_res.value.update(*args))
                         self.candidate_writethrough()
                     elif op == "get":
                         result = JacValue(self, value=atom_res.value.get(*args))
                     if result:
                         return result
             except Exception as e:
-                self.rt_error(f"{e}", jac_ast)
+                self.rt_error(e, jac_ast)
             self.rt_error(f"Call to {op} is invalid.", jac_ast)
 
         return atom_res
 
     def run_list_built_in(self, jac_ast, atom_res):
         """
         list_built_in:
@@ -1097,15 +1103,15 @@
                         result = JacValue(self, value=atom_res.value.count(*args))
                     elif op == "pop":
                         result = JacValue(self, value=atom_res.value.pop(*args))
                         self.candidate_writethrough()
                     if result:
                         return result
             except Exception as e:
-                self.rt_error(f"{e}", jac_ast)
+                self.rt_error(e, jac_ast)
             self.rt_error(f"Call to {op} is invalid.", jac_ast)
         return atom_res
 
     def run_string_built_in(self, jac_ast, atom_res):
         """
         string_built_in:
         (TYP_STRING DBL_COLON | STR_DBL_COLON) NAME (
@@ -1187,15 +1193,15 @@
                 elif str_op == "lstrip":
                     result = JacValue(self, value=atom_res.value.lstrip(*args))
                 elif str_op == "rstrip":
                     result = JacValue(self, value=atom_res.value.rstrip(*args))
                 if result:
                     return result
         except Exception as e:
-            self.rt_error(f"{e}", jac_ast)
+            self.rt_error(e, jac_ast)
         self.rt_error(f"Call to {str_op} is invalid.", jac_ast)
         return atom_res
 
     def run_node_edge_ref(self, jac_ast, viable_nodes=None):
         """
         node_edge_ref:
             node_ref filter_ctx? node_edge_ref?
@@ -1401,33 +1407,31 @@
                     f"Index of type {type(idx)} not valid. "
                     f"Indicies must be an integer or string!",
                     kid[1],
                 )
                 return atom_res
             try:
                 return JacValue(self, ctx=atom_res.value, name=idx)
-            except Exception:
-                self.rt_error("List index out of range", kid[1])
-                return atom_res
+            except Exception as e:
+                self.rt_error(e, jac_ast, isinstance(e, (IndexError, AttributeError)))
         else:
             self.run_expression(kid[3])
             end = self.pop().value
             if not self.rt_check_type(idx, [int], kid[1]) or not self.rt_check_type(
                 end, [int], kid[3]
             ):
                 self.rt_error(
-                    "List slice range not valid. " "Indicies must be an integers!",
+                    "List slice range not valid. Indicies must be an integers!",
                     kid[1],
                 )
                 return atom_res
             try:
                 return JacValue(self, ctx=atom_res.value, name=idx, end=end)
-            except Exception:
-                self.rt_error("List slice out of range", kid[1])
-                return atom_res
+            except Exception as e:
+                self.rt_error(e, jac_ast, isinstance(e, (IndexError, AttributeError)))
 
     def run_dict_val(self, jac_ast):
         """
         dict_val: LBRACE (kv_pair (COMMA kv_pair)*)? RBRACE;
         """
         kid = self.set_cur_ast(jac_ast)
         dict_res = {}
@@ -1772,9 +1776,11 @@
             if not hasattr(self, f"run_{jac_ast.name}"):
                 self.rt_error(
                     f"This scope cannot execute the statement "
                     f'"{jac_ast.get_text()}" of type {jac_ast.name}',
                     jac_ast,
                 )
             else:
-                self.rt_error(f"{e}", jac_ast)
+                self.rt_error(e, jac_ast)
             return
+        except Exception as e:
+            self.rt_error(e, jac_ast)
```

### Comparing `jaseci-1.4.1.7/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.1.8/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.1.8/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.1.8/jaseci/jac/interpreter/walker_interp.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,17 +198,17 @@
                 visitor=self,
             )
         )
 
         if kid[1].name == "param_list":
             param_list = self.run_param_list(kid[1]).value
         try:
-            result = act.run_action(param_list, self._jac_scope, self)
+            result = act.run_action(param_list, self._jac_scope, self, jac_ast)
         except Exception as e:
-            self.rt_error(f"Internal Exception: {e}", self._cur_jac_ast)
+            self.rt_error(e, jac_ast)
             result = None
         if kid[-1].name == "expression":
             self.run_expression(kid[-1])
             dest = self.pop()
             dest.value = result
             dest.write(kid[-1])
         self.pop_scope()
```

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/ast.py` & `jaseci-1.4.1.8/jaseci/jac/ir/ast.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.1.8/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.1.8/jaseci/jac/ir/jac_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.1.8/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.1.8/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.1.8/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.1.8/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.1.8/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jac.g4` & `jaseci-1.4.1.8/jaseci/jac/jac.g4`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.1.8/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.1.8/jaseci/jac/jac_parse/jacListener.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.1.8/jaseci/jac/jac_parse/jacParser.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jac_set.py` & `jaseci-1.4.1.8/jaseci/jac/jac_set.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.1.8/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.1.8/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.1.8/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.1.8/jaseci/jac/jsci_vm/op_codes.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.1.8/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.1.8/jaseci/jac/machine/jac_scope.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.1.8/jaseci/jac/machine/jac_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,18 @@
                 not self.parent._assign_mode
                 and not create_mode
                 and (
                     not self.is_element
                     or self.name not in self.is_element.get_architype().has_vars
                 )
             ):
-                self.parent.rt_error(f"Key {self.name} not found in object/dict.")
+                self.parent.rt_error(
+                    f"Key {self.name} not found in object/dict.",
+                    self.parent._cur_jac_ast,
+                )
         else:
             return None
 
     def write(self, jac_ast, force=False):
         if (
             not force
             and self.is_element
```

### Comparing `jaseci-1.4.1.7/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.1.8/jaseci/jac/machine/machine_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
 from copy import copy
-from jaseci.utils.utils import logger
+from jaseci.utils.utils import logger, exc_stack_as_str_list, generate_stack_as_str_list
 from jaseci.jsorc.live_actions import live_actions, load_preconfig_actions
 
 # from jaseci.actions.find_action import find_action
 from jaseci.prim.element import Element
 
 from jaseci.jac.jac_set import JacSet
 from jaseci.jac.machine.jac_scope import JacScope
@@ -28,16 +28,18 @@
     recur_detect_set = []
     profile_stack = [None]
 
     def __init__(self):
         self.report = []
         self.report_status = None
         self.report_custom = None
+        self.report_file = None
         self.request_context = None
         self.runtime_errors = []
+        self.runtime_stack_trace = []
         self.yielded_walkers_ids = IdList(self)
         self.ignore_node_ids = IdList(self)
         self._scope_stack = [None]
         self._jac_scope = None
         self._relevant_edges = []
         self._loop_ctrl = None
         self._stopped = None
@@ -54,15 +56,17 @@
         if hasattr(self, "_h"):
             self._h._machine = self
 
     def reset(self):
         self.report = []
         self.report_status = None
         self.report_custom = None
+        self.report_file = None
         self.runtime_errors = []
+        self.runtime_stack_trace = []
         self._scope_stack = [None]
         self._jac_scope = None
         self._loop_ctrl = None
         self._stopped = None
 
     def push_scope(self, scope: JacScope):
         self.profile_pause()
@@ -153,15 +157,17 @@
 
     # Core State Management ##################
     def load_variable(self, name, assign_mode=None, jac_ast=None):
         val = self._jac_scope.get_live_var(
             name, create_mode=self._assign_mode if assign_mode is None else assign_mode
         )
         if val is None:
-            self.rt_error(f"Variable not defined - {name}", jac_ast)
+            self.rt_error(
+                f"Variable not defined - {name}", jac_ast or self._cur_jac_ast
+            )
             self.push(JacValue(self))
         else:
             self.push(val)
 
     def candidate_writethrough(self):
         if self._write_candidate:
             self._write_candidate.save()
@@ -207,14 +213,16 @@
     def inherit_runtime_state(self, mach):
         """Inherits runtime output state from another machine"""
         self.report += mach.report
         if mach.report_status:
             self.report_status = mach.report_status
         if mach.report_custom:
             self.report_custom = mach.report_custom
+        if mach.report_file:
+            self.report_file = mach.report_file
         self.runtime_errors += mach.runtime_errors
 
     def obj_set_to_jac_set(self, obj_set):
         """
         Returns nodes jac_set from edge jac_set from current node
         """
         ret = JacSet()
@@ -270,14 +278,15 @@
             "mod": jac_ast.loc[2],
             "msg": str(e),
             "args": e.args,
             "line": jac_ast.loc[0],
             "col": jac_ast.loc[1],
             "name": self.name if hasattr(self, "name") else "blank",
             "rule": jac_ast.name,
+            "stack_trace": exc_stack_as_str_list(),
         }
 
     def rt_log_str(self, msg, jac_ast=None):
         """Generates string for screen output"""
         if jac_ast is None:
             jac_ast = self._cur_jac_ast
         name = self.name if hasattr(self, "name") else "blank"
@@ -291,21 +300,47 @@
         return msg
 
     def rt_warn(self, error, jac_ast=None):
         """Prints runtime error to screen"""
         error = self.rt_log_str(error, jac_ast)
         logger.warning(str(error))
 
-    def rt_error(self, error, jac_ast=None):
+    def rt_error(self, error, jac_ast, append=False):
         """Prints runtime error to screen"""
-        if self._jac_try_mode:
-            raise Exception(error)
-        error = self.rt_log_str(error, jac_ast)
-        logger.error(str(error))
-        self.runtime_errors.append(error)
+
+        if isinstance(error, Exception):
+            if self._jac_try_mode:
+                self.jac_try_exception(error, jac_ast)
+            else:
+                if append:
+                    msg = self.rt_log_str(error, jac_ast)
+                    logger.error(msg)
+                    self.runtime_errors.append(msg)
+                raise error
+        else:
+            if self._jac_try_mode:
+                raise TryException(
+                    {
+                        "type": "RunTimeException",
+                        "mod": jac_ast.loc[2],
+                        "msg": error,
+                        "args": [],
+                        "line": jac_ast.loc[0],
+                        "col": jac_ast.loc[1],
+                        "name": self.name if hasattr(self, "name") else "blank",
+                        "rule": jac_ast.name,
+                        "stack_trace": generate_stack_as_str_list(error),
+                    }
+                )
+            else:
+                msg = self.rt_log_str(error, jac_ast)
+                logger.error(msg)
+                self.runtime_errors.append(msg)
+                error = Exception(error)
+                raise error
 
     def rt_info(self, msg, jac_ast=None):
         """Prints runtime info to screen"""
         logger.info(str(self.rt_log_str(msg, jac_ast)))
 
     def rt_check_type(self, obj, typ, jac_ast=None):
         """Prints error if type mismatach"""
@@ -323,14 +358,15 @@
         return False
 
     def get_info(self):
         return {
             "report": copy(self.report),
             "report_status": self.report_status,
             "report_custom": self.report_custom,
+            "report_file": self.report_file,
             "request_context": self.request_context,
             "runtime_errors": self.runtime_errors,
         }
 
 
 class TryException(Exception):
     def __init__(self, ref: dict):
```

### Comparing `jaseci-1.4.1.7/jaseci/jac/tests/book_code.py` & `jaseci-1.4.1.8/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/tests/test_book.py` & `jaseci-1.4.1.8/jaseci/jac/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.1.8/jaseci/jac/tests/test_lang_14.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/jsorc.py` & `jaseci-1.4.1.8/jaseci/jsorc/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/jsorc_settings.py` & `jaseci-1.4.1.8/jaseci/jsorc/jsorc_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,27 @@
         "index_template_name": ELASTIC_INDEX_TEMPLATE_NAME,
         "index_template": ELASTIC_INDEX_TEMPLATE,
     }
 
     ELASTIC_MANIFEST = load_default_yaml("elastic")
 
     ###############################################################################################################
+    # ------------------------------------------------- STORAGE ------------------------------------------------- #
+    ###############################################################################################################
+
+    STORE_CONFIG = {
+        "enabled": False,
+        "quiet": False,
+        "default": None,
+        "providers": {},
+    }
+
+    STORE_MANIFEST = {}
+
+    ###############################################################################################################
     # ------------------------------------------------ DATABASE ------------------------------------------------- #
     ###############################################################################################################
 
     DB_REGEN_CONFIG = {
         "enabled": os.environ.get("JSORC_DB_REGEN") == "true",
         "host": os.environ.get("POSTGRES_HOST", "jaseci-db"),
         "db": os.environ.get("DBNAME", "postgres"),
```

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/jsorc_utils.py` & `jaseci-1.4.1.8/jaseci/jsorc/jsorc_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/live_actions.py` & `jaseci-1.4.1.8/jaseci/jsorc/live_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/manifests/database.yaml` & `jaseci-1.4.1.8/jaseci/jsorc/manifests/database.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/manifests/elastic.yaml` & `jaseci-1.4.1.8/jaseci/jsorc/manifests/elastic.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/manifests/prometheus.yaml` & `jaseci-1.4.1.8/jaseci/jsorc/manifests/prometheus.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/manifests/redis.yaml` & `jaseci-1.4.1.8/jaseci/jsorc/manifests/redis.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/memory.py` & `jaseci-1.4.1.8/jaseci/jsorc/memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from json import dumps, loads
 import sys
+from jaseci.utils.file_handler import FileHandler
 from jaseci.utils.utils import find_class_and_import
 from jaseci.jsorc.jsorc import JsOrc
 
 
 @JsOrc.repository(name="hook")
 class MemoryHook:
     """
@@ -16,14 +17,15 @@
     def __init__(self):
         from jaseci.jsorc.live_actions import get_global_actions
 
         self.mem = {"global": {}}
         self._machine = None
         self.save_obj_list = set()
         self.save_glob_dict = {}
+        self.file_handlers = {}
 
     ####################################################
     #               COMMON GETTER/SETTER               #
     ####################################################
 
     # --------------------- OBJ ---------------------- #
 
@@ -227,7 +229,30 @@
         if not cls:
             cls = find_class_and_import(j_type, mod)
 
         return cls
 
     def clear_cache(self):
         MemoryHook.__init__(self)
+
+    ####################################################
+    #                   FILE HANDLER                   #
+    ####################################################
+
+    def add_file_handler(self, file_handler: FileHandler) -> str:
+        self.file_handlers.update({file_handler.id: file_handler})
+        return file_handler.id
+
+    def get_file_handler(self, file_id: str):
+        return self.file_handlers.get(file_id, None)
+
+    def pop_file_handler(self, file_id: str):
+        return self.file_handlers.pop(file_id, None)
+
+    def clean_file_handler(self):
+        for file_handler in list(self.file_handlers.values()):
+            self.file_handlers.pop(file_handler.id, None)
+            if not file_handler.persist:
+                file_handler.delete()
+
+    def __del__(self):
+        self.clean_file_handler()
```

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/redis.py` & `jaseci-1.4.1.8/jaseci/jsorc/redis.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/remote_actions.py` & `jaseci-1.4.1.8/jaseci/jsorc/remote_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/tests/test_actions.py` & `jaseci-1.4.1.8/jaseci/jsorc/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/jsorc/tests/test_jsorc.py` & `jaseci-1.4.1.8/jaseci/jsorc/tests/test_jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/ability.py` & `jaseci-1.4.1.8/jaseci/prim/ability.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,23 +43,23 @@
                 here=here,
                 visitor=visitor,
             )
         )
         self.run_code_block(self.get_jac_ast())
         self.pop_scope()
 
-    def run_action(self, param_list, scope, interp):
+    def run_action(self, param_list, scope, interp, jac_ast):
         """
         param_list should be passed as list of values to lib functions
         Also note that Jac stores preset_in_out as input/output list of hex
         ids since preset_in_out doesn't use _ids convention
         """
         action_name = self.name
         if not interp.check_builtin_action(action_name):
-            interp.rt_error(f"Cannot execute {action_name} - Not Found")
+            interp.rt_error(f"Cannot execute {action_name} - Not Found", jac_ast)
             return None
         func = live_actions[action_name]
         args = inspect.getfullargspec(func)
         self.do_auto_conversions(args, param_list)
         args = args[0] + args[4]
 
         action_manager = JsOrc.get("action_manager", ActionManager)
@@ -80,23 +80,18 @@
         else:
             try:
                 result = func(*param_list["args"], **param_list["kwargs"])
             except TypeError as e:
                 params = str(inspect.signature(func))
                 interp.rt_error(
                     f"Invalid arguments {param_list} to action call {self.name}! Valid paramters are {params}.",
-                    interp._cur_jac_ast,
+                    jac_ast,
                 )
-                raise
             except Exception as e:
-                interp.rt_error(
-                    f"Execption within action call {self.name}! {e}",
-                    interp._cur_jac_ast,
-                )
-                raise
+                interp.rt_error(e, jac_ast, True)
         t = time.time() - ts
         action_manager.post_action_call_hook(action_name, t)
         return result
 
     def do_auto_conversions(self, args, params):
         """
         Automatically make conversions for jac to internal, e.g., list to jac_set
```

### Comparing `jaseci-1.4.1.7/jaseci/prim/architype.py` & `jaseci-1.4.1.8/jaseci/prim/architype.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/edge.py` & `jaseci-1.4.1.8/jaseci/prim/edge.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/element.py` & `jaseci-1.4.1.8/jaseci/prim/element.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/graph.py` & `jaseci-1.4.1.8/jaseci/prim/graph.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/master.py` & `jaseci-1.4.1.8/jaseci/prim/master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/node.py` & `jaseci-1.4.1.8/jaseci/prim/node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/obj_mixins.py` & `jaseci-1.4.1.8/jaseci/prim/obj_mixins.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/sentinel.py` & `jaseci-1.4.1.8/jaseci/prim/sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,19 +214,21 @@
                 if not silent:
                     print(f"Testing {title}: ", end="")
                 sys.stdout, sys.stderr = buff_out[0], buff_out[1]
                 wlk.run()
                 sys.stdout, sys.stderr = screen_out[0], screen_out[1]
                 if i["assert_block"]:
                     wlk._loop_ctrl = None
+                    wlk._jac_try_mode += 1
                     wlk.scope_and_run(
                         jac_ir_to_ast(i["assert_block"]),
                         run_func=wlk.run_code_block,
                         scope_name="assert_block",
                     )
+                    wlk._jac_try_mode -= 1
                 i["passed"] = True
                 if not silent:
                     print(
                         f"[{Cc.TG}PASSED{Cc.EC} in {Cc.TY}{time()-stime:.2f}s{Cc.EC}]"
                     )
                 if detailed and not silent:
                     print("REPORT: " + pformat(wlk.report))
```

### Comparing `jaseci-1.4.1.7/jaseci/prim/super_master.py` & `jaseci-1.4.1.8/jaseci/prim/super_master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/prim/walker.py` & `jaseci-1.4.1.8/jaseci/prim/walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     perf_test_start,
     perf_test_stop,
     exc_stack_as_str_list,
 )
 from jaseci.prim.element import Element
 from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.id_list import IdList
+from jaseci.jac.machine.machine_state import TryException
 from jaseci.jac.interpreter.walker_interp import WalkerInterp
 import uuid
 import hashlib
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.task_svc import TaskService
 from jaseci.utils.utils import format_jac_profile
@@ -167,33 +168,40 @@
         report_ret = {"success": True}
         WalkerInterp.reset(self)
         self.yielded = False
 
         try:
             while self.step() and not self.yielded:
                 pass
-        except Exception as e:
-            self.rt_error(f"Internal Exception: {e}", self._cur_jac_ast)
+        except Exception:
+            report_ret["success"] = False
             report_ret["stack_trace"] = exc_stack_as_str_list()
 
         self.save()
 
         if not self.report:
             logger.debug(str(f"Walker {self.name} did not have anything to report"))
         report_ret["report"] = self.report
         report_ret["final_node"] = self.current_node_id
         report_ret["yielded"] = self.yielded
 
         if self.report_status:
             report_ret["status_code"] = self.report_status
         if self.report_custom:
             report_ret["report_custom"] = self.report_custom
+        if self.report_file:
+            report_ret["report_file"] = self.report_file
+
         if len(self.runtime_errors):
             report_ret["errors"] = self.runtime_errors
             report_ret["success"] = False
+        if len(self.runtime_stack_trace):
+            report_ret["stack_trace"] = (
+                report_ret.get("stack_trace", []) + self.runtime_stack_trace
+            )
         if profiling:
             self.profile["jac"] = format_jac_profile(self.get_master()._jac_profile)
             calls, graph = perf_test_stop(pr)
             self.profile["perf"] = calls
             self.profile["graph"] = graph
             report_ret["profile"] = self.profile
```

### Comparing `jaseci-1.4.1.7/jaseci/tests/infer.py` & `jaseci-1.4.1.8/jaseci/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/tests/jac_test_code.py` & `jaseci-1.4.1.8/jaseci/tests/jac_test_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -640,15 +640,19 @@
 
 typecasts_error = """
     walker init {
         a=5.6;
         report (a+2);
         report (a+2).int;
         report (a+2).str;
-        report (a+2).edge;
+
+        try {
+            report (a+2).edge;
+        } else with error: report:error = error;
+
         report ("a+2").int.float;
 
         if(a.str.type == str and !(a.int.type == str)
            and a.int.type == int):
             report "Types comes back correct";
     }
     """
@@ -814,26 +818,33 @@
         report b;
         a=[1,2,3,5,6,7,8,9];
         destroy a[2:4];
         report a;
         a[2:4]=[45,33];
         report a;
         destroy a;
-        report a;
-        person1.banana=45;
+        try {
+            report a;
+        } else with error: report:error = error;
+        try {
+            person1.banana=45;
+        } else with error: report:error = error;
         report person1.context;
         report 'age' in person1.context;
     }
     """
 
 arbitrary_assign_on_element = """
     node person: has name, age, birthday, profession;
     walker init {
         some = spawn here ++> node::person;
-        some.apple = 45;
+        try {
+            some.apple = 45;
+        } else with error: report:error = error;
+
         report some.context;
     }
     """
 
 try_else_stmts = """
     walker init {
         a=null;
@@ -843,14 +854,31 @@
         else {report 'dont need err';}
         try {a=2/0;}
         try {a=2/0;}
         report a;
         try {a=2/1;}
         report a;
     }
+
+    walker sample {
+        with entry {
+            try {
+                a = {};
+                b = {};
+
+                b.dict::update({
+                    "test2": 1,
+                    "test": a["test"]
+                });
+                report b;
+            } else with error {
+                report:error = error;
+            }
+        }
+    }
     """
 
 node_edge_same_name = """
     node person: has name, age, birthday, profession;
     edge person: has meeting_place;
 
     walker init {
```

### Comparing `jaseci-1.4.1.7/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.1.8/jaseci/tests/jac_test_progs.py`

 * *Files 2% similar despite different names*

```diff
@@ -541,22 +541,25 @@
             }
         }
     }
 
     walker var_as_key_for_dict {
         with entry {
             key = "key1";
-            not_str_key = 1;
             testing = {
                 key: key,
-                "key2": 2,
-                not_str_key: not_str_key
+                "key2": 2
             };
 
             report testing;
+
+            not_str_key = 1;
+            testing = {
+                not_str_key: not_str_key
+            };
         }
     }
 """
 
 list_pairwise = """
 walker init{
     with entry{
```

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_core.py` & `jaseci-1.4.1.8/jaseci/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_jac.py` & `jaseci-1.4.1.8/jaseci/tests/test_jac.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,15 +417,18 @@
     def test_typecast_error(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.typecasts_error)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
-        self.assertIn("Cannot get edges from 7.6", test_walker.runtime_errors[0])
+        self.assertEqual(
+            "basic:init - line 9, col 25 - rule any_type - Cannot get edges from 7.6. Type JAC_TYPE.FLOAT invalid",
+            test_walker.runtime_errors[0],
+        )
         self.assertIn(
             "Invalid cast of JAC_TYPE.STR to JAC_TYPE.INT",
             test_walker.runtime_errors[1],
         )
 
     def test_filter_on_context(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
@@ -562,40 +565,55 @@
         self.assertEqual(
             rep[2], {"age": 32, "birthday": None, "name": "pete", "profession": None}
         )
         self.assertEqual(rep[3], [1, 3])
         self.assertEqual(rep[4], {"a": "b"})
         self.assertEqual(rep[5], [1, 2, 5, 6, 7, 8, 9])
         self.assertEqual(rep[6], [1, 2, 45, 33, 7, 8, 9])
-        self.assertEqual(rep[7], None)
         self.assertEqual(
-            rep[8], {"age": 32, "birthday": None, "name": "pete", "profession": None}
+            rep[7], {"age": 32, "birthday": None, "name": "pete", "profession": None}
+        )
+        self.assertEqual(rep[8], True)
+
+        err = test_walker.runtime_errors
+        self.assertEqual(
+            err[0],
+            "basic:init - line 30, col 0 - rule report_action - Variable not defined - a",
+        )
+        self.assertEqual(
+            err[1],
+            "basic:init - line 33, col 0 - rule atom - Creating variable banana in graph element <class 'jaseci.prim.node.Node'> is not allowed, please define",
         )
-        self.assertEqual(rep[9], True)
 
     def test_arbitrary_assign_on_element(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.arbitrary_assign_on_element)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(
             rep[0], {"name": None, "age": None, "birthday": None, "profession": None}
         )
+        err = test_walker.runtime_errors
+        self.assertEqual(
+            err[0],
+            "basic:init - line 6, col 0 - rule atom - Creating variable apple in graph element <class 'jaseci.prim.node.Node'> is not allowed, please define",
+        )
 
     def test_try_else_stmts(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.try_else_stmts)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
+        rep[0].pop("stack_trace", None)  # remove stack_trace
         self.assertEqual(
             rep[0],
             {
                 "args": ("division by zero",),
                 "col": 13,
                 "line": 4,
                 "mod": "basic",
@@ -605,14 +623,24 @@
                 "rule": "expression",
             },
         )
         self.assertEqual(rep[1], "dont need err")
         self.assertEqual(rep[2], None)
         self.assertEqual(rep[3], 2)
 
+        test_walker = sent.run_architype("sample")
+        test_walker.prime(gph)
+        resp = test_walker.run()
+
+        # exact line and error
+        self.assertEqual(
+            resp["errors"][0],
+            "basic:sample - line 23, col 29 - rule index_slice - Key test not found in object/dict.",
+        )
+
     def test_node_edge_same_name(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.node_edge_same_name)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
@@ -683,17 +711,18 @@
     def test_rt_error_test1(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.rt_error_test1)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
-        self.assertIn("List index out of range", test_walker.runtime_errors[0])
-        self.assertIn(" line ", test_walker.runtime_errors[0])
-        self.assertIn(" col ", test_walker.runtime_errors[0])
+        self.assertEqual(
+            "basic:init - line 4, col 0 - rule index_slice - list index out of range",
+            test_walker.runtime_errors[0],
+        )
 
     def test_root_type_nodes(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.root_type_nodes)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
```

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_node.py` & `jaseci-1.4.1.8/jaseci/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_progs.py` & `jaseci-1.4.1.8/jaseci/tests/test_progs.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,21 @@
 
     def test_action_load_std_lib_only_super(self):
         mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.action_load_std_lib)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "aload"}
         )
-        report = report["report"]
-        self.assertEqual(report[0], False)
+        self.assertFalse(report["success"])
+        self.assertEqual(
+            [
+                "test:aload - line 3, col 33 - rule expr_list - Only super master can load actions."
+            ],
+            report["errors"],
+        )
 
     def test_globals(self):
         sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtp.globals)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
@@ -325,15 +330,18 @@
             name="test", code=jtp.check_dict_for_in_loop, auto_run=""
         )
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "var_as_key_for_dict"}
         )
 
         self.assertEqual(res["report"], [{"key1": "key1", "key2": 2}])
-        self.assertIn("Key is not str type : <class 'int'>!", res["errors"][0])
+        self.assertEqual(
+            "test:var_as_key_for_dict - line 42, col 16 - rule expression - Key is not str type : <class 'int'>!",
+            res["errors"][0],
+        )
 
     def test_list_pairwise(self):
         mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.list_pairwise, auto_run="")
 
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
```

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_stack.py` & `jaseci-1.4.1.8/jaseci/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/tests/test_stripe.py` & `jaseci-1.4.1.8/jaseci/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/actions/actions_manager.py` & `jaseci-1.4.1.8/jaseci/utils/actions/actions_manager.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/actions/actions_optimizer.py` & `jaseci-1.4.1.8/jaseci/utils/actions/actions_optimizer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/actions/actions_state.py` & `jaseci-1.4.1.8/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/gprof2dot.py` & `jaseci-1.4.1.8/jaseci/utils/gprof2dot.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/id_list.py` & `jaseci-1.4.1.8/jaseci/utils/id_list.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/json_handler.py` & `jaseci-1.4.1.8/jaseci/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/log_utils.py` & `jaseci-1.4.1.8/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/test_core.py` & `jaseci-1.4.1.8/jaseci/utils/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.1.7/jaseci/utils/utils.py` & `jaseci-1.4.1.8/jaseci/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,23 @@
     log_var_out(tb)
 
 
 def exc_stack_as_str_list():
     return traceback.format_exception(*sys.exc_info())
 
 
+def generate_stack_as_str_list(error=None):
+    stack = traceback.format_stack()
+    stack.pop()  # format_stack
+    stack.pop()  # generate_stack_as_str_list
+    if error:
+        stack.append(error)
+    return stack
+
+
 uuid_re = re.compile(
     "([a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89aAbB][a-f0-9]{3}-?[a-f0-9]{12})"
 )
 
 
 def is_urn(s: str):
     """Test if is uuid string in urn format"""
```

### Comparing `jaseci-1.4.1.7/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.1.8/jaseci.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 jaseci/cli_tools/tests/__init__.py
 jaseci/cli_tools/tests/test_jsctl.py
 jaseci/extens/__init__.py
 jaseci/extens/act_lib/__init__.py
 jaseci/extens/act_lib/date.py
 jaseci/extens/act_lib/elastic.py
 jaseci/extens/act_lib/file.py
+jaseci/extens/act_lib/file_handler.py
 jaseci/extens/act_lib/internal.py
 jaseci/extens/act_lib/jaseci.py
 jaseci/extens/act_lib/mail.py
 jaseci/extens/act_lib/maths.py
 jaseci/extens/act_lib/net.py
 jaseci/extens/act_lib/rand.py
 jaseci/extens/act_lib/regex.py
 jaseci/extens/act_lib/request.py
 jaseci/extens/act_lib/std.py
+jaseci/extens/act_lib/storage.py
 jaseci/extens/act_lib/stripe.py
 jaseci/extens/act_lib/task.py
 jaseci/extens/act_lib/url.py
 jaseci/extens/act_lib/vector.py
 jaseci/extens/act_lib/webtool.py
 jaseci/extens/act_lib/zip.py
 jaseci/extens/act_lib/tests/__init__.py
 jaseci/extens/act_lib/tests/std_test_code.py
 jaseci/extens/act_lib/tests/test_date.py
 jaseci/extens/act_lib/tests/test_elastic.py
+jaseci/extens/act_lib/tests/test_file.py
 jaseci/extens/act_lib/tests/test_file_lib.py
 jaseci/extens/act_lib/tests/test_mail_lib.py
 jaseci/extens/act_lib/tests/test_maths.py
 jaseci/extens/act_lib/tests/test_net_lib.py
 jaseci/extens/act_lib/tests/test_regex.py
 jaseci/extens/act_lib/tests/test_std.py
 jaseci/extens/act_lib/tests/test_std_lib.py
@@ -81,14 +84,15 @@
 jaseci/extens/api/tests/test_walker_api.py
 jaseci/extens/svc/__init__.py
 jaseci/extens/svc/elastic_svc.py
 jaseci/extens/svc/kube_svc.py
 jaseci/extens/svc/mail_svc.py
 jaseci/extens/svc/prome_svc.py
 jaseci/extens/svc/redis_svc.py
+jaseci/extens/svc/storage_svc.py
 jaseci/extens/svc/stripe_svc.py
 jaseci/extens/svc/task_svc.py
 jaseci/extens/svc/tasks.py
 jaseci/jac/__init__.py
 jaseci/jac/jac.g4
 jaseci/jac/jac_set.py
 jaseci/jac/interpreter/__init__.py
@@ -153,25 +157,27 @@
 jaseci/prim/graph.py
 jaseci/prim/master.py
 jaseci/prim/node.py
 jaseci/prim/obj_mixins.py
 jaseci/prim/sentinel.py
 jaseci/prim/super_master.py
 jaseci/prim/walker.py
+jaseci/svc/__init__.py
 jaseci/tests/__init__.py
 jaseci/tests/infer.py
 jaseci/tests/jac_test_code.py
 jaseci/tests/jac_test_progs.py
 jaseci/tests/test_core.py
 jaseci/tests/test_jac.py
 jaseci/tests/test_node.py
 jaseci/tests/test_progs.py
 jaseci/tests/test_stack.py
 jaseci/tests/test_stripe.py
 jaseci/utils/__init__.py
+jaseci/utils/file_handler.py
 jaseci/utils/gprof2dot.py
 jaseci/utils/id_list.py
 jaseci/utils/json_handler.py
 jaseci/utils/log_utils.py
 jaseci/utils/test_core.py
 jaseci/utils/utils.py
 jaseci/utils/actions/__init__.py
```

### Comparing `jaseci-1.4.1.7/setup.py` & `jaseci-1.4.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "psycopg2-binary==2.9.5",
         "pygls",
         "mock",
         "beautifulsoup4>=4.12.2, <4.13.0",
         "lxml>=4.9.2, <4.10.0",
         "html5lib>=1.1, <1.2",
         "prettytable>=3.7.0, <3.8.0",
+        "apache-libcloud==3.7.0",
     ],
     package_data={
         "": ["*.ini", "*.yaml", "jac.g4", "VERSION"],
     },
     entry_points={
         "console_scripts": [
             "jsctl = jaseci.cli_tools.jsctl:jsctl",
```

