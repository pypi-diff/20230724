# Comparing `tmp/djangoldp_community-2.3.9.tar.gz` & `tmp/djangoldp_community-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_community-2.3.9.tar", last modified: Thu Sep 15 09:33:39 2022, max compression
+gzip compressed data, was "djangoldp_community-3.0.0.tar", last modified: Mon Jul 24 21:52:42 2023, max compression
```

## Comparing `djangoldp_community-2.3.9.tar` & `djangoldp_community-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/
--rw-rw-rw-   0 root         (0) root         (0)      921 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      293 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community/
--rw-rw-rw-   0 root         (0) root         (0)     1479 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13101 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/tests/tests_model.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)    13126 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/models.py
--rw-rw-rw-   0 root         (0) root         (0)    11129 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2870 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/management/commands/create_community.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-09-15 09:33:37.000000 djangoldp_community-2.3.9/djangoldp_community/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6598 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0011_auto_20220711_0837.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0007_auto_20210324_1146.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0010_auto_20220630_0034.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0002_auto_20210217_1205.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0003_auto_20210218_1145.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0004_auto_20210323_1121.py
--rw-rw-rw-   0 root         (0) root         (0)     4916 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0005_communityaddress_communityprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0009_auto_20220630_0033.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0008_auto_20210415_1744.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2022-09-15 09:33:21.000000 djangoldp_community-2.3.9/djangoldp_community/migrations/0006_auto_20210324_1113.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/
--rw-r--r--   0 root         (0) root         (0)      293 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1533 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      135 2022-09-15 09:33:39.000000 djangoldp_community-2.3.9/djangoldp_community.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.114885 djangoldp_community-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-24 21:52:42.114885 djangoldp_community-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.110885 djangoldp_community-3.0.0/djangoldp_community/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-24 21:52:38.000000 djangoldp_community-3.0.0/djangoldp_community/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.110885 djangoldp_community-3.0.0/djangoldp_community/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.110885 djangoldp_community-3.0.0/djangoldp_community/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/management/commands/create_community.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.110885 djangoldp_community-3.0.0/djangoldp_community/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0002_auto_20210217_1205.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0003_auto_20210218_1145.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0004_auto_20210323_1121.py
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0005_communityaddress_communityprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0006_auto_20210324_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0007_auto_20210324_1146.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0008_auto_20210415_1744.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0009_auto_20220630_0033.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0010_auto_20220630_0034.py
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/0011_auto_20220711_0837.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13205 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11239 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.114885 djangoldp_community-3.0.0/djangoldp_community/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/tests/tests_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    13181 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/djangoldp_community/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:52:42.110885 djangoldp_community-3.0.0/djangoldp_community.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-07-24 21:52:42.000000 djangoldp_community-3.0.0/djangoldp_community.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-24 21:52:42.000000 djangoldp_community-3.0.0/djangoldp_community.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:52:42.000000 djangoldp_community-3.0.0/djangoldp_community.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-24 21:52:42.000000 djangoldp_community-3.0.0/djangoldp_community.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 21:52:42.000000 djangoldp_community-3.0.0/djangoldp_community.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-07-24 21:52:42.114885 djangoldp_community-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 21:52:21.000000 djangoldp_community-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_community-2.3.9/README.md` & `djangoldp_community-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 
 Where:
 
 - `MyModelInline` is the name of your inline class, should be a `admin.StackedInline` or a `admin.TabularInline`.
 - `djangoldp_mypackage` is your package name
 
 You can nest as many inlines as needed.
+
+
+## Changelog
+
+- Now supports Django4.2 and Python3.11
```

### Comparing `djangoldp_community-2.3.9/setup.cfg` & `djangoldp_community-3.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 author_email = jbaptiste@startinblox.com
 description = djangoldp package for circle data models
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
-	djangoldp_account~=2.0
-	djangoldp_circle~=2.1
-	djangoldp_project~=2.1
-	djangoldp_joboffer~=2.0
-	djangoldp_conversation~=2.0
+	djangoldp~=3.0
+	djangoldp_account~=3.0
+	djangoldp_circle~=3.0
+	djangoldp_project~=3.0
+	djangoldp_joboffer~=3.0
+	djangoldp_conversation~=3.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_community/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/views.py` & `djangoldp_community-3.0.0/djangoldp_community/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/tests/tests_permissions.py` & `djangoldp_community-3.0.0/djangoldp_community/tests/tests_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 import json
 from rest_framework.test import APITestCase, APIClient
 
 from djangoldp_community.models import Community, CommunityMember
-from djangoldp_community.tests.models import User
+from djangoldp_account.models import LDPUser as User
 
 
 class PermissionsTestCase(APITestCase):
     # Django runs setUp automatically before every test
     def setUp(self):
         # we set up a client, that allows us
         self.client = APIClient()
@@ -126,19 +126,17 @@
         self.assertEqual(len(members_permissions), 1)
 
     def test_get_communities_is_admin(self):
         self.setUpLoggedInUser(is_superuser=False)
         community = self._get_random_community()
         me = self._get_community_member(user=self.user, community=community, is_admin=True)
 
-        response = self.client.get('/communities/')
+        response = self.client.get('/communities/{}/members/'.format(community.slug))
         self.assertEqual(response.status_code, 200)
-        communities = response.data['ldp:contains']
-        self.assertEqual(len(communities), 1)
-        members_permissions = communities[0]['members']['permissions']
+        members_permissions = response.data['permissions']
         self.assertIn({'mode': {'@type': 'add'}}, members_permissions)
         self.assertIn({'mode': {'@type': 'view'}}, members_permissions)
         self.assertEqual(len(members_permissions), 2)
 
     # only community admins can do any operation on community members
     def test_add_community_member_is_admin(self):
         self.setUpLoggedInUser(is_superuser=False)
@@ -164,16 +162,16 @@
         me = self._get_community_member(user=self.user, community=community, is_admin=False)
 
         body = {
             'http://happy-dev.fr/owl#community': community.urlid,
             'http://happy-dev.fr/owl#user': another_user.urlid
         }
 
-        response = self.client.post('/communities/{}/members/', body=json.dumps(body), content_type='application/ld+json')
-        self.assertEqual(response.status_code, 404)
+        response = self.client.post('/communities/{}/members/'.format(community.slug), body=json.dumps(body), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 403)
 
     # TODO: https://git.startinblox.com/djangoldp-packages/djangoldp-community/issues/3
     '''
     def test_add_community_member_is_admin_no_parent(self):
         self.setUpLoggedInUser(is_superuser=False)
         another_user = self._get_random_user()
 
@@ -243,24 +241,25 @@
         me = self._get_community_member(user=self.user, community=community, is_admin=True)
         member = self._get_community_member(user=another_user, community=community, is_admin=True)
 
         response = self.client.delete('/community-members/{}/'.format(me.pk))
         self.assertEqual(response.status_code, 204)
 
     # community admins cannot remove themselves if they are the last admin
-    def test_delete_self_is_last_admin(self):
-        self.setUpLoggedInUser(is_superuser=False)
-        another_user = self._get_random_user()
+    #TODO: currently, if we prevent the removal of last admin, community cannot be deleted. We need a workaround.
+    # def test_delete_self_is_last_admin(self):
+    #     self.setUpLoggedInUser(is_superuser=False)
+    #     another_user = self._get_random_user()
+
+    #     community = self._get_random_community()
+    #     me = self._get_community_member(user=self.user, community=community, is_admin=True)
+    #     member = self._get_community_member(user=another_user, community=community, is_admin=False)
 
-        community = self._get_random_community()
-        me = self._get_community_member(user=self.user, community=community, is_admin=True)
-        member = self._get_community_member(user=another_user, community=community, is_admin=False)
-
-        response = self.client.delete('/community-members/{}/'.format(me.pk))
-        self.assertEqual(response.status_code, 403)
+    #     response = self.client.delete('/community-members/{}/'.format(me.pk))
+    #     self.assertEqual(response.status_code, 403)
 
     # regular users can remove themselves
     def test_delete_self(self):
         self.setUpLoggedInUser(is_superuser=True)
         another_user = self._get_random_user()
 
         community = self._get_random_community()
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/tests/tests_model.py` & `djangoldp_community-3.0.0/djangoldp_community/tests/tests_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/tests/runner.py` & `djangoldp_community-3.0.0/djangoldp_community/tests/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from django.conf import settings as django_settings
 from djangoldp.conf.ldpsettings import LDPSettings
 from djangoldp.tests.server_settings import yaml_config
 
 # this is where we configure the server settings that we will run our tests with
 config = {
     # add the packages to the reference list
-    'ldppackages': ['modeltranslation', 'djangoldp_circle', 'djangoldp_project', 'djangoldp_conversation', 'djangoldp_community',
-                    'djangoldp_skill', 'djangoldp_joboffer', 'djangoldp_community.tests'],
+    'ldppackages': ['modeltranslation', 'djangoldp_account', 'djangoldp_circle', 'djangoldp_notification',
+                    'djangoldp_project', 'djangoldp_conversation', 'djangoldp_community',
+                    'djangoldp_skill', 'djangoldp_joboffer'],
 
     # required values for server
     'server': {
-        'AUTH_USER_MODEL': 'tests.User',
+        # 'AUTH_USER_MODEL': 'tests.User',
+        'SECRET_KEY': "$r&)p-4k@h5b!1yrft6&q%j)_p$lxqh6#)jeeu0z1iag&y&wdu",
         'REST_FRAMEWORK': {
             'DEFAULT_PAGINATION_CLASS': 'djangoldp.pagination.LDPPagination',
             'PAGE_SIZE': 5
         },
         # map the config of the core settings (avoid asserts to fail)
         'SITE_URL': 'http://happy-dev.fr',
         'BASE_URL': 'http://happy-dev.fr',
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/models.py` & `djangoldp_community-3.0.0/djangoldp_community/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from django.contrib.auth import get_user_model
 from django.conf import settings
 from django.db import models
 from django.db.models.signals import pre_save, post_save, post_delete
 from django.dispatch import receiver
 from djangoldp.models import Model
 from django.utils.text import slugify
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from importlib import import_module
+from django.core.exceptions import ObjectDoesNotExist
 
 from djangoldp_community.permissions import CommunityPermissions, CommunityCirclePermissions, \
     CommunityProjectPermissions, CommunityJobPermissions, CommunityMembersPermissions, \
     CommunityProfilePermissions
 from djangoldp_community.views import CommunityMembersViewset
 
 from djangoldp_circle.models import Circle
@@ -123,14 +124,15 @@
     def __str__(self):
         try:
             return '{} -> {} ({})'.format(self.user.urlid, self.community.urlid, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
+        ordering = ['pk']
         verbose_name = _('community member')
         verbose_name_plural = _("community members")
         view_set = CommunityMembersViewset
         permission_classes = [CommunityMembersPermissions]
         anonymous_perms = ['view']
         authenticated_perms = ['inherit']
         superuser_perms = ['inherit']
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/permissions.py` & `djangoldp_community-3.0.0/djangoldp_community/permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,52 +19,50 @@
 
         return obj.community
 
     def get_object_permissions(self, request, view, obj):
         from djangoldp_community.models import Community, CommunityMember, CommunityProfile, CommunityAddress
 
         perms = set(super().get_object_permissions(request, view, obj))
-        allow_continue = True
         if hasattr(obj, 'project'):
             if (is_authenticated_user(request.user) and not obj.project.members.filter(user=request.user).exists()) or obj.project.status != "Public":
-                allow_continue = False
+                return perms
         elif hasattr(obj, 'circle'):
             if (is_authenticated_user(request.user) and not obj.circle.members.filter(user=request.user).exists()) or obj.circle.status != "Public":
-                allow_continue = False
+                return perms
 
-        if allow_continue:
-            perms = perms.union({'view'})
-
-            community = self._get_community_from_obj(obj)
+        perms = perms.union({'view'})
+        community = self._get_community_from_obj(obj)
 
-            if is_authenticated_user(request.user) and community.members.filter(user=request.user).exists():
-                # Any member can add a job offer, circle or project to the community
-                if not isinstance(obj, Community) and not isinstance(obj, CommunityMember) and\
-                   not isinstance(obj, CommunityProfile) and not isinstance(obj, CommunityAddress):
-                    perms = perms.union({'add'})
+        if is_authenticated_user(request.user) and community.members.filter(user=request.user).exists():
+            # Any member can add a job offer, circle or project to the community
+            if not isinstance(obj, Community) and not isinstance(obj, CommunityMember) and\
+                not isinstance(obj, CommunityProfile) and not isinstance(obj, CommunityAddress):
+                perms = perms.union({'add'})
 
-                member = community.members.get(user=request.user)
-                if member.is_admin:
-                    # Admins can add members
-                    perms = perms.union({'add', 'change'})
-
-                    if isinstance(obj, CommunityMember):
-                        if (obj.user == request.user and community.members.filter(is_admin=True).count() > 1) \
-                                or not obj.is_admin:
-                            # Admins can't delete community or other admins, but have super-powers on everything else
-                            # I can't delete myself if I am the last member
-                            perms = perms.union({'delete'})
-                    elif not isinstance(obj, Community) and not isinstance(obj, CommunityProfile):
+            member = community.members.get(user=request.user)
+            if member.is_admin:
+                # Admins can add members
+                perms = perms.union({'add', 'change'})
+
+                if isinstance(obj, CommunityMember):
+                    if (obj.user == request.user and community.members.filter(is_admin=True).count() > 1) \
+                            or not obj.is_admin:
+                        # Admins can't delete community or other admins, but have super-powers on everything else
+                        # I can't delete myself if I am the last member
                         perms = perms.union({'delete'})
-                elif isinstance(obj, CommunityMember) and obj.user == request.user:
+                elif not isinstance(obj, Community) and not isinstance(obj, CommunityProfile):
                     perms = perms.union({'delete'})
+            elif isinstance(obj, CommunityMember) and obj.user == request.user:
+                perms = perms.union({'delete'})
 
         return perms
 
     def get_container_permissions(self, request, view, obj=None):
+        #TODO: refactor this method. There are object specific checks here, yet there should be only general model level checks
         perms = set({'view'})
         if obj is None:
             resolved = resolve(request.path_info)
             community = None
             if 'slug' in resolved.kwargs and (resolved.url_name == "community-communitycircle-list" \
                 or resolved.url_name == "community-communityproject-list" \
                 or resolved.url_name == "community-communitymember-list" \
@@ -83,15 +81,16 @@
             if community:
                 if is_authenticated_user(request.user) and community.members.filter(user=request.user).exists():
                     if community.members.get(user=request.user).is_admin:
                         perms = perms.union({'add'})
                 if community.allow_self_registration and ('slug' in resolved.kwargs and resolved.url_name == "community-communitymember-list"):
                     perms = perms.union({'add'})
             elif (resolved.url_name == "open-communities-community-list" or resolved.url_name == "community-list"):
-                perms = perms.union({'add'})
+                if(is_authenticated_user(request.user)):
+                    perms = perms.union({'add'})
 
         else:
             perms = self.get_object_permissions(request, view, obj)
 
         return perms
 
 
@@ -158,24 +157,23 @@
 
 class CommunityMembersPermissions(CommunityPermissions):
     filter_backends = []
 
     def get_object_permissions(self, request, view, obj):
         perms = super().get_object_permissions(request, view, obj)
 
-        user = request.user
-
-        if is_authenticated_user(user):
+        if is_authenticated_user(request.user):
+            #TODO: every authenticated user can see all memberships??
             perms = perms.union({'view'})
-            if obj.user == user:
+            if obj.user == request.user:
                 if obj.community.allow_self_registration == True or obj.is_admin:
                     perms = perms.union({'add', 'delete'})
 
-            elif obj.community.members.filter(user=user).count() > 0:
-                if obj.community.members.filter(user=user).get().is_admin:
+            elif obj.community.members.filter(user=request.user).exists():
+                if obj.community.members.get(user=request.user).is_admin and not obj.is_admin:
                     perms = perms.union({'add', 'delete', 'change'})
 
         return perms
 
     def get_container_permissions(self, request, view, obj=None):
         perms = set({'view'})
         if obj is None:
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/admin.py` & `djangoldp_community-3.0.0/djangoldp_community/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from djangoldp.admin import DjangoLDPAdmin
 from djangoldp.models import Model
 from djangoldp_community.models import Community, CommunityMember, CommunityCircle,\
     CommunityProject, CommunityJobOffer, CommunityProfile, CommunityAddress
 from importlib import import_module
 
 
+@admin.register(CommunityAddress, CommunityCircle, CommunityJobOffer, CommunityMember, CommunityProfile, CommunityProject)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class MemberInline(admin.TabularInline):
     model = CommunityMember
@@ -59,14 +60,15 @@
         for module in module_community_inlines:
             module_admin = import_module(module[0])
             community_inlines += [getattr(module_admin, module[1])]
     except:
         pass
 
 
+@admin.register(Community)
 class CommunityAdmin(DjangoLDPAdmin):
     list_display = ('urlid', 'name', 'allow_self_registration')
     exclude = ('urlid', 'slug', 'is_backlink', 'allow_create_backlink')
     inlines = community_inlines
     search_fields = ['urlid', 'name',
                      'members__user__urlid', 'circles__circle__name']
     ordering = ['urlid']
@@ -74,14 +76,7 @@
     def get_queryset(self, request):
         # Hide distant communities
         queryset = super(CommunityAdmin, self).get_queryset(request)
         internal_ids = [x.pk for x in queryset if not Model.is_external(x)]
         return queryset.filter(pk__in=internal_ids)
 
 
-admin.site.register(Community, CommunityAdmin)
-admin.site.register(CommunityMember, EmptyAdmin)
-admin.site.register(CommunityCircle, EmptyAdmin)
-admin.site.register(CommunityProject, EmptyAdmin)
-admin.site.register(CommunityJobOffer, EmptyAdmin)
-admin.site.register(CommunityProfile, EmptyAdmin)
-admin.site.register(CommunityAddress, EmptyAdmin)
```

### Comparing `djangoldp_community-2.3.9/djangoldp_community/management/commands/create_community.py` & `djangoldp_community-3.0.0/djangoldp_community/management/commands/create_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0001_initial.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0011_auto_20220711_0837.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0011_auto_20220711_0837.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0007_auto_20210324_1146.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0007_auto_20210324_1146.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0010_auto_20220630_0034.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0010_auto_20220630_0034.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0002_auto_20210217_1205.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0002_auto_20210217_1205.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0003_auto_20210218_1145.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0003_auto_20210218_1145.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0004_auto_20210323_1121.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0004_auto_20210323_1121.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0005_communityaddress_communityprofile.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0005_communityaddress_communityprofile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community/migrations/0006_auto_20210324_1113.py` & `djangoldp_community-3.0.0/djangoldp_community/migrations/0006_auto_20210324_1113.py`

 * *Files identical despite different names*

### Comparing `djangoldp_community-2.3.9/djangoldp_community.egg-info/SOURCES.txt` & `djangoldp_community-3.0.0/djangoldp_community.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,11 +26,10 @@
 djangoldp_community/migrations/0007_auto_20210324_1146.py
 djangoldp_community/migrations/0008_auto_20210415_1744.py
 djangoldp_community/migrations/0009_auto_20220630_0033.py
 djangoldp_community/migrations/0010_auto_20220630_0034.py
 djangoldp_community/migrations/0011_auto_20220711_0837.py
 djangoldp_community/migrations/__init__.py
 djangoldp_community/tests/__init__.py
-djangoldp_community/tests/models.py
 djangoldp_community/tests/runner.py
 djangoldp_community/tests/tests_model.py
 djangoldp_community/tests/tests_permissions.py
```

