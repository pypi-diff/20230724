# Comparing `tmp/bento_sts-0.1.2.tar.gz` & `tmp/bento_sts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_sts-0.1.2.tar", max compression
+gzip compressed data, was "bento_sts-0.1.3.tar", max compression
```

## Comparing `bento_sts-0.1.2.tar` & `bento_sts-0.1.3.tar`

### file list

```diff
@@ -1,84 +1,73 @@
--rw-r--r--   0        0        0     1079 2020-10-19 17:56:24.008960 bento_sts-0.1.2/LICENSE
--rw-r--r--   0        0        0      415 2023-07-08 22:03:48.092764 bento_sts-0.1.2/README.md
--rw-r--r--   0        0        0     1900 2023-07-24 01:57:05.759789 bento_sts-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       51 2023-07-09 19:32:46.361891 bento_sts-0.1.2/src/bento_sts/__init__.py
--rw-r--r--   0        0        0       84 2023-07-09 19:16:57.363182 bento_sts-0.1.2/src/bento_sts/api/__init__.py
--rw-r--r--   0        0        0     3941 2023-07-09 19:39:48.617466 bento_sts-0.1.2/src/bento_sts/api/routes.py
--rw-r--r--   0        0        0       28 2023-07-07 02:01:31.478631 bento_sts-0.1.2/src/bento_sts/cli.py
--rw-r--r--   0        0        0      855 2023-07-09 20:05:36.333841 bento_sts-0.1.2/src/bento_sts/config.py
--rw-r--r--   0        0        0        0 2022-02-25 02:56:46.496832 bento_sts-0.1.2/src/bento_sts/config_sts/__init__.py
--rw-r--r--   0        0        0     5687 2022-02-25 02:56:46.497407 bento_sts-0.1.2/src/bento_sts/config_sts/query_paths.yml
--rw-r--r--   0        0        0       82 2023-07-09 19:34:07.790210 bento_sts-0.1.2/src/bento_sts/errors/__init__.py
--rw-r--r--   0        0        0      390 2023-07-09 20:07:09.565949 bento_sts-0.1.2/src/bento_sts/errors/handlers.py
--rw-r--r--   0        0        0       87 2023-07-09 19:16:54.204908 bento_sts-0.1.2/src/bento_sts/main/__init__.py
--rw-r--r--   0        0        0      813 2023-07-07 02:01:31.476646 bento_sts-0.1.2/src/bento_sts/main/forms.py
--rw-r--r--   0        0        0    10631 2023-07-19 13:57:43.363802 bento_sts-0.1.2/src/bento_sts/main/routes.py
--rw-r--r--   0        0        0    11492 2023-07-19 01:58:03.297841 bento_sts-0.1.2/src/bento_sts/mdb.py
--rw-r--r--   0        0        0    13185 2023-07-19 14:00:20.242576 bento_sts-0.1.2/src/bento_sts/mdb_tags.py
--rw-r--r--   0        0        0    14611 2023-07-07 02:01:31.473005 bento_sts-0.1.2/src/bento_sts/mdb_update.py
--rw-r--r--   0        0        0      673 2023-07-07 02:01:31.472418 bento_sts-0.1.2/src/bento_sts/static/loading.gif
--rw-r--r--   0        0        0      282 2023-07-07 02:01:31.471927 bento_sts-0.1.2/src/bento_sts/static/sts.css
--rw-r--r--   0        0        0     1892 2023-07-09 20:15:02.823333 bento_sts-0.1.2/src/bento_sts/sts.py
--rw-r--r--   0        0        0     4633 2023-07-23 02:58:27.489244 bento_sts-0.1.2/src/bento_sts/templates/_intro.html
--rw-r--r--   0        0        0     1511 2023-07-24 01:17:01.447618 bento_sts-0.1.2/src/bento_sts/templates/about-mdb.html
--rw-r--r--   0        0        0     2160 2023-07-24 01:37:45.147781 bento_sts-0.1.2/src/bento_sts/templates/about-sts.html
--rw-r--r--   0        0        0     3920 2023-07-09 20:16:17.668929 bento_sts-0.1.2/src/bento_sts/templates/base.html
--rw-r--r--   0        0        0      188 2023-07-07 02:01:31.468445 bento_sts-0.1.2/src/bento_sts/templates/errors/400.html
--rw-r--r--   0        0        0      163 2023-07-07 02:01:31.467946 bento_sts-0.1.2/src/bento_sts/templates/errors/404.html
--rw-r--r--   0        0        0      234 2023-07-07 02:01:31.467192 bento_sts-0.1.2/src/bento_sts/templates/errors/500.html
--rw-r--r--   0        0        0      756 2023-07-09 20:12:27.105105 bento_sts-0.1.2/src/bento_sts/templates/explore.html
--rw-r--r--   0        0        0     2557 2023-07-24 01:24:40.494734 bento_sts-0.1.2/src/bento_sts/templates/index.html
--rw-r--r--   0        0        0     1172 2023-07-09 20:12:08.555392 bento_sts-0.1.2/src/bento_sts/templates/mdb-model.html
--rw-r--r--   0        0        0     1422 2023-07-09 20:11:41.928393 bento_sts-0.1.2/src/bento_sts/templates/mdb-node-list.html
--rw-r--r--   0        0        0     3524 2023-07-07 02:01:31.463259 bento_sts-0.1.2/src/bento_sts/templates/mdb-node.html
--rw-r--r--   0        0        0      602 2023-07-07 02:01:31.462192 bento_sts-0.1.2/src/bento_sts/templates/mdb-origin.html
--rw-r--r--   0        0        0     3532 2023-07-07 02:01:31.461399 bento_sts-0.1.2/src/bento_sts/templates/mdb-property.html
--rw-r--r--   0        0        0     1611 2023-07-07 02:01:31.460557 bento_sts-0.1.2/src/bento_sts/templates/mdb-tag.html
--rw-r--r--   0        0        0     1236 2023-07-21 02:43:23.999867 bento_sts-0.1.2/src/bento_sts/templates/mdb-term.html
--rw-r--r--   0        0        0     1789 2023-07-09 20:12:03.737714 bento_sts-0.1.2/src/bento_sts/templates/mdb-valueset.html
--rw-r--r--   0        0        0     4004 2023-07-09 20:10:58.458009 bento_sts-0.1.2/src/bento_sts/templates/mdb.html
--rw-r--r--   0        0        0     2589 2023-07-09 20:12:31.308854 bento_sts-0.1.2/src/bento_sts/templates/reports.html
--rw-r--r--   0        0        0     1872 2023-07-07 02:01:31.455624 bento_sts-0.1.2/src/bento_sts/templates/search.html
--rw-r--r--   0        0        0      495 2023-07-09 20:12:22.063962 bento_sts-0.1.2/src/bento_sts/templates/version-history-report.html
--rw-r--r--   0        0        0      500 2023-07-09 20:12:13.305029 bento_sts-0.1.2/src/bento_sts/templates/version-history.html
--rw-r--r--   0        0        0      204 2023-07-07 02:01:31.454103 bento_sts-0.1.2/src/bento_sts/util.py
--rw-r--r--   0        0        0    10852 2023-07-07 02:01:31.309361 bento_sts-0.1.2/swagger/nodejs-server-server-generated.zip
--rw-r--r--   0        0        0    18715 2023-07-18 16:42:04.940479 bento_sts-0.1.2/swagger/pysts-api.yaml
--rw-r--r--   0        0        0      885 2023-07-07 02:01:31.310135 bento_sts-0.1.2/swagger/python-flask-server/.dockerignore
--rw-r--r--   0        0        0      786 2023-07-07 02:01:31.310787 bento_sts-0.1.2/swagger/python-flask-server/.gitignore
--rw-r--r--   0        0        0        6 2023-07-07 02:01:31.312195 bento_sts-0.1.2/swagger/python-flask-server/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     1030 2023-07-07 02:01:31.311497 bento_sts-0.1.2/swagger/python-flask-server/.swagger-codegen-ignore
--rw-r--r--   0        0        0      246 2023-07-07 02:01:31.313276 bento_sts-0.1.2/swagger/python-flask-server/Dockerfile
--rw-r--r--   0        0        0     1115 2023-07-14 01:07:14.515754 bento_sts-0.1.2/swagger/python-flask-server/README.md
--rw-r--r--   0        0        0     1628 2023-07-07 02:01:31.314846 bento_sts-0.1.2/swagger/python-flask-server/git_push.sh
--rw-r--r--   0        0        0       65 2023-07-14 01:15:29.318240 bento_sts-0.1.2/swagger/python-flask-server/requirements.txt
--rw-r--r--   0        0        0     1253 2023-07-07 02:01:31.315777 bento_sts-0.1.2/swagger/python-flask-server/setup.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.315951 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/__init__.py
--rw-r--r--   0        0        0      353 2023-07-07 02:01:31.316657 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.316976 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      346 2023-07-07 02:01:31.318229 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/id_controller.py
--rw-r--r--   0        0        0     5910 2023-07-07 02:01:31.319216 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/model_controller.py
--rw-r--r--   0        0        0      426 2023-07-07 02:01:31.320206 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/models_controller.py
--rw-r--r--   0        0        0     1081 2023-07-07 02:01:31.321098 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tag_controller.py
--rw-r--r--   0        0        0      356 2023-07-07 02:01:31.321801 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tags_controller.py
--rw-r--r--   0        0        0      608 2023-07-07 02:01:31.322521 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/encoder.py
--rw-r--r--   0        0        0      393 2023-07-07 02:01:31.323225 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-07 02:01:31.323881 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     2291 2023-07-07 02:01:31.324334 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/entity.py
--rw-r--r--   0        0        0     3551 2023-07-07 02:01:31.324767 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model.py
--rw-r--r--   0        0        0     6112 2023-07-07 02:01:31.325214 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model_property.py
--rw-r--r--   0        0        0     2978 2023-07-07 02:01:31.325734 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/node.py
--rw-r--r--   0        0        0     2885 2023-07-07 02:01:31.326336 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/tag.py
--rw-r--r--   0        0        0     4604 2023-07-07 02:01:31.326925 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/term.py
--rw-r--r--   0        0        0    21512 2023-07-07 02:01:31.327834 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      415 2023-07-07 02:01:31.328553 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/__init__.py
--rw-r--r--   0        0        0      716 2023-07-07 02:01:31.329053 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_id_controller.py
--rw-r--r--   0        0        0     5798 2023-07-07 02:01:31.329691 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_model_controller.py
--rw-r--r--   0        0        0     1029 2023-07-07 02:01:31.330310 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_models_controller.py
--rw-r--r--   0        0        0     1688 2023-07-07 02:01:31.331002 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tag_controller.py
--rw-r--r--   0        0        0      952 2023-07-07 02:01:31.331519 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tags_controller.py
--rw-r--r--   0        0        0     3384 2023-07-07 02:01:31.332007 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/util.py
--rw-r--r--   0        0        0       90 2023-07-07 02:01:31.332560 bento_sts-0.1.2/swagger/python-flask-server/test-requirements.txt
--rw-r--r--   0        0        0      143 2023-07-07 02:01:31.333171 bento_sts-0.1.2/swagger/python-flask-server/tox.ini
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bento_sts-0.1.2/setup.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 bento_sts-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-24 02:02:23.897090 bento_sts-0.1.3/LICENSE
+-rw-r--r--   0        0        0      415 2023-07-24 02:02:23.898594 bento_sts-0.1.3/README.md
+-rw-r--r--   0        0        0     2198 2023-07-24 16:53:21.068473 bento_sts-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-24 02:02:23.902217 bento_sts-0.1.3/src/bento_sts/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-24 02:02:23.903158 bento_sts-0.1.3/src/bento_sts/api/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-24 02:02:23.903811 bento_sts-0.1.3/src/bento_sts/api/routes.py
+-rw-r--r--   0        0        0       28 2023-07-24 02:02:23.904006 bento_sts-0.1.3/src/bento_sts/cli.py
+-rw-r--r--   0        0        0      855 2023-07-24 02:02:23.904524 bento_sts-0.1.3/src/bento_sts/config.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:02:23.904615 bento_sts-0.1.3/src/bento_sts/config_sts/__init__.py
+-rw-r--r--   0        0        0     5687 2023-07-24 02:02:23.904928 bento_sts-0.1.3/src/bento_sts/config_sts/query_paths.yml
+-rw-r--r--   0        0        0       82 2023-07-24 02:02:23.905622 bento_sts-0.1.3/src/bento_sts/errors/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-24 02:02:23.906388 bento_sts-0.1.3/src/bento_sts/errors/handlers.py
+-rw-r--r--   0        0        0       87 2023-07-24 02:02:23.907031 bento_sts-0.1.3/src/bento_sts/main/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-24 02:02:23.907610 bento_sts-0.1.3/src/bento_sts/main/forms.py
+-rw-r--r--   0        0        0    10631 2023-07-24 02:02:23.908475 bento_sts-0.1.3/src/bento_sts/main/routes.py
+-rw-r--r--   0        0        0    11492 2023-07-24 02:02:23.909044 bento_sts-0.1.3/src/bento_sts/mdb.py
+-rw-r--r--   0        0        0    13185 2023-07-24 02:02:23.909553 bento_sts-0.1.3/src/bento_sts/mdb_tags.py
+-rw-r--r--   0        0        0    14611 2023-07-24 02:02:23.909904 bento_sts-0.1.3/src/bento_sts/mdb_update.py
+-rw-r--r--   0        0        0      673 2023-07-24 02:02:23.910083 bento_sts-0.1.3/src/bento_sts/static/loading.gif
+-rw-r--r--   0        0        0      282 2023-07-24 02:02:23.910361 bento_sts-0.1.3/src/bento_sts/static/sts.css
+-rw-r--r--   0        0        0     1892 2023-07-24 02:02:23.910857 bento_sts-0.1.3/src/bento_sts/sts.py
+-rw-r--r--   0        0        0     4633 2023-07-23 02:58:27.489244 bento_sts-0.1.3/src/bento_sts/templates/_intro.html
+-rw-r--r--   0        0        0     1511 2023-07-24 02:02:23.911581 bento_sts-0.1.3/src/bento_sts/templates/about-mdb.html
+-rw-r--r--   0        0        0     2160 2023-07-24 02:02:23.912163 bento_sts-0.1.3/src/bento_sts/templates/about-sts.html
+-rw-r--r--   0        0        0     3920 2023-07-24 02:02:23.912941 bento_sts-0.1.3/src/bento_sts/templates/base.html
+-rw-r--r--   0        0        0      188 2023-07-24 02:02:23.913233 bento_sts-0.1.3/src/bento_sts/templates/errors/400.html
+-rw-r--r--   0        0        0      163 2023-07-24 02:02:23.913389 bento_sts-0.1.3/src/bento_sts/templates/errors/404.html
+-rw-r--r--   0        0        0      234 2023-07-24 02:02:23.913790 bento_sts-0.1.3/src/bento_sts/templates/errors/500.html
+-rw-r--r--   0        0        0      756 2023-07-24 02:02:23.914414 bento_sts-0.1.3/src/bento_sts/templates/explore.html
+-rw-r--r--   0        0        0     2557 2023-07-24 02:02:23.914898 bento_sts-0.1.3/src/bento_sts/templates/index.html
+-rw-r--r--   0        0        0     1172 2023-07-24 02:02:23.915329 bento_sts-0.1.3/src/bento_sts/templates/mdb-model.html
+-rw-r--r--   0        0        0     1422 2023-07-24 02:02:23.915670 bento_sts-0.1.3/src/bento_sts/templates/mdb-node-list.html
+-rw-r--r--   0        0        0     3524 2023-07-24 02:02:23.915923 bento_sts-0.1.3/src/bento_sts/templates/mdb-node.html
+-rw-r--r--   0        0        0      602 2023-07-24 02:02:23.916458 bento_sts-0.1.3/src/bento_sts/templates/mdb-origin.html
+-rw-r--r--   0        0        0     3532 2023-07-24 02:02:23.917114 bento_sts-0.1.3/src/bento_sts/templates/mdb-property.html
+-rw-r--r--   0        0        0     1611 2023-07-24 02:02:23.917814 bento_sts-0.1.3/src/bento_sts/templates/mdb-tag.html
+-rw-r--r--   0        0        0     1236 2023-07-24 02:02:23.918564 bento_sts-0.1.3/src/bento_sts/templates/mdb-term.html
+-rw-r--r--   0        0        0     1789 2023-07-24 02:02:23.919157 bento_sts-0.1.3/src/bento_sts/templates/mdb-valueset.html
+-rw-r--r--   0        0        0     4004 2023-07-24 02:02:23.919622 bento_sts-0.1.3/src/bento_sts/templates/mdb.html
+-rw-r--r--   0        0        0     2589 2023-07-24 02:02:23.920402 bento_sts-0.1.3/src/bento_sts/templates/reports.html
+-rw-r--r--   0        0        0     1872 2023-07-24 02:02:23.920874 bento_sts-0.1.3/src/bento_sts/templates/search.html
+-rw-r--r--   0        0        0      495 2023-07-24 02:02:23.921699 bento_sts-0.1.3/src/bento_sts/templates/version-history-report.html
+-rw-r--r--   0        0        0      500 2023-07-24 02:02:23.922369 bento_sts-0.1.3/src/bento_sts/templates/version-history.html
+-rw-r--r--   0        0        0      204 2023-07-24 02:02:23.922654 bento_sts-0.1.3/src/bento_sts/util.py
+-rw-r--r--   0        0        0        6 2023-07-24 02:02:23.930765 bento_sts-0.1.3/src/swagger_server/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     1115 2023-07-24 02:02:23.932920 bento_sts-0.1.3/src/swagger_server/README.md
+-rw-r--r--   0        0        0      418 2023-07-24 17:26:10.359254 bento_sts-0.1.3/src/swagger_server/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-24 02:02:23.936898 bento_sts-0.1.3/src/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:02:23.937063 bento_sts-0.1.3/src/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-24 13:59:01.025711 bento_sts-0.1.3/src/swagger_server/controllers/id_controller.py
+-rw-r--r--   0        0        0     5910 2023-07-24 13:58:17.127265 bento_sts-0.1.3/src/swagger_server/controllers/model_controller.py
+-rw-r--r--   0        0        0      426 2023-07-24 13:58:25.899767 bento_sts-0.1.3/src/swagger_server/controllers/models_controller.py
+-rw-r--r--   0        0        0     1081 2023-07-24 13:59:26.157288 bento_sts-0.1.3/src/swagger_server/controllers/tag_controller.py
+-rw-r--r--   0        0        0      356 2023-07-24 13:58:55.182069 bento_sts-0.1.3/src/swagger_server/controllers/tags_controller.py
+-rw-r--r--   0        0        0      608 2023-07-24 02:02:23.941987 bento_sts-0.1.3/src/swagger_server/encoder.py
+-rw-r--r--   0        0        0      393 2023-07-24 13:56:36.590118 bento_sts-0.1.3/src/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-24 13:56:57.706900 bento_sts-0.1.3/src/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     2291 2023-07-24 13:57:42.382264 bento_sts-0.1.3/src/swagger_server/models/entity.py
+-rw-r--r--   0        0        0     3551 2023-07-24 13:56:45.251417 bento_sts-0.1.3/src/swagger_server/models/model.py
+-rw-r--r--   0        0        0     6112 2023-07-24 13:57:32.107167 bento_sts-0.1.3/src/swagger_server/models/model_property.py
+-rw-r--r--   0        0        0     2978 2023-07-24 13:57:51.518200 bento_sts-0.1.3/src/swagger_server/models/node.py
+-rw-r--r--   0        0        0     2885 2023-07-24 13:58:03.739932 bento_sts-0.1.3/src/swagger_server/models/tag.py
+-rw-r--r--   0        0        0     4604 2023-07-24 14:00:16.782905 bento_sts-0.1.3/src/swagger_server/models/term.py
+-rw-r--r--   0        0        0    21512 2023-07-24 02:02:23.947259 bento_sts-0.1.3/src/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      415 2023-07-24 02:02:23.947845 bento_sts-0.1.3/src/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0      710 2023-07-24 13:40:40.786562 bento_sts-0.1.3/src/swagger_server/test/test_id_controller.py
+-rw-r--r--   0        0        0     5798 2023-07-24 13:56:26.490845 bento_sts-0.1.3/src/swagger_server/test/test_model_controller.py
+-rw-r--r--   0        0        0     1029 2023-07-24 13:56:01.730065 bento_sts-0.1.3/src/swagger_server/test/test_models_controller.py
+-rw-r--r--   0        0        0     1688 2023-07-24 13:56:08.596499 bento_sts-0.1.3/src/swagger_server/test/test_tag_controller.py
+-rw-r--r--   0        0        0      952 2023-07-24 13:56:17.706375 bento_sts-0.1.3/src/swagger_server/test/test_tags_controller.py
+-rw-r--r--   0        0        0     3384 2023-07-24 02:02:23.950637 bento_sts-0.1.3/src/swagger_server/util.py
+-rw-r--r--   0        0        0     2225 1970-01-01 00:00:00.000000 bento_sts-0.1.3/setup.py
+-rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 bento_sts-0.1.3/PKG-INFO
```

### Comparing `bento_sts-0.1.2/LICENSE` & `bento_sts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/pyproject.toml` & `bento_sts-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-sts"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 { name="Mark Benson", email="mark.benson@nih.gov"},
 { name="Mark A. Jensen", email="mark.jensen@nih.gov"},
 ]
 maintainer = "Mark A. Jensen"
 maintainer_email = "mark.jensen@nih.gov"
 description = "Bento Simple Terminology Server"
@@ -15,23 +15,27 @@
 ]
 [project.urls]
 "Homepage" = "https://github.com/CBIIT/bento-sts"
 "Bug Tracker" = "https:/github.com/CBIIT/bento-sts/issues"
 
 [tool.poetry]
 name = "bento-sts"
-version = "0.1.2"
+version = "0.1.3"
 description = "Bento Simple Terminology Server"
 authors = [
 	"Mark Benson <mark.benson@nih.gov>",
 	"Mark A. Jensen <mark.jensen@nih.gov>",
 ]
 license = "Apache 2.0"
 readme = "README.md"
-include = ["swagger"]
+packages = [
+	 { include = "bento_sts", from = "src" },
+	 { include = "swagger_server", from = "src" },
+	 ]
+include = ["swagger_server"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 bento-meta = ">=0.0.32"
 importlib_resources = ">=5.4.0"
 Flask-WTF =  ">=0.14.3"
 Bootstrap-Flask =  ">=1.5.2"
@@ -52,14 +56,20 @@
 requests = ">=2.20.0"
 six = ">=1.15.0"
 urllib3 = ">=1.26.5"
 visitor = ">=0.1.3"
 Werkzeug = ">=1.0.1"
 WTForms = ">=2.1"
 WTForms-Components = ">=0.10.5"
+connexion = {version = ">= 2.6.0", optional = false}
+swagger-ui-bundle = {version = ">=0.0.9", optional = false}
+
+
+#[tool.poetry.extras]
+#swagger = ["connexion", "swagger-ui-bundle"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
```

### Comparing `bento_sts-0.1.2/src/bento_sts/api/routes.py` & `bento_sts-0.1.3/src/bento_sts/api/routes.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/config.py` & `bento_sts-0.1.3/src/bento_sts/config.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/config_sts/query_paths.yml` & `bento_sts-0.1.3/src/bento_sts/config_sts/query_paths.yml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/main/forms.py` & `bento_sts-0.1.3/src/bento_sts/main/forms.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/main/routes.py` & `bento_sts-0.1.3/src/bento_sts/main/routes.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/mdb.py` & `bento_sts-0.1.3/src/bento_sts/mdb.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/mdb_tags.py` & `bento_sts-0.1.3/src/bento_sts/mdb_tags.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/mdb_update.py` & `bento_sts-0.1.3/src/bento_sts/mdb_update.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/static/loading.gif` & `bento_sts-0.1.3/src/bento_sts/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/sts.py` & `bento_sts-0.1.3/src/bento_sts/sts.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/_intro.html` & `bento_sts-0.1.3/src/bento_sts/templates/_intro.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/about-mdb.html` & `bento_sts-0.1.3/src/bento_sts/templates/about-mdb.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/about-sts.html` & `bento_sts-0.1.3/src/bento_sts/templates/about-sts.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/base.html` & `bento_sts-0.1.3/src/bento_sts/templates/base.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/explore.html` & `bento_sts-0.1.3/src/bento_sts/templates/explore.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/index.html` & `bento_sts-0.1.3/src/bento_sts/templates/index.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-model.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-model.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-node-list.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-node-list.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-node.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-node.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-origin.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-origin.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-property.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-property.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-tag.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-tag.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-term.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-term.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb-valueset.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb-valueset.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/mdb.html` & `bento_sts-0.1.3/src/bento_sts/templates/mdb.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/reports.html` & `bento_sts-0.1.3/src/bento_sts/templates/reports.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/src/bento_sts/templates/search.html` & `bento_sts-0.1.3/src/bento_sts/templates/search.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/README.md` & `bento_sts-0.1.3/src/swagger_server/README.md`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/model_controller.py` & `bento_sts-0.1.3/src/swagger_server/controllers/model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tag_controller.py` & `bento_sts-0.1.3/src/swagger_server/controllers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/encoder.py` & `bento_sts-0.1.3/src/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/base_model_.py` & `bento_sts-0.1.3/src/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/entity.py` & `bento_sts-0.1.3/src/swagger_server/models/entity.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model.py` & `bento_sts-0.1.3/src/swagger_server/models/model.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model_property.py` & `bento_sts-0.1.3/src/swagger_server/models/model_property.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/node.py` & `bento_sts-0.1.3/src/swagger_server/models/node.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/tag.py` & `bento_sts-0.1.3/src/swagger_server/models/tag.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/term.py` & `bento_sts-0.1.3/src/swagger_server/models/term.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/swagger/swagger.yaml` & `bento_sts-0.1.3/src/swagger_server/swagger/swagger.yaml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_model_controller.py` & `bento_sts-0.1.3/src/swagger_server/test/test_model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_models_controller.py` & `bento_sts-0.1.3/src/swagger_server/test/test_models_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tag_controller.py` & `bento_sts-0.1.3/src/swagger_server/test/test_tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tags_controller.py` & `bento_sts-0.1.3/src/swagger_server/test/test_tags_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/util.py` & `bento_sts-0.1.3/src/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.2/setup.py` & `bento_sts-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
-{'': 'src'}
+{'': 'src',
+ 'swagger_server': 'src/swagger_server',
+ 'swagger_server.controllers': 'src/swagger_server/controllers',
+ 'swagger_server.models': 'src/swagger_server/models',
+ 'swagger_server.test': 'src/swagger_server/test'}
 
 packages = \
 ['bento_sts',
  'bento_sts.api',
  'bento_sts.config_sts',
  'bento_sts.errors',
- 'bento_sts.main']
+ 'bento_sts.main',
+ 'swagger_server',
+ 'swagger_server.controllers',
+ 'swagger_server.models',
+ 'swagger_server.test']
 
 package_data = \
-{'': ['*'], 'bento_sts': ['static/*', 'templates/*', 'templates/errors/*']}
+{'': ['*'],
+ 'bento_sts': ['static/*', 'templates/*', 'templates/errors/*'],
+ 'swagger_server': ['.swagger-codegen/*', 'swagger/*']}
 
 install_requires = \
 ['Bootstrap-Flask>=1.5.2',
  'Flask-Moment>=0.5.2',
  'Flask-Paginate>=2021.10.29',
  'Flask-WTF>=0.14.3',
  'Jinja2>=2.11.3',
  'MarkupSafe>=1.1.1',
  'PyYAML>=5.4.1',
  'WTForms-Components>=0.10.5',
  'WTForms>=2.1',
  'Werkzeug>=1.0.1',
  'bento-meta>=0.0.32',
+ 'connexion>=2.6.0',
  'guess-language-spirit>=0.5.3',
  'gunicorn>=20.1.0',
  'idna>=2.6',
  'importlib_resources>=5.4.0',
  'itsdangerous>=0.24',
  'neo4j>=4.1',
  'python-dateutil>=2.6.1',
  'python-dotenv>=0.15.0',
  'python-editor>=1.0.3',
  'pytz>=2017.2',
  'requests>=2.20.0',
  'six>=1.15.0',
+ 'swagger-ui-bundle>=0.0.9',
  'urllib3>=1.26.5',
  'visitor>=0.1.3']
 
 setup_kwargs = {
     'name': 'bento-sts',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Bento Simple Terminology Server',
     'long_description': '# Welcome to bento-sts\n\nThis is a flask-based implementation of the Simple Terminology Service (STS) for the Bento Metadatabase (MDB).\n\n## Install\n\n\t$ git clone https://github.com/CBIIT/bento-sts.git\n\t$ cd pysts\n\t$ virtualenv sts-venv\n\t$ source sts-venv/bin/activate\n\t$ pip install -r requirements.txt\n\t$ flask run\n\n## Dependencies\n\n`bento-sts` requires a Neo4j-based [MDB](https://github.com/CBIIT/bento-meta).\n\n\n\n',
     'author': 'Mark Benson',
     'author_email': 'mark.benson@nih.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bento_sts-0.1.2/PKG-INFO` & `bento_sts-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-sts
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bento Simple Terminology Server
 License: Apache 2.0
 Author: Mark Benson
 Author-email: mark.benson@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -19,26 +19,28 @@
 Requires-Dist: Jinja2 (>=2.11.3)
 Requires-Dist: MarkupSafe (>=1.1.1)
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: WTForms (>=2.1)
 Requires-Dist: WTForms-Components (>=0.10.5)
 Requires-Dist: Werkzeug (>=1.0.1)
 Requires-Dist: bento-meta (>=0.0.32)
+Requires-Dist: connexion (>=2.6.0)
 Requires-Dist: guess-language-spirit (>=0.5.3)
 Requires-Dist: gunicorn (>=20.1.0)
 Requires-Dist: idna (>=2.6)
 Requires-Dist: importlib_resources (>=5.4.0)
 Requires-Dist: itsdangerous (>=0.24)
 Requires-Dist: neo4j (>=4.1)
 Requires-Dist: python-dateutil (>=2.6.1)
 Requires-Dist: python-dotenv (>=0.15.0)
 Requires-Dist: python-editor (>=1.0.3)
 Requires-Dist: pytz (>=2017.2)
 Requires-Dist: requests (>=2.20.0)
 Requires-Dist: six (>=1.15.0)
+Requires-Dist: swagger-ui-bundle (>=0.0.9)
 Requires-Dist: urllib3 (>=1.26.5)
 Requires-Dist: visitor (>=0.1.3)
 Description-Content-Type: text/markdown
 
 # Welcome to bento-sts
 
 This is a flask-based implementation of the Simple Terminology Service (STS) for the Bento Metadatabase (MDB).
```

