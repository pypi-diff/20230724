# Comparing `tmp/jaseci_serv-1.4.1.7.tar.gz` & `tmp/jaseci_serv-1.4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci_serv-1.4.1.7.tar", last modified: Thu Jul 20 04:02:45 2023, max compression
+gzip compressed data, was "jaseci_serv-1.4.1.8.tar", last modified: Mon Jul 24 17:00:59 2023, max compression
```

## Comparing `jaseci_serv-1.4.1.7.tar` & `jaseci_serv-1.4.1.8.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.696066 jaseci_serv-1.4.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 04:02:45.696066 jaseci_serv-1.4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.676066 jaseci_serv-1.4.1.7/jaseci_serv/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/jaseci_serv/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/discussion_analysis.jac
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/flight_chatbot.jac
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/flow_analysis.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/restaurant_chatbot.jac
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/sentence_pairing.jac
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/virtual_assistant.jac
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/jsorc_loadtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/jaseci_serv/base/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/createdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/dropdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/wait_for_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.688065 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/aitest_ai_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/mock_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_orm_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_orm_hooks_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.688065 jaseci_serv-1.4.1.7/jaseci_serv/hook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/hook/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.688065 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.688065 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/async_update.jac
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/general.jac
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/ll.jac
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/ll_wall.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/object_bug.jac
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/public.jac
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/public_updated.jac
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    76005 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_ll_wall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_pub_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/try-syntax.jac
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/various.jac
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/zsb.jac
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jac_api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3514 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/tests/test_social_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/tests/test_obj_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/obj_api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/studio/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/studio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/studio/tests/test_studio_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/studio/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/studio/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/svc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/task_svc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/svc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/tests/test_task_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/svc/tests/testing.jac
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.692065 jaseci_serv-1.4.1.7/jaseci_serv/user_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/user_api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jaseci_serv/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.676066 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 04:02:45.000000 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-20 04:02:45.000000 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:02:45.000000 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 04:02:45.000000 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 04:02:45.000000 jaseci_serv-1.4.1.7/jaseci_serv.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/jsserv
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:02:45.696066 jaseci_serv-1.4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.672066 jaseci_serv-1.4.1.7/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.676066 jaseci_serv-1.4.1.7/static/studio/
--rw-r--r--   0 runner    (1001) docker     (123)   217364 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/Jaseci-Submark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.672066 jaseci_serv-1.4.1.7/static/studio/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.672066 jaseci_serv-1.4.1.7/static/studio/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.676066 jaseci_serv-1.4.1.7/static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.680065 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    78281 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/113-f20cf828040267fc.js
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
--rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/3-d801e16fe6466f20.js
--rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/30-825cca92eb40c60a.js
--rw-r--r--   0 runner    (1001) docker     (123)    53501 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
--rw-r--r--   0 runner    (1001) docker     (123)   151456 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/707-69e1edf708a55a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
--rw-r--r--   0 runner    (1001) docker     (123)   141058 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
--rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/main-1844b67c68085ff6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.680065 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   287285 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js
--rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/webpack-620c68345e03c539.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.680065 jaseci_serv-1.4.1.7/static/studio/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/css/cc49d8d41e055bcd.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/static/studio/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/media/2e1b830192b7974a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/media/d607327a37a507c7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/_next/static/media/ebec2867f40f78ec.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 04:02:27.000000 jaseci_serv-1.4.1.7/static/studio/test.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.696066 jaseci_serv-1.4.1.7/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.696066 jaseci_serv-1.4.1.7/templates/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/templates/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-20 04:00:37.000000 jaseci_serv-1.4.1.7/templates/examples/social_auth.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:02:45.684065 jaseci_serv-1.4.1.7/templates/studio/
--rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/404.html
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/architype.html
--rw-r--r--   0 runner    (1001) docker     (123)    25538 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/emotion.html
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/graph-viewer.html
--rw-r--r--   0 runner    (1001) docker     (123)    33279 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-07-20 04:02:28.000000 jaseci_serv-1.4.1.7/templates/studio/logs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.673293 jaseci_serv-1.4.1.8/jaseci_serv/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/jaseci_serv/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/discussion_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/flight_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/flow_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/restaurant_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/sentence_pairing.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/virtual_assistant.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/jsorc_loadtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/jaseci_serv/base/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.685293 jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/createdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/dropdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/wait_for_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.685293 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/aitest_ai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/mock_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_orm_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_orm_hooks_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.685293 jaseci_serv-1.4.1.8/jaseci_serv/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/hook/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.685293 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/async_update.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/general.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/ll.jac
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/ll_wall.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/object_bug.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/public.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/public_updated.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77226 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_ll_wall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_pub_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/try-syntax.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/various.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/zsb.jac
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jac_api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3514 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/tests/test_social_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/tests/test_obj_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/obj_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/studio/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/studio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/studio/tests/test_studio_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/studio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/studio/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/task_svc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/svc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/tests/test_task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/svc/tests/testing.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.689293 jaseci_serv-1.4.1.8/jaseci_serv/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/jaseci_serv/user_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/user_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jaseci_serv/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.673293 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 17:00:59.000000 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-24 17:00:59.000000 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:00:59.000000 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-24 17:00:59.000000 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 17:00:59.000000 jaseci_serv-1.4.1.8/jaseci_serv.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/jsserv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.673293 jaseci_serv-1.4.1.8/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.677293 jaseci_serv-1.4.1.8/static/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)   217364 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/Jaseci-Submark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.673293 jaseci_serv-1.4.1.8/static/studio/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.673293 jaseci_serv-1.4.1.8/static/studio/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.677293 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    78281 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/113-f20cf828040267fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/3-d801e16fe6466f20.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/30-825cca92eb40c60a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    53501 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)   151456 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/707-69e1edf708a55a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141058 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/main-1844b67c68085ff6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.677293 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   287285 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/webpack-620c68345e03c539.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.677293 jaseci_serv-1.4.1.8/static/studio/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/css/cc49d8d41e055bcd.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/static/studio/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/media/2e1b830192b7974a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/media/d607327a37a507c7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/media/ebec2867f40f78ec.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/static/studio/_next/static/u7vhajvBe15o56dx6n_tS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-24 17:00:41.000000 jaseci_serv-1.4.1.8/static/studio/test.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.693293 jaseci_serv-1.4.1.8/templates/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/templates/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-24 16:58:50.000000 jaseci_serv-1.4.1.8/templates/examples/social_auth.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:00:59.681293 jaseci_serv-1.4.1.8/templates/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/architype.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25538 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/emotion.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/graph-viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33279 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-07-24 17:00:42.000000 jaseci_serv-1.4.1.8/templates/studio/logs.html
```

### Comparing `jaseci_serv-1.4.1.7/LICENSE` & `jaseci_serv-1.4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/__init__.py` & `jaseci_serv-1.4.1.8/jaseci_serv/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class JsOrcSettings(jss):
     ###############################################################################################################
     # -------------------------------------------------- JSORC -------------------------------------------------- #
     ###############################################################################################################
 
     JSORC_CONFIG = {
         "backoff_interval": 10,
-        "pre_loaded_services": ["redis", "prome", "mail", "task", "elastic"],
+        "pre_loaded_services": ["redis", "prome", "mail", "task", "elastic", "store"],
     }
 
     ###############################################################################################################
     # -------------------------------------------------- TASK --------------------------------------------------- #
     ###############################################################################################################
 
     TASK_CONFIG = {
```

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/admin.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/discussion_analysis.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/discussion_analysis.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/flight_chatbot.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/flight_chatbot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/flow_analysis.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/flow_analysis.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/restaurant_chatbot.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/restaurant_chatbot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/sentence_pairing.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/sentence_pairing.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/virtual_assistant.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/virtual_assistant.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/jsorc.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/jsorc_loadtest.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/jsorc_loadtest.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/createdb.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/createdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/dropdb.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/dropdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/management/commands/wait_for_db.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/management/commands/wait_for_db.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/models.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/aitest_ai_models.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/aitest_ai_models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/mock_redis.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/mock_redis.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_admin.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_commands.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_models.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_orm_hooks.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_orm_hooks.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/base/tests/test_orm_hooks_cfg.py` & `jaseci_serv-1.4.1.8/jaseci_serv/base/tests/test_orm_hooks_cfg.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/hook/orm.py` & `jaseci_serv-1.4.1.8/jaseci_serv/hook/orm.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/api.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/infer.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/ll.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/ll.jac`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             latest_day = spawn here walker::get_latest_day(before_date=date);
             new = spawn here ++> node::day;
             new.day = infer.day_from_date(date);
             if(latest_day) {
                 new.order = latest_day.order;
                 new.ll_version = latest_day.ll_version;
                 spawn latest_day walker::carry_forward(parent=new);
-                for i=0 to i<new.order.length by i+=1:
+                if new.order: for i=0 to i<new.order.length by i+=1:
                     new.order[i] = &(spawn new.order[i] walker::past_to_now);
                 take new;
             }
             else: take new;
         }
     day {
         day_node = here;
@@ -278,15 +278,15 @@
             here.status == 'canceled')): skip;
         new_workette = spawn here <+[past]+ node::workette;
         new_workette <+[parent]+ parent;
         new_workette := here;
         if(new_workette.is_ritual): new_workette.status="open";
         spawn -[parent]-> node::workette
             walker::carry_forward(parent=new_workette);
-        for i=0 to i<new_workette.order.length by i+=1:
+        if new_workette.order: for i=0 to i<new_workette.order.length by i+=1:
             new_workette.order[i] = &(spawn new_workette.order[i]
                                       walker::past_to_now);
     }
 }
 
 walker gen_rand_life {
     has num_workettes;
```

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/ll_wall.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/ll_wall.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/object_bug.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/object_bug.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_admin_api.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_admin_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_api.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1547,15 +1547,16 @@
         )
         payload = {"op": "walker_run", "name": "global_actions"}
         res = self.client.post(
             reverse(f'jac_api:{payload["op"]}'), payload, format="json"
         ).data
 
         self.assertFalse(res["success"])
-        self.assertEqual(payload, res["report"][4]["body"])
+        self.assertEqual(payload, res["report"][3]["body"])
+        self.assertIn("Global not defined - b", res["errors"][0])
 
     def test_multipart_json_file(self):
         """Test multipart using json file as ctx parameter"""
         zsb_file = open(os.path.dirname(__file__) + "/zsb.jac").read()
         payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
         self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
         with open(os.path.dirname(__file__) + "/test.json", "rb") as ctx:
@@ -1705,42 +1706,59 @@
         }
 
         res = self.client.post(reverse(f'jac_api:{"walker_run"}'), data=form).data
 
         self.assertTrue(res["success"])
         self.assertEqual({"sample": "sample"}, res["report"][0]["ctx"])
 
-    def test_multipart_with_additional_file(self):
+    def test_multipart_with_additional_files(self):
         """Test multipart with additional file"""
         zsb_file = open(os.path.dirname(__file__) + "/zsb.jac").read()
         payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
         self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
         with open(os.path.dirname(__file__) + "/test.json", "rb") as ctx, open(
             os.path.dirname(__file__) + "/test.json", "rb"
-        ) as ctx2:
+        ) as ctx2, open(os.path.dirname(__file__) + "/image.png", "rb") as ctx3:
             form = {
                 "name": "simple_with_file",
                 "ctx": ctx,
                 "nd": "active:graph",
                 "snt": "active:sentinel",
                 "fileTypeField": ctx2,
+                "binaryFile": ctx3,
             }
             res = self.client.post(reverse(f'jac_api:{"walker_run"}'), data=form).data
 
-        default_file = [
+        self.assertTrue(res["success"])
+        self.assertEqual("sample", res["report"][0])
+        self.assertTrue(res["report"][1])
+
+        uuid = res["report"][2]
+
+        self.assertEqual(
             {
+                "id": f"{uuid}",
                 "name": "test.json",
-                "base64": "eyJzYW1wbGUiOiJzYW1wbGUifQ==",
-                "content-type": "application/json",
-            }
-        ]
-
-        self.assertTrue(res["success"])
-        self.assertEqual(default_file, res["report"][0])
-        self.assertEqual(default_file, res["report"][1])
+                "content_type": "application/json",
+                "field": "fileTypeField",
+                "absolute_name": f"{uuid}-test.json",
+                "absolute_path": f"/tmp/{uuid}-test.json",
+                "persist": False,
+            },
+            res["report"][3],
+        )
+        self.assertEqual('{"sample":"sample"}', res["report"][4])
+        self.assertEqual({"sample": "sample"}, res["report"][5])
+        self.assertEqual('b\'{"sample":"sample"}\'', res["report"][6])
+        self.assertEqual("eyJzYW1wbGUiOiJzYW1wbGUifQ==", res["report"][7])
+
+        with open(os.path.dirname(__file__) + "/image.png", "rb") as img:
+            string_bytes = str(img.read())
+            self.assertEqual(string_bytes, res["report"][8])
+            self.assertEqual(string_bytes, res["report"][9])
 
     def test_multipart_custom_payload_with_additional_file(self):
         """Test multipart custom payload (non ctx format) with additional file"""
         zsb_file = open(os.path.dirname(__file__) + "/zsb.jac").read()
         payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
         self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
         with open(os.path.dirname(__file__) + "/test.json", "rb") as ctx:
@@ -1749,83 +1767,83 @@
                 "ctx": "",
                 "nd": "active:graph",
                 "snt": "active:sentinel",
                 "fileTypeField": ctx,
             }
             res = self.client.post(reverse(f'jac_api:{"walker_run"}'), data=form).data
 
-        default_file = [
+        self.assertTrue(res["success"])
+        self.assertTrue(res["report"][0])
+
+        uuid = res["report"][1]
+
+        self.assertEqual(
             {
+                "id": f"{uuid}",
                 "name": "test.json",
-                "base64": "eyJzYW1wbGUiOiJzYW1wbGUifQ==",
-                "content-type": "application/json",
-            }
-        ]
-
-        self.assertTrue(res["success"])
-        self.assertEqual(default_file, res["report"][2])
+                "content_type": "application/json",
+                "field": "fileTypeField",
+                "absolute_name": f"{uuid}-test.json",
+                "absolute_path": f"/tmp/{uuid}-test.json",
+                "persist": False,
+            },
+            res["report"][2],
+        )
+        self.assertEqual('{"sample":"sample"}', res["report"][3])
+        self.assertEqual({"sample": "sample"}, res["report"][4])
+        self.assertEqual('b\'{"sample":"sample"}\'', res["report"][5])
+        self.assertEqual("eyJzYW1wbGUiOiJzYW1wbGUifQ==", res["report"][6])
 
     def test_try_catch(self):
         """Test try catch triggers"""
         zsb_file = open(os.path.dirname(__file__) + "/try-syntax.jac").read()
         payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
         self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
 
         payload = {"op": "walker_run", "name": "walker_exception_no_try_else"}
         res = self.client.post(
             reverse(f'jac_api:{payload["op"]}'), payload, format="json"
         ).data
 
-        self.assertIn("in jac_try_exception", " ".join(res["stack_trace"]))
-        self.assertIn(
-            "raise TryException(self.jac_exception(e, jac_ast))",
-            " ".join(res["stack_trace"]),
-        )
-        self.assertIn(
-            "jaseci.jac.machine.machine_state.TryException: ",
-            " ".join(res["stack_trace"]),
-        )
         self.assertIn(
-            "zsb:walker_exception_no_try_else - line 6, col 20",
+            "zsb:walker_exception_no_try_else - line 6, col 19",
             res["errors"][0],
         )
 
         payload = {"op": "walker_run", "name": "walker_exception_with_try_else"}
         res = self.client.post(
             reverse(f'jac_api:{payload["op"]}'), payload, format="json"
         ).data
 
-        self.assertFalse("stack_trace" in res)
+        self.assertTrue("stack_trace" in res)
         self.assertEqual("walker_exception_with_try_else", res["report"][0]["name"])
         self.assertEqual(14, res["report"][0]["line"])
         self.assertEqual(23, res["report"][0]["col"])
         self.assertIn(
-            "zsb:walker_exception_with_try_else -"
-            " line 14, col 23 - rule atom_trailer - ",
+            "zsb:walker_exception_with_try_else - line 14, col 23 - rule ability_call - Invalid arguments {'args': ['invalidUrl'], 'kwargs': {}} to action call request.get! Valid paramters are (url: str, data: dict, header: dict).",
             res["errors"][0],
         )
 
         payload = {
             "op": "walker_run",
             "name": "walker_exception_with_try_else_multiple_line",
         }
 
         res = self.client.post(
             reverse(f'jac_api:{payload["op"]}'), payload, format="json"
         ).data
 
-        self.assertFalse("stack_trace" in res)
+        self.assertTrue("stack_trace" in res)
         self.assertEqual(
             "walker_exception_with_try_else_multiple_line", res["report"][0]["name"]
         )
         self.assertEqual(32, res["report"][0]["line"])
         self.assertEqual(23, res["report"][0]["col"])
         self.assertIn(
-            "zsb:walker_exception_with_try_else_multiple_line "
-            "- line 32, col 23 - rule atom_trailer - ",
+            "zsb:walker_exception_with_try_else_multiple_line - line 32, col 23 - rule ability_call - Invalid URL 'invalidUrl': No scheme supplied. Perhaps you meant https://invalidUrl?",
             res["errors"][0],
         )
 
     def quick_call(self, bywho, ops):
         return bywho.post(reverse(f'jac_api:{ops["op"]}'), ops, format="json")
 
     def test_walker_smart_yield(self):
```

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_jac_general.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_jac_general.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_ll.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_ll.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_ll_wall.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_ll_wall.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_logging.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/test_pub_walker.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/test_pub_walker.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/try-syntax.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/try-syntax.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/tests/various.jac` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/tests/various.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jac_api/views.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jac_api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
-from base64 import b64encode
 from io import BytesIO
 from tempfile import _TemporaryFileWrapper
 from time import time
 
+from django.http import FileResponse
 from knox.auth import TokenAuthentication
 from rest_framework.permissions import AllowAny, IsAdminUser, IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.prim.element import Element
+from jaseci.utils.file_handler import FileHandler
 from jaseci.utils.utils import logger, ColCodes as Cc
 from jaseci.utils.actions.actions_manager import ActionManager
 from jaseci_serv.base.models import Master as ServMaster
 from jaseci_serv.user_api import serializers as user_slzr
 
 # The limit for logging an object (request payload and response): 5MB
 # Will truncate in the logs if the object exceeds this limit
@@ -26,14 +27,32 @@
         super().__init__(*args, **kwargs)
         self.hook = master._h
         self.hook.commit_all_cache_sync()
 
     def close(self):
         super(JResponse, self).close()
         # Commit db changes after response to user
+        self.hook.clean_file_handler()
+        self.hook.commit(True)
+
+
+class JFileResponse(FileResponse):
+    def __init__(self, hook, file_id: str) -> None:
+        file_handler: FileHandler = hook.get_file_handler(file_id)
+        file_handler.close()
+        file_handler.open(mode="rb", encoding=None)
+
+        super().__init__(file_handler.buffer, filename=file_handler.name)
+
+        self.hook = hook
+        self.hook.commit_all_cache_sync()
+
+    def close(self) -> None:
+        super().close()
+        self.hook.clean_file_handler()
         self.hook.commit(True)
 
 
 class AbstractJacAPIView(APIView):
     """
     The builder set of Jaseci APIs
     """
@@ -127,51 +146,60 @@
                     req_data["ctx"] = json.loads(ctx.read().decode("utf-8"))
             elif "ctx" in req_data and type(req_data["ctx"]) is not dict:
                 req_data["ctx"] = json.loads(req_data["ctx"])
         except ValueError:
             logger.error("Invalid ctx format! Ignoring ctx parsing!")
 
     def proc_file_ctx(self, request, req_data):
+        hook = self.caller._h
         for key in request.FILES:
             req_data.pop(key)
             file_ref = (
                 req_data["ctx"]
                 if "ctx" in req_data and type(req_data["ctx"]) is dict
                 else req_data
             )
             file_ref[key] = []
 
             for file in request.FILES.getlist(key):
                 file_type = type(file.file)
                 if file_type is BytesIO:
-                    file_base64 = b64encode(file.file.getvalue()).decode("utf-8")
+                    file_ref[key].append(
+                        hook.add_file_handler(
+                            FileHandler.fromBytesIO(
+                                file.file, file.name, file.content_type, key
+                            )
+                        )
+                    )
                 elif file_type is _TemporaryFileWrapper:
-                    file_base64 = b64encode(file.file.read()).decode("utf-8")
-
-                if "file_base64" in vars():
                     file_ref[key].append(
-                        {
-                            "name": file.name,
-                            "base64": file_base64,
-                            "content-type": file.content_type,
-                        }
+                        hook.add_file_handler(
+                            FileHandler.fromTemporaryFileWrapper(
+                                file.file, file.name, file.content_type, key
+                            )
+                        )
                     )
 
     def proc_request_ctx(self, request, req_data, raw_req_data):
         user_slzr.requests_for_emails = request
+        hook = self.caller._h
         req_query = request.GET.dict()
         req_data.update(
             {
                 "_req_ctx": {
                     "method": request.method,
                     "headers": dict(request.headers),
                     "query": req_query,
                     "body": req_data.copy(),
-                },
-                "_raw_req_ctx": raw_req_data.decode("utf-8"),
+                    "raw": hook.add_file_handler(
+                        FileHandler.fromBytesIO(
+                            BytesIO(raw_req_data), "raw_request", None
+                        )
+                    ),
+                }
             }
         )
         req_data.update(req_query)
 
     def proc_request(self, request, **kwargs):
         """Parse request to field set"""
         raw_req_data = request.body
@@ -201,14 +229,16 @@
 
         self.start_time = time()
 
         req_data = (
             request.data.dict() if type(request.data) is not dict else request.data
         )
 
+        self.set_caller(request)
+
         self.proc_prime_ctx(request, req_data)
         self.proc_file_ctx(request, req_data)
         self.proc_request_ctx(request, req_data, raw_req_data)
 
         req_data.update(kwargs)
 
         self.cmd = req_data
@@ -228,20 +258,28 @@
     def issue_response(self, api_result):
         """Issue response from call"""
         # self.caller._h.commit()
         # return Response(api_result)
         # for i in self.caller._h.save_obj_list:
         #     self.caller._h.commit_obj_to_redis(i)
         status = self.pluck_status_code(api_result)
-        if (
-            isinstance(api_result, dict)
-            and "report_custom" in api_result.keys()
-            and api_result["report_custom"] is not None
-        ):
-            api_result = api_result["report_custom"]
+        if isinstance(api_result, dict):
+            if (
+                "report_custom" in api_result.keys()
+                and api_result["report_custom"] is not None
+            ):
+                return JResponse(
+                    self.caller, api_result["report_custom"], status=status
+                )
+            elif (
+                "report_file" in api_result.keys()
+                and api_result["report_file"] is not None
+            ):
+                return JFileResponse(self.caller._h, api_result["report_file"])
+
         return JResponse(self.caller, api_result, status=status)
 
 
 class AbstractAdminJacAPIView(AbstractJacAPIView):
     """
     The abstract base for Jaseci Admin APIs
     """
```

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/admin.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/models.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/models.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/tests/test_social_auth.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/tests/test_social_auth.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/urls.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/utils.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/jsx_oauth/views.py` & `jaseci_serv-1.4.1.8/jaseci_serv/jsx_oauth/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/obj_api/tests/test_obj_api.py` & `jaseci_serv-1.4.1.8/jaseci_serv/obj_api/tests/test_obj_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/obj_api/views.py` & `jaseci_serv-1.4.1.8/jaseci_serv/obj_api/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/settings.py` & `jaseci_serv-1.4.1.8/jaseci_serv/settings.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/studio/tests/test_studio_routes.py` & `jaseci_serv-1.4.1.8/jaseci_serv/studio/tests/test_studio_routes.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/studio/urls.py` & `jaseci_serv-1.4.1.8/jaseci_serv/studio/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/studio/views.py` & `jaseci_serv-1.4.1.8/jaseci_serv/studio/views.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/svc/mail_svc.py` & `jaseci_serv-1.4.1.8/jaseci_serv/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/svc/task_svc.py` & `jaseci_serv-1.4.1.8/jaseci_serv/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/svc/tests/test_task_svc.py` & `jaseci_serv-1.4.1.8/jaseci_serv/svc/tests/test_task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/urls.py` & `jaseci_serv-1.4.1.8/jaseci_serv/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/user_api/serializers.py` & `jaseci_serv-1.4.1.8/jaseci_serv/user_api/serializers.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/user_api/tests/test_user_api.py` & `jaseci_serv-1.4.1.8/jaseci_serv/user_api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/user_api/urls.py` & `jaseci_serv-1.4.1.8/jaseci_serv/user_api/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv/user_api/views.py` & `jaseci_serv-1.4.1.8/jaseci_serv/user_api/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     authentication_classes = (TokenAuthentication,)
     permission_classes = (permissions.IsAuthenticated,)
 
     def get_object(self):
         """Retrieve and return authenticated user"""
         return self.request.user
 
-    def put(self, request, *args, **kwargs):
+    def process_update(self, request, *args, **kwargs):
         user = request.user
         current_user = {
             "id": user.id,
             "email": user.email,
             "name": user.name,
             "is_activated": user.is_activated,
             "is_superuser": user.is_superuser,
@@ -130,14 +130,21 @@
                     "is_superuser": user["is_superuser"],
                 },
             }
             elastic.app.doc_activity(activity)
 
         return response
 
+    def put(self, request, *args, **kwargs):
+        return self.process_update(request, *args, **kwargs)
+
+    def patch(self, request, *args, **kwargs):
+        kwargs["partial"] = True
+        return self.process_update(request, *args, **kwargs)
+
 
 class LogoutAllUsersView(APIView):
     """
     Log out of all user sessions across all users
     I.E. deletes all auth tokens for all users
     """
```

### Comparing `jaseci_serv-1.4.1.7/jaseci_serv.egg-info/SOURCES.txt` & `jaseci_serv-1.4.1.8/jaseci_serv.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 jaseci_serv.egg-info/SOURCES.txt
 jaseci_serv.egg-info/dependency_links.txt
 jaseci_serv.egg-info/requires.txt
 jaseci_serv.egg-info/top_level.txt
 jaseci_serv/../static/studio/Jaseci-Submark.png
 jaseci_serv/../static/studio/react.svg
 jaseci_serv/../static/studio/test.css
-jaseci_serv/../static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js
-jaseci_serv/../static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js
 jaseci_serv/../static/studio/_next/static/chunks/113-f20cf828040267fc.js
 jaseci_serv/../static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
 jaseci_serv/../static/studio/_next/static/chunks/3-d801e16fe6466f20.js
 jaseci_serv/../static/studio/_next/static/chunks/30-825cca92eb40c60a.js
 jaseci_serv/../static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
 jaseci_serv/../static/studio/_next/static/chunks/707-69e1edf708a55a15.js
 jaseci_serv/../static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
@@ -41,14 +39,16 @@
 jaseci_serv/../static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
 jaseci_serv/../static/studio/_next/static/css/cc49d8d41e055bcd.css
 jaseci_serv/../static/studio/_next/static/media/2e1b830192b7974a.woff2
 jaseci_serv/../static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
 jaseci_serv/../static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
 jaseci_serv/../static/studio/_next/static/media/d607327a37a507c7.woff2
 jaseci_serv/../static/studio/_next/static/media/ebec2867f40f78ec.woff2
+jaseci_serv/../static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js
+jaseci_serv/../static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js
 jaseci_serv/../templates/examples/social_auth.html
 jaseci_serv/../templates/studio/404.html
 jaseci_serv/../templates/studio/actions.html
 jaseci_serv/../templates/studio/architype.html
 jaseci_serv/../templates/studio/dashboard.html
 jaseci_serv/../templates/studio/emotion.html
 jaseci_serv/../templates/studio/graph-viewer.html
@@ -144,16 +144,14 @@
 jaseci_serv/user_api/views.py
 jaseci_serv/user_api/tests/__init__.py
 jaseci_serv/user_api/tests/test_user_api.py
 templates/__init__.py
 templates/../static/studio/Jaseci-Submark.png
 templates/../static/studio/react.svg
 templates/../static/studio/test.css
-templates/../static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js
-templates/../static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js
 templates/../static/studio/_next/static/chunks/113-f20cf828040267fc.js
 templates/../static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
 templates/../static/studio/_next/static/chunks/3-d801e16fe6466f20.js
 templates/../static/studio/_next/static/chunks/30-825cca92eb40c60a.js
 templates/../static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
 templates/../static/studio/_next/static/chunks/707-69e1edf708a55a15.js
 templates/../static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
@@ -173,14 +171,16 @@
 templates/../static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
 templates/../static/studio/_next/static/css/cc49d8d41e055bcd.css
 templates/../static/studio/_next/static/media/2e1b830192b7974a.woff2
 templates/../static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
 templates/../static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
 templates/../static/studio/_next/static/media/d607327a37a507c7.woff2
 templates/../static/studio/_next/static/media/ebec2867f40f78ec.woff2
+templates/../static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js
+templates/../static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js
 templates/examples/__init__.py
 templates/examples/social_auth.html
 templates/studio/404.html
 templates/studio/actions.html
 templates/studio/architype.html
 templates/studio/dashboard.html
 templates/studio/emotion.html
```

### Comparing `jaseci_serv-1.4.1.7/jsserv` & `jaseci_serv-1.4.1.8/jsserv`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/setup.py` & `jaseci_serv-1.4.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/Jaseci-Submark.png` & `jaseci_serv-1.4.1.8/static/studio/Jaseci-Submark.png`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/113-f20cf828040267fc.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/113-f20cf828040267fc.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/3-d801e16fe6466f20.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/3-d801e16fe6466f20.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/30-825cca92eb40c60a.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/30-825cca92eb40c60a.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/707-69e1edf708a55a15.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/707-69e1edf708a55a15.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/main-1844b67c68085ff6.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/main-1844b67c68085ff6.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/chunks/webpack-620c68345e03c539.js` & `jaseci_serv-1.4.1.8/static/studio/_next/static/chunks/webpack-620c68345e03c539.js`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/css/cc49d8d41e055bcd.css` & `jaseci_serv-1.4.1.8/static/studio/_next/static/css/cc49d8d41e055bcd.css`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/media/2e1b830192b7974a.woff2` & `jaseci_serv-1.4.1.8/static/studio/_next/static/media/2e1b830192b7974a.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2` & `jaseci_serv-1.4.1.8/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2` & `jaseci_serv-1.4.1.8/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/media/d607327a37a507c7.woff2` & `jaseci_serv-1.4.1.8/static/studio/_next/static/media/d607327a37a507c7.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/_next/static/media/ebec2867f40f78ec.woff2` & `jaseci_serv-1.4.1.8/static/studio/_next/static/media/ebec2867f40f78ec.woff2`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/static/studio/react.svg` & `jaseci_serv-1.4.1.8/static/studio/react.svg`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/templates/examples/social_auth.html` & `jaseci_serv-1.4.1.8/templates/examples/social_auth.html`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.1.7/templates/studio/404.html` & `jaseci_serv-1.4.1.8/templates/studio/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -194,11 +194,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}
+   {"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/actions.html` & `jaseci_serv-1.4.1.8/templates/studio/actions.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/3-d801e16fe6466f20.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg">
    .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
@@ -162,11 +162,11 @@
       <main class="mantine-13jfpqk mantine-AppShell-main">
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/actions","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/actions","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/architype.html` & `jaseci_serv-1.4.1.8/templates/studio/architype.html`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/707-69e1edf708a55a15.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 11q5icf 14fpfx2 1o9zy70 zf12j9 3xbgk5 qo1k2 69vjwn 6j7erx 1vm4dsg 1n25hpt q1zkt0 1s8spa1 1lis5e 1j6r4wy ngdamr 12o4rl6 1dkv5kp pcb9km 1wvsdi7 11eb7y rbbj0h 137kca9 1avyp1d gyncl 1jftnom nyw25r 1hfjdaf o8x4z2 14swocp 1bkqg0k um9jxx 1s9rvpg 1m3pqry ittua2 12sbrde 265hdg 180iq9w 33vjzt r7pni9 15e18iv ze06i1 1jc5t4g q1fxpn 775zd8 g0only uquezq 18jy38z 1bjr02m 1ynez2c 1ekl79i 6wburq 1jvugyc 11jfaka 1e8ljqt 26ugy1 qvatf7 xlwgkm 1j1ni8n">
    .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-11q5icf{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-14fpfx2{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;overflow-y:scroll;padding:30px;width:90%;height:90vh;}.mantine-1o9zy70{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:start;-webkit-box-align:start;-ms-flex-align:start;align-items:start;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;}.mantine-1o9zy70>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-zf12j9{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:24px;}.mantine-zf12j9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-zf12j9:focus:not(:focus-visible){outline:none;}.mantine-3xbgk5{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;height:100%;overflow:visible;}.mantine-qo1k2{white-space:nowrap;height:100%;overflow:hidden;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-69vjwn{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:36px;padding-left:18px;padding-right:18px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:14px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#fd7e14;color:#fff;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}.mantine-69vjwn:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-69vjwn:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-69vjwn:hover{background-color:#f76707;}}@media (hover: none){.mantine-69vjwn:active{background-color:#f76707;}}.mantine-69vjwn:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-69vjwn:disabled,.mantine-69vjwn[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-69vjwn:disabled:active,.mantine-69vjwn[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-69vjwn[data-loading]{pointer-events:none;}.mantine-69vjwn[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-6j7erx{margin:-8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;height:600px;}.mantine-1vm4dsg{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:41.66666666666667%;-ms-flex-preferred-size:41.66666666666667%;flex-basis:41.66666666666667%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:41.66666666666667%;}@media (min-width: 576px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-1vm4dsg{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1n25hpt{width:100%;height:100%;overflow-y:auto;background:#f5f5f5;padding-right:16px;padding-left:16px;padding-top:16px;padding-bottom:16px;}.mantine-q1zkt0{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:16px;line-height:1.5;margin:0;margin-bottom:16px;}.mantine-q1zkt0:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-q1zkt0:focus:not(:focus-visible){outline:none;}.mantine-1lis5e{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;}.mantine-1j6r4wy{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-1j6r4wy:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1j6r4wy:focus:not(:focus-visible){outline:none;}.mantine-1j6r4wy:hover{color:#000;}.mantine-ngdamr{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;}.mantine-ngdamr:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-12o4rl6{height:0;width:0;position:absolute;overflow:hidden;white-space:nowrap;opacity:0;}.mantine-12o4rl6:focus{outline:none;}.mantine-12o4rl6:focus+.__mantine-ref-label{outline-offset:2px;outline:2px solid #ff922b;}.mantine-12o4rl6:focus:focus:not(:focus-visible)+.__mantine-ref-label{outline:none;}.mantine-1dkv5kp{position:relative;box-sizing:border-box;-webkit-flex:1;-ms-flex:1;flex:1;z-index:2;-webkit-transition:border-left-color 0ms ease;transition:border-left-color 0ms ease;border-left-color:transparent!important;border-top-color:transparent!important;border-radius:4px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),0 1px 2px rgba(0, 0, 0, 0.1);background-color:#fff;}.mantine-1dkv5kp:not(:first-of-type){border-style:solid;border-width:0 0 0 1px;border-color:#dee2e6;}.mantine-1dkv5kp+.__mantine-ref-control{border-left-color:transparent!important;border-top-color:transparent!important;}.mantine-pcb9km{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;border-radius:4px;font-weight:500;font-size:14px;cursor:pointer;display:block;text-align:center;padding:5px 10px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#495057;-webkit-transition:color 0ms ease;transition:color 0ms ease;}.mantine-pcb9km:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-pcb9km:focus:not(:focus-visible){outline:none;}.mantine-pcb9km:hover{color:#000;}.mantine-pcb9km,.mantine-pcb9km:hover{color:#000;}.mantine-1wvsdi7{position:relative;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;width:auto;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;background-color:#f1f3f5;border-radius:4px;overflow:hidden;padding:4px;}.mantine-11eb7y{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;margin-bottom:16px;}.mantine-rbbj0h{overflow:scroll;height:500px;position:relative;}.mantine-137kca9{position:absolute;top:0;left:0;right:0;bottom:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;overflow:hidden;}.mantine-gyncl{position:absolute;top:0;bottom:0;left:0;right:0;z-index:400;background-color:#fff;opacity:0.75;border-radius:0;}.mantine-1jftnom{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:top;-ms-flex-pack:top;-webkit-justify-content:top;justify-content:top;gap:16px;padding:10px;}.mantine-nyw25r{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:58.333333333333336%;-ms-flex-preferred-size:58.333333333333336%;flex-basis:58.333333333333336%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:58.333333333333336%;}@media (min-width: 576px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-nyw25r{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1hfjdaf{-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}.mantine-o8x4z2{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;border-bottom:2px solid #dee2e6;}.mantine-14swocp{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;}.mantine-14swocp:not(:only-child){margin-right:7px;}.mantine-1bkqg0k{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;position:relative;padding:10px 16px;padding-left:10px;font-size:14px;white-space:nowrap;z-index:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;line-height:1;border-bottom:2px solid transparent;margin-bottom:-2px;border-radius:4px 4px 0 0;}.mantine-1bkqg0k:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bkqg0k:focus:not(:focus-visible){outline:none;}.mantine-1bkqg0k:disabled{opacity:0.5;cursor:not-allowed;}@media (hover: hover){.mantine-1bkqg0k:disabled:hover{background-color:transparent;}}@media (hover: none){.mantine-1bkqg0k:disabled:active{background-color:transparent;}}.mantine-1bkqg0k:focus{z-index:1;}@media (hover: hover){.mantine-1bkqg0k:hover{background-color:#f8f9fa;border-color:#dee2e6;}}@media (hover: none){.mantine-1bkqg0k:active{background-color:#f8f9fa;border-color:#dee2e6;}}.mantine-1bkqg0k[data-active]{border-color:#fd7e14;color:#000;}@media (hover: hover){.mantine-1bkqg0k[data-active]:hover{border-color:#fd7e14;}}@media (hover: none){.mantine-1bkqg0k[data-active]:active{border-color:#fd7e14;}}.mantine-um9jxx{padding-top:10px;}.mantine-1s9rvpg{padding-top:10px;display:none;height:100%;}.mantine-1m3pqry{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;}.mantine-ittua2{display:inline-block;font-size:14px;font-weight:500;color:#212529;word-break:break-word;cursor:default;-webkit-tap-highlight-color:transparent;}.mantine-12sbrde{position:relative;}.mantine-265hdg{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:auto;-webkit-tap-highlight-color:transparent;line-height:1.55;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:12px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;padding-top:10px;padding-bottom:10px;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:12px;}.mantine-265hdg:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-265hdg:disabled::-webkit-input-placeholder{color:#909296;}.mantine-265hdg:disabled::-moz-placeholder{color:#909296;}.mantine-265hdg:disabled:-ms-input-placeholder{color:#909296;}.mantine-265hdg:disabled::placeholder{color:#909296;}.mantine-265hdg::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-265hdg::-webkit-inner-spin-button,.mantine-265hdg::-webkit-outer-spin-button,.mantine-265hdg::-webkit-search-decoration,.mantine-265hdg::-webkit-search-cancel-button,.mantine-265hdg::-webkit-search-results-button,.mantine-265hdg::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-265hdg[type=number]{-moz-appearance:textfield;}.mantine-265hdg:focus,.mantine-265hdg:focus-within{outline:none;border-color:#fd7e14;}.mantine-180iq9w{color:#fff;-webkit-transform:translateY(5px) scale(0.5);-moz-transform:translateY(5px) scale(0.5);-ms-transform:translateY(5px) scale(0.5);transform:translateY(5px) scale(0.5);opacity:0;transition-property:opacity,transform;transition-timing-function:ease;transition-duration:100ms;pointer-events:none;width:10px;position:absolute;z-index:1;top:0;bottom:0;left:0;right:0;margin:auto;}@media (prefers-reduced-motion){.mantine-180iq9w{transition-duration:0ms;}}.mantine-33vjzt{position:relative;width:20px;height:20px;-webkit-order:1;-ms-flex-order:1;order:1;}.mantine-r7pni9{-webkit-tap-highlight-color:transparent;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;background-color:#fff;border:1px solid #ced4da;width:20px;height:20px;border-radius:4px;padding:0;display:block;margin:0;-webkit-transition:border-color 100ms ease,background-color 100ms ease;transition:border-color 100ms ease,background-color 100ms ease;cursor:default;}.mantine-r7pni9:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-r7pni9:focus:not(:focus-visible){outline:none;}.mantine-r7pni9:checked{background-color:#fd7e14;border-color:#fd7e14;}.mantine-r7pni9:checked+.__mantine-ref-icon{opacity:1;color:#fff;-webkit-transform:translateY(0) scale(1);-moz-transform:translateY(0) scale(1);-ms-transform:translateY(0) scale(1);transform:translateY(0) scale(1);}.mantine-r7pni9:disabled{background-color:#e9ecef;border-color:#dee2e6;cursor:not-allowed;}.mantine-r7pni9:disabled+.__mantine-ref-icon{color:#adb5bd;}.mantine-15e18iv{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;}.mantine-ze06i1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;font-size:14px;line-height:20px;color:#000;cursor:default;-webkit-order:2;-ms-flex-order:2;order:2;}.mantine-1jc5t4g{cursor:default;padding-left:12px;}.mantine-1jc5t4g[data-disabled]{color:#adb5bd;}.mantine-q1fxpn{margin-top:12px;margin-bottom:12px;}.mantine-775zd8{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;gap:16px;margin-top:12px;margin-bottom:12px;}.mantine-775zd8>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-g0only{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;line-height:1.55;min-width:300px;}.mantine-uquezq{position:absolute;top:0;bottom:0;right:0;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;width:30px;pointer-events:none;}.mantine-18jy38z{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;height:36px;-webkit-tap-highlight-color:transparent;line-height:34px;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;resize:none;box-sizing:border-box;font-size:14px;width:100%;color:#000;display:block;text-align:left;min-height:36px;padding-left:12px;padding-right:30px;border-radius:4px;border:1px solid #ced4da;background-color:#fff;-webkit-transition:border-color 100ms ease;transition:border-color 100ms ease;}.mantine-18jy38z:disabled{background-color:#f1f3f5;color:#909296;opacity:0.6;cursor:not-allowed;}.mantine-18jy38z:disabled::-webkit-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::-moz-placeholder{color:#909296;}.mantine-18jy38z:disabled:-ms-input-placeholder{color:#909296;}.mantine-18jy38z:disabled::placeholder{color:#909296;}.mantine-18jy38z::-webkit-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-moz-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z:-ms-input-placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::placeholder{opacity:1;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;color:#adb5bd;}.mantine-18jy38z::-webkit-inner-spin-button,.mantine-18jy38z::-webkit-outer-spin-button,.mantine-18jy38z::-webkit-search-decoration,.mantine-18jy38z::-webkit-search-cancel-button,.mantine-18jy38z::-webkit-search-results-button,.mantine-18jy38z::-webkit-search-results-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}.mantine-18jy38z[type=number]{-moz-appearance:textfield;}.mantine-18jy38z:focus,.mantine-18jy38z:focus-within{outline:none;border-color:#fd7e14;}.mantine-1bjr02m{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;height:30px;padding-left:14px;padding-right:14px;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;display:inline-block;width:auto;border-radius:4px;font-weight:600;position:relative;line-height:1;font-size:12px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;cursor:pointer;border:1px solid transparent;background-color:#12b886;color:#fff;margin-top:16px;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}.mantine-1bjr02m:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1bjr02m:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-1bjr02m:hover{background-color:#0ca678;}}@media (hover: none){.mantine-1bjr02m:active{background-color:#0ca678;}}.mantine-1bjr02m:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-1bjr02m:disabled,.mantine-1bjr02m[data-disabled]{border-color:transparent;background-color:#e9ecef;color:#adb5bd;cursor:not-allowed;background-image:none;pointer-events:none;}.mantine-1bjr02m:disabled:active,.mantine-1bjr02m[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-1bjr02m[data-loading]{pointer-events:none;}.mantine-1bjr02m[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-1ynez2c{background:#e9ecef;border:#adb5bd;border-radius:8px;min-height:300px;max-height:400px;overflow-y:scroll;margin-top:20px;margin-bottom:20px;padding-right:16px;padding-left:16px;padding-top:10px;padding-bottom:10px;}.mantine-1ekl79i{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;gap:10px;margin-bottom:12px;}.mantine-1ekl79i>*{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;}.mantine-6wburq{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-weight:bold;}.mantine-6wburq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-6wburq:focus:not(:focus-visible){outline:none;}.mantine-1jvugyc{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;box-sizing:border-box;width:20px;height:20px;min-width:20px;min-height:20px;border-radius:32px;background-color:#fa5252;color:#fff;border:1px solid transparent;}.mantine-11jfaka{box-sizing:border-box;position:relative;font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;line-height:1.7;font-size:13px;border-radius:4px;padding:12px 0;margin-top:0;margin-bottom:0;}.mantine-1e8ljqt{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;width:100%;padding:0 16px;}.mantine-26ugy1{width:100%;}.mantine-qvatf7{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;border:1px solid transparent;background-color:transparent;color:#868e96;position:relative;height:28px;min-height:28px;width:28px;min-width:28px;border-radius:4px;padding:0;line-height:1;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:absolute;top:10px;right:10px;left:unset;z-index:2;}.mantine-qvatf7:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-qvatf7:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-qvatf7:hover{background-color:rgba(248, 249, 250, 1);}}@media (hover: none){.mantine-qvatf7:active{background-color:rgba(248, 249, 250, 1);}}.mantine-qvatf7:active{-webkit-transform:translateY(1px);-moz-transform:translateY(1px);-ms-transform:translateY(1px);transform:translateY(1px);}.mantine-qvatf7:disabled,.mantine-qvatf7[data-disabled]{color:#ced4da;cursor:not-allowed;background-color:#f1f3f5;border-color:#f1f3f5;background-image:none;pointer-events:none;}.mantine-qvatf7:disabled:active,.mantine-qvatf7[data-disabled]:active{-webkit-transform:none;-moz-transform:none;-ms-transform:none;transform:none;}.mantine-qvatf7[data-loading]{pointer-events:none;}.mantine-qvatf7[data-loading]::before{content:"";position:absolute;top:-1px;left:-1px;right:-1px;bottom:-1px;background-color:rgba(255, 255, 255, .5);border-radius:4px;cursor:not-allowed;}.mantine-qvatf7,.mantine-qvatf7:hover{background-color:#f8f9fa;}.mantine-xlwgkm{width:100%;height:100%;}.mantine-1j1ni8n{overflow:hidden;}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
@@ -381,11 +381,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/architype","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/architype","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/dashboard.html` & `jaseci_serv-1.4.1.8/templates/studio/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine ibbm6b 13jfpqk osix87 hhjyz1 8od8ev p7xtuc 1h8zs6q hv1yhu 1l34ikq khtkeg 1avyp1d nsdj 1eid6d8 10wxedn 1mk5h8q pzrbb4 us9vra 1q9ffne svfr8w 1onk4kl 1wbj66w 1rq7tn8 13oshj5">
    .mantine-ibbm6b{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;box-sizing:border-box;}.mantine-13jfpqk{-webkit-flex:1;-ms-flex:1;flex:1;width:100vw;box-sizing:border-box;min-height:100vh;padding-top:calc(var(--mantine-header-height, 0px) + 16px);padding-bottom:calc(var(--mantine-footer-height, 0px) + 16px);padding-left:calc(var(--mantine-navbar-width, 0px) + 16px);padding-right:calc(var(--mantine-aside-width, 0px) + 16px);}@media (max-width: -1px){.mantine-13jfpqk{padding-right:16px;}}.mantine-osix87{box-sizing:border-box;}.mantine-hhjyz1{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;top:var(--mantine-header-height);left:0;bottom:0;z-index:100;height:100vh;width:80px;position:fixed;box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;background-color:#fff;border-right:1px solid #e9ecef;padding:16px;}@media (max-width: 991px){.mantine-hhjyz1[data-hidden]{display:none;}}.mantine-8od8ev{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;}.mantine-p7xtuc{margin-top:50px;-webkit-flex:1;-ms-flex:1;flex:1;box-sizing:border-box;}.mantine-1h8zs6q{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;gap:0;}.mantine-hv1yhu{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-hv1yhu:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-hv1yhu:focus:not(:focus-visible){outline:none;}.mantine-hv1yhu:hover{background-color:#f8f9fa;}.mantine-1l34ikq{-webkit-tap-highlight-color:transparent;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;cursor:pointer;border:0;padding:0;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;font-size:16px;background-color:transparent;text-align:left;color:#000;-webkit-text-decoration:none;text-decoration:none;box-sizing:border-box;width:50px;height:50px;border-radius:8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;color:#495057;}.mantine-1l34ikq:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1l34ikq:focus:not(:focus-visible){outline:none;}.mantine-1l34ikq:hover{background-color:#f8f9fa;}.mantine-1l34ikq,.mantine-1l34ikq:hover{background-color:rgba(255, 244, 230, 1);color:#fd7e14;}.mantine-khtkeg{-webkit-flex:0;-ms-flex:0;flex:0;box-sizing:border-box;}.mantine-nsdj{margin:-8px;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;}.mantine-1eid6d8{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:66.66666666666667%;-ms-flex-preferred-size:66.66666666666667%;flex-basis:66.66666666666667%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:66.66666666666667%;}@media (min-width: 576px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-1eid6d8{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-10wxedn{outline:0;-webkit-tap-highlight-color:transparent;display:block;-webkit-text-decoration:none;text-decoration:none;color:#000;background-color:#fff;box-sizing:border-box;border-radius:8px;box-shadow:0 1px 3px rgba(0, 0, 0, 0.05),rgba(0, 0, 0, 0.05) 0px 20px 25px -5px,rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;border:1px solid #dee2e6;position:relative;overflow:hidden;background-color:#fff;margin:0 auto;padding:30px;}.mantine-1mk5h8q{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:22px;line-height:1.4;margin:0;margin-bottom:20px;}.mantine-1mk5h8q:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1mk5h8q:focus:not(:focus-visible){outline:none;}.mantine-pzrbb4{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:25%;-ms-flex-preferred-size:25%;flex-basis:25%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:25%;}@media (min-width: 576px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-pzrbb4{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-us9vra{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;font-weight:700;font-size:16px;line-height:1.5;margin:0;}.mantine-us9vra:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-us9vra:focus:not(:focus-visible){outline:none;}.mantine-1q9ffne{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:#868e96;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;font-weight:normal;}.mantine-1q9ffne:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1q9ffne:focus:not(:focus-visible){outline:none;}.mantine-svfr8w{box-sizing:border-box;-webkit-box-flex:0;-webkit-flex-grow:0;-ms-flex-positive:0;flex-grow:0;padding:8px;-webkit-flex-basis:33.333333333333336%;-ms-flex-preferred-size:33.333333333333336%;flex-basis:33.333333333333336%;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;max-width:33.333333333333336%;}@media (min-width: 576px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 768px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 992px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1200px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}@media (min-width: 1400px){.mantine-svfr8w{-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;}}.mantine-1onk4kl{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;-webkit-box-pack:top;-ms-flex-pack:top;-webkit-justify-content:top;justify-content:top;gap:2px;}.mantine-1wbj66w{border:0;border-top-width:1px;border-top-color:#ced4da;border-top-style:solid;margin:0;border-top:0!important;}.mantine-1rq7tn8{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:inherit;font-size:12px;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;margin-top:2px;}.mantine-1rq7tn8:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-1rq7tn8:focus:not(:focus-visible){outline:none;}.mantine-1rq7tn8::before{content:"";-webkit-flex:1;-ms-flex:1;flex:1;height:1px;border-top:1px solid #ced4da;margin-right:10px;}.mantine-1rq7tn8::after{content:"";-webkit-flex:1;-ms-flex:1;flex:1;border-top:1px solid #ced4da;margin-left:10px;}.mantine-1rq7tn8::before{display:none;}.mantine-13oshj5{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;-webkit-tap-highlight-color:transparent;color:#868e96;font-size:inherit;line-height:1.55;-webkit-text-decoration:none;text-decoration:none;background-color:transparent;cursor:pointer;padding:0;border:0;}.mantine-13oshj5:focus{outline-offset:2px;outline:2px solid #ff922b;}.mantine-13oshj5:focus:not(:focus-visible){outline:none;}@media (hover: hover){.mantine-13oshj5:hover{-webkit-text-decoration:underline;text-decoration:underline;}}@media (hover: none){.mantine-13oshj5:active{-webkit-text-decoration:underline;text-decoration:underline;}}
   </style>
   <script>
    window.django = {is_authenticated: "{{ request.user.is_authenticated }}" === "True" ? true : false, user: "{{request.user}}"};
   </script>
@@ -260,11 +260,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/dashboard","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/dashboard","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/emotion.html` & `jaseci_serv-1.4.1.8/templates/studio/emotion.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -164,11 +164,11 @@
       <main class="mantine-13jfpqk mantine-AppShell-main">
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/emotion","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/emotion","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/graph-viewer.html` & `jaseci_serv-1.4.1.8/templates/studio/graph-viewer.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/289-4a13cf748d6cfb17.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -179,11 +179,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/graph-viewer","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/graph-viewer","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/index.html` & `jaseci_serv-1.4.1.8/templates/studio/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/76-3f26e2d93951e5cd.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/113-f20cf828040267fc.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -249,11 +249,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/layout.html` & `jaseci_serv-1.4.1.8/templates/studio/layout.html`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/main-1844b67c68085ff6.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -280,11 +280,11 @@
        </html>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/layout","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/layout","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

### Comparing `jaseci_serv-1.4.1.7/templates/studio/logs.html` & `jaseci_serv-1.4.1.8/templates/studio/logs.html`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/30-825cca92eb40c60a.js" %}'>
   </script>
   <script defer="" src='{% static "/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_buildManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_buildManifest.js" %}'>
   </script>
-  <script defer="" src='{% static "/studio/_next/static/6EQdsZVD3BsNeiGbKOH3C/_ssgManifest.js" %}'>
+  <script defer="" src='{% static "/studio/_next/static/u7vhajvBe15o56dx6n_tS/_ssgManifest.js" %}'>
   </script>
   <style data-emotion="mantine-global zl4edr">
    html{font-family:sans-serif;line-height:1.15;-webkit-text-size-adjust:100%;-moz-text-size-adjust:100%;-ms-text-size-adjust:100%;text-size-adjust:100%;}body{margin:0;}article,aside,footer,header,nav,section,figcaption,figure,main{display:block;}h1{font-size:2em;}hr{box-sizing:content-box;height:0;overflow:visible;}pre{font-family:monospace,monospace;font-size:1em;}a{background:transparent;text-decoration-skip:objects;}a:active,a:hover{outline-width:0;}abbr[title]{border-bottom:none;-webkit-text-decoration:underline;text-decoration:underline;}b,strong{font-weight:bolder;}code,kbp,samp{font-family:monospace,monospace;font-size:1em;}dfn{font-style:italic;}mark{background-color:#ff0;color:#000;}small{font-size:80%;}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline;}sup{top:-0.5em;}sub{bottom:-0.25em;}audio,video{display:inline-block;}audio:not([controls]){display:none;height:0;}img{border-style:none;vertical-align:middle;}svg:not(:root){overflow:hidden;}button,input,optgroup,select,textarea{font-family:sans-serif;font-size:100%;line-height:1.15;margin:0;}button,input{overflow:visible;}button,select{text-transform:none;}button,[type=reset],[type=submit]{-webkit-appearance:button;}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0;}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText;}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal;}progress{display:inline-block;vertical-align:baseline;}textarea{overflow:auto;}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0;}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto;}[type=search]{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}[type=search]::-webkit-search-cancel-button,[type=search]::-webkit-search-decoration{-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;appearance:none;}::-webkit-file-upload-button{-webkit-appearance:button;-moz-appearance:button;-ms-appearance:button;appearance:button;font:inherit;}details,menu{display:block;}summary{display:-webkit-box;display:-webkit-list-item;display:-ms-list-itembox;display:list-item;}canvas{display:inline-block;}template{display:none;}[hidden]{display:none;}
   </style>
   <style data-emotion="mantine-global 1j3c5om">
    *,*::before,*::after{box-sizing:border-box;}html{-webkit-print-color-scheme:light;color-scheme:light;}body{font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;background-color:#fff;color:#000;line-height:1.55;font-size:16px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
   </style>
@@ -280,11 +280,11 @@
        </div>
       </main>
      </div>
     </div>
    </div>
   </div>
   <script id="__NEXT_DATA__" type="application/json">
-   {"props":{"pageProps":{}},"page":"/logs","query":{},"buildId":"6EQdsZVD3BsNeiGbKOH3C","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
+   {"props":{"pageProps":{}},"page":"/logs","query":{},"buildId":"u7vhajvBe15o56dx6n_tS","assetPrefix":"/studio","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}
   </script>
  </body>
 </html>
```

