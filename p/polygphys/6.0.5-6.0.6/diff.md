# Comparing `tmp/polygphys-6.0.5.tar.gz` & `tmp/polygphys-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygphys-6.0.5.tar", last modified: Tue Jun 20 12:44:42 2023, max compression
+gzip compressed data, was "polygphys-6.0.6.tar", last modified: Mon Jul 24 13:16:36 2023, max compression
```

## Comparing `polygphys-6.0.5.tar` & `polygphys-6.0.6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.856296 polygphys-6.0.5/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-06-20 12:44:42.856501 polygphys-6.0.5/PKG-INFO
--rw-r--r--   0 emilejetzer   (501) staff       (20)      120 2022-03-03 18:41:47.000000 polygphys-6.0.5/pyproject.toml
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5477 2022-04-05 17:13:17.000000 polygphys-6.0.5/readme.md
--rw-r--r--   0 emilejetzer   (501) staff       (20)      976 2023-06-20 12:44:42.857468 polygphys-6.0.5/setup.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)      179 2022-01-12 21:30:35.000000 polygphys-6.0.5/setup.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.783305 polygphys-6.0.5/src/
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.793734 polygphys-6.0.5/src/polygphys/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/__main__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.796896 polygphys-6.0.5/src/polygphys/admin/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/admin/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.799526 polygphys-6.0.5/src/polygphys/admin/heures/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3112 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/exporter.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       40 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/heures.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2506 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/heures.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.802509 polygphys-6.0.5/src/polygphys/admin/inventaire/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      424 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/default.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.807113 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     7228 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/importer.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1722 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/script.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)       51 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_argv.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2681 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_foreignkey.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4099 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/inventaire.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5913 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/modeles.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.810058 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      248 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1340 2022-08-17 21:05:30.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/script_zotero.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2790 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/zotero.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.811185 polygphys-6.0.5/src/polygphys/atelier/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/atelier/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.814216 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:05:31.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3978 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/assistant_gui.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1810 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/gcode.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     3805 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_svg.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)      989 2022-07-12 22:05:31.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_trous.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     2998 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_xlsx.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.815884 polygphys-6.0.5/src/polygphys/outils/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/__main__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.817965 polygphys-6.0.5/src/polygphys/outils/appareils/
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.821020 polygphys-6.0.5/src/polygphys/outils/appareils/HP/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5662 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_dev.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)    26130 2023-04-05 13:58:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_lab.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       44 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.823208 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/lab.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2148 2023-04-04 15:27:54.000000 polygphys-6.0.5/src/polygphys/outils/appareils/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       24 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       75 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/phs8302.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.829692 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    19409 2022-11-24 21:26:10.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1393 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       81 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4420 2022-11-11 21:24:31.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/dtypes.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      806 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/gestion.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3503 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/modeles.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.834150 polygphys-6.0.5/src/polygphys/outils/config/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    11277 2023-03-08 16:35:11.000000 polygphys-6.0.5/src/polygphys/outils/config/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1079 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      273 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/json.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      113 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/toml.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/yaml.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.836634 polygphys-6.0.5/src/polygphys/outils/interface_graphique/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1367 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       64 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4678 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/html.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    10018 2022-07-12 20:31:46.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tableau.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.838619 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3263 2022-10-11 20:31:37.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       59 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    18300 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/onglets.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     7480 2023-06-20 12:43:39.000000 polygphys-6.0.5/src/polygphys/outils/journal.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.842295 polygphys-6.0.5/src/polygphys/outils/reseau/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9197 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      172 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    15918 2023-03-31 20:31:02.000000 polygphys-6.0.5/src/polygphys/outils/reseau/courriel.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4021 2022-11-16 15:28:42.000000 polygphys-6.0.5/src/polygphys/outils/reseau/msforms.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.842930 polygphys-6.0.5/src/polygphys/outils/reseau/serveur/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2405 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/serveur/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.846218 polygphys-6.0.5/src/polygphys/serveur/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9705 2022-11-09 22:44:53.000000 polygphys-6.0.5/src/polygphys/serveur/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1565 2022-11-09 22:46:26.000000 polygphys-6.0.5/src/polygphys/serveur/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2339 2022-11-09 22:10:40.000000 polygphys-6.0.5/src/polygphys/serveur/nouveau_script.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      102 2022-11-09 21:36:04.000000 polygphys-6.0.5/src/polygphys/serveur/serveur.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.847052 polygphys-6.0.5/src/polygphys/sst/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/sst/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.849905 polygphys-6.0.5/src/polygphys/sst/certificats_laser/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:49.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1096 2022-07-12 22:04:49.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9741 2022-09-23 19:39:17.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificats.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1304 2022-07-12 22:07:57.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/vérifier.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.852129 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:26.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)      652 2022-07-12 22:04:26.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscription.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3821 2022-09-22 11:30:09.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.855644 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1450 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2744 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.796345 polygphys-6.0.5/src/polygphys.egg-info/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/PKG-INFO
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3800 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/SOURCES.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)        1 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/dependency_links.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)      342 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/requires.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)       10 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/top_level.txt
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.739812 polygphys-6.0.6/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-07-24 13:16:36.740040 polygphys-6.0.6/PKG-INFO
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      120 2022-03-03 18:41:47.000000 polygphys-6.0.6/pyproject.toml
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5477 2022-04-05 17:13:17.000000 polygphys-6.0.6/readme.md
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      976 2023-07-24 13:16:36.741575 polygphys-6.0.6/setup.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      179 2022-01-12 21:30:35.000000 polygphys-6.0.6/setup.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.673574 polygphys-6.0.6/src/
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.682212 polygphys-6.0.6/src/polygphys/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/__main__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.684893 polygphys-6.0.6/src/polygphys/admin/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/admin/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.687425 polygphys-6.0.6/src/polygphys/admin/heures/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:02:35.000000 polygphys-6.0.6/src/polygphys/admin/heures/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3112 2022-07-12 22:02:35.000000 polygphys-6.0.6/src/polygphys/admin/heures/exporter.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       40 2022-07-12 22:02:35.000000 polygphys-6.0.6/src/polygphys/admin/heures/heures.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2506 2022-07-12 22:02:35.000000 polygphys-6.0.6/src/polygphys/admin/heures/heures.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.689787 polygphys-6.0.6/src/polygphys/admin/inventaire/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      424 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/default.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.693402 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     7228 2022-08-19 17:01:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/importer.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1722 2022-08-19 17:01:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/script.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)       51 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/test_argv.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2681 2022-08-19 17:01:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/importer/test_foreignkey.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4099 2022-08-19 17:01:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/inventaire.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5913 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/modeles.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.695564 polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      248 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1340 2022-08-17 21:05:30.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/script_zotero.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2790 2022-07-12 22:03:51.000000 polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/zotero.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.696162 polygphys-6.0.6/src/polygphys/atelier/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/atelier/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.699355 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:05:31.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3978 2022-09-07 18:34:40.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/assistant_gui.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1810 2022-09-07 18:34:40.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/gcode.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     3805 2022-09-07 18:34:40.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_svg.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)      989 2022-07-12 22:05:31.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_trous.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     2998 2022-09-07 18:34:40.000000 polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_xlsx.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.701309 polygphys-6.0.6/src/polygphys/outils/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/__main__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.703173 polygphys-6.0.6/src/polygphys/outils/appareils/
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.706234 polygphys-6.0.6/src/polygphys/outils/appareils/HP/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5662 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/HP/HP4274A_dev.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)    26130 2023-04-05 13:58:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/HP/HP4274A_lab.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       44 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/HP/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.708011 polygphys-6.0.6/src/polygphys/outils/appareils/Thorlabs/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/Thorlabs/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/Thorlabs/lab.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2148 2023-04-04 15:27:54.000000 polygphys-6.0.6/src/polygphys/outils/appareils/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       24 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       75 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/appareils/phs8302.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.714670 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    19409 2022-11-24 21:26:10.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1393 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       81 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4420 2022-11-11 21:24:31.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/dtypes.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      806 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/gestion.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3503 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/base_de_donnees/modeles.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.718993 polygphys-6.0.6/src/polygphys/outils/config/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    11277 2023-03-08 16:35:11.000000 polygphys-6.0.6/src/polygphys/outils/config/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1079 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/config/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      273 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/config/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/config/json.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      113 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/config/toml.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/config/yaml.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.721335 polygphys-6.0.6/src/polygphys/outils/interface_graphique/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1367 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       64 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4678 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/html.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    10018 2022-07-12 20:31:46.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/tableau.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.723545 polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3263 2022-10-11 20:31:37.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       59 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    18300 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/onglets.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     7482 2023-07-24 13:15:23.000000 polygphys-6.0.6/src/polygphys/outils/journal.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.727631 polygphys-6.0.6/src/polygphys/outils/reseau/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9197 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/reseau/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      172 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/reseau/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    15918 2023-03-31 20:31:02.000000 polygphys-6.0.6/src/polygphys/outils/reseau/courriel.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4021 2022-11-16 15:28:42.000000 polygphys-6.0.6/src/polygphys/outils/reseau/msforms.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.728380 polygphys-6.0.6/src/polygphys/outils/reseau/serveur/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2405 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/outils/reseau/serveur/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.730497 polygphys-6.0.6/src/polygphys/serveur/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9708 2023-07-24 12:52:28.000000 polygphys-6.0.6/src/polygphys/serveur/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1565 2022-11-09 22:46:26.000000 polygphys-6.0.6/src/polygphys/serveur/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2339 2022-11-09 22:10:40.000000 polygphys-6.0.6/src/polygphys/serveur/nouveau_script.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      102 2022-11-09 21:36:04.000000 polygphys-6.0.6/src/polygphys/serveur/serveur.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.731050 polygphys-6.0.6/src/polygphys/sst/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.6/src/polygphys/sst/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.733965 polygphys-6.0.6/src/polygphys/sst/certificats_laser/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:49.000000 polygphys-6.0.6/src/polygphys/sst/certificats_laser/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1096 2022-07-12 22:04:49.000000 polygphys-6.0.6/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9741 2022-09-23 19:39:17.000000 polygphys-6.0.6/src/polygphys/sst/certificats_laser/nouveau_certificats.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1304 2022-07-12 22:07:57.000000 polygphys-6.0.6/src/polygphys/sst/certificats_laser/vérifier.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.736151 polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:26.000000 polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)      652 2022-07-12 22:04:26.000000 polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/inscription.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3821 2022-09-22 11:30:09.000000 polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.739058 polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:15.000000 polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1450 2022-07-12 22:03:15.000000 polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2744 2022-07-12 22:03:15.000000 polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-07-24 13:16:36.684398 polygphys-6.0.6/src/polygphys.egg-info/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-07-24 13:16:36.000000 polygphys-6.0.6/src/polygphys.egg-info/PKG-INFO
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3800 2023-07-24 13:16:36.000000 polygphys-6.0.6/src/polygphys.egg-info/SOURCES.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)        1 2023-07-24 13:16:36.000000 polygphys-6.0.6/src/polygphys.egg-info/dependency_links.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      342 2023-07-24 13:16:36.000000 polygphys-6.0.6/src/polygphys.egg-info/requires.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       10 2023-07-24 13:16:36.000000 polygphys-6.0.6/src/polygphys.egg-info/top_level.txt
```

### Comparing `polygphys-6.0.5/PKG-INFO` & `polygphys-6.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygphys
-Version: 6.0.5
+Version: 6.0.6
 Summary: Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 Author: Émile Jetzer
 Author-email: emile.jetzer@polymtl.ca
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Outils & programmes du département de génie physique de Polytechnique [![Python application](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml) [![CodeQL](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml) [![Upload Python Package](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml) [![Documentation Status](https://readthedocs.org/projects/polygphys/badge/?version=latest)](https://polygphys.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `polygphys-6.0.5/readme.md` & `polygphys-6.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/setup.cfg` & `polygphys-6.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = polygphys
-version = 6.0.5
+version = 6.0.6
 description = Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 author = Émile Jetzer
 author_email = emile.jetzer@polymtl.ca
 long_description = file: readme.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `polygphys-6.0.5/src/polygphys/admin/heures/exporter.py` & `polygphys-6.0.6/src/polygphys/admin/heures/exporter.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/heures/heures.py` & `polygphys-6.0.6/src/polygphys/admin/heures/heures.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/importer.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/importer/importer.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/script.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/importer/script.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_foreignkey.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/importer/test_foreignkey.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/inventaire.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/inventaire.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/modeles.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/modeles.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/script_zotero.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/script_zotero.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/zotero.py` & `polygphys-6.0.6/src/polygphys/admin/inventaire/zotero/zotero.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/assistant_gui.py` & `polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/assistant_gui.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/gcode.py` & `polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/gcode.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_svg.py` & `polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_svg.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_trous.py` & `polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_trous.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_xlsx.py` & `polygphys-6.0.6/src/polygphys/atelier/assistant_gcode/script_xlsx.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_dev.py` & `polygphys-6.0.6/src/polygphys/outils/appareils/HP/HP4274A_dev.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_lab.py` & `polygphys-6.0.6/src/polygphys/outils/appareils/HP/HP4274A_lab.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/appareils/Thorlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/lab.py` & `polygphys-6.0.6/src/polygphys/outils/appareils/Thorlabs/lab.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/appareils/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/appareils/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/base_de_donnees/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__main__.py` & `polygphys-6.0.6/src/polygphys/outils/base_de_donnees/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/dtypes.py` & `polygphys-6.0.6/src/polygphys/outils/base_de_donnees/dtypes.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/gestion.py` & `polygphys-6.0.6/src/polygphys/outils/base_de_donnees/gestion.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/modeles.py` & `polygphys-6.0.6/src/polygphys/outils/base_de_donnees/modeles.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/config/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/config/__main__.py` & `polygphys-6.0.6/src/polygphys/outils/config/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/interface_graphique/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/interface_graphique/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/interface_graphique/html.py` & `polygphys-6.0.6/src/polygphys/outils/interface_graphique/html.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tableau.py` & `polygphys-6.0.6/src/polygphys/outils/interface_graphique/tableau.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/onglets.py` & `polygphys-6.0.6/src/polygphys/outils/interface_graphique/tkinter/onglets.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/journal.py` & `polygphys-6.0.6/src/polygphys/outils/journal.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,12 +322,12 @@
         if csv.exists():
             en_têtes = False
         else:
             en_têtes = True
             csv.touch()
 
         message.to_csv(csv, mode='a', header=en_têtes, index=False)
-        self.repo.add(csv.name)
+        #self.repo.add(csv.name)
 
-        self.repo.commit(msg, '-a', '--amend')
+        #self.repo.commit(msg, '-a', '--amend')
 
 # TODO Modèle de base de données pour journal
```

### Comparing `polygphys-6.0.5/src/polygphys/outils/reseau/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/reseau/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/reseau/courriel.py` & `polygphys-6.0.6/src/polygphys/outils/reseau/courriel.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/reseau/msforms.py` & `polygphys-6.0.6/src/polygphys/outils/reseau/msforms.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/outils/reseau/serveur/__init__.py` & `polygphys-6.0.6/src/polygphys/outils/reseau/serveur/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/serveur/__init__.py` & `polygphys-6.0.6/src/polygphys/serveur/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-# -*- coding: utf-8 -*-"""Serveur d'exécution de scripts programmés.Créé le Thu Sep  8 13:59:06 2022 par emilejetzer."""import timeimport loggingimport importlibimport jsonimport sysfrom pathlib import Pathfrom typing import Callablefrom functools import wraps, cached_property, partialfrom datetime import datetimefrom threading import Threadfrom http.server import ThreadingHTTPServer, SimpleHTTPRequestHandlerimport schedulefrom polygphys.outils.config import FichierConfigfrom polygphys.outils.journal import Journal, JournalBDfrom polygphys.outils.base_de_donnees import BaseTableauclass WebScriptConfig(FichierConfig):    def default(self):        return '''[script]    nom =     chemin =     fonction = [horaire]    intervalle =     unité = [journal]    adresse =     répertoire = [html]    modèle = '''class WebScript:    def __init__(self, config: WebScriptConfig):        if isinstance(config, (str, Path)):            self.config = WebScriptConfig(config)        else:            self.config = config        self.journal = Journal(logging.DEBUG,                               self.répertoire,                               JournalBD(self.adresse, self.nom))        self.logger.addHandler(self.journal)    @property    def nom(self) -> str:        return self.config.get('script', 'nom')    @property    def script(self) -> Path:        return Path(self.config.get('script', 'chemin'))    @property    def adresse(self) -> str:        return self.config.get('journal', 'adresse')    @property    def répertoire(self):        return self.config.get('journal', 'répertoire')    @property    def fonction(self) -> Callable:        return getattr(self.module, self.config.get('script', 'fonction'))    @property    def intervalle(self) -> int:        return self.config.getint('horaire', 'intervalle', fallback=1)    @property    def unité(self) -> str:        return self.config.get('horaire', 'unité', fallback='hours')    @property    def à(self):        return self.config.get('horaire', 'à', fallback=':00')    @property    def modèle(self) -> str:        chemin = self.config.get('html', 'modèle')        return open(chemin, encoding='utf-8').read()    def load(self):        self.logger.info('Exécution de load() pour %s', self.nom)        spec = importlib.util.spec_from_file_location(self.nom, self.script)        self.logger.debug('%r', spec)        module = importlib.util.module_from_spec(spec)        self.logger.debug('%r', module)        spec.loader.exec_module(module)        self.module = module        self.logger.debug('%r', self.module)    def reload(self):        self.logger.info('Exécution de reload() pour %s', self.nom)        importlib.reload(self.module)    def getLogger(self):        return logging.getLogger(self.nom)    @property    def logger(self):        return self.getLogger()    def __call__(self, *args, **kargs):        self.logger.info('Exécution de %s', self.nom)        fct = partial(self.fonction, *args, **kargs)        thread = Thread(target=fct)        thread.start()        thread.join()    def programmer(self):        self.logger.info('Programmation de %s', self.nom)        self.logger.debug('Aux %s %s', self.intervalle, self.unité)        self.jobid = getattr(schedule.every(self.intervalle),                             self.unité)\            .at(self.à)\            .do(self)        self.logger.debug('Avec jobid %s', self.jobid)    def annuler(self):        schedule.cancel_job(self.jobid)    def __str__(self):        self.logger.info('Affichage de %s', self.nom)        return self.modèle.format(script=self)    def json(self):        objet = {'script': {'nom': self.nom,                            'chemin': str(self.script),                            'fonction': self.fonction.__name__},                 'horaire': {'intervalle': self.intervalle,                             'unité': self.unité},                 'journal': {'adresse': self.adresse,                             'répertoire': self.répertoire},                 'html': {'modèle': self.modèle}}        return json.dumps(objet)class ScriptServeurConfig(FichierConfig):    def default(self):        return '''[scripts]    canari = config/canari.config[serveur]    adresse = localhost:8888    racine = racine/'''class ScriptServeur(ThreadingHTTPServer):    def __init__(self, config: ScriptServeurConfig):        if isinstance(config, (str, Path)):            self.config = ScriptServeurConfig(config)        else:            self.config = config        adresse, port = self.config\            .get('serveur', 'adresse')\            .split(':')        logging.info('Serveur pour %s:%s', adresse, port)        super().__init__((adresse, int(port)), ScriptHTTPRequestHandler)    @cached_property    def scripts(self):        return {script.script: script                for script in (WebScript(config)                               for nom, config in self.config.items('scripts'))}    @property    def racine(self):        return Path(self.config.get('serveur', 'racine'))    def update(self):        # On s'asssure de créer l'attribut s'il n'a pas été appelé encore        self.scripts        # On efface l'attribut de cache        del self.scripts        # On rappelle la propriété pour reconstruire le cache        self.scripts    def __call__(self):        try:            thread = Thread(target=self.serve_forever)            thread.start()            for script in self.scripts.values():                script.load()                script.programmer()            while True:                schedule.run_pending()                time.sleep(1)        except KeyboardInterrupt:            logging.exception('Fin du programme par l\'utilisateur.')        except Exception:            logging.exception(                'Une erreur s\'est produite pendant l\'exécution du serveur.')        finally:            self.shutdown()            schedule.clear()            thread.join(1)class ScriptHTTPRequestHandler(SimpleHTTPRequestHandler):    def __init__(self, request, client_adress, server):        self.serveur = server        super().__init__(request, client_adress, server)    @property    def chemin(self):        chemin = self.path.lstrip('/')        return Path(chemin)    def do_GET(self):        logging.debug('Accès à %s', self.chemin)        if self.chemin in self.serveur.scripts:            script = self.serveur.scripts[self.chemin]            try:                message = bytes(str(script), encoding='utf-8')            except Exception as erreur:                message = bytes(                    f'Erreur {erreur} dans la tentative d\'exécuter {self.path}.',                    encoding='utf-8')                logging.exception(message)                script.logger.exception(message)                self.send_response(502, message)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))                self.end_headers()                self.wfile.write(message)            else:                self.send_response(200)                self.send_header(                    'Content-type', 'text/html; charset=utf-8')                self.send_header('Content-length', len(message))            finally:                self.end_headers()                self.wfile.write(message)        elif self.serveur.racine in self.chemin.parents\                or self.serveur.racine == self.chemin:            super().do_GET()        else:            message = bytes('Ce répertoire n\'est pas accessible.',                            encoding='utf-8')            self.send_response(401, message)            self.send_header(                'Content-type', 'text/plain; charset=utf-8')            self.send_header('Content-length', len(message))            self.end_headers()            self.wfile.write(message)    def do_POST(self):        if self.chemin in self.serveur.scripts:            try:                message = self.serveur.scripts[self.chemin].json()            except Exception as erreur:                message = f'Erreur {erreur} dans la tentative d\'exécuter {self.path}.'                logging.exception(message)                self.send_response(502, message)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))                self.end_headers()                self.wfile.write(message)            else:                self.send_response(200)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))            finally:                self.end_headers()                self.wfile.write(message)        else:            message = 'Erreur 418: Je ne suis pas une cafetière, mais je ne peux quand même pas accomplir ce que vous me demandez.'            self.send_response(418, message)            self.send_header('Content-type', 'text/plain; charset=utf-8')            self.send_header('Content-length', len(message))            self.end_headers()            self.wfile.write(message)def main(config='serveur.cfg'):    logging.basicConfig(stream=sys.stdout,                        level=logging.DEBUG)    serveur = ScriptServeur(config)    serveur()if __name__ == '__main__':    main()
+# -*- coding: utf-8 -*-"""Serveur d'exécution de scripts programmés.Créé le Thu Sep  8 13:59:06 2022 par emilejetzer."""import timeimport loggingimport importlibimport jsonimport sysfrom pathlib import Pathfrom typing import Callablefrom functools import wraps, cached_property, partialfrom datetime import datetimefrom threading import Threadfrom http.server import ThreadingHTTPServer, SimpleHTTPRequestHandlerimport schedulefrom polygphys.outils.config import FichierConfigfrom polygphys.outils.journal import Journal, JournalBDfrom polygphys.outils.base_de_donnees import BaseTableauclass WebScriptConfig(FichierConfig):    def default(self):        return '''[script]    nom =     chemin =     fonction = [horaire]    intervalle =     unité = [journal]    adresse =     répertoire = [html]    modèle = '''class WebScript:    def __init__(self, config: WebScriptConfig):        if isinstance(config, (str, Path)):            self.config = WebScriptConfig(config)        else:            self.config = config        self.journal = Journal(logging.DEBUG,                               self.répertoire,                               JournalBD(self.adresse, self.nom))        self.logger.addHandler(self.journal)    @property    def nom(self) -> str:        return self.config.get('script', 'nom')    @property    def script(self) -> Path:        return Path(self.config.get('script', 'chemin'))    @property    def adresse(self) -> str:        return self.config.get('journal', 'adresse')    @property    def répertoire(self):        return self.config.get('journal', 'répertoire')    @property    def fonction(self) -> Callable:        return getattr(self.module, self.config.get('script', 'fonction'))    @property    def intervalle(self) -> int:        return self.config.getint('horaire', 'intervalle', fallback=1)    @property    def unité(self) -> str:        return self.config.get('horaire', 'unité', fallback='hours')    @property    def à(self):        return self.config.get('horaire', 'à', fallback=':00')    @property    def modèle(self) -> str:        chemin = self.config.get('html', 'modèle')        return open(chemin, encoding='utf-8').read()    def load(self):        self.logger.info('Exécution de load() pour %s', self.nom)        spec = importlib.util.spec_from_file_location(self.nom, self.script)        self.logger.debug('%r', spec)        module = importlib.util.module_from_spec(spec)        self.logger.debug('%r', module)        spec.loader.exec_module(module)        self.module = module        self.logger.debug('%r', self.module)    def reload(self):        self.logger.info('Exécution de reload() pour %s', self.nom)        importlib.reload(self.module)    def getLogger(self):        return logging.getLogger(self.nom)    @property    def logger(self):        return self.getLogger()    def __call__(self, *args, **kargs):        self.logger.info('Exécution de %s', self.nom)        fct = partial(self.fonction, *args, **kargs)        thread = Thread(target=fct)        thread.start()        thread.join()    def programmer(self):        self.logger.info('Programmation de %s', self.nom)        self.logger.debug('Aux %s %s', self.intervalle, self.unité)        self.jobid = getattr(schedule.every(self.intervalle),                             self.unité)\            .at(self.à)\            .do(self)        self.logger.debug('Avec jobid %s', self.jobid)    def annuler(self):        schedule.cancel_job(self.jobid)    def __str__(self):        self.logger.info('Affichage de %s', self.nom)        return self.modèle.format(script=self)    def json(self):        objet = {'script': {'nom': self.nom,                            'chemin': str(self.script),                            'fonction': self.fonction.__name__},                 'horaire': {'intervalle': self.intervalle,                             'unité': self.unité},                 'journal': {'adresse': self.adresse,                             'répertoire': self.répertoire},                 'html': {'modèle': self.modèle}}        return json.dumps(objet)class ScriptServeurConfig(FichierConfig):    def default(self):        return '''[scripts]    canari = config/canari.config[serveur]    adresse = localhost:8888    racine = racine/'''class ScriptServeur(ThreadingHTTPServer):    def __init__(self, config: ScriptServeurConfig):        if isinstance(config, (str, Path)):            self.config = ScriptServeurConfig(config)        else:            self.config = config        adresse, port = self.config\            .get('serveur', 'adresse')\            .split(':')        logging.info('Serveur pour %s:%s', adresse, port)        super().__init__((adresse, int(port)), ScriptHTTPRequestHandler)    @cached_property    def scripts(self):        return {script.script: script                for script in (WebScript(config)                               for nom, config in self.config.items('scripts'))}    @property    def racine(self):        return Path(self.config.get('serveur', 'racine'))    def update(self):        # On s'asssure de créer l'attribut s'il n'a pas été appelé encore        self.scripts        # On efface l'attribut de cache        del self.scripts        # On rappelle la propriété pour reconstruire le cache        self.scripts    def __call__(self):        try:            thread = Thread(target=self.serve_forever)            thread.start()            for script in self.scripts.values():                script.load()                script.programmer()            while True:                schedule.run_pending()                time.sleep(1)        except KeyboardInterrupt:            logging.exception('Fin du programme par l\'utilisateur.')        except Exception:            logging.exception(                'Une erreur s\'est produite pendant l\'exécution du serveur.')        finally:            self.shutdown()            schedule.clear()            thread.join(1)class ScriptHTTPRequestHandler(SimpleHTTPRequestHandler):    def __init__(self, request, client_adress, server):        self.serveur = server        super().__init__(request, client_adress, server)    @property    def chemin(self):        chemin = self.path.lstrip('/')        return Path(chemin)    def do_GET(self):        logging.debug('Accès à %s', self.chemin)        if self.chemin in self.serveur.scripts:            script = self.serveur.scripts[self.chemin]            try:                message = bytes(str(script), encoding='utf-8')            except Exception as erreur:                message = bytes(                    f'Erreur {erreur} dans la tentative d\'exécuter {self.path}.',                    encoding='utf-8')                logging.exception(message)                script.logger.exception(message)                self.send_response(502, message)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))                self.end_headers()                self.wfile.write(message)            else:                self.send_response(200)                self.send_header(                    'Content-type', 'text/html; charset=utf-8')                self.send_header('Content-length', len(message))            finally:                self.end_headers()                self.wfile.write(message)        elif self.serveur.racine in self.chemin.parents\                or self.serveur.racine == self.chemin:            super().do_GET()        else:            message = bytes('Ce répertoire n\'est pas accessible.',                            encoding='utf-8')            self.send_response(401, message)            self.send_header(                'Content-type', 'text/plain; charset=utf-8')            self.send_header('Content-length', len(message))            self.end_headers()            self.wfile.write(message)    def do_POST(self):        if self.chemin in self.serveur.scripts:            try:                message = self.serveur.scripts[self.chemin].json()            except Exception as erreur:                message = f'Erreur {erreur} dans la tentative d\'exécuter {self.path}.'                logging.exception(message)                self.send_response(502, message)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))                self.end_headers()                self.wfile.write(message)            else:                self.send_response(200)                self.send_header(                    'Content-type', 'text/plain; charset=utf-8')                self.send_header('Content-length', len(message))            finally:                self.end_headers()                self.wfile.write(message)        else:            message = 'Erreur 418: Je ne suis pas une cafetière, mais je ne peux quand même pas accomplir ce que vous me demandez.'            self.send_response(418, message)            self.send_header('Content-type', 'text/plain; charset=utf-8')            self.send_header('Content-length', len(message))            self.end_headers()            self.wfile.write(message)def main(config='serveur.cfg'):    # logging.basicConfig(stream=sys.stdout,    #                    level=logging.DEBUG)    serveur = ScriptServeur(config)    serveur()if __name__ == '__main__':    main()
```

### Comparing `polygphys-6.0.5/src/polygphys/serveur/__main__.py` & `polygphys-6.0.6/src/polygphys/serveur/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/serveur/nouveau_script.py` & `polygphys-6.0.6/src/polygphys/serveur/nouveau_script.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg` & `polygphys-6.0.6/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificats.py` & `polygphys-6.0.6/src/polygphys/sst/certificats_laser/nouveau_certificats.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/certificats_laser/vérifier.py` & `polygphys-6.0.6/src/polygphys/sst/certificats_laser/vérifier.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscription.cfg` & `polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/inscription.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py` & `polygphys-6.0.6/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg` & `polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py` & `polygphys-6.0.6/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py`

 * *Files identical despite different names*

### Comparing `polygphys-6.0.5/src/polygphys.egg-info/PKG-INFO` & `polygphys-6.0.6/src/polygphys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygphys
-Version: 6.0.5
+Version: 6.0.6
 Summary: Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 Author: Émile Jetzer
 Author-email: emile.jetzer@polymtl.ca
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Outils & programmes du département de génie physique de Polytechnique [![Python application](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml) [![CodeQL](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml) [![Upload Python Package](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml) [![Documentation Status](https://readthedocs.org/projects/polygphys/badge/?version=latest)](https://polygphys.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `polygphys-6.0.5/src/polygphys.egg-info/SOURCES.txt` & `polygphys-6.0.6/src/polygphys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

