# Comparing `tmp/meili-sdk-0.5.7.tar.gz` & `tmp/meili-sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.5.7.tar", last modified: Thu Apr 20 12:52:04 2023, max compression
+gzip compressed data, was "meili-sdk-0.6.0.tar", last modified: Mon Jul 24 14:07:02 2023, max compression
```

## Comparing `meili-sdk-0.5.7.tar` & `meili-sdk-0.6.0.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.136443 meili-sdk-0.5.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5035 2023-04-20 12:52:04.136443 meili-sdk-0.5.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.116274 meili-sdk-0.5.7/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.120858 meili-sdk-0.5.7/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.121775 meili-sdk-0.5.7/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.125442 meili-sdk-0.5.7/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.126358 meili-sdk-0.5.7/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8383 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.129109 meili-sdk-0.5.7/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.131859 meili-sdk-0.5.7/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.133692 meili-sdk-0.5.7/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.134609 meili-sdk-0.5.7/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14306 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.136443 meili-sdk-0.5.7/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     6253 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/meili_sdk/websockets/models/traffic_control_action_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:52:04.119025 meili-sdk-0.5.7/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5035 2023-04-20 12:52:04.000000 meili-sdk-0.5.7/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-20 12:52:04.000000 meili-sdk-0.5.7/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 12:52:04.000000 meili-sdk-0.5.7/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-20 12:52:04.000000 meili-sdk-0.5.7/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 12:52:04.000000 meili-sdk-0.5.7/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-04-20 12:52:04.137359 meili-sdk-0.5.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-20 12:51:51.000000 meili-sdk-0.5.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.957427 meili-sdk-0.6.0/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.958427 meili-sdk-0.6.0/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.959427 meili-sdk-0.6.0/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.960427 meili-sdk-0.6.0/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.961427 meili-sdk-0.6.0/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.962427 meili-sdk-0.6.0/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.963427 meili-sdk-0.6.0/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.964427 meili-sdk-0.6.0/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.965427 meili-sdk-0.6.0/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15825 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.967427 meili-sdk-0.6.0/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6253 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/meili_sdk/websockets/models/update_map_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:02.957427 meili-sdk-0.6.0/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 14:07:02.000000 meili-sdk-0.6.0/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-24 14:07:02.968427 meili-sdk-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-24 14:06:54.000000 meili-sdk-0.6.0/setup.py
```

### Comparing `meili-sdk-0.5.7/LICENSE.txt` & `meili-sdk-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/PKG-INFO` & `meili-sdk-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.5.7
+Version: 0.6.0
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Rimvydas Zilinskas
 Author-email: rimvydas@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.5.7/README.md` & `meili-sdk-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/clients/__init__.py` & `meili-sdk-0.6.0/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.6.0/meili_sdk/clients/apitoken_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __all__ = ("APITokenClient",)
 
 logger = logging.getLogger("meili")
 
 
 class APITokenClient(BaseAPIClient):
-    AUTHORIZATION_TOKEN_HEADER = "Token"  # nosec
+    AUTHORIZATION_TOKEN_HEADER = "Bearer"  # nosec
 
     def __init__(self, *args, **kwargs):
         logging.warning(
             "This client is about to be deprecated, please use PersistentTokenClient instead"
         )
         super().__init__(*args, **kwargs)
```

### Comparing `meili-sdk-0.5.7/meili_sdk/clients/base.py` & `meili-sdk-0.6.0/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.6.0/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/exceptions.py` & `meili-sdk-0.6.0/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/base.py` & `meili-sdk-0.6.0/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/form.py` & `meili-sdk-0.6.0/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/task.py` & `meili-sdk-0.6.0/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/team.py` & `meili-sdk-0.6.0/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/trigger.py` & `meili-sdk-0.6.0/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/models/vehicle.py` & `meili-sdk-0.6.0/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/client.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,17 +81,17 @@
         resource = client.get_ros_resources()
         token = resource.get_token(setup_uuid)
         _, setup, _, _ = resource.get_ros_setup(setup_uuid)
         return cls(
             client_id=setup.mqtt_id, token=token, setup_uuid=setup_uuid, *args, *kwargs
         )
 
-    def subscribe_default_topics(self, vehicle_uuid):
-        self.subscribe_to_orders(vehicle_uuid)
-        self.subscribe_to_actions(vehicle_uuid)
+    def subscribe_default_topics(self, vehicle_serial_number, manufacturer = "meili"):
+        self.subscribe_to_orders(vehicle_serial_number, manufacturer=manufacturer)
+        self.subscribe_to_actions(vehicle_serial_number, manufacturer=manufacturer)
 
     def run(self, block=False):
         try:
             self.connection_state = MqttConnectionStatus.CONNECTING
             self.client.connect(
                 self.url, port=self.port, keepalive=True, bind_address=""
             )
@@ -135,18 +135,16 @@
             try:
                 message = json.dumps(message)
             except (TypeError, ValueError):
                 message = str(message)
 
         self.client.publish(topic=topic, payload=message, qos=qos)
 
-    def publish_to_state_topic(self, vehicle_uuid: str, message: any, qos=0):
-        if self.setup_uuid is None:
-            raise ValueError("Cannot build topics without setup_uuid provided")
-        topic = f"meili/setup/{self.setup_uuid}/vehicle/{vehicle_uuid}/state"
+    def publish_to_state_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/state"
         return self.publish(topic, message, qos)
 
     def wait_for_connection(self, timeout=10):
         """
         Block execution until connection is established
 
         If connection is still closed after timeout provided, it will raise TimeoutError
@@ -165,20 +163,20 @@
             and (datetime.now() - start_time).seconds < timeout
         ):
             continue
 
         if self.connection_state != MqttConnectionStatus.CONNECTED:
             raise TimeoutError("Timed out")
 
-    def subscribe_to_actions(self, vehicle_uuid: str):
-        topic = f"meili/vehicle/{vehicle_uuid}/actions"
+    def subscribe_to_actions(self, vehicle_serial_number: str, manufacturer: str = "meili"):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/instantactions"
         return self.subscribe(topic)
 
-    def subscribe_to_orders(self, vehicle_uuid):
-        topic = f"meili/vehicle/{vehicle_uuid}/orders"
+    def subscribe_to_orders(self, vehicle_serial_number: str, manufacturer: str = "meili"):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/order"
         return self.subscribe(topic)
 
     def __check_connection(self, custom_message=None):
         if not self.client.is_connected():
             raise ConnectionError(custom_message or "Connection is closed")
 
     def __on_connect(self, client: _Client, _: t.Optional[dict], flags: dict, rc: int):
```

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/models/state.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/mqtt/site.py` & `meili-sdk-0.6.0/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/base.py` & `meili-sdk-0.6.0/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/forms.py` & `meili-sdk-0.6.0/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/organizations.py` & `meili-sdk-0.6.0/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/tasks.py` & `meili-sdk-0.6.0/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/teams.py` & `meili-sdk-0.6.0/meili_sdk/resources/teams.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 
     def update_team(self, team):
         return self.patch(f"api/teams/{team.uuid}/", data=team, expected_class=Team)
 
     def delete_team(self, team):
         return self.delete(f"api/teams/{team.uuid}/")
 
+    def get_indoor_area_map(self,team):
+        return self.get(f"api/teams/{team.uuid}/indoors/area/images/")
+
+    def get_indoor_team_area(self,team):
+        return self.get(f"api/teams/{team.uuid}/indoors/area/")
+
+
 
 class SDKTeamResource(BaseResource):
     def get_teams(self):
         return self.get("sdk/teams/", expected_class=Team)
 
     def update_team(self, team):
         return self.patch(f"sdk/teams/{team.uuid}/", data=team, expected_class=Team)
```

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/triggers.py` & `meili-sdk-0.6.0/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/resources/vehicles.py` & `meili-sdk-0.6.0/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/schedules/loader.py` & `meili-sdk-0.6.0/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/schedules/models.py` & `meili-sdk-0.6.0/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/site.py` & `meili-sdk-0.6.0/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/websockets/client.py` & `meili-sdk-0.6.0/meili_sdk/websockets/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 
 from meili_sdk.exceptions import MeiliException, WebsocketException
 from meili_sdk.resources.base import BaseResource
 from meili_sdk.site import get_host
 from meili_sdk.version import VERSION
 from meili_sdk.websockets import constants
 from meili_sdk.websockets.models import DockingRoutineMessage
+from meili_sdk.websockets.models.update_map_message import UpdateMapMessage
 from meili_sdk.websockets.models.message import Message
 from meili_sdk.websockets.models.move_message import MoveMessage
 from meili_sdk.websockets.models.task import process_task_message
+from meili_sdk.websockets.models.task_v2 import process_task_v2_message
 from meili_sdk.websockets.models.topic import RosTopic
+from meili_sdk.websockets.models.cancel_task_message import CancelTaskMessage
 from meili_sdk.websockets.models.traffic_control_action_message import (
     PathReroutingMessage,
     SlowDownMessage,
     process_clearance_data,
 )
+import datetime
 
 logger = logging.getLogger("meili_sdk")
 
 __all__ = ("MeiliWebsocketClient",)
 
 
 class MeiliWebsocketClient:
@@ -49,33 +53,36 @@
     """
 
     __vehicles = []
     __connection: t.Optional[websocket.WebSocketApp]
     thread: threading.Thread
 
     def __init__(
-        self,
-        token: str,
-        override_host: t.Optional[str] = None,
-        fleet: t.Optional[bool] = True,
-        open_handler: t.Optional[t.Callable] = None,
-        close_handler: t.Optional[t.Callable] = None,
-        error_handler: t.Optional[t.Callable] = None,
-        docking_routine_request_handler: t.Optional[t.Callable] = None,
-        docking_routine_finalize_handler: t.Optional[t.Callable] = None,
-        task_handler: t.Optional[t.Callable] = None,
-        task_cancellation_handler: t.Optional[t.Callable] = None,
-        move_action_handler: t.Optional[t.Callable] = None,
-        slow_down_handler: t.Optional[t.Callable] = None,
-        path_rerouting_handler: t.Optional[t.Callable] = None,
-        collision_clearance_handler: t.Optional[t.Callable] = None,
-        topic_list_handler: t.Optional[t.Callable] = None,
-        topic_list_initializer_handler: t.Optional[t.Callable] = None,
-        fake_opened_connection: t.Optional[bool] = False,
-        message_error_handler: t.Optional[t.Callable] = None,
+            self,
+            token: str,
+            override_host: t.Optional[str] = None,
+            fleet: t.Optional[bool] = True,
+            open_handler: t.Optional[t.Callable] = None,
+            close_handler: t.Optional[t.Callable] = None,
+            error_handler: t.Optional[t.Callable] = None,
+            docking_routine_request_handler: t.Optional[t.Callable] = None,
+            docking_routine_finalize_handler: t.Optional[t.Callable] = None,
+            task_handler: t.Optional[t.Callable] = None,
+            task_v2_handler: t.Optional[t.Callable] = None,
+            task_cancellation_handler: t.Optional[t.Callable] = None,
+            move_action_handler: t.Optional[t.Callable] = None,
+            slow_down_handler: t.Optional[t.Callable] = None,
+            path_rerouting_handler: t.Optional[t.Callable] = None,
+            collision_clearance_handler: t.Optional[t.Callable] = None,
+            topic_list_handler: t.Optional[t.Callable] = None,
+            topic_list_initializer_handler: t.Optional[t.Callable] = None,
+            fake_opened_connection: t.Optional[bool] = False,
+            message_error_handler: t.Optional[t.Callable] = None,
+            update_map_handler: t.Optional[t.Callable] = None,
+
     ) -> None:
         self.token = token
         self.__connection_is_open = fake_opened_connection
         self.__fleet = fleet
 
         host = override_host or get_host()
         self.url = BaseResource.build_url(
@@ -85,22 +92,24 @@
         self.__open_handler = open_handler
         self.__close_handler = close_handler
         self.__error_handler = error_handler
 
         self.__docking_routine_request_handler = docking_routine_request_handler
         self.__docking_routine_finalize_handler = docking_routine_finalize_handler
         self.__task_handler = task_handler
+        self.__task_v2_handler = task_v2_handler
         self.__task_cancellation_handler = task_cancellation_handler
         self.__move_handler = move_action_handler
         self.__slow_down_handler = slow_down_handler
         self.__path_rerouting_handler = path_rerouting_handler
         self.__collision_clearance_handler = collision_clearance_handler
         self.__topic_list_handler = topic_list_handler
         self.__topic_list_initializer_handler = topic_list_initializer_handler
         self.__message_error_handler = message_error_handler
+        self.__update_map_handler = update_map_handler
         self.__connection = None
 
     def get_headers(self) -> dict:
         return {
             "x-meili-app-name": "sdk",
             "x-meili-app-version": VERSION,
             "x-meili-fleet-token": self.token,
@@ -202,117 +211,140 @@
         if isinstance(message, Message):
             message = dict(message)
         if not isinstance(message, str):
             message = json.dumps(message)
         self.send_raw(message)
 
     def send_raw(self, message):
+
         self.__connection.send(message)
 
     def process_message(
-        self, action: str, message: dict, vehicle: t.Optional[str] = None
+            self, action: str, message: dict, vehicle: t.Optional[str] = None
     ):
         processors = {
             constants.ACTION_DOCKING_ROUTINE_REQUEST: self.process_docking_routine_request,
             constants.ACTION_DOCKING_ROUTINE_FINALIZE: self.process_docking_routine_finalize,
             constants.ACTION_TASK: self.process_task,
+            constants.ACTION_TASK_V2: self.process_task_v2,
             constants.ACTION_TASK_CANCELLATION: self.process_task_cancellation,
             constants.ACTION_MOVE: self.process_move,
             constants.ACTION_MOVE_TO_CHARGING_POINT: self.process_move,
             constants.ACTION_SLOW_DOWN: self.process_slow_down,
             constants.ACTION_PATH_REROUTING: self.process_path_rerouting,
             constants.ACTION_COLLISION_CLEARANCE: self.process_collision_clearance,
             constants.ACTION_TOPIC_LIST: self.process_request_for_topics,
             constants.ACTION_TOPIC_INITIALIZATION: self.process_topic_list,
+            constants.ACTION_UPDATE_MAP : self.process_update_map,
         }
         try:
             processor = processors[action]
         except KeyError:
             logger.warning(
                 f"Cannot handle action {action}. Maybe you are using an outdated library?"
             )
             return
 
         if processor and callable(processor):
             processor(message, vehicle)
+    def process_update_map(
+        self, message: dict, vehicle: t.Optional[str] = None
+    ):
+        update_map_message = UpdateMapMessage(**message["data"])
 
+        if self.__update_map_handler and callable(self.__update_map_handler):
+            self.__update_map_handler(update_map_message,vehicle)
     def process_docking_routine_request(
-        self, message: dict, vehicle: t.Optional[str] = None
+            self, message: dict, vehicle: t.Optional[str] = None
     ):
         dock_message = DockingRoutineMessage(**message["data"])
         if self.__docking_routine_request_handler and callable(
-            self.__docking_routine_request_handler
+                self.__docking_routine_request_handler
         ):
             self.__docking_routine_request_handler(dock_message, vehicle)
 
     def process_docking_routine_finalize(
-        self, message: dict, vehicle: t.Optional[str] = None
+            self, message: dict, vehicle: t.Optional[str] = None
     ):
         dock_message = DockingRoutineMessage(**message["data"])
         if self.__docking_routine_finalize_handler and callable(
-            self.__docking_routine_finalize_handler
+                self.__docking_routine_finalize_handler
         ):
             self.__docking_routine_finalize_handler(dock_message, vehicle)
 
     def process_task(self, message: dict, vehicle: t.Optional[str] = None):
         """
         Load task to a Python object and pass it to task handler provided in the __init__
         method by implementers if applicable
         """
         task_data = message["data"]
         task = process_task_message(task_data)
 
         if self.__task_handler and callable(self.__task_handler):
             self.__task_handler(task, task_data, vehicle)
 
+    def process_task_v2(self, message: dict, vehicle: t.Optional[str] = None):
+        """
+        Load task to a Python object and pass it to task handler provided in the __init__
+        method by implementers if applicable
+        """
+        task_data = message["data"]
+        task = process_task_v2_message(task_data)
+
+        if self.__task_v2_handler and callable(self.__task_v2_handler):
+            self.__task_v2_handler(task, vehicle)
+
     def process_task_cancellation(self, message: dict, vehicle: t.Optional[str] = None):
+        task_cancel = CancelTaskMessage(**message["data"])
+
         if self.__task_cancellation_handler and callable(
-            self.__task_cancellation_handler
+                self.__task_cancellation_handler
         ):
-            self.__task_cancellation_handler(message.get("goal_id", None), vehicle)
+            self.__task_cancellation_handler(task_cancel, vehicle)
 
     def process_move(self, message: dict, vehicle: t.Optional[str] = None):
-        move_message = MoveMessage(**message)
+        move_message = MoveMessage(**message["data"])
         if self.__move_handler and callable(self.__move_handler):
             self.__move_handler(move_message, message, vehicle)
 
     def process_slow_down(self, message: dict, vehicle: t.Optional[str] = None):
         slow_down = SlowDownMessage(**message["data"])
         if self.__slow_down_handler and callable(self.__slow_down_handler):
             self.__slow_down_handler(slow_down, message, vehicle)
 
     def process_path_rerouting(self, message: dict, vehicle: t.Optional[str] = None):
         path_rerouting = PathReroutingMessage(**message)
         if self.__path_rerouting_handler and callable(self.__path_rerouting_handler):
             self.__path_rerouting_handler(path_rerouting, message, vehicle)
 
     def process_collision_clearance(
-        self, message: dict, vehicle: t.Optional[str] = None
+            self, message: dict, vehicle: t.Optional[str] = None
     ):
+
         collision_message = message["data"]
         clear_collision = process_clearance_data(collision_message)
         if self.__collision_clearance_handler and callable(
-            self.__collision_clearance_handler
+                self.__collision_clearance_handler
         ):
             self.__collision_clearance_handler(clear_collision, message, vehicle)
 
     def process_request_for_topics(
-        self, message: dict, vehicle: t.Optional[str] = None
+            self, message: dict, vehicle: t.Optional[str] = None
     ):
         if self.__topic_list_handler and callable(self.__topic_list_handler):
             self.__topic_list_handler(message, vehicle)
 
     def process_topic_list(self, message: dict, vehicle: t.Optional[str] = None):
         topics = []
 
         for topic in message.get("data", []):
             topics.append(RosTopic(**topic))
 
         if self.__topic_list_initializer_handler and callable(
-            self.__topic_list_initializer_handler
+                self.__topic_list_initializer_handler
         ):
             self.__topic_list_initializer_handler(topics, message, vehicle)
 
     def process_message_error(self, message: dict):
         logger.warning(
             f"Validation failed for message with the following errors: {message}"
         )
```

### Comparing `meili-sdk-0.5.7/meili_sdk/websockets/constants.py` & `meili-sdk-0.6.0/meili_sdk/websockets/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,34 +22,38 @@
     EVENT_PATH_DATA,
 )
 
 # Incoming actions
 ACTION_DOCKING_ROUTINE_REQUEST = "docking_routine_request"
 ACTION_DOCKING_ROUTINE_FINALIZE = "docking_routine_finalize_request"
 ACTION_TASK = "task"
+ACTION_TASK_V2 = "taskv2"
 ACTION_TASK_CANCELLATION = "cancelOrder"
 ACTION_MOVE = "move"
 ACTION_MOVE_TO_CHARGING_POINT = "move_charge"
 ACTION_SLOW_DOWN = "slow_down"
 ACTION_TOPIC_LIST = "request_topics"
 ACTION_TOPIC_INITIALIZATION = "topic_init"
 ACTION_ERROR = "errors"
 ACTION_PATH_REROUTING = "path_rerouting"
 ACTION_COLLISION_CLEARANCE = "clear_collision"
+ACTION_UPDATE_MAP = "update_maps"
 
 ALL_ACTIONS = (
     ACTION_DOCKING_ROUTINE_REQUEST,
     ACTION_DOCKING_ROUTINE_FINALIZE,
     ACTION_TASK,
+    ACTION_TASK_V2,
     ACTION_MOVE,
     ACTION_MOVE_TO_CHARGING_POINT,
     ACTION_SLOW_DOWN,
     ACTION_PATH_REROUTING,
     ACTION_TOPIC_LIST,
     ACTION_TOPIC_INITIALIZATION,
     ACTION_ERROR,
+    ACTION_UPDATE_MAP
 )
 
 IGNORED_TYPES = (
     "initialized",
     "not_initialized",
 )
```

### Comparing `meili-sdk-0.5.7/meili_sdk/websockets/models/message.py` & `meili-sdk-0.6.0/meili_sdk/websockets/models/message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/websockets/models/task.py` & `meili-sdk-0.6.0/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.5.7/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.6.0/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from meili_sdk.models.base import BaseModel
 from meili_sdk.websockets.models.task import BatchedTask, Task, process_task_message
 
 __all__ = (
     "SlowDownMessage",
     "PathReroutingMessage",
     "process_clearance_data",
+    "SingleCollisionClearanceMessage",
+    "CollisionClearanceMessage"
 )
 
 
 def process_clearance_data(message):
     if "task_data" in message:
         message["task_data"] = process_task_message(message["task_data"])
         return CollisionClearanceMessage(**message)
```

### Comparing `meili-sdk-0.5.7/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.6.0/meili_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.5.7
+Version: 0.6.0
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Rimvydas Zilinskas
 Author-email: rimvydas@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.5.7/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.6.0/meili_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 meili_sdk/mqtt/models/__init__.py
 meili_sdk/mqtt/models/action.py
 meili_sdk/mqtt/models/order.py
 meili_sdk/mqtt/models/state.py
 meili_sdk/resources/__init__.py
 meili_sdk/resources/base.py
 meili_sdk/resources/forms.py
+meili_sdk/resources/maps.py
 meili_sdk/resources/organizations.py
 meili_sdk/resources/ros.py
 meili_sdk/resources/tasks.py
 meili_sdk/resources/teams.py
 meili_sdk/resources/triggers.py
 meili_sdk/resources/users.py
 meili_sdk/resources/vehicles.py
@@ -52,13 +53,16 @@
 meili_sdk/schedules/exceptions.py
 meili_sdk/schedules/loader.py
 meili_sdk/schedules/models.py
 meili_sdk/websockets/__init__.py
 meili_sdk/websockets/client.py
 meili_sdk/websockets/constants.py
 meili_sdk/websockets/models/__init__.py
+meili_sdk/websockets/models/cancel_task_message.py
 meili_sdk/websockets/models/docking_routine_message.py
 meili_sdk/websockets/models/message.py
 meili_sdk/websockets/models/move_message.py
 meili_sdk/websockets/models/task.py
+meili_sdk/websockets/models/task_v2.py
 meili_sdk/websockets/models/topic.py
-meili_sdk/websockets/models/traffic_control_action_message.py
+meili_sdk/websockets/models/traffic_control_action_message.py
+meili_sdk/websockets/models/update_map_message.py
```

### Comparing `meili-sdk-0.5.7/setup.cfg` & `meili-sdk-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.5.7
+version = 0.6.0
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rimvydas Zilinskas
 author_email = rimvydas@meilirobots.com
```

