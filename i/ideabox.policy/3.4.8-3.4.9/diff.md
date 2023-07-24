# Comparing `tmp/ideabox.policy-3.4.8.tar.gz` & `tmp/ideabox.policy-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ideabox.policy-3.4.8.tar", last modified: Wed Jun  1 14:26:36 2022, max compression
+gzip compressed data, was "dist/ideabox.policy-3.4.9.tar", last modified: Thu Jun  2 12:46:44 2022, max compression
```

## Comparing `ideabox.policy-3.4.8.tar` & `ideabox.policy-3.4.9.tar`

### file list

```diff
@@ -1,183 +1,188 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       77 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    27714 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      154 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      429 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17834 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2420 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      649 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      337 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/setup.cfg
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/scripts/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4809 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/scripts/data_recovery.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1464 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/scripts/users_recovery.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/scripts/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      195 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1026 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/datasource.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2562 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6935 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/export/export.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      728 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/adapters.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1927 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/testing.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      200 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1434 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/vocabularies.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6911 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/setuphandlers.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2076 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/test_vocabularies.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      702 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/robot/test_project_submission.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1730 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      824 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tests/test_robot.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      103 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/news.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/tests/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4464 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/tests/test_subscriber.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1936 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/subscriber.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3727 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/projects.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3104 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/projects.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5564 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/explorer.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/faceted_query.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3640 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/projets.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5569 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/campaign.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      964 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/news.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2830 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/sort_widget.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/events.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2900 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/news.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2108 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/project_sorting_widget.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2879 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/events.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1589 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/faceted/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/data/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4564 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-theme.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1351 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-locality.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2027 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-iam.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1112 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-district.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4735 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6768 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2036 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1032 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/userschema.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      357 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/workflows.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      274 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/Document.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2310 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/campaign.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2291 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/priority_action.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1992 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/state_progress.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2653 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/Project.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      272 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      511 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      532 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/controlpanel.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/workflows/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/workflows/project_workflow/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20038 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/workflows/project_workflow/definition.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      156 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/viewlets.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      833 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      424 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/memberdata_properties.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1543 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/resources/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      123 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/profiles/resources/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/upgrades.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8665 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4137 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1892 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/userdataschema.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1103 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/viewlets/footer.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      315 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/viewlets/footer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      477 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/viewlets/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3176 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/plone.pot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10538 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/ideabox.policy.pot
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12991 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/LC_MESSAGES/ideabox.policy.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3591 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/LC_MESSAGES/plone.po
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      532 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/locales/update.sh
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3876 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      420 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2971 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1312 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/subscriber.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10447 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/project.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1213 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/indexer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      971 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/syndication.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1354 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/state_progress.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      962 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/state_progress.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      668 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/campaign.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9092 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/project.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2362 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/priority_action.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2748 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/content/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5006 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/vote_encoding.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5187 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/project_encoding.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      595 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4201 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/form/project_submission.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      171 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      285 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/testing.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      598 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/user_menu.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      838 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/project_submission.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2206 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/rating.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1267 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/project_summary.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1994 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/register_form.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2938 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/workflow.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      808 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1701 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/controlpanel.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   340569 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       93 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox.less
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       78 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   189463 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2361 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/comment.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1248 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/overrides/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      620 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/viewlet.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1746 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/project.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      613 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/rating.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1816 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/register.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4238 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      649 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/browser/project_submission.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      608 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/newsletter.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2372 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/projects.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2976 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/priority_action.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1417 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/timeline.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      816 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/newsletter.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2850 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/projects.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2787 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/priority_action.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1239 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/timeline.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2474 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/tile/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2953 2022-06-01 14:26:35.000000 ideabox.policy-3.4.8/src/ideabox/policy/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/top_level.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    27714 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      692 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6234 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       53 2022-06-01 14:26:36.000000 ideabox.policy-3.4.8/src/ideabox.policy.egg-info/entry_points.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       77 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    28079 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      154 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      429 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/README.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18095 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2420 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      649 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      337 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/setup.cfg
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/scripts/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4788 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/scripts/data_recovery.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1464 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/scripts/users_recovery.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/scripts/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      195 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1026 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/datasource.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2562 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6935 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/export/export.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      728 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/adapters.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1927 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/testing.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      200 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1434 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/vocabularies.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6911 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/setuphandlers.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2411 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2076 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/test_vocabularies.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      702 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/robot/test_project_submission.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1730 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      824 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tests/test_robot.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      103 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/news.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/tests/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4464 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/tests/test_subscriber.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1936 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/subscriber.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3727 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/projects.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3104 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/projects.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5564 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/explorer.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/faceted_query.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3640 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/projets.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5569 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/campaign.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      964 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/news.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2830 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/sort_widget.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/events.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2900 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/news.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2108 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/project_sorting_widget.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2879 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/events.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1589 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/faceted/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/data/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4564 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-theme.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1351 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-locality.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2027 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-iam.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1112 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-district.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      124 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4735 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6768 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2036 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1032 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/userschema.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      357 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      274 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2310 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/campaign.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2291 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/priority_action.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1992 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/state_progress.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2653 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/Project.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      272 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      511 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      532 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/controlpanel.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/workflows/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/workflows/project_workflow/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20038 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/workflows/project_workflow/definition.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      156 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/viewlets.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      833 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/rolemap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      424 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/memberdata_properties.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1543 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/resources/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      123 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/profiles/resources/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/upgrades.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8665 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4026 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1892 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/userdataschema.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1103 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/viewlets/footer.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      315 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/viewlets/footer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      477 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/viewlets/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/rest_services/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/rest_services/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      552 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/rest_services/endpoints.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      689 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/rest_services/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3176 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/plone.pot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10538 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/ideabox.policy.pot
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12991 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/LC_MESSAGES/ideabox.policy.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3591 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/LC_MESSAGES/plone.po
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      532 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/locales/update.sh
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3894 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      420 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2971 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1312 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/subscriber.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10936 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/project.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1213 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/indexer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      971 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/syndication.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1354 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/state_progress.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      962 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/state_progress.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      668 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/campaign.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9853 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/project.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2362 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/priority_action.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2748 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/content/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5006 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/vote_encoding.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5187 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/project_encoding.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      595 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4201 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/form/project_submission.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      171 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      285 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/testing.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      598 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/user_menu.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      838 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/project_submission.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2206 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/rating.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1267 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/project_summary.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1994 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/register_form.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2938 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/workflow.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      808 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1701 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/controlpanel.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   340569 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       93 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       78 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   189463 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2361 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/comment.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1248 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/overrides/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      620 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/viewlet.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1746 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/project.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      613 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/rating.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1816 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/register.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4238 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      649 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/browser/project_submission.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      608 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/newsletter.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2372 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/projects.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2976 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/priority_action.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1417 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/timeline.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      816 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/newsletter.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2850 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/projects.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2787 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/priority_action.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1239 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/timeline.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2474 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/tile/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2992 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox/policy/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/top_level.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    28079 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      692 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6412 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       53 2022-06-02 12:46:44.000000 ideabox.policy-3.4.9/src/ideabox.policy.egg-info/entry_points.txt
```

### Comparing `ideabox.policy-3.4.8/PKG-INFO` & `ideabox.policy-3.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ideabox.policy
-Version: 3.4.8
+Version: 3.4.9
 Summary: IdeaBox
 Home-page: https://pypi.python.org/pypi/ideabox.policy
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -30,14 +30,27 @@
         - Maud Gennart [IMIO]
         
         
         Changelog
         =========
         
         
+        3.4.9 (2022-06-02)
+        ------------------
+        
+        - Add endpoints to get projects themes and projects districts
+          [boulch]
+        
+        - Refactor default_image project and take project leadimage in consideration
+          [boulch]
+        
+        - Add map and coordinates in project template
+          [boulch]
+        
+        
         3.4.8 (2022-06-01)
         ------------------
         
         - Add new geolocated faceted view
           [boulch]
         
         - Add geolocation field to project content type
```

### Comparing `ideabox.policy-3.4.8/LICENSE.GPL` & `ideabox.policy-3.4.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/CHANGES.rst` & `ideabox.policy-3.4.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+3.4.9 (2022-06-02)
+------------------
+
+- Add endpoints to get projects themes and projects districts
+  [boulch]
+
+- Refactor default_image project and take project leadimage in consideration
+  [boulch]
+
+- Add map and coordinates in project template
+  [boulch]
+
+
 3.4.8 (2022-06-01)
 ------------------
 
 - Add new geolocated faceted view
   [boulch]
 
 - Add geolocation field to project content type
```

### Comparing `ideabox.policy-3.4.8/setup.py` & `ideabox.policy-3.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="ideabox.policy",
-    version="3.4.8",
+    version="3.4.9",
     description="IdeaBox",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 5.2",
```

### Comparing `ideabox.policy-3.4.8/LICENSE.rst` & `ideabox.policy-3.4.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/scripts/data_recovery.py` & `ideabox.policy-3.4.9/src/ideabox/policy/scripts/data_recovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         project_theme = line[1]
         project_body = line[18]
         project_author = line[3]
         project_mail = line[4]
         project_like = line[15]
         project_unlike = line[16]
 
-        token_type = token_type_recovery(project_theme)
+        token_type = project_theme
 
         if len(project_author) < 3:
             project_author = urlnormalizer.normalize(
                 project_mail[0:3].decode("utf8"), locale="fr"
             )
         else:
             project_author = urlnormalizer.normalize(
```

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/scripts/users_recovery.py` & `ideabox.policy-3.4.9/src/ideabox/policy/scripts/users_recovery.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/export/datasource.py` & `ideabox.policy-3.4.9/src/ideabox/policy/export/datasource.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/export/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/export/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/export/export.py` & `ideabox.policy-3.4.9/src/ideabox/policy/export/export.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/adapters.py` & `ideabox.policy-3.4.9/src/ideabox/policy/adapters.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/testing.py` & `ideabox.policy-3.4.9/src/ideabox/policy/testing.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/vocabularies.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/setuphandlers.py` & `ideabox.policy-3.4.9/src/ideabox/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tests/test_vocabularies.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tests/robot/test_project_submission.robot` & `ideabox.policy-3.4.9/src/ideabox/policy/tests/robot/test_project_submission.robot`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tests/test_setup.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tests/test_robot.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/tests/test_subscriber.py` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/tests/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/subscriber.py` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/subscriber.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/projects.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/projects.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/projects.py` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/projects.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/explorer.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/explorer.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/faceted_query.py` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/faceted_query.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/projets.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/projets.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/campaign.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/campaign.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/config/news.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/config/news.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/sort_widget.py` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/sort_widget.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/news.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/news.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/project_sorting_widget.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/project_sorting_widget.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/events.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/events.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/faceted/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-theme.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-theme.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-locality.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-locality.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-iam.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-iam.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/data/taxonomy-settings-district.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/data/taxonomy-settings-district.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/actions.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/registry.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/catalog.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/userschema.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/userschema.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/campaign.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/campaign.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/priority_action.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/priority_action.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/state_progress.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/state_progress.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/types/Project.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/types/Project.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/controlpanel.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/workflows/project_workflow/definition.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/workflows/project_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/metadata.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/default/rolemap.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/profiles/resources/registry.xml` & `ideabox.policy-3.4.9/src/ideabox/policy/profiles/resources/registry.xml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/upgrades.py` & `ideabox.policy-3.4.9/src/ideabox/policy/upgrades.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/utils.py` & `ideabox.policy-3.4.9/src/ideabox/policy/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,15 @@
 from plone.portlets.constants import CONTEXT_CATEGORY
 from plone.portlets.interfaces import ILocalPortletAssignmentManager
 from plone.portlets.interfaces import IPortletManager
 from zope.component import getMultiAdapter
 from zope.component import getSiteManager
 from zope.component import getUtility
 from zope.i18n import translate
-
-
-def token_type_recovery(value):
-    value = value.decode("utf8")
-    return value
-    # Deprecated ?
-    # from ideabox.policy import vocabularies
-    # vocabulary = vocabularies.ThemeVocabulary(None)
-    # return [
-    #     e.token for e in vocabulary.by_value.values() if translate(e.title) == value
-    # ][0]
+from zope.schema.interfaces import IVocabularyFactory
 
 
 class UnrestrictedUser(BaseUnrestrictedUser):
     """Unrestricted user that still has an id."""
 
     def getId(self):
         """Return the ID of the user."""
@@ -129,7 +119,12 @@
     sm = getSiteManager()
     return sm.queryUtility(ITaxonomy, name="collective.taxonomy.district")
 
 
 def get_theme():
     sm = getSiteManager()
     return sm.queryUtility(ITaxonomy, name="collective.taxonomy.theme")
+
+def get_vocabulary(voc_name):
+    factory = getUtility(IVocabularyFactory, voc_name)
+    vocabulary = factory(api.portal.get())
+    return vocabulary
```

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/userdataschema.py` & `ideabox.policy-3.4.9/src/ideabox/policy/userdataschema.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/viewlets/footer.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/viewlets/footer.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/locales/plone.pot` & `ideabox.policy-3.4.9/src/ideabox/policy/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/locales/ideabox.policy.pot` & `ideabox.policy-3.4.9/src/ideabox/policy/locales/ideabox.policy.pot`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/LC_MESSAGES/ideabox.policy.po` & `ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/LC_MESSAGES/ideabox.policy.po`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/locales/fr/LC_MESSAGES/plone.po` & `ideabox.policy-3.4.9/src/ideabox/policy/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/locales/update.sh` & `ideabox.policy-3.4.9/src/ideabox/policy/locales/update.sh`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/vocabularies.py` & `ideabox.policy-3.4.9/src/ideabox/policy/vocabularies.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,21 +104,21 @@
 SortProjectVocabulary = SortProjectVocabularyFactory()
 
 
 class DistrictVocabularyFactory:
     def __call__(self, context=None):
         district_taxo = get_district()
         language = api.portal.get_current_language(context=context)
-        district_voca = district_taxo.makeVocabulary(language)
+        district_voca = district_taxo.makeVocabulary(language).inv_data
         return district_voca
 
 DistrictVocabulary = DistrictVocabularyFactory()
 
 
 class ThemeVocabularyFactory:
     def __call__(self, context=None):
         theme_taxo = get_theme()
         language = api.portal.get_current_language(context=context)
-        theme_voca = theme_taxo.makeVocabulary(language)
+        theme_voca = theme_taxo.makeVocabulary(language).inv_data
         return theme_voca
 
 ThemeVocabulary = ThemeVocabularyFactory()
```

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/upgrades/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/subscriber.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/subscriber.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/project.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/content/project.pt`

 * *Files 8% similar despite different names*

```diff
@@ -104,14 +104,25 @@
                       </div>
                     </div>
                   </a>
                 </tal:block>
               </div>
             </div>
           </div>
+          <tal:block condition="view/is_geolocated">
+            <tal:widget
+              tal:define="widget python:view.widgets.get('geolocation', None)"
+              tal:replace="structure widget/@@ploneform-render-widget" />
+            <label class="horizontal" i18n:translate="">
+              Coordinates
+            </label>
+            <span tal:content="context/geolocation/latitude" /> ;
+            <span tal:content="context/geolocation/longitude" />
+          </tal:block>
+
           <div>
             <div i18n:translate="" id="ap-comment" class="ap-button">Comment</div>
             <div class="ap-comment ap-toggle" tal:content="structure provider:plone.belowcontentbody" />
           </div>
         </div>
 
         <div tal:condition="python: context.portal_type=='priority_action'" class="ap-state">
```

#### html2text {}

```diff
@@ -5,14 +5,15 @@
 District(s) :
 Edit timeline dates
 Read more
 
 title
 description
 
+   Coordinates   ;
 Comment
 Project Status
 There is no progress for the moment.
 [Image]
 See more
 Would you like to be kept up to date on the progress of the project?
```

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/indexer.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/indexer.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/syndication.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/syndication.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/state_progress.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/content/state_progress.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/state_progress.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/state_progress.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/campaign.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/campaign.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/project.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,17 @@
             "cmf.ModifyPortalContent", obj=self.context, user=api.user.get_current()
         )
 
     @property
     def default_image(self):
         """Try to find the default image for the project, return `None` otherwise"""
         portal = api.portal.get()
+        context = self.context
+        if context.project_image is not None:
+            return "{}/@@images/project_image/large".format(context.absolute_url())
         if "project_default_large.jpg" in portal:
             return portal["project_default_large.jpg"].absolute_url()
 
     @property
     def get_images_url(self):
         contents = self.context.listFolderContents(
             contentFilter={"portal_type": "Image"}
@@ -244,14 +247,17 @@
 
     def get_campaign_image(self):
         parent = self.context.aq_parent
         if parent.portal_type == "campaign" and parent.image:
             return "{0}/@@images/image".format(parent.absolute_url())
         return ""
 
+    def is_geolocated(self):
+        return is_geolocated(self.context)
+
 
 @indexer(IProject)
 def searchabletext_project(object, **kw):
     result = []
 
     fields = ["title", "description", "body", "original_author"]
     for field_name in fields:
@@ -267,7 +273,25 @@
             )
             result.append(text)
         else:
             text = value
             if text:
                 result.append(text)
     return " ".join(result)
+
+
+def is_geolocated(obj):
+    if getattr(obj, "geolocation", None) is not None:
+        if (
+            getattr(obj.geolocation, "latitude", None) is not None
+            and getattr(obj.geolocation, "longitude", None) is not None
+        ):
+            if float(obj.geolocation.latitude) != float(0) and float(
+                obj.geolocation.longitude
+            ) != float(0):
+                return True
+            else:
+                return False
+        else:
+            return False
+    else:
+        return False
```

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/priority_action.py` & `ideabox.policy-3.4.9/src/ideabox/policy/content/priority_action.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/content/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/form/vote_encoding.py` & `ideabox.policy-3.4.9/src/ideabox/policy/form/vote_encoding.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/form/project_encoding.py` & `ideabox.policy-3.4.9/src/ideabox/policy/form/project_encoding.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/form/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/form/project_submission.py` & `ideabox.policy-3.4.9/src/ideabox/policy/form/project_submission.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/user_menu.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/user_menu.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/project_submission.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/project_submission.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/rating.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/rating.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/project_summary.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/project_summary.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/templates/register_form.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/templates/register_form.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/workflow.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/workflow.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/folder.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/folder.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/controlpanel.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox-compiled.js` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox-compiled.js`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/static/ideabox-compiled.css` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/static/ideabox-compiled.css`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/comment.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/comment.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/overrides/plone.app.contenttypes.browser.templates.newsitem.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/viewlet.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/viewlet.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/project.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/project.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/rating.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/rating.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/register.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/register.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/browser/project_submission.py` & `ideabox.policy-3.4.9/src/ideabox/policy/browser/project_submission.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/newsletter.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/newsletter.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/projects.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/projects.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/priority_action.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/priority_action.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/templates/timeline.pt` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/templates/timeline.pt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/newsletter.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/newsletter.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/projects.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/projects.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/priority_action.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/priority_action.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/timeline.py` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/timeline.py`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/tile/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/tile/configure.zcml`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox/policy/configure.zcml` & `ideabox.policy-3.4.9/src/ideabox/policy/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   <include package=".content" />
   <include package=".faceted" />
   <include package=".tile" />
   <include package=".viewlets" />
   <include package=".export" />
   <include package=".form" />
   <include package=".upgrades" />
+  <include package=".rest_services" />
 
   <genericsetup:registerProfile
       name="default"
       title="ideabox.policy"
       directory="profiles/default"
       description="Installs the ideabox.policy add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
```

### Comparing `ideabox.policy-3.4.8/src/ideabox.policy.egg-info/PKG-INFO` & `ideabox.policy-3.4.9/src/ideabox.policy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ideabox.policy
-Version: 3.4.8
+Version: 3.4.9
 Summary: IdeaBox
 Home-page: https://pypi.python.org/pypi/ideabox.policy
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -30,14 +30,27 @@
         - Maud Gennart [IMIO]
         
         
         Changelog
         =========
         
         
+        3.4.9 (2022-06-02)
+        ------------------
+        
+        - Add endpoints to get projects themes and projects districts
+          [boulch]
+        
+        - Refactor default_image project and take project leadimage in consideration
+          [boulch]
+        
+        - Add map and coordinates in project template
+          [boulch]
+        
+        
         3.4.8 (2022-06-01)
         ------------------
         
         - Add new geolocated faceted view
           [boulch]
         
         - Add geolocation field to project content type
```

### Comparing `ideabox.policy-3.4.8/src/ideabox.policy.egg-info/requires.txt` & `ideabox.policy-3.4.9/src/ideabox.policy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ideabox.policy-3.4.8/src/ideabox.policy.egg-info/SOURCES.txt` & `ideabox.policy-3.4.9/src/ideabox.policy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,24 @@
 src/ideabox/policy/profiles/default/types/campaign.xml
 src/ideabox/policy/profiles/default/types/priority_action.xml
 src/ideabox/policy/profiles/default/types/state_progress.xml
 src/ideabox/policy/profiles/default/workflows/project_workflow/definition.xml
 src/ideabox/policy/profiles/resources/metadata.xml
 src/ideabox/policy/profiles/resources/registry.xml
 src/ideabox/policy/profiles/uninstall/browserlayer.xml
+src/ideabox/policy/rest_services/__init__.py
+src/ideabox/policy/rest_services/configure.zcml
+src/ideabox/policy/rest_services/endpoints.py
 src/ideabox/policy/scripts/__init__.py
 src/ideabox/policy/scripts/data_recovery.py
 src/ideabox/policy/scripts/users_recovery.py
 src/ideabox/policy/tests/__init__.py
 src/ideabox/policy/tests/test_robot.py
 src/ideabox/policy/tests/test_setup.py
+src/ideabox/policy/tests/test_utils.py
 src/ideabox/policy/tests/test_vocabularies.py
 src/ideabox/policy/tests/robot/test_project_submission.robot
 src/ideabox/policy/tile/__init__.py
 src/ideabox/policy/tile/configure.zcml
 src/ideabox/policy/tile/newsletter.py
 src/ideabox/policy/tile/priority_action.py
 src/ideabox/policy/tile/projects.py
```

