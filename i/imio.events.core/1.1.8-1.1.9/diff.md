# Comparing `tmp/imio.events.core-1.1.8.tar.gz` & `tmp/imio.events.core-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.events.core-1.1.8.tar", last modified: Tue Jul 18 09:42:30 2023, max compression
+gzip compressed data, was "imio.events.core-1.1.9.tar", last modified: Mon Jul 24 08:35:10 2023, max compression
```

## Comparing `imio.events.core-1.1.8.tar` & `imio.events.core-1.1.9.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3438 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6492 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.957409 imio.events.core-1.1.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      691 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/json_recurrence.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/agenda/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio/events/core/contents/event/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/event/views.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/contents/folder/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/faceted/config/events.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/rest/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3792 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/rest/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_agenda.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14464 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_event.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.961410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.969410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1002_to_1003/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.973410 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio/events/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-18 09:42:30.965410 imio.events.core-1.1.8/src/imio.events.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6492 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4317 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-07-18 09:42:30.000000 imio.events.core-1.1.8/src/imio.events.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3551 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6605 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.849536 imio.events.core-1.1.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1728 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1410 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      691 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/json_recurrence.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/browser/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      850 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio/events/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/contents/agenda/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/agenda/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/agenda/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/agenda/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/contents/entity/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/entity/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/entity/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/entity/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/contents/event/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6641 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/serializer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8341 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4323 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/event/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/converters.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.849536 imio.events.core-1.1.9/src/imio/events/core/faceted/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/faceted/config/events.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.849536 imio.events.core-1.1.9/src/imio/events/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      685 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/taxonomies/event_public.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1386 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1583 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1659 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.857536 imio.events.core-1.1.9/src/imio/events/core/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3792 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/rest/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5607 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/resources/plone.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_agenda.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1573 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_entity.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16337 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_event.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_multilingual.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7479 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3567 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.849536 imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/1002_to_1003/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.861536 imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/1005_to_1006/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3772 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4548 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1006 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio/events/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-07-24 08:35:10.853536 imio.events.core-1.1.9/src/imio.events.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6605 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4355 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-07-24 08:35:10.000000 imio.events.core-1.1.9/src/imio.events.core.egg-info/top_level.txt
```

### Comparing `imio.events.core-1.1.8/CHANGES.rst` & `imio.events.core-1.1.9/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.9 (2023-07-24)
+------------------
+
+- [WEB-3937] Limit event duration to maximum 3 years
+  [boulch, laulaz]
+
+
 1.1.8 (2023-07-18)
 ------------------
 
 - Add logs in endpoint. Help us to find why agenda go slowlier
   [boulch]
```

### Comparing `imio.events.core-1.1.8/DEVELOP.rst` & `imio.events.core-1.1.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/LICENSE.GPL` & `imio.events.core-1.1.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/LICENSE.rst` & `imio.events.core-1.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/PKG-INFO` & `imio.events.core-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-07-24)
+------------------
+
+- [WEB-3937] Limit event duration to maximum 3 years
+  [boulch, laulaz]
+
+
 1.1.8 (2023-07-18)
 ------------------
 
 - Add logs in endpoint. Help us to find why agenda go slowlier
   [boulch]
```

### Comparing `imio.events.core-1.1.8/README.rst` & `imio.events.core-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/docs/conf.py` & `imio.events.core-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/setup.cfg` & `imio.events.core-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/setup.py` & `imio.events.core-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.events.core",
-    version="1.1.8",
+    version="1.1.9",
     description="Core product for iMio events website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.events.core-1.1.8/src/imio/events/core/browser/json_recurrence.py` & `imio.events.core-1.1.9/src/imio/events/core/browser/json_recurrence.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/browser/utils.py` & `imio.events.core-1.1.9/src/imio/events/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/configure.zcml` & `imio.events.core-1.1.9/src/imio/events/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/agenda/content.py` & `imio.events.core-1.1.9/src/imio/events/core/contents/agenda/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/entity/content.py` & `imio.events.core-1.1.9/src/imio/events/core/contents/entity/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/event/configure.zcml` & `imio.events.core-1.1.9/src/imio/events/core/contents/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/event/content.py` & `imio.events.core-1.1.9/src/imio/events/core/contents/event/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/event/serializer.py` & `imio.events.core-1.1.9/src/imio/events/core/contents/event/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/event/view.pt` & `imio.events.core-1.1.9/src/imio/events/core/contents/event/view.pt`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/contents/event/views.py` & `imio.events.core-1.1.9/src/imio/events/core/contents/event/views.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/faceted/config/events.xml` & `imio.events.core-1.1.9/src/imio/events/core/faceted/config/events.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/indexers.py` & `imio.events.core-1.1.9/src/imio/events/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/indexers.zcml` & `imio.events.core-1.1.9/src/imio/events/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/permissions.zcml` & `imio.events.core-1.1.9/src/imio/events/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/catalog.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/metadata.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/registry.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/rolemap.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/taxonomies/event_public.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Event.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml` & `imio.events.core-1.1.9/src/imio/events/core/profiles/default/types/imio.events.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/profiles.zcml` & `imio.events.core-1.1.9/src/imio/events/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/rest/endpoint.py` & `imio.events.core-1.1.9/src/imio/events/core/rest/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/setuphandlers.py` & `imio.events.core-1.1.9/src/imio/events/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/subscribers.py` & `imio.events.core-1.1.9/src/imio/events/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/subscribers.zcml` & `imio.events.core-1.1.9/src/imio/events/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/testing.py` & `imio.events.core-1.1.9/src/imio/events/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/resources/plone.png` & `imio.events.core-1.1.9/src/imio/events/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot` & `imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot` & `imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot` & `imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/robot/test_example.robot` & `imio.events.core-1.1.9/src/imio/events/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_agenda.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_agenda.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_cropping.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_entity.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_event.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # -*- coding: utf-8 -*-
 
 from collective.geolocationbehavior.geolocation import IGeolocatable
-from imio.smartweb.common.utils import geocode_object
+from datetime import datetime
+from imio.events.core.browser.forms import EventCustomAddForm
+from imio.events.core.browser.forms import EventCustomEditForm
 from imio.events.core.contents.event.content import IEvent
 from imio.events.core.interfaces import IImioEventsCoreLayer
 from imio.events.core.testing import IMIO_EVENTS_CORE_INTEGRATION_TESTING
 from imio.events.core.tests.utils import make_named_image
+from imio.smartweb.common.utils import geocode_object
 from plone import api
 from plone.api.exc import InvalidParameterError
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from plone.app.z3cform.interfaces import IPloneFormLayer
 from plone.dexterity.interfaces import IDexterityFTI
 from plone.formwidget.geolocation.geolocation import Geolocation
 from plone.namedfile.file import NamedBlobFile
 from plone.namedfile.file import NamedBlobImage
 from unittest import mock
+from z3c.form.interfaces import WidgetActionExecutionError
 from z3c.relationfield import RelationValue
 from z3c.relationfield.interfaces import IRelationList
 from zope.component import createObject
 from zope.component import getUtility
 from zope.component import getMultiAdapter
 from zope.component import queryMultiAdapter
 from zope.component import queryUtility
 from zope.interface import alsoProvides
 from zope.intid.interfaces import IIntIds
 from zope.lifecycleevent import Attributes
 from zope.lifecycleevent import modified
+from zope.publisher.browser import TestRequest
 from zope.schema.interfaces import IVocabularyFactory
 
 import geopy
+import pytz
 import unittest
 
 
 class TestEvent(unittest.TestCase):
     layer = IMIO_EVENTS_CORE_INTEGRATION_TESTING
 
     def setUp(self):
@@ -395,7 +402,46 @@
             container=event,
             type="File",
             title="file",
         )
         file_obj.file = NamedBlobFile(data="file data", filename="file.txt")
         view = queryMultiAdapter((event, self.request), name="view")
         self.assertIn("++resource++mimetype.icons/txt.png", view())
+
+    def test_timespan_invariant(self):
+        request = TestRequest(
+            form={
+                "form.widgets.IBasic.title": "My Event",
+                "form.widgets.ticket_url": "https://www.kamoulox.be",
+                "form.widgets.IEventBasic.start": "2023-09-01T22:00",
+                "form.widgets.IEventBasic.end": "2050-09-01T22:00",
+                "form.buttons.apply": "Apply",
+            }
+        )
+        alsoProvides(request, IPloneFormLayer)
+        form = EventCustomAddForm(self.folder, request)
+        form.portal_type = "imio.events.Event"
+        form.update()
+        with self.assertRaises(WidgetActionExecutionError):
+            form.handleApply(form, {})
+
+        event = api.content.create(
+            container=self.folder,
+            type="imio.events.Event",
+            id="my-event",
+        )
+        utc_timezone = pytz.UTC
+        event.start = datetime(2023, 9, 1, 22, 00, tzinfo=utc_timezone)
+        event.end = datetime(2024, 9, 1, 22, 00, tzinfo=utc_timezone)
+        request = TestRequest(
+            form={
+                "form.widgets.IEventBasic.start": "2023-09-01T22:00",
+                "form.widgets.IEventBasic.end": "2050-09-01T22:00",
+                "form.buttons.apply": "Apply",
+            }
+        )
+        alsoProvides(request, IPloneFormLayer)
+        form = EventCustomEditForm(event, request)
+        form.portal_type = "imio.events.Event"
+        form.update()
+        with self.assertRaises(WidgetActionExecutionError):
+            form.handleApply(form, {})
```

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_folder.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_indexes.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_local_roles.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_multilingual.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_rest.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_robot.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_setup.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_utils.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/tests/test_vocabularies.py` & `imio.events.core-1.1.9/src/imio/events/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/upgrades/configure.zcml` & `imio.events.core-1.1.9/src/imio/events/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml` & `imio.events.core-1.1.9/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/upgrades/upgrades.py` & `imio.events.core-1.1.9/src/imio/events/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/utils.py` & `imio.events.core-1.1.9/src/imio/events/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/vocabularies.py` & `imio.events.core-1.1.9/src/imio/events/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio/events/core/vocabularies.zcml` & `imio.events.core-1.1.9/src/imio/events/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.1.8/src/imio.events.core.egg-info/PKG-INFO` & `imio.events.core-1.1.9/src/imio.events.core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.9 (2023-07-24)
+------------------
+
+- [WEB-3937] Limit event duration to maximum 3 years
+  [boulch, laulaz]
+
+
 1.1.8 (2023-07-18)
 ------------------
 
 - Add logs in endpoint. Help us to find why agenda go slowlier
   [boulch]
```

### Comparing `imio.events.core-1.1.8/src/imio.events.core.egg-info/SOURCES.txt` & `imio.events.core-1.1.9/src/imio.events.core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/imio/events/core/subscribers.zcml
 src/imio/events/core/testing.py
 src/imio/events/core/utils.py
 src/imio/events/core/vocabularies.py
 src/imio/events/core/vocabularies.zcml
 src/imio/events/core/browser/__init__.py
 src/imio/events/core/browser/configure.zcml
+src/imio/events/core/browser/forms.py
 src/imio/events/core/browser/json_recurrence.py
 src/imio/events/core/browser/utils.py
 src/imio/events/core/browser/overrides/.gitkeep
 src/imio/events/core/browser/static/.gitkeep
 src/imio/events/core/contents/__init__.py
 src/imio/events/core/contents/configure.zcml
 src/imio/events/core/contents/agenda/__init__.py
```

