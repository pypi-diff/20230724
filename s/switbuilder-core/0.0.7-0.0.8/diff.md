# Comparing `tmp/switbuilder_core-0.0.7.tar.gz` & `tmp/switbuilder_core-0.0.8.tar.gz`

## Comparing `switbuilder_core-0.0.7.tar` & `switbuilder_core-0.0.8.tar`

### file list

```diff
@@ -1,104 +1,59 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.DS_Store
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/build.sh
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0    23295 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/constants.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/logger.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/lokalise.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/activity_router.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/dependencies.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/exceptions.py
--rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/channel/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/channel/schemas.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/channel/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/channel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/conversation/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/conversation/schemas.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/conversation/service.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/conversation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/constants.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/exception.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/schemas.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/service.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/__init__.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/tests.py
--rw-r--r--   0        0        0   306291 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/cid_image_email.json
--rw-r--r--   0        0        0  1499842 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/email_with_attachment.json
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/empty_receiver_email.json
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/html_email.json
--rw-r--r--   0        0        0    64730 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/invalid_swit_image.json
--rw-r--r--   0        0        0   631221 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/large_cid_image_email.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/email/plain_text_email.json
--rw-r--r--   0        0        0    34901 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/html/example1.html
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/html/example2.html
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/html/example3.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/imap/tests/html/example4.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/membership/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/membership/schemas.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/membership/service.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/membership/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/project/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/project/schemas.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/project/service.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/project/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/task/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/task/schemas.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/task/service.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/task/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/workspace/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/workspace/schemas.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/workspace/service.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/apis/v1/workspace/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/constants.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/exception.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/models.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/oauth2.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/repository.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/service.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/tests/test_path_resolver.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/tests/test_router.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/tests/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.DS_Store
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/build.sh
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/workspace.xml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/constants.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/logger.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/lokalise.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/exception.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/models.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/oauth2.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/schemas.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_oauth2.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_path_resolver.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/test_router.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/tests/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 switbuilder_core-0.0.8/PKG-INFO
```

### Comparing `switbuilder_core-0.0.7/.DS_Store` & `switbuilder_core-0.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.7/requirements.txt` & `switbuilder_core-0.0.8/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 urllib3==2.0.3
 webencodings==0.5.1
 zipp==3.15.0
 
 httpx~=0.24.1
 fastapi~=0.98.0
 starlette~=0.27.0
-SQLAlchemy~=2.0.17
+SQLAlchemy==1.4.49
 PyMySQL~=1.1.0
 PyJWT~=2.7.0
```

### Comparing `switbuilder_core-0.0.7/.idea/workspace.xml` & `switbuilder_core-0.0.8/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `switbuilder_core-0.0.7/.idea/workspace.xml` & `switbuilder_core-0.0.8/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="first commit"/>
+    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="first commit">
+      <change beforePath="$PROJECT_DIR$/switcore/auth/models.py" beforeDir="false" afterPath="$PROJECT_DIR$/switcore/auth/models.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -29,41 +31,41 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230720_0020",
+    "com.google.cloudcode.ide_session_index": "20230724_0021",
     "git-widget-placeholder": "main",
     "last_opened_file_path": "/Users/el/PycharmProjects/core/tests",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "settings.editor.selected.configurable": "preferences.lookFeel",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
+      <recent name="$PROJECT_DIR$/switcore/auth"/>
       <recent name="$PROJECT_DIR$/switcore"/>
       <recent name="$PROJECT_DIR$/apis"/>
       <recent name="$PROJECT_DIR$"/>
-      <recent name="$PROJECT_DIR$/ui"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/switcore"/>
       <recent name="$PROJECT_DIR$/apis/v1"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/switbuilder-core"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.Python tests for test_router.RouterTest">
+  <component name="RunManager" selected="Python tests.Python tests for test_router.RouterTest.test_router03">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -78,71 +80,26 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for switcore.apis.v1.imap.tests" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/ui/signin"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;switcore.apis.v1.imap.tests&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests for switcore.apis.v1.imap.tests" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/ui/header"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;switcore.apis.v1.imap.tests&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests for test_path_resolver.PathResolverTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_path_resolver.PathResolverTest&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests for test_path_resolver.PathResolverTest.test_escape" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_oauth2.OAuth2Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_path_resolver.PathResolverTest.test_escape&quot;"/>
+      <option name="_new_target" value="&quot;test_oauth2.OAuth2Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Python tests for test_router.RouterTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -153,71 +110,56 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_router.RouterTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest.test_escape_router" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest.test_router03" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest.test_escape_router&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest.test_router03&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_router.RouterTest.test_router" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest.test_router_without_view_id" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_router.RouterTest.test_router&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest.test_router_without_view_id&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest.test_router_without_view_ids" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/ui/header"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.Test&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/ui/input"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.Test&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest.test_router_without_view_ids&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -320,19 +262,19 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router03"/>
         <item itemvalue="Python tests.Python tests for test_router.RouterTest"/>
-        <item itemvalue="Python tests.Python tests for test_path_resolver.PathResolverTest"/>
-        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_escape_router"/>
-        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router"/>
-        <item itemvalue="Python tests.Python tests for test_path_resolver.PathResolverTest.test_escape"/>
+        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router_without_view_id"/>
+        <item itemvalue="Python tests.Python tests for test_router.RouterTest.test_router_without_view_ids"/>
+        <item itemvalue="Python tests.Python tests for test_oauth2.OAuth2Test"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment=""/>
@@ -355,15 +297,25 @@
       <workItem from="1689309026861" duration="1964000"/>
       <workItem from="1689550354850" duration="22254000"/>
       <workItem from="1689764094217" duration="1443000"/>
       <workItem from="1689808899597" duration="15896000"/>
       <workItem from="1689831489315" duration="996000"/>
       <workItem from="1689834548055" duration="374000"/>
       <workItem from="1689837516403" duration="1023000"/>
-      <workItem from="1689838551694" duration="220000"/>
+      <workItem from="1689838551694" duration="872000"/>
+      <workItem from="1689839729816" duration="218000"/>
+      <workItem from="1689895265377" duration="24786000"/>
+      <workItem from="1690017519765" duration="343000"/>
+      <workItem from="1690059954555" duration="24000"/>
+      <workItem from="1690155177421" duration="4996000"/>
+      <workItem from="1690160472435" duration="247000"/>
+      <workItem from="1690160722459" duration="29000"/>
+      <workItem from="1690160759296" duration="452000"/>
+      <workItem from="1690161233838" duration="114000"/>
+      <workItem from="1690161356699" duration="17199000"/>
     </task>
     <task id="LOCAL-00001" summary="first commit">
       <option name="closed" value="true"/>
       <created>1689566168015</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -405,15 +357,39 @@
       <option name="closed" value="true"/>
       <created>1689838728707</created>
       <option name="number" value="00006"/>
       <option name="presentableId" value="LOCAL-00006"/>
       <option name="project" value="LOCAL"/>
       <updated>1689838728707</updated>
     </task>
-    <option name="localTasksCounter" value="7"/>
+    <task id="LOCAL-00007" summary="first commit">
+      <option name="closed" value="true"/>
+      <created>1689839904181</created>
+      <option name="number" value="00007"/>
+      <option name="presentableId" value="LOCAL-00007"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1689839904181</updated>
+    </task>
+    <task id="LOCAL-00008" summary="first commit">
+      <option name="closed" value="true"/>
+      <created>1690164923039</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690164923039</updated>
+    </task>
+    <task id="LOCAL-00009" summary="first commit">
+      <option name="closed" value="true"/>
+      <created>1690182180278</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1690182180278</updated>
+    </task>
+    <option name="localTasksCounter" value="10"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -426,11 +402,32 @@
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="first commit"/>
     <option name="LAST_COMMIT_MESSAGE" value="first commit"/>
   </component>
+  <component name="XDebuggerManager">
+    <breakpoint-manager>
+      <breakpoints>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/venv/lib/python3.10/site-packages/httpx_oauth/oauth2.py</url>
+          <line>47</line>
+          <option name="timeStamp" value="28"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/switcore/action/activity_handler_abc.py</url>
+          <line>82</line>
+          <option name="timeStamp" value="43"/>
+        </line-breakpoint>
+      </breakpoints>
+    </breakpoint-manager>
+    <watches-manager>
+      <configuration name="tests">
+        <watch expression="unquote(response.headers[&quot;location&quot;])" language="Python"/>
+      </configuration>
+    </watches-manager>
+  </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
-    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1689838675260" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1690182109684" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `switbuilder_core-0.0.7/.idea/inspectionProfiles/Project_Default.xml` & `switbuilder_core-0.0.8/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.7/switcore/logger.py` & `switbuilder_core-0.0.8/switcore/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import logging
+from typing import Callable
 from functools import wraps
 
 
-def add_handler(logger: logging.Logger):
+def get_logger() -> logging.Logger:
+    logger = logging.getLogger('[swit-logger]')
+    logger.setLevel(logging.INFO)
+
     if not any(isinstance(handler, logging.StreamHandler) for handler in logger.handlers):
         console_handler = logging.StreamHandler()
         console_formatter = logging.Formatter(
-            '[swit-logger] %(asctime)s - (function)%(name)s - %(levelname)s - %(message)s')
+            '%(asctime)s - [%(levelname)s] - %(name)s - (PID: %(process)d) - (File: %(filename)s - Function: %(funcName)s - Line: %(lineno)d) - %(message)s')
         console_handler.setFormatter(console_formatter)
         logger.addHandler(console_handler)
 
-
-def get_logger(func_name: str):
-    logger = logging.getLogger(func_name)
-    add_handler(logger)
     return logger
 
 
 def logger_decorator():
-    def decorator(func):
+    def decorator(func: Callable):
+        logger = get_logger()
+        func.logger = logger
+
         @wraps(func)
         async def wrapper(*args, **kwargs):
-            logger = logging.getLogger(f"{func.__name__}")
-            add_handler(logger)
-            return await func(*args, **kwargs, logger=logger)
+            return await func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `switbuilder_core-0.0.7/switcore/lokalise.py` & `switbuilder_core-0.0.8/switcore/lokalise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
 import os
-from functools import wraps
 
 import httpx
 
 
 async def set_translate():
     localise_token: str = os.getenv('LOCALIZE_PROJECT_ID', None)
 
     assert localise_token is not None, "LOCALIZE_PROJECT_ID is not set check .env file"
-    
+
     params = {
         "project_id": localise_token,
         "tags": "webhook proxy",
     }
 
     async with httpx.AsyncClient() as client:
         res = await client.get("https://ur.swit.support/get_trans", params=params, timeout=60)
```

### Comparing `switbuilder_core-0.0.7/switcore/action/activity_handler_abc.py` & `switbuilder_core-0.0.8/switcore/action/activity_handler_abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 
 from switcore.action.activity_router import ActivityRouter, PathResolver
+from switcore.action.exceptions import UndefinedSubmitAction
 from switcore.action.schemas import SwitRequest, BaseState, SwitResponse, UserActionType
 from switcore.type import DrawerHandler
 
 
 class ActivityHandlerABC(ABC):
     def __init__(self) -> None:
         self.handler: dict[str, dict[str, DrawerHandler]] = defaultdict(dict)
+        self.action_ids_to_be_called_in_views: set[str] = set()
 
     def include_activity_router(self, activity_router: ActivityRouter):
+        self.action_ids_to_be_called_in_views.update(activity_router.action_ids_to_be_called_in_views)
         for view_id, _dict in activity_router.handler.items():
             for action_id, func in _dict.items():
+                if view_id == '*':
+                    self.action_ids_to_be_called_in_views.remove(action_id)
+
                 self.handler[view_id][action_id] = func
 
     async def on_turn(self, swit_request: SwitRequest, state: BaseState) -> SwitResponse:
         if swit_request.user_action.type == UserActionType.view_actions_drop:
             response = await self.on_view_actions_drop(swit_request, state)
         elif swit_request.user_action.type == UserActionType.view_actions_submit:
             response = await self.on_view_actions_submit(swit_request, state)
@@ -73,20 +79,29 @@
         raise NotImplementedError()
 
     async def on_view_actions_submit(self, swit_request: SwitRequest, state: BaseState) -> SwitResponse:
         user_action: str = swit_request.user_action.id
         action_id_path_resolver: PathResolver = PathResolver.from_combined(user_action)
         view_id_path_resolver: PathResolver = PathResolver.from_combined(swit_request.current_view.view_id)
 
-        drawer_func_or_null: DrawerHandler | None = (
+        view_drawer_func_or_null: DrawerHandler | None = (
             self.handler
             .get(view_id_path_resolver.id, {})
             .get(action_id_path_resolver.id, None))
 
-        assert drawer_func_or_null, f"undefined submit action!!: {user_action}"
+        if action_id_path_resolver.id in self.action_ids_to_be_called_in_views and view_drawer_func_or_null is None:
+            raise UndefinedSubmitAction(f"undefined submit action in view: {user_action}")
+
+        if view_drawer_func_or_null:
+            drawer_func_or_null = view_drawer_func_or_null
+        else:
+            drawer_func_or_null = self.handler.get('*', {}).get(action_id_path_resolver.id, None)
+
+        if drawer_func_or_null is None:
+            raise UndefinedSubmitAction(f"undefined submit action: {user_action}")
 
         args = [swit_request, state, *action_id_path_resolver.paths]
         response = await drawer_func_or_null(*args)
         return response
 
     @abstractmethod
     async def on_view_actions_oauth_complete(self, swit_request: SwitRequest, state: BaseState) -> SwitResponse:
```

### Comparing `switbuilder_core-0.0.7/switcore/action/activity_router.py` & `switbuilder_core-0.0.8/switcore/action/activity_router.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 
 def escape(text: str) -> str:
     return text.replace('/', '\\')
 
 
 class PathResolver:
-    def __init__(self, id: str, paths: list[int | str]) -> None:
+    def __init__(self, id: str, paths: list[int | str] | None = None) -> None:
+        if paths is None:
+            paths = []
+
         self._id: str = escape(id)
         self._paths: list[str] = []
         for path in paths:
             self.add_path(path)
 
     def __str__(self):
         return self.combined_path
@@ -36,30 +39,41 @@
                 ret.append(path)
 
         return ret
 
     @staticmethod
     def from_combined(combined_id: str) -> 'PathResolver':
         arr: list[str] = combined_id.split('/')
-        return PathResolver(arr[0], arr[1:])
+        paths: list[str] = arr[1:]
+
+        if len(paths) == 1 and paths[0] == '':
+            paths = []
+
+        return PathResolver(arr[0], paths)
 
     def add_path(self, path: int | str):
         assert isinstance(path, int) or isinstance(path, str), "only int or str is allowed"
 
         if isinstance(path, int):
             path = str(path)
 
         self._paths.append(escape(path))
 
 
 class ActivityRouter:
 
     def __init__(self) -> None:
         self.handler: dict[str, dict[str, DrawerHandler]] = defaultdict(dict)
+        self.action_ids_to_be_called_in_views: set[str] = set()
+
+    def register(self, action_id: str, view_ids: list[str] | None = None):
+        if view_ids is None:
+            view_ids = ['*']
 
-    def register(self, view_ids: list[str], action_id: str):
         def decorator(func):
             for view_id in view_ids:
-                self.handler[escape(view_id)][escape(action_id)] = func
+                _action_id = escape(action_id)
+                self.action_ids_to_be_called_in_views.add(_action_id)
+                self.handler[escape(view_id)][_action_id] = func
             return func
 
         return decorator
```

### Comparing `switbuilder_core-0.0.7/switcore/action/schemas.py` & `switbuilder_core-0.0.8/switcore/action/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import bz2
 import json
-from abc import ABC
 from datetime import datetime
 from enum import Enum
 from typing import Any
 from typing import Optional, Dict, List
 
 from pydantic import BaseModel
 from pydantic import validator
@@ -72,26 +71,14 @@
 
 
 class Context(BaseModel):
     workspace_id: str
     channel_id: str
 
 
-class BaseState(BaseModel):
-    autoincrement_id: int = 1
-
-    @staticmethod
-    def from_bytes(byte: bytes) -> 'BaseState':
-        d = json.loads(bz2.decompress(base64.b64decode(byte)).decode("utf-8"))
-        return BaseState(**d)
-
-    def to_bytes(self) -> bytes:
-        return base64.b64encode(bz2.compress(json.dumps(self.dict()).encode("utf-8"), 1))
-
-
 ElementType = CollectionEntry | Button | Divider | File \
               | HtmlFrame | Input | Select | SignInPage | TextParagraph | Image | Textarea | Container | Tabs
 
 
 def contain_only_dict(elements_data: list[dict | ElementType]) -> bool:
     for element_data in elements_data:
         if isinstance(element_data, ElementType):
@@ -226,7 +213,19 @@
 
 
 class SwitResponse(BaseModel):
     callback_type: ViewCallbackType | AttachmentCallbackType
     new_view: View | None
     attachments: AttachmentView | None
     reference_view_id: str | None
+
+
+class BaseState(BaseModel):
+    autoincrement_id: int = 1
+
+    @staticmethod
+    def from_bytes(byte: bytes) -> 'BaseState':
+        d = json.loads(bz2.decompress(base64.b64decode(byte)).decode("utf-8"))
+        return BaseState(**d)
+
+    def to_bytes(self) -> bytes:
+        return base64.b64encode(bz2.compress(json.dumps(self.dict()).encode("utf-8"), 1))
```

### Comparing `switbuilder_core-0.0.7/switcore/auth/utils.py` & `switbuilder_core-0.0.8/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.7/switcore/ui/collection_entry.py` & `switbuilder_core-0.0.8/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.7/switcore/ui/file.py` & `switbuilder_core-0.0.8/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `switbuilder_core-0.0.7/tests/test_path_resolver.py` & `switbuilder_core-0.0.8/tests/test_path_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from switcore.action.activity_router import PathResolver
 from tests.utils import ActionIdTypes
 
 
 class PathResolverTest(unittest.TestCase):
     def test_combined_path(self):
-        path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id, ["a"])
+        path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id01, ["a"])
         self.assertEqual(path_resolver.combined_path, "test_action_id/a")
         self.assertEqual(path_resolver.id, "test_action_id")
 
         path_resolver._paths.append("b")
         self.assertEqual(path_resolver.combined_path, "test_action_id/a/b")
         self.assertEqual(path_resolver.id, "test_action_id")
 
     def test_from_combined(self):
         path_resolver: PathResolver = PathResolver.from_combined("test_action_id/a/b")
         self.assertEqual(path_resolver.combined_path, "test_action_id/a/b")
         self.assertEqual(path_resolver.id, "test_action_id")
         self.assertEqual(path_resolver._paths, ["a", "b"])
 
     def test_convert_int(self):
-        path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id, [1, "a"])
+        path_resolver: PathResolver = PathResolver(ActionIdTypes.test_action_id01, [1, "a"])
         self.assertEqual(path_resolver.combined_path, "test_action_id/1/a")
         self.assertEqual(path_resolver.paths, [1, "a"])
 
     def test_escape(self):
         path_resolver: PathResolver = PathResolver(ActionIdTypes.test_escape_action_id, ["a"])
         self.assertEqual(path_resolver.combined_path, "test_escape_action_id\escape/a")
         self.assertEqual(path_resolver.id, "test_escape_action_id\escape")
```

### Comparing `switbuilder_core-0.0.7/pyproject.toml` & `switbuilder_core-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "switbuilder-core"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "ur-team", email = "el.lee@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `switbuilder_core-0.0.7/PKG-INFO` & `switbuilder_core-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switbuilder-core
-Version: 0.0.7
+Version: 0.0.8
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <el.lee@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

