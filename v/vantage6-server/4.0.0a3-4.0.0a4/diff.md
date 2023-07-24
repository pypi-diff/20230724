# Comparing `tmp/vantage6-server-4.0.0a3.tar.gz` & `tmp/vantage6-server-4.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.0.0a3.tar", last modified: Tue Jul 18 15:34:11 2023, max compression
+gzip compressed data, was "vantage6-server-4.0.0a4.tar", last modified: Mon Jul 24 13:22:28 2023, max compression
```

## Comparing `vantage6-server-4.0.0a3.tar` & `vantage6-server-4.0.0a4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.835274 vantage6-server-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:34:11.835274 vantage6-server-4.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.819273 vantage6-server-4.0.0a3/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   139499 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.811273 vantage6-server-4.0.0a3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.823273 vantage6-server-4.0.0a3/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.823273 vantage6-server-4.0.0a3/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.827273 vantage6-server-4.0.0a3/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.827273 vantage6-server-4.0.0a3/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.827273 vantage6-server-4.0.0a3/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/common/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    22359 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    28270 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    22580 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    32644 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-18 15:33:57.000000 vantage6-server-4.0.0a3/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:34:11.831273 vantage6-server-4.0.0a3/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 15:34:11.000000 vantage6-server-4.0.0a3/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139499 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.776587 vantage6-server-4.0.0a4/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.780588 vantage6-server-4.0.0a4/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18896 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28270 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22580 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32644 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-24 13:22:06.000000 vantage6-server-4.0.0a4/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:22:28.784588 vantage6-server-4.0.0a4/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 13:22:28.000000 vantage6-server-4.0.0a4/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.0.0a3/PKG-INFO` & `vantage6-server-4.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a4 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-4.0.0a3/setup.py` & `vantage6-server-4.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/tests_server/test_models.py` & `vantage6-server-4.0.0a4/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/tests_server/test_resources.py` & `vantage6-server-4.0.0a4/tests_server/test_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/__init__.py` & `vantage6-server-4.0.0a4/vantage6/server/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.0.0a4/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/_version.py` & `vantage6-server-4.0.0a4/vantage6/server/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # Module version
 version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
-  '.'+_specifier_[version_info[3]]+str(version_info[4])
+    _specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
 
 # Module version accessible using thomas.__version__
 __version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-server-4.0.0a3/vantage6/server/cli/server.py` & `vantage6-server-4.0.0a4/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/context.py` & `vantage6-server-4.0.0a4/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/controller/fixture.py` & `vantage6-server-4.0.0a4/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/db.py` & `vantage6-server-4.0.0a4/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/default_roles.py` & `vantage6-server-4.0.0a4/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/globals.py` & `vantage6-server-4.0.0a4/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/mail_service.py` & `vantage6-server-4.0.0a4/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/__init__.py` & `vantage6-server-4.0.0a4/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.0.0a4/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/authenticatable.py` & `vantage6-server-4.0.0a4/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/base.py` & `vantage6-server-4.0.0a4/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/collaboration.py` & `vantage6-server-4.0.0a4/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/common/utils.py` & `vantage6-server-4.0.0a4/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/member.py` & `vantage6-server-4.0.0a4/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/node.py` & `vantage6-server-4.0.0a4/vantage6/server/model/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         session = DatabaseSessionManager.get_session()
 
         result = session.query(cls).filter_by(status='online').all()
         session.commit()
         return result
 
     @classmethod
-    def exists(cls, organization_id: int, collaboration_id: int) -> bool:
+    def exists_by_id(cls, organization_id: int, collaboration_id: int) -> bool:
         """
         Check if a node exists for the given organization and collaboration.
 
         Parameters
         ----------
         organization_id : int
             The id of the organization
```

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/node_config.py` & `vantage6-server-4.0.0a4/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/organization.py` & `vantage6-server-4.0.0a4/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/permission.py` & `vantage6-server-4.0.0a4/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/role.py` & `vantage6-server-4.0.0a4/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/rule.py` & `vantage6-server-4.0.0a4/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/run.py` & `vantage6-server-4.0.0a4/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/task.py` & `vantage6-server-4.0.0a4/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/task_database.py` & `vantage6-server-4.0.0a4/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/model/user.py` & `vantage6-server-4.0.0a4/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/permission.py` & `vantage6-server-4.0.0a4/vantage6/server/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/__init__.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/collaboration.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/common/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/common/pagination.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/common/pagination.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/event.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/health.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/node.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,25 +347,25 @@
         # collaboration
         if not (organization in collaboration.organizations):
             return {'msg': f'The organization id={org_id} is not part of '
                     f'collabotation id={collaboration.id}. Add it first!'}, \
                         HTTPStatus.BAD_REQUEST
 
         # verify that this node does not already exist
-        if db.Node.exists(organization.id, collaboration.id):
+        if db.Node.exists_by_id(organization.id, collaboration.id):
             return {'msg': f'Organization id={organization.id} already has a '
                     f'node for collaboration id={collaboration.id}'}, \
                         HTTPStatus.BAD_REQUEST
 
         # if no name is provided, generate one
         name = data['name'] if 'name' in data else \
             f"{organization.name} - {collaboration.name} Node"
         if db.Node.exists("name", name):
             return {
-                "msg": f"Node name '{name}' already exists!"
+                "msg": f"Node with name '{name}' already exists!"
             }, HTTPStatus.BAD_REQUEST
 
         # Ok we're good to go!
         api_key = str(uuid.uuid4())
         node = db.Node(
             name=name,
             collaboration=collaboration,
@@ -611,15 +611,16 @@
                             f'={collaboration.id}'}
 
             node.collaboration = collaboration
 
         # validate that node does not already exist when we change either
         # the organization and/or collaboration
         if updated_org or updated_col:
-            if db.Node.exists(node.organization.id, node.collaboration.id):
+            if db.Node.exists_by_id(node.organization.id,
+                                    node.collaboration.id):
                 return {'msg': 'A node with organization id='
                         f'{node.organization.id} and collaboration id='
                         f'{node.collaboration.id} already exists!'}, \
                             HTTPStatus.BAD_REQUEST
 
         # update node IP address if it is given
         ip = data.get('ip')
```

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/organization.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/port.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/recover.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/result.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/role.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/rule.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/run.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/stats.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/task.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/token.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/user.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/version.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/vpn.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.0.0a4/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/utils.py` & `vantage6-server-4.0.0a4/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6/server/websockets.py` & `vantage6-server-4.0.0a4/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.0.0a3/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.0.0a4/vantage6_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.0.0a3
+Version: 4.0.0a4
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.0.0a4 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-4.0.0a3/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.0.0a4/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

