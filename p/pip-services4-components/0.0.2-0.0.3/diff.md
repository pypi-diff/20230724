# Comparing `tmp/pip_services4_components-0.0.2.tar.gz` & `tmp/pip_services4_components-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_components-0.0.2.tar", last modified: Mon Jul 24 10:07:56 2023, max compression
+gzip compressed data, was "pip_services4_components-0.0.3.tar", last modified: Mon Jul 24 11:16:47 2023, max compression
```

## Comparing `pip_services4_components-0.0.2.tar` & `pip_services4_components-0.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.275069 pip_services4_components-0.0.2/
--rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5480 2023-07-24 10:07:56.275069 pip_services4_components-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.169103 pip_services4_components-0.0.2/pip_services4_components/
--rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.2/pip_services4_components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.195466 pip_services4_components-0.0.2/pip_services4_components/build/
--rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.2/pip_services4_components/build/CompositeFactory.py
--rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.2/pip_services4_components/build/CreateException.py
--rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.2/pip_services4_components/build/Factory.py
--rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.2/pip_services4_components/build/IFactory.py
--rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.2/pip_services4_components/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.205465 pip_services4_components-0.0.2/pip_services4_components/config/
--rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.2/pip_services4_components/config/ConfigParams.py
--rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.2/pip_services4_components/config/IConfigurable.py
--rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.2/pip_services4_components/config/IReconfigurable.py
--rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.2/pip_services4_components/config/NameResolver.py
--rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.2/pip_services4_components/config/OptionsResolver.py
--rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.2/pip_services4_components/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.215468 pip_services4_components-0.0.2/pip_services4_components/context/
--rw-rw-rw-   0        0        0     2414 2023-07-24 07:31:51.000000 pip_services4_components-0.0.2/pip_services4_components/context/Context.py
--rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.2/pip_services4_components/context/ContextInfo.py
--rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.2/pip_services4_components/context/ContextResolver.py
--rw-rw-rw-   0        0        0     1211 2023-07-24 08:08:12.000000 pip_services4_components-0.0.2/pip_services4_components/context/DefaultInfoFactory.py
--rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.2/pip_services4_components/context/IContext.py
--rw-rw-rw-   0        0        0      701 2023-07-21 15:01:50.000000 pip_services4_components-0.0.2/pip_services4_components/context/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.229539 pip_services4_components-0.0.2/pip_services4_components/exec/
--rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/Executor.py
--rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/FixedRateTimer.py
--rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/IExecutable.py
--rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/INotifiable.py
--rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/IParameterized.py
--rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/Notifier.py
--rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/Parameters.py
--rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/exec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.248537 pip_services4_components-0.0.2/pip_services4_components/refer/
--rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/DependencyResolver.py
--rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.2/pip_services4_components/refer/Descriptor.py
--rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/IReferenceable.py
--rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/IReferences.py
--rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/IUnreferenceable.py
--rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/Reference.py
--rw-rw-rw-   0        0        0     1196 2023-07-24 07:50:07.000000 pip_services4_components-0.0.2/pip_services4_components/refer/ReferenceException.py
--rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/Referencer.py
--rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/References.py
--rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/refer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.261547 pip_services4_components-0.0.2/pip_services4_components/run/
--rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/Cleaner.py
--rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/Closer.py
--rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/ICleanable.py
--rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/IClosable.py
--rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/IOpenable.py
--rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/Opener.py
--rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.2/pip_services4_components/run/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.186467 pip_services4_components-0.0.2/pip_services4_components.egg-info/
--rw-rw-rw-   0        0        0     5480 2023-07-24 10:07:56.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2470 2023-07-24 10:07:56.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 10:07:56.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-24 10:07:56.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-07-24 10:07:56.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.2/pip_services4_components.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-24 10:07:56.287071 pip_services4_components-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-07-24 10:06:31.000000 pip_services4_components-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.158118 pip_services4_components-0.0.2/test/
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.264543 pip_services4_components-0.0.2/test/context/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.2/test/context/__init__.py
--rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.2/test/context/test_ContextInfo.py
-drwxrwxrwx   0        0        0        0 2023-07-24 10:07:56.273074 pip_services4_components-0.0.2/test/exec/
--rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.2/test/exec/ClassTest.py
--rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.2/test/exec/__init__.py
--rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.2/test/exec/test_FixedRateTimer.py
--rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.2/test/exec/test_Parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.789438 pip_services4_components-0.0.3/
+-rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5480 2023-07-24 11:16:47.789438 pip_services4_components-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.716437 pip_services4_components-0.0.3/pip_services4_components/
+-rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.3/pip_services4_components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.744439 pip_services4_components-0.0.3/pip_services4_components/build/
+-rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.3/pip_services4_components/build/CompositeFactory.py
+-rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.3/pip_services4_components/build/CreateException.py
+-rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.3/pip_services4_components/build/Factory.py
+-rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.3/pip_services4_components/build/IFactory.py
+-rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.3/pip_services4_components/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.750437 pip_services4_components-0.0.3/pip_services4_components/config/
+-rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.3/pip_services4_components/config/ConfigParams.py
+-rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.3/pip_services4_components/config/IConfigurable.py
+-rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.3/pip_services4_components/config/IReconfigurable.py
+-rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.3/pip_services4_components/config/NameResolver.py
+-rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.3/pip_services4_components/config/OptionsResolver.py
+-rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.3/pip_services4_components/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.756438 pip_services4_components-0.0.3/pip_services4_components/context/
+-rw-rw-rw-   0        0        0     2415 2023-07-24 11:15:53.000000 pip_services4_components-0.0.3/pip_services4_components/context/Context.py
+-rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.3/pip_services4_components/context/ContextInfo.py
+-rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.3/pip_services4_components/context/ContextResolver.py
+-rw-rw-rw-   0        0        0     1211 2023-07-24 08:08:12.000000 pip_services4_components-0.0.3/pip_services4_components/context/DefaultInfoFactory.py
+-rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.3/pip_services4_components/context/IContext.py
+-rw-rw-rw-   0        0        0      701 2023-07-21 15:01:50.000000 pip_services4_components-0.0.3/pip_services4_components/context/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.764438 pip_services4_components-0.0.3/pip_services4_components/exec/
+-rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/Executor.py
+-rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/FixedRateTimer.py
+-rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/IExecutable.py
+-rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/INotifiable.py
+-rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/IParameterized.py
+-rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/Notifier.py
+-rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/Parameters.py
+-rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/exec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.775437 pip_services4_components-0.0.3/pip_services4_components/refer/
+-rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/DependencyResolver.py
+-rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.3/pip_services4_components/refer/Descriptor.py
+-rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/IReferenceable.py
+-rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/IReferences.py
+-rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/IUnreferenceable.py
+-rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/Reference.py
+-rw-rw-rw-   0        0        0     1196 2023-07-24 07:50:07.000000 pip_services4_components-0.0.3/pip_services4_components/refer/ReferenceException.py
+-rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/Referencer.py
+-rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/References.py
+-rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/refer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.782438 pip_services4_components-0.0.3/pip_services4_components/run/
+-rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/Cleaner.py
+-rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/Closer.py
+-rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/ICleanable.py
+-rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/IClosable.py
+-rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/IOpenable.py
+-rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/Opener.py
+-rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.3/pip_services4_components/run/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.738441 pip_services4_components-0.0.3/pip_services4_components.egg-info/
+-rw-rw-rw-   0        0        0     5480 2023-07-24 11:16:47.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2470 2023-07-24 11:16:47.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 11:16:47.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-24 11:16:47.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-07-24 11:16:47.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.3/pip_services4_components.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:16:47.794437 pip_services4_components-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-24 11:16:22.000000 pip_services4_components-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.710437 pip_services4_components-0.0.3/test/
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.784438 pip_services4_components-0.0.3/test/context/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.3/test/context/__init__.py
+-rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.3/test/context/test_ContextInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-24 11:16:47.788437 pip_services4_components-0.0.3/test/exec/
+-rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.3/test/exec/ClassTest.py
+-rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.3/test/exec/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.3/test/exec/test_FixedRateTimer.py
+-rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.3/test/exec/test_Parameters.py
```

### Comparing `pip_services4_components-0.0.2/LICENSE` & `pip_services4_components-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/PKG-INFO` & `pip_services4_components-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_components
-Version: 0.0.2
+Version: 0.0.3
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.2/README.md` & `pip_services4_components-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/build/CompositeFactory.py` & `pip_services4_components-0.0.3/pip_services4_components/build/CompositeFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/build/CreateException.py` & `pip_services4_components-0.0.3/pip_services4_components/build/CreateException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/build/Factory.py` & `pip_services4_components-0.0.3/pip_services4_components/build/Factory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/build/IFactory.py` & `pip_services4_components-0.0.3/pip_services4_components/build/IFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/build/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/ConfigParams.py` & `pip_services4_components-0.0.3/pip_services4_components/config/ConfigParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/IConfigurable.py` & `pip_services4_components-0.0.3/pip_services4_components/config/IConfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/IReconfigurable.py` & `pip_services4_components-0.0.3/pip_services4_components/config/IReconfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/NameResolver.py` & `pip_services4_components-0.0.3/pip_services4_components/config/NameResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/OptionsResolver.py` & `pip_services4_components-0.0.3/pip_services4_components/config/OptionsResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/config/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/context/Context.py` & `pip_services4_components-0.0.3/pip_services4_components/context/Context.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Context(IContext):
     """
     Basic implementation of an execution context.
 
     See :class:`IContext <pip_services4_components.context.IContext.IContext>`
     See :class:`AnyValueMap <pip_services4_commons.data.AnyValueMap.AnyValueMap>`
     """
-    def __int__(self, values: Any):
+    def __init__(self, values: Any):
         """
         Gets a map element specified by its key.
 
         :param values: a key of the element to get.
         :return: the value of the map element.
         """
         self._values = AnyValueMap(values)
```

### Comparing `pip_services4_components-0.0.2/pip_services4_components/context/ContextInfo.py` & `pip_services4_components-0.0.3/pip_services4_components/context/ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/context/ContextResolver.py` & `pip_services4_components-0.0.3/pip_services4_components/context/ContextResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/context/DefaultInfoFactory.py` & `pip_services4_components-0.0.3/pip_services4_components/context/DefaultInfoFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/context/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/context/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/Executor.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/Executor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/FixedRateTimer.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/IExecutable.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/IExecutable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/INotifiable.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/INotifiable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/IParameterized.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/IParameterized.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/Notifier.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/Notifier.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/Parameters.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/Parameters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/exec/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/DependencyResolver.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/DependencyResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/Descriptor.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/Descriptor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/IReferenceable.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/IReferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/IReferences.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/IReferences.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/IUnreferenceable.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/IUnreferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/Reference.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/Reference.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/ReferenceException.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/ReferenceException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/Referencer.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/Referencer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/References.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/References.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/refer/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/refer/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/Cleaner.py` & `pip_services4_components-0.0.3/pip_services4_components/run/Cleaner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/Closer.py` & `pip_services4_components-0.0.3/pip_services4_components/run/Closer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/ICleanable.py` & `pip_services4_components-0.0.3/pip_services4_components/run/ICleanable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/IClosable.py` & `pip_services4_components-0.0.3/pip_services4_components/run/IClosable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/IOpenable.py` & `pip_services4_components-0.0.3/pip_services4_components/run/IOpenable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/Opener.py` & `pip_services4_components-0.0.3/pip_services4_components/run/Opener.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components/run/__init__.py` & `pip_services4_components-0.0.3/pip_services4_components/run/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/pip_services4_components.egg-info/PKG-INFO` & `pip_services4_components-0.0.3/pip_services4_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-components
-Version: 0.0.2
+Version: 0.0.3
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.2/pip_services4_components.egg-info/SOURCES.txt` & `pip_services4_components-0.0.3/pip_services4_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/setup.py` & `pip_services4_components-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_components',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-components-python',
     license='MIT',
     description='Component definitions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `pip_services4_components-0.0.2/test/context/test_ContextInfo.py` & `pip_services4_components-0.0.3/test/context/test_ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/test/exec/test_FixedRateTimer.py` & `pip_services4_components-0.0.3/test/exec/test_FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.2/test/exec/test_Parameters.py` & `pip_services4_components-0.0.3/test/exec/test_Parameters.py`

 * *Files identical despite different names*

