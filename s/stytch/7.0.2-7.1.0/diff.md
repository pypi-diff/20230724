# Comparing `tmp/stytch-7.0.2.tar.gz` & `tmp/stytch-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stytch-7.0.2.tar", last modified: Tue Jul 18 17:23:24 2023, max compression
+gzip compressed data, was "stytch-7.1.0.tar", last modified: Mon Jul 24 19:43:48 2023, max compression
```

## Comparing `stytch-7.0.2.tar` & `stytch-7.1.0.tar`

### file list

```diff
@@ -1,107 +1,115 @@
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.721485 stytch-7.0.2/
--rw-r--r--   0 gorel      (501) staff       (20)     1059 2022-12-06 17:10:39.000000 stytch-7.0.2/LICENSE.txt
--rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-18 17:23:24.721552 stytch-7.0.2/PKG-INFO
--rw-r--r--   0 gorel      (501) staff       (20)     4367 2023-04-20 19:06:08.000000 stytch-7.0.2/README.md
--rw-r--r--   0 gorel      (501) staff       (20)      110 2023-07-18 17:23:24.721768 stytch-7.0.2/setup.cfg
--rw-r--r--   0 gorel      (501) staff       (20)     1739 2023-07-18 15:29:31.000000 stytch-7.0.2/setup.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.705752 stytch-7.0.2/stytch/
--rw-r--r--   0 gorel      (501) staff       (20)      181 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/__init__.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.706545 stytch-7.0.2/stytch/b2b/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.2/stytch/b2b/__init__.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.710308 stytch-7.0.2/stytch/b2b/api/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.2/stytch/b2b/api/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)      892 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     7036 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/discovery_intermediate_sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)    21373 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/discovery_organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     8980 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)     2833 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/magic_links_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    16783 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     5807 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/magic_links_email_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    31415 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)    22509 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/organizations_members.py
--rw-r--r--   0 gorel      (501) staff       (20)    22270 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)    18614 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     8525 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)     3439 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)    19582 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)    11114 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/sso.py
--rw-r--r--   0 gorel      (501) staff       (20)    10786 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/sso_oidc.py
--rw-r--r--   0 gorel      (501) staff       (20)    10369 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/api/sso_saml.py
--rw-r--r--   0 gorel      (501) staff       (20)     1423 2023-07-18 17:22:31.000000 stytch-7.0.2/stytch/b2b/client.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.713431 stytch-7.0.2/stytch/b2b/models/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-02-22 04:57:31.000000 stytch-7.0.2/stytch/b2b/models/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)     1452 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     1159 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/discovery_intermediate_sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)     2325 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/discovery_organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     1712 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)     1674 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/magic_links_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)     1536 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)      431 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/magic_links_email_discovery.py
--rw-r--r--   0 gorel      (501) staff       (20)    11086 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/organizations.py
--rw-r--r--   0 gorel      (501) staff       (20)     2938 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/organizations_members.py
--rw-r--r--   0 gorel      (501) staff       (20)     5719 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)     1883 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     1149 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)      957 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)     3829 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)     3314 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/sso.py
--rw-r--r--   0 gorel      (501) staff       (20)     1400 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/sso_oidc.py
--rw-r--r--   0 gorel      (501) staff       (20)     1307 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/b2b/models/sso_saml.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.713673 stytch-7.0.2/stytch/consumer/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-07-18 16:50:44.000000 stytch-7.0.2/stytch/consumer/__init__.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.716767 stytch-7.0.2/stytch/consumer/api/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/consumer/api/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)    10339 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/crypto_wallets.py
--rw-r--r--   0 gorel      (501) staff       (20)    10629 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)    32410 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)    11720 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/oauth.py
--rw-r--r--   0 gorel      (501) staff       (20)     8142 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/otp.py
--rw-r--r--   0 gorel      (501) staff       (20)    16525 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/otp_email.py
--rw-r--r--   0 gorel      (501) staff       (20)    14129 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/otp_sms.py
--rw-r--r--   0 gorel      (501) staff       (20)    14165 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/otp_whatsapp.py
--rw-r--r--   0 gorel      (501) staff       (20)    28091 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)    16810 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     6424 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)     2876 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)    15782 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)    15027 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/totps.py
--rw-r--r--   0 gorel      (501) staff       (20)    28332 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/users.py
--rw-r--r--   0 gorel      (501) staff       (20)    17303 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/api/webauthn.py
--rw-r--r--   0 gorel      (501) staff       (20)     1823 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/client.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.720031 stytch-7.0.2/stytch/consumer/models/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/consumer/models/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)      467 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/attribute.py
--rw-r--r--   0 gorel      (501) staff       (20)     1673 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/crypto_wallets.py
--rw-r--r--   0 gorel      (501) staff       (20)     2324 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/magic_links.py
--rw-r--r--   0 gorel      (501) staff       (20)     1546 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/magic_links_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     3889 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/oauth.py
--rw-r--r--   0 gorel      (501) staff       (20)     1584 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/otp.py
--rw-r--r--   0 gorel      (501) staff       (20)     1082 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/otp_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     1064 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/otp_sms.py
--rw-r--r--   0 gorel      (501) staff       (20)     1074 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/otp_whatsapp.py
--rw-r--r--   0 gorel      (501) staff       (20)     8528 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/passwords.py
--rw-r--r--   0 gorel      (501) staff       (20)     1560 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/passwords_email.py
--rw-r--r--   0 gorel      (501) staff       (20)     1202 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/passwords_existing_password.py
--rw-r--r--   0 gorel      (501) staff       (20)     1010 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/passwords_session.py
--rw-r--r--   0 gorel      (501) staff       (20)    10130 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/sessions.py
--rw-r--r--   0 gorel      (501) staff       (20)     3779 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/totps.py
--rw-r--r--   0 gorel      (501) staff       (20)    15455 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/users.py
--rw-r--r--   0 gorel      (501) staff       (20)     2291 2023-07-18 17:21:53.000000 stytch-7.0.2/stytch/consumer/models/webauthn.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.720718 stytch-7.0.2/stytch/core/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-16 21:16:07.000000 stytch-7.0.2/stytch/core/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)      586 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/core/api_base.py
--rw-r--r--   0 gorel      (501) staff       (20)     1210 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/core/client_base.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.720961 stytch-7.0.2/stytch/core/http/
--rw-r--r--   0 gorel      (501) staff       (20)        0 2022-12-20 16:48:17.000000 stytch-7.0.2/stytch/core/http/__init__.py
--rw-r--r--   0 gorel      (501) staff       (20)     3605 2023-06-05 21:01:43.000000 stytch-7.0.2/stytch/core/http/client.py
--rw-r--r--   0 gorel      (501) staff       (20)     2106 2023-07-17 16:16:44.000000 stytch-7.0.2/stytch/core/response_base.py
--rw-r--r--   0 gorel      (501) staff       (20)       22 2023-07-18 17:22:48.000000 stytch-7.0.2/stytch/version.py
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.706344 stytch-7.0.2/stytch.egg-info/
--rw-r--r--   0 gorel      (501) staff       (20)     5142 2023-07-18 17:23:24.000000 stytch-7.0.2/stytch.egg-info/PKG-INFO
--rw-r--r--   0 gorel      (501) staff       (20)     3093 2023-07-18 17:23:24.000000 stytch-7.0.2/stytch.egg-info/SOURCES.txt
--rw-r--r--   0 gorel      (501) staff       (20)        1 2023-07-18 17:23:24.000000 stytch-7.0.2/stytch.egg-info/dependency_links.txt
--rw-r--r--   0 gorel      (501) staff       (20)       69 2023-07-18 17:23:24.000000 stytch-7.0.2/stytch.egg-info/requires.txt
--rw-r--r--   0 gorel      (501) staff       (20)        7 2023-07-18 17:23:24.000000 stytch-7.0.2/stytch.egg-info/top_level.txt
-drwxr-xr-x   0 gorel      (501) staff       (20)        0 2023-07-18 17:23:24.721349 stytch-7.0.2/test/
--rw-r--r--   0 gorel      (501) staff       (20)     9527 2023-07-17 16:16:44.000000 stytch-7.0.2/test/test_integration.py
--rw-r--r--   0 gorel      (501) staff       (20)    12747 2023-07-17 16:16:44.000000 stytch-7.0.2/test/test_integration_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 19:43:31.000000 stytch-7.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-24 19:43:48.327844 stytch-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-24 19:43:31.000000 stytch-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-24 19:43:48.327844 stytch-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-24 19:43:31.000000 stytch-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch/b2b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.315844 stytch-7.1.0/stytch/b2b/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32087 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25074 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/api/sso_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.319844 stytch-7.1.0/stytch/b2b/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery_intermediate_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/discovery_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/magic_links_email_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/oauth_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/organizations_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/b2b/models/sso_saml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.319844 stytch-7.1.0/stytch/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.323844 stytch-7.1.0/stytch/consumer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32410 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28091 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/api/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/consumer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/crypto_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/magic_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/magic_links_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/otp_whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_existing_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/passwords_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/totps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/consumer/models/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/stytch/core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/core/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:43:31.000000 stytch-7.1.0/stytch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.311844 stytch-7.1.0/stytch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 19:43:48.000000 stytch-7.1.0/stytch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:43:48.327844 stytch-7.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-24 19:43:31.000000 stytch-7.1.0/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-24 19:43:31.000000 stytch-7.1.0/test/test_integration_async.py
```

### Comparing `stytch-7.0.2/LICENSE.txt` & `stytch-7.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/PKG-INFO` & `stytch-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.0.2
+Version: 7.1.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.0.2/README.md` & `stytch-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/setup.py` & `stytch-7.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/discovery.py` & `stytch-7.1.0/stytch/b2b/api/discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/discovery_intermediate_sessions.py` & `stytch-7.1.0/stytch/b2b/api/discovery_intermediate_sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.models.discovery_intermediate_sessions import ExchangeResponse
+from stytch.b2b.models.discovery_intermediate_sessions import (
+    ExchangeRequestLocale,
+    ExchangeResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class IntermediateSessions:
     def __init__(
         self,
@@ -26,14 +29,15 @@
 
     def exchange(
         self,
         intermediate_session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ExchangeRequestLocale] = None,
     ) -> ExchangeResponse:
         """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
         This operation consumes the Intermediate Session.
 
         This endpoint can be used to accept invites and create new members via domain matching.
 
         Fields:
@@ -49,36 +53,40 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_id": organization_id,
         }
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for(
             "/v1/b2b/discovery/intermediate_sessions/exchange", data
         )
         res = self.sync_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status_code, res.json)
 
     async def exchange_async(
         self,
         intermediate_session_token: str,
         organization_id: str,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ExchangeRequestLocale] = None,
     ) -> ExchangeResponse:
         """Exchange an Intermediate Session for a fully realized [Member Session](https://stytch.com/docs/b2b/api/session-object) in a desired [Organization](https://stytch.com/docs/b2b/api/organization-object).
         This operation consumes the Intermediate Session.
 
         This endpoint can be used to accept invites and create new members via domain matching.
 
         Fields:
@@ -94,22 +102,25 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_id": organization_id,
         }
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for(
             "/v1/b2b/discovery/intermediate_sessions/exchange", data
         )
         res = await self.async_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/discovery_organizations.py` & `stytch-7.1.0/stytch/b2b/api/discovery_organizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
@@ -99,14 +100,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
         if session_duration_minutes is not None:
@@ -125,14 +127,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
         res = self.sync_client.post(url, data)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
@@ -145,14 +149,15 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """If an end user does not want to join any already-existing organization, or has no possible organizations to join, this endpoint can be used to create a new
         [Organization](https://stytch.com/docs/b2b/api/organization-object) and [Member](https://stytch.com/docs/b2b/api/member-object).
 
         This operation consumes the Intermediate Session.
 
         This endpoint can also be used to start an initial session for the newly created member and organization.
@@ -209,14 +214,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "intermediate_session_token": intermediate_session_token,
             "organization_name": organization_name,
             "organization_slug": organization_slug,
         }
         if session_duration_minutes is not None:
@@ -235,14 +241,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/discovery/organizations/create", data)
         res = await self.async_client.post(url, data)
         return CreateResponse.from_json(res.response.status, res.json)
 
     def list(
         self,
```

### Comparing `stytch-7.0.2/stytch/b2b/api/magic_links.py` & `stytch-7.1.0/stytch/b2b/api/magic_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from stytch.b2b.api.magic_links_discovery import Discovery
 from stytch.b2b.api.magic_links_email import Email
-from stytch.b2b.models.magic_links import AuthenticateResponse
+from stytch.b2b.models.magic_links import (
+    AuthenticateRequestLocale,
+    AuthenticateResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class MagicLinks:
     def __init__(
         self,
@@ -32,14 +35,15 @@
         self,
         magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
 
         Fields:
           - magic_links_token: The Email Magic Link token to authenticate.
           - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
@@ -58,41 +62,45 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "magic_links_token": magic_links_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         magic_links_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a Member with a Magic Link. This endpoint requires a Magic Link token that is not expired or previously used. If the Member’s status is `pending` or `invited`, they will be updated to `active`. Provide the `session_duration_minutes` parameter to set the lifetime of the session. If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
 
         Fields:
           - magic_links_token: The Email Magic Link token to authenticate.
           - pkce_code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_token: Reuse an existing session instead of creating a new one. If you provide a `session_token`, Stytch will update the session.
@@ -111,25 +119,28 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "magic_links_token": magic_links_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/magic_links/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/magic_links_discovery.py` & `stytch-7.1.0/stytch/b2b/api/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/magic_links_email.py` & `stytch-7.1.0/stytch/b2b/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/magic_links_email_discovery.py` & `stytch-7.1.0/stytch/b2b/api/magic_links_email_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/organizations.py` & `stytch-7.1.0/stytch/b2b/api/organizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """Creates an Organization. An `organization_name` and a unique `organization_slug` are required.
 
         By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED` if no Organization authentication settings are explicitly defined in the request.
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
@@ -89,14 +90,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_name": organization_name,
         }
         if organization_slug is not None:
             data["organization_slug"] = organization_slug
         if organization_logo_url is not None:
@@ -111,14 +113,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/organizations", data)
         res = self.sync_client.post(url, data)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
     async def create_async(
         self,
@@ -128,14 +132,15 @@
         trusted_metadata: Optional[Dict[str, Any]] = None,
         sso_jit_provisioning: Optional[str] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> CreateResponse:
         """Creates an Organization. An `organization_name` and a unique `organization_slug` are required.
 
         By default, `email_invites` and `sso_jit_provisioning` will be set to `ALL_ALLOWED` if no Organization authentication settings are explicitly defined in the request.
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
@@ -176,14 +181,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_name": organization_name,
         }
         if organization_slug is not None:
             data["organization_slug"] = organization_slug
         if organization_logo_url is not None:
@@ -198,14 +204,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/organizations", data)
         res = await self.async_client.post(url, data)
         return CreateResponse.from_json(res.response.status, res.json)
 
     def get(
         self,
@@ -252,14 +260,15 @@
         sso_jit_provisioning: Optional[str] = None,
         sso_jit_provisioning_allowed_connections: Optional[List[str]] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> UpdateResponse:
         """Updates an Organization specified by `organization_id`. An Organization must always have at least one auth setting set to either `RESTRICTED` or `ALL_ALLOWED` in order to provision new Members. test
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
@@ -302,14 +311,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if organization_name is not None:
             data["organization_name"] = organization_name
         if organization_slug is not None:
@@ -332,14 +342,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/organizations/{organization_id}", data)
         res = self.sync_client.put(url, data)
         return UpdateResponse.from_json(res.response.status_code, res.json)
 
     async def update_async(
         self,
@@ -352,14 +364,15 @@
         sso_jit_provisioning: Optional[str] = None,
         sso_jit_provisioning_allowed_connections: Optional[List[str]] = None,
         email_allowed_domains: Optional[List[str]] = None,
         email_jit_provisioning: Optional[str] = None,
         email_invites: Optional[str] = None,
         auth_methods: Optional[str] = None,
         allowed_auth_methods: Optional[List[str]] = None,
+        mfa_policy: Optional[str] = None,
     ) -> UpdateResponse:
         """Updates an Organization specified by `organization_id`. An Organization must always have at least one auth setting set to either `RESTRICTED` or `ALL_ALLOWED` in order to provision new Members. test
 
         *See the [Organization authentication settings](https://stytch.com/docs/b2b/api/org-auth-settings) resource to learn more about fields like `email_jit_provisioning`, `email_invites`, `sso_jit_provisioning`, etc., and their behaviors.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
@@ -402,14 +415,15 @@
 
           `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
           - allowed_auth_methods:
           An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
           The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+          - mfa_policy: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if organization_name is not None:
             data["organization_name"] = organization_name
         if organization_slug is not None:
@@ -432,14 +446,16 @@
             data["email_jit_provisioning"] = email_jit_provisioning
         if email_invites is not None:
             data["email_invites"] = email_invites
         if auth_methods is not None:
             data["auth_methods"] = auth_methods
         if allowed_auth_methods is not None:
             data["allowed_auth_methods"] = allowed_auth_methods
+        if mfa_policy is not None:
+            data["mfa_policy"] = mfa_policy
 
         url = self.api_base.url_for("/v1/b2b/organizations/{organization_id}", data)
         res = await self.async_client.put(url, data)
         return UpdateResponse.from_json(res.response.status, res.json)
 
     def delete(
         self,
```

### Comparing `stytch-7.0.2/stytch/b2b/api/organizations_members.py` & `stytch-7.1.0/stytch/b2b/api/organizations_members.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from typing import Any, Dict, List, Optional
 
 from stytch.b2b.models.organizations import SearchQuery
 from stytch.b2b.models.organizations_members import (
     CreateResponse,
     DeletePasswordResponse,
+    DeletePhoneNumberResponse,
     DeleteResponse,
     GetResponse,
     SearchResponse,
     UpdateResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
@@ -36,39 +37,47 @@
         self,
         organization_id: str,
         member_id: str,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         is_breakglass: Optional[bool] = None,
+        phone_number: Optional[str] = None,
+        mfa_enrolled: Optional[bool] = None,
     ) -> UpdateResponse:
         """Updates a Member specified by `organization_id` and `member_id`.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+          - phone_number: (no documentation yet)
+          - mfa_enrolled: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
         if name is not None:
             data["name"] = name
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if is_breakglass is not None:
             data["is_breakglass"] = is_breakglass
+        if phone_number is not None:
+            data["phone_number"] = phone_number
+        if mfa_enrolled is not None:
+            data["mfa_enrolled"] = mfa_enrolled
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members/{member_id}", data
         )
         res = self.sync_client.put(url, data)
         return UpdateResponse.from_json(res.response.status_code, res.json)
 
@@ -76,39 +85,47 @@
         self,
         organization_id: str,
         member_id: str,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         is_breakglass: Optional[bool] = None,
+        phone_number: Optional[str] = None,
+        mfa_enrolled: Optional[bool] = None,
     ) -> UpdateResponse:
         """Updates a Member specified by `organization_id` and `member_id`.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - member_id: Globally unique UUID that identifies a specific Member. The `member_id` is critical to perform operations on a Member, so be sure to preserve this value.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+          - phone_number: (no documentation yet)
+          - mfa_enrolled: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "member_id": member_id,
         }
         if name is not None:
             data["name"] = name
         if trusted_metadata is not None:
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if is_breakglass is not None:
             data["is_breakglass"] = is_breakglass
+        if phone_number is not None:
+            data["phone_number"] = phone_number
+        if mfa_enrolled is not None:
+            data["mfa_enrolled"] = mfa_enrolled
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members/{member_id}", data
         )
         res = await self.async_client.put(url, data)
         return UpdateResponse.from_json(res.response.status, res.json)
 
@@ -152,14 +169,48 @@
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members/{member_id}", data
         )
         res = await self.async_client.delete(url)
         return DeleteResponse.from_json(res.response.status, res.json)
 
+    def delete_phone_number(
+        self,
+        organization_id: str,
+        member_id: str,
+    ) -> DeletePhoneNumberResponse:
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "member_id": member_id,
+        }
+
+        url = self.api_base.url_for(
+            "/v1/b2b/organizations/{organization_id}/members/phone_numbers/{member_id}",
+            data,
+        )
+        res = self.sync_client.delete(url)
+        return DeletePhoneNumberResponse.from_json(res.response.status_code, res.json)
+
+    async def delete_phone_number_async(
+        self,
+        organization_id: str,
+        member_id: str,
+    ) -> DeletePhoneNumberResponse:
+        data: Dict[str, Any] = {
+            "organization_id": organization_id,
+            "member_id": member_id,
+        }
+
+        url = self.api_base.url_for(
+            "/v1/b2b/organizations/{organization_id}/members/phone_numbers/{member_id}",
+            data,
+        )
+        res = await self.async_client.delete(url)
+        return DeletePhoneNumberResponse.from_json(res.response.status, res.json)
+
     def search(
         self,
         organization_ids: List[str],
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
         query: Optional[SearchQuery] = None,
     ) -> SearchResponse:
@@ -269,27 +320,31 @@
         organization_id: str,
         email_address: str,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         create_member_as_pending: Optional[bool] = None,
         is_breakglass: Optional[bool] = None,
+        phone_number: Optional[str] = None,
+        mfa_enrolled: Optional[bool] = None,
     ) -> CreateResponse:
         """Creates a Member. An `organization_id` and `email_address` are required.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - create_member_as_pending: Flag for whether or not to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+          - phone_number: (no documentation yet)
+          - mfa_enrolled: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
         if name is not None:
             data["name"] = name
@@ -297,14 +352,18 @@
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if create_member_as_pending is not None:
             data["create_member_as_pending"] = create_member_as_pending
         if is_breakglass is not None:
             data["is_breakglass"] = is_breakglass
+        if phone_number is not None:
+            data["phone_number"] = phone_number
+        if mfa_enrolled is not None:
+            data["mfa_enrolled"] = mfa_enrolled
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members", data
         )
         res = self.sync_client.post(url, data)
         return CreateResponse.from_json(res.response.status_code, res.json)
 
@@ -313,27 +372,31 @@
         organization_id: str,
         email_address: str,
         name: Optional[str] = None,
         trusted_metadata: Optional[Dict[str, Any]] = None,
         untrusted_metadata: Optional[Dict[str, Any]] = None,
         create_member_as_pending: Optional[bool] = None,
         is_breakglass: Optional[bool] = None,
+        phone_number: Optional[str] = None,
+        mfa_enrolled: Optional[bool] = None,
     ) -> CreateResponse:
         """Creates a Member. An `organization_id` and `email_address` are required.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
           - email_address: The email address of the Member.
           - name: The name of the Member.
           - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
           - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
           frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
           for complete field behavior details.
           - create_member_as_pending: Flag for whether or not to save a Member as `pending` or `active` in Stytch. It defaults to false. If true, new Members will be created with status `pending` in Stytch's backend. Their status will remain `pending` and they will continue to receive signup email templates for every Email Magic Link until that Member authenticates and becomes `active`. If false, new Members will be created with status `active`.
           - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
+          - phone_number: (no documentation yet)
+          - mfa_enrolled: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
         }
         if name is not None:
             data["name"] = name
@@ -341,14 +404,18 @@
             data["trusted_metadata"] = trusted_metadata
         if untrusted_metadata is not None:
             data["untrusted_metadata"] = untrusted_metadata
         if create_member_as_pending is not None:
             data["create_member_as_pending"] = create_member_as_pending
         if is_breakglass is not None:
             data["is_breakglass"] = is_breakglass
+        if phone_number is not None:
+            data["phone_number"] = phone_number
+        if mfa_enrolled is not None:
+            data["mfa_enrolled"] = mfa_enrolled
 
         url = self.api_base.url_for(
             "/v1/b2b/organizations/{organization_id}/members", data
         )
         res = await self.async_client.post(url, data)
         return CreateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/passwords.py` & `stytch-7.1.0/stytch/b2b/api/passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from typing import Any, Dict, Optional
 
 from stytch.b2b.api.passwords_email import Email
 from stytch.b2b.api.passwords_existing_password import ExistingPassword
 from stytch.b2b.api.passwords_session import Sessions
 from stytch.b2b.models.passwords import (
+    AuthenticateRequestLocale,
     AuthenticateResponse,
     MigrateRequestHashType,
     MigrateResponse,
     StrengthCheckResponse,
 )
 from stytch.consumer.models.passwords import (
     Argon2Config,
@@ -227,14 +228,15 @@
         organization_id: str,
         email_address: str,
         password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a member with their email address and password. This endpoint verifies that the member has a password currently set, and that the entered password is correct. There are two instances where the endpoint will return a reset_password error even if they enter their previous password:
         * The member’s credentials appeared in the HaveIBeenPwned dataset.
             * We force a password reset to ensure that the member is the legitimate owner of the email address, and not a malicious actor abusing the compromised credentials.
         * A member that has previously authenticated with email/password uses a passwordless authentication method tied to the same email address (e.g. Magic Links) for the first time. Any subsequent email/password authentication attempt will result in this error.
             * We force a password reset in this instance in order to safely deduplicate the account by email address, without introducing the risk of a pre-hijack account takeover attack.
             * Imagine a bad actor creates many accounts using passwords and the known email addresses of their victims. If a victim comes to the site and logs in for the first time with an email-based passwordless authentication method then both the victim and the bad actor have credentials to access to the same account. To prevent this, any further email/password login attempts first require a password reset which can only be accomplished by someone with access to the underlying email address.
@@ -255,42 +257,46 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         organization_id: str,
         email_address: str,
         password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a member with their email address and password. This endpoint verifies that the member has a password currently set, and that the entered password is correct. There are two instances where the endpoint will return a reset_password error even if they enter their previous password:
         * The member’s credentials appeared in the HaveIBeenPwned dataset.
             * We force a password reset to ensure that the member is the legitimate owner of the email address, and not a malicious actor abusing the compromised credentials.
         * A member that has previously authenticated with email/password uses a passwordless authentication method tied to the same email address (e.g. Magic Links) for the first time. Any subsequent email/password authentication attempt will result in this error.
             * We force a password reset in this instance in order to safely deduplicate the account by email address, without introducing the risk of a pre-hijack account takeover attack.
             * Imagine a bad actor creates many accounts using passwords and the known email addresses of their victims. If a victim comes to the site and logs in for the first time with an email-based passwordless authentication method then both the victim and the bad actor have credentials to access to the same account. To prevent this, any further email/password login attempts first require a password reset which can only be accomplished by someone with access to the underlying email address.
@@ -311,25 +317,28 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
             "email_address": email_address,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/passwords_email.py` & `stytch-7.1.0/stytch/b2b/api/passwords_email.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from stytch.b2b.models.passwords_email import (
+    ResetRequestLocale,
     ResetResponse,
     ResetStartRequestLocale,
     ResetStartResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
@@ -157,14 +158,15 @@
         password_reset_token: str,
         password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         code_verifier: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member's password and authenticate them. This endpoint checks that the password reset token is valid, hasn’t expired, or already been used.
 
         The provided password needs to meet our password strength requirements, which can be checked in advance with the password strength endpoint. If the token and password are accepted, the password is securely stored for future authentication and the user is authenticated.
 
         Fields:
           - password_reset_token: The password reset token to authenticate.
@@ -186,14 +188,15 @@
               and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
               are provided.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "password_reset_token": password_reset_token,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
@@ -201,28 +204,31 @@
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/email/reset", data)
         res = self.sync_client.post(url, data)
         return ResetResponse.from_json(res.response.status_code, res.json)
 
     async def reset_async(
         self,
         password_reset_token: str,
         password: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         code_verifier: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member's password and authenticate them. This endpoint checks that the password reset token is valid, hasn’t expired, or already been used.
 
         The provided password needs to meet our password strength requirements, which can be checked in advance with the password strength endpoint. If the token and password are accepted, the password is securely stored for future authentication and the user is authenticated.
 
         Fields:
           - password_reset_token: The password reset token to authenticate.
@@ -244,14 +250,15 @@
               and `magic_links_token` belong to different Members, the `session_jwt` will be ignored. This endpoint will error if both `session_token` and `session_jwt`
               are provided.
           - code_verifier: A base64url encoded one time secret used to validate that the request starts and ends on the same device.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "password_reset_token": password_reset_token,
             "password": password,
         }
         if session_token is not None:
             data["session_token"] = session_token
@@ -259,11 +266,13 @@
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if code_verifier is not None:
             data["code_verifier"] = code_verifier
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/email/reset", data)
         res = await self.async_client.post(url, data)
         return ResetResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/passwords_existing_password.py` & `stytch-7.1.0/stytch/b2b/api/passwords_existing_password.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
-from stytch.b2b.models.passwords_existing_password import ResetResponse
+from stytch.b2b.models.passwords_existing_password import (
+    ResetRequestLocale,
+    ResetResponse,
+)
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
 
 class ExistingPassword:
     def __init__(
         self,
@@ -30,14 +33,15 @@
         existing_password: str,
         new_password: str,
         organization_id: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member’s password using their existing password.
 
         This endpoint adapts to your Project's password strength configuration.
         If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
         if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
@@ -60,14 +64,15 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "email_address": email_address,
             "existing_password": existing_password,
             "new_password": new_password,
             "organization_id": organization_id,
         }
@@ -75,14 +80,16 @@
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/existing_password/reset", data)
         res = self.sync_client.post(url, data)
         return ResetResponse.from_json(res.response.status_code, res.json)
 
     async def reset_async(
         self,
@@ -90,14 +97,15 @@
         existing_password: str,
         new_password: str,
         organization_id: str,
         session_token: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_jwt: Optional[str] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ResetRequestLocale] = None,
     ) -> ResetResponse:
         """Reset the member’s password using their existing password.
 
         This endpoint adapts to your Project's password strength configuration.
         If you're using [zxcvbn](https://stytch.com/docs/passwords#strength-requirements), the default, your passwords are considered valid
         if the strength score is >= 3. If you're using [LUDS](https://stytch.com/docs/passwords#strength-requirements), your passwords are
         considered valid if they meet the requirements that you've set with Stytch.
@@ -120,14 +128,15 @@
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "email_address": email_address,
             "existing_password": existing_password,
             "new_password": new_password,
             "organization_id": organization_id,
         }
@@ -135,11 +144,13 @@
             data["session_token"] = session_token
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/passwords/existing_password/reset", data)
         res = await self.async_client.post(url, data)
         return ResetResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/passwords_session.py` & `stytch-7.1.0/stytch/b2b/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/sessions.py` & `stytch-7.1.0/stytch/b2b/api/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from stytch.b2b.models.sessions import (
     AuthenticateResponse,
+    ExchangeRequestLocale,
     ExchangeResponse,
     GetJWKSResponse,
     GetResponse,
     RevokeResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
@@ -217,14 +218,15 @@
     def exchange(
         self,
         organization_id: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ExchangeRequestLocale] = None,
     ) -> ExchangeResponse:
         """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
 
         To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
@@ -240,38 +242,42 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
         res = self.sync_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status_code, res.json)
 
     async def exchange_async(
         self,
         organization_id: str,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[ExchangeRequestLocale] = None,
     ) -> ExchangeResponse:
         """Use this endpoint to exchange a Member's existing session for another session in a different Organization. This can be used to accept an invite, but not to create a new member via domain matching.
 
         To create a new member via domain matching, use the [Exchange Intermediate Session](https://stytch.com/docs/b2b/api/exchange-intermediate-session) flow instead.
 
         Fields:
           - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
@@ -287,26 +293,29 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "organization_id": organization_id,
         }
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/sessions/exchange", data)
         res = await self.async_client.post(url, data)
         return ExchangeResponse.from_json(res.response.status, res.json)
 
     def get_jwks(
         self,
```

### Comparing `stytch-7.0.2/stytch/b2b/api/sso.py` & `stytch-7.1.0/stytch/b2b/api/sso.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from stytch.b2b.api.sso_oidc import OIDC
 from stytch.b2b.api.sso_saml import SAML
 from stytch.b2b.models.sso import (
+    AuthenticateRequestLocale,
     AuthenticateResponse,
     DeleteConnectionResponse,
     GetConnectionsResponse,
 )
 from stytch.core.api_base import ApiBase
 from stytch.core.http.client import AsyncClient, SyncClient
 
@@ -114,14 +115,15 @@
         self,
         sso_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a user given a token.
         This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
         Provide the `session_duration_minutes` parameter to set the lifetime of the session.
         If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
         To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
 
@@ -140,41 +142,45 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "sso_token": sso_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/sso/authenticate", data)
         res = self.sync_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status_code, res.json)
 
     async def authenticate_async(
         self,
         sso_token: str,
         pkce_code_verifier: Optional[str] = None,
         session_token: Optional[str] = None,
         session_jwt: Optional[str] = None,
         session_duration_minutes: Optional[int] = None,
         session_custom_claims: Optional[Dict[str, Any]] = None,
+        locale: Optional[AuthenticateRequestLocale] = None,
     ) -> AuthenticateResponse:
         """Authenticate a user given a token.
         This endpoint verifies that the user completed the SSO Authentication flow by verifying that the token is valid and hasn't expired.
         Provide the `session_duration_minutes` parameter to set the lifetime of the session.
         If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration.
         To link this authentication event to an existing Stytch session, include either the `session_token` or `session_jwt` param.
 
@@ -193,25 +199,28 @@
 
           If the `session_duration_minutes` parameter is not specified, a Stytch session will be created with a 60 minute duration. If you don't want
           to use the Stytch session product, you can ignore the session fields in the response.
           - session_custom_claims: Add a custom claims map to the Session being authenticated. Claims are only created if a Session is initialized by providing a value in
           `session_duration_minutes`. Claims will be included on the Session object and in the JWT. To update a key in an existing Session, supply a new value. To
           delete a key, supply a null value. Custom claims made with reserved claims (`iss`, `sub`, `aud`, `exp`, `nbf`, `iat`, `jti`) will be ignored.
           Total custom claims size cannot exceed four kilobytes.
+          - locale: (no documentation yet)
         """  # noqa
         data: Dict[str, Any] = {
             "sso_token": sso_token,
         }
         if pkce_code_verifier is not None:
             data["pkce_code_verifier"] = pkce_code_verifier
         if session_token is not None:
             data["session_token"] = session_token
         if session_jwt is not None:
             data["session_jwt"] = session_jwt
         if session_duration_minutes is not None:
             data["session_duration_minutes"] = session_duration_minutes
         if session_custom_claims is not None:
             data["session_custom_claims"] = session_custom_claims
+        if locale is not None:
+            data["locale"] = locale.value
 
         url = self.api_base.url_for("/v1/b2b/sso/authenticate", data)
         res = await self.async_client.post(url, data)
         return AuthenticateResponse.from_json(res.response.status, res.json)
```

### Comparing `stytch-7.0.2/stytch/b2b/api/sso_oidc.py` & `stytch-7.1.0/stytch/b2b/api/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/api/sso_saml.py` & `stytch-7.1.0/stytch/b2b/api/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/client.py` & `stytch-7.1.0/stytch/consumer/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 
 from typing import Optional
 
-from stytch.b2b.api.discovery import Discovery
-from stytch.b2b.api.magic_links import MagicLinks
-from stytch.b2b.api.organizations import Organizations
-from stytch.b2b.api.passwords import Passwords
-from stytch.b2b.api.sessions import Sessions
-from stytch.b2b.api.sso import SSO
+from stytch.consumer.api.crypto_wallets import CryptoWallets
+from stytch.consumer.api.magic_links import MagicLinks
+from stytch.consumer.api.oauth import OAuth
+from stytch.consumer.api.otp import OTPs
+from stytch.consumer.api.passwords import Passwords
+from stytch.consumer.api.sessions import Sessions
+from stytch.consumer.api.totps import TOTPs
+from stytch.consumer.api.users import Users
+from stytch.consumer.api.webauthn import WebAuthn
 from stytch.core.client_base import ClientBase
 
 
 class Client(ClientBase):
     """
     Stytch API Python client.
 
@@ -28,17 +31,20 @@
         project_id: str,
         secret: str,
         environment: Optional[str] = None,
         suppress_warnings: bool = False,
     ):
         super().__init__(project_id, secret, environment, suppress_warnings)
 
-        self.organizations = Organizations(
+        self.crypto_wallets = CryptoWallets(
             self.api_base, self.sync_client, self.async_client
         )
-        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
-        self.discovery = Discovery(self.api_base, self.sync_client, self.async_client)
         self.magic_links = MagicLinks(
             self.api_base, self.sync_client, self.async_client
         )
+        self.oauth = OAuth(self.api_base, self.sync_client, self.async_client)
+        self.otps = OTPs(self.api_base, self.sync_client, self.async_client)
         self.passwords = Passwords(self.api_base, self.sync_client, self.async_client)
-        self.sso = SSO(self.api_base, self.sync_client, self.async_client)
+        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
+        self.totps = TOTPs(self.api_base, self.sync_client, self.async_client)
+        self.users = Users(self.api_base, self.sync_client, self.async_client)
+        self.webauthn = WebAuthn(self.api_base, self.sync_client, self.async_client)
```

### Comparing `stytch-7.0.2/stytch/b2b/models/discovery.py` & `stytch-7.1.0/stytch/b2b/models/discovery_organizations.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,39 +2,54 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
-
-import pydantic
+from typing import List, Optional
 
+from stytch.b2b.models.discovery import DiscoveredOrganization
 from stytch.b2b.models.organizations import Member, Organization
+from stytch.b2b.models.sessions import MemberSession
+from stytch.core.response_base import ResponseBase
 
 
-class Membership(pydantic.BaseModel):
-    """
+class CreateResponse(ResponseBase):
+    """Response type for `Organizations.create`.
     Fields:
-      - type: Either `active_member`, `pending_member`, `invited_member`, or `eligible_to_join_by_email_domain`
-      - details: An object containing additional metadata about the membership, if available.
-      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object) if one already exists, or null if one does not.
+      - member_id: Globally unique UUID that identifies a specific Member.
+      - session_token: A secret token for a given Stytch Session.
+      - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
+      - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
+      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
     """  # noqa
 
-    type: str
-    details: Optional[Dict[str, Any]] = None
-    member: Optional[Member] = None
+    member_id: str
+    session_token: str
+    session_jwt: str
+    member: Member
+    member_session: Optional[MemberSession] = None
+    organization: Optional[Organization] = None
 
 
-class DiscoveredOrganization(pydantic.BaseModel):
-    """
+class ListResponse(ResponseBase):
+    """Response type for `Organizations.list`.
     Fields:
-      - member_authenticated: Indicates whether or not the discovery magic link initiated session is valid for the organization's allowed auth method settings.
-      If not, the member needs to perform additional authentication before logging in - such as password or SSO auth.
-      - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
-      - membership: Information about the membership.
+      - email_address: The email address.
+      - discovered_organizations: An array of `discovered_organization` objects tied to the `intermediate_session_token`, `session_token`, or `session_jwt`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
+
+      Note that Organizations will only appear here under any of the following conditions:
+      1. The end user is already a Member of the Organization.
+      2. The end user is invited to the Organization.
+      3. The end user can join the Organization because:
+
+          a) The Organization allows JIT provisioning.
+
+          b) The Organizations' allowed domains list contains the Member's email domain.
+
+          c) The Organization has at least one other Member with a verified email address with the same domain as the end user (to prevent phishing attacks).
     """  # noqa
 
-    member_authenticated: bool
-    organization: Optional[Organization] = None
-    membership: Optional[Membership] = None
+    email_address: str
+    discovered_organizations: List[DiscoveredOrganization]
```

### Comparing `stytch-7.0.2/stytch/b2b/models/discovery_intermediate_sessions.py` & `stytch-7.1.0/stytch/b2b/models/discovery_intermediate_sessions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
+import enum
 from typing import Optional
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
+class ExchangeRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class ExchangeResponse(ResponseBase):
     """Response type for `IntermediateSessions.exchange`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
```

### Comparing `stytch-7.0.2/stytch/b2b/models/discovery_organizations.py` & `stytch-7.1.0/stytch/b2b/models/magic_links.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,54 +2,44 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
-from typing import List, Optional
+import enum
 
-from stytch.b2b.models.discovery import DiscoveredOrganization
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
-class CreateResponse(ResponseBase):
-    """Response type for `Organizations.create`.
+class AuthenticateRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
+class AuthenticateResponse(ResponseBase):
+    """Response type for `MagicLinks.authenticate`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
+      - method_id: The email or device involved in the authentication.
+      - reset_sessions: Indicates if all Sessions linked to the Member need to be reset. You should check this field if you aren't using
+        Stytch's Session product. If you are using Stytch's Session product, we revoke the Member’s other Sessions for you.
+      - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
+      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
-      - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - organization: The [Organization object](https://stytch.com/docs/b2b/api/organization-object).
     """  # noqa
 
     member_id: str
+    method_id: str
+    reset_sessions: bool
+    organization_id: str
+    member: Member
     session_token: str
     session_jwt: str
-    member: Member
-    member_session: Optional[MemberSession] = None
-    organization: Optional[Organization] = None
-
-
-class ListResponse(ResponseBase):
-    """Response type for `Organizations.list`.
-    Fields:
-      - email_address: The email address.
-      - discovered_organizations: An array of `discovered_organization` objects tied to the `intermediate_session_token`, `session_token`, or `session_jwt`. See the [Discovered Organization Object](https://stytch.com/docs/b2b/api/discovered-organization-object) for complete details.
-
-      Note that Organizations will only appear here under any of the following conditions:
-      1. The end user is already a Member of the Organization.
-      2. The end user is invited to the Organization.
-      3. The end user can join the Organization because:
-
-          a) The Organization allows JIT provisioning.
-
-          b) The Organizations' allowed domains list contains the Member's email domain.
-
-          c) The Organization has at least one other Member with a verified email address with the same domain as the end user (to prevent phishing attacks).
-    """  # noqa
-
-    email_address: str
-    discovered_organizations: List[DiscoveredOrganization]
+    member_session: MemberSession
+    organization: Organization
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stytch-7.0.2/stytch/b2b/models/magic_links_discovery.py` & `stytch-7.1.0/stytch/b2b/models/magic_links_discovery.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/models/magic_links_email.py` & `stytch-7.1.0/stytch/b2b/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/models/organizations.py` & `stytch-7.1.0/stytch/b2b/models/organizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
       `RESTRICTED` – only methods that comply with `allowed_auth_methods` can be used for authentication. This setting does not apply to Members with `is_breakglass` set to `true`.
 
       - allowed_auth_methods:
       An array of allowed authentication methods. This list is enforced when `auth_methods` is set to `RESTRICTED`.
       The list's accepted values are: `sso`, `magic_link`, `password`, `google_oauth`, and `microsoft_oauth`.
 
+      - mfa_policy: (no documentation yet)
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - sso_default_connection_id: The default connection used for SSO when there are multiple active connections.
     """  # noqa
 
     organization_id: str
     organization_name: str
     organization_logo_url: str
@@ -105,14 +106,15 @@
     sso_jit_provisioning_allowed_connections: List[str]
     sso_active_connections: List[ActiveSSOConnection]
     email_allowed_domains: List[str]
     email_jit_provisioning: str
     email_invites: str
     auth_methods: str
     allowed_auth_methods: List[str]
+    mfa_policy: str
     trusted_metadata: Optional[Dict[str, Any]] = None
     sso_default_connection_id: Optional[str] = None
 
 
 class ResultsMetadata(pydantic.BaseModel):
     """
     Fields:
@@ -147,14 +149,16 @@
       - email_address: The email address of the Member.
       - status: The status of the Member. The possible values are: `pending`, `invited`, `active`, or `deleted`.
       - name: The name of the Member.
       - sso_registrations: An array of registered [SAML Connection](saml-connection-object) objects the Member has authenticated with.
       - is_breakglass: Identifies the Member as a break glass user - someone who has permissions to authenticate into an Organization by bypassing the Organization's settings. A break glass account is typically used for emergency purposes to gain access outside of normal authentication procedures. Refer to the [Organization object](organization-object) and its `auth_methods` and `allowed_auth_methods` fields for more details.
       - member_password_id: Globally unique UUID that identifies a Member's password.
       - oauth_registrations: A list of OAuth registrations for this member.
+      - mfa_enrolled: (no documentation yet)
+      - mfa_phone_number: (no documentation yet)
       - trusted_metadata: An arbitrary JSON object for storing application-specific data or identity-provider-specific data.
       - untrusted_metadata: An arbitrary JSON object of application-specific data. These fields can be edited directly by the
       frontend SDK, and should not be used to store critical information. See the [Metadata resource](https://stytch.com/docs/b2b/api/metadata)
       for complete field behavior details.
     """  # noqa
 
     organization_id: str
@@ -162,14 +166,16 @@
     email_address: str
     status: str
     name: str
     sso_registrations: List[SSORegistration]
     is_breakglass: bool
     member_password_id: str
     oauth_registrations: List[OAuthRegistration]
+    mfa_enrolled: bool
+    mfa_phone_number: str
     trusted_metadata: Optional[Dict[str, Any]] = None
     untrusted_metadata: Optional[Dict[str, Any]] = None
 
 
 class SearchQuery(pydantic.BaseModel):
     """
     Fields:
```

### Comparing `stytch-7.0.2/stytch/b2b/models/organizations_members.py` & `stytch-7.1.0/stytch/b2b/models/organizations_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,20 @@
     """  # noqa
 
     member_id: str
     member: Member
     organization: Organization
 
 
+class DeletePhoneNumberResponse(ResponseBase):
+    member_id: str
+    member: Member
+    organization: Organization
+
+
 class DeleteResponse(ResponseBase):
     """Response type for `Members.delete`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
     """  # noqa
 
     member_id: str
```

### Comparing `stytch-7.0.2/stytch/b2b/models/passwords.py` & `stytch-7.1.0/stytch/b2b/models/passwords.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 import pydantic
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
+class AuthenticateRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class MigrateRequestHashType(enum.Enum):
     BCRYPT = "bcrypt"
     MD_5 = "md_5"
     ARGON_2I = "argon_2i"
     ARGON_2ID = "argon_2id"
     SHA_1 = "sha_1"
     SCRYPT = "scrypt"
```

### Comparing `stytch-7.0.2/stytch/b2b/models/passwords_email.py` & `stytch-7.1.0/stytch/b2b/models/passwords_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 from typing import Optional
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
+class ResetRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class ResetStartRequestLocale(enum.Enum):
     EN = "en"
     ES = "es"
     PTBR = "pt-br"
 
 
 class ResetResponse(ResponseBase):
```

### Comparing `stytch-7.0.2/stytch/b2b/models/passwords_existing_password.py` & `stytch-7.1.0/stytch/b2b/models/passwords_existing_password.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 # WARNING: This file is autogenerated
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
+import enum
 from typing import Optional
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
+class ResetRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class ResetResponse(ResponseBase):
     """Response type for `ExistingPassword.reset`.
     Fields:
       - member_id: Globally unique UUID that identifies a specific Member.
       - member: The [Member object](https://stytch.com/docs/b2b/api/member-object).
       - session_token: A secret token for a given Stytch Session.
       - session_jwt: The JSON Web Token (JWT) for a given Stytch Session.
```

### Comparing `stytch-7.0.2/stytch/b2b/models/passwords_session.py` & `stytch-7.1.0/stytch/b2b/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/models/sessions.py` & `stytch-7.1.0/stytch/b2b/models/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,44 +3,51 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 import datetime
-from typing import Any, Dict, List, Optional
+import enum
+from typing import Any, Dict, List
 
 import pydantic
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.consumer.models.sessions import JWK, AuthenticationFactor
 from stytch.core.response_base import ResponseBase
 
 
+class ExchangeRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class MemberSession(pydantic.BaseModel):
     """
     Fields:
       - member_session_id: Globally unique UUID that identifies a specific Session.
       - member_id: Globally unique UUID that identifies a specific Member.
       - started_at: The timestamp when the Session was created. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - last_accessed_at: The timestamp when the Session was last accessed. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - expires_at: The timestamp when the Session expires. Values conform to the RFC 3339 standard and are expressed in UTC, e.g. `2021-12-29T12:33:09Z`.
       - authentication_factors: An array of different authentication factors that have initiated a Session.
-      - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
       - custom_claims: The custom claims map for a Session. Claims can be added to a session during a Sessions authenticate call.
+      - organization_id: Globally unique UUID that identifies a specific Organization. The `organization_id` is critical to perform operations on an Organization, so be sure to preserve this value.
     """  # noqa
 
     member_session_id: str
     member_id: str
     started_at: datetime.datetime
     last_accessed_at: datetime.datetime
     expires_at: datetime.datetime
     authentication_factors: List[AuthenticationFactor]
+    custom_claims: Dict[str, Any]
     organization_id: str
-    custom_claims: Optional[Dict[str, Any]] = None
 
 
 class AuthenticateResponse(ResponseBase):
     """Response type for `Sessions.authenticate`.
     Fields:
       - member_session: The [Session object](https://stytch.com/docs/b2b/api/session-object).
       - session_token: A secret token for a given Stytch Session.
```

### Comparing `stytch-7.0.2/stytch/b2b/models/sso.py` & `stytch-7.1.0/stytch/b2b/models/sso.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 from __future__ import annotations
 
 import datetime
+import enum
 from typing import Any, Dict, List, Optional
 
 import pydantic
 
 from stytch.b2b.models.organizations import Member, Organization
 from stytch.b2b.models.sessions import MemberSession
 from stytch.core.response_base import ResponseBase
 
 
+class AuthenticateRequestLocale(enum.Enum):
+    EN = "en"
+    ES = "es"
+    PTBR = "pt-br"
+
+
 class OIDCConnection(pydantic.BaseModel):
     organization_id: str
     connection_id: str
     status: str
     display_name: str
     redirect_url: str
     client_id: str
```

### Comparing `stytch-7.0.2/stytch/b2b/models/sso_oidc.py` & `stytch-7.1.0/stytch/b2b/models/sso_oidc.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/b2b/models/sso_saml.py` & `stytch-7.1.0/stytch/b2b/models/sso_saml.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/crypto_wallets.py` & `stytch-7.1.0/stytch/consumer/api/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/magic_links.py` & `stytch-7.1.0/stytch/consumer/api/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/magic_links_email.py` & `stytch-7.1.0/stytch/consumer/api/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/oauth.py` & `stytch-7.1.0/stytch/consumer/api/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/otp.py` & `stytch-7.1.0/stytch/consumer/api/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/otp_email.py` & `stytch-7.1.0/stytch/consumer/api/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/otp_sms.py` & `stytch-7.1.0/stytch/consumer/api/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/otp_whatsapp.py` & `stytch-7.1.0/stytch/consumer/api/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/passwords.py` & `stytch-7.1.0/stytch/consumer/api/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/passwords_email.py` & `stytch-7.1.0/stytch/consumer/api/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/passwords_existing_password.py` & `stytch-7.1.0/stytch/consumer/api/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/passwords_session.py` & `stytch-7.1.0/stytch/consumer/api/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/sessions.py` & `stytch-7.1.0/stytch/consumer/api/sessions.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/totps.py` & `stytch-7.1.0/stytch/consumer/api/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/users.py` & `stytch-7.1.0/stytch/consumer/api/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/api/webauthn.py` & `stytch-7.1.0/stytch/consumer/api/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/client.py` & `stytch-7.1.0/stytch/b2b/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # Only modify code within MANUAL() sections
 # or your changes may be overwritten later!
 # !!!
 
 
 from typing import Optional
 
-from stytch.consumer.api.crypto_wallets import CryptoWallets
-from stytch.consumer.api.magic_links import MagicLinks
-from stytch.consumer.api.oauth import OAuth
-from stytch.consumer.api.otp import OTPs
-from stytch.consumer.api.passwords import Passwords
-from stytch.consumer.api.sessions import Sessions
-from stytch.consumer.api.totps import TOTPs
-from stytch.consumer.api.users import Users
-from stytch.consumer.api.webauthn import WebAuthn
+from stytch.b2b.api.discovery import Discovery
+from stytch.b2b.api.magic_links import MagicLinks
+from stytch.b2b.api.oauth import OAuth
+from stytch.b2b.api.organizations import Organizations
+from stytch.b2b.api.otp import OTPs
+from stytch.b2b.api.passwords import Passwords
+from stytch.b2b.api.sessions import Sessions
+from stytch.b2b.api.sso import SSO
 from stytch.core.client_base import ClientBase
 
 
 class Client(ClientBase):
     """
     Stytch API Python client.
 
@@ -31,20 +30,19 @@
         project_id: str,
         secret: str,
         environment: Optional[str] = None,
         suppress_warnings: bool = False,
     ):
         super().__init__(project_id, secret, environment, suppress_warnings)
 
-        self.users = Users(self.api_base, self.sync_client, self.async_client)
-        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
-        self.crypto_wallets = CryptoWallets(
-            self.api_base, self.sync_client, self.async_client
-        )
+        self.discovery = Discovery(self.api_base, self.sync_client, self.async_client)
         self.magic_links = MagicLinks(
             self.api_base, self.sync_client, self.async_client
         )
-        self.passwords = Passwords(self.api_base, self.sync_client, self.async_client)
         self.oauth = OAuth(self.api_base, self.sync_client, self.async_client)
         self.otps = OTPs(self.api_base, self.sync_client, self.async_client)
-        self.totps = TOTPs(self.api_base, self.sync_client, self.async_client)
-        self.webauthn = WebAuthn(self.api_base, self.sync_client, self.async_client)
+        self.organizations = Organizations(
+            self.api_base, self.sync_client, self.async_client
+        )
+        self.passwords = Passwords(self.api_base, self.sync_client, self.async_client)
+        self.sso = SSO(self.api_base, self.sync_client, self.async_client)
+        self.sessions = Sessions(self.api_base, self.sync_client, self.async_client)
```

### Comparing `stytch-7.0.2/stytch/consumer/models/crypto_wallets.py` & `stytch-7.1.0/stytch/consumer/models/crypto_wallets.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/magic_links.py` & `stytch-7.1.0/stytch/consumer/models/magic_links.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/magic_links_email.py` & `stytch-7.1.0/stytch/consumer/models/magic_links_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/oauth.py` & `stytch-7.1.0/stytch/consumer/models/oauth.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/otp.py` & `stytch-7.1.0/stytch/consumer/models/otp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/otp_email.py` & `stytch-7.1.0/stytch/consumer/models/otp_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/otp_sms.py` & `stytch-7.1.0/stytch/consumer/models/otp_sms.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/otp_whatsapp.py` & `stytch-7.1.0/stytch/consumer/models/otp_whatsapp.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/passwords.py` & `stytch-7.1.0/stytch/consumer/models/passwords.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/passwords_email.py` & `stytch-7.1.0/stytch/consumer/models/passwords_email.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/passwords_existing_password.py` & `stytch-7.1.0/stytch/consumer/models/passwords_existing_password.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/passwords_session.py` & `stytch-7.1.0/stytch/consumer/models/passwords_session.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/sessions.py` & `stytch-7.1.0/stytch/consumer/models/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     OAUTH_TWITCH = "oauth_twitch"
     OAUTH_TWITTER = "oauth_twitter"
     KNOWLEDGE = "knowledge"
     BIOMETRIC = "biometric"
     SSO_SAML = "sso_saml"
     SSO_OIDC = "sso_oidc"
     OAUTH_SALESFORCE = "oauth_salesforce"
+    OAUTH_YAHOO = "oauth_yahoo"
 
 
 class AuthenticationFactorType(enum.Enum):
     MAGIC_LINK = "magic_link"
     OTP = "otp"
     OAUTH = "oauth"
     WEBAUTHN = "webauthn"
@@ -256,14 +257,20 @@
 
 class WebAuthnFactor(pydantic.BaseModel):
     webauthn_registration_id: str
     domain: str
     user_agent: str
 
 
+class YahooOAuthFactor(pydantic.BaseModel):
+    id: str
+    email_id: str
+    provider_subject: str
+
+
 class AuthenticationFactor(pydantic.BaseModel):
     type: AuthenticationFactorType
     delivery_method: AuthenticationFactorDeliveryMethod
     last_authenticated_at: Optional[datetime.datetime] = None
     created_at: Optional[datetime.datetime] = None
     updated_at: Optional[datetime.datetime] = None
     email_factor: Optional[EmailFactor] = None
@@ -294,14 +301,15 @@
     twitch_oauth_factor: Optional[TwitchOAuthFactor] = None
     twitter_oauth_factor: Optional[TwitterOAuthFactor] = None
     embeddable_magic_link_factor: Optional[EmbeddableMagicLinkFactor] = None
     biometric_factor: Optional[BiometricFactor] = None
     saml_sso_factor: Optional[SAMLSSOFactor] = None
     oidc_sso_factor: Optional[OIDCSSOFactor] = None
     salesforce_oauth_factor: Optional[SalesforceOAuthFactor] = None
+    yahoo_oauth_factor: Optional[YahooOAuthFactor] = None
 
     class Config:
         use_enum_values = True
 
 
 class Session(pydantic.BaseModel):
     """
```

### Comparing `stytch-7.0.2/stytch/consumer/models/totps.py` & `stytch-7.1.0/stytch/consumer/models/totps.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/users.py` & `stytch-7.1.0/stytch/consumer/models/users.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/consumer/models/webauthn.py` & `stytch-7.1.0/stytch/consumer/models/webauthn.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/core/api_base.py` & `stytch-7.1.0/stytch/core/api_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/core/client_base.py` & `stytch-7.1.0/stytch/core/client_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/core/http/client.py` & `stytch-7.1.0/stytch/core/http/client.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch/core/response_base.py` & `stytch-7.1.0/stytch/core/response_base.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/stytch.egg-info/PKG-INFO` & `stytch-7.1.0/stytch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stytch
-Version: 7.0.2
+Version: 7.1.0
 Summary: Stytch python client
 Download-URL: https://github.com/stytchauth/stytch-python
 Author: Stytch
 Author-email: hello@stytch.com
 License: MIT
 Keywords: stytch,user,authentication
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stytch-7.0.2/stytch.egg-info/SOURCES.txt` & `stytch-7.1.0/stytch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 stytch/b2b/api/discovery.py
 stytch/b2b/api/discovery_intermediate_sessions.py
 stytch/b2b/api/discovery_organizations.py
 stytch/b2b/api/magic_links.py
 stytch/b2b/api/magic_links_discovery.py
 stytch/b2b/api/magic_links_email.py
 stytch/b2b/api/magic_links_email_discovery.py
+stytch/b2b/api/oauth.py
+stytch/b2b/api/oauth_discovery.py
 stytch/b2b/api/organizations.py
 stytch/b2b/api/organizations_members.py
+stytch/b2b/api/otp.py
+stytch/b2b/api/otp_sms.py
 stytch/b2b/api/passwords.py
 stytch/b2b/api/passwords_email.py
 stytch/b2b/api/passwords_existing_password.py
 stytch/b2b/api/passwords_session.py
 stytch/b2b/api/sessions.py
 stytch/b2b/api/sso.py
 stytch/b2b/api/sso_oidc.py
@@ -33,16 +37,20 @@
 stytch/b2b/models/discovery.py
 stytch/b2b/models/discovery_intermediate_sessions.py
 stytch/b2b/models/discovery_organizations.py
 stytch/b2b/models/magic_links.py
 stytch/b2b/models/magic_links_discovery.py
 stytch/b2b/models/magic_links_email.py
 stytch/b2b/models/magic_links_email_discovery.py
+stytch/b2b/models/mfa.py
+stytch/b2b/models/oauth.py
+stytch/b2b/models/oauth_discovery.py
 stytch/b2b/models/organizations.py
 stytch/b2b/models/organizations_members.py
+stytch/b2b/models/otp_sms.py
 stytch/b2b/models/passwords.py
 stytch/b2b/models/passwords_email.py
 stytch/b2b/models/passwords_existing_password.py
 stytch/b2b/models/passwords_session.py
 stytch/b2b/models/sessions.py
 stytch/b2b/models/sso.py
 stytch/b2b/models/sso_oidc.py
```

### Comparing `stytch-7.0.2/test/test_integration.py` & `stytch-7.1.0/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `stytch-7.0.2/test/test_integration_async.py` & `stytch-7.1.0/test/test_integration_async.py`

 * *Files identical despite different names*

