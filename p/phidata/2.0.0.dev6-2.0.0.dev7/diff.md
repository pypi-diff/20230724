# Comparing `tmp/phidata-2.0.0.dev6.tar.gz` & `tmp/phidata-2.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.0.0.dev6.tar", last modified: Tue Jul 18 15:16:25 2023, max compression
+gzip compressed data, was "phidata-2.0.0.dev7.tar", last modified: Mon Jul 24 14:18:58 2023, max compression
```

## Comparing `phidata-2.0.0.dev6.tar` & `phidata-2.0.0.dev7.tar`

### file list

```diff
@@ -1,751 +1,755 @@
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.848658 phidata-2.0.0.dev6/
--rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev6/LICENSE
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-18 15:16:25.848469 phidata-2.0.0.dev6/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev6/README.md
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.714363 phidata-2.0.0.dev6/phi/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.715512 phidata-2.0.0.dev6/phi/api/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1684 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/client.py
--rw-r--r--   0 zu         (501) staff       (20)      843 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)      794 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/routes.py
--rw-r--r--   0 zu         (501) staff       (20)     4464 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/user.py
--rw-r--r--   0 zu         (501) staff       (20)     7188 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/api/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.715778 phidata-2.0.0.dev6/phi/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.716314 phidata-2.0.0.dev6/phi/aws/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.716585 phidata-2.0.0.dev6/phi/aws/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.716852 phidata-2.0.0.dev6/phi/aws/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.717099 phidata-2.0.0.dev6/phi/aws/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.717360 phidata-2.0.0.dev6/phi/aws/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.718544 phidata-2.0.0.dev6/phi/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.719021 phidata-2.0.0.dev6/phi/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.719460 phidata-2.0.0.dev6/phi/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.720522 phidata-2.0.0.dev6/phi/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.721391 phidata-2.0.0.dev6/phi/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.722612 phidata-2.0.0.dev6/phi/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.723090 phidata-2.0.0.dev6/phi/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.723853 phidata-2.0.0.dev6/phi/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.724152 phidata-2.0.0.dev6/phi/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.724421 phidata-2.0.0.dev6/phi/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.724818 phidata-2.0.0.dev6/phi/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.725673 phidata-2.0.0.dev6/phi/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.726031 phidata-2.0.0.dev6/phi/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.726514 phidata-2.0.0.dev6/phi/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.728261 phidata-2.0.0.dev6/phi/cli/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3667 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/auth_server.py
--rw-r--r--   0 zu         (501) staff       (20)    13385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/config.py
--rw-r--r--   0 zu         (501) staff       (20)     3316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/console.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/credentials.py
--rw-r--r--   0 zu         (501) staff       (20)    20599 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/entrypoint.py
--rw-r--r--   0 zu         (501) staff       (20)    15893 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.728561 phidata-2.0.0.dev6/phi/cli/ws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/ws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/cli/ws/ws_cli.py
--rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.728867 phidata-2.0.0.dev6/phi/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.729498 phidata-2.0.0.dev6/phi/docker/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.729887 phidata-2.0.0.dev6/phi/docker/app/django/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/django/django.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.730260 phidata-2.0.0.dev6/phi/docker/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.730589 phidata-2.0.0.dev6/phi/docker/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.731295 phidata-2.0.0.dev6/phi/docker/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 zu         (501) staff       (20)     4740 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.731603 phidata-2.0.0.dev6/phi/docker/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.731902 phidata-2.0.0.dev6/phi/docker/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.733073 phidata-2.0.0.dev6/phi/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.733374 phidata-2.0.0.dev6/phi/document/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/document/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/document/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.733735 phidata-2.0.0.dev6/phi/document/reader/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/document/reader/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/document/reader/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/document/reader/pdf.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.734222 phidata-2.0.0.dev6/phi/embedder/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/embedder/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/embedder/base.py
--rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/embedder/openai.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.734497 phidata-2.0.0.dev6/phi/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.736967 phidata-2.0.0.dev6/phi/infra/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/app/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1253 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/app/db_app.py
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/enums.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.737431 phidata-2.0.0.dev6/phi/infra/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/infra/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.737583 phidata-2.0.0.dev6/phi/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/k8s/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.737889 phidata-2.0.0.dev6/phi/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/llm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.738298 phidata-2.0.0.dev6/phi/llm/conversation/
--rw-r--r--   0 zu         (501) staff       (20)      108 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/llm/conversation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10430 2023-07-18 15:14:48.000000 phidata-2.0.0.dev6/phi/llm/conversation/conversation.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/conversation/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.739321 phidata-2.0.0.dev6/phi/llm/conversation/storage/
--rw-r--r--   0 zu         (501) staff       (20)       66 2023-07-16 11:59:13.000000 phidata-2.0.0.dev6/phi/llm/conversation/storage/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      899 2023-07-18 10:39:15.000000 phidata-2.0.0.dev6/phi/llm/conversation/storage/base.py
--rw-r--r--   0 zu         (501) staff       (20)     5845 2023-07-18 12:22:33.000000 phidata-2.0.0.dev6/phi/llm/conversation/storage/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.739887 phidata-2.0.0.dev6/phi/llm/knowledge/
--rw-r--r--   0 zu         (501) staff       (20)       49 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/knowledge/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      646 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/knowledge/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2515 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/knowledge/pdf.py
--rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/llm/openai.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.742803 phidata-2.0.0.dev6/phi/schemas/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/schemas/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      208 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/schemas/response.py
--rw-r--r--   0 zu         (501) staff       (20)     1484 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/schemas/user.py
--rw-r--r--   0 zu         (501) staff       (20)      677 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/schemas/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.742997 phidata-2.0.0.dev6/phi/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.743291 phidata-2.0.0.dev6/phi/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/table/sql/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.748259 phidata-2.0.0.dev6/phi/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/defaults.py
--rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/git.py
--rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/load_env.py
--rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/pickle.py
--rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/py_io.py
--rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/pyproject.py
--rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/resource_filter.py
--rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.748540 phidata-2.0.0.dev6/phi/vectordb/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/vectordb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/vectordb/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.748820 phidata-2.0.0.dev6/phi/vectordb/pgvector/
--rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev6/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5536 2023-07-18 15:15:54.000000 phidata-2.0.0.dev6/phi/vectordb/pgvector/pgvector.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.749844 phidata-2.0.0.dev6/phi/workspace/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9927 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)    20826 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev6/phi/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.750483 phidata-2.0.0.dev6/phidata/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.751937 phidata-2.0.0.dev6/phidata/airflow/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev6/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.752363 phidata-2.0.0.dev6/phidata/airflow/operators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/airflow/operators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.754696 phidata-2.0.0.dev6/phidata/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev6/phidata/app/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.757196 phidata-2.0.0.dev6/phidata/app/airflow/
--rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev6/phidata/app/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.757608 phidata-2.0.0.dev6/phidata/app/alertmanager/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.758600 phidata-2.0.0.dev6/phidata/app/amundsen/
--rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev6/phidata/app/amundsen/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/amundsen/frontend.py
--rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/amundsen/metadata.py
--rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/amundsen/search.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.759066 phidata-2.0.0.dev6/phidata/app/assistant/
--rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev6/phidata/app/assistant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/assistant/assistant.py
--rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/aws_app.py
--rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/base_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.759501 phidata-2.0.0.dev6/phidata/app/cadvisor/
--rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.760163 phidata-2.0.0.dev6/phidata/app/databox/
--rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev6/phidata/app/databox/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/databox/databox.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.761202 phidata-2.0.0.dev6/phidata/app/db/
--rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev6/phidata/app/db/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev6/phidata/app/db/base_db.py
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev6/phidata/app/db/db_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.761734 phidata-2.0.0.dev6/phidata/app/django/
--rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev6/phidata/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/django/django_app.py
--rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/django/django_backup.py
--rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/docker_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.762278 phidata-2.0.0.dev6/phidata/app/elastic/
--rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/app/elastic/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.762667 phidata-2.0.0.dev6/phidata/app/elasticsearch/
--rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.763327 phidata-2.0.0.dev6/phidata/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.763846 phidata-2.0.0.dev6/phidata/app/grafana/
--rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/grafana/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/grafana/grafana.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.765044 phidata-2.0.0.dev6/phidata/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.765846 phidata-2.0.0.dev6/phidata/app/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev6/phidata/app/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/k8s/app.py
--rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/k8s/dir.py
--rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/k8s/url.py
--rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/k8s_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.766200 phidata-2.0.0.dev6/phidata/app/mysql/
--rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev6/phidata/app/mysql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.766549 phidata-2.0.0.dev6/phidata/app/neo4j/
--rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/neo4j/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.766932 phidata-2.0.0.dev6/phidata/app/nodeexporter/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/phidata_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.767462 phidata-2.0.0.dev6/phidata/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev6/phidata/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.767925 phidata-2.0.0.dev6/phidata/app/prometheus/
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev6/phidata/app/prometheus/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.768363 phidata-2.0.0.dev6/phidata/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.768997 phidata-2.0.0.dev6/phidata/app/redis/
--rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev6/phidata/app/redis/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/redis/redis.py
--rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/redis/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.770279 phidata-2.0.0.dev6/phidata/app/server/
--rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev6/phidata/app/server/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/server/api_server.py
--rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/server/server_base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.771793 phidata-2.0.0.dev6/phidata/app/spark/
--rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev6/phidata/app/spark/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/spark/spark_base.py
--rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/spark/spark_driver.py
--rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.772421 phidata-2.0.0.dev6/phidata/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev6/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.775281 phidata-2.0.0.dev6/phidata/app/superset/
--rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev6/phidata/app/superset/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/superset/superset_base.py
--rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/superset/superset_init.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/superset/superset_worker.py
--rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.776770 phidata-2.0.0.dev6/phidata/app/traefik/
--rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev6/phidata/app/traefik/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/traefik/crds.py
--rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/app/traefik/router.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.777198 phidata-2.0.0.dev6/phidata/asset/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/asset/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.777562 phidata-2.0.0.dev6/phidata/asset/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/asset/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/asset/data_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.778406 phidata-2.0.0.dev6/phidata/asset/local/
--rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/asset/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/asset/local/file.py
--rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.780303 phidata-2.0.0.dev6/phidata/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev6/phidata/aws/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/aws/args.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.780758 phidata-2.0.0.dev6/phidata/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev6/phidata/aws/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/aws/config.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.781038 phidata-2.0.0.dev6/phidata/aws/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.781460 phidata-2.0.0.dev6/phidata/aws/create/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev6/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev6/phidata/aws/create/iam/role.py
--rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/driver.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.781834 phidata-2.0.0.dev6/phidata/aws/enums/
--rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.782671 phidata-2.0.0.dev6/phidata/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.782966 phidata-2.0.0.dev6/phidata/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.783271 phidata-2.0.0.dev6/phidata/aws/resource/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.783558 phidata-2.0.0.dev6/phidata/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.784155 phidata-2.0.0.dev6/phidata/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.786438 phidata-2.0.0.dev6/phidata/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.787999 phidata-2.0.0.dev6/phidata/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.788537 phidata-2.0.0.dev6/phidata/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.789406 phidata-2.0.0.dev6/phidata/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev6/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.789662 phidata-2.0.0.dev6/phidata/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.790443 phidata-2.0.0.dev6/phidata/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev6/phidata/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.791317 phidata-2.0.0.dev6/phidata/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/iam/group.py
--rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.792066 phidata-2.0.0.dev6/phidata/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.792336 phidata-2.0.0.dev6/phidata/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.792788 phidata-2.0.0.dev6/phidata/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev6/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.793626 phidata-2.0.0.dev6/phidata/aws/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/aws/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/s3/dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/s3/object.py
--rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/aws/worker.py
--rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.794157 phidata-2.0.0.dev6/phidata/checks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/checks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev6/phidata/checks/check.py
--rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev6/phidata/checks/not_empty.py
--rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev6/phidata/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.794906 phidata-2.0.0.dev6/phidata/decorators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/decorators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/decorators/timer.py
--rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/decorators/validate_env.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.797168 phidata-2.0.0.dev6/phidata/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/args.py
--rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/config.py
--rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/enums.py
--rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.798566 phidata-2.0.0.dev6/phidata/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev6/phidata/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/resource/utils.py
--rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.798799 phidata-2.0.0.dev6/phidata/docker/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/docker/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/utils/container.py
--rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/docker/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.799778 phidata-2.0.0.dev6/phidata/exceptions/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev6/phidata/exceptions/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev6/phidata/exceptions/app.py
--rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev6/phidata/exceptions/task.py
--rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev6/phidata/exceptions/workflow.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.800984 phidata-2.0.0.dev6/phidata/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/infra/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/infra/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev6/phidata/infra/args.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/infra/config.py
--rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/infra/resource.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.802555 phidata-2.0.0.dev6/phidata/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/k8s/args.py
--rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/config.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.803378 phidata-2.0.0.dev6/phidata/k8s/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.803632 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.804252 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.804466 phidata-2.0.0.dev6/phidata/k8s/create/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.805044 phidata-2.0.0.dev6/phidata/k8s/create/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev6/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.805657 phidata-2.0.0.dev6/phidata/k8s/create/common/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/common/labels.py
--rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.805866 phidata-2.0.0.dev6/phidata/k8s/create/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.807916 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.808168 phidata-2.0.0.dev6/phidata/k8s/create/crb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/group.py
--rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.808413 phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.808612 phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.808903 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.809274 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.809423 phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.809600 phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.811423 phidata-2.0.0.dev6/phidata/k8s/enums/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/api_group.py
--rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev6/phidata/k8s/enums/api_version.py
--rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev6/phidata/k8s/enums/kind.py
--rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/protocol.py
--rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/pv.py
--rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/service_type.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.812528 phidata-2.0.0.dev6/phidata/k8s/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.812718 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.813142 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.813401 phidata-2.0.0.dev6/phidata/k8s/resource/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.819985 phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.820275 phidata-2.0.0.dev6/phidata/k8s/resource/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.825851 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev6/phidata/k8s/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.826180 phidata-2.0.0.dev6/phidata/k8s/resource/meta/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.826776 phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.827021 phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.827291 phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.827478 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.828091 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.828238 phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.828439 phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.828812 phidata-2.0.0.dev6/phidata/k8s/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/k8s/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/utils/pod.py
--rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/k8s/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.828963 phidata-2.0.0.dev6/phidata/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/llm/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.830173 phidata-2.0.0.dev6/phidata/llm/duckdb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/agent.py
--rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/chain.py
--rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/connection.py
--rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/loader.py
--rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/query.py
--rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.830665 phidata-2.0.0.dev6/phidata/product/
--rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev6/phidata/product/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/product/data_product.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.831012 phidata-2.0.0.dev6/phidata/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.831299 phidata-2.0.0.dev6/phidata/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.832183 phidata-2.0.0.dev6/phidata/table/local/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/table/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/local/csv.py
--rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/local/local_table.py
--rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/local/parquet.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.832865 phidata-2.0.0.dev6/phidata/table/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/table/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/s3/csv.py
--rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/s3/parquet.py
--rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.833479 phidata-2.0.0.dev6/phidata/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev6/phidata/table/sql/postgres.py
--rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.835131 phidata-2.0.0.dev6/phidata/task/
--rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/task/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.835413 phidata-2.0.0.dev6/phidata/task/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/aws/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.835841 phidata-2.0.0.dev6/phidata/task/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.836393 phidata-2.0.0.dev6/phidata/task/aws/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.836778 phidata-2.0.0.dev6/phidata/task/aws/glue/
--rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.836923 phidata-2.0.0.dev6/phidata/task/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/dev/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.837045 phidata-2.0.0.dev6/phidata/task/download/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/download/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.837461 phidata-2.0.0.dev6/phidata/task/download/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/download/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.838696 phidata-2.0.0.dev6/phidata/task/download/url/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/download/url/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/task/download/url/to_file.py
--rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/task/download/url/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.838896 phidata-2.0.0.dev6/phidata/task/plot/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/plot/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.839272 phidata-2.0.0.dev6/phidata/task/plot/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/plot/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/task/python_task.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.839788 phidata-2.0.0.dev6/phidata/task/run/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/run/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.840099 phidata-2.0.0.dev6/phidata/task/run/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/run/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev6/phidata/task/run/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/task/task.py
--rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev6/phidata/task/task_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.840400 phidata-2.0.0.dev6/phidata/task/upload/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/upload/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.840770 phidata-2.0.0.dev6/phidata/task/upload/file/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/task/upload/file/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.841660 phidata-2.0.0.dev6/phidata/types/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/types/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/types/airflow.py
--rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/types/context.py
--rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/types/phidata_runtime.py
--rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev6/phidata/types/run_status.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.845449 phidata-2.0.0.dev6/phidata/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/cli_console.py
--rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev6/phidata/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev6/phidata/utils/compare.py
--rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev6/phidata/utils/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev6/phidata/utils/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/env_file.py
--rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev6/phidata/utils/env_var.py
--rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/utils/k8s.py
--rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev6/phidata/utils/print_table.py
--rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/utils/workspace_path.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.846752 phidata-2.0.0.dev6/phidata/workflow/
--rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev6/phidata/workflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev6/phidata/workflow/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.847099 phidata-2.0.0.dev6/phidata/workflow/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev6/phidata/workflow/dev/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/workflow/workflow.py
--rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev6/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.847756 phidata-2.0.0.dev6/phidata/workspace/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev6/phidata/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev6/phidata/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev6/phidata/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.751649 phidata-2.0.0.dev6/phidata.egg-info/
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)    18749 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/entry_points.txt
--rw-r--r--   0 zu         (501) staff       (20)      179 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/requires.txt
--rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-18 15:16:25.000000 phidata-2.0.0.dev6/phidata.egg-info/top_level.txt
--rw-r--r--   0 zu         (501) staff       (20)     1629 2023-07-18 15:14:42.000000 phidata-2.0.0.dev6/pyproject.toml
--rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-18 15:16:25.848719 phidata-2.0.0.dev6/setup.cfg
--rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev6/setup.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-18 15:16:25.848080 phidata-2.0.0.dev6/tests/
--rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev6/tests/test_placeholder.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.928250 phidata-2.0.0.dev7/
+-rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev7/LICENSE
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 14:18:58.928084 phidata-2.0.0.dev7/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev7/README.md
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.749858 phidata-2.0.0.dev7/phi/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.751591 phidata-2.0.0.dev7/phi/api/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/api/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1543 2023-07-22 20:26:57.000000 phidata-2.0.0.dev7/phi/api/client.py
+-rw-r--r--   0 zu         (501) staff       (20)      815 2023-07-21 16:44:29.000000 phidata-2.0.0.dev7/phi/api/routes.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.752534 phidata-2.0.0.dev7/phi/api/schemas/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/api/schemas/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      131 2023-07-21 11:59:13.000000 phidata-2.0.0.dev7/phi/api/schemas/response.py
+-rw-r--r--   0 zu         (501) staff       (20)      490 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/api/schemas/user.py
+-rw-r--r--   0 zu         (501) staff       (20)      442 2023-07-22 19:50:20.000000 phidata-2.0.0.dev7/phi/api/schemas/workspace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3514 2023-07-22 17:30:21.000000 phidata-2.0.0.dev7/phi/api/user.py
+-rw-r--r--   0 zu         (501) staff       (20)     5735 2023-07-22 21:39:50.000000 phidata-2.0.0.dev7/phi/api/workspace.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.752898 phidata-2.0.0.dev7/phi/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.753625 phidata-2.0.0.dev7/phi/aws/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.753960 phidata-2.0.0.dev7/phi/aws/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.754321 phidata-2.0.0.dev7/phi/aws/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.754685 phidata-2.0.0.dev7/phi/aws/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.755022 phidata-2.0.0.dev7/phi/aws/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.756398 phidata-2.0.0.dev7/phi/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.756741 phidata-2.0.0.dev7/phi/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.757000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.757811 phidata-2.0.0.dev7/phi/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.759041 phidata-2.0.0.dev7/phi/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.760324 phidata-2.0.0.dev7/phi/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.760869 phidata-2.0.0.dev7/phi/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.761734 phidata-2.0.0.dev7/phi/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762087 phidata-2.0.0.dev7/phi/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762374 phidata-2.0.0.dev7/phi/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762925 phidata-2.0.0.dev7/phi/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.763668 phidata-2.0.0.dev7/phi/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.763989 phidata-2.0.0.dev7/phi/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.764470 phidata-2.0.0.dev7/phi/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.766441 phidata-2.0.0.dev7/phi/cli/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3659 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/cli/auth_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    13299 2023-07-22 20:21:48.000000 phidata-2.0.0.dev7/phi/cli/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     2907 2023-07-22 21:44:58.000000 phidata-2.0.0.dev7/phi/cli/console.py
+-rw-r--r--   0 zu         (501) staff       (20)      804 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/cli/credentials.py
+-rw-r--r--   0 zu         (501) staff       (20)    20376 2023-07-22 21:47:11.000000 phidata-2.0.0.dev7/phi/cli/entrypoint.py
+-rw-r--r--   0 zu         (501) staff       (20)    15872 2023-07-22 17:24:33.000000 phidata-2.0.0.dev7/phi/cli/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.766793 phidata-2.0.0.dev7/phi/cli/ws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/ws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27460 2023-07-22 20:35:52.000000 phidata-2.0.0.dev7/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.767325 phidata-2.0.0.dev7/phi/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768128 phidata-2.0.0.dev7/phi/docker/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768540 phidata-2.0.0.dev7/phi/docker/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/django/django.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768928 phidata-2.0.0.dev7/phi/docker/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.769365 phidata-2.0.0.dev7/phi/docker/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770054 phidata-2.0.0.dev7/phi/docker/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 zu         (501) staff       (20)     4732 2023-07-24 12:43:04.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770431 phidata-2.0.0.dev7/phi/docker/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770781 phidata-2.0.0.dev7/phi/docker/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.778637 phidata-2.0.0.dev7/phi/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.779030 phidata-2.0.0.dev7/phi/document/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/document/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.800444 phidata-2.0.0.dev7/phi/document/reader/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/document/reader/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/reader/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/reader/pdf.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.801808 phidata-2.0.0.dev7/phi/embedder/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/embedder/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/embedder/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/embedder/openai.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.802086 phidata-2.0.0.dev7/phi/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.802829 phidata-2.0.0.dev7/phi/infra/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1778 2023-07-23 12:14:29.000000 phidata-2.0.0.dev7/phi/infra/app/db_app.py
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/enums.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.803390 phidata-2.0.0.dev7/phi/infra/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.803571 phidata-2.0.0.dev7/phi/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/k8s/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.804113 phidata-2.0.0.dev7/phi/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/llm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/llm/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.804667 phidata-2.0.0.dev7/phi/llm/conversation/
+-rw-r--r--   0 zu         (501) staff       (20)       85 2023-07-23 19:28:29.000000 phidata-2.0.0.dev7/phi/llm/conversation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11301 2023-07-24 14:14:56.000000 phidata-2.0.0.dev7/phi/llm/conversation/conversation.py
+-rw-r--r--   0 zu         (501) staff       (20)     1293 2023-07-24 14:04:35.000000 phidata-2.0.0.dev7/phi/llm/conversation/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.805191 phidata-2.0.0.dev7/phi/llm/history/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:47:16.000000 phidata-2.0.0.dev7/phi/llm/history/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1636 2023-07-24 13:53:07.000000 phidata-2.0.0.dev7/phi/llm/history/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1027 2023-07-24 11:31:02.000000 phidata-2.0.0.dev7/phi/llm/history/simple.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.805783 phidata-2.0.0.dev7/phi/llm/knowledge/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-23 16:38:05.000000 phidata-2.0.0.dev7/phi/llm/knowledge/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      714 2023-07-24 11:47:28.000000 phidata-2.0.0.dev7/phi/llm/knowledge/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2382 2023-07-24 13:11:31.000000 phidata-2.0.0.dev7/phi/llm/knowledge/pdf.py
+-rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/llm/openai.py
+-rw-r--r--   0 zu         (501) staff       (20)     1030 2023-07-24 11:43:07.000000 phidata-2.0.0.dev7/phi/llm/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806437 phidata-2.0.0.dev7/phi/llm/storage/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:37:22.000000 phidata-2.0.0.dev7/phi/llm/storage/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      789 2023-07-24 11:25:53.000000 phidata-2.0.0.dev7/phi/llm/storage/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7675 2023-07-24 14:12:29.000000 phidata-2.0.0.dev7/phi/llm/storage/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806717 phidata-2.0.0.dev7/phi/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806998 phidata-2.0.0.dev7/phi/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/sql/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.809325 phidata-2.0.0.dev7/phi/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/defaults.py
+-rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/git.py
+-rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/load_env.py
+-rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/pickle.py
+-rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/py_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/pyproject.py
+-rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/resource_filter.py
+-rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.809680 phidata-2.0.0.dev7/phi/vectordb/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.810147 phidata-2.0.0.dev7/phi/vectordb/pgvector/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5592 2023-07-24 10:26:29.000000 phidata-2.0.0.dev7/phi/vectordb/pgvector/pgvector.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.811722 phidata-2.0.0.dev7/phi/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9931 2023-07-21 11:56:44.000000 phidata-2.0.0.dev7/phi/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/helpers.py
+-rw-r--r--   0 zu         (501) staff       (20)    25401 2023-07-22 21:51:25.000000 phidata-2.0.0.dev7/phi/workspace/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.812310 phidata-2.0.0.dev7/phidata/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.813702 phidata-2.0.0.dev7/phidata/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev7/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.814412 phidata-2.0.0.dev7/phidata/airflow/operators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.817301 phidata-2.0.0.dev7/phidata/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev7/phidata/app/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.819907 phidata-2.0.0.dev7/phidata/app/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev7/phidata/app/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.820383 phidata-2.0.0.dev7/phidata/app/alertmanager/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.821401 phidata-2.0.0.dev7/phidata/app/amundsen/
+-rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev7/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/search.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.821865 phidata-2.0.0.dev7/phidata/app/assistant/
+-rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev7/phidata/app/assistant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/assistant/assistant.py
+-rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/aws_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/base_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.822342 phidata-2.0.0.dev7/phidata/app/cadvisor/
+-rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.823228 phidata-2.0.0.dev7/phidata/app/databox/
+-rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev7/phidata/app/databox/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/databox/databox.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.824275 phidata-2.0.0.dev7/phidata/app/db/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev7/phidata/app/db/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev7/phidata/app/db/base_db.py
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev7/phidata/app/db/db_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.825044 phidata-2.0.0.dev7/phidata/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev7/phidata/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/django/django_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/django/django_backup.py
+-rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/docker_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.825729 phidata-2.0.0.dev7/phidata/app/elastic/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/app/elastic/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.826207 phidata-2.0.0.dev7/phidata/app/elasticsearch/
+-rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.826900 phidata-2.0.0.dev7/phidata/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.827482 phidata-2.0.0.dev7/phidata/app/grafana/
+-rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/grafana/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/grafana/grafana.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.828704 phidata-2.0.0.dev7/phidata/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.829547 phidata-2.0.0.dev7/phidata/app/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev7/phidata/app/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/app.py
+-rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/dir.py
+-rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/url.py
+-rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.830189 phidata-2.0.0.dev7/phidata/app/mysql/
+-rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev7/phidata/app/mysql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.830747 phidata-2.0.0.dev7/phidata/app/neo4j/
+-rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.831201 phidata-2.0.0.dev7/phidata/app/nodeexporter/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/phidata_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.831817 phidata-2.0.0.dev7/phidata/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev7/phidata/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.832414 phidata-2.0.0.dev7/phidata/app/prometheus/
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.832973 phidata-2.0.0.dev7/phidata/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.833611 phidata-2.0.0.dev7/phidata/app/redis/
+-rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev7/phidata/app/redis/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/redis/redis.py
+-rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/redis/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.834666 phidata-2.0.0.dev7/phidata/app/server/
+-rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev7/phidata/app/server/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/server/api_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/server/server_base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.836293 phidata-2.0.0.dev7/phidata/app/spark/
+-rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev7/phidata/app/spark/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.836826 phidata-2.0.0.dev7/phidata/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.839705 phidata-2.0.0.dev7/phidata/app/superset/
+-rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev7/phidata/app/superset/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_init.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.863699 phidata-2.0.0.dev7/phidata/app/traefik/
+-rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev7/phidata/app/traefik/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/crds.py
+-rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/router.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.864133 phidata-2.0.0.dev7/phidata/asset/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.864474 phidata-2.0.0.dev7/phidata/asset/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/asset/data_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.865227 phidata-2.0.0.dev7/phidata/asset/local/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/asset/local/file.py
+-rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867055 phidata-2.0.0.dev7/phidata/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/aws/args.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867506 phidata-2.0.0.dev7/phidata/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/aws/config.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867761 phidata-2.0.0.dev7/phidata/aws/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.868224 phidata-2.0.0.dev7/phidata/aws/create/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/role.py
+-rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/driver.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.868850 phidata-2.0.0.dev7/phidata/aws/enums/
+-rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.869743 phidata-2.0.0.dev7/phidata/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870040 phidata-2.0.0.dev7/phidata/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870367 phidata-2.0.0.dev7/phidata/aws/resource/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870740 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.871500 phidata-2.0.0.dev7/phidata/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.873047 phidata-2.0.0.dev7/phidata/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.874406 phidata-2.0.0.dev7/phidata/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.874948 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.875612 phidata-2.0.0.dev7/phidata/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.875898 phidata-2.0.0.dev7/phidata/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.876253 phidata-2.0.0.dev7/phidata/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877026 phidata-2.0.0.dev7/phidata/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877734 phidata-2.0.0.dev7/phidata/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877982 phidata-2.0.0.dev7/phidata/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.878498 phidata-2.0.0.dev7/phidata/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.879367 phidata-2.0.0.dev7/phidata/aws/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/object.py
+-rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/worker.py
+-rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.880003 phidata-2.0.0.dev7/phidata/checks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/checks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev7/phidata/checks/check.py
+-rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev7/phidata/checks/not_empty.py
+-rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev7/phidata/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.880728 phidata-2.0.0.dev7/phidata/decorators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/decorators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/decorators/timer.py
+-rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/decorators/validate_env.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.882772 phidata-2.0.0.dev7/phidata/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.884527 phidata-2.0.0.dev7/phidata/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/utils.py
+-rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.884804 phidata-2.0.0.dev7/phidata/docker/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/utils/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.885904 phidata-2.0.0.dev7/phidata/exceptions/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/exceptions/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev7/phidata/exceptions/app.py
+-rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/exceptions/task.py
+-rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/exceptions/workflow.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.887292 phidata-2.0.0.dev7/phidata/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/infra/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/infra/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev7/phidata/infra/args.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/infra/config.py
+-rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/infra/resource.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.888973 phidata-2.0.0.dev7/phidata/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/k8s/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.889858 phidata-2.0.0.dev7/phidata/k8s/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890122 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890583 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890888 phidata-2.0.0.dev7/phidata/k8s/create/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891163 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891809 phidata-2.0.0.dev7/phidata/k8s/create/common/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891973 phidata-2.0.0.dev7/phidata/k8s/create/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.893573 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.893938 phidata-2.0.0.dev7/phidata/k8s/create/crb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894228 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894484 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894783 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895198 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895505 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895754 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.898205 phidata-2.0.0.dev7/phidata/k8s/enums/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev7/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev7/phidata/k8s/enums/kind.py
+-rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/pv.py
+-rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899341 phidata-2.0.0.dev7/phidata/k8s/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899527 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899957 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900226 phidata-2.0.0.dev7/phidata/k8s/resource/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900762 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900951 phidata-2.0.0.dev7/phidata/k8s/resource/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.905240 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/k8s/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.905833 phidata-2.0.0.dev7/phidata/k8s/resource/meta/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906372 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906639 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906907 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907125 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907670 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907863 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908092 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908505 phidata-2.0.0.dev7/phidata/k8s/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/utils/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908679 phidata-2.0.0.dev7/phidata/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.910141 phidata-2.0.0.dev7/phidata/llm/duckdb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.910975 phidata-2.0.0.dev7/phidata/product/
+-rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev7/phidata/product/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/product/data_product.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.911353 phidata-2.0.0.dev7/phidata/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.911607 phidata-2.0.0.dev7/phidata/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.912230 phidata-2.0.0.dev7/phidata/table/local/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/local_table.py
+-rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/parquet.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.912963 phidata-2.0.0.dev7/phidata/table/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/parquet.py
+-rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.913937 phidata-2.0.0.dev7/phidata/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev7/phidata/table/sql/postgres.py
+-rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.915832 phidata-2.0.0.dev7/phidata/task/
+-rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916106 phidata-2.0.0.dev7/phidata/task/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916577 phidata-2.0.0.dev7/phidata/task/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916979 phidata-2.0.0.dev7/phidata/task/aws/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917357 phidata-2.0.0.dev7/phidata/task/aws/glue/
+-rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917579 phidata-2.0.0.dev7/phidata/task/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/dev/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917688 phidata-2.0.0.dev7/phidata/task/download/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917884 phidata-2.0.0.dev7/phidata/task/download/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.918749 phidata-2.0.0.dev7/phidata/task/download/url/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/url/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.918899 phidata-2.0.0.dev7/phidata/task/plot/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/plot/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919129 phidata-2.0.0.dev7/phidata/task/plot/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/plot/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/task/python_task.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919389 phidata-2.0.0.dev7/phidata/task/run/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/run/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919573 phidata-2.0.0.dev7/phidata/task/run/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/task/run/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/task/task.py
+-rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/task/task_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919855 phidata-2.0.0.dev7/phidata/task/upload/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/upload/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.920190 phidata-2.0.0.dev7/phidata/task/upload/file/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.921123 phidata-2.0.0.dev7/phidata/types/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/types/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/types/airflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/types/context.py
+-rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/types/phidata_runtime.py
+-rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/types/run_status.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.925127 phidata-2.0.0.dev7/phidata/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/cli_console.py
+-rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev7/phidata/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev7/phidata/utils/compare.py
+-rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/utils/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev7/phidata/utils/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/env_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev7/phidata/utils/env_var.py
+-rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/k8s.py
+-rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/utils/print_table.py
+-rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/workspace_path.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.926451 phidata-2.0.0.dev7/phidata/workflow/
+-rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev7/phidata/workflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/workflow/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.926773 phidata-2.0.0.dev7/phidata/workflow/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/workflow/workflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.927403 phidata-2.0.0.dev7/phidata/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev7/phidata/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.813444 phidata-2.0.0.dev7/phidata.egg-info/
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)    18804 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 zu         (501) staff       (20)      181 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/requires.txt
+-rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/top_level.txt
+-rw-r--r--   0 zu         (501) staff       (20)     1676 2023-07-24 14:18:36.000000 phidata-2.0.0.dev7/pyproject.toml
+-rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-24 14:18:58.928291 phidata-2.0.0.dev7/setup.cfg
+-rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev7/setup.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.927695 phidata-2.0.0.dev7/tests/
+-rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev7/tests/test_placeholder.py
```

### Comparing `phidata-2.0.0.dev6/LICENSE` & `phidata-2.0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/PKG-INFO` & `phidata-2.0.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev6 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev7 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev6/README.md` & `phidata-2.0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/api/client.py` & `phidata-2.0.0.dev7/phi/api/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-from httpx import Client, AsyncClient
 from typing import Optional
 
+import aiohttp
+
 from phi.cli.settings import phi_cli_settings
 from phi.cli.credentials import read_auth_token
 from phi.utils.log import logger
 
-base_headers = {
-    "user-agent": f"{phi_cli_settings.app_name}/{phi_cli_settings.app_version}",
-    "Content-Type": "application/json",
-}
-
-
-def get_authenticated_client() -> Optional[Client]:
-    """Returns an instance of httpx.Client with preconfigured auth and base url"""
-
-    try:
-        auth_token: Optional[str] = read_auth_token()
-    except Exception as e:
-        logger.warning(f"Failed to read auth token: {e}")
-        return None
-
-    if auth_token is None:
-        return None
-
-    authenticated_headers = base_headers.copy()
-    authenticated_headers[phi_cli_settings.auth_token_header] = auth_token
-    return Client(
-        base_url=phi_cli_settings.api_url,
-        headers=authenticated_headers,
-        cookies={phi_cli_settings.auth_token_cookie: auth_token},
-        timeout=60,
-    )
-
-
-def get_async_client() -> Optional[AsyncClient]:
-    """Returns an instance of httpx.AsyncClient with preconfigured auth and base url"""
-
-    try:
-        auth_token: Optional[str] = read_auth_token()
-    except Exception as e:
-        logger.warning(f"Failed to read auth token: {e}")
-        return None
-
-    if auth_token is None:
-        return None
-
-    authenticated_headers = base_headers.copy()
-    authenticated_headers[phi_cli_settings.auth_token_header] = auth_token
-    return AsyncClient(
-        base_url=phi_cli_settings.api_url,
-        headers=authenticated_headers,
-        cookies={phi_cli_settings.auth_token_cookie: auth_token},
-        timeout=60,
-    )
+
+class ApiClient:
+    def __init__(self):
+        self.base_url = phi_cli_settings.api_url
+        self.headers = {
+            "user-agent": f"{phi_cli_settings.app_name}/{phi_cli_settings.app_version}",
+            "Content-Type": "application/json",
+        }
+        self._authenticated_headers = None
+        self._client_session = None
+        self._authenticated_session = None
+
+    @property
+    def auth_token(self) -> Optional[str]:
+        try:
+            return read_auth_token()
+        except Exception as e:
+            logger.warning(f"Failed to read auth token: {e}")
+            return None
+
+    @property
+    def authenticated_headers(self):
+        if self._authenticated_headers is None:
+            self._authenticated_headers = self.headers.copy()
+            if self.auth_token is not None:
+                self._authenticated_headers[phi_cli_settings.auth_token_header] = self.auth_token
+        return self._authenticated_headers
+
+    def Session(self):
+        return aiohttp.ClientSession(base_url=self.base_url, headers=self.headers)
+
+    def AuthenticatedSession(self):
+        return aiohttp.ClientSession(base_url=self.base_url, headers=self.authenticated_headers)
+
+
+api_client = ApiClient()
+
+
+def invalid_respose(response: aiohttp.ClientResponse):
+    status = response.status
+    if status >= 400:
+        return True
+    return False
```

### Comparing `phidata-2.0.0.dev6/phi/api/user.py` & `phidata-2.0.0.dev7/phidata/utils/cli_console.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,169 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, Any, Optional, List, Union
 
-from httpx import Client, Response, NetworkError
+from rich.console import Console
+from rich.style import Style
 
-from phi.api.client import base_headers, get_authenticated_client
-from phi.api.helpers import is_valid_response, is_invalid_response
-from phi.api.routes import ApiRoutes
-from phi.cli.config import PhiCliConfig
-from phi.cli.console import log_network_error_msg
-from phi.cli.settings import phi_cli_settings
-from phi.schemas.user import UserSchema, EmailPasswordSignInSchema
-from phi.utils.log import logger
-
-
-def user_ping() -> bool:
-    logger.debug("--o-o-- Ping user api")
-    with Client(base_url=phi_cli_settings.api_url, headers=base_headers, timeout=60) as api:
-        try:
-            r: Response = api.get(ApiRoutes.USER_PING)
-            if is_invalid_response(r):
-                return False
-        except NetworkError:
-            log_network_error_msg()
-            return False
-
-        if is_valid_response(r):
-            return True
-    return False
-
-
-def is_user_authenticated() -> bool:
-    logger.debug("--o-o-- Authenticating user")
-    authenticated_client: Optional[Client] = get_authenticated_client()
-    if authenticated_client is None:
-        logger.debug("Session not available")
-        return False
+from phidata.utils.log import logger
+from phidata.types.run_status import RunStatus
 
-    phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
-    if phi_config is None:
-        return False
-    user: Optional[UserSchema] = phi_config.user
-    if user is None:
+console = Console()
+
+######################################################
+## Styles
+# Standard Colors: https://rich.readthedocs.io/en/stable/appendix/colors.html#appendix-colors
+######################################################
+
+heading_style = Style(
+    color="green",
+    bold=True,
+    underline=True,
+)
+subheading_style = Style(
+    color="chartreuse3",
+    bold=True,
+)
+success_style = Style(color="chartreuse3")
+fail_style = Style(color="red")
+error_style = Style(color="red")
+info_style = Style()
+warn_style = Style(color="magenta")
+
+
+######################################################
+## Print functions
+######################################################
+
+
+def print_heading(msg: str) -> None:
+    console.print(msg, style=heading_style)
+
+
+def print_subheading(msg: str) -> None:
+    console.print(msg, style=subheading_style)
+
+
+def print_horizontal_line() -> None:
+    console.rule()
+
+
+def print_info(msg: str) -> None:
+    console.print(msg, style=info_style)
+
+
+def print_fix(msg: str) -> None:
+    console.print("FIX  : {}".format(msg), style=info_style)
+
+
+def print_error(msg: Union[str, Exception]) -> None:
+    logger.error("{}".format(msg))
+
+
+def print_warning(msg: Union[str, Exception]) -> None:
+    logger.warning(f"{msg}")
+
+
+def print_dict(_dict: dict) -> None:
+    from rich.pretty import pprint
+
+    pprint(_dict)
+
+
+def get_validation_error_loc(validation_error: Dict[str, Any]) -> Optional[str]:
+    if "loc" not in validation_error:
+        return None
+    return " -> ".join(str(e) for e in validation_error["loc"])
+
+
+def print_validation_errors(validation_errors: List[Dict[str, Any]]) -> None:
+    """
+    Pretty prints pydantic validation errors.
+    TODO: pydantic validation is known to be buggy for nested models, test this function
+    """
+    from rich import box
+    from rich.table import Column, Table
+
+    table = Table(
+        Column(header="Field", justify="center"),
+        Column(header="Error", justify="center"),
+        Column(header="Context", justify="center"),
+        box=box.MINIMAL,
+        show_lines=True,
+    )
+
+    for err in validation_errors:
+        # print("err: {}".format(err))
+        error_loc = get_validation_error_loc(err)
+        _error_ctx_raw = err.get("ctx")
+        error_ctx = (
+            "\n".join(f"{k}: {v}" for k, v in _error_ctx_raw.items())
+            if _error_ctx_raw is not None and isinstance(_error_ctx_raw, dict)
+            else ""
+        )
+        error_msg = err.get("msg")
+
+        if error_loc is not None:
+            table.add_row(error_loc, error_msg, error_ctx)
+
+    if table.row_count > 0:
+        console.print(table)
+
+
+def confirm_yes_no(question, default: str = "yes") -> bool:
+    """Ask a yes/no question via raw_input().
+
+    "question" is a string that is presented to the user.
+    "default" is the presumed answer if the user just hits <Enter>.
+            It must be "yes" (the default), "no" or None (meaning
+            an answer is required of the user).
+
+    The "answer" return value is True for "yes" or False for "no".
+    """
+    inp_to_result_map = {"yes": True, "y": True, "ye": True, "no": False, "n": False}
+    if default is None:
+        prompt = " [y/n]: "
+    elif default == "yes":
+        prompt = " [Y/n]: "
+    elif default == "no":
+        prompt = " [y/N]: "
+    else:
+        raise ValueError(f"Invalid default answer: {default}")
+
+    choice = console.input(prompt=(question + prompt)).lower()
+    if default is not None and choice == "":
+        return inp_to_result_map[default]
+    elif choice in inp_to_result_map:
+        return inp_to_result_map[choice]
+    else:
+        print_error(f"{choice} invalid")
         return False
 
-    with authenticated_client as api:
-        try:
-            r: Response = api.post(
-                ApiRoutes.USER_AUTHENTICATE, data=user.model_dump_json(exclude_none=True)  # type: ignore
+
+def print_run_status_table(
+    heading: str, task_run_status: List[RunStatus], min_width: Optional[int] = None
+) -> None:
+    from rich import box
+    from rich.table import Column, Table
+
+    table = Table(
+        title=heading,
+        box=box.ASCII2,
+        show_lines=True,
+        min_width=(min_width or 50)
+        # title_style=Style(bold=True, underline=True)
+    )
+    table.add_column(header="Name", justify="center")
+    table.add_column(header="Status", justify="center")
+
+    for task in task_run_status:
+        if task.success:
+            table.add_row(
+                task.name, "Success" if task.success else "Fail", style=success_style
             )
-            if is_invalid_response(r):
-                return False
-        except NetworkError:
-            log_network_error_msg()
-            return False
-
-        response_data: Union[Dict[Any, Any], List[Any]] = r.json()
-        if response_data is None or not isinstance(response_data, dict):
-            logger.error("Could not parse response")
-            return False
-        if response_data.get("status", "fail") == "success":
-            return True
-    return False
-
-
-def authenticate_and_get_user(
-    tmp_auth_token: str,
-) -> Optional[UserSchema]:
-    from phi.cli.credentials import save_auth_token
-
-    logger.debug("--o-o-- Getting user")
-    authenticated_headers = base_headers.copy()
-    authenticated_headers[phi_cli_settings.auth_token_header] = tmp_auth_token
-    with Client(
-        base_url=phi_cli_settings.api_url,
-        headers=authenticated_headers,
-        timeout=None,
-    ) as api:
-        try:
-            r: Response = api.post(ApiRoutes.USER_CLI_AUTH, data={"token": tmp_auth_token})
-            if is_invalid_response(r):
-                return None
-        except NetworkError:
-            log_network_error_msg()
-            return None
-
-        phidata_auth_token = r.headers.get(phi_cli_settings.auth_token_header)
-        if phidata_auth_token is None:
-            logger.error("Could not authenticate user")
-            return None
-
-        user_data = r.json()
-        if not isinstance(user_data, dict):
-            raise Exception("Could not parse response")
-
-        current_user: UserSchema = UserSchema.from_dict(user_data)
-        if current_user is not None:
-            save_auth_token(phidata_auth_token)
-            return current_user
-    return None
-
-
-def sign_in_user(
-    sign_in_data: EmailPasswordSignInSchema,
-) -> Optional[UserSchema]:
-    from phi.cli.credentials import save_auth_token
-
-    logger.debug("--o-o-- Sign in user")
-    with Client(
-        base_url=phi_cli_settings.api_url,
-        headers=base_headers,
-        timeout=None,
-    ) as api:
-        try:
-            r: Response = api.post(ApiRoutes.USER_SIGN_IN, json=sign_in_data.dict())
-            if is_invalid_response(r):
-                return None
-        except NetworkError:
-            log_network_error_msg()
-            return None
-
-        phidata_auth_token = r.headers.get(phi_cli_settings.auth_token_header)
-        if phidata_auth_token is None:
-            logger.error("Could not authenticate user")
-            return None
-
-        user_data = r.json()
-        if not isinstance(user_data, dict):
-            raise Exception("Could not parse response")
-
-        current_user: UserSchema = UserSchema.from_dict(user_data)
-        if current_user is not None:
-            save_auth_token(phidata_auth_token)
-            return current_user
-    return None
+        else:
+            table.add_row(
+                task.name, "Success" if task.success else "Fail", style=fail_style
+            )
+
+    if table.row_count > 0:
+        console.print("")
+        console.print(table)
```

### Comparing `phidata-2.0.0.dev6/phi/aws/api_client.py` & `phidata-2.0.0.dev7/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/app/base.py` & `phidata-2.0.0.dev7/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/app/fastapi/fastapi.py` & `phidata-2.0.0.dev7/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/app/jupyter/jupyter.py` & `phidata-2.0.0.dev7/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/app/qdrant/qdrant.py` & `phidata-2.0.0.dev7/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/app/streamlit/streamlit.py` & `phidata-2.0.0.dev7/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev7/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/base.py` & `phidata-2.0.0.dev7/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev7/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev7/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev7/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev7/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev7/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ecs/container.py` & `phidata-2.0.0.dev7/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ecs/service.py` & `phidata-2.0.0.dev7/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev7/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev7/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/eks/addon.py` & `phidata-2.0.0.dev7/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev7/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev7/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev7/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev7/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev7/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev7/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/elb/listener.py` & `phidata-2.0.0.dev7/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev7/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev7/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev7/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev7/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/group.py` & `phidata-2.0.0.dev7/phi/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/iam/policy.py` & `phidata-2.0.0.dev7/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/iam/role.py` & `phidata-2.0.0.dev7/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev7/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev7/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev7/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev7/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/secret/manager.py` & `phidata-2.0.0.dev7/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/secret/reader.py` & `phidata-2.0.0.dev7/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/aws/resource/types.py` & `phidata-2.0.0.dev7/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/base.py` & `phidata-2.0.0.dev7/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/cli/auth_server.py` & `phidata-2.0.0.dev7/phi/cli/auth_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from typing import Optional
 
 from phi.cli.settings import phi_cli_settings
-from phi.utils.log import logger
 
 
 class CliAuthRequestHandler(BaseHTTPRequestHandler):
     """Request Handler to accept the CLI auth token after the web based auth flow.
     References:
         https://medium.com/@hasinthaindrajee/browser-sso-for-cli-applications-b0be743fa656
         https://gist.github.com/mdonkers/63e115cc0c79b4f6b8b3a6b797e485c7
@@ -25,32 +24,32 @@
 
     # def do_GET(self):
     #     logger.info("GET request,\nPath: %s\nHeaders:\n%s\n", str(self.path), str(self.headers))
     #     self._set_response()
     #     self.wfile.write("GET request for {}".format(self.path).encode('utf-8'))
 
     def do_OPTIONS(self):
-        logger.info(
-            "OPTIONS request,\nPath: %s\nHeaders:\n%s\n",
-            str(self.path),
-            str(self.headers),
-        )
+        # logger.debug(
+        #     "OPTIONS request,\nPath: %s\nHeaders:\n%s\n",
+        #     str(self.path),
+        #     str(self.headers),
+        # )
         self._set_response()
         # self.wfile.write("OPTIONS request for {}".format(self.path).encode('utf-8'))
 
     def do_POST(self):
         content_length = int(self.headers["Content-Length"])  # <--- Gets the size of data
         post_data = self.rfile.read(content_length)  # <--- Gets the data itself
         decoded_post_data = post_data.decode("utf-8")
-        logger.info(
-            "POST request,\nPath: {}\nHeaders:\n{}\n\nBody:\n{}\n".format(
-                str(self.path), str(self.headers), decoded_post_data
-            )
-        )
-        logger.info("Data: {}".format(decoded_post_data))
+        # logger.debug(
+        #     "POST request,\nPath: {}\nHeaders:\n{}\n\nBody:\n{}\n".format(
+        #         str(self.path), str(self.headers), decoded_post_data
+        #     )
+        # )
+        # logger.debug("Data: {}".format(decoded_post_data))
         # logger.info("type: {}".format(type(post_data)))
         phi_cli_settings.auth_token_path.touch(exist_ok=True)
         phi_cli_settings.auth_token_path.write_text(decoded_post_data)
         # TODO: Add checks before shutting down the server
         self.server.running = False  # type: ignore
         self._set_response()
 
@@ -59,15 +58,15 @@
 
 
 class CliAuthServer:
     """
     Source: https://stackoverflow.com/a/38196725/10953921
     """
 
-    def __init__(self, port=9190):
+    def __init__(self, port=9191):
         import threading
 
         self._server = HTTPServer(("", port), CliAuthRequestHandler)
         self._thread = threading.Thread(target=self.run)
         self._thread.daemon = True
         self._server.running = False  # type: ignore
 
@@ -81,21 +80,21 @@
 
     def shut_down(self):
         self._thread.close()  # type: ignore
 
 
 def get_port_for_auth_server():
     # TODO: Check if port is available
-    return 9190
+    return 9191
 
 
 def get_auth_token_from_web_flow(port) -> Optional[str]:
     """
-    GET request: curl http://localhost:9190
-    POST request: curl -d "foo=bar&bin=baz" http://localhost:9190
+    GET request: curl http://localhost:9191
+    POST request: curl -d "foo=bar&bin=baz" http://localhost:9191
     """
     import json
 
     server = CliAuthServer(port)
     server.run()
 
     if phi_cli_settings.auth_token_path.exists() and phi_cli_settings.auth_token_path.is_file():
```

### Comparing `phidata-2.0.0.dev6/phi/cli/config.py` & `phidata-2.0.0.dev7/phi/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import OrderedDict
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from phi.cli.console import print_heading, print_info
 from phi.cli.settings import phi_cli_settings
-from phi.schemas.user import UserSchema
-from phi.schemas.workspace import WorkspaceSchema
+from phi.api.schemas.user import UserSchema
+from phi.api.schemas.workspace import WorkspaceSchema
 from phi.utils.log import logger
 from phi.utils.pickle import pickle_object_to_file, unpickle_object_from_file
 from phi.workspace.config import WorkspaceConfig
 
 
 class PhiCliConfig:
     """The PhiCliConfig class manages user data for the phi cli"""
@@ -179,48 +179,45 @@
             ws_schema=ws_schema,
             ws_root_path=ws_root_path,
         )
         if set_as_active:
             self.active_ws_name = ws_name
         self.save_config()
 
-    def delete_ws(self, ws_name: str) -> bool:
-        """Handles Deleting a workspace from the PhiCliConfig"""
+    async def delete_ws(self, ws_name: str) -> None:
+        """Handles Deleting a workspace from the PhiCliConfig and api"""
+
         print_heading(f"Deleting record for: {ws_name}")
         print_info("-*- Note: this does not delete any files on disk, please delete them manually")
 
         ws_config: Optional[WorkspaceConfig] = self.ws_config_map.pop(ws_name, None)
         if ws_config is None:
             logger.warning(f"No record of workspace {ws_name}")
-            return True
+            return
 
         if ws_config.ws_root_path is not None:
             self.path_to_ws_config_map.pop(ws_config.ws_root_path, None)
 
         # Check if we're deleting the active workspace, if yes, unset the active ws
         if (
             self._active_ws_name is not None
             and ws_config.ws_name is not None
             and self._active_ws_name == ws_config.ws_name
         ):
             print_info(f"Removing {ws_config.ws_name} as the active workspace")
             self._active_ws_name = None
 
-        # TODO: Delete the workspace from the api
-        # from phi.api.workspace import delete_workspaces_api
-        # workspaces_deleted = delete_workspaces_api(
-        #     user=phi_config.user, workspaces_to_delete=ws_to_delete
-        # )
-        # if workspaces_deleted:
-        #     pass
-        #     # phi_conf.delete_ws_data(ws_name=ws)
-        # return workspaces_deleted
+        if self.user is not None and ws_config.ws_schema is not None:
+            print_info(f"Deleting workspace {ws_config.ws_name} from the server")
+
+            from phi.api.workspace import delete_workspace_for_user
+
+            await delete_workspace_for_user(user=self.user, workspace=ws_config.ws_schema)
 
         self.save_config()
-        return True
 
     ######################################################
     ## Get Workspace Data
     ######################################################
 
     def get_ws_config_by_name(self, ws_name: str) -> Optional[WorkspaceConfig]:
         return self.ws_config_map[ws_name] if ws_name in self.ws_config_map else None
@@ -261,37 +258,35 @@
         logger.debug(f"++**++ Config refreshed: {ws_name}")
         self.save_config()
 
     ######################################################
     ## Sync Workspace Data from api
     ######################################################
 
-    def sync_workspaces_from_api(self) -> bool:
+    async def sync_workspaces_from_api(self) -> None:
         from phi.api.workspace import get_primary_workspace, get_available_workspaces
 
         if self.user is None:
             logger.error("User not available for workspace sync")
-            return False
+            return
 
         # Call api to get the available workspaces
-        available_workspaces: Optional[List[WorkspaceSchema]] = get_available_workspaces(self.user)
+        available_workspaces: Optional[List[WorkspaceSchema]] = await get_available_workspaces(self.user)
         if available_workspaces is not None:
             logger.debug(f"Received {len(available_workspaces)} available workspaces")
             self.available_ws = available_workspaces
 
         # Call api to get the primary_ws
-        primary_ws: Optional[WorkspaceSchema] = get_primary_workspace(self.user)
+        primary_ws: Optional[WorkspaceSchema] = await get_primary_workspace(self.user)
         if primary_ws is None:
             logger.debug("No primary workspace available")
         else:
             logger.debug(f"Received primary ws: {primary_ws.model_dump_json(indent=2)}")
             self.active_ws_name = primary_ws.ws_name
 
-        return True
-
     ######################################################
     ## Save PhiCliConfig
     ######################################################
 
     def save_config(self):
         logger.debug(f"Saving config to {str(phi_cli_settings.config_file_path)}")
         pickle_object_to_file(self, phi_cli_settings.config_file_path)
```

### Comparing `phidata-2.0.0.dev6/phi/cli/console.py` & `phidata-2.0.0.dev7/phi/cli/console.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,32 +59,16 @@
 
 
 def print_available_workspaces(avl_ws_list) -> None:
     avl_ws_names = [w.name for w in avl_ws_list] if avl_ws_list else []
     print_info("Available Workspaces:\n  - {}".format("\n  - ".join(avl_ws_names)))
 
 
-def log_generic_error_msg() -> None:
-    logger.error("Something went wrong. Please try again.")
-
-
-def log_client_error_msg() -> None:
-    logger.error("ClientError: Please try again.")
-
-
-def log_network_error_msg() -> None:
-    logger.error("NetworkError: Please check internet connectivity.")
-
-
-def log_server_error_msg() -> None:
-    logger.error("ServerError: Could not reach phidata servers.")
-
-
-def log_auth_error_msg() -> None:
-    logger.error("AuthError: could not authenticate, please run `phi auth`")
+def log_phi_init_failed_msg() -> None:
+    logger.error("phi initialization failed, please try again")
 
 
 def confirm_yes_no(question, default: str = "yes") -> bool:
     """Ask a yes/no question via raw_input().
 
     "question" is a string that is presented to the user.
     "default" is the presumed answer if the user just hits <Enter>.
```

### Comparing `phidata-2.0.0.dev6/phi/cli/credentials.py` & `phidata-2.0.0.dev7/phi/cli/credentials.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Optional
 
 from phi.cli.settings import phi_cli_settings
 from phi.utils.pickle import pickle_object_to_file, unpickle_object_from_file
-from phi.utils.log import logger
 
 
 class PhiCliCreds:
     def __init__(self, auth_token: str):
         self._auth_token = auth_token
 
     @property
     def auth_token(self) -> str:
         return self._auth_token
 
 
 def save_auth_token(auth_token: str):
-    logger.debug(f"Storing {auth_token} to {str(phi_cli_settings.credentials_path)}")
+    # logger.debug(f"Storing {auth_token} to {str(phi_cli_settings.credentials_path)}")
     creds = PhiCliCreds(auth_token)
     pickle_object_to_file(creds, phi_cli_settings.credentials_path)
 
 
 def read_auth_token() -> Optional[str]:
-    logger.debug(f"Reading token from {str(phi_cli_settings.credentials_path)}")
+    # logger.debug(f"Reading token from {str(phi_cli_settings.credentials_path)}")
     creds: PhiCliCreds = unpickle_object_from_file(phi_cli_settings.credentials_path)
     return creds.auth_token
```

### Comparing `phidata-2.0.0.dev6/phi/cli/entrypoint.py` & `phidata-2.0.0.dev7/phi/cli/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Phi Cli
 
 This is the entrypoint for the `phi` cli application.
 """
+from asyncio import run as aiorun
 from typing import Optional
 
 import typer
 
 from phi.cli.ws.ws_cli import ws_cli
 
 # from phi.cli.k8s.k8s_app import k8s_app
@@ -51,18 +52,18 @@
     * `phi init -r` -> Reset and initializing phidata
     """
     if print_debug_log:
         set_log_level_to_debug()
 
     from phi.cli.operator import initialize_phi
 
-    initialize_phi(reset=reset, login=login)
+    aiorun(initialize_phi(reset=reset, login=login))
 
 
-@phi_cli.command(short_help="Reset phidata installation")
+@phi_cli.command(short_help="Reset phi installation")
 def reset(
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
@@ -73,15 +74,15 @@
     After resetting please run `phi init` to initialize again.
     """
     if print_debug_log:
         set_log_level_to_debug()
 
     from phi.cli.operator import initialize_phi
 
-    initialize_phi(reset=True)
+    aiorun(initialize_phi(reset=True))
 
 
 @phi_cli.command(short_help="Authenticate with phidata.com")
 def auth(
     print_debug_log: bool = typer.Option(
         False,
         "-d",
@@ -94,15 +95,15 @@
     Authenticate your account with phidata.
     """
     if print_debug_log:
         set_log_level_to_debug()
 
     from phi.cli.operator import authenticate_user
 
-    authenticate_user()
+    aiorun(authenticate_user())
 
 
 @phi_cli.command(short_help="Log in from the cli", hidden=True)
 def login(
     print_debug_log: bool = typer.Option(
         False,
         "-d",
@@ -119,46 +120,41 @@
     * `phi login`
     """
     if print_debug_log:
         set_log_level_to_debug()
 
     from phi.cli.operator import sign_in_using_cli
 
-    sign_in_using_cli()
+    aiorun(sign_in_using_cli())
 
 
-@phi_cli.command(short_help="Ping phidata servers", hidden=True)
+@phi_cli.command(short_help="Ping phidata servers")
 def ping(
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
 ):
     """Ping the phidata servers and check if you are authenticated"""
     if print_debug_log:
         set_log_level_to_debug()
 
-    from phi.api.user import user_ping, is_user_authenticated
+    from phi.api.user import user_ping
     from phi.cli.console import print_info
 
-    ping_success = user_ping()
+    ping_success = aiorun(user_ping())
     if ping_success:
         print_info("Ping successful")
     else:
         print_info("Could not reach phidata servers")
 
-    if is_user_authenticated():
-        print_info("User is authenticated")
-    else:
-        print_info("User is not authenticated, run `phi auth` to log in")
-
 
-@phi_cli.command(short_help="Print phidata config", hidden=True)
+@phi_cli.command(short_help="Print phi config")
 def config(
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
@@ -179,45 +175,45 @@
     conf: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if conf is not None:
         conf.print_to_cli(show_all=show_all)
     else:
         print_info("Phi not initialized, run `phi init` to get started")
 
 
-# @phi_cli.command(short_help="Set current directory as active workspace")
-# def set(
-#     ws_name: str = typer.Option(None, "-ws", help="Active workspace name"),
-#     print_debug_log: bool = typer.Option(
-#         False,
-#         "-d",
-#         "--debug",
-#         help="Print debug logs.",
-#     ),
-# ):
-#     """
-#     \b
-#     Setup the current directory as the active workspace.
-#     This command can be run from within the workspace directory
-#         OR with a -ws flag to set another workspace as primary.
-#
-#     Set a workspace as active
-#
-#     \b
-#     Examples:
-#     $ `phi ws set`           -> Set the current directory as the active phidata workspace
-#     $ `phi ws set -ws idata` -> Set the workspace named idata as the active phidata workspace
-#     """
-#     from phi.workspace.ws_operator import set_workspace_as_active
-#
-#     if print_debug_log:
-#         set_log_level_to_debug()
-#
-#     operation_success: bool = set_workspace_as_active(ws_name)
-#
-#
+@phi_cli.command(short_help="Set current directory as active workspace")
+def set(
+    ws_name: str = typer.Option(None, "-ws", help="Active workspace name"),
+    print_debug_log: bool = typer.Option(
+        False,
+        "-d",
+        "--debug",
+        help="Print debug logs.",
+    ),
+):
+    """
+    \b
+    Set the current directory as the active workspace.
+    This command can be run from within the workspace directory
+        OR with a -ws flag to set another workspace as primary.
+
+    Set a workspace as active
+
+    \b
+    Examples:
+    $ `phi ws set`           -> Set the current directory as the active phidata workspace
+    $ `phi ws set -ws idata` -> Set the workspace named idata as the active phidata workspace
+    """
+    from phi.workspace.operator import set_workspace_as_active
+
+    if print_debug_log:
+        set_log_level_to_debug()
+
+    aiorun(set_workspace_as_active(ws_name))
+
+
 # @phi_cli.command(short_help="Start resources defined in a resources.py file")
 # def start(
 #     resources_file: str = typer.Argument(
 #         "resources.py",
 #         help="Path to workspace file.",
 #         show_default=False,
 #     ),
```

### Comparing `phidata-2.0.0.dev6/phi/cli/operator.py` & `phidata-2.0.0.dev7/phi/cli/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 def delete_phidata_conf() -> None:
     from phi.utils.filesystem import delete_from_fs
 
     logger.debug("Removing existing Phidata configuration")
     delete_from_fs(PHI_CLI_DIR)
 
 
-def authenticate_user() -> bool:
+async def authenticate_user() -> None:
     """Authenticate the user using credentials from phidata.com
     Steps:
     1. Authenticate the user by opening the phidata sign-in url
         and the web-app will post an auth token to a mini http server
         running on the auth_server_port.
     2. Using the auth_token, authenticate the CLI with api and
         save the auth_token. This step is handled by authenticate_and_get_user()
     3. After the user is authenticated update the PhiCliConfig.
     """
     from phi.api.user import authenticate_and_get_user
-    from phi.schemas.user import UserSchema
+    from phi.api.schemas.user import UserSchema
     from phi.cli.auth_server import (
         get_port_for_auth_server,
         get_auth_token_from_web_flow,
     )
 
     print_heading("Authenticating with phidata.com ...")
 
@@ -40,36 +40,38 @@
     print_info("\nYour browser will be opened to visit:\n{}".format(auth_url))
     typer_launch(auth_url)
     print_info("\nWaiting for a response from browser...\n")
 
     tmp_auth_token = get_auth_token_from_web_flow(auth_server_port)
     if tmp_auth_token is None:
         logger.error("Could not authenticate, please try again")
-        return False
+        return
 
     try:
-        user: Optional[UserSchema] = authenticate_and_get_user(tmp_auth_token)
+        user: Optional[UserSchema] = await authenticate_and_get_user(tmp_auth_token)
     except Exception as e:
         logger.exception(e)
         logger.error("Could not authenticate, please try again")
-        return False
+        return
 
     if user is None:
         logger.error("Could not get user data, please try again")
-        return False
+        return
 
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if phi_config is None:
         phi_config = PhiCliConfig(user)
+    else:
+        phi_config.user = user
 
-    print_info("Welcome {}, you are authenticated\n".format(user.email))
-    return phi_config.sync_workspaces_from_api()
+    print_info("Welcome {}".format(user.email))
+    await phi_config.sync_workspaces_from_api()
 
 
-def initialize_phi(reset: bool = False, login: bool = False) -> bool:
+async def initialize_phi(reset: bool = False, login: bool = False) -> bool:
     """Initialize phi on the users machine.
 
     Steps:
     1. Check if PHI_CLI_DIR exists, if not, create it. If reset == True, recreate PHI_CLI_DIR.
     2. Authenticates the user if login == True.
     3. If PhiCliConfig exists and auth is valid, return True.
     """
@@ -103,55 +105,56 @@
 
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if phi_config is None:
         logger.debug("Creating new PhiCliConfig")
         phi_config = PhiCliConfig()
 
     # Authenticate user
-    auth_valid: bool = True
     if login:
-        auth_valid = authenticate_user()
+        await authenticate_user()
 
-    if phi_config is not None and auth_valid:
+    if phi_config is not None:
         logger.debug("Phidata initialized")
         return True
     else:
         logger.error("Something went wrong, please try again")
         return False
 
 
-def sign_in_using_cli() -> bool:
+async def sign_in_using_cli() -> None:
     from getpass import getpass
     from phi.api.user import sign_in_user
-    from phi.schemas.user import UserSchema, EmailPasswordSignInSchema
+    from phi.api.schemas.user import UserSchema, EmailPasswordAuthSchema
 
     print_heading("Log in")
     email_raw = input("email: ")
     pass_raw = getpass()
 
     if email_raw is None or pass_raw is None:
         logger.error("Incorrect email or password")
 
     try:
-        user: Optional[UserSchema] = sign_in_user(EmailPasswordSignInSchema(email=email_raw, password=pass_raw))
+        user: Optional[UserSchema] = await sign_in_user(EmailPasswordAuthSchema(email=email_raw, password=pass_raw))
     except Exception as e:
         logger.exception(e)
         logger.error("Could not authenticate, please try again")
-        return False
+        return
 
     if user is None:
-        logger.error("Could not get user data, please try again")
-        return False
+        logger.error("Could not get user, please try again")
+        return
 
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if phi_config is None:
         phi_config = PhiCliConfig(user)
+    else:
+        phi_config.user = user
 
-    print_info("Welcome {}, you are authenticated\n".format(user.email))
-    return phi_config.sync_workspaces_from_api()
+    print_info("Welcome {}".format(user.email))
+    await phi_config.sync_workspaces_from_api()
 
 
 # def start_resources(
 #     resources_file_path: Path,
 #     target_env: Optional[str] = None,
 #     target_config: Optional[Any] = None,
 #     target_name: Optional[str] = None,
```

### Comparing `phidata-2.0.0.dev6/phi/cli/settings.py` & `phidata-2.0.0.dev7/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/cli/ws/ws_cli.py` & `phidata-2.0.0.dev7/phi/cli/ws/ws_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Phi Workspace Cli
 
 This is the entrypoint for the `phi ws` application.
 """
+from asyncio import run as aiorun
 from pathlib import Path
 from typing import Optional, cast
 
 import typer
 
 from phi.cli.console import (
     print_info,
@@ -70,15 +71,15 @@
     > phi ws create -t llm-app -n llm   -> Create an `llm-app` named `llm` in the current directory
     """
     if print_debug_log:
         set_log_level_to_debug()
 
     from phi.workspace.operator import create_workspace
 
-    create_workspace(name=name, template=template, url=url)
+    aiorun(create_workspace(name=name, template=template, url=url))
 
 
 @ws_cli.command(short_help="Setup workspace from the current directory")
 def setup(
     path: Optional[str] = typer.Argument(
         None,
         help="Path to workspace [default: current directory]",
@@ -106,15 +107,15 @@
     # By default, we assume this command is run from the workspace directory
     ws_root_path: Path = Path(".").resolve()
 
     # If the user provides a path, use that to setup the workspace
     if path is not None:
         ws_root_path = Path(".").joinpath(path).resolve()
 
-    setup_workspace(ws_root_path=ws_root_path)
+    aiorun(setup_workspace(ws_root_path=ws_root_path))
 
 
 @ws_cli.command(short_help="Create resources for the active workspace")
 def up(
     resource_filter: Optional[str] = typer.Argument(
         None,
         help="Resource filter. Format - ENV:INFRA:GROUP:NAME:TYPE",
@@ -262,24 +263,26 @@
     logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     logger.debug(f"\tforce        : {force}")
     print_heading("Starting workspace: {}\n".format(active_ws_config.ws_name))
-    start_workspace(
-        ws_config=active_ws_config,
-        target_env=target_env,
-        target_infra=target_infra,
-        target_group=target_group,
-        target_name=target_name,
-        target_type=target_type,
-        dry_run=dry_run,
-        auto_confirm=auto_confirm,
-        force=force,
+    aiorun(
+        start_workspace(
+            ws_config=active_ws_config,
+            target_env=target_env,
+            target_infra=target_infra,
+            target_group=target_group,
+            target_name=target_name,
+            target_type=target_type,
+            dry_run=dry_run,
+            auto_confirm=auto_confirm,
+            force=force,
+        )
     )
 
 
 @ws_cli.command(short_help="Delete resources for active workspace")
 def down(
     resource_filter: Optional[str] = typer.Argument(
         None,
@@ -426,24 +429,26 @@
     logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     logger.debug(f"\tforce        : {force}")
     print_heading("Stopping workspace: {}\n".format(active_ws_config.ws_name))
-    stop_workspace(
-        ws_config=active_ws_config,
-        target_env=target_env,
-        target_infra=target_infra,
-        target_group=target_group,
-        target_name=target_name,
-        target_type=target_type,
-        dry_run=dry_run,
-        auto_confirm=auto_confirm,
-        force=force,
+    aiorun(
+        stop_workspace(
+            ws_config=active_ws_config,
+            target_env=target_env,
+            target_infra=target_infra,
+            target_group=target_group,
+            target_name=target_name,
+            target_type=target_type,
+            dry_run=dry_run,
+            auto_confirm=auto_confirm,
+            force=force,
+        )
     )
 
 
 @ws_cli.command(short_help="Update resources for active workspace")
 def patch(
     resource_filter: Optional[str] = typer.Argument(
         None,
@@ -588,24 +593,26 @@
     logger.debug(f"\ttarget_group : {target_group}")
     logger.debug(f"\ttarget_name  : {target_name}")
     logger.debug(f"\ttarget_type  : {target_type}")
     logger.debug(f"\tdry_run      : {dry_run}")
     logger.debug(f"\tauto_confirm : {auto_confirm}")
     logger.debug(f"\tforce        : {force}")
     print_heading("Updating workspace: {}\n".format(active_ws_config.ws_name))
-    update_workspace(
-        ws_config=active_ws_config,
-        target_env=target_env,
-        target_infra=target_infra,
-        target_group=target_group,
-        target_name=target_name,
-        target_type=target_type,
-        dry_run=dry_run,
-        auto_confirm=auto_confirm,
-        force=force,
+    aiorun(
+        update_workspace(
+            ws_config=active_ws_config,
+            target_env=target_env,
+            target_infra=target_infra,
+            target_group=target_group,
+            target_name=target_name,
+            target_type=target_type,
+            dry_run=dry_run,
+            auto_confirm=auto_confirm,
+            force=force,
+        )
     )
 
 
 @ws_cli.command(short_help="Restart resources for active workspace")
 def restart(
     resource_filter: Optional[str] = typer.Argument(
         None,
@@ -765,18 +772,20 @@
 
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if not phi_config:
         log_config_not_available_msg()
         return
 
     ws_to_delete = []
-    # By default, we assume this command is run from the workspace directory
+    # Delete workspace by name if provided
     if ws_name is not None:
         ws_to_delete.append(ws_name)
     else:
+        # Delete all workspaces if flag is set
         if all_workspaces:
             ws_to_delete = [ws.ws_name for ws in phi_config.available_ws if ws.ws_name is not None]
         else:
+            # # By default, we assume this command is run for the active workspace
             if phi_config.active_ws_name is not None:
                 ws_to_delete.append(phi_config.active_ws_name)
 
-    delete_workspace(phi_config, ws_to_delete)
+    aiorun(delete_workspace(phi_config, ws_to_delete))
```

### Comparing `phidata-2.0.0.dev6/phi/constants.py` & `phidata-2.0.0.dev7/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/api_client.py` & `phidata-2.0.0.dev7/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/base.py` & `phidata-2.0.0.dev7/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/django/django.py` & `phidata-2.0.0.dev7/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/fastapi/fastapi.py` & `phidata-2.0.0.dev7/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/jupyter/jupyter.py` & `phidata-2.0.0.dev7/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/postgres/postgres.py` & `phidata-2.0.0.dev7/phi/docker/app/postgres/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # -*- Postgres Configuration
     # Provide POSTGRES_USER as db_user or POSTGRES_USER in secrets_file
     db_user: Optional[str] = None
     # Provide POSTGRES_PASSWORD as db_password or POSTGRES_PASSWORD in secrets_file
     db_password: Optional[str] = None
     # Provide POSTGRES_DB as db_schema or POSTGRES_DB in secrets_file
     db_schema: Optional[str] = None
-    db_driver: str = "postgresql"
+    db_driver: str = "postgresql+psycopg"
     pgdata: Optional[str] = "/var/lib/postgresql/data/pgdata"
     postgres_initdb_args: Optional[str] = None
     postgres_initdb_waldir: Optional[str] = None
     postgres_host_auth_method: Optional[str] = None
     postgres_password_file: Optional[str] = None
     postgres_user_file: Optional[str] = None
     postgres_db_file: Optional[str] = None
@@ -49,15 +49,15 @@
     def get_db_password(self) -> Optional[str]:
         return self.db_password or self.get_secret_from_file("POSTGRES_PASSWORD")
 
     def get_db_schema(self) -> Optional[str]:
         return self.db_schema or self.get_secret_from_file("POSTGRES_DB")
 
     def get_db_driver(self) -> Optional[str]:
-        return self.db_driver or "postgresql"
+        return self.db_driver
 
     def get_db_host(self) -> Optional[str]:
         return self.get_container_name()
 
     def get_db_port(self) -> Optional[int]:
         return self.container_port
```

### Comparing `phidata-2.0.0.dev6/phi/docker/app/qdrant/qdrant.py` & `phidata-2.0.0.dev7/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/app/streamlit/streamlit.py` & `phidata-2.0.0.dev7/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/base.py` & `phidata-2.0.0.dev7/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/container.py` & `phidata-2.0.0.dev7/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/group.py` & `phidata-2.0.0.dev7/phi/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/image.py` & `phidata-2.0.0.dev7/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/network.py` & `phidata-2.0.0.dev7/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/types.py` & `phidata-2.0.0.dev7/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/docker/resource/volume.py` & `phidata-2.0.0.dev7/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/document/base.py` & `phidata-2.0.0.dev7/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/document/reader/base.py` & `phidata-2.0.0.dev7/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/document/reader/pdf.py` & `phidata-2.0.0.dev7/phi/document/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/embedder/openai.py` & `phidata-2.0.0.dev7/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/infra/app/base.py` & `phidata-2.0.0.dev7/phi/infra/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/infra/app/context.py` & `phidata-2.0.0.dev7/phi/infra/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/infra/app/db_app.py` & `phidata-2.0.0.dev7/phi/infra/app/db_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,35 @@
     def get_db_schema(self) -> Optional[str]:
         return self.db_schema or self.get_secret_from_file("DB_SCHEMA")
 
     def get_db_driver(self) -> Optional[str]:
         return self.db_driver or self.get_secret_from_file("DB_DRIVER")
 
     def get_db_host(self) -> Optional[str]:
-        return "localhost"
+        raise NotImplementedError
 
     def get_db_port(self) -> Optional[int]:
-        return self.host_port
+        raise NotImplementedError
 
-    def get_db_connection_url(self) -> Optional[str]:
+    def get_db_connection(self) -> Optional[str]:
         user = self.get_db_user()
         password = self.get_db_password()
         schema = self.get_db_schema()
         driver = self.get_db_driver()
         host = self.get_db_host()
         port = self.get_db_port()
         return f"{driver}://{user}:{password}@{host}:{port}/{schema}"
+
+    def get_db_host_local(self) -> Optional[str]:
+        return "localhost"
+
+    def get_db_port_local(self) -> Optional[int]:
+        return self.host_port
+
+    def get_db_connection_local(self) -> Optional[str]:
+        user = self.get_db_user()
+        password = self.get_db_password()
+        schema = self.get_db_schema()
+        driver = self.get_db_driver()
+        host = self.get_db_host_local()
+        port = self.get_db_port_local()
+        return f"{driver}://{user}:{password}@{host}:{port}/{schema}"
```

### Comparing `phidata-2.0.0.dev6/phi/infra/resource/base.py` & `phidata-2.0.0.dev7/phi/infra/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/infra/resource/group.py` & `phidata-2.0.0.dev7/phi/infra/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/llm/conversation/conversation.py` & `phidata-2.0.0.dev7/phi/llm/conversation/conversation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,146 @@
 from typing import List, Any, Optional, Dict, Iterator
 
-from pydantic import BaseModel, ConfigDict, field_validator, model_validator
+from pydantic import BaseModel, ConfigDict, field_validator
 
 from phi.document import Document
 from phi.llm.base import LLM
-from phi.llm.conversation.schemas import Message
-from phi.llm.conversation.storage.base import ConversationStorage
-from phi.llm.knowledge.base import KnowledgeBase
+from phi.llm.schemas import Message, References
+from phi.llm.conversation.schemas import ConversationRow
+from phi.llm.storage.base import LLMStorage
+from phi.llm.history.base import LLMHistory
+from phi.llm.history.simple import SimpleConversationHistory
+from phi.llm.knowledge.base import LLMKnowledgeBase
 from phi.llm.openai import OpenAIChat
 from phi.utils.log import logger, set_log_level_to_debug
 
 
 class Conversation(BaseModel):
-    # System settings
+    # The ID of this conversation.
+    id: Optional[int] = None
+    # The name of this conversation.
+    name: Optional[str] = None
     # Set log level to debug
     debug_logs: bool = False
+    # Send monitoring data to phidata.com
+    monitoring: bool = False
 
     # LLM settings
     llm: LLM = OpenAIChat()
     llm_name: Optional[str] = None
-    llm_messages: List[Message] = []
+    system_prompt: Optional[str] = None
 
     # User settings
     user_id: str = "anonymous"
     user_persona: Optional[str] = None
     user_data: Optional[Dict[str, Any]] = None
-    user_messages: List[Message] = []
-
-    # Prompt settings
-    system_prompt: Optional[str] = None
-    # Chat history settings
-    max_chat_history_messages: int = 6
-    max_chat_history_tokens: Optional[int] = None
-    include_responses_in_chat_history: bool = True
 
     # Usage data
     usage_data: Dict[str, Any] = {}
 
-    # Knowledge base for conversation
-    knowledge_base: Optional[KnowledgeBase] = None
+    # Conversation history
+    history: LLMHistory = SimpleConversationHistory()
+    add_history_to_prompt: bool = True
+    add_history_to_messages: bool = False
 
-    # Storage for conversation
-    storage: Optional[ConversationStorage] = None
+    # Knowledge base for the LLM
+    knowledge_base: Optional[LLMKnowledgeBase] = None
+
+    # Conversation storage
+    storage: Optional[LLMStorage] = None
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     @field_validator("debug_logs", mode="before")
     def set_log_level(cls, v: bool) -> bool:
         if v:
             set_log_level_to_debug()
             logger.debug("Debug logs enabled")
         return v
 
-    @model_validator(mode="after")  # type: ignore
-    def initialize_storage(self):
-        if self.storage is not None:
-            logger.debug("Initializing storage")
-            self.storage.create()
-            self.read_from_storage()  # type: ignore
-        return self
-
     @property
-    def user_chat_history(self) -> List[Dict[str, Any]]:
-        return [message.model_dump(exclude_none=True) for message in self.user_messages]
+    def conversation_row(self) -> ConversationRow:
+        """Return the conversation row"""
+
+        return ConversationRow(
+            id=self.id,
+            name=self.name,
+            user_id=self.user_id,
+            user_persona=self.user_persona,
+            user_data=self.user_data,
+            is_active=True,
+            history=self.history,
+            usage_data=self.usage_data,
+            created_at=None,
+            updated_at=None,
+        )
+
+    @conversation_row.setter
+    def conversation_row(self, conversation_row: ConversationRow):
+        """Set the conversation row"""
+
+        # Values that should be overwritten only if they are None
+        if self.id is None and conversation_row.id is not None:
+            self.id = conversation_row.id
+        if self.name is None and conversation_row.name is not None:
+            self.name = conversation_row.name
+        if self.user_persona is None and conversation_row.user_persona is not None:
+            self.user_persona = conversation_row.user_persona
+        if self.user_data is None and conversation_row.user_data is not None:
+            self.user_data = conversation_row.user_data
+
+        # Update current conversation using existing conversation
+        if conversation_row.history is not None:
+            self.history.chat_history = conversation_row.history.chat_history
+            self.history.llm_history = conversation_row.history.llm_history
+            self.history.references = conversation_row.history.references
+        if conversation_row.usage_data is not None:
+            self.usage_data = conversation_row.usage_data
 
     @property
-    def llm_chat_history(self) -> List[Dict[str, Any]]:
-        return [message.model_dump(exclude_none=True) for message in self.llm_messages]
+    def conversation_id(self) -> Optional[int]:
+        if self.id is not None:
+            return self.id
+
+        # The create function creates a new conversation row in the database
+        # and returns the ID of the new conversation.
+        return self.start()
+
+    def start(self) -> Optional[int]:
+        """Creates a new conversation and returns the conversation ID
+        that can be used to retrieve this conversation later"""
 
-    def get_chat_history_for_prompt(self) -> Optional[str]:
-        """Build formatted chat history for the conversation"""
-        if len(self.user_messages) == 0:
-            return None
+        _conversation: Optional[ConversationRow] = None
+
+        if self.storage is not None:
+            logger.debug("Initializing storage")
+            self.storage.create()
 
-        chat_history = ""
-        chat_history_messages: List[Message] = []
-        for message in self.user_messages[::-1]:
-            if message.role == "user":
-                chat_history_messages.insert(0, message)
-            if message.role == "assistant" and self.include_responses_in_chat_history:
-                chat_history_messages.insert(0, message)
-            if len(chat_history_messages) >= self.max_chat_history_messages:
-                break
-
-        for message in chat_history_messages:
-            if message.role == "user":
-                chat_history += "\n---\n"
-            chat_history += f"{message.role.upper()}: {message.content}\n"
-        return chat_history
+            if self.id is not None:
+                logger.debug(f"Reading conversation: {self.id}")
+                # If the conversation ID is already set, read the conversation from the database
+                _conversation = self.storage.read_conversation(conversation_id=self.id, user_id=self.user_id)
+                if _conversation is None:
+                    raise Exception(f"Conversation not found: {self.id}")
+                logger.debug(f"Conversation found: {self.id}")
+            else:
+                logger.debug("Creating new conversation")
+                # If the conversation ID is not set, create a new conversation in the database
+                _conversation = self.storage.upsert_conversation(conversation=self.conversation_row)
+                if _conversation is None:
+                    raise Exception("Failed to create conversation")
+                logger.debug(f"Created conversation: {_conversation.id}")
 
-    def load_knowledge_base(self, recreate: bool = False) -> None:
-        """Loads the knowledge base"""
-        if self.knowledge_base is None:
-            return
-        self.knowledge_base.load_knowledge_base(recreate=recreate)
+        if _conversation is not None:
+            self.conversation_row = _conversation
+
+        return self.id
 
     def get_system_prompt(self) -> str:
-        """Build the system prompt for the conversation"""
+        """Return the system prompt for the conversation"""
 
         if self.system_prompt:
             return "\n".join([line.strip() for line in self.system_prompt.split("\n")])
 
         _system_prompt = ""
         if self.llm_name:
             _system_prompt += f"You are a chatbot named '{self.llm_name}'"
@@ -111,16 +151,17 @@
             _system_prompt += f"that is designed to help a '{self.user_persona}' with their work.\n"
         else:
             _system_prompt += "that is designed to help a user with their work.\n"
 
         _system_prompt += "If you don't know the answer, say 'I don't know'. You can ask follow up questions if needed."
         return _system_prompt
 
-    def get_relevant_information(self, question: str) -> Optional[str]:
-        """Get relevant information for answering a question"""
+    def get_references(self, question: str) -> Optional[str]:
+        """Return relevant information from the knowledge base"""
+
         if self.knowledge_base is None:
             return None
 
         relevant_docs: List[Document] = self.knowledge_base.search(query=question)
         relevant_info = ""
         for doc in relevant_docs:
             relevant_info += f"---\n{doc.content}\n"
@@ -130,89 +171,98 @@
                 ref = f"Title: {doc_name}"
                 if doc_page:
                     ref += f", Page: {doc_page}"
                 relevant_info += f"Reference: {ref}\n"
             relevant_info += "---\n"
         return relevant_info
 
-    def get_user_prompt(self, question: str) -> str:
-        """Build the user prompt for the conversation"""
+    def get_user_prompt(
+        self, question: str, references: Optional[str] = None, chat_history: Optional[str] = None
+    ) -> str:
+        """Build the user prompt given a question, references and chat_history"""
 
-        _user_prompt = "Your task is to answer the following question in the best way possible.\n"
+        _user_prompt = "Your task is to answer the following question "
+        if self.user_persona:
+            _user_prompt += f"for a '{self.user_persona}' "
+        _user_prompt += "using the following information:\n"
         # Add question to the prompt
         _user_prompt += f"\nQuestion: {question}\n"
 
-        # Add context to prompt
-        relevant_info = self.get_relevant_information(question=question)
-        if relevant_info:
+        # Add relevant_information to prompt
+        if references:
             _user_prompt += f"""
-                You have access to the following information that you can use to answer the question if it helps.
-                START OF INFORMATION
+                You can use the following references if they help you answer the question.
+                If you use the information from the references, please cite them as a bulleted list at the end.
+                START OF REFERENCES
                 ```
-                {relevant_info}
+                {references}
                 ```
-                END OF INFORMATION
+                END OF REFERENCES
                 """
 
         # Add chat history to prompt
-        chat_history = self.get_chat_history_for_prompt()
         if chat_history:
             _user_prompt += f"""
-                You have access to the following chat history that you can use to answer the question if it helps.
+                You can use the following chat history if it helps you answer the question.
                 START OF CHAT HISTORY
                 ```
                 {chat_history}
                 ```
                 END OF CHAT HISTORY
                 """
 
-        _user_prompt += "\nRemember, your task is to answer the following question:\n"
+        _user_prompt += "\nRemember, your task is to answer the following question using the provided information:\n"
         _user_prompt += f"Question: {question}\n"
 
+        # Return the user prompt after removing newlines and indenting
         return "\n".join([line.strip() for line in _user_prompt.split("\n")])
 
     def review(self, question: str) -> Iterator[str]:
         logger.debug(f"Reviewing: {question}")
 
+        # Build the system prompt
         system_prompt = self.get_system_prompt()
-        user_prompt = self.get_user_prompt(question=question)
 
-        # Create messages
-        messages: List[Message] = [
-            Message(role="system", content=system_prompt),
-            Message(role="user", content=user_prompt),
-        ]
-
-        # Update user_messages and llm_messages
-        # Add the question to user_messages
-        self.user_messages.append(Message(role="user", content=question))
-        # Add the system prompt to llm_messages if needed
-        if len(self.llm_messages) == 0:
-            self.llm_messages.append(Message(role="system", content=system_prompt))
-        # Add the user prompt to llm_messages
-        self.llm_messages.append(Message(role="user", content=user_prompt))
+        # Build the user prompt
+        references = self.get_references(question=question)
+        chat_history = self.history.get_formatted_history() if self.add_history_to_prompt else None
+        user_prompt = self.get_user_prompt(question=question, references=references, chat_history=chat_history)
+
+        # Create messages for the LLM
+        system_message = Message(role="system", content=system_prompt)
+        user_message = Message(role="user", content=user_prompt)
+        messages: List[Message] = [system_message, user_message]
+
+        # Add messages to the history
+        # Add the system prompt to the history - only added if this is the first message to the LLM
+        self.history.add_system_prompt(message=system_message)
+        # Add user question to the history - this is added to the chat history
+        self.history.add_user_question(message=Message(role="user", content=question))
+        # Add user prompt to the history - this is added to the llm history
+        self.history.add_user_prompt(message=user_message)
+        # Add references to the history
+        if references:
+            self.history.add_references(references=References(question=question, references=references))
 
         # Log messages
-        for message in messages:
+        for message in self.history.chat_history:
             logger.debug(f"{message.role}: {message.content}")
 
         # Generate response
         response = ""
         response_tokens = 0
         for delta in self.llm.streaming_response(messages=[m.model_dump(exclude_none=True) for m in messages]):
             response += delta
             response_tokens += 1
             yield response
 
         logger.debug(f"Response: {response}")
 
-        # Add response to user_messages
-        self.user_messages.append(Message(role="assistant", content=response))
-        # Add response to llm_messages
-        self.llm_messages.append(Message(role="assistant", content=response))
+        # Add response to the history - this is added to the chat and llm history
+        self.history.add_llm_response(message=Message(role="assistant", content=response))
 
         # Add response tokens to usage data
         if "response_tokens" in self.usage_data:
             self.usage_data["response_tokens"] += response_tokens
         else:
             self.usage_data["response_tokens"] = response_tokens
 
@@ -221,53 +271,18 @@
             self.usage_data["questions"] += 1
         else:
             self.usage_data["questions"] = 1
 
         # Save conversation to storage
         self.save_to_storage()
 
-    def read_from_storage(self) -> None:
-        """Read existing conversation from storage"""
-        if self.storage is None:
-            return
-
-        existing_conversation = self.storage.read(user_id=self.user_id)
-        if existing_conversation is None:
-            logger.debug(f"No conversation found for user: {self.user_id}")
-            return
-
-        logger.debug(f"Found existing conversation for user: {self.user_id}")
-        # Values that should not be overwritten if provided
-        if self.user_persona is None and existing_conversation.get("user_persona") is not None:
-            self.user_persona = existing_conversation["user_persona"]
-        if self.user_data is None and existing_conversation.get("user_data") is not None:
-            self.user_data = existing_conversation["user_data"]
-
-        # Update conversation using existing conversation
-        user_chat_history = existing_conversation.get("user_chat_history")
-        if user_chat_history is not None and len(user_chat_history) > 0:
-            self.user_messages = [Message(**message) for message in user_chat_history]
-        llm_chat_history = existing_conversation.get("llm_chat_history")
-        if llm_chat_history is not None and len(llm_chat_history) > 0:
-            self.llm_messages = [Message(**message) for message in llm_chat_history]
-        if existing_conversation.get("usage_data") is not None:
-            self.usage_data = existing_conversation["usage_data"]
-
     def save_to_storage(self) -> None:
         """Save the conversation to the storage"""
         if self.storage is None:
             return
-        self.storage.upsert(
-            user_id=self.user_id,
-            user_persona=self.user_persona,
-            user_data=self.user_data,
-            user_chat_history=self.user_chat_history,
-            llm_chat_history=self.llm_chat_history,
-            usage_data=self.usage_data,
-        )
+        self.storage.upsert_conversation(conversation=self.conversation_row)
 
     def end(self) -> None:
         """End the conversation"""
-        self.user_messages = []
-        self.llm_messages = []
         if self.storage is not None:
-            self.storage.end(user_id=self.user_id)
+            if self.id is not None:
+                self.storage.end_conversation(conversation_id=self.id, user_id=self.user_id)
```

### Comparing `phidata-2.0.0.dev6/phi/llm/conversation/storage/postgres.py` & `phidata-2.0.0.dev7/phi/vectordb/pgvector/pgvector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,152 @@
-from typing import Optional, List, Dict, Any
+from typing import Optional, List
+
 try:
-    from sqlalchemy.orm import Session, sessionmaker
-    from sqlalchemy.schema import MetaData, Table
-    from sqlalchemy.sql.expression import text, select
-    from sqlalchemy.engine import create_engine, Engine
     from sqlalchemy.dialects import postgresql
-    from sqlalchemy.engine.row import Row
+    from sqlalchemy.engine import create_engine, Engine
+    from sqlalchemy.inspection import inspect
+    from sqlalchemy.orm import Session, sessionmaker
+    from sqlalchemy.schema import MetaData, Table, Column
+    from sqlalchemy.sql.expression import text
+    from sqlalchemy.types import DateTime, String
 except ImportError:
     raise ImportError("`sqlalchemy` not installed")
 
-from phi.llm.conversation.storage.base import ConversationStorage
+try:
+    from pgvector.sqlalchemy import Vector
+except ImportError:
+    raise ImportError("`pgvector` not installed")
+
+from phi.document import Document
+from phi.embedder import Embedder
+from phi.embedder.openai import OpenAIEmbedder
+from phi.vectordb.base import VectorDb
 from phi.utils.log import logger
 
 
-class PgConversationStorage(ConversationStorage):
+class PgVector(VectorDb):
     def __init__(
         self,
-        table_name: str,
+        collection: str,
         schema: Optional[str] = None,
         db_url: Optional[str] = None,
         db_engine: Optional[Engine] = None,
+        embedder: Optional[Embedder] = None,
     ):
         _engine: Optional[Engine] = db_engine
         if _engine is None and db_url is not None:
             _engine = create_engine(db_url)
 
         if _engine is None:
             raise ValueError("Must provide either db_url or db_engine")
 
+        # Collection attributes
+        self.collection: str = collection
+
         # Database attributes
-        self.table_name: str = table_name
         self.schema: Optional[str] = schema
         self.db_url: Optional[str] = db_url
         self.db_engine: Engine = _engine
         self.metadata: MetaData = MetaData(schema=self.schema)
 
+        # Embedder for embedding the document contents
+        self.embedder: Embedder = embedder or OpenAIEmbedder()
+        self.dimensions: int = self.embedder.dimensions
+
         # Database session
         self.Session: sessionmaker[Session] = sessionmaker(bind=self.db_engine)
 
         # Database table for the collection
         self.table: Table = self.get_table()
 
-        if self.schema is not None:
-            logger.debug(f"Creating schema: {self.schema}")
-            with self.Session() as sess:
-                with sess.begin():
-                    sess.execute(text(f"create schema if not exists {self.schema};"))
-            logger.debug("Schema created")
-
     def get_table(self) -> Table:
-        from sqlalchemy.schema import Column
-        from sqlalchemy.types import DateTime, String, BigInteger
-
         return Table(
-            self.table_name,
+            self.collection,
             self.metadata,
-            Column("id", BigInteger, primary_key=True, autoincrement=True),
-            Column("user_id", String),
-            Column("user_persona", String),
-            Column("user_data", postgresql.JSONB),
-            Column("is_active", postgresql.BOOLEAN, server_default=text("true")),
-            Column("user_chat_history", postgresql.JSONB),
-            Column("llm_chat_history", postgresql.JSONB),
-            Column("usage_data", postgresql.JSONB),
+            Column("name", String),
+            Column("meta_data", postgresql.JSONB, server_default=text("'{}'::jsonb")),
+            Column("content", postgresql.TEXT),
+            Column("embedding", Vector(self.dimensions)),
+            Column("usage", postgresql.JSONB),
             Column("created_at", DateTime(timezone=True), server_default=text("now()")),
             Column("updated_at", DateTime(timezone=True), onupdate=text("now()")),
             extend_existing=True,
         )
 
     def table_exists(self) -> bool:
-        from sqlalchemy import inspect
-
         logger.debug(f"Checking if table exists: {self.table.name}")
         try:
-            return inspect(self.db_engine).has_table(self.table.name)
+            return inspect(self.db_engine).has_table(self.table.name, schema=self.schema)
         except Exception as e:
             logger.error(e)
             return False
 
     def create(self) -> None:
         if not self.table_exists():
-            logger.debug(f"Creating table: {self.table_name}")
+            with self.Session() as sess:
+                with sess.begin():
+                    logger.debug("Creating extension: vector")
+                    sess.execute(text("create extension if not exists vector;"))
+                    if self.schema is not None:
+                        sess.execute(text(f"create schema if not exists {self.schema};"))
+            logger.debug(f"Creating table: {self.collection}")
             self.table.create(self.db_engine)
 
-    def _read(self, session: Session, user_id: str) -> Optional[Row[Any]]:
-        stmt = select(self.table)\
-            .where(self.table.c.user_id == user_id)\
-            .where(self.table.c.is_active == True)
-        result = session.execute(stmt).first()
-        return result
-
-    def read(self, user_id: str) -> Optional[Dict[str, Any]]:
-        with self.Session() as sess:
-            with sess.begin():
-                existing_row: Optional[Row[Any]] = self._read(sess, user_id)
-                return existing_row._asdict() if existing_row is not None else None
-
-    def upsert(
-        self,
-        user_id: str,
-        user_persona: Optional[str] = None,
-        user_data: Optional[Dict[str, Any]] = None,
-        user_chat_history: Optional[List[Dict[str, Any]]] = None,
-        llm_chat_history: Optional[List[Dict[str, Any]]] = None,
-        usage_data: Optional[Dict[str, Any]] = None
-    ) -> None:
+    def insert(self, documents: List[Document]) -> None:
         with self.Session() as sess:
             with sess.begin():
-                existing_row: Optional[Row[Any]] = self._read(sess, user_id)
-                if existing_row is None:
-                    insert_stmt = postgresql.insert(self.table).values(
-                        user_id=user_id,
-                        user_persona=user_persona,
-                        user_data=user_data,
-                        user_chat_history=user_chat_history,
-                        llm_chat_history=llm_chat_history,
-                        usage_data=usage_data,
+                for document in documents:
+                    document.embed(embedder=self.embedder)
+                    stmt = postgresql.insert(self.table).values(
+                        name=document.name,
+                        meta_data=document.meta_data,
+                        content=document.content,
+                        embedding=document.embedding,
+                        usage=document.usage,
                     )
-                    sess.execute(insert_stmt)
-                else:
-                    update_stmt = self.table.update()\
-                        .where(self.table.c.user_id == user_id)\
-                        .values(
-                            user_persona=user_persona,
-                            user_data=user_data,
-                            user_chat_history=user_chat_history,
-                            llm_chat_history=llm_chat_history,
-                            usage_data=usage_data,
-                        )
-                    sess.execute(update_stmt)
+                    sess.execute(stmt)
+                    logger.debug(f"Inserted document: {document.name} ({document.meta_data})")
+
+    def search(self, query: str, num_documents: int = 5) -> List[Document]:
+        from sqlalchemy.sql.expression import select
+
+        query_embedding = self.embedder.get_embedding(query)
+        if query_embedding is None:
+            logger.error(f"Error getting embedding for Query: {query}")
+            return []
+
+        columns = [
+            self.table.c.name,
+            self.table.c.meta_data,
+            self.table.c.content,
+            self.table.c.embedding,
+            self.table.c.usage,
+        ]
+
+        stmt = select(*columns).order_by(self.table.c.embedding.max_inner_product(query_embedding)).limit(num_documents)
+        logger.debug(f"Query: {stmt}")
 
-    def end(self, user_id: str) -> None:
+        # Get neighbors
         with self.Session() as sess:
             with sess.begin():
-                existing_row: Optional[Row[Any]] = self._read(sess, user_id)
-                if existing_row is not None:
-                    stmt = self.table.update()\
-                        .where(self.table.c.user_id == user_id)\
-                        .values(is_active=False)
-                    sess.execute(stmt)
+                neighbors = sess.execute(stmt).fetchall() or []
+
+        # Build search results
+        search_results: List[Document] = []
+        for neighbor in neighbors:
+            search_results.append(
+                Document(
+                    name=neighbor.name,
+                    meta_data=neighbor.meta_data,
+                    content=neighbor.content,
+                    embedder=self.embedder,
+                    embedding=neighbor.embedding,
+                    usage=neighbor.usage,
+                )
+            )
+
+        return search_results
 
     def delete(self) -> None:
         if self.table_exists():
-            logger.debug(f"Deleting table: {self.table_name}")
+            logger.debug(f"Deleting table: {self.collection}")
             self.table.drop(self.db_engine)
```

### Comparing `phidata-2.0.0.dev6/phi/llm/knowledge/pdf.py` & `phidata-2.0.0.dev7/phi/llm/knowledge/pdf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from pathlib import Path
 from typing import Union, List, Optional, Iterator
 
 from phi.document import Document
 from phi.document.reader.pdf import PDFReader
-from phi.llm.knowledge.base import KnowledgeBase
+from phi.llm.knowledge.base import LLMKnowledgeBase
 from phi.vectordb import VectorDb
 from phi.utils.log import logger
 
 
-class PDFKnowledgeBase(KnowledgeBase):
-    def __init__(
-        self, path: Union[str, Path], reader: Optional[PDFReader] = None, vector_db: Optional[VectorDb] = None
-    ):
-        if not (isinstance(path, str) or isinstance(path, Path)):
-            raise TypeError(f"Path must be of type str or Path, got: {type(path)}")
-
-        self.path: Path = Path(path) if isinstance(path, str) else path
-        self.reader: PDFReader = reader or PDFReader()
-        self.vector_db: Optional[VectorDb] = vector_db
+class PDFKnowledgeBase(LLMKnowledgeBase):
+    path: Union[str, Path]
+    reader: PDFReader = PDFReader()
+    vector_db: Optional[VectorDb] = None
+    relevant_documents: int = 5
 
     @property
     def document_lists(self) -> Iterator[List[Document]]:
         """Iterate over PDFs and return a list of document in each PDF
         Returns:
             Iterator[List[Document]]: Iterator over List of documents in each PDF
         """
 
-        if self.path.exists() and self.path.is_dir():
-            for _pdf in self.path.glob("*.pdf"):
+        pdf_dir_path: Path = Path(self.path) if isinstance(self.path, str) else self.path
+
+        if pdf_dir_path.exists() and pdf_dir_path.is_dir():
+            for _pdf in pdf_dir_path.glob("*.pdf"):
                 yield self.reader.read(path=_pdf)
-        elif self.path.exists() and self.path.is_file() and self.path.suffix == ".pdf":
-            yield self.reader.read(path=self.path)
+        elif pdf_dir_path.exists() and pdf_dir_path.is_file() and pdf_dir_path.suffix == ".pdf":
+            yield self.reader.read(path=pdf_dir_path)
 
-    def search(self, query: str, num_documents: int = 5) -> List[Document]:
+    def search(self, query: str, num_documents: Optional[int] = None) -> List[Document]:
         """Return all relevant documents matching the query"""
         if self.vector_db is None:
             logger.warning("No vector db provided")
             return []
 
-        logger.debug(f"Getting relevant documents for query: {query}")
-        return self.vector_db.search(query=query, num_documents=num_documents)
+        _num_documents = num_documents or self.relevant_documents
+        logger.debug(f"Getting {_num_documents} relevant documents for query: {query}")
+        return self.vector_db.search(query=query, num_documents=_num_documents)
 
-    def load_knowledge_base(self, recreate: bool = False) -> None:
+    def load(self, recreate: bool = False) -> None:
         """Load the knowledge base to vector db"""
         if self.vector_db is None:
             logger.warning("No vector db provided")
             return
 
         if recreate:
             logger.debug("Recreating collection")
```

### Comparing `phidata-2.0.0.dev6/phi/llm/openai.py` & `phidata-2.0.0.dev7/phi/llm/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/common.py` & `phidata-2.0.0.dev7/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/defaults.py` & `phidata-2.0.0.dev7/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/filesystem.py` & `phidata-2.0.0.dev7/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/git.py` & `phidata-2.0.0.dev7/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/json_io.py` & `phidata-2.0.0.dev7/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/load_env.py` & `phidata-2.0.0.dev7/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/log.py` & `phidata-2.0.0.dev7/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/pickle.py` & `phidata-2.0.0.dev7/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/py_io.py` & `phidata-2.0.0.dev7/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/pyproject.py` & `phidata-2.0.0.dev7/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/resource_filter.py` & `phidata-2.0.0.dev7/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/utils/yaml_io.py` & `phidata-2.0.0.dev7/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/vectordb/base.py` & `phidata-2.0.0.dev7/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/workspace/config.py` & `phidata-2.0.0.dev7/phi/workspace/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Optional, List, Any
 
 from pydantic import BaseModel, ConfigDict
 
 from phi.infra.enums import InfraType
 from phi.infra.resource.group import InfraResourceGroup
-from phi.schemas.workspace import WorkspaceSchema
+from phi.api.schemas.workspace import WorkspaceSchema
 from phi.workspace.settings import WorkspaceSettings
 from phi.utils.dttm import current_datetime_utc
 from phi.utils.log import logger
 
 
 class WorkspaceConfig(BaseModel):
     """The WorkspaceConfig stores data for a phidata workspace."""
```

### Comparing `phidata-2.0.0.dev6/phi/workspace/helpers.py` & `phidata-2.0.0.dev7/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phi/workspace/operator.py` & `phidata-2.0.0.dev7/phi/workspace/operator.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     print_heading,
     print_info,
     print_subheading,
     log_config_not_available_msg,
 )
 from phi.infra.enums import InfraType
 from phi.infra.resource.group import InfraResourceGroup
-from phi.schemas.workspace import WorkspaceSchema
+from phi.api.schemas.workspace import WorkspaceSchema
 from phi.workspace.config import WorkspaceConfig
 from phi.workspace.enums import WorkspaceStarterTemplate
 from phi.utils.log import logger
 
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.api_app: "api-app",
     WorkspaceStarterTemplate.llm_app: "llm-app",
@@ -33,15 +33,17 @@
     WorkspaceStarterTemplate.streamlit_app: "https://github.com/phihq/streamlit-app.git",
     WorkspaceStarterTemplate.data_platform: "https://github.com/phihq/data-platform.git",
     WorkspaceStarterTemplate.spark_data_platform: "https://github.com/phihq/spark-data-platform.git",
     WorkspaceStarterTemplate.snowflake_data_platform: "https://github.com/phihq/snowflake-data-platform.git",
 }
 
 
-def create_workspace(name: Optional[str] = None, template: Optional[str] = None, url: Optional[str] = None) -> bool:
+async def create_workspace(
+    name: Optional[str] = None, template: Optional[str] = None, url: Optional[str] = None
+) -> None:
     """Creates a new workspace.
 
     This function clones a template or url on the users machine at the path:
         cwd/name
     """
     import git
     from shutil import copytree
@@ -54,20 +56,25 @@
     from phi.utils.git import GitCloneProgress
 
     current_dir: Path = Path(".").resolve()
 
     # Phi should be initialized before creating a workspace
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if not phi_config:
-        initialize_phi()
+        init_success = await initialize_phi()
+        if not init_success:
+            from phi.cli.console import log_phi_init_failed_msg
+
+            log_phi_init_failed_msg()
+            return
         phi_config = PhiCliConfig.from_saved_config()
         # If phi_config is still None, throw an error
         if not phi_config:
             log_config_not_available_msg()
-            return False
+            return
 
     ws_name: Optional[str] = name
     repo_to_clone: Optional[str] = url
     ws_template = WorkspaceStarterTemplate.api_app
     templates = list(WorkspaceStarterTemplate.__members__.values())
 
     if repo_to_clone is None:
@@ -105,44 +112,44 @@
             default_ws_name = TEMPLATE_TO_NAME_MAP.get(ws_template, "api-app")
 
         # Ask user for workspace name if not provided
         ws_name = Prompt.ask("Workspace Name", default=default_ws_name)
 
     if ws_name is None:
         logger.error("Workspace name is required")
-        return False
+        return
     if repo_to_clone is None:
         logger.error("URL or Template is required")
-        return False
+        return
 
     # Check if a workspace with the same name exists
     existing_ws_config: Optional[WorkspaceConfig] = phi_config.get_ws_config_by_name(ws_name)
     if existing_ws_config is not None:
         logger.error(f"Found existing record for a workspace: {ws_name}")
         delete_existing_ws_config = typer.confirm("Replace existing record?", default=True)
         if delete_existing_ws_config:
-            phi_config.delete_ws(ws_name)
+            await phi_config.delete_ws(ws_name)
         else:
-            return False
+            return
 
     # Check if we can create the workspace in the current dir
     ws_root_path: Path = current_dir.joinpath(ws_name)
     if ws_root_path.exists():
         logger.error(f"Directory {ws_root_path} exists, please delete directory or choose another name for workspace")
-        return False
+        return
 
     print_info(f"Creating {str(ws_root_path)}")
     logger.debug("Cloning: {}".format(repo_to_clone))
     try:
         _cloned_git_repo: git.Repo = git.Repo.clone_from(
             repo_to_clone, str(ws_root_path), progress=GitCloneProgress()  # type: ignore
         )
     except Exception as e:
         logger.error(e)
-        return False
+        return
 
     # Remove existing .git folder
     _dot_git_folder = ws_root_path.joinpath(".git")
     _dot_git_exists = _dot_git_folder.exists()
     if _dot_git_exists:
         logger.debug(f"Deleting {_dot_git_folder}")
         try:
@@ -169,18 +176,18 @@
             str(workspace_secrets_dir),
         )
     except Exception as e:
         logger.warning(f"Could not create workspace/secrets: {e}")
         logger.warning("Please manually copy workspace/example_secrets to workspace/secrets")
 
     print_info(f"Your new workspace is available at {str(ws_root_path)}\n")
-    return setup_workspace(ws_root_path=ws_root_path)
+    await setup_workspace(ws_root_path=ws_root_path)
 
 
-def setup_workspace(ws_root_path: Path) -> bool:
+async def setup_workspace(ws_root_path: Path) -> None:
     """Setup a phi workspace at `ws_root_path`.
 
     1. Validate pre-requisites
     1.1 Check ws_root_path is valid
     1.2 Check PhiCliConfig is valid
     1.3 Validate WorkspaceConfig is available
     1.4 Set workspace as active
@@ -203,23 +210,28 @@
     ######################################################
     ######################################################
     # 1.1 Check ws_root_path is valid
     ######################################################
     _ws_is_valid: bool = ws_root_path is not None and ws_root_path.exists() and ws_root_path.is_dir()
     if not _ws_is_valid:
         logger.error("Invalid directory: {}".format(ws_root_path))
-        return False
+        return
 
     ######################################################
     # 1.2 Check PhiCliConfig is valid
     ######################################################
     phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
     if not phi_config:
         # Phidata should be initialized before workspace setup
-        initialize_phi()
+        init_success = await initialize_phi()
+        if not init_success:
+            from phi.cli.console import log_phi_init_failed_msg
+
+            log_phi_init_failed_msg()
+            return
         phi_config = PhiCliConfig.from_saved_config()
         # If phi_config is still None, throw an error
         if not phi_config:
             raise Exception("Failed to initialize phi")
 
     ######################################################
     # 1.3 Validate WorkspaceConfig is available
@@ -243,15 +255,15 @@
         logger.debug(f"Found workspace {ws_config.ws_name}")
         phi_config.refresh_ws_config(ws_config.ws_name)
 
     # If the ws_config is still None it means the workspace is corrupt
     if ws_config is None:
         logger.error(f"Could not add workspace from: {ws_root_path}")
         logger.error("Please try again")
-        return False
+        return
 
     ######################################################
     # 1.4 Set workspace as active
     ######################################################
     phi_config.active_ws_name = ws_config.ws_name
     is_active_ws = True
 
@@ -268,43 +280,43 @@
         # If a ws_schema exists for this workspace, this workspace is synced with the api
         ws_schema: Optional[WorkspaceSchema] = ws_config.ws_schema
 
         ######################################################
         # 2.1 Create WorkspaceSchema for NEW WORKSPACE
         ######################################################
         if ws_schema is None:
-            from phi.api.workspace import create_workspace
+            from phi.api.workspace import create_workspace_for_user
 
             # If ws_schema is None, this is a NEWLY CREATED WORKSPACE.
             # We make a call to the api to create a new ws_schema
             logger.debug("Creating ws_schema for new workspace")
             logger.debug("ws_name: {}".format(ws_config.ws_name))
             logger.debug("is_active_ws: {}".format(is_active_ws))
 
-            ws_schema = create_workspace(
+            ws_schema = await create_workspace_for_user(
                 user=phi_config.user,
                 workspace=WorkspaceSchema(
                     ws_name=ws_config.ws_name,
                     is_primary_ws_for_user=is_active_ws,
                 ),
             )
             if ws_schema is not None:
                 phi_config.update_ws_config(ws_name=ws_config.ws_name, ws_schema=ws_schema)
         ######################################################
         # 2.2 Update WorkspaceSchema for EXISTING WORKSPACE
         ######################################################
         else:
-            from phi.api.workspace import update_workspace
+            from phi.api.workspace import update_workspace_for_user
 
             logger.debug("Updating ws_schema for existing workspace")
             logger.debug("ws_name: {}".format(ws_config.ws_name))
             logger.debug("is_active_ws: {}".format(is_active_ws))
 
             ws_schema.is_primary_ws_for_user = is_active_ws
-            ws_schema_updated = update_workspace(
+            ws_schema_updated = await update_workspace_for_user(
                 user=phi_config.user,
                 workspace=ws_schema,
             )
             if ws_schema_updated is not None:
                 # Update the ws_schema for this workspace.
                 phi_config.update_ws_config(ws_name=ws_config.ws_name, ws_schema=ws_schema_updated)
 
@@ -323,25 +335,23 @@
         print_info("2. Stop workspace:")
         print_info("\tphi ws down")
         if ws_config.workspace_settings is not None:
             scripts_dir = ws_config.workspace_settings.scripts_dir
             install_ws_file = f"sh {ws_root_path}/{scripts_dir}/install.sh"
             print_info("3. Install workspace dependencies:")
             print_info(f"\t{install_ws_file}")
-        return True
     else:
         print_info("Workspace setup unsuccessful. Please try again.")
-        return False
 
     ######################################################
     ## End Workspace setup
     ######################################################
 
 
-def start_workspace(
+async def start_workspace(
     ws_config: WorkspaceConfig,
     target_env: Optional[str] = None,
     target_infra: Optional[InfraType] = None,
     target_group: Optional[str] = None,
     target_name: Optional[str] = None,
     target_type: Optional[str] = None,
     dry_run: Optional[bool] = False,
@@ -394,15 +404,15 @@
     if num_rgs_to_create == num_rgs_created:
         if not dry_run:
             print_subheading("Workspace started")
     else:
         logger.error("Workspace start failed")
 
 
-def stop_workspace(
+async def stop_workspace(
     ws_config: WorkspaceConfig,
     target_env: Optional[str] = None,
     target_infra: Optional[InfraType] = None,
     target_group: Optional[str] = None,
     target_name: Optional[str] = None,
     target_type: Optional[str] = None,
     dry_run: Optional[bool] = False,
@@ -452,15 +462,15 @@
     if num_rgs_to_delete == num_rgs_deleted:
         if not dry_run:
             print_subheading("Workspace stopped")
     else:
         logger.error("Workspace stop failed")
 
 
-def update_workspace(
+async def update_workspace(
     ws_config: WorkspaceConfig,
     target_env: Optional[str] = None,
     target_infra: Optional[InfraType] = None,
     target_group: Optional[str] = None,
     target_name: Optional[str] = None,
     target_type: Optional[str] = None,
     dry_run: Optional[bool] = False,
@@ -510,14 +520,106 @@
     if num_rgs_to_update == num_rgs_updated:
         if not dry_run:
             print_subheading("Workspace updated")
     else:
         logger.error("Workspace update failed")
 
 
-def delete_workspace(phi_config: PhiCliConfig, ws_to_delete: Optional[List[str]]) -> None:
+async def delete_workspace(phi_config: PhiCliConfig, ws_to_delete: Optional[List[str]]) -> None:
     if ws_to_delete is None or len(ws_to_delete) == 0:
         print_heading("No workspaces to delete")
         return
 
     for ws in ws_to_delete:
-        phi_config.delete_ws(ws_name=ws)
+        await phi_config.delete_ws(ws_name=ws)
+
+
+async def set_workspace_as_active(ws_name: Optional[str], refresh: bool = True) -> None:
+    from phi.cli.operator import initialize_phi
+
+    ######################################################
+    ## 1. Validate Pre-requisites
+    ######################################################
+    ######################################################
+    # 1.1 Check PhiConf is valid
+    ######################################################
+    phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
+    if not phi_config:
+        # Phidata should be initialized before workspace setup
+        init_success = await initialize_phi()
+        if not init_success:
+            from phi.cli.console import log_phi_init_failed_msg
+
+            log_phi_init_failed_msg()
+            return
+        phi_config = PhiCliConfig.from_saved_config()
+        # If phi_config is still None, throw an error
+        if not phi_config:
+            raise Exception("Failed to initialize phi")
+
+    ######################################################
+    # 1.2 Check ws_root_path is valid
+    ######################################################
+    # By default, we assume this command is run from the workspace directory
+    ws_root_path: Optional[Path] = None
+    if ws_name is None:
+        # If the user does not provide a ws_name, that implies `phi set` is ran from
+        # the workspace directory.
+        ws_root_path = Path(".").resolve()
+    else:
+        # If the user provides a workspace name manually, we find the dir for that ws
+        ws_root_path = phi_config.get_ws_root_path_by_name(ws_name)
+        if ws_root_path is None:
+            logger.error(f"Could not find workspace {ws_name}")
+            return
+
+    ws_dir_is_valid: bool = ws_root_path is not None and ws_root_path.exists() and ws_root_path.is_dir()
+    if not ws_dir_is_valid:
+        logger.error("Invalid workspace directory: {}".format(ws_root_path))
+        return
+
+    ######################################################
+    # 1.3 Validate PhiWsData is available i.e. a workspace is available at this directory
+    ######################################################
+    logger.debug(f"Checking for a workspace at path: {ws_root_path}")
+    active_ws_config: Optional[WorkspaceConfig] = phi_config.get_ws_config_by_path(ws_root_path)
+    if active_ws_config is None:
+        # This happens when the workspace is not yet setup
+        print_info(f"Could not find a workspace at path: {ws_root_path}")
+        print_info("If this workspace has not been setup, please run `phi ws setup` from the workspace directory")
+        return
+
+    new_active_ws_name: str = active_ws_config.ws_name
+    print_heading(f"Setting workspace {new_active_ws_name} as active")
+    if refresh:
+        try:
+            phi_config.refresh_ws_config(new_active_ws_name)
+        except Exception as e:
+            logger.error("Could not refresh workspace config, please fix errors and try again")
+            logger.error(e)
+            return
+
+    ######################################################
+    # 1.4 Make api request if updating active workspace
+    ######################################################
+    logger.debug("Updating active workspace api")
+    if phi_config.user is not None:
+        ws_schema: Optional[WorkspaceSchema] = active_ws_config.ws_schema
+        if ws_schema is None:
+            logger.warning(f"Please setup {new_active_ws_name} by running `phi ws setup`")
+        else:
+            from phi.api.workspace import update_primary_workspace_for_user
+
+            updated_workspace_schema = await update_primary_workspace_for_user(
+                user=phi_config.user,
+                workspace=ws_schema,
+            )
+            if updated_workspace_schema is not None:
+                # Update the ws_schema for this workspace.
+                phi_config.update_ws_config(ws_name=new_active_ws_name, ws_schema=updated_workspace_schema)
+
+    ######################################################
+    ## 2. Set workspace as active
+    ######################################################
+    phi_config.active_ws_name = new_active_ws_name
+    print_info("Active workspace updated")
+    return
```

### Comparing `phidata-2.0.0.dev6/phi/workspace/settings.py` & `phidata-2.0.0.dev7/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/airflow/operators/empty.py` & `phidata-2.0.0.dev7/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_base.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_flower.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_manager.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_scheduler.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_webserver.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/airflow/airflow_worker.py` & `phidata-2.0.0.dev7/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/alertmanager/alertmanager.py` & `phidata-2.0.0.dev7/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/amundsen/frontend.py` & `phidata-2.0.0.dev7/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/amundsen/metadata.py` & `phidata-2.0.0.dev7/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/amundsen/search.py` & `phidata-2.0.0.dev7/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/assistant/assistant.py` & `phidata-2.0.0.dev7/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/aws_app.py` & `phidata-2.0.0.dev7/phidata/app/aws_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/base_app.py` & `phidata-2.0.0.dev7/phidata/app/base_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/cadvisor/cadvisor.py` & `phidata-2.0.0.dev7/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/databox/databox.py` & `phidata-2.0.0.dev7/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/db/base_db.py` & `phidata-2.0.0.dev7/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/django/django_app.py` & `phidata-2.0.0.dev7/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/django/django_backup.py` & `phidata-2.0.0.dev7/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/docker_app.py` & `phidata-2.0.0.dev7/phidata/app/docker_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/elastic/elastic_app.py` & `phidata-2.0.0.dev7/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/elasticsearch/elasticsearch.py` & `phidata-2.0.0.dev7/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/fastapi/fastapi_server.py` & `phidata-2.0.0.dev7/phidata/app/fastapi/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/grafana/grafana.py` & `phidata-2.0.0.dev7/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/group.py` & `phidata-2.0.0.dev7/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/jupyter/jupyter.py` & `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/jupyter/jupyter_hub.py` & `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/jupyter/jupyter_lab.py` & `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/k8s/app.py` & `phidata-2.0.0.dev7/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/k8s/dir.py` & `phidata-2.0.0.dev7/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/k8s/url.py` & `phidata-2.0.0.dev7/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/k8s_app.py` & `phidata-2.0.0.dev7/phidata/app/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/mysql/mysql_db.py` & `phidata-2.0.0.dev7/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/neo4j/neo4j.py` & `phidata-2.0.0.dev7/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/nodeexporter/nodeexporter.py` & `phidata-2.0.0.dev7/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/phidata_app.py` & `phidata-2.0.0.dev7/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/postgres/postgres_db.py` & `phidata-2.0.0.dev7/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/prometheus/prometheus.py` & `phidata-2.0.0.dev7/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/qdrant/qdrant.py` & `phidata-2.0.0.dev7/phidata/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/redis/redis.py` & `phidata-2.0.0.dev7/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/redis/stack.py` & `phidata-2.0.0.dev7/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/server/api_server.py` & `phidata-2.0.0.dev7/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/server/server_base.py` & `phidata-2.0.0.dev7/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/spark/spark_base.py` & `phidata-2.0.0.dev7/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/spark/spark_driver.py` & `phidata-2.0.0.dev7/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/spark/spark_worker.py` & `phidata-2.0.0.dev7/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/streamlit/streamlit_app.py` & `phidata-2.0.0.dev7/phidata/app/streamlit/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/superset/superset_base.py` & `phidata-2.0.0.dev7/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/superset/superset_init.py` & `phidata-2.0.0.dev7/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/superset/superset_webserver.py` & `phidata-2.0.0.dev7/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/superset/superset_worker.py` & `phidata-2.0.0.dev7/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/superset/superset_worker_beat.py` & `phidata-2.0.0.dev7/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/traefik/crds.py` & `phidata-2.0.0.dev7/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/traefik/ingress_route.py` & `phidata-2.0.0.dev7/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/app/traefik/router.py` & `phidata-2.0.0.dev7/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/asset/aws/aws_asset.py` & `phidata-2.0.0.dev7/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/asset/data_asset.py` & `phidata-2.0.0.dev7/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/asset/local/file.py` & `phidata-2.0.0.dev7/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/asset/local/local_asset.py` & `phidata-2.0.0.dev7/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/api_client.py` & `phidata-2.0.0.dev7/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/athena/query.py` & `phidata-2.0.0.dev7/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/config.py` & `phidata-2.0.0.dev7/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/create/iam/eks_admin_role.py` & `phidata-2.0.0.dev7/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/create/iam/role.py` & `phidata-2.0.0.dev7/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/driver.py` & `phidata-2.0.0.dev7/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/enums/manager_status.py` & `phidata-2.0.0.dev7/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/manager.py` & `phidata-2.0.0.dev7/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev7/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/athena/query.py` & `phidata-2.0.0.dev7/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/base.py` & `phidata-2.0.0.dev7/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ecs/container.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ecs/service.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev7/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/eks/addon.py` & `phidata-2.0.0.dev7/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev7/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev7/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev7/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev7/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/elb/listener.py` & `phidata-2.0.0.dev7/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev7/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev7/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev7/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/iam/group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/iam/policy.py` & `phidata-2.0.0.dev7/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/iam/role.py` & `phidata-2.0.0.dev7/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev7/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/secret/manager.py` & `phidata-2.0.0.dev7/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/secret/reader.py` & `phidata-2.0.0.dev7/phidata/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/types.py` & `phidata-2.0.0.dev7/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/resource/utils.py` & `phidata-2.0.0.dev7/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/s3/csv_dataset.py` & `phidata-2.0.0.dev7/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/s3/dataset.py` & `phidata-2.0.0.dev7/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/s3/dataset_base.py` & `phidata-2.0.0.dev7/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/s3/object.py` & `phidata-2.0.0.dev7/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/aws/worker.py` & `phidata-2.0.0.dev7/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/base.py` & `phidata-2.0.0.dev7/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/checks/check.py` & `phidata-2.0.0.dev7/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/checks/not_empty.py` & `phidata-2.0.0.dev7/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/constants.py` & `phidata-2.0.0.dev7/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/decorators/timer.py` & `phidata-2.0.0.dev7/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/decorators/validate_env.py` & `phidata-2.0.0.dev7/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/api_client.py` & `phidata-2.0.0.dev7/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/args.py` & `phidata-2.0.0.dev7/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/config.py` & `phidata-2.0.0.dev7/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/enums.py` & `phidata-2.0.0.dev7/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/manager.py` & `phidata-2.0.0.dev7/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/base.py` & `phidata-2.0.0.dev7/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/container.py` & `phidata-2.0.0.dev7/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/group.py` & `phidata-2.0.0.dev7/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/image.py` & `phidata-2.0.0.dev7/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/network.py` & `phidata-2.0.0.dev7/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/types.py` & `phidata-2.0.0.dev7/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/utils.py` & `phidata-2.0.0.dev7/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/resource/volume.py` & `phidata-2.0.0.dev7/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/utils/container.py` & `phidata-2.0.0.dev7/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/docker/worker.py` & `phidata-2.0.0.dev7/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/infra/args.py` & `phidata-2.0.0.dev7/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/infra/config.py` & `phidata-2.0.0.dev7/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/infra/resource.py` & `phidata-2.0.0.dev7/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/api_client.py` & `phidata-2.0.0.dev7/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/args.py` & `phidata-2.0.0.dev7/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/config.py` & `phidata-2.0.0.dev7/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/apps/v1/deployment.py` & `phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/common/port.py` & `phidata-2.0.0.dev7/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/config_map.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/container.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/namespace.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/secret.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/service.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/service_account.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/core/v1/volume.py` & `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-2.0.0.dev7/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/group.py` & `phidata-2.0.0.dev7/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/kubeconfig.py` & `phidata-2.0.0.dev7/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/enums/api_version.py` & `phidata-2.0.0.dev7/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/enums/kind.py` & `phidata-2.0.0.dev7/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/enums/manager_status.py` & `phidata-2.0.0.dev7/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/enums/pv.py` & `phidata-2.0.0.dev7/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/manager.py` & `phidata-2.0.0.dev7/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/base.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/config_map.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/container.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/namespace.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/secret.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/service.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/service_account.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/toleration.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/group.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/kubeconfig.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/types.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/resource/utils.py` & `phidata-2.0.0.dev7/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/utils/pod.py` & `phidata-2.0.0.dev7/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/k8s/worker.py` & `phidata-2.0.0.dev7/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/agent.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/chain.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/connection.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/loader.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/query.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/llm/duckdb/tool.py` & `phidata-2.0.0.dev7/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/product/data_product.py` & `phidata-2.0.0.dev7/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/local/csv.py` & `phidata-2.0.0.dev7/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/local/local_table.py` & `phidata-2.0.0.dev7/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/local/parquet.py` & `phidata-2.0.0.dev7/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/s3/csv.py` & `phidata-2.0.0.dev7/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/s3/parquet.py` & `phidata-2.0.0.dev7/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/s3/s3_table.py` & `phidata-2.0.0.dev7/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/sql/postgres.py` & `phidata-2.0.0.dev7/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/table/sql/sql_table.py` & `phidata-2.0.0.dev7/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/aws/athena/run_query.py` & `phidata-2.0.0.dev7/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/aws/emr/create_cluster.py` & `phidata-2.0.0.dev7/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/aws/emr/delete_cluster.py` & `phidata-2.0.0.dev7/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/aws/glue/start_crawler.py` & `phidata-2.0.0.dev7/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/decorator.py` & `phidata-2.0.0.dev7/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/download/s3/to_file.py` & `phidata-2.0.0.dev7/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/download/url/to_file.py` & `phidata-2.0.0.dev7/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/download/url/to_s3.py` & `phidata-2.0.0.dev7/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/download/url/to_sql.py` & `phidata-2.0.0.dev7/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/plot/sql/query.py` & `phidata-2.0.0.dev7/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/python_task.py` & `phidata-2.0.0.dev7/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/run/sql/query.py` & `phidata-2.0.0.dev7/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/task.py` & `phidata-2.0.0.dev7/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/task_relatives.py` & `phidata-2.0.0.dev7/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/upload/file/to_s3.py` & `phidata-2.0.0.dev7/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/task/upload/file/to_sql.py` & `phidata-2.0.0.dev7/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/types/airflow.py` & `phidata-2.0.0.dev7/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/types/context.py` & `phidata-2.0.0.dev7/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/types/phidata_runtime.py` & `phidata-2.0.0.dev7/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/common.py` & `phidata-2.0.0.dev7/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/compare.py` & `phidata-2.0.0.dev7/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/context.py` & `phidata-2.0.0.dev7/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/dttm.py` & `phidata-2.0.0.dev7/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/enums.py` & `phidata-2.0.0.dev7/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/env_file.py` & `phidata-2.0.0.dev7/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/env_var.py` & `phidata-2.0.0.dev7/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/filesystem.py` & `phidata-2.0.0.dev7/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/get_python_objects_from_module.py` & `phidata-2.0.0.dev7/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/json_io.py` & `phidata-2.0.0.dev7/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/k8s.py` & `phidata-2.0.0.dev7/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/log.py` & `phidata-2.0.0.dev7/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/print_table.py` & `phidata-2.0.0.dev7/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/workspace_path.py` & `phidata-2.0.0.dev7/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/utils/yaml_io.py` & `phidata-2.0.0.dev7/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/workflow/decorator.py` & `phidata-2.0.0.dev7/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/workflow/workflow.py` & `phidata-2.0.0.dev7/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/workflow/workflow_relatives.py` & `phidata-2.0.0.dev7/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/workspace/config.py` & `phidata-2.0.0.dev7/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata/workspace/settings.py` & `phidata-2.0.0.dev7/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev6/phidata.egg-info/PKG-INFO` & `phidata-2.0.0.dev7/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev6
+Version: 2.0.0.dev7
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev6 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev7 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev6/phidata.egg-info/SOURCES.txt` & `phidata-2.0.0.dev7/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 pyproject.toml
 setup.py
 phi/__init__.py
 phi/base.py
 phi/constants.py
 phi/api/__init__.py
 phi/api/client.py
-phi/api/helpers.py
 phi/api/routes.py
 phi/api/user.py
 phi/api/workspace.py
+phi/api/schemas/__init__.py
+phi/api/schemas/response.py
+phi/api/schemas/user.py
+phi/api/schemas/workspace.py
 phi/aws/__init__.py
 phi/aws/api_client.py
 phi/aws/app/__init__.py
 phi/aws/app/base.py
 phi/aws/app/context.py
 phi/aws/app/fastapi/__init__.py
 phi/aws/app/fastapi/fastapi.py
@@ -125,27 +128,27 @@
 phi/infra/resource/__init__.py
 phi/infra/resource/base.py
 phi/infra/resource/group.py
 phi/k8s/__init__.py
 phi/llm/__init__.py
 phi/llm/base.py
 phi/llm/openai.py
+phi/llm/schemas.py
 phi/llm/conversation/__init__.py
 phi/llm/conversation/conversation.py
 phi/llm/conversation/schemas.py
-phi/llm/conversation/storage/__init__.py
-phi/llm/conversation/storage/base.py
-phi/llm/conversation/storage/postgres.py
+phi/llm/history/__init__.py
+phi/llm/history/base.py
+phi/llm/history/simple.py
 phi/llm/knowledge/__init__.py
 phi/llm/knowledge/base.py
 phi/llm/knowledge/pdf.py
-phi/schemas/__init__.py
-phi/schemas/response.py
-phi/schemas/user.py
-phi/schemas/workspace.py
+phi/llm/storage/__init__.py
+phi/llm/storage/base.py
+phi/llm/storage/postgres.py
 phi/table/__init__.py
 phi/table/sql/__init__.py
 phi/table/sql/base.py
 phi/utils/__init__.py
 phi/utils/common.py
 phi/utils/defaults.py
 phi/utils/dttm.py
```

### Comparing `phidata-2.0.0.dev6/pyproject.toml` & `phidata-2.0.0.dev7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "phidata"
-version = "2.0.0.dev6"
+version = "2.0.0.dev7"
 description = "A toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
+  "aiohttp",
   "boto3",
   "docker",
   "gitpython",
-  "httpx",
   "kubernetes",
   "pydantic",
   "pydantic-settings",
   "python-dotenv",
   "pyyaml",
   "rich",
   "tomli",
@@ -85,11 +85,14 @@
 ]
 
 [[tool.mypy.overrides]]
 module = [
   "boto3.*",
   "botocore.*",
   "docker.*",
+  "openai.*",
   "pgvector.*",
+  "pypdf.*",
+  "sqlalchemy.*",
   "setuptools.*",
 ]
 ignore_missing_imports = true
```

