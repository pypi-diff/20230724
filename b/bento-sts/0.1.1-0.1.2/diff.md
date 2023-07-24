# Comparing `tmp/bento_sts-0.1.1.tar.gz` & `tmp/bento_sts-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_sts-0.1.1.tar", max compression
+gzip compressed data, was "bento_sts-0.1.2.tar", max compression
```

## Comparing `bento_sts-0.1.1.tar` & `bento_sts-0.1.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1079 2020-10-19 17:56:24.008960 bento_sts-0.1.1/LICENSE
--rw-r--r--   0        0        0      415 2023-07-08 22:03:48.092764 bento_sts-0.1.1/README.md
--rw-r--r--   0        0        0     1908 2023-07-19 14:03:32.194118 bento_sts-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       51 2023-07-09 19:32:46.361891 bento_sts-0.1.1/src/bento_sts/__init__.py
--rw-r--r--   0        0        0       84 2023-07-09 19:16:57.363182 bento_sts-0.1.1/src/bento_sts/api/__init__.py
--rw-r--r--   0        0        0     3941 2023-07-09 19:39:48.617466 bento_sts-0.1.1/src/bento_sts/api/routes.py
--rw-r--r--   0        0        0       28 2023-07-07 02:01:31.478631 bento_sts-0.1.1/src/bento_sts/cli.py
--rw-r--r--   0        0        0      855 2023-07-09 20:05:36.333841 bento_sts-0.1.1/src/bento_sts/config.py
--rw-r--r--   0        0        0        0 2022-02-25 02:56:46.496832 bento_sts-0.1.1/src/bento_sts/config_sts/__init__.py
--rw-r--r--   0        0        0     5687 2022-02-25 02:56:46.497407 bento_sts-0.1.1/src/bento_sts/config_sts/query_paths.yml
--rw-r--r--   0        0        0       82 2023-07-09 19:34:07.790210 bento_sts-0.1.1/src/bento_sts/errors/__init__.py
--rw-r--r--   0        0        0      390 2023-07-09 20:07:09.565949 bento_sts-0.1.1/src/bento_sts/errors/handlers.py
--rw-r--r--   0        0        0       87 2023-07-09 19:16:54.204908 bento_sts-0.1.1/src/bento_sts/main/__init__.py
--rw-r--r--   0        0        0      813 2023-07-07 02:01:31.476646 bento_sts-0.1.1/src/bento_sts/main/forms.py
--rw-r--r--   0        0        0    10631 2023-07-19 13:57:43.363802 bento_sts-0.1.1/src/bento_sts/main/routes.py
--rw-r--r--   0        0        0    11492 2023-07-19 01:58:03.297841 bento_sts-0.1.1/src/bento_sts/mdb.py
--rw-r--r--   0        0        0    13185 2023-07-19 14:00:20.242576 bento_sts-0.1.1/src/bento_sts/mdb_tags.py
--rw-r--r--   0        0        0    14611 2023-07-07 02:01:31.473005 bento_sts-0.1.1/src/bento_sts/mdb_update.py
--rw-r--r--   0        0        0      673 2023-07-07 02:01:31.472418 bento_sts-0.1.1/src/bento_sts/static/loading.gif
--rw-r--r--   0        0        0      282 2023-07-07 02:01:31.471927 bento_sts-0.1.1/src/bento_sts/static/sts.css
--rw-r--r--   0        0        0     1892 2023-07-09 20:15:02.823333 bento_sts-0.1.1/src/bento_sts/sts.py
--rw-r--r--   0        0        0     4422 2023-07-07 02:01:31.470911 bento_sts-0.1.1/src/bento_sts/templates/_intro.html
--rw-r--r--   0        0        0      175 2023-07-07 02:01:31.470494 bento_sts-0.1.1/src/bento_sts/templates/about-mdb.html
--rw-r--r--   0        0        0     1083 2023-07-09 20:12:17.632256 bento_sts-0.1.1/src/bento_sts/templates/about-sts.html
--rw-r--r--   0        0        0     3920 2023-07-09 20:16:17.668929 bento_sts-0.1.1/src/bento_sts/templates/base.html
--rw-r--r--   0        0        0      188 2023-07-07 02:01:31.468445 bento_sts-0.1.1/src/bento_sts/templates/errors/400.html
--rw-r--r--   0        0        0      163 2023-07-07 02:01:31.467946 bento_sts-0.1.1/src/bento_sts/templates/errors/404.html
--rw-r--r--   0        0        0      234 2023-07-07 02:01:31.467192 bento_sts-0.1.1/src/bento_sts/templates/errors/500.html
--rw-r--r--   0        0        0      756 2023-07-09 20:12:27.105105 bento_sts-0.1.1/src/bento_sts/templates/explore.html
--rw-r--r--   0        0        0     2132 2023-07-09 20:11:04.493347 bento_sts-0.1.1/src/bento_sts/templates/index.html
--rw-r--r--   0        0        0     1172 2023-07-09 20:12:08.555392 bento_sts-0.1.1/src/bento_sts/templates/mdb-model.html
--rw-r--r--   0        0        0     1422 2023-07-09 20:11:41.928393 bento_sts-0.1.1/src/bento_sts/templates/mdb-node-list.html
--rw-r--r--   0        0        0     3524 2023-07-07 02:01:31.463259 bento_sts-0.1.1/src/bento_sts/templates/mdb-node.html
--rw-r--r--   0        0        0      602 2023-07-07 02:01:31.462192 bento_sts-0.1.1/src/bento_sts/templates/mdb-origin.html
--rw-r--r--   0        0        0     3532 2023-07-07 02:01:31.461399 bento_sts-0.1.1/src/bento_sts/templates/mdb-property.html
--rw-r--r--   0        0        0     1611 2023-07-07 02:01:31.460557 bento_sts-0.1.1/src/bento_sts/templates/mdb-tag.html
--rw-r--r--   0        0        0     1745 2023-07-07 02:01:31.459307 bento_sts-0.1.1/src/bento_sts/templates/mdb-term.html
--rw-r--r--   0        0        0     1789 2023-07-09 20:12:03.737714 bento_sts-0.1.1/src/bento_sts/templates/mdb-valueset.html
--rw-r--r--   0        0        0     4004 2023-07-09 20:10:58.458009 bento_sts-0.1.1/src/bento_sts/templates/mdb.html
--rw-r--r--   0        0        0     2589 2023-07-09 20:12:31.308854 bento_sts-0.1.1/src/bento_sts/templates/reports.html
--rw-r--r--   0        0        0     1872 2023-07-07 02:01:31.455624 bento_sts-0.1.1/src/bento_sts/templates/search.html
--rw-r--r--   0        0        0      495 2023-07-09 20:12:22.063962 bento_sts-0.1.1/src/bento_sts/templates/version-history-report.html
--rw-r--r--   0        0        0      500 2023-07-09 20:12:13.305029 bento_sts-0.1.1/src/bento_sts/templates/version-history.html
--rw-r--r--   0        0        0      204 2023-07-07 02:01:31.454103 bento_sts-0.1.1/src/bento_sts/util.py
--rw-r--r--   0        0        0    10852 2023-07-07 02:01:31.309361 bento_sts-0.1.1/swagger/nodejs-server-server-generated.zip
--rw-r--r--   0        0        0    18715 2023-07-18 16:42:04.940479 bento_sts-0.1.1/swagger/pysts-api.yaml
--rw-r--r--   0        0        0      885 2023-07-07 02:01:31.310135 bento_sts-0.1.1/swagger/python-flask-server/.dockerignore
--rw-r--r--   0        0        0      786 2023-07-07 02:01:31.310787 bento_sts-0.1.1/swagger/python-flask-server/.gitignore
--rw-r--r--   0        0        0        6 2023-07-07 02:01:31.312195 bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     1030 2023-07-07 02:01:31.311497 bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen-ignore
--rw-r--r--   0        0        0      246 2023-07-07 02:01:31.313276 bento_sts-0.1.1/swagger/python-flask-server/Dockerfile
--rw-r--r--   0        0        0     1115 2023-07-14 01:07:14.515754 bento_sts-0.1.1/swagger/python-flask-server/README.md
--rw-r--r--   0        0        0     1628 2023-07-07 02:01:31.314846 bento_sts-0.1.1/swagger/python-flask-server/git_push.sh
--rw-r--r--   0        0        0       65 2023-07-14 01:15:29.318240 bento_sts-0.1.1/swagger/python-flask-server/requirements.txt
--rw-r--r--   0        0        0     1253 2023-07-07 02:01:31.315777 bento_sts-0.1.1/swagger/python-flask-server/setup.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.315951 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/__init__.py
--rw-r--r--   0        0        0      353 2023-07-07 02:01:31.316657 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-07-07 02:01:31.316976 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      346 2023-07-07 02:01:31.318229 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/id_controller.py
--rw-r--r--   0        0        0     5910 2023-07-07 02:01:31.319216 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/model_controller.py
--rw-r--r--   0        0        0      426 2023-07-07 02:01:31.320206 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/models_controller.py
--rw-r--r--   0        0        0     1081 2023-07-07 02:01:31.321098 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tag_controller.py
--rw-r--r--   0        0        0      356 2023-07-07 02:01:31.321801 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tags_controller.py
--rw-r--r--   0        0        0      608 2023-07-07 02:01:31.322521 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/encoder.py
--rw-r--r--   0        0        0      393 2023-07-07 02:01:31.323225 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-07 02:01:31.323881 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     2291 2023-07-07 02:01:31.324334 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/entity.py
--rw-r--r--   0        0        0     3551 2023-07-07 02:01:31.324767 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model.py
--rw-r--r--   0        0        0     6112 2023-07-07 02:01:31.325214 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model_property.py
--rw-r--r--   0        0        0     2978 2023-07-07 02:01:31.325734 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/node.py
--rw-r--r--   0        0        0     2885 2023-07-07 02:01:31.326336 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/tag.py
--rw-r--r--   0        0        0     4604 2023-07-07 02:01:31.326925 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/term.py
--rw-r--r--   0        0        0    21512 2023-07-07 02:01:31.327834 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      415 2023-07-07 02:01:31.328553 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/__init__.py
--rw-r--r--   0        0        0      716 2023-07-07 02:01:31.329053 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_id_controller.py
--rw-r--r--   0        0        0     5798 2023-07-07 02:01:31.329691 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_model_controller.py
--rw-r--r--   0        0        0     1029 2023-07-07 02:01:31.330310 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_models_controller.py
--rw-r--r--   0        0        0     1688 2023-07-07 02:01:31.331002 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tag_controller.py
--rw-r--r--   0        0        0      952 2023-07-07 02:01:31.331519 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tags_controller.py
--rw-r--r--   0        0        0     3384 2023-07-07 02:01:31.332007 bento_sts-0.1.1/swagger/python-flask-server/swagger_server/util.py
--rw-r--r--   0        0        0       90 2023-07-07 02:01:31.332560 bento_sts-0.1.1/swagger/python-flask-server/test-requirements.txt
--rw-r--r--   0        0        0      143 2023-07-07 02:01:31.333171 bento_sts-0.1.1/swagger/python-flask-server/tox.ini
--rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bento_sts-0.1.1/setup.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 bento_sts-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2020-10-19 17:56:24.008960 bento_sts-0.1.2/LICENSE
+-rw-r--r--   0        0        0      415 2023-07-08 22:03:48.092764 bento_sts-0.1.2/README.md
+-rw-r--r--   0        0        0     1900 2023-07-24 01:57:05.759789 bento_sts-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-09 19:32:46.361891 bento_sts-0.1.2/src/bento_sts/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-09 19:16:57.363182 bento_sts-0.1.2/src/bento_sts/api/__init__.py
+-rw-r--r--   0        0        0     3941 2023-07-09 19:39:48.617466 bento_sts-0.1.2/src/bento_sts/api/routes.py
+-rw-r--r--   0        0        0       28 2023-07-07 02:01:31.478631 bento_sts-0.1.2/src/bento_sts/cli.py
+-rw-r--r--   0        0        0      855 2023-07-09 20:05:36.333841 bento_sts-0.1.2/src/bento_sts/config.py
+-rw-r--r--   0        0        0        0 2022-02-25 02:56:46.496832 bento_sts-0.1.2/src/bento_sts/config_sts/__init__.py
+-rw-r--r--   0        0        0     5687 2022-02-25 02:56:46.497407 bento_sts-0.1.2/src/bento_sts/config_sts/query_paths.yml
+-rw-r--r--   0        0        0       82 2023-07-09 19:34:07.790210 bento_sts-0.1.2/src/bento_sts/errors/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-09 20:07:09.565949 bento_sts-0.1.2/src/bento_sts/errors/handlers.py
+-rw-r--r--   0        0        0       87 2023-07-09 19:16:54.204908 bento_sts-0.1.2/src/bento_sts/main/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-07 02:01:31.476646 bento_sts-0.1.2/src/bento_sts/main/forms.py
+-rw-r--r--   0        0        0    10631 2023-07-19 13:57:43.363802 bento_sts-0.1.2/src/bento_sts/main/routes.py
+-rw-r--r--   0        0        0    11492 2023-07-19 01:58:03.297841 bento_sts-0.1.2/src/bento_sts/mdb.py
+-rw-r--r--   0        0        0    13185 2023-07-19 14:00:20.242576 bento_sts-0.1.2/src/bento_sts/mdb_tags.py
+-rw-r--r--   0        0        0    14611 2023-07-07 02:01:31.473005 bento_sts-0.1.2/src/bento_sts/mdb_update.py
+-rw-r--r--   0        0        0      673 2023-07-07 02:01:31.472418 bento_sts-0.1.2/src/bento_sts/static/loading.gif
+-rw-r--r--   0        0        0      282 2023-07-07 02:01:31.471927 bento_sts-0.1.2/src/bento_sts/static/sts.css
+-rw-r--r--   0        0        0     1892 2023-07-09 20:15:02.823333 bento_sts-0.1.2/src/bento_sts/sts.py
+-rw-r--r--   0        0        0     4633 2023-07-23 02:58:27.489244 bento_sts-0.1.2/src/bento_sts/templates/_intro.html
+-rw-r--r--   0        0        0     1511 2023-07-24 01:17:01.447618 bento_sts-0.1.2/src/bento_sts/templates/about-mdb.html
+-rw-r--r--   0        0        0     2160 2023-07-24 01:37:45.147781 bento_sts-0.1.2/src/bento_sts/templates/about-sts.html
+-rw-r--r--   0        0        0     3920 2023-07-09 20:16:17.668929 bento_sts-0.1.2/src/bento_sts/templates/base.html
+-rw-r--r--   0        0        0      188 2023-07-07 02:01:31.468445 bento_sts-0.1.2/src/bento_sts/templates/errors/400.html
+-rw-r--r--   0        0        0      163 2023-07-07 02:01:31.467946 bento_sts-0.1.2/src/bento_sts/templates/errors/404.html
+-rw-r--r--   0        0        0      234 2023-07-07 02:01:31.467192 bento_sts-0.1.2/src/bento_sts/templates/errors/500.html
+-rw-r--r--   0        0        0      756 2023-07-09 20:12:27.105105 bento_sts-0.1.2/src/bento_sts/templates/explore.html
+-rw-r--r--   0        0        0     2557 2023-07-24 01:24:40.494734 bento_sts-0.1.2/src/bento_sts/templates/index.html
+-rw-r--r--   0        0        0     1172 2023-07-09 20:12:08.555392 bento_sts-0.1.2/src/bento_sts/templates/mdb-model.html
+-rw-r--r--   0        0        0     1422 2023-07-09 20:11:41.928393 bento_sts-0.1.2/src/bento_sts/templates/mdb-node-list.html
+-rw-r--r--   0        0        0     3524 2023-07-07 02:01:31.463259 bento_sts-0.1.2/src/bento_sts/templates/mdb-node.html
+-rw-r--r--   0        0        0      602 2023-07-07 02:01:31.462192 bento_sts-0.1.2/src/bento_sts/templates/mdb-origin.html
+-rw-r--r--   0        0        0     3532 2023-07-07 02:01:31.461399 bento_sts-0.1.2/src/bento_sts/templates/mdb-property.html
+-rw-r--r--   0        0        0     1611 2023-07-07 02:01:31.460557 bento_sts-0.1.2/src/bento_sts/templates/mdb-tag.html
+-rw-r--r--   0        0        0     1236 2023-07-21 02:43:23.999867 bento_sts-0.1.2/src/bento_sts/templates/mdb-term.html
+-rw-r--r--   0        0        0     1789 2023-07-09 20:12:03.737714 bento_sts-0.1.2/src/bento_sts/templates/mdb-valueset.html
+-rw-r--r--   0        0        0     4004 2023-07-09 20:10:58.458009 bento_sts-0.1.2/src/bento_sts/templates/mdb.html
+-rw-r--r--   0        0        0     2589 2023-07-09 20:12:31.308854 bento_sts-0.1.2/src/bento_sts/templates/reports.html
+-rw-r--r--   0        0        0     1872 2023-07-07 02:01:31.455624 bento_sts-0.1.2/src/bento_sts/templates/search.html
+-rw-r--r--   0        0        0      495 2023-07-09 20:12:22.063962 bento_sts-0.1.2/src/bento_sts/templates/version-history-report.html
+-rw-r--r--   0        0        0      500 2023-07-09 20:12:13.305029 bento_sts-0.1.2/src/bento_sts/templates/version-history.html
+-rw-r--r--   0        0        0      204 2023-07-07 02:01:31.454103 bento_sts-0.1.2/src/bento_sts/util.py
+-rw-r--r--   0        0        0    10852 2023-07-07 02:01:31.309361 bento_sts-0.1.2/swagger/nodejs-server-server-generated.zip
+-rw-r--r--   0        0        0    18715 2023-07-18 16:42:04.940479 bento_sts-0.1.2/swagger/pysts-api.yaml
+-rw-r--r--   0        0        0      885 2023-07-07 02:01:31.310135 bento_sts-0.1.2/swagger/python-flask-server/.dockerignore
+-rw-r--r--   0        0        0      786 2023-07-07 02:01:31.310787 bento_sts-0.1.2/swagger/python-flask-server/.gitignore
+-rw-r--r--   0        0        0        6 2023-07-07 02:01:31.312195 bento_sts-0.1.2/swagger/python-flask-server/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     1030 2023-07-07 02:01:31.311497 bento_sts-0.1.2/swagger/python-flask-server/.swagger-codegen-ignore
+-rw-r--r--   0        0        0      246 2023-07-07 02:01:31.313276 bento_sts-0.1.2/swagger/python-flask-server/Dockerfile
+-rw-r--r--   0        0        0     1115 2023-07-14 01:07:14.515754 bento_sts-0.1.2/swagger/python-flask-server/README.md
+-rw-r--r--   0        0        0     1628 2023-07-07 02:01:31.314846 bento_sts-0.1.2/swagger/python-flask-server/git_push.sh
+-rw-r--r--   0        0        0       65 2023-07-14 01:15:29.318240 bento_sts-0.1.2/swagger/python-flask-server/requirements.txt
+-rw-r--r--   0        0        0     1253 2023-07-07 02:01:31.315777 bento_sts-0.1.2/swagger/python-flask-server/setup.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:01:31.315951 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/__init__.py
+-rw-r--r--   0        0        0      353 2023-07-07 02:01:31.316657 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-07 02:01:31.316976 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-07 02:01:31.318229 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/id_controller.py
+-rw-r--r--   0        0        0     5910 2023-07-07 02:01:31.319216 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/model_controller.py
+-rw-r--r--   0        0        0      426 2023-07-07 02:01:31.320206 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/models_controller.py
+-rw-r--r--   0        0        0     1081 2023-07-07 02:01:31.321098 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tag_controller.py
+-rw-r--r--   0        0        0      356 2023-07-07 02:01:31.321801 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tags_controller.py
+-rw-r--r--   0        0        0      608 2023-07-07 02:01:31.322521 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/encoder.py
+-rw-r--r--   0        0        0      393 2023-07-07 02:01:31.323225 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-07 02:01:31.323881 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     2291 2023-07-07 02:01:31.324334 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/entity.py
+-rw-r--r--   0        0        0     3551 2023-07-07 02:01:31.324767 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model.py
+-rw-r--r--   0        0        0     6112 2023-07-07 02:01:31.325214 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model_property.py
+-rw-r--r--   0        0        0     2978 2023-07-07 02:01:31.325734 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/node.py
+-rw-r--r--   0        0        0     2885 2023-07-07 02:01:31.326336 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/tag.py
+-rw-r--r--   0        0        0     4604 2023-07-07 02:01:31.326925 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/term.py
+-rw-r--r--   0        0        0    21512 2023-07-07 02:01:31.327834 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      415 2023-07-07 02:01:31.328553 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-07 02:01:31.329053 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_id_controller.py
+-rw-r--r--   0        0        0     5798 2023-07-07 02:01:31.329691 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_model_controller.py
+-rw-r--r--   0        0        0     1029 2023-07-07 02:01:31.330310 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_models_controller.py
+-rw-r--r--   0        0        0     1688 2023-07-07 02:01:31.331002 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tag_controller.py
+-rw-r--r--   0        0        0      952 2023-07-07 02:01:31.331519 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tags_controller.py
+-rw-r--r--   0        0        0     3384 2023-07-07 02:01:31.332007 bento_sts-0.1.2/swagger/python-flask-server/swagger_server/util.py
+-rw-r--r--   0        0        0       90 2023-07-07 02:01:31.332560 bento_sts-0.1.2/swagger/python-flask-server/test-requirements.txt
+-rw-r--r--   0        0        0      143 2023-07-07 02:01:31.333171 bento_sts-0.1.2/swagger/python-flask-server/tox.ini
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 bento_sts-0.1.2/setup.py
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 bento_sts-0.1.2/PKG-INFO
```

### Comparing `bento_sts-0.1.1/LICENSE` & `bento_sts-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/pyproject.toml` & `bento_sts-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 [project]
 name = "bento-sts"
-version = "0.1.1"
-author = "Mark Benson"
-author_email = "mark.benson@nih.gov"
+version = "0.1.2"
+authors = [
+{ name="Mark Benson", email="mark.benson@nih.gov"},
+{ name="Mark A. Jensen", email="mark.jensen@nih.gov"},
+]
 maintainer = "Mark A. Jensen"
 maintainer_email = "mark.jensen@nih.gov"
 description = "Bento Simple Terminology Server"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache License"
 ]
 [project.urls]
 "Homepage" = "https://github.com/CBIIT/bento-sts"
 "Bug Tracker" = "https:/github.com/CBIIT/bento-sts/issues"
 
-
-#[options]
-#    package_dir =
-#        = app
-#    packages = find:
-
 [tool.poetry]
 name = "bento-sts"
-version = "0.1.1"
+version = "0.1.2"
 description = "Bento Simple Terminology Server"
 authors = [
 	"Mark Benson <mark.benson@nih.gov>",
 	"Mark A. Jensen <mark.jensen@nih.gov>",
 ]
 license = "Apache 2.0"
 readme = "README.md"
```

### Comparing `bento_sts-0.1.1/src/bento_sts/api/routes.py` & `bento_sts-0.1.2/src/bento_sts/api/routes.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/config.py` & `bento_sts-0.1.2/src/bento_sts/config.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/config_sts/query_paths.yml` & `bento_sts-0.1.2/src/bento_sts/config_sts/query_paths.yml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/main/forms.py` & `bento_sts-0.1.2/src/bento_sts/main/forms.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/main/routes.py` & `bento_sts-0.1.2/src/bento_sts/main/routes.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/mdb.py` & `bento_sts-0.1.2/src/bento_sts/mdb.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/mdb_tags.py` & `bento_sts-0.1.2/src/bento_sts/mdb_tags.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/mdb_update.py` & `bento_sts-0.1.2/src/bento_sts/mdb_update.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/static/loading.gif` & `bento_sts-0.1.2/src/bento_sts/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/sts.py` & `bento_sts-0.1.2/src/bento_sts/sts.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/_intro.html` & `bento_sts-0.1.2/src/bento_sts/templates/_intro.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 <div>
 
-    <h2> Bento Meta DB </h2>
+    <h2> Bento Metamodel Database </h2>
     The metamodel database (MDB) records
     <ul>
         <li>node/relationship/property structure of models;</li>
         <li>the official local vocabulary - terms that are employed in the backend data system;;</li>
         <li>synonyms for local vocabulary mapped from external standards; and;</li>
         <li>the value sets for properties with enumerated value domains, and data types for other properties.;</li>
     </ul>
-    <p>    
+    <p>
 The production instance of MDB will contain the "official" representation of a data model, in that it will record the curated external terminology mappings and official sets of valid terms for each relevant property. In this way, the MDB is an extension of the MDF for any model it contains.
-<p>
+    <p>
+
 As the central location for official mappings to external vocabularies, the MDC can (should) be used as part of software modules that convert between the data physically stored in the production database and external standards. For example, an API known as the Simple Terminology Service STS, using MDB as its backend, will be used for simple queries about a given model and validation of incoming data.
 
 <h3>Structure </h3>
 
-The MDB is formulated as a graph model. This model contains more structure than will be exposed by the Simple Terminology Service (in order to keep it Simple). Other services can be built on the DB to perform translations, add terms and mappings, create visualizations, and other functions.
+The MDB schema is formulated as a graph model. This model contains more structure than exposed by the Simple Terminology Service (keeping it Simple). Other services can be built on the DB to perform translations, add terms and mappings, create visualizations, and other functions.
 
 The metamodel is described in a Model Description File. Documents and tools for this format are at bento-mdf.
 
 The MDB model contains the following nodes.
 
 <h3>Node</h3>
 A node with the label "node" in the MDB represents a model node: for example, a Diagnosis node.
@@ -29,21 +30,23 @@
 
 <h3>Property</h3>
 A Property node in the Model DB represents a property of a model node: for example, the disease property of a Diagnosis node.
 
 <h3>Concept</h3>
 A Concept node represents an intellectual concept. It is abstract, in that it has no human readable name as such; it will however have a unique ID. The Concept node can be thought of as a connecting point for sets of Terms that are identical in meaning (are synonymous).
 
+The Concept node in the MDB is loosely related, but not the same as, a concept entity defined in, for example, the NCI Thesaurus.
+
 <h3>Origin</h3>
-An Origin node represents an entity (institution, internal project, defined standard, recognized body, public database) that defines and/or promulgates a terminology and represents it authoritatively.
+An Origin node represents an entity (institution, internal project, defined standard, recognized body, public database) that defines and/or promulgates a terminology and represents it normatively or authoritatively. 
 
 <h3>Term > Value</h3>
-A Term node is an instance of encoding (a "representation") of a concept. Each Term node is linked to at least one Origin node, which represents the entity that provides the term value/code and/or the term semantics.
+A Term node is an instance of an encoding (a "representation") of a concept. Each Term node refers to an Origin node (via the property "origin_name"). This indicates the authority that provides the term value/code and/or the term semantics.
 
-The value property of a Term node is the string representation of the term. This is a token that, for example, may be physically stored in a database as a datum.
+The value property of a Term node is the string representation of the term, according to the authority (Origin). This is a string that, for example, may be physically stored in a database as a datum.
 
 <h3>Value Set</h3>
 A Value Set node aggregates (links to) a number of Term nodes that define the list of acceptable values for a property slot. The value set does not directly aggregate Concepts; it is meant to define the pragmatic set of valid representations of values for a property.
 
 <h3>Concept Group</h3>
 A Concept Group node aggregates (i.e., links to) Concept nodes. Concept Groups might be implicit. A Value Set node, for example, implicitly defines a Concept Group - the set of those Concept nodes that are linked to the Term nodes aggregated by the Value Set.
```

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/base.html` & `bento_sts-0.1.2/src/bento_sts/templates/base.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/explore.html` & `bento_sts-0.1.2/src/bento_sts/templates/explore.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/index.html` & `bento_sts-0.1.2/src/bento_sts/templates/reports.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,89 @@
 {% extends "base.html" %}
 {% from 'bootstrap4/form.html' import render_form, render_field %}
 
 {% block app_content %}
+    <br>
+    <h4> Model Data by Browser</h4>
+    <nav aria-label="...">
+        <ul class="pager">
+      <li class="model">
+         <a href="{{ url_for('main.models') }}"> List Models </a>
+      </li>
+      <li class="nodes">
+         <a href="{{ url_for('main.nodes') }}"> List Nodes </a>
+      </li>
+      <li class="properties">
+         <a href="{{ url_for('main.properties') }}"> List Properties </a>
+      </li>
+      <li class="terms">
+         <a href="{{ url_for('main.terms') }}"> List Terms </a>
+      </li>
+      <li class="origins">
+         <a href="{{ url_for('main.origins') }}"> List Origins </a>
+      </li>
+    </ul>
+    </nav>
 
-<div class="container">
-   <div class="row">
-       <div class="col-6">
-
-            <br>
-            <h4> Model Data Browser</h4>
-            <nav aria-label="...">
-               <ul class="pager">
-               <li class="model">
-                  <a href="{{ url_for('main.models') }}"> List Models </a>
-               </li>
-               <li class="nodes">
-                  <a href="{{ url_for('main.entities',entities='nodes') }}"> List Nodes </a>
-               </li>
-               <li class="properties">
-                  <a href="{{ url_for('main.entities',entities='properties') }}"> List Properties </a>
-               </li>
-               <li class="terms">
-                  <a href="{{ url_for('main.entities',entities='terms') }}"> List Terms </a>
-               </li>
-               <li class="origins">
-                  <a href="{{ url_for('main.entities',entities='origins') }}"> List Origins </a>
-               </li>
-            </ul>
-            </nav> 
-         <br>
-      </div>
 
-<div class="col-6">
-      <br>
-      <h4> About </h4>
-      <ul class="pager">
-        <li class="aboutmdb">
-         <a href="{{ url_for( 'main.about_mdb') }}">About MDB</a>
-        </li>
-        <li>
-         <a href="{{ url_for( 'main.about_sts') }}">About STS</a> and how to filter
-        </li>
-       </ul> 
+
+    <br>
+    <div>
+    <h4><a href="{{ url_for( 'main.about_mdb') }}">About MDB</a></h4>
+    <br>
+    <br>
+    <h4><a href="{{ url_for( 'main.about_sts') }}">About STS</a> and how to filter</h4>
+    <br>
+    <br>
+    <h4><a href="{{ url_for( 'main.diff') }}">MDF Diff</a> -- Find the diff between 2 MDF files</h4>
+
+    <br>
+    <br>
+    <h4> Data Subsets</h4>
+    <ul class="pager">
+         <li class="tags">
+               <a href="{{ url_for('datasubsets.tags') }}"> List All Tagged Data</a>
+         </li>
+         <li class="tag-select">
+               <a href="{{ url_for('datasubsets.tagselect') }}"> Select Data Subsets</a>
+         </li>
+         <li class="tag-delta">
+               <a href="{{ url_for('datasubsets.tagdelta') }}"> Edit Data Subsets</a>
+         </li>
+         <li class="tag-export">
+               <a href="{{ url_for('datasubsets.tagexport') }}"> Export Data Plan</a>
+         </li>
+   </ul>
 
    <br>
+   <br>
    <h4> Reports and Version History</h4>
    <ul class="pager">
+      <li class="reports">
+         <a href="{{ url_for('main.reports') }}"> Releases and Data Reports</a>
+      </li>
+        <li class="version-history">
+              <a href="{{ url_for('main.versionhistory') }}"> Version History</a>
+        </li>
       </ul>     
 
+      <br>
    <br>
    <h4> External Resources</h4>
    <ul class="pager">
 
       <li class="ncit">
          <a href="https://ncithesaurus.nci.nih.gov/ncitbrowser/"> NCI Thesaurus</a>
       </li>
         <li class="evs">
               <a href="https://evs.nci.nih.gov/"> NCI EVS</a>
         </li>
-        <li class="cde">
-         <a href="https://cdebrowser.nci.nih.gov/cdebrowserClient/cdeBrowser.html#/search"> NCI CDE Browser </a>
+        <li class="icdc">
+         <a href="https://caninecommons.cancer.gov/#/"> ICDC </a>
       </li>
       <li class="umls">
-         <a href="https://www.nlm.nih.gov/research/umls/index.html"> UMLS</a>
+         <a href="https://www.nlm.nih.gov/research/umls/index.htm"> UMLS</a>
       </li>
       </ul>
-   </div>
 
 </div>
-</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,23 +1,36 @@
 {% extends "base.html" %} {% from 'bootstrap4/form.html' import render_form,
 render_field %} {% block app_content %}
-
-*** Model Data Browser ***
+*** Model Data by Browser ***
     * List_Models
     * List_Nodes
     * List_Properties
     * List_Terms
     * List_Origins
 
+*** About_MDB ***
+
+
+*** About_STS and how to filter ***
+
+
+*** MDF_Diff -- Find the diff between 2 MDF files ***
+
+
+*** Data Subsets ***
+    * List_All_Tagged_Data
+    * Select_Data_Subsets
+    * Edit_Data_Subsets
+    * Export_Data_Plan
 
-*** About ***
-    * About_MDB
-    * About_STS and how to filter
 
 *** Reports and Version History ***
+    * Releases_and_Data_Reports
+    * Version_History
+
 
 *** External Resources ***
     * NCI_Thesaurus
     * NCI_EVS
-    * NCI_CDE_Browser
+    * ICDC
     * UMLS
 {% endblock %}
```

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-model.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-model.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-node-list.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-node-list.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-node.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-node.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-origin.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-origin.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-property.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-property.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-tag.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-tag.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-term.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-term.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,42 +14,27 @@
       <table class="table-striped">
          <tr>
             <th style="width:300px"> Term Value </th> 
             <td style="width:300px"> <a href="{{url_for( 'main.entities', entities=subtype, id=mdb.id ) }}"> {{mdb.value}} </a>        </td>
        </tr>
          <tr>
              <th> Id </th> <td>{{mdb.id}} </td>
-        </tr>
+         </tr>
+     {% if mdb.has_origin  %}	 
+	 <tr>
+	   <th> Origin </th> <td><a href="{{mdb.has_origin.link}}">{{mdb.origin_name}}</a></td>
+	 </tr>
        <tr>
         <th> Origin Id </th> <td>{{mdb.origin_id}} </td>
-   </tr>
+       </tr>
+     {% endif %}
    <tr>
        <th> Origin Definition </th> <td>{{mdb.origin_definition}} </td>
   </tr>
       </table>
       </div>
     </div>
 {% block edit_functions %}
 {% endblock edit_functions %}
     <br><br>
-    <div>
-        {% if mdb.has_origin %}
-        <h3> Origin  </h3>
-        <div id="valuesetDetail" name="valuesetDetail" style="margin:20px; padding:20x">
-
-            <table  class="table-striped">
-                <tr> <th style="width:300px"> Origin Name  </th>  
-		<td style="width:300px">
-		  <a href="{{url_for( 'main.entities', entities='origins',id=mdb.has_origin.id ) }}"> {{ mdb.has_origin.name }}</a> </td>
-                </tr>
-                <tr> 
-                    <th>  Id </th>  
-                    <td> {{ mdb.has_origin.id }} </td>
-                </tr>
-            </table>
-            <br>
-            </div>
-        {% endif %}
-    </div>
-
     {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,18 +3,13 @@
 {% if display == 'detail' %}
 Export_JSON
 
 
 **** Details ****
 Term Value        {{mdb.value}}
 Id                {{mdb.id}}
+Origin            {{mdb.origin_name}}
 Origin Id         {{mdb.origin_id}}
 Origin Definition {{mdb.origin_definition}}
 {% block edit_functions %} {% endblock edit_functions %}
 
-{% if mdb.has_origin %}
-**** Origin ****
-Origin Name {{_mdb.has_origin.name_}}
-Id          {{ mdb.has_origin.id }}
-
-{% endif %}
 {% endif %} {% endblock %}
```

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb-valueset.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb-valueset.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/mdb.html` & `bento_sts-0.1.2/src/bento_sts/templates/mdb.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/src/bento_sts/templates/search.html` & `bento_sts-0.1.2/src/bento_sts/templates/search.html`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/nodejs-server-server-generated.zip` & `bento_sts-0.1.2/swagger/nodejs-server-server-generated.zip`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/pysts-api.yaml` & `bento_sts-0.1.2/swagger/pysts-api.yaml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/.dockerignore` & `bento_sts-0.1.2/swagger/python-flask-server/.dockerignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/.gitignore` & `bento_sts-0.1.2/swagger/python-flask-server/.gitignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/.swagger-codegen-ignore` & `bento_sts-0.1.2/swagger/python-flask-server/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/README.md` & `bento_sts-0.1.2/swagger/python-flask-server/README.md`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/git_push.sh` & `bento_sts-0.1.2/swagger/python-flask-server/git_push.sh`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/setup.py` & `bento_sts-0.1.2/swagger/python-flask-server/setup.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/model_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/controllers/tag_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/controllers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/encoder.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/base_model_.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/entity.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/entity.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/model_property.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/model_property.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/node.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/node.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/tag.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/tag.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/models/term.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/models/term.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/swagger/swagger.yaml` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/swagger/swagger.yaml`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_id_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_id_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_model_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_model_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_models_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_models_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tag_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tag_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/test/test_tags_controller.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/test/test_tags_controller.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/swagger/python-flask-server/swagger_server/util.py` & `bento_sts-0.1.2/swagger/python-flask-server/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `bento_sts-0.1.1/setup.py` & `bento_sts-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'requests>=2.20.0',
  'six>=1.15.0',
  'urllib3>=1.26.5',
  'visitor>=0.1.3']
 
 setup_kwargs = {
     'name': 'bento-sts',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Bento Simple Terminology Server',
     'long_description': '# Welcome to bento-sts\n\nThis is a flask-based implementation of the Simple Terminology Service (STS) for the Bento Metadatabase (MDB).\n\n## Install\n\n\t$ git clone https://github.com/CBIIT/bento-sts.git\n\t$ cd pysts\n\t$ virtualenv sts-venv\n\t$ source sts-venv/bin/activate\n\t$ pip install -r requirements.txt\n\t$ flask run\n\n## Dependencies\n\n`bento-sts` requires a Neo4j-based [MDB](https://github.com/CBIIT/bento-meta).\n\n\n\n',
     'author': 'Mark Benson',
     'author_email': 'mark.benson@nih.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bento_sts-0.1.1/PKG-INFO` & `bento_sts-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-sts
-Version: 0.1.1
+Version: 0.1.2
 Summary: Bento Simple Terminology Server
 License: Apache 2.0
 Author: Mark Benson
 Author-email: mark.benson@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

