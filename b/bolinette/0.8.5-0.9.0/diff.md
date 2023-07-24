# Comparing `tmp/Bolinette-0.8.5.tar.gz` & `tmp/Bolinette-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bolinette-0.8.5.tar", last modified: Thu May  6 22:22:19 2021, max compression
+gzip compressed data, was "Bolinette-0.9.0.tar", last modified: Mon Jun 28 15:54:11 2021, max compression
```

## Comparing `Bolinette-0.8.5.tar` & `Bolinette-0.9.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.502314 Bolinette-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/Bolinette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-05-06 22:22:19.000000 Bolinette-0.8.5/Bolinette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2021-05-06 22:22:19.000000 Bolinette-0.8.5/Bolinette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-06 22:22:19.000000 Bolinette-0.8.5/Bolinette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-05-06 22:22:19.000000 Bolinette-0.8.5/Bolinette.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-05-06 22:22:19.000000 Bolinette-0.8.5/Bolinette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-05-06 22:21:58.000000 Bolinette-0.8.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-06 22:21:58.000000 Bolinette-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-05-06 22:22:19.502314 Bolinette-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-05-06 22:21:58.000000 Bolinette-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/bolinette/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.486314 Bolinette-0.8.5/bolinette/_files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/bolinette/_files/env/
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/_files/env/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/bolinette/_files/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/bolinette/_files/templates/common/
--rw-r--r--   0 runner    (1001) docker     (121)    56745 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/_files/templates/common/base.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/_files/templates/common/error.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.490314 Bolinette-0.8.5/bolinette/_files/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/_files/templates/errors/404.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/_files/templates/no_docs.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/bcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/blnt/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/blnt/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/commands/argument.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2879 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/commands/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/context.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/blnt/database/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/blnt/database/engines/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/engines/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/engines/relational.py
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/blnt/database/queries/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/queries/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/queries/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/database/queries/relational.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/props.py
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/transaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/blnt/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3842 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/bolinette.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/create_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/init_db.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/init_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/commands/run_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/console.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/core/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/core/models/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/models/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/core/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     7904 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.494314 Bolinette-0.8.5/bolinette/defaults/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/static.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/timezone.py
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/controllers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/middlewares/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/middlewares/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/middlewares/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/mixins/historized.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/models/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/models/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/models/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/services/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/services/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/services/role.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/services/timezone.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/services/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/defaults/topics/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/topics/role.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/defaults/topics/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     8810 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/mail/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/mail/providers/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mail/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mail/providers/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mail/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/mapping/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mapping/mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/mapping/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.498314 Bolinette-0.8.5/bolinette/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/testing/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/testing/fixture.py
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/testing/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.502314 Bolinette-0.8.5/bolinette/types/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/types/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/types/defs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.502314 Bolinette-0.8.5/bolinette/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/utils/serializing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 22:22:19.502314 Bolinette-0.8.5/bolinette/web/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13457 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/method.py
--rw-r--r--   0 runner    (1001) docker     (121)     3074 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/sockets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2021-05-06 22:21:58.000000 Bolinette-0.8.5/bolinette/web/topic.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-06 22:21:58.000000 Bolinette-0.8.5/manifest.blnt.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-06 22:22:19.502314 Bolinette-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-05-06 22:21:58.000000 Bolinette-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/Bolinette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-06-28 15:54:11.000000 Bolinette-0.9.0/Bolinette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2021-06-28 15:54:11.000000 Bolinette-0.9.0/Bolinette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-28 15:54:11.000000 Bolinette-0.9.0/Bolinette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-06-28 15:54:11.000000 Bolinette-0.9.0/Bolinette.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-06-28 15:54:11.000000 Bolinette-0.9.0/Bolinette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-06-28 15:53:48.000000 Bolinette-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-06-28 15:53:48.000000 Bolinette-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-06-28 15:54:11.225754 Bolinette-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-06-28 15:53:48.000000 Bolinette-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.209754 Bolinette-0.9.0/bolinette/_files/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/_files/env/
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/_files/env/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/_files/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/_files/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (121)    56745 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/_files/templates/common/base.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/_files/templates/common/error.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/_files/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/_files/templates/errors/404.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/_files/templates/no_docs.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/bcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/blnt/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/blnt/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/commands/argument.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4567 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/commands/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4758 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/context.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/blnt/database/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.217754 Bolinette-0.9.0/bolinette/blnt/database/engines/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/engines/collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/engines/relational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/blnt/database/queries/
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2642 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/queries/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2659 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/queries/collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/database/queries/relational.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/props.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/blnt/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3642 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/bolinette.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/init_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/commands/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/console.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/core/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4095 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/models/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2451 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4825 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3251 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/core/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7904 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/static.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6871 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/controllers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/middlewares/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5927 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/middlewares/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/mixins/historized.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2271 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.221754 Bolinette-0.9.0/bolinette/defaults/services/
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/services/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/services/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/services/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/services/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/defaults/topics/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/topics/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/defaults/topics/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9343 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9309 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/init.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/mail/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/mail/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mail/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mail/providers/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mail/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/mapping/
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6388 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mapping/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3050 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/mapping/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/testing/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/testing/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4239 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/testing/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/types/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/types/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/types/defs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/utils/serializing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-28 15:54:11.225754 Bolinette-0.9.0/bolinette/web/
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15135 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3074 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5546 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2105 2021-06-28 15:53:48.000000 Bolinette-0.9.0/bolinette/web/topic.py
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-06-28 15:53:48.000000 Bolinette-0.9.0/manifest.blnt.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-06-28 15:54:11.225754 Bolinette-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-06-28 15:53:48.000000 Bolinette-0.9.0/setup.py
```

### Comparing `Bolinette-0.8.5/Bolinette.egg-info/PKG-INFO` & `Bolinette-0.9.0/Bolinette.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bolinette
-Version: 0.8.5
+Version: 0.9.0
 Summary: An asynchronous Python web framework
 Home-page: https://github.com/TheCaptainCat/bolinette
 Author: Pierre Chat
 Author-email: pierrechat@outlook.com
 License: MIT
 Description: # Bolinette
```

### Comparing `Bolinette-0.8.5/Bolinette.egg-info/SOURCES.txt` & `Bolinette-0.9.0/Bolinette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/LICENSE.txt` & `Bolinette-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/PKG-INFO` & `Bolinette-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bolinette
-Version: 0.8.5
+Version: 0.9.0
 Summary: An asynchronous Python web framework
 Home-page: https://github.com/TheCaptainCat/bolinette
 Author: Pierre Chat
 Author-email: pierrechat@outlook.com
 License: MIT
 Description: # Bolinette
```

### Comparing `Bolinette-0.8.5/README.md` & `Bolinette-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/_files/templates/common/base.jinja2` & `Bolinette-0.9.0/bolinette/_files/templates/common/base.jinja2`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/_files/templates/common/error.jinja2` & `Bolinette-0.9.0/bolinette/_files/templates/common/error.jinja2`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/_files/templates/no_docs.html.jinja2` & `Bolinette-0.9.0/bolinette/_files/templates/no_docs.html.jinja2`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/cache.py` & `Bolinette-0.9.0/bolinette/blnt/cache.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/commands/parser.py` & `Bolinette-0.9.0/bolinette/blnt/commands/parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,92 @@
 import asyncio
 import inspect
 import sys
 from argparse import ArgumentParser
-from typing import Dict
+from typing import Dict, List
 
 import bolinette
 from bolinette import Console
+from bolinette.exceptions import InitError
 from bolinette.blnt.commands import Command, Argument
 from bolinette.utils.functions import async_invoke, invoke
 
 
 class Parser:
     def __init__(self, blnt: 'bolinette.Bolinette', commands: Dict[str, Command]):
         self.blnt = blnt
         self.commands = commands
         self._factories = {
             'argument': self._create_argument,
             'option': self._create_option,
             'flag': self._create_flag
         }
+        self._console = Console()
+        self._sub_commands = {}
 
     def run(self):
+        tree = self._parse_commands()
         parser = ArgumentParser(description='Bolinette Web Framework')
         sub_parsers = parser.add_subparsers()
-        for _, command in self.commands.items():
-            sub_parser = sub_parsers.add_parser(command.name, help=command.summary)
-            for arg in command.args:
-                self._factories[arg.arg_type](arg, sub_parser)
-            sub_parser.set_defaults(__blnt__=command.name)
+        self._build_parsers(tree, sub_parsers, [])
         parsed = vars(parser.parse_args())
-        if '__blnt__' not in parsed:
-            Console().error('Use the -h option to see CLI usage')
+        if '__blnt_cmd__' in parsed:
+            cmd = parsed.pop('__blnt_cmd__')
+            self._run_command(cmd, parsed)
+        elif '__blnt_path__' in parsed:
+            self._console.error(self._sub_commands[parsed['__blnt_path__']].format_help())
+            sys.exit(1)
+        else:
+            self._console.error(parser.format_help())
             sys.exit(1)
-        cmd = parsed.pop('__blnt__')
+
+    def _run_command(self, cmd: str, parsed: dict):
         func = self.commands[cmd].func
         parsed['blnt'] = self.blnt
         parsed['context'] = self.blnt.context
+        self.blnt.init_bolinette()
         if inspect.iscoroutinefunction(func):
             loop = asyncio.get_event_loop()
             loop.run_until_complete(async_invoke(func, **parsed))
         else:
             invoke(func, **parsed)
 
+    def _parse_commands(self):
+        command_tree = {}
+        for _, command in self.commands.items():
+            cur_node = command_tree
+            path = command.path.split(' ')
+            for elem in path[:-1]:
+                if elem not in cur_node:
+                    cur_node[elem] = {}
+                cur_node = cur_node[elem]
+            elem = path[-1]
+            if elem in cur_node:
+                raise InitError(f'Conflict with "{command.name}" command')
+            cur_node[elem] = command
+        return command_tree
+
+    def _build_parsers(self, command_tree: dict, sub_parsers, path: List[str]):
+        for name, elem in command_tree.items():
+            if isinstance(elem, Command):
+                sub_parser = sub_parsers.add_parser(name, help=elem.summary)
+                for arg in elem.args:
+                    self._factories[arg.arg_type](arg, sub_parser)
+                sub_parser.set_defaults(__blnt_cmd__=elem.name)
+            else:
+                sub_parser = sub_parsers.add_parser(name, help=self._build_help(elem, path + [name]))
+                sub_parser.set_defaults(__blnt_path__=name)
+                self._sub_commands[name] = sub_parser
+                self._build_parsers(elem, sub_parser.add_subparsers(), path + [name])
+    
+    @staticmethod
+    def _build_help(command_tree: dict, path: List[str]):
+        cmds = [f'"{" ".join(path + [x])}"' for x in command_tree]
+        return 'Sub-commands: ' + ', '.join(cmds)
+
     @staticmethod
     def _create_parser_arg(arg: Argument, *, optional: bool = False, use_flag: bool = False,
                            action: str = None):
         args = []
         kwargs = {}
         if optional:
             args.append(f'--{arg.name}')
```

### Comparing `Bolinette-0.8.5/bolinette/blnt/context.py` & `Bolinette-0.9.0/bolinette/blnt/context.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/engines/collection.py` & `Bolinette-0.9.0/bolinette/blnt/database/engines/collection.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/engines/relational.py` & `Bolinette-0.9.0/bolinette/blnt/database/engines/relational.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/manager.py` & `Bolinette-0.9.0/bolinette/blnt/database/manager.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/queries/base.py` & `Bolinette-0.9.0/bolinette/blnt/database/queries/base.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/queries/collection.py` & `Bolinette-0.9.0/bolinette/blnt/database/queries/collection.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/database/queries/relational.py` & `Bolinette-0.9.0/bolinette/blnt/database/queries/relational.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sqlalchemy
+from sqlalchemy import orm as sqlalchemy_orm
 
 from bolinette import blnt, core
 from bolinette.blnt.database.engines import RelationalDatabase
 from bolinette.blnt.database.queries import BaseQueryBuilder, BaseQuery
+from bolinette.exceptions import InternalError
 
 
 class RelationalQueryBuilder(BaseQueryBuilder):
     def __init__(self, model: 'core.Model', context: 'blnt.BolinetteContext'):
         super().__init__(model, context)
         self._database: RelationalDatabase = context.db[model.__blnt__.database]
         self._table = self.context.table(model.__blnt__.name)
@@ -46,21 +48,32 @@
 
     async def get_by_id(self, identifier):
         return self._query().get(identifier)
 
     async def count(self):
         return self._build_query().count()
 
-    def _query(self):
+    def _query(self) -> sqlalchemy_orm.Query:
         return self._database.session.query(self._table)
 
+    def _build_filters_by(self, query: sqlalchemy_orm.Query) -> sqlalchemy_orm.Query:
+        for key, value in self._filters_by.items():
+            path = key.split('.')
+            if len(path) == 1:
+                query = query.filter(getattr(self._table, key) == value)
+            elif len(path) == 2:
+                query = query.filter(getattr(self._table, path[0]).has(**{path[1]: value}))
+            else:
+                raise InternalError(f'internal.query.wrong_model_id_path:{key}')
+        return query
+
     def _build_query(self):
         query = self._query()
         if len(self._filters_by) > 0:
-            query = query.filter_by(**self._filters_by)
+            query = self._build_filters_by(query)
         if len(self._filters) > 0:
             for function in self._filters:
                 query = query.filter(function(self._table))
         if len(self._order_by) > 0:
             for column, desc in self._order_by:
                 if hasattr(self._table, column):
                     col = getattr(self._table, column)
```

### Comparing `Bolinette-0.8.5/bolinette/blnt/environment.py` & `Bolinette-0.9.0/bolinette/blnt/environment.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/jwt.py` & `Bolinette-0.9.0/bolinette/blnt/jwt.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/objects.py` & `Bolinette-0.9.0/bolinette/blnt/objects.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/props.py` & `Bolinette-0.9.0/bolinette/blnt/props.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/transaction.py` & `Bolinette-0.9.0/bolinette/blnt/transaction.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/blnt/validation.py` & `Bolinette-0.9.0/bolinette/blnt/validation.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/bolinette.py` & `Bolinette-0.9.0/bolinette/bolinette.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 from bolinette.utils import paths
 
 
 class Bolinette:
     def __init__(self, *, extensions: List[BolinetteExtension] = None,
                  profile: str = None, overrides: Dict[str, Any] = None):
         self._start_time = datetime.utcnow()
-        self._init = False
-        self._init_ext = False
+        self._initialized = False
         self.app = None
         try:
             self.context = blnt.BolinetteContext(paths.dirname(__file__), extensions=extensions,
                                                  profile=profile, overrides=overrides)
             self.context.use_extension(Extensions.ALL)
         except InitError as init_error:
             Console().error(f'Error raised during Bolinette init phase\n{str(init_error)}')
@@ -39,51 +38,47 @@
                 self.console.debug(', ', end='')
             self.console.debug(str(func), end='')
             loop.run_until_complete(func(self.context))
             index += 1
         if index > 0:
             self.console.debug('')
 
-    def init(self, *, force=False):
-        if self._init and not force:
-            return
+    def init_bolinette(self):
         self._run_init_functions()
-        self._init = True
+        self.init_extensions()
+        self._initialized = True
 
-    def init_extensions(self, *, force=False):
-        if self._init_ext and not force:
-            return
+    def init_extensions(self):
         self.app = None
         if self.context.has_extension(Extensions.WEB):
-            if self.context.env['build_docs']:
-                self.context.docs.build()
-            self.context.docs.setup()
             self._init_web()
         if self.context.has_extension(Extensions.SOCKETS):
             self._init_sockets()
-        self._init_ext = True
 
     def _init_web(self):
         if self.app is None:
             self.app = aio_web.Application()
             self.app['blnt'] = self.context
         self.context.init_web(self.app)
+        if self.context.env['build_docs']:
+            self.context.docs.build()
+        self.context.docs.setup()
 
     def _init_sockets(self):
         if self.app is None:
             self.app = aio_web.Application()
             self.app['blnt'] = self.context
         self.context.init_sockets(self.app)
 
     def start_server(self, *, host: str = None, port: int = None):
+        if not self._initialized:
+            self.init_bolinette()
         if not self.context.has_extension((Extensions.WEB, Extensions.SOCKETS)):
             self.context.logger.error(f'The web or sockets extensions must be activated to start the aiohttp server!')
             sys.exit(1)
-        self.init()
-        self.init_extensions()
         self.console.debug(f'Startup took {int((datetime.utcnow() - self._start_time).microseconds / 1000)}ms')
         self.context.logger.info(f"Starting Bolinette with '{self.context.env['profile']}' environment profile")
         aio_web.run_app(self.app,
                         host=host or self.context.env['host'],
                         port=port or self.context.env['port'],
                         access_log=self.context.logger)
         self.context.logger.info(f"Bolinette stopped gracefully")
@@ -91,11 +86,9 @@
     def use(self, *extensions) -> 'Bolinette':
         self.context.clear_extensions()
         for ext in extensions:
             self.context.use_extension(ext)
         return self
 
     def exec_cmd_args(self):
-        self.init()
-        self.init_extensions()
         parser = Parser(self, blnt.cache.commands)
         parser.run()
```

### Comparing `Bolinette-0.8.5/bolinette/commands/create_user.py` & `Bolinette-0.9.0/bolinette/commands/create_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import bolinette
 from bolinette import Console
 from bolinette.blnt import Transaction
 from bolinette.decorators import command
 from bolinette.exceptions import ParamConflictError, EntityNotFoundError, APIError, APIErrors
 
 
-@command('create_user', 'Add a user to the database')
+@command('create user', 'Add a user to the database')
 @command.argument('argument', 'username', summary='The new user\'s username')
 @command.argument('argument', 'email', summary='The new user\'s email')
 @command.argument('option', 'roles', flag='r', summary='The user\'s roles, comma separated')
 async def create_user(blnt: 'bolinette.Bolinette', username: str, email: str, roles: str = None):
     console = Console()
     user_service = blnt.context.service('user')
     role_service = blnt.context.service('role')
```

### Comparing `Bolinette-0.8.5/bolinette/commands/init_db.py` & `Bolinette-0.9.0/bolinette/commands/init_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from bolinette import blnt
 from bolinette.decorators import command
 
 
-@command('init_db', 'Initialize the database')
+@command('init db', 'Initialize the database')
 @command.argument('flag', 'seeders', flag='s', summary='Run the seeders after database creation')
 async def init_db(context: 'blnt.BolinetteContext', seeders: bool):
     context.logger.info('==== Initializing database ====')
     context.logger.info('**** Dropping all tables')
     await context.db.drop_all()
     context.logger.info('**** Creating all tables')
     await context.db.create_all()
```

### Comparing `Bolinette-0.8.5/bolinette/console.py` & `Bolinette-0.9.0/bolinette/console.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/core/mixin.py` & `Bolinette-0.9.0/bolinette/core/mixin.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/core/models/attributes.py` & `Bolinette-0.9.0/bolinette/core/models/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,21 @@
         return f'{self.target_model_name}.{self.target_column_name}'
 
     def __repr__(self):
         return f'<Reference {self.model_name}.{self.column_name} -> {self.target_path}>'
 
 
 class Column:
-    def __init__(self, name: str, model: 'core.Model', data_type: 'types.db.DataType', reference: Optional[Reference],
-                 primary_key: bool, nullable: bool, unique: bool, model_id: bool, default: Optional[Any]):
+    def __init__(self, name: str, model: 'core.Model', data_type: 'types.db.DataType',
+                 reference: Optional[Reference], primary_key: bool, auto: Optional[bool],
+                 nullable: bool, unique: bool, model_id: bool, default: Optional[Any]):
         self.name = name
         self.type = data_type
         self.model = model
+        self.auto_increment = auto
         self.reference = reference
         self.primary_key = primary_key
         self.nullable = nullable
         self.unique = unique
         self.model_id = model_id
         self.default = default
```

### Comparing `Bolinette-0.8.5/bolinette/core/models/model.py` & `Bolinette-0.9.0/bolinette/core/models/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from typing import List, Union, Tuple, Dict, Iterator, Literal
 
 from bolinette import core, blnt
 from bolinette.blnt.database.engines import DatabaseEngine
-from bolinette.exceptions import InitError
 
 MappingPyTyping = List[Union['types.mapping.Column', 'types.mapping.Field',
                              'types.mapping.List', 'types.mapping.Definition']]
 MappingListPyTyping = Union[MappingPyTyping, Tuple[str, MappingPyTyping]]
 
 
 class Model:
     __blnt__: 'ModelMetadata' = None
 
     def __init__(self, database: 'DatabaseEngine'):
         self.__props__ = ModelProps(self, database)
 
-    @classmethod
-    def payloads(cls) -> MappingListPyTyping:
+    def payloads(self) -> MappingListPyTyping:
         pass
 
-    @classmethod
-    def responses(cls) -> MappingListPyTyping:
+    def responses(self) -> MappingListPyTyping:
         pass
 
     def get_mixin(self, name: str):
         return self.__props__.mixins[name]
 
     def __repr__(self):
         return f'<Model {self.__blnt__.name}>'
@@ -43,37 +40,16 @@
 
 class ModelProps(blnt.Properties):
     def __init__(self, model: Model, database: 'DatabaseEngine'):
         super().__init__(model)
         self.model = model
         self.database = database
         self.mixins: Dict[str, core.Mixin] = {}
-        # self.model_id: 'core.models.Column' = self._set_model_id()
-
-    @property
-    def model_id(self):
-        attrs = filter(lambda col: col[1].model_id, self.get_columns())
-        model_id = next(attrs)
-        return model_id[1]
-
-    def _set_model_id(self):
-        model_id = None
-        if self.model.__blnt__.join:
-            return model_id
-        for col_name, column in self.get_columns():
-            if column.model_id and model_id is not None:
-                raise InitError(f'Model "{self.model.__blnt__.name}" already has a model id')
-            if column.model_id:
-                model_id = column
-        if model_id is None:
-            raise InitError(f'Model "{self.model.__blnt__.name}" has no column marked as model id')
-        if not model_id.unique and not model_id.primary_key:
-            raise InitError(f'Model "{self.model.__blnt__.name}"\'s model id should be either '
-                            'a unique column or a primary key')
-        return model_id
+        self.primary: Union['core.models.Column', List['core.models.Column'], None] = None
+        self.model_id: Union['core.models.Column', List['core.models.Column'], None] = None
 
     def get_columns(self) -> Iterator[Tuple[str, 'core.models.Column']]:
         return self._get_attributes_of_type(self.parent, core.models.Column)
 
     def get_relationships(self) -> Iterator[Tuple[str, 'core.models.Relationship']]:
         return self._get_attributes_of_type(self.parent, core.models.Relationship)
```

### Comparing `Bolinette-0.8.5/bolinette/core/repository.py` & `Bolinette-0.9.0/bolinette/core/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,18 +73,19 @@
 
     async def _validate_model(self, values: Dict[str, Any]):
         api_errors = APIErrors()
         ignore_keys = []
         for _, relationship in self.model.__props__.get_relationships():
             key = relationship.name
             if key in values and values[key] is not None:
-                ignore_keys.append(relationship.foreign_key.name)
+                if relationship.foreign_key is not None:
+                    ignore_keys.append(relationship.foreign_key.name)
         for _, column in self.model.__props__.get_columns():
             key = column.name
-            if column.primary_key or key in ignore_keys:
+            if column.auto_increment or key in ignore_keys:
                 continue
             if key in values:
                 value = values.get(key)
                 if value is None and not column.nullable:
                     api_errors.append(ParamNonNullableError(key))
                 if column.unique:
                     if await self.get_first_by(column.name, value) is not None:
```

### Comparing `Bolinette-0.8.5/bolinette/core/service.py` & `Bolinette-0.9.0/bolinette/core/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Dict, Any
 
-from bolinette import blnt
+from bolinette import blnt, core
 from bolinette.blnt.objects import PaginationParams, OrderByParams
 from bolinette.exceptions import EntityNotFoundError
 from bolinette.utils.functions import async_invoke
 
 
 class Service:
     __blnt__: 'ServiceMetadata' = None
 
     def __init__(self, context: 'blnt.BolinetteContext'):
         self.__props__ = ServiceProps(self)
         self.context = context
-        self.repo = context.repo(self.__blnt__.model_name)
+        self.repo: core.Repository = context.repo(self.__blnt__.model_name)
 
     def __repr__(self):
         return f'<Service {self.__blnt__.name}>'
 
     async def get(self, identifier, *, safe=False):
         entity = await self.repo.get(identifier)
         if entity is None and not safe:
@@ -28,14 +28,22 @@
 
     async def get_first_by(self, key: str, value, *, safe=False):
         entity = await self.repo.get_first_by(key, value)
         if entity is None and not safe:
             raise EntityNotFoundError(model=self.__blnt__.name, key=key, value=value)
         return entity
 
+    async def get_first_by_keys(self, keys: Dict[str, Any], *, safe=False):
+        entity = await self.repo.query().filter_by(**keys).first()
+        if entity is None and not safe:
+            key = ','.join(keys.keys())
+            value = ','.join(keys.values())
+            raise EntityNotFoundError(model=self.__blnt__.name, key=key, value=value)
+        return entity
+
     async def get_all(self, *, pagination: PaginationParams = None, order_by: List[OrderByParams] = None):
         return await self.repo.get_all(pagination, order_by)
 
     async def create(self, values: Dict[str, Any], **kwargs):
         await self.__props__.call_mixin_methods('create', self, values=values, **kwargs)
         return await self.repo.create(values)
```

### Comparing `Bolinette-0.8.5/bolinette/decorators.py` & `Bolinette-0.9.0/bolinette/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         def decorator(arg):
             if isinstance(arg, _Command):
                 cmd = arg
             elif _inspect.isfunction(arg):
                 cmd = self._create_command(arg)
             else:
                 raise ValueError('@command must only decorate function or async functions')
-            cmd.name = name
+            cmd.path = name
             cmd.summary = summary
             blnt.cache.commands[cmd.name] = cmd
             return cmd
         return decorator
 
     def argument(self, arg_type: _typing.Literal['argument', 'option', 'flag', 'count'],
                  name: str, *, flag: str = None, summary: str = None,
```

### Comparing `Bolinette-0.8.5/bolinette/defaults/controllers/file.py` & `Bolinette-0.9.0/bolinette/defaults/controllers/file.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/controllers/static.py` & `Bolinette-0.9.0/bolinette/defaults/controllers/static.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/controllers/user.py` & `Bolinette-0.9.0/bolinette/defaults/controllers/user.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/middlewares/auth.py` & `Bolinette-0.9.0/bolinette/defaults/middlewares/auth.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/middlewares/internal.py` & `Bolinette-0.9.0/bolinette/defaults/middlewares/internal.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/mixins/historized.py` & `Bolinette-0.9.0/bolinette/defaults/mixins/historized.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/models/file.py` & `Bolinette-0.9.0/bolinette/defaults/models/file.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/models/role.py` & `Bolinette-0.9.0/bolinette/defaults/models/role.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/models/user.py` & `Bolinette-0.9.0/bolinette/defaults/models/user.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/services/file.py` & `Bolinette-0.9.0/bolinette/defaults/services/file.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/services/user.py` & `Bolinette-0.9.0/bolinette/defaults/services/user.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/topics/role.py` & `Bolinette-0.9.0/bolinette/defaults/topics/role.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/defaults/topics/user.py` & `Bolinette-0.9.0/bolinette/defaults/topics/user.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/docs.py` & `Bolinette-0.9.0/bolinette/docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         content = {
             'openapi': '3.0.0',
             'info': {
                 'title': self.context.manifest.get('name', 'Bolinette App'),
                 'description': self.context.manifest.get('desc', 'My web app built with the Bolinette framework'),
                 'version': self.context.manifest.get('version', '0.0.1')
             },
-            'servers': [{'url': 'http://localhost:5000'}],
+            'servers': [{'url': f'http://localhost:{self.context.env.get("port", 5000)}'}],
             'paths': self._build_routes(),
             'components': {
                 'schemas': self._build_schemas()
             }
         }
         files.write(self.swagger_path, yaml.safe_dump(content))
 
@@ -125,15 +125,16 @@
                         response['content'] = {'application/json': {'schema': ref}}
                 elif (match := self._response_type_regex.match(res_type)) is not None:
                     if mime := match.group(1):
                         response['content'] = {mime: {'schema': {'type': 'string'}}}
             if len(response) > 0:
                 docs['responses'][code] = response
 
-    def _build_ref(self, route: web.ControllerRoute, schema_type: Literal['response', 'payload']):
+    @staticmethod
+    def _build_ref(route: web.ControllerRoute, schema_type: Literal['response', 'payload']):
         returns = route.returns
         if returns:
             ref = {'$ref': f'#/components/schemas/{schema_type}.{returns.model}.{returns.key}'}
             if returns.as_list:
                 return {'type': 'array', 'items': ref}
             return ref
         return {}
@@ -151,25 +152,34 @@
 
     def _build_schemas(self):
         schemas = {}
         collections = {
             'payloads': self.context.mapper.payloads,
             'response': self.context.mapper.responses
         }
+        include_defs = {'payloads': False, 'response': True}
+        include_fks = {'payloads': True, 'response': False}
         for def_type, collection in collections.items():
+            inc_defs = include_defs[def_type]
+            inc_fks = include_fks[def_type]
             for model, key, definition in collection:
                 properties = {}
                 for field in definition.fields:
                     if isinstance(field, mapping.Field):
                         properties[field.name] = self._type_map[field.type]
                     elif isinstance(field, mapping.Definition):
-                        properties[field.name] = {
-                            '$ref': f'#/components/schemas/{def_type}.{field.model_name}.{field.model_key}'
-                        }
-                    elif isinstance(field, mapping.List):
+                        if inc_defs:
+                            properties[field.name] = {
+                                '$ref': f'#/components/schemas/{def_type}.{field.model_name}.{field.model_key}'
+                            }
+                        if inc_fks and isinstance(field, mapping.Reference):
+                            properties[field.foreign_key] = {
+                                'type': 'int'
+                            }
+                    elif isinstance(field, mapping.List) and inc_defs:
                         elem = field.element
                         if isinstance(elem, mapping.Definition):
                             properties[field.name] = {
                                 'type': 'array',
                                 'items': {
                                     '$ref': f'#/components/schemas/{def_type}.{elem.model_name}.{elem.model_key}'
                                 }
```

### Comparing `Bolinette-0.8.5/bolinette/exceptions.py` & `Bolinette-0.9.0/bolinette/exceptions.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/extensions.py` & `Bolinette-0.9.0/bolinette/extensions.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/init.py` & `Bolinette-0.9.0/bolinette/init.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,60 +9,99 @@
 from bolinette.utils import InitProxy
 
 
 @init_func(extension=Extensions.MODELS)
 async def init_model_classes(context: blnt.BolinetteContext):
     models = {}
     proxies = {}
+
+    # Instantiate models & process columns
     for model_name, model_cls in blnt.cache.models.items():
         db_key = model_cls.__blnt__.database
         if db_key not in context.db:
             raise InitError(f'Undefined "{db_key}" database for model "{model_name}"')
         model = model_cls(context.db[db_key])
+        # Instantiate columns
         for col_name, proxy in model.__props__.get_proxies(core.models.Column):
             col = proxy.instantiate(name=col_name, model=model)
             proxies[proxy] = col
             setattr(model, col_name, col)
+        # Add mixin columns
         for mixin_name in model.__blnt__.mixins:
             if mixin_name not in blnt.cache.mixins:
                 raise InitError(f'Model "{model_name}": mixin "{mixin_name}" is not defined')
             mixin = blnt.cache.mixins[mixin_name]()
             for col_name, proxy in mixin.columns().items():
                 col = proxy.instantiate(name=col_name, model=model)
                 setattr(model, col_name, col)
             model.__props__.mixins[mixin_name] = mixin
         models[model_name] = model
+
+    for _, model in models.items():
+        # Process auto generated primary keys
+        primary = [c for _, c in model.__props__.get_columns() if c.primary_key]
+        if not primary:
+            model.__props__.primary = None
+        elif len(primary) == 1:
+            if primary[0].auto_increment is None:
+                primary[0].auto_increment = True
+            model.__props__.primary = primary[0]
+        else:
+            model.__props__.primary = primary
+        for column in primary:
+            column.nullable = False
+        # Find model id
+        model_id = [c for _, c in model.__props__.get_columns() if c.model_id]
+        if not model_id:
+            model.__props__.model_id = model.__props__.primary
+        elif len(model_id) == 1:
+            model.__props__.model_id = model_id[0]
+        else:
+            model.__props__.model_id = model_id
+
+    # Process relationships
     for model_name, model in models.items():
+        # Instantiate relationships
         for rel_name, proxy in model.__props__.get_proxies(core.models.Relationship):
             rel = proxy.instantiate(name=rel_name, model=model, models=models)
             proxies[proxy] = rel
             setattr(model, rel_name, rel)
+        # Add mixin relationships
         for _, mixin in model.__props__.mixins.items():
             for rel_name, proxy in mixin.relationships(model).items():
                 rel = proxy.instantiate(name=rel_name, model=model, models=models)
                 setattr(model, rel_name, rel)
+
+    # Process references
     for model_name, model in models.items():
+        # Instantiate references
         for col_name, col in model.__props__.get_columns():
             if isinstance(col.reference, InitProxy) and col.reference.of_type(core.models.Reference):
                 col.reference = col.reference.instantiate(model=model, column=col, models=models)
+        # Process back references
         added_back_refs: Dict[core.Model, List[core.models.ColumnList]] = {}
         for rel_name, rel in model.__props__.get_relationships():
+            # Instantiate back references
             if isinstance(rel.backref, InitProxy) and rel.backref.of_type(core.models.Backref):
                 rel.backref = rel.backref.instantiate(model=model, relationship=rel)
                 if rel.backref.key not in added_back_refs:
                     added_back_refs[rel.target_model] = []
                 added_back_refs[rel.target_model].append(
                     core.models.ColumnList(rel.backref.key, rel.target_model, model))
+            # Link foreign keys
             if isinstance(rel.foreign_key, InitProxy) and rel.foreign_key.of_type(core.models.Column):
                 rel.foreign_key = proxies[rel.foreign_key]
+            # Link remote side foreign keys for same-model-references
             if isinstance(rel.remote_side, InitProxy) and rel.remote_side.of_type(core.models.Column):
                 rel.remote_side = proxies[rel.remote_side]
+        # Add back refs to the target model
         for target_model, back_refs in added_back_refs.items():
             for back_ref in back_refs:
                 setattr(target_model, back_ref.name, back_ref)
+
     for model_name, model in models.items():
         context.add_model(model_name, model)
 
 
 @init_func(extension=Extensions.MODELS)
 async def init_relational_models(context: blnt.BolinetteContext):
     models = {}
@@ -75,16 +114,18 @@
         orm_cols[model_name] = {}
         for att_name, attribute in model.__props__.get_columns():
             attribute.name = att_name
             ref = None
             if attribute.reference:
                 ref = sqlalchemy.ForeignKey(attribute.reference.target_path)
             orm_cols[model_name][att_name] = sqlalchemy.Column(
-                att_name, attribute.type.sqlalchemy_type, ref, default=attribute.default, index=attribute.model_id,
-                primary_key=attribute.primary_key, nullable=attribute.nullable, unique=attribute.unique)
+                att_name, attribute.type.sqlalchemy_type, ref,
+                default=attribute.default, index=attribute.model_id,
+                primary_key=attribute.primary_key, nullable=attribute.nullable,
+                unique=attribute.unique, autoincrement=attribute.auto_increment)
         orm_tables[model_name] = sqlalchemy.Table(model_name,
                                                   model.__props__.database.base.metadata,
                                                   *(orm_cols[model_name].values()))
 
     for model_name, model in models.items():
         orm_defs = {}
         for att_name, attribute in model.__props__.get_relationships():
```

### Comparing `Bolinette-0.8.5/bolinette/mail/providers/mailgun.py` & `Bolinette-0.9.0/bolinette/mail/providers/mailgun.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/mail/sender.py` & `Bolinette-0.9.0/bolinette/mail/sender.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/mapping/mapper.py` & `Bolinette-0.9.0/bolinette/mapping/mapper.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/mapping/objects.py` & `Bolinette-0.9.0/bolinette/mapping/objects.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/testing/client.py` & `Bolinette-0.9.0/bolinette/testing/client.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/testing/decorator.py` & `Bolinette-0.9.0/bolinette/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/testing/fixture.py` & `Bolinette-0.9.0/bolinette/testing/fixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 @pytest.fixture
 def client(loop):
     global bolinette_app
     if bolinette_app is None:
         bolinette_app = Bolinette(profile='test', overrides={
             'secret_key': ''.join(random.choices(string.ascii_letters + string.digits, k=32))
         })
-        bolinette_app.init()
+        bolinette_app.init_bolinette()
 
     async def create_client():
         return TestClient(bolinette_app, loop)
-    bolinette_app.init_extensions(force=True)
+    bolinette_app.init_extensions()
     return loop.run_until_complete(create_client())
```

### Comparing `Bolinette-0.8.5/bolinette/testing/mock.py` & `Bolinette-0.9.0/bolinette/testing/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import random
 import string
 from types import SimpleNamespace
 from typing import Dict, Any
 
-from bolinette import blnt, types
+from bolinette import blnt, types, core
 
 
 class Mocked:
     def __init__(self, name, context: 'blnt.BolinetteContext'):
         self.context = context
         self.name = name
         self.model = self.context.model(self.name)
@@ -84,18 +84,18 @@
         random_number_of_days = rng.randrange(days_between_dates)
         return start_date + datetime.timedelta(days=random_number_of_days)
 
     def __call__(self, m_id, model_name, *, post_mock_fn=None):
         self._id = m_id
         rng = random.Random(hash(f'{model_name}.{m_id}'))
         mocked = Mocked(model_name, self.context)
-        model = self.context.model(model_name)
+        model: core.Model = self.context.model(model_name)
         columns = model.__props__.get_columns()
         for _, column in columns:
-            if column.primary_key:
+            if column.auto_increment:
                 continue
             col_type = column.type
             if col_type == types.db.String:
                 mocked[column.name] = self._random_lower(rng, 15)
             if col_type == types.db.Email:
                 mocked[column.name] = f'{self._random_lower(rng, 10)}@{self._random_lower(rng, 5)}.com'
             if col_type == types.db.Password:
```

### Comparing `Bolinette-0.8.5/bolinette/types/db.py` & `Bolinette-0.9.0/bolinette/types/db.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/types/defs.py` & `Bolinette-0.9.0/bolinette/types/defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,21 @@
         return InitProxy(core.models.Reference, model_name=model_name, column_name=column_name)
 
 
 class Column:
     def __new__(cls, data_type: 'types.db.DataType', *,
                 reference: Optional['core.models.Reference'] = None,
                 primary_key: bool = False,
+                auto: Optional[bool] = None,
                 nullable: bool = True,
                 unique: bool = False,
                 model_id: bool = False,
                 default: Optional[Any] = None) -> InitProxy['core.models.Column']:
         return InitProxy(core.models.Column, data_type=data_type, reference=reference, primary_key=primary_key,
-                         nullable=nullable, unique=unique, model_id=model_id, default=default)
+                         auto=auto, nullable=nullable, unique=unique, model_id=model_id, default=default)
 
 
 class Backref:
     def __new__(cls, key: str, *, lazy: bool = True) -> InitProxy['core.models.Backref']:
         return InitProxy(core.models.Backref, key=key, lazy=lazy)
```

### Comparing `Bolinette-0.8.5/bolinette/utils/files.py` & `Bolinette-0.9.0/bolinette/utils/files.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/utils/functions.py` & `Bolinette-0.9.0/bolinette/utils/functions.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/utils/paths.py` & `Bolinette-0.9.0/bolinette/utils/paths.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/utils/serializing.py` & `Bolinette-0.9.0/bolinette/utils/serializing.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/web/controller.py` & `Bolinette-0.9.0/bolinette/web/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Callable, List, Dict, Any, Generator, Optional, Tuple
+import re
+from typing import Callable, List, Dict, Any, Generator, Optional, Tuple, Union
 
 from aiohttp.web_request import Request
 
 from bolinette import blnt, core, web
 from bolinette.exceptions import InitError
 from bolinette.utils import functions
 
@@ -174,116 +175,156 @@
         self.model = model
         self.key = key
         self.as_list = as_list
         self.skip_none = skip_none
 
 
 class ControllerDefaults:
+    PARAM_NAME_DOT_REGEX = re.compile(r'\.')
+    PARAM_NAME_CHAR_REGEX = re.compile(r'[^a-zA-Z0-9_]')
+
     def __init__(self, controller: Controller):
         self.controller = controller
         self.service: core.Service = controller.service
 
+    def _get_url_keys(self, key: Optional[Union[str, List[str]]], *, route: str) -> List[str]:
+        if key is None:
+            model_id = self.service.repo.model.__props__.model_id
+            if model_id is None:
+                raise InitError(f'Default route "{route}" for controller "{self.service.repo.model.__blnt__.name}" '
+                                f'must define a key or set model_id=True in one or more columns in the model')
+            if not isinstance(model_id, list):
+                model_id = [model_id]
+            key = [m.name for m in model_id]
+        if not isinstance(key, list):
+            key = [key]
+        return key
+
+    def _get_url(self, keys: List[str], *, prefix='') -> str:
+        return f'{prefix}/' + '/'.join([f'{{{self._translate_param_name(k)}}}' for k in keys])
+
+    def _get_match_params(self, keys: List[str], match: Dict[str, Any]) -> Dict[str, Any]:
+        return dict((keys[i], match.get(self._translate_param_name(keys[i]))) for i in range(len(keys)))
+
+    def _translate_param_name(self, param: str):
+        return self.PARAM_NAME_CHAR_REGEX.sub('', self.PARAM_NAME_DOT_REGEX.sub('_', param))
+
     def get_all(self, returns='default', *, prefix='',
                 middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+
         async def route(controller: web.Controller, **kwargs):
             resp = await functions.async_invoke(controller.service.get_all, **kwargs)
             return controller.response.ok(data=resp)
 
-        model_name = self.service.__blnt__.model_name
         docstring = docstring or f"""
         Gets all records from {model_name} collection
 
         -response 200 returns: The list of {model_name} entities
         """
         return ControllerRoute(self.controller, route, f'{prefix}', web.HttpMethod.GET, docstring,
                                returns=Returns(model_name, returns, as_list=True),
                                middlewares=middlewares)
 
-    def get_one(self, returns='default', *, key: str = None, prefix='',
-                middlewares: List[str] = None, docstring: str = None):
+    def get_one(self, returns='default', *, key: Union[str, List[str], None] = None,
+                prefix='', middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+        url_keys = self._get_url_keys(key, route='get_one')
+        url = self._get_url(url_keys, prefix=prefix)
+
         async def route(controller: web.Controller, *, match, **kwargs):
-            resp = await functions.async_invoke(controller.service.get_first_by, key, match.get(key), **kwargs)
+            keys = self._get_match_params(url_keys, match)
+            resp = await functions.async_invoke(controller.service.get_first_by_keys, keys, **kwargs)
             return controller.response.ok(data=resp)
 
-        model_name = self.service.__blnt__.model_name
-        key = key or self.service.repo.model.__props__.model_id.name
         docstring = docstring or f"""
         Gets one record from {model_name} collection, identified by {key} field
 
         -response 200 returns: The {model_name} entity
+        -response 404: The {model_name} identified by "{key}" was not found
         """
-        return ControllerRoute(self.controller, route, f'{prefix}/{{{key}}}', web.HttpMethod.GET, docstring,
+        return ControllerRoute(self.controller, route, url, web.HttpMethod.GET, docstring,
                                returns=Returns(model_name, returns),
                                middlewares=middlewares)
 
     def create(self, returns='default', expects='default', *, prefix='',
                middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+
         async def route(controller: web.Controller, payload, **kwargs):
             resp = await functions.async_invoke(controller.service.create, payload, **kwargs)
             return controller.response.created(messages=f'{controller.service.__blnt__.model_name}.created', data=resp)
 
-        model_name = self.service.__blnt__.model_name
         docstring = docstring or f"""
         Inserts a new entity in {model_name} collection
 
         -response 201 returns: The created {model_name} entity
         """
         return ControllerRoute(self.controller, route, f'{prefix}', web.HttpMethod.POST, docstring,
                                expects=Expects(self.service.__blnt__.model_name, expects),
                                returns=Returns(model_name, returns),
                                middlewares=middlewares)
 
     def update(self, returns='default', expects='default', *, key: str = None, prefix='',
                middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+        url_keys = self._get_url_keys(key, route='update')
+        url = self._get_url(url_keys, prefix=prefix)
+
         async def route(controller: web.Controller, payload, match, **kwargs):
-            entity = await controller.service.get_first_by(key, match.get(key))
+            keys = self._get_match_params(url_keys, match)
+            entity = await controller.service.get_first_by_keys(keys)
             resp = await functions.async_invoke(controller.service.update, entity, payload, **kwargs)
             return controller.response.ok(messages=f'{controller.service.__blnt__.model_name}.updated', data=resp)
 
-        model_name = self.service.__blnt__.model_name
-        key = key or self.service.repo.model.__props__.model_id.name
         docstring = docstring or f"""
         Updates all fields from one {model_name} entity, identified by {key} field
 
         -response 200 returns: The updated {model_name} entity
         """
-        return ControllerRoute(self.controller, route, f'{prefix}/{{{key}}}', web.HttpMethod.PUT, docstring,
+        return ControllerRoute(self.controller, route, url, web.HttpMethod.PUT, docstring,
                                expects=Expects(self.service.__blnt__.model_name, expects),
                                returns=Returns(model_name, returns),
                                middlewares=middlewares)
 
     def patch(self, returns='default', expects='default', *, key: str = None, prefix='',
               middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+        url_keys = self._get_url_keys(key, route='patch')
+        url = self._get_url(url_keys, prefix=prefix)
+
         async def route(controller: web.Controller, payload, match, **kwargs):
-            entity = await controller.service.get_first_by(key, match.get(key))
+            keys = self._get_match_params(url_keys, match)
+            entity = await controller.service.get_first_by_keys(keys)
             resp = await functions.async_invoke(controller.service.patch, entity, payload, **kwargs)
             return controller.response.ok(messages=f'{controller.service.__blnt__.model_name}.updated', data=resp)
 
-        model_name = self.service.__blnt__.model_name
-        key = key or self.service.repo.model.__props__.model_id.name
         docstring = docstring or f"""
         Updates some fields from one {model_name} entity, identified by {key} field
 
         -response 200 returns: The updated {model_name} entity
         """
-        return ControllerRoute(self.controller, route, f'{prefix}/{{{key}}}', web.HttpMethod.PATCH, docstring,
+        return ControllerRoute(self.controller, route, url, web.HttpMethod.PATCH, docstring,
                                expects=Expects(self.service.__blnt__.model_name, expects, patch=True),
                                returns=Returns(model_name, returns),
                                middlewares=middlewares)
 
     def delete(self, returns='default', *, key: str = None, prefix='',
                middlewares: List[str] = None, docstring: str = None):
+        model_name = self.service.__blnt__.model_name
+        url_keys = self._get_url_keys(key, route='delete')
+        url = self._get_url(url_keys, prefix=prefix)
+
         async def route(controller: web.Controller, match, **kwargs):
-            entity = await controller.service.get_first_by(key, match.get(key))
+            keys = self._get_match_params(url_keys, match)
+            entity = await controller.service.get_first_by_keys(keys)
             resp = await functions.async_invoke(controller.service.delete, entity, **kwargs)
             return controller.response.ok(messages=f'{controller.service.__blnt__.model_name}.deleted', data=resp)
 
-        model_name = self.service.__blnt__.model_name
-        key = key or self.service.repo.model.__props__.model_id.name
         docstring = docstring or f"""
         Deletes on record from {model_name} collection, identified by {key} field
 
         -response 200 returns: The deleted {model_name} entity
         """
-        return ControllerRoute(self.controller, route, f'{prefix}/{{{key}}}', web.HttpMethod.DELETE, docstring,
+        return ControllerRoute(self.controller, route, url, web.HttpMethod.DELETE, docstring,
                                returns=Returns(model_name, returns),
                                middlewares=middlewares)
```

### Comparing `Bolinette-0.8.5/bolinette/web/middleware.py` & `Bolinette-0.9.0/bolinette/web/middleware.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/web/resources.py` & `Bolinette-0.9.0/bolinette/web/resources.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/web/response.py` & `Bolinette-0.9.0/bolinette/web/response.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/web/sockets.py` & `Bolinette-0.9.0/bolinette/web/sockets.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/bolinette/web/topic.py` & `Bolinette-0.9.0/bolinette/web/topic.py`

 * *Files identical despite different names*

### Comparing `Bolinette-0.8.5/setup.py` & `Bolinette-0.9.0/setup.py`

 * *Files identical despite different names*

