# Comparing `tmp/yyxx_game_pkg-2023.7.6.1.tar.gz` & `tmp/yyxx_game_pkg-2023.7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.7.6.1.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.7.6.2.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.7.6.1.tar` & `yyxx_game_pkg-2023.7.6.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     4895 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/README.md
--rw-r--r--   0        0        0     1945 2023-07-06 06:28:53.398334 yyxx_game_pkg-2023.7.6.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0      124 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/__init__.py
--rw-r--r--   0        0        0     5166 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/Operator.py
--rw-r--r--   0        0        0     1505 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/OperatorServer.py
--rw-r--r--   0        0        0     2572 2023-07-06 06:28:42.506160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/RechargeConfig.py
--rw-r--r--   0        0        0     2600 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/TableFieldConf.py
--rw-r--r--   0        0        0      124 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/__init__.py
--rw-r--r--   0        0        0      124 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/__init__.py
--rw-r--r--   0        0        0     4353 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/check_token.py
--rw-r--r--   0        0        0     5805 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/map_core.py
--rw-r--r--   0        0        0     3506 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/recharge.py
--rw-r--r--   0        0        0     6894 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/conf/__init__.py
--rw-r--r--   0        0        0     2053 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/conf/global_settings.py
--rw-r--r--   0        0        0      128 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/aes.py
--rw-r--r--   0        0        0     1113 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/basic.py
--rw-r--r--   0        0        0     1351 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/make_sign.py
--rw-r--r--   0        0        0     2652 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/rsa.py
--rw-r--r--   0        0        0       83 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1304 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5596 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      149 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/__init__.py
--rw-r--r--   0        0        0     3443 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
--rw-r--r--   0        0        0      326 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
--rw-r--r--   0        0        0    10527 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
--rw-r--r--   0        0        0     7993 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
--rw-r--r--   0        0        0     3955 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2722 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     3215 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/op_helper.py
--rw-r--r--   0        0        0     1266 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2966 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-07-06 06:28:42.510160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0      666 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/formatters.py
--rw-r--r--   0        0        0     3467 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.570160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0      428 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/__init__.py
--rw-r--r--   0        0        0      132 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/cookiecutter.json
--rw-r--r--   0        0        0     4023 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
--rw-r--r--   0        0        0      624 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
--rw-r--r--   0        0        0     4077 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
--rw-r--r--   0        0        0       83 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5650 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     3135 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/error_code.py
--rw-r--r--   0        0        0     2845 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     9461 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     7441 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     2092 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xfutures.py
--rw-r--r--   0        0        0     3653 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0      573 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xstring.py
--rw-r--r--   0        0        0       69 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/__init__.py
--rw-r--r--   0        0        0     2669 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/middleware.py
--rw-r--r--   0        0        0       71 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/util/__init__.py
--rw-r--r--   0        0        0      564 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/util/common.py
--rw-r--r--   0        0        0      663 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/util/log_handlers.py
--rw-r--r--   0        0        0     1994 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/flask/__init__.py
--rw-r--r--   0        0        0     2969 2023-07-06 06:28:42.574160 yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     7116 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.7.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/README.md
+-rw-r--r--   0        0        0     1945 2023-07-06 07:53:26.321999 yyxx_game_pkg-2023.7.6.2/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5805 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3506 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1351 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5596 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      149 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/__init__.py
+-rw-r--r--   0        0        0     3443 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
+-rw-r--r--   0        0        0      326 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
+-rw-r--r--   0        0        0    10527 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
+-rw-r--r--   0        0        0     7993 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
+-rw-r--r--   0        0        0     3955 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2722 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0      666 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/formatters.py
+-rw-r--r--   0        0        0     3467 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     4023 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4077 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5650 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     9461 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7441 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     2092 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xfutures.py
+-rw-r--r--   0        0        0     3653 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/__init__.py
+-rw-r--r--   0        0        0     2852 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/middleware.py
+-rw-r--r--   0        0        0       71 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/__init__.py
+-rw-r--r--   0        0        0      564 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/common.py
+-rw-r--r--   0        0        0      663 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/log_handlers.py
+-rw-r--r--   0        0        0     1994 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/flask/__init__.py
+-rw-r--r--   0        0        0     2969 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     7116 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.7.6.2/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.7.6.1/README.md` & `yyxx_game_pkg-2023.7.6.2/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/pyproject.toml` & `yyxx_game_pkg-2023.7.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.07.06.001"
+version = "v2023.07.06.002"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
```

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.7.6.2/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.7.6.2/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.7.6.2/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.7.6.2/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/test_logger.py` & `yyxx_game_pkg-2023.7.6.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/test_xtrace.py` & `yyxx_game_pkg-2023.7.6.2/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.7.6.2/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/Operator.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/Operator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/OperatorServer.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/OperatorServer.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/RechargeConfig.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/RechargeConfig.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/model/TableFieldConf.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/TableFieldConf.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/check_token.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/map_core.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/map_core.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/center_api/sdk/recharge.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/conf/__init__.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/conf/global_settings.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/aes.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/basic.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/basic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/make_sign.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/make_sign.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/crypto/rsa.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/das_api.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/mongo_op.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/op_helper.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/op_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/formatters.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/formatters.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/error_code.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/error_code.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdataframe.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xfutures.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xfutures.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xhttp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/utils/xstring.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xstring.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/__init__.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/middleware.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,48 +12,50 @@
 from yyxx_game_pkg.xtrace.django.util.common import get_django_middleware_setting
 
 
 class _DjangoJaegerMiddleware(MiddlewareMixin):
     _jaeger_config = getattr(settings, "JAEGER", {})
     _log_max_size = _jaeger_config.get("log_max_size", 2048)
     _is_log = _jaeger_config.get("is_log", False)
+    _ignore_paths = _jaeger_config.get("ignore_paths", [])
 
     def __call__(self, request):
         try:
             span = xtrace_helper.get_current_span()
-            span.update_name(f"{request.environ['REQUEST_METHOD']} {request.environ['PATH_INFO']}")
-            if getattr(request, "REQUEST", None):
-                request_params = dict(request.REQUEST)
-            else:
-                request_params = {}
-                request_params.update(request.GET)
-                request_params.update(request.POST)
-            span.add_event("request", {"params": json.dumps(request_params)[:self._log_max_size]})
+            path_info = request.environ['PATH_INFO']
+            span.update_name(f"{request.environ['REQUEST_METHOD']} {path_info}")
+            if path_info not in self._ignore_paths:
+                if getattr(request, "REQUEST", None):
+                    request_params = dict(request.REQUEST)
+                else:
+                    request_params = {}
+                    request_params.update(request.GET)
+                    request_params.update(request.POST)
+                span.add_event("request", {"params": json.dumps(request_params)[:self._log_max_size]})
         except Exception as e:
             print(e)
         return super().__call__(request)
 
     def process_response(self, request, response):
-        if self._is_log:
-            try:
+        try:
+            if self._is_log and (request.environ['PATH_INFO'] not in self._ignore_paths):
                 span = xtrace_helper.get_current_span()
                 admin_alias = getattr(getattr(request, "admin", None), "alias", None)
                 if admin_alias:
                     span.set_attributes({"request.admin.alias": admin_alias})
                 settings_middleware = getattr(settings, get_django_middleware_setting(), [])
                 if "django.middleware.gzip.GZipMiddleware" in settings_middleware and response.headers.get(
                         "Content-Encoding") == 'gzip':
-                    span.add_event("response",
-                                   {"params": gzip.decompress(response.content).decode()[:self._log_max_size]})
+                    span.add_event("response", {"params": gzip.decompress(response.content).decode()[:self._log_max_size]})
                 else:
                     span.add_event("response", {"params": response.content.decode()[:self._log_max_size]})
-                # inject trace parent to response header
-                TraceContextTextMapPropagator().inject(response.headers)
-            except Exception as e:
-                print(e)
+            # inject trace parent to response header
+            TraceContextTextMapPropagator().inject(response.headers)
+        except Exception as e:
+            print(e)
         return response
 
     def process_exception(self, request, exception):
         try:
             span = xtrace_helper.get_current_span()
             span.set_status(xtrace_helper.Status(xtrace_helper.StatusCode.ERROR, exception.__str__()))
         except Exception as e:
```

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/util/common.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/django/util/log_handlers.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/log_handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/flask/__init__.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.1/PKG-INFO` & `yyxx_game_pkg-2023.7.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg
-Version: 2023.7.6.1
+Version: 2023.7.6.2
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.7.6.1 Summary: yyxx
+Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.7.6.2 Summary: yyxx
 game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg License:
 MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: center-api Provides-Extra: server-
```

