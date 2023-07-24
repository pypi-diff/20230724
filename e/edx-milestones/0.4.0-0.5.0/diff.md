# Comparing `tmp/edx-milestones-0.4.0.tar.gz` & `tmp/edx-milestones-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-milestones-0.4.0.tar", last modified: Tue Feb 22 10:37:22 2022, max compression
+gzip compressed data, was "edx-milestones-0.5.0.tar", last modified: Mon Jul 24 08:42:27 2023, max compression
```

## Comparing `edx-milestones-0.4.0.tar` & `edx-milestones-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/
--rwxr-xr-x   0 runner    (1000) docker     (121)      128 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/AUTHORS
--rwxr-xr-x   0 runner    (1000) docker     (121)    35136 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/LICENSE
--rwxr-xr-x   0 runner    (1000) docker     (121)       92 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker     (121)     4539 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1000) docker     (121)     3736 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/README.md
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/edx_milestones.egg-info/
--rw-r--r--   0 runner    (1000) docker     (121)     4539 2022-02-22 10:37:22.000000 edx-milestones-0.4.0/edx_milestones.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker     (121)     1173 2022-02-22 10:37:22.000000 edx-milestones-0.4.0/edx_milestones.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker     (121)        1 2022-02-22 10:37:22.000000 edx-milestones-0.4.0/edx_milestones.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker     (121)       53 2022-02-22 10:37:22.000000 edx-milestones-0.4.0/edx_milestones.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker     (121)       11 2022-02-22 10:37:22.000000 edx-milestones-0.4.0/edx_milestones.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/
--rw-r--r--   0 runner    (1000) docker     (121)       69 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)      419 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/admin.py
--rw-r--r--   0 runner    (1000) docker     (121)    12504 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/api.py
--rw-r--r--   0 runner    (1000) docker     (121)    19354 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/data.py
--rw-r--r--   0 runner    (1000) docker     (121)     1019 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/exceptions.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/management/
--rw-r--r--   0 runner    (1000) docker     (121)       60 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/management/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/management/commands/
--rw-r--r--   0 runner    (1000) docker     (121)       69 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/management/commands/tests/
--rw-r--r--   0 runner    (1000) docker     (121)       75 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/management/commands/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/migrations/
--rw-r--r--   0 runner    (1000) docker     (121)     5677 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/migrations/0001_initial.py
--rw-r--r--   0 runner    (1000) docker     (121)     1057 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/migrations/0002_data__seed_relationship_types.py
--rw-r--r--   0 runner    (1000) docker     (121)      469 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/migrations/0003_coursecontentmilestone_requirements.py
--rw-r--r--   0 runner    (1000) docker     (121)      919 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/migrations/0004_auto_20151221_1445.py
--rw-r--r--   0 runner    (1000) docker     (121)       62 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/migrations/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)     6759 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/models.py
--rw-r--r--   0 runner    (1000) docker     (121)      475 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/resources.py
--rw-r--r--   0 runner    (1000) docker     (121)     2679 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/serializers.py
--rw-r--r--   0 runner    (1000) docker     (121)     1408 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/services.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/tests/
--rw-r--r--   0 runner    (1000) docker     (121)       47 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/__init__.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/milestones/tests/mocks/
--rw-r--r--   0 runner    (1000) docker     (121)       53 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1000) docker     (121)       71 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/mocks/resources.py
--rw-r--r--   0 runner    (1000) docker     (121)    47445 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/test_api.py
--rw-r--r--   0 runner    (1000) docker     (121)     7085 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/test_data.py
--rw-r--r--   0 runner    (1000) docker     (121)      680 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/test_model.py
--rw-r--r--   0 runner    (1000) docker     (121)     1116 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/test_services.py
--rw-r--r--   0 runner    (1000) docker     (121)     1550 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/tests/utils.py
--rw-r--r--   0 runner    (1000) docker     (121)       61 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/urls.py
--rw-r--r--   0 runner    (1000) docker     (121)     1992 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/validators.py
--rw-r--r--   0 runner    (1000) docker     (121)      305 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/milestones/views.py
-drwxr-xr-x   0 runner    (1000) docker     (121)        0 2022-02-22 10:37:22.417755 edx-milestones-0.4.0/requirements/
--rw-r--r--   0 runner    (1000) docker     (121)      429 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1000) docker     (121)      235 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/requirements/test.in
--rw-r--r--   0 runner    (1000) docker     (121)      126 2022-02-22 10:37:22.421754 edx-milestones-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1000) docker     (121)     2743 2022-02-22 10:37:15.000000 edx-milestones-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.381929 edx-milestones-0.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      128 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/AUTHORS
+-rwxr-xr-x   0 runner    (1001) docker     (122)    35136 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (122)       92 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4519 2023-07-24 08:42:27.381929 edx-milestones-0.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3732 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.373929 edx-milestones-0.5.0/edx_milestones.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4519 2023-07-24 08:42:27.000000 edx-milestones-0.5.0/edx_milestones.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-07-24 08:42:27.000000 edx-milestones-0.5.0/edx_milestones.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 08:42:27.000000 edx-milestones-0.5.0/edx_milestones.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-24 08:42:27.000000 edx-milestones-0.5.0/edx_milestones.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-24 08:42:27.000000 edx-milestones-0.5.0/edx_milestones.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12504 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19354 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/management/commands/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     5677 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/migrations/0002_data__seed_relationship_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/migrations/0003_coursecontentmilestone_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/migrations/0004_auto_20151221_1445.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6733 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.377929 edx-milestones-0.5.0/milestones/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/mocks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47445 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7085 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1992 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/milestones/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 08:42:27.381929 edx-milestones-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-24 08:42:27.381929 edx-milestones-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-24 08:42:20.000000 edx-milestones-0.5.0/setup.py
```

### Comparing `edx-milestones-0.4.0/LICENSE` & `edx-milestones-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/PKG-INFO` & `edx-milestones-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: edx-milestones
-Version: 0.4.0
+Version: 0.5.0
 Summary: Significant events module for Open edX
-Home-page: https://github.com/edx/edx-milestones
+Home-page: https://github.com/openedx/edx-milestones
 Author: edX
 License: AGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-edx-milestones [![Build Status](https://github.com/edx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/edx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
+edx-milestones [![Build Status](https://github.com/openedx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/openedx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
 ===================
 
 edx-milestones (`milestones`) is a Django application which manages significant Course and/or Student events in the Open edX platform.
 
 Usage
 -----
 *  A Milestone represents an event which can occur for a student while interacting with the Open edX platform.
@@ -57,36 +56,34 @@
 ------------------------------------
 
         $ make quality
         $ make test
 
 Open edX Platform Integration
 -----------------------------
-* This package is included in the [base](https://github.com/edx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/edx/edx-platform/)
+* This package is included in the [base](https://github.com/openedx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/openedx/edx-platform/)
 * `milestones` is included in the list of installed apps for edx-platform:
 * These documents outline the feature flags required to enable the features that use edx-milestones.
   * [Course Run prerequisites](https://edx.readthedocs.io/projects/edx-installing-configuring-and-running/en/latest/configuration/enable_prerequisites.html#enable-course-prerequisites)
   * [Subsection prerequisites](https://edx-partner-course-staff.readthedocs.io/en/latest/developing_course/controlling_content_visibility.html#prerequisite-course-subsections)
 
 
 How to Contribute
 -----------------
 Contributions are very welcome please see our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
 
 Getting Help
 ------------
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the community.
 
 Our real-time conversations are on Slack. You can request a [Slack
-invitation](https://openedx-slack-invite.herokuapp.com/), then join our [community Slack team](http://openedx.slack.com/).
+invitation](https://openedx.org/slack), then join our [community Slack team](http://openedx.slack.com/).
 
 For more information about these options, see the [Getting Help](https://openedx.org/getting-help) page.
 
 Reporting Security Issues
 -------------------------
 Please do not report security issues in public. Please email security@edx.org.
-
-
```

### Comparing `edx-milestones-0.4.0/README.md` & `edx-milestones-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-edx-milestones [![Build Status](https://github.com/edx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/edx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
+edx-milestones [![Build Status](https://github.com/openedx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/openedx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
 ===================
 
 edx-milestones (`milestones`) is a Django application which manages significant Course and/or Student events in the Open edX platform.
 
 Usage
 -----
 *  A Milestone represents an event which can occur for a student while interacting with the Open edX platform.
@@ -34,34 +34,34 @@
 ------------------------------------
 
         $ make quality
         $ make test
 
 Open edX Platform Integration
 -----------------------------
-* This package is included in the [base](https://github.com/edx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/edx/edx-platform/)
+* This package is included in the [base](https://github.com/openedx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/openedx/edx-platform/)
 * `milestones` is included in the list of installed apps for edx-platform:
 * These documents outline the feature flags required to enable the features that use edx-milestones.
   * [Course Run prerequisites](https://edx.readthedocs.io/projects/edx-installing-configuring-and-running/en/latest/configuration/enable_prerequisites.html#enable-course-prerequisites)
   * [Subsection prerequisites](https://edx-partner-course-staff.readthedocs.io/en/latest/developing_course/controlling_content_visibility.html#prerequisite-course-subsections)
 
 
 How to Contribute
 -----------------
 Contributions are very welcome please see our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
 
 Getting Help
 ------------
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the community.
 
 Our real-time conversations are on Slack. You can request a [Slack
-invitation](https://openedx-slack-invite.herokuapp.com/), then join our [community Slack team](http://openedx.slack.com/).
+invitation](https://openedx.org/slack), then join our [community Slack team](http://openedx.slack.com/).
 
 For more information about these options, see the [Getting Help](https://openedx.org/getting-help) page.
 
 Reporting Security Issues
 -------------------------
 Please do not report security issues in public. Please email security@edx.org.
```

### Comparing `edx-milestones-0.4.0/edx_milestones.egg-info/PKG-INFO` & `edx-milestones-0.5.0/edx_milestones.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: edx-milestones
-Version: 0.4.0
+Version: 0.5.0
 Summary: Significant events module for Open edX
-Home-page: https://github.com/edx/edx-milestones
+Home-page: https://github.com/openedx/edx-milestones
 Author: edX
 License: AGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-edx-milestones [![Build Status](https://github.com/edx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/edx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
+edx-milestones [![Build Status](https://github.com/openedx/edx-milestones/workflows/Python%20CI/badge.svg?branch=master)](https://github.com/openedx/edx-milestones/actions?query=workflow%3A%22Python+CI%22) [![Coverage Status](https://img.shields.io/coveralls/edx/edx-milestones.svg)](https://coveralls.io/r/edx/edx-milestones?branch=master)
 ===================
 
 edx-milestones (`milestones`) is a Django application which manages significant Course and/or Student events in the Open edX platform.
 
 Usage
 -----
 *  A Milestone represents an event which can occur for a student while interacting with the Open edX platform.
@@ -57,36 +56,34 @@
 ------------------------------------
 
         $ make quality
         $ make test
 
 Open edX Platform Integration
 -----------------------------
-* This package is included in the [base](https://github.com/edx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/edx/edx-platform/)
+* This package is included in the [base](https://github.com/openedx/edx-platform/blob/master/requirements/edx/base.in#L85) requirements of [edx-platform](https://github.com/openedx/edx-platform/)
 * `milestones` is included in the list of installed apps for edx-platform:
 * These documents outline the feature flags required to enable the features that use edx-milestones.
   * [Course Run prerequisites](https://edx.readthedocs.io/projects/edx-installing-configuring-and-running/en/latest/configuration/enable_prerequisites.html#enable-course-prerequisites)
   * [Subsection prerequisites](https://edx-partner-course-staff.readthedocs.io/en/latest/developing_course/controlling_content_visibility.html#prerequisite-course-subsections)
 
 
 How to Contribute
 -----------------
 Contributions are very welcome please see our
-[CONTRIBUTING](https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst)
+[CONTRIBUTING](https://github.com/openedx/.github/blob/master/CONTRIBUTING.md)
 file for more information -- it also contains guidelines for how to maintain
 high code quality, which will make your contribution more likely to be accepted.
 
 Getting Help
 ------------
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the community.
 
 Our real-time conversations are on Slack. You can request a [Slack
-invitation](https://openedx-slack-invite.herokuapp.com/), then join our [community Slack team](http://openedx.slack.com/).
+invitation](https://openedx.org/slack), then join our [community Slack team](http://openedx.slack.com/).
 
 For more information about these options, see the [Getting Help](https://openedx.org/getting-help) page.
 
 Reporting Security Issues
 -------------------------
 Please do not report security issues in public. Please email security@edx.org.
-
-
```

### Comparing `edx-milestones-0.4.0/edx_milestones.egg-info/SOURCES.txt` & `edx-milestones-0.5.0/edx_milestones.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/api.py` & `edx-milestones-0.5.0/milestones/api.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/data.py` & `edx-milestones-0.5.0/milestones/data.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/exceptions.py` & `edx-milestones-0.5.0/milestones/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/migrations/0001_initial.py` & `edx-milestones-0.5.0/milestones/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/migrations/0002_data__seed_relationship_types.py` & `edx-milestones-0.5.0/milestones/migrations/0002_data__seed_relationship_types.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/migrations/0004_auto_20151221_1445.py` & `edx-milestones-0.5.0/milestones/migrations/0004_auto_20151221_1445.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/models.py` & `edx-milestones-0.5.0/milestones/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=no-init
 # pylint: disable=too-few-public-methods
 """
 Database ORM models managed by this Django app
 Please do not integrate directly with these models!!!  This app currently
 offers two APIs -- api.py for direct Python integration and receivers.py,
 which leverages Django's signal framework.
 """
```

### Comparing `edx-milestones-0.4.0/milestones/serializers.py` & `edx-milestones-0.5.0/milestones/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/services.py` & `edx-milestones-0.5.0/milestones/services.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/tests/test_api.py` & `edx-milestones-0.5.0/milestones/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/tests/test_data.py` & `edx-milestones-0.5.0/milestones/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/tests/test_model.py` & `edx-milestones-0.5.0/milestones/tests/test_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     def test_check_model_str(self):
         """
         checking model str methods
         """
         milestone_relation_ship = MilestoneRelationshipType.objects.create(name='milestone_relation_ship')
         milestone = Milestone.objects.create(namespace='milestone')
 
-        self.assertEqual(milestone_relation_ship.__str__(), 'milestone_relation_ship')
-        self.assertEqual(milestone.__str__(), 'milestone')
+        self.assertEqual(str(milestone_relation_ship), 'milestone_relation_ship')
+        self.assertEqual(str(milestone), 'milestone')
```

### Comparing `edx-milestones-0.4.0/milestones/tests/test_services.py` & `edx-milestones-0.5.0/milestones/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/tests/utils.py` & `edx-milestones-0.5.0/milestones/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/milestones/validators.py` & `edx-milestones-0.5.0/milestones/validators.py`

 * *Files identical despite different names*

### Comparing `edx-milestones-0.4.0/setup.py` & `edx-milestones-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,26 @@
 setup(
     name='edx-milestones',
     version=VERSION,
     description='Significant events module for Open edX',
     long_description=open('README.md', encoding='utf-8').read(),  # pylint: disable=consider-using-with
     long_description_content_type="text/markdown",
     author='edX',
-    url='https://github.com/edx/edx-milestones',
+    url='https://github.com/openedx/edx-milestones',
     license='AGPL',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
     ],
     packages=find_packages(exclude=["tests"]),
     install_requires=load_requirements('requirements/base.in'),
     tests_require=load_requirements('requirements/test.in')
 )
```

