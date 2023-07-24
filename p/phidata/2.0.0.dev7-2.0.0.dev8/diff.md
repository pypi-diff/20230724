# Comparing `tmp/phidata-2.0.0.dev7.tar.gz` & `tmp/phidata-2.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.0.0.dev7.tar", last modified: Mon Jul 24 14:18:58 2023, max compression
+gzip compressed data, was "phidata-2.0.0.dev8.tar", last modified: Mon Jul 24 17:46:49 2023, max compression
```

## Comparing `phidata-2.0.0.dev7.tar` & `phidata-2.0.0.dev8.tar`

### file list

```diff
@@ -1,755 +1,755 @@
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.928250 phidata-2.0.0.dev7/
--rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev7/LICENSE
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 14:18:58.928084 phidata-2.0.0.dev7/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev7/README.md
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.749858 phidata-2.0.0.dev7/phi/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.751591 phidata-2.0.0.dev7/phi/api/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/api/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1543 2023-07-22 20:26:57.000000 phidata-2.0.0.dev7/phi/api/client.py
--rw-r--r--   0 zu         (501) staff       (20)      815 2023-07-21 16:44:29.000000 phidata-2.0.0.dev7/phi/api/routes.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.752534 phidata-2.0.0.dev7/phi/api/schemas/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/api/schemas/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      131 2023-07-21 11:59:13.000000 phidata-2.0.0.dev7/phi/api/schemas/response.py
--rw-r--r--   0 zu         (501) staff       (20)      490 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/api/schemas/user.py
--rw-r--r--   0 zu         (501) staff       (20)      442 2023-07-22 19:50:20.000000 phidata-2.0.0.dev7/phi/api/schemas/workspace.py
--rw-r--r--   0 zu         (501) staff       (20)     3514 2023-07-22 17:30:21.000000 phidata-2.0.0.dev7/phi/api/user.py
--rw-r--r--   0 zu         (501) staff       (20)     5735 2023-07-22 21:39:50.000000 phidata-2.0.0.dev7/phi/api/workspace.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.752898 phidata-2.0.0.dev7/phi/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.753625 phidata-2.0.0.dev7/phi/aws/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.753960 phidata-2.0.0.dev7/phi/aws/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.754321 phidata-2.0.0.dev7/phi/aws/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.754685 phidata-2.0.0.dev7/phi/aws/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.755022 phidata-2.0.0.dev7/phi/aws/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.756398 phidata-2.0.0.dev7/phi/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.756741 phidata-2.0.0.dev7/phi/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.757000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.757811 phidata-2.0.0.dev7/phi/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.759041 phidata-2.0.0.dev7/phi/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.760324 phidata-2.0.0.dev7/phi/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.760869 phidata-2.0.0.dev7/phi/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.761734 phidata-2.0.0.dev7/phi/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762087 phidata-2.0.0.dev7/phi/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762374 phidata-2.0.0.dev7/phi/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.762925 phidata-2.0.0.dev7/phi/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.763668 phidata-2.0.0.dev7/phi/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.763989 phidata-2.0.0.dev7/phi/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.764470 phidata-2.0.0.dev7/phi/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.766441 phidata-2.0.0.dev7/phi/cli/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3659 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/cli/auth_server.py
--rw-r--r--   0 zu         (501) staff       (20)    13299 2023-07-22 20:21:48.000000 phidata-2.0.0.dev7/phi/cli/config.py
--rw-r--r--   0 zu         (501) staff       (20)     2907 2023-07-22 21:44:58.000000 phidata-2.0.0.dev7/phi/cli/console.py
--rw-r--r--   0 zu         (501) staff       (20)      804 2023-07-22 20:24:19.000000 phidata-2.0.0.dev7/phi/cli/credentials.py
--rw-r--r--   0 zu         (501) staff       (20)    20376 2023-07-22 21:47:11.000000 phidata-2.0.0.dev7/phi/cli/entrypoint.py
--rw-r--r--   0 zu         (501) staff       (20)    15872 2023-07-22 17:24:33.000000 phidata-2.0.0.dev7/phi/cli/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.766793 phidata-2.0.0.dev7/phi/cli/ws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/cli/ws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27460 2023-07-22 20:35:52.000000 phidata-2.0.0.dev7/phi/cli/ws/ws_cli.py
--rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.767325 phidata-2.0.0.dev7/phi/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/api_client.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768128 phidata-2.0.0.dev7/phi/docker/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/context.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768540 phidata-2.0.0.dev7/phi/docker/app/django/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/django/django.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.768928 phidata-2.0.0.dev7/phi/docker/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.769365 phidata-2.0.0.dev7/phi/docker/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770054 phidata-2.0.0.dev7/phi/docker/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 zu         (501) staff       (20)     4732 2023-07-24 12:43:04.000000 phidata-2.0.0.dev7/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770431 phidata-2.0.0.dev7/phi/docker/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.770781 phidata-2.0.0.dev7/phi/docker/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.778637 phidata-2.0.0.dev7/phi/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.779030 phidata-2.0.0.dev7/phi/document/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/document/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.800444 phidata-2.0.0.dev7/phi/document/reader/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/document/reader/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/reader/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/document/reader/pdf.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.801808 phidata-2.0.0.dev7/phi/embedder/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/embedder/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/embedder/base.py
--rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/embedder/openai.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.802086 phidata-2.0.0.dev7/phi/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.802829 phidata-2.0.0.dev7/phi/infra/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/base.py
--rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/app/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1778 2023-07-23 12:14:29.000000 phidata-2.0.0.dev7/phi/infra/app/db_app.py
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/enums.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.803390 phidata-2.0.0.dev7/phi/infra/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/infra/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.803571 phidata-2.0.0.dev7/phi/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/k8s/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.804113 phidata-2.0.0.dev7/phi/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/llm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/llm/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.804667 phidata-2.0.0.dev7/phi/llm/conversation/
--rw-r--r--   0 zu         (501) staff       (20)       85 2023-07-23 19:28:29.000000 phidata-2.0.0.dev7/phi/llm/conversation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11301 2023-07-24 14:14:56.000000 phidata-2.0.0.dev7/phi/llm/conversation/conversation.py
--rw-r--r--   0 zu         (501) staff       (20)     1293 2023-07-24 14:04:35.000000 phidata-2.0.0.dev7/phi/llm/conversation/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.805191 phidata-2.0.0.dev7/phi/llm/history/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:47:16.000000 phidata-2.0.0.dev7/phi/llm/history/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1636 2023-07-24 13:53:07.000000 phidata-2.0.0.dev7/phi/llm/history/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1027 2023-07-24 11:31:02.000000 phidata-2.0.0.dev7/phi/llm/history/simple.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.805783 phidata-2.0.0.dev7/phi/llm/knowledge/
--rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-23 16:38:05.000000 phidata-2.0.0.dev7/phi/llm/knowledge/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      714 2023-07-24 11:47:28.000000 phidata-2.0.0.dev7/phi/llm/knowledge/base.py
--rw-r--r--   0 zu         (501) staff       (20)     2382 2023-07-24 13:11:31.000000 phidata-2.0.0.dev7/phi/llm/knowledge/pdf.py
--rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/llm/openai.py
--rw-r--r--   0 zu         (501) staff       (20)     1030 2023-07-24 11:43:07.000000 phidata-2.0.0.dev7/phi/llm/schemas.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806437 phidata-2.0.0.dev7/phi/llm/storage/
--rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:37:22.000000 phidata-2.0.0.dev7/phi/llm/storage/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      789 2023-07-24 11:25:53.000000 phidata-2.0.0.dev7/phi/llm/storage/base.py
--rw-r--r--   0 zu         (501) staff       (20)     7675 2023-07-24 14:12:29.000000 phidata-2.0.0.dev7/phi/llm/storage/postgres.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806717 phidata-2.0.0.dev7/phi/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.806998 phidata-2.0.0.dev7/phi/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/table/sql/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.809325 phidata-2.0.0.dev7/phi/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/defaults.py
--rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/git.py
--rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/load_env.py
--rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/pickle.py
--rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/py_io.py
--rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/pyproject.py
--rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/resource_filter.py
--rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.809680 phidata-2.0.0.dev7/phi/vectordb/
--rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.810147 phidata-2.0.0.dev7/phi/vectordb/pgvector/
--rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev7/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5592 2023-07-24 10:26:29.000000 phidata-2.0.0.dev7/phi/vectordb/pgvector/pgvector.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.811722 phidata-2.0.0.dev7/phi/workspace/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9931 2023-07-21 11:56:44.000000 phidata-2.0.0.dev7/phi/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/helpers.py
--rw-r--r--   0 zu         (501) staff       (20)    25401 2023-07-22 21:51:25.000000 phidata-2.0.0.dev7/phi/workspace/operator.py
--rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev7/phi/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.812310 phidata-2.0.0.dev7/phidata/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.813702 phidata-2.0.0.dev7/phidata/airflow/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev7/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.814412 phidata-2.0.0.dev7/phidata/airflow/operators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/operators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.817301 phidata-2.0.0.dev7/phidata/app/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev7/phidata/app/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.819907 phidata-2.0.0.dev7/phidata/app/airflow/
--rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev7/phidata/app/airflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.820383 phidata-2.0.0.dev7/phidata/app/alertmanager/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.821401 phidata-2.0.0.dev7/phidata/app/amundsen/
--rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev7/phidata/app/amundsen/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/frontend.py
--rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/metadata.py
--rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/amundsen/search.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.821865 phidata-2.0.0.dev7/phidata/app/assistant/
--rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev7/phidata/app/assistant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/assistant/assistant.py
--rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/aws_app.py
--rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/base_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.822342 phidata-2.0.0.dev7/phidata/app/cadvisor/
--rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.823228 phidata-2.0.0.dev7/phidata/app/databox/
--rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev7/phidata/app/databox/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/databox/databox.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.824275 phidata-2.0.0.dev7/phidata/app/db/
--rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev7/phidata/app/db/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev7/phidata/app/db/base_db.py
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev7/phidata/app/db/db_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.825044 phidata-2.0.0.dev7/phidata/app/django/
--rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev7/phidata/app/django/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/django/django_app.py
--rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/django/django_backup.py
--rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/docker_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.825729 phidata-2.0.0.dev7/phidata/app/elastic/
--rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/app/elastic/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.826207 phidata-2.0.0.dev7/phidata/app/elasticsearch/
--rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.826900 phidata-2.0.0.dev7/phidata/app/fastapi/
--rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/fastapi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.827482 phidata-2.0.0.dev7/phidata/app/grafana/
--rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/grafana/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/grafana/grafana.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.828704 phidata-2.0.0.dev7/phidata/app/jupyter/
--rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/jupyter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.829547 phidata-2.0.0.dev7/phidata/app/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev7/phidata/app/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/app.py
--rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/dir.py
--rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s/url.py
--rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/k8s_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.830189 phidata-2.0.0.dev7/phidata/app/mysql/
--rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev7/phidata/app/mysql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.830747 phidata-2.0.0.dev7/phidata/app/neo4j/
--rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/neo4j/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.831201 phidata-2.0.0.dev7/phidata/app/nodeexporter/
--rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/phidata_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.831817 phidata-2.0.0.dev7/phidata/app/postgres/
--rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev7/phidata/app/postgres/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.832414 phidata-2.0.0.dev7/phidata/app/prometheus/
--rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev7/phidata/app/prometheus/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.832973 phidata-2.0.0.dev7/phidata/app/qdrant/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/qdrant/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.833611 phidata-2.0.0.dev7/phidata/app/redis/
--rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev7/phidata/app/redis/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/redis/redis.py
--rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/redis/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.834666 phidata-2.0.0.dev7/phidata/app/server/
--rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev7/phidata/app/server/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/server/api_server.py
--rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/server/server_base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.836293 phidata-2.0.0.dev7/phidata/app/spark/
--rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev7/phidata/app/spark/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_base.py
--rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_driver.py
--rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.836826 phidata-2.0.0.dev7/phidata/app/streamlit/
--rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/streamlit/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.839705 phidata-2.0.0.dev7/phidata/app/superset/
--rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev7/phidata/app/superset/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_base.py
--rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_init.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_worker.py
--rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.863699 phidata-2.0.0.dev7/phidata/app/traefik/
--rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev7/phidata/app/traefik/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/crds.py
--rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/app/traefik/router.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.864133 phidata-2.0.0.dev7/phidata/asset/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.864474 phidata-2.0.0.dev7/phidata/asset/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/asset/data_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.865227 phidata-2.0.0.dev7/phidata/asset/local/
--rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/asset/local/file.py
--rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867055 phidata-2.0.0.dev7/phidata/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/aws/args.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867506 phidata-2.0.0.dev7/phidata/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/aws/config.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.867761 phidata-2.0.0.dev7/phidata/aws/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.868224 phidata-2.0.0.dev7/phidata/aws/create/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev7/phidata/aws/create/iam/role.py
--rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/driver.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.868850 phidata-2.0.0.dev7/phidata/aws/enums/
--rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.869743 phidata-2.0.0.dev7/phidata/aws/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870040 phidata-2.0.0.dev7/phidata/aws/resource/acm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870367 phidata-2.0.0.dev7/phidata/aws/resource/athena/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/athena/query.py
--rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.870740 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.871500 phidata-2.0.0.dev7/phidata/aws/resource/ec2/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.873047 phidata-2.0.0.dev7/phidata/aws/resource/ecs/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.874406 phidata-2.0.0.dev7/phidata/aws/resource/eks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.874948 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.875612 phidata-2.0.0.dev7/phidata/aws/resource/elb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.875898 phidata-2.0.0.dev7/phidata/aws/resource/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.876253 phidata-2.0.0.dev7/phidata/aws/resource/glue/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/aws/resource/group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877026 phidata-2.0.0.dev7/phidata/aws/resource/iam/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/group.py
--rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877734 phidata-2.0.0.dev7/phidata/aws/resource/rds/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.877982 phidata-2.0.0.dev7/phidata/aws/resource/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.878498 phidata-2.0.0.dev7/phidata/aws/resource/secret/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.879367 phidata-2.0.0.dev7/phidata/aws/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/aws/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/dataset.py
--rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/s3/object.py
--rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/aws/worker.py
--rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.880003 phidata-2.0.0.dev7/phidata/checks/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/checks/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev7/phidata/checks/check.py
--rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev7/phidata/checks/not_empty.py
--rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev7/phidata/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.880728 phidata-2.0.0.dev7/phidata/decorators/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/decorators/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/decorators/timer.py
--rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/decorators/validate_env.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.882772 phidata-2.0.0.dev7/phidata/docker/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/args.py
--rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/config.py
--rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/enums.py
--rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.884527 phidata-2.0.0.dev7/phidata/docker/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/base.py
--rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/container.py
--rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/docker/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/image.py
--rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/network.py
--rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/resource/utils.py
--rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/resource/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.884804 phidata-2.0.0.dev7/phidata/docker/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/docker/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/utils/container.py
--rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/docker/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.885904 phidata-2.0.0.dev7/phidata/exceptions/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/exceptions/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev7/phidata/exceptions/app.py
--rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/exceptions/task.py
--rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/exceptions/workflow.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.887292 phidata-2.0.0.dev7/phidata/infra/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/infra/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/infra/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev7/phidata/infra/args.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/infra/config.py
--rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/infra/resource.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.888973 phidata-2.0.0.dev7/phidata/k8s/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/api_client.py
--rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/k8s/args.py
--rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/config.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.889858 phidata-2.0.0.dev7/phidata/k8s/create/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890122 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890583 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.890888 phidata-2.0.0.dev7/phidata/k8s/create/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891163 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891809 phidata-2.0.0.dev7/phidata/k8s/create/common/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/labels.py
--rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.891973 phidata-2.0.0.dev7/phidata/k8s/create/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.893573 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.893938 phidata-2.0.0.dev7/phidata/k8s/create/crb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/group.py
--rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894228 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894484 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.894783 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895198 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895505 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.895754 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.898205 phidata-2.0.0.dev7/phidata/k8s/enums/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/api_group.py
--rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev7/phidata/k8s/enums/api_version.py
--rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev7/phidata/k8s/enums/kind.py
--rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/protocol.py
--rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/pv.py
--rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/service_type.py
--rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/exceptions.py
--rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/manager.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899341 phidata-2.0.0.dev7/phidata/k8s/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899527 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.899957 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900226 phidata-2.0.0.dev7/phidata/k8s/resource/apps/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900762 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/base.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.900951 phidata-2.0.0.dev7/phidata/k8s/resource/core/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.905240 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev7/phidata/k8s/resource/group.py
--rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.905833 phidata-2.0.0.dev7/phidata/k8s/resource/meta/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906372 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906639 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.906907 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907125 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907670 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.907863 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908092 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/types.py
--rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908505 phidata-2.0.0.dev7/phidata/k8s/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/k8s/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/utils/pod.py
--rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/k8s/worker.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.908679 phidata-2.0.0.dev7/phidata/llm/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.910141 phidata-2.0.0.dev7/phidata/llm/duckdb/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/agent.py
--rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/chain.py
--rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/connection.py
--rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/loader.py
--rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/query.py
--rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.910975 phidata-2.0.0.dev7/phidata/product/
--rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev7/phidata/product/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/product/data_product.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.911353 phidata-2.0.0.dev7/phidata/resource/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/resource/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/resource/reference.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.911607 phidata-2.0.0.dev7/phidata/table/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.912230 phidata-2.0.0.dev7/phidata/table/local/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/local/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/csv.py
--rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/local_table.py
--rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/local/parquet.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.912963 phidata-2.0.0.dev7/phidata/table/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/csv.py
--rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/parquet.py
--rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.913937 phidata-2.0.0.dev7/phidata/table/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/table/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev7/phidata/table/sql/postgres.py
--rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.915832 phidata-2.0.0.dev7/phidata/task/
--rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916106 phidata-2.0.0.dev7/phidata/task/aws/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916577 phidata-2.0.0.dev7/phidata/task/aws/athena/
--rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.916979 phidata-2.0.0.dev7/phidata/task/aws/emr/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917357 phidata-2.0.0.dev7/phidata/task/aws/glue/
--rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917579 phidata-2.0.0.dev7/phidata/task/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/dev/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917688 phidata-2.0.0.dev7/phidata/task/download/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.917884 phidata-2.0.0.dev7/phidata/task/download/s3/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/s3/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.918749 phidata-2.0.0.dev7/phidata/task/download/url/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/download/url/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_file.py
--rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.918899 phidata-2.0.0.dev7/phidata/task/plot/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/plot/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919129 phidata-2.0.0.dev7/phidata/task/plot/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/plot/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/task/python_task.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919389 phidata-2.0.0.dev7/phidata/task/run/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/run/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919573 phidata-2.0.0.dev7/phidata/task/run/sql/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/run/sql/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev7/phidata/task/run/sql/query.py
--rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/task/task.py
--rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/task/task_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.919855 phidata-2.0.0.dev7/phidata/task/upload/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/upload/__init__.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.920190 phidata-2.0.0.dev7/phidata/task/upload/file/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/task/upload/file/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.921123 phidata-2.0.0.dev7/phidata/types/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/types/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/types/airflow.py
--rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/types/context.py
--rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/types/phidata_runtime.py
--rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev7/phidata/types/run_status.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.925127 phidata-2.0.0.dev7/phidata/utils/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/utils/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/cli_console.py
--rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev7/phidata/utils/common.py
--rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev7/phidata/utils/compare.py
--rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev7/phidata/utils/context.py
--rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/dttm.py
--rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev7/phidata/utils/enums.py
--rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/env_file.py
--rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev7/phidata/utils/env_var.py
--rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/utils/filesystem.py
--rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/json_io.py
--rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/k8s.py
--rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/log.py
--rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev7/phidata/utils/print_table.py
--rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/utils/workspace_path.py
--rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/utils/yaml_io.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.926451 phidata-2.0.0.dev7/phidata/workflow/
--rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev7/phidata/workflow/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev7/phidata/workflow/decorator.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.926773 phidata-2.0.0.dev7/phidata/workflow/dev/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev7/phidata/workflow/dev/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/workflow/workflow.py
--rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev7/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.927403 phidata-2.0.0.dev7/phidata/workspace/
--rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev7/phidata/workspace/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev7/phidata/workspace/config.py
--rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev7/phidata/workspace/settings.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.813444 phidata-2.0.0.dev7/phidata.egg-info/
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)    18804 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/entry_points.txt
--rw-r--r--   0 zu         (501) staff       (20)      181 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/requires.txt
--rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-24 14:18:58.000000 phidata-2.0.0.dev7/phidata.egg-info/top_level.txt
--rw-r--r--   0 zu         (501) staff       (20)     1676 2023-07-24 14:18:36.000000 phidata-2.0.0.dev7/pyproject.toml
--rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-24 14:18:58.928291 phidata-2.0.0.dev7/setup.cfg
--rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev7/setup.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 14:18:58.927695 phidata-2.0.0.dev7/tests/
--rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev7/tests/test_placeholder.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.702121 phidata-2.0.0.dev8/
+-rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev8/LICENSE
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 17:46:49.701968 phidata-2.0.0.dev8/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev8/README.md
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.568589 phidata-2.0.0.dev8/phi/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.569746 phidata-2.0.0.dev8/phi/api/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/api/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1543 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/client.py
+-rw-r--r--   0 zu         (501) staff       (20)      815 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/routes.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.570393 phidata-2.0.0.dev8/phi/api/schemas/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      131 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/response.py
+-rw-r--r--   0 zu         (501) staff       (20)      490 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/user.py
+-rw-r--r--   0 zu         (501) staff       (20)      442 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/schemas/workspace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3514 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/user.py
+-rw-r--r--   0 zu         (501) staff       (20)     5735 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/api/workspace.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.570752 phidata-2.0.0.dev8/phi/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1310 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.571662 phidata-2.0.0.dev8/phi/aws/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    26919 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572136 phidata-2.0.0.dev8/phi/aws/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      766 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572533 phidata-2.0.0.dev8/phi/aws/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2862 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.572932 phidata-2.0.0.dev8/phi/aws/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      649 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.573447 phidata-2.0.0.dev8/phi/aws/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       90 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      735 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.574754 phidata-2.0.0.dev8/phi/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.575136 phidata-2.0.0.dev8/phi/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10489 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 zu         (501) staff       (20)     8725 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.575410 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10247 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.576393 phidata-2.0.0.dev8/phi/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21177 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2427 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.577742 phidata-2.0.0.dev8/phi/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6316 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    11368 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19592 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    21760 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3385 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.579195 phidata-2.0.0.dev8/phi/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7252 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    29689 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13244 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    24791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23405 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.579737 phidata-2.0.0.dev8/phi/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15451 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     5922 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.580480 phidata-2.0.0.dev8/phi/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10268 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7618 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9507 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.580800 phidata-2.0.0.dev8/phi/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12578 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.581129 phidata-2.0.0.dev8/phi/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12558 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)    23734 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.581655 phidata-2.0.0.dev8/phi/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7481 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9714 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.582497 phidata-2.0.0.dev8/phi/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    35097 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    34346 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7611 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      290 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.582786 phidata-2.0.0.dev8/phi/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6400 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.583363 phidata-2.0.0.dev8/phi/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11028 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)      999 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3475 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     5037 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.584639 phidata-2.0.0.dev8/phi/cli/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3659 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/auth_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    13299 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     2907 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/console.py
+-rw-r--r--   0 zu         (501) staff       (20)      804 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/credentials.py
+-rw-r--r--   0 zu         (501) staff       (20)    20376 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/entrypoint.py
+-rw-r--r--   0 zu         (501) staff       (20)    15872 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     2045 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.584973 phidata-2.0.0.dev8/phi/cli/ws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/cli/ws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27460 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-24 15:34:09.000000 phidata-2.0.0.dev8/phi/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.585317 phidata-2.0.0.dev8/phi/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1150 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/api_client.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.585841 phidata-2.0.0.dev8/phi/docker/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14659 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/context.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586135 phidata-2.0.0.dev8/phi/docker/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      917 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/django/django.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586592 phidata-2.0.0.dev8/phi/docker/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.586909 phidata-2.0.0.dev8/phi/docker/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)       87 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3275 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.587694 phidata-2.0.0.dev8/phi/docker/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      148 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      232 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 zu         (501) staff       (20)     4732 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.588213 phidata-2.0.0.dev8/phi/docker/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)       84 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      731 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.588620 phidata-2.0.0.dev8/phi/docker/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)       93 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.590233 phidata-2.0.0.dev8/phi/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4871 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    15125 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    21704 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14791 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1130 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     4785 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.590679 phidata-2.0.0.dev8/phi/document/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/document/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      809 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.591544 phidata-2.0.0.dev8/phi/document/reader/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/document/reader/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2149 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/reader/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2074 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/document/reader/pdf.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.592252 phidata-2.0.0.dev8/phi/embedder/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/embedder/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      466 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/embedder/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      976 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/embedder/openai.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.592615 phidata-2.0.0.dev8/phi/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.593500 phidata-2.0.0.dev8/phi/infra/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    13633 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      522 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/app/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1778 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/infra/app/db_app.py
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/enums.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594062 phidata-2.0.0.dev8/phi/infra/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6896 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1679 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/infra/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594259 phidata-2.0.0.dev8/phi/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/k8s/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.594910 phidata-2.0.0.dev8/phi/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/llm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      362 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/llm/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.595742 phidata-2.0.0.dev8/phi/llm/conversation/
+-rw-r--r--   0 zu         (501) staff       (20)       85 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/conversation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11437 2023-07-24 16:43:22.000000 phidata-2.0.0.dev8/phi/llm/conversation/conversation.py
+-rw-r--r--   0 zu         (501) staff       (20)     1293 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/conversation/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.596225 phidata-2.0.0.dev8/phi/llm/history/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1636 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1027 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/history/simple.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.596752 phidata-2.0.0.dev8/phi/llm/knowledge/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      714 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     2382 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/knowledge/pdf.py
+-rw-r--r--   0 zu         (501) staff       (20)     1169 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/llm/openai.py
+-rw-r--r--   0 zu         (501) staff       (20)     1030 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/llm/schemas.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.597469 phidata-2.0.0.dev8/phi/llm/storage/
+-rw-r--r--   0 zu         (501) staff       (20)       44 2023-07-23 16:37:22.000000 phidata-2.0.0.dev8/phi/llm/storage/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      670 2023-07-24 17:38:59.000000 phidata-2.0.0.dev8/phi/llm/storage/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7930 2023-07-24 17:39:14.000000 phidata-2.0.0.dev8/phi/llm/storage/postgres.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.597792 phidata-2.0.0.dev8/phi/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.598101 phidata-2.0.0.dev8/phi/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)       41 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      403 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/table/sql/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.600727 phidata-2.0.0.dev8/phi/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      747 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1342 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/defaults.py
+-rw-r--r--   0 zu         (501) staff       (20)      120 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)     1020 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)     1640 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/git.py
+-rw-r--r--   0 zu         (501) staff       (20)      889 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      665 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/load_env.py
+-rw-r--r--   0 zu         (501) staff       (20)     1009 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)     1010 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/pickle.py
+-rw-r--r--   0 zu         (501) staff       (20)      724 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/py_io.py
+-rw-r--r--   0 zu         (501) staff       (20)      589 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/pyproject.py
+-rw-r--r--   0 zu         (501) staff       (20)      962 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/resource_filter.py
+-rw-r--r--   0 zu         (501) staff       (20)      829 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.601152 phidata-2.0.0.dev8/phi/vectordb/
+-rw-r--r--   0 zu         (501) staff       (20)       39 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      700 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.601712 phidata-2.0.0.dev8/phi/vectordb/pgvector/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2023-07-18 13:44:43.000000 phidata-2.0.0.dev8/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5592 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/vectordb/pgvector/pgvector.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.603105 phidata-2.0.0.dev8/phi/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10069 2023-07-24 15:35:53.000000 phidata-2.0.0.dev8/phi/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      321 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1914 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/helpers.py
+-rw-r--r--   0 zu         (501) staff       (20)    25401 2023-07-24 14:21:57.000000 phidata-2.0.0.dev8/phi/workspace/operator.py
+-rw-r--r--   0 zu         (501) staff       (20)     9063 2023-07-18 13:43:48.000000 phidata-2.0.0.dev8/phi/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.603761 phidata-2.0.0.dev8/phidata/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.605162 phidata-2.0.0.dev8/phidata/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      140 2022-10-01 00:05:40.000000 phidata-2.0.0.dev8/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.605592 phidata-2.0.0.dev8/phidata/airflow/operators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      584 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.608629 phidata-2.0.0.dev8/phidata/app/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-10-28 00:34:05.000000 phidata-2.0.0.dev8/phidata/app/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.611500 phidata-2.0.0.dev8/phidata/app/airflow/
+-rw-r--r--   0 zu         (501) staff       (20)      385 2022-11-02 02:52:41.000000 phidata-2.0.0.dev8/phidata/app/airflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   100927 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    30469 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 zu         (501) staff       (20)    30508 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 zu         (501) staff       (20)    30505 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 zu         (501) staff       (20)    30515 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    30710 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.612136 phidata-2.0.0.dev8/phidata/app/alertmanager/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47889 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.613269 phidata-2.0.0.dev8/phidata/app/amundsen/
+-rw-r--r--   0 zu         (501) staff       (20)      398 2023-03-11 17:40:59.000000 phidata-2.0.0.dev8/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48031 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 zu         (501) staff       (20)    48032 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 zu         (501) staff       (20)    47944 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/amundsen/search.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.613912 phidata-2.0.0.dev8/phidata/app/assistant/
+-rw-r--r--   0 zu         (501) staff       (20)      139 2023-01-15 00:33:10.000000 phidata-2.0.0.dev8/phidata/app/assistant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49912 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/assistant/assistant.py
+-rw-r--r--   0 zu         (501) staff       (20)    30166 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/aws_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    17164 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/base_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.614417 phidata-2.0.0.dev8/phidata/app/cadvisor/
+-rw-r--r--   0 zu         (501) staff       (20)      118 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49678 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.615130 phidata-2.0.0.dev8/phidata/app/databox/
+-rw-r--r--   0 zu         (501) staff       (20)      157 2023-01-15 00:32:07.000000 phidata-2.0.0.dev8/phidata/app/databox/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    86151 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/databox/databox.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.616101 phidata-2.0.0.dev8/phidata/app/db/
+-rw-r--r--   0 zu         (501) staff       (20)       52 2022-03-29 16:28:05.000000 phidata-2.0.0.dev8/phidata/app/db/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3187 2023-01-05 15:43:33.000000 phidata-2.0.0.dev8/phidata/app/db/base_db.py
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-04 16:30:27.000000 phidata-2.0.0.dev8/phidata/app/db/db_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.616735 phidata-2.0.0.dev8/phidata/app/django/
+-rw-r--r--   0 zu         (501) staff       (20)      105 2023-05-18 09:49:43.000000 phidata-2.0.0.dev8/phidata/app/django/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27483 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/django/django_app.py
+-rw-r--r--   0 zu         (501) staff       (20)    30070 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/django/django_backup.py
+-rw-r--r--   0 zu         (501) staff       (20)    17172 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/docker_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.617307 phidata-2.0.0.dev8/phidata/app/elastic/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/app/elastic/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3723 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.617797 phidata-2.0.0.dev8/phidata/app/elasticsearch/
+-rw-r--r--   0 zu         (501) staff       (20)      138 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    48675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.618559 phidata-2.0.0.dev8/phidata/app/fastapi/
+-rw-r--r--   0 zu         (501) staff       (20)      175 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20266 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.619193 phidata-2.0.0.dev8/phidata/app/grafana/
+-rw-r--r--   0 zu         (501) staff       (20)      114 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/grafana/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49781 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/grafana/grafana.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.620485 phidata-2.0.0.dev8/phidata/app/jupyter/
+-rw-r--r--   0 zu         (501) staff       (20)      273 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    27093 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 zu         (501) staff       (20)    46942 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 zu         (501) staff       (20)    93432 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.621349 phidata-2.0.0.dev8/phidata/app/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-05-24 02:25:43.000000 phidata-2.0.0.dev8/phidata/app/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3930 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/app.py
+-rw-r--r--   0 zu         (501) staff       (20)     1766 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/dir.py
+-rw-r--r--   0 zu         (501) staff       (20)     6550 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s/url.py
+-rw-r--r--   0 zu         (501) staff       (20)    37830 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/k8s_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.621746 phidata-2.0.0.dev8/phidata/app/mysql/
+-rw-r--r--   0 zu         (501) staff       (20)      151 2023-05-03 15:21:14.000000 phidata-2.0.0.dev8/phidata/app/mysql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49110 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.622277 phidata-2.0.0.dev8/phidata/app/neo4j/
+-rw-r--r--   0 zu         (501) staff       (20)      106 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47856 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.622806 phidata-2.0.0.dev8/phidata/app/nodeexporter/
+-rw-r--r--   0 zu         (501) staff       (20)      134 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    47898 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 zu         (501) staff       (20)    38495 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/phidata_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.623512 phidata-2.0.0.dev8/phidata/app/postgres/
+-rw-r--r--   0 zu         (501) staff       (20)      166 2023-01-15 00:33:00.000000 phidata-2.0.0.dev8/phidata/app/postgres/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    53156 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.624101 phidata-2.0.0.dev8/phidata/app/prometheus/
+-rw-r--r--   0 zu         (501) staff       (20)      126 2023-03-11 17:22:33.000000 phidata-2.0.0.dev8/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49051 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.624710 phidata-2.0.0.dev8/phidata/app/qdrant/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12372 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.625411 phidata-2.0.0.dev8/phidata/app/redis/
+-rw-r--r--   0 zu         (501) staff       (20)      144 2023-01-15 00:32:35.000000 phidata-2.0.0.dev8/phidata/app/redis/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/redis/redis.py
+-rw-r--r--   0 zu         (501) staff       (20)    53296 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/redis/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.626559 phidata-2.0.0.dev8/phidata/app/server/
+-rw-r--r--   0 zu         (501) staff       (20)      207 2023-05-18 09:49:43.000000 phidata-2.0.0.dev8/phidata/app/server/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    18424 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/server/api_server.py
+-rw-r--r--   0 zu         (501) staff       (20)    58714 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/server/server_base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.628175 phidata-2.0.0.dev8/phidata/app/spark/
+-rw-r--r--   0 zu         (501) staff       (20)      193 2023-02-07 16:41:27.000000 phidata-2.0.0.dev8/phidata/app/spark/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    49424 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    17222 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 zu         (501) staff       (20)    17332 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.628677 phidata-2.0.0.dev8/phidata/app/streamlit/
+-rw-r--r--   0 zu         (501) staff       (20)      174 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    20207 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.630543 phidata-2.0.0.dev8/phidata/app/superset/
+-rw-r--r--   0 zu         (501) staff       (20)      411 2022-11-02 02:52:41.000000 phidata-2.0.0.dev8/phidata/app/superset/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    71570 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)    22925 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_init.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 zu         (501) staff       (20)    22910 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 zu         (501) staff       (20)    22917 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.631848 phidata-2.0.0.dev8/phidata/app/traefik/
+-rw-r--r--   0 zu         (501) staff       (20)      173 2023-01-15 00:32:52.000000 phidata-2.0.0.dev8/phidata/app/traefik/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)   115905 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/crds.py
+-rw-r--r--   0 zu         (501) staff       (20)    48190 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 zu         (501) staff       (20)    44972 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/app/traefik/router.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.632276 phidata-2.0.0.dev8/phidata/asset/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.632691 phidata-2.0.0.dev8/phidata/asset/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3210 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24787 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/asset/data_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.633444 phidata-2.0.0.dev8/phidata/asset/local/
+-rw-r--r--   0 zu         (501) staff       (20)       71 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    14564 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/asset/local/file.py
+-rw-r--r--   0 zu         (501) staff       (20)      574 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.635438 phidata-2.0.0.dev8/phidata/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1835 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)      487 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/aws/args.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.635932 phidata-2.0.0.dev8/phidata/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8186 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     3168 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/aws/config.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.636200 phidata-2.0.0.dev8/phidata/aws/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.636690 phidata-2.0.0.dev8/phidata/aws/create/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3233 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 zu         (501) staff       (20)     2472 2023-03-13 15:21:09.000000 phidata-2.0.0.dev8/phidata/aws/create/iam/role.py
+-rw-r--r--   0 zu         (501) staff       (20)    23058 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/driver.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.637235 phidata-2.0.0.dev8/phidata/aws/enums/
+-rw-r--r--   0 zu         (501) staff       (20)       62 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1083 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      304 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8588 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638248 phidata-2.0.0.dev8/phidata/aws/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638597 phidata-2.0.0.dev8/phidata/aws/resource/acm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.638987 phidata-2.0.0.dev8/phidata/aws/resource/athena/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     9127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.639299 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.640026 phidata-2.0.0.dev8/phidata/aws/resource/ec2/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21341 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 zu         (501) staff       (20)     2563 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 zu         (501) staff       (20)    11801 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.641388 phidata-2.0.0.dev8/phidata/aws/resource/ecs/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6140 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    26253 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    19630 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 zu         (501) staff       (20)    22397 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 zu         (501) staff       (20)     3614 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.642970 phidata-2.0.0.dev8/phidata/aws/resource/eks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 zu         (501) staff       (20)    30104 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    13731 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 zu         (501) staff       (20)    23785 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 zu         (501) staff       (20)    23742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.643617 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    15823 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     6305 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.644526 phidata-2.0.0.dev8/phidata/aws/resource/elb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-07 15:40:41.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10727 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 zu         (501) staff       (20)     7994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 zu         (501) staff       (20)     9834 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.644930 phidata-2.0.0.dev8/phidata/aws/resource/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12806 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.645429 phidata-2.0.0.dev8/phidata/aws/resource/glue/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    12850 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/aws/resource/group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.648124 phidata-2.0.0.dev8/phidata/aws/resource/iam/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     9958 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     7653 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 zu         (501) staff       (20)     9828 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.648999 phidata-2.0.0.dev8/phidata/aws/resource/rds/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    36056 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)    35380 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 zu         (501) staff       (20)     7990 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.649286 phidata-2.0.0.dev8/phidata/aws/resource/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6472 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.649780 phidata-2.0.0.dev8/phidata/aws/resource/secret/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11398 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 zu         (501) staff       (20)     1007 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 zu         (501) staff       (20)     3604 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)     9688 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.650903 phidata-2.0.0.dev8/phidata/aws/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/aws/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    21797 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    24100 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/dataset.py
+-rw-r--r--   0 zu         (501) staff       (20)    14394 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 zu         (501) staff       (20)     7409 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/s3/object.py
+-rw-r--r--   0 zu         (501) staff       (20)    22470 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/aws/worker.py
+-rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.651552 phidata-2.0.0.dev8/phidata/checks/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/checks/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2790 2023-01-31 22:57:08.000000 phidata-2.0.0.dev8/phidata/checks/check.py
+-rw-r--r--   0 zu         (501) staff       (20)      754 2023-02-03 21:54:28.000000 phidata-2.0.0.dev8/phidata/checks/not_empty.py
+-rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev8/phidata/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.652345 phidata-2.0.0.dev8/phidata/decorators/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/decorators/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      582 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/decorators/timer.py
+-rw-r--r--   0 zu         (501) staff       (20)     1110 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/decorators/validate_env.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.654310 phidata-2.0.0.dev8/phidata/docker/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1728 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1645 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     4482 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     1166 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)      322 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8899 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.656302 phidata-2.0.0.dev8/phidata/docker/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3804 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/base.py
+-rw-r--r--   0 zu         (501) staff       (20)    16440 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      932 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/docker/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)    14773 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/image.py
+-rw-r--r--   0 zu         (501) staff       (20)     5226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/network.py
+-rw-r--r--   0 zu         (501) staff       (20)     1165 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10737 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/resource/utils.py
+-rw-r--r--   0 zu         (501) staff       (20)     4961 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/resource/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.656610 phidata-2.0.0.dev8/phidata/docker/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/docker/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3584 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/utils/container.py
+-rw-r--r--   0 zu         (501) staff       (20)    24179 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/docker/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.657799 phidata-2.0.0.dev8/phidata/exceptions/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/exceptions/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)       47 2022-05-24 18:09:11.000000 phidata-2.0.0.dev8/phidata/exceptions/app.py
+-rw-r--r--   0 zu         (501) staff       (20)       39 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/exceptions/task.py
+-rw-r--r--   0 zu         (501) staff       (20)       43 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/exceptions/workflow.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.659315 phidata-2.0.0.dev8/phidata/infra/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/infra/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      341 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/infra/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     2466 2023-01-25 22:40:46.000000 phidata-2.0.0.dev8/phidata/infra/args.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/infra/config.py
+-rw-r--r--   0 zu         (501) staff       (20)    12048 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/infra/resource.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.661159 phidata-2.0.0.dev8/phidata/k8s/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/api_client.py
+-rw-r--r--   0 zu         (501) staff       (20)     1986 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/k8s/args.py
+-rw-r--r--   0 zu         (501) staff       (20)     7871 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/config.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662123 phidata-2.0.0.dev8/phidata/k8s/create/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662408 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.662887 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3418 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)     2430 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663113 phidata-2.0.0.dev8/phidata/k8s/create/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663297 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5429 2023-01-24 16:40:47.000000 phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663833 phidata-2.0.0.dev8/phidata/k8s/create/common/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      357 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 zu         (501) staff       (20)     1553 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.663982 phidata-2.0.0.dev8/phidata/k8s/create/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.665953 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1395 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)     5490 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)     1515 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     6695 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     2005 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     1555 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)     4200 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     2030 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     4516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666225 phidata-2.0.0.dev8/phidata/k8s/create/crb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2115 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 zu         (501) staff       (20)    19062 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     5795 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666521 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.666741 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:52:37.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2069 2023-01-31 02:29:01.000000 phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667083 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667508 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1754 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     1503 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667689 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.667917 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     3882 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.670111 phidata-2.0.0.dev8/phidata/k8s/enums/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      226 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 zu         (501) staff       (20)      542 2023-01-31 02:03:51.000000 phidata-2.0.0.dev8/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 zu         (501) staff       (20)      162 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      762 2023-01-31 02:04:08.000000 phidata-2.0.0.dev8/phidata/k8s/enums/kind.py
+-rw-r--r--   0 zu         (501) staff       (20)     1085 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 zu         (501) staff       (20)      127 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 zu         (501) staff       (20)      753 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/pv.py
+-rw-r--r--   0 zu         (501) staff       (20)      153 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 zu         (501) staff       (20)      171 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      143 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)      377 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 zu         (501) staff       (20)      419 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/exceptions.py
+-rw-r--r--   0 zu         (501) staff       (20)     8596 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/manager.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671386 phidata-2.0.0.dev8/phidata/k8s/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671562 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.671976 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8592 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 zu         (501) staff       (20)    15390 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.672308 phidata-2.0.0.dev8/phidata/k8s/resource/apps/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.672922 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10211 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 zu         (501) staff       (20)     1958 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/base.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.673134 phidata-2.0.0.dev8/phidata/k8s/resource/core/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.677517 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     6602 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 zu         (501) staff       (20)    18530 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 zu         (501) staff       (20)      822 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)     6635 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 zu         (501) staff       (20)     3863 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     1614 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 zu         (501) staff       (20)    12419 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 zu         (501) staff       (20)     8107 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 zu         (501) staff       (20)     2693 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)     7468 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)      901 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 zu         (501) staff       (20)     1244 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 zu         (501) staff       (20)     6196 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 zu         (501) staff       (20)    18982 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 zu         (501) staff       (20)     8657 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 zu         (501) staff       (20)     2313 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 zu         (501) staff       (20)     4086 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 zu         (501) staff       (20)     4788 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 zu         (501) staff       (20)      890 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 zu         (501) staff       (20)    13397 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 zu         (501) staff       (20)    12690 2023-06-20 14:11:22.000000 phidata-2.0.0.dev8/phidata/k8s/resource/group.py
+-rw-r--r--   0 zu         (501) staff       (20)     4475 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.678983 phidata-2.0.0.dev8/phidata/k8s/resource/meta/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679471 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1058 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 zu         (501) staff       (20)     2739 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679679 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:16.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.679988 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-31 01:30:42.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    10026 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.680248 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.680940 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     8969 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 zu         (501) staff       (20)     6675 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.681175 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.681540 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     7198 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 zu         (501) staff       (20)     3415 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/types.py
+-rw-r--r--   0 zu         (501) staff       (20)    10127 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.682023 phidata-2.0.0.dev8/phidata/k8s/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1864 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/utils/pod.py
+-rw-r--r--   0 zu         (501) staff       (20)    43059 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/k8s/worker.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.682200 phidata-2.0.0.dev8/phidata/llm/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.683655 phidata-2.0.0.dev8/phidata/llm/duckdb/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4403 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 zu         (501) staff       (20)     3896 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 zu         (501) staff       (20)      920 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 zu         (501) staff       (20)     1194 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 zu         (501) staff       (20)     2177 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     1063 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684330 phidata-2.0.0.dev8/phidata/product/
+-rw-r--r--   0 zu         (501) staff       (20)       70 2022-03-13 21:20:10.000000 phidata-2.0.0.dev8/phidata/product/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    29505 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/product/data_product.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684671 phidata-2.0.0.dev8/phidata/resource/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/resource/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)      445 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/resource/reference.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.684908 phidata-2.0.0.dev8/phidata/table/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.685547 phidata-2.0.0.dev8/phidata/table/local/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/local/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4616 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)    23516 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/local_table.py
+-rw-r--r--   0 zu         (501) staff       (20)     4624 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/local/parquet.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.686201 phidata-2.0.0.dev8/phidata/table/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4673 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/csv.py
+-rw-r--r--   0 zu         (501) staff       (20)     4668 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/parquet.py
+-rw-r--r--   0 zu         (501) staff       (20)    23064 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.686832 phidata-2.0.0.dev8/phidata/table/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/table/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1752 2023-04-07 15:40:41.000000 phidata-2.0.0.dev8/phidata/table/sql/postgres.py
+-rw-r--r--   0 zu         (501) staff       (20)    35497 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.688477 phidata-2.0.0.dev8/phidata/task/
+-rw-r--r--   0 zu         (501) staff       (20)       79 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.688755 phidata-2.0.0.dev8/phidata/task/aws/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.689298 phidata-2.0.0.dev8/phidata/task/aws/athena/
+-rw-r--r--   0 zu         (501) staff       (20)       81 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2210 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.689843 phidata-2.0.0.dev8/phidata/task/aws/emr/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 zu         (501) staff       (20)     1637 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690405 phidata-2.0.0.dev8/phidata/task/aws/glue/
+-rw-r--r--   0 zu         (501) staff       (20)      100 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2038 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 zu         (501) staff       (20)     1381 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690618 phidata-2.0.0.dev8/phidata/task/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/dev/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690740 phidata-2.0.0.dev8/phidata/task/download/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.690976 phidata-2.0.0.dev8/phidata/task/download/s3/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2114 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.691866 phidata-2.0.0.dev8/phidata/task/download/url/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/download/url/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4775 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     3681 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     8180 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692021 phidata-2.0.0.dev8/phidata/task/plot/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/plot/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692263 phidata-2.0.0.dev8/phidata/task/plot/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2541 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/plot/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)    12300 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/task/python_task.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692537 phidata-2.0.0.dev8/phidata/task/run/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/run/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692725 phidata-2.0.0.dev8/phidata/task/run/sql/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4126 2023-04-09 17:01:38.000000 phidata-2.0.0.dev8/phidata/task/run/sql/query.py
+-rw-r--r--   0 zu         (501) staff       (20)     7636 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/task/task.py
+-rw-r--r--   0 zu         (501) staff       (20)     1041 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/task/task_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.692995 phidata-2.0.0.dev8/phidata/task/upload/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/upload/__init__.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.693332 phidata-2.0.0.dev8/phidata/task/upload/file/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     2039 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 zu         (501) staff       (20)     4721 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.694457 phidata-2.0.0.dev8/phidata/types/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/types/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1023 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/types/airflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     2063 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/types/context.py
+-rw-r--r--   0 zu         (501) staff       (20)      705 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/types/phidata_runtime.py
+-rw-r--r--   0 zu         (501) staff       (20)      101 2022-04-22 20:24:07.000000 phidata-2.0.0.dev8/phidata/types/run_status.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.699386 phidata-2.0.0.dev8/phidata/utils/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/utils/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     4779 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/cli_console.py
+-rw-r--r--   0 zu         (501) staff       (20)     2044 2023-01-31 02:10:08.000000 phidata-2.0.0.dev8/phidata/utils/common.py
+-rw-r--r--   0 zu         (501) staff       (20)     1037 2022-11-28 16:47:00.000000 phidata-2.0.0.dev8/phidata/utils/compare.py
+-rw-r--r--   0 zu         (501) staff       (20)     2146 2023-03-13 15:21:10.000000 phidata-2.0.0.dev8/phidata/utils/context.py
+-rw-r--r--   0 zu         (501) staff       (20)     1113 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/dttm.py
+-rw-r--r--   0 zu         (501) staff       (20)      786 2022-06-12 23:07:23.000000 phidata-2.0.0.dev8/phidata/utils/enums.py
+-rw-r--r--   0 zu         (501) staff       (20)     1595 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/env_file.py
+-rw-r--r--   0 zu         (501) staff       (20)     1430 2022-07-31 02:48:39.000000 phidata-2.0.0.dev8/phidata/utils/env_var.py
+-rw-r--r--   0 zu         (501) staff       (20)      661 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/utils/filesystem.py
+-rw-r--r--   0 zu         (501) staff       (20)      742 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 zu         (501) staff       (20)      893 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/json_io.py
+-rw-r--r--   0 zu         (501) staff       (20)     1257 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/k8s.py
+-rw-r--r--   0 zu         (501) staff       (20)     1459 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/log.py
+-rw-r--r--   0 zu         (501) staff       (20)      707 2023-01-14 19:22:32.000000 phidata-2.0.0.dev8/phidata/utils/print_table.py
+-rw-r--r--   0 zu         (501) staff       (20)      994 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/utils/workspace_path.py
+-rw-r--r--   0 zu         (501) staff       (20)      833 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/utils/yaml_io.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.700552 phidata-2.0.0.dev8/phidata/workflow/
+-rw-r--r--   0 zu         (501) staff       (20)      109 2022-04-15 05:02:36.000000 phidata-2.0.0.dev8/phidata/workflow/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1855 2022-04-18 19:05:50.000000 phidata-2.0.0.dev8/phidata/workflow/decorator.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.700854 phidata-2.0.0.dev8/phidata/workflow/dev/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev8/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    42342 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/workflow/workflow.py
+-rw-r--r--   0 zu         (501) staff       (20)     1105 2022-04-25 21:05:27.000000 phidata-2.0.0.dev8/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.701374 phidata-2.0.0.dev8/phidata/workspace/
+-rw-r--r--   0 zu         (501) staff       (20)      110 2023-06-15 14:48:05.000000 phidata-2.0.0.dev8/phidata/workspace/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)    11316 2023-07-07 23:39:27.000000 phidata-2.0.0.dev8/phidata/workspace/config.py
+-rw-r--r--   0 zu         (501) staff       (20)     8781 2023-07-06 09:54:23.000000 phidata-2.0.0.dev8/phidata/workspace/settings.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.604904 phidata-2.0.0.dev8/phidata.egg-info/
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)    18804 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 zu         (501) staff       (20)      181 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/requires.txt
+-rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-24 17:46:49.000000 phidata-2.0.0.dev8/phidata.egg-info/top_level.txt
+-rw-r--r--   0 zu         (501) staff       (20)     1676 2023-07-24 17:42:03.000000 phidata-2.0.0.dev8/pyproject.toml
+-rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-24 17:46:49.702166 phidata-2.0.0.dev8/setup.cfg
+-rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev8/setup.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-24 17:46:49.701653 phidata-2.0.0.dev8/tests/
+-rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev8/tests/test_placeholder.py
```

### Comparing `phidata-2.0.0.dev7/LICENSE` & `phidata-2.0.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/PKG-INFO` & `phidata-2.0.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev7
+Version: 2.0.0.dev8
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
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev7 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev8 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev7/README.md` & `phidata-2.0.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/api/client.py` & `phidata-2.0.0.dev8/phi/api/client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/api/routes.py` & `phidata-2.0.0.dev8/phi/api/routes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/api/user.py` & `phidata-2.0.0.dev8/phi/api/user.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/api/workspace.py` & `phidata-2.0.0.dev8/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/api_client.py` & `phidata-2.0.0.dev8/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/app/base.py` & `phidata-2.0.0.dev8/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/app/fastapi/fastapi.py` & `phidata-2.0.0.dev8/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/app/jupyter/jupyter.py` & `phidata-2.0.0.dev8/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/app/qdrant/qdrant.py` & `phidata-2.0.0.dev8/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/app/streamlit/streamlit.py` & `phidata-2.0.0.dev8/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev8/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/base.py` & `phidata-2.0.0.dev8/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev8/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev8/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev8/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev8/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev8/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ecs/container.py` & `phidata-2.0.0.dev8/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ecs/service.py` & `phidata-2.0.0.dev8/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev8/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev8/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/eks/addon.py` & `phidata-2.0.0.dev8/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev8/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev8/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev8/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev8/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev8/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev8/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/elb/listener.py` & `phidata-2.0.0.dev8/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev8/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev8/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev8/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev8/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/group.py` & `phidata-2.0.0.dev8/phi/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/iam/policy.py` & `phidata-2.0.0.dev8/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/iam/role.py` & `phidata-2.0.0.dev8/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev8/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev8/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev8/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev8/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/secret/manager.py` & `phidata-2.0.0.dev8/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/secret/reader.py` & `phidata-2.0.0.dev8/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/aws/resource/types.py` & `phidata-2.0.0.dev8/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/base.py` & `phidata-2.0.0.dev8/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/auth_server.py` & `phidata-2.0.0.dev8/phi/cli/auth_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/config.py` & `phidata-2.0.0.dev8/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/console.py` & `phidata-2.0.0.dev8/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/credentials.py` & `phidata-2.0.0.dev8/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/entrypoint.py` & `phidata-2.0.0.dev8/phi/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/operator.py` & `phidata-2.0.0.dev8/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/settings.py` & `phidata-2.0.0.dev8/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/cli/ws/ws_cli.py` & `phidata-2.0.0.dev8/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/constants.py` & `phidata-2.0.0.dev8/phi/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 PYTHONPATH_ENV_VAR: str = "PYTHONPATH"
 PHI_RUNTIME_ENV_VAR: str = "PHI_RUNTIME"
 
 SCRIPTS_DIR_ENV_VAR: str = "PHI_SCRIPTS_DIR"
 STORAGE_DIR_ENV_VAR: str = "PHI_STORAGE_DIR"
 WORKFLOWS_DIR_ENV_VAR: str = "PHI_WORKFLOWS_DIR"
+WORKSPACE_NAME_ENV_VAR: str = "PHI_WORKSPACE_NAME"
 WORKSPACE_ROOT_ENV_VAR: str = "PHI_WORKSPACE_ROOT"
 WORKSPACES_MOUNT_ENV_VAR: str = "PHI_WORKSPACES_MOUNT"
 WORKSPACE_DIR_ENV_VAR: str = "PHI_WORKSPACE_DIR"
 REQUIREMENTS_FILE_PATH_ENV_VAR: str = "REQUIREMENTS_FILE_PATH"
 
 AWS_REGION_ENV_VAR: str = "AWS_REGION"
 AWS_DEFAULT_REGION_ENV_VAR: str = "AWS_DEFAULT_REGION"
```

### Comparing `phidata-2.0.0.dev7/phi/docker/api_client.py` & `phidata-2.0.0.dev8/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/base.py` & `phidata-2.0.0.dev8/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/django/django.py` & `phidata-2.0.0.dev8/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/fastapi/fastapi.py` & `phidata-2.0.0.dev8/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/jupyter/jupyter.py` & `phidata-2.0.0.dev8/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/postgres/postgres.py` & `phidata-2.0.0.dev8/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/qdrant/qdrant.py` & `phidata-2.0.0.dev8/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/app/streamlit/streamlit.py` & `phidata-2.0.0.dev8/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/base.py` & `phidata-2.0.0.dev8/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/container.py` & `phidata-2.0.0.dev8/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/group.py` & `phidata-2.0.0.dev8/phi/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/image.py` & `phidata-2.0.0.dev8/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/network.py` & `phidata-2.0.0.dev8/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/types.py` & `phidata-2.0.0.dev8/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/docker/resource/volume.py` & `phidata-2.0.0.dev8/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/document/base.py` & `phidata-2.0.0.dev8/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/document/reader/base.py` & `phidata-2.0.0.dev8/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/document/reader/pdf.py` & `phidata-2.0.0.dev8/phi/document/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/embedder/openai.py` & `phidata-2.0.0.dev8/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/infra/app/base.py` & `phidata-2.0.0.dev8/phi/infra/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/infra/app/context.py` & `phidata-2.0.0.dev8/phi/infra/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/infra/app/db_app.py` & `phidata-2.0.0.dev8/phi/infra/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/infra/resource/base.py` & `phidata-2.0.0.dev8/phi/infra/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/infra/resource/group.py` & `phidata-2.0.0.dev8/phi/infra/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/conversation/conversation.py` & `phidata-2.0.0.dev8/phi/llm/conversation/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class Conversation(BaseModel):
     # The ID of this conversation.
     id: Optional[int] = None
     # The name of this conversation.
     name: Optional[str] = None
     # Set log level to debug
     debug_logs: bool = False
-    # Send monitoring data to phidata.com
+    # Monitor conversations on phidata.com
     monitoring: bool = False
 
     # LLM settings
     llm: LLM = OpenAIChat()
     llm_name: Optional[str] = None
     system_prompt: Optional[str] = None
 
@@ -271,18 +271,25 @@
             self.usage_data["questions"] += 1
         else:
             self.usage_data["questions"] = 1
 
         # Save conversation to storage
         self.save_to_storage()
 
+        # Monitor conversation
+        self.monitor()
+
     def save_to_storage(self) -> None:
         """Save the conversation to the storage"""
         if self.storage is None:
             return
         self.storage.upsert_conversation(conversation=self.conversation_row)
 
     def end(self) -> None:
         """End the conversation"""
         if self.storage is not None:
             if self.id is not None:
                 self.storage.end_conversation(conversation_id=self.id, user_id=self.user_id)
+
+    def monitor(self):
+        logger.debug("Monitoring request")
+        pass
```

### Comparing `phidata-2.0.0.dev7/phi/llm/conversation/schemas.py` & `phidata-2.0.0.dev8/phi/llm/conversation/schemas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/history/base.py` & `phidata-2.0.0.dev8/phi/llm/history/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/history/simple.py` & `phidata-2.0.0.dev8/phi/llm/history/simple.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/knowledge/base.py` & `phidata-2.0.0.dev8/phi/llm/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/knowledge/pdf.py` & `phidata-2.0.0.dev8/phi/llm/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/openai.py` & `phidata-2.0.0.dev8/phi/llm/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/schemas.py` & `phidata-2.0.0.dev8/phi/llm/schemas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/llm/storage/base.py` & `phidata-2.0.0.dev8/phi/llm/storage/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Dict, List, Any
-
-from phi.llm.conversation.schemas import ConversationRow
+from typing import Optional, Any
 
 
 class LLMStorage(ABC):
     @abstractmethod
     def create(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def read_conversation(self, conversation_id: int, user_id: str) -> Optional[ConversationRow]:
+    def read_conversation(self, conversation_id: int, user_id: str) -> Optional[Any]:
         raise NotImplementedError
 
     @abstractmethod
-    def upsert_conversation(self, conversation: ConversationRow) -> Optional[ConversationRow]:
+    def upsert_conversation(self, conversation: Any) -> Optional[Any]:
         raise NotImplementedError
 
     @abstractmethod
-    def end_conversation(self, conversation_id: int, user_id: str) -> Optional[ConversationRow]:
+    def end_conversation(self, conversation_id: int, user_id: str) -> Optional[Any]:
         raise NotImplementedError
 
     @abstractmethod
     def delete(self) -> None:
         raise NotImplementedError
-
```

### Comparing `phidata-2.0.0.dev7/phi/llm/storage/postgres.py` & `phidata-2.0.0.dev8/phi/llm/storage/postgres.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, Dict, Any
+
 try:
     from sqlalchemy.dialects import postgresql
     from sqlalchemy.engine import create_engine, Engine
     from sqlalchemy.engine.row import Row
     from sqlalchemy.inspection import inspect
     from sqlalchemy.orm import Session, sessionmaker
     from sqlalchemy.schema import MetaData, Table, Column
@@ -86,40 +87,46 @@
                     with sess.begin():
                         logger.debug(f"Creating schema: {self.schema}")
                         sess.execute(text(f"create schema if not exists {self.schema};"))
             logger.debug(f"Creating table: {self.table_name}")
             self.table.create(self.db_engine)
 
     def _read_conversation(self, session: Session, conversation_id: int, user_id: str) -> Optional[Row[Any]]:
-        stmt = select(self.table) \
-            .where(self.table.c.id == conversation_id) \
-            .where(self.table.c.user_id == user_id) \
-            .where(self.table.c.is_active == True)
+        stmt = (
+            select(self.table)
+            .where(self.table.c.id == conversation_id)
+            .where(self.table.c.user_id == user_id)
+            .where(self.table.c.is_active == True)  # noqa: E712
+        )
 
         return session.execute(stmt).one()
 
     def read_conversation(self, conversation_id: int, user_id: str) -> Optional[ConversationRow]:
         with self.Session() as sess:
             with sess.begin():
-                existing_row: Optional[Row[Any]] = self._read_conversation(session=sess, conversation_id=conversation_id, user_id=user_id)
+                existing_row: Optional[Row[Any]] = self._read_conversation(
+                    session=sess, conversation_id=conversation_id, user_id=user_id
+                )
                 return ConversationRow.model_validate(existing_row) if existing_row is not None else None
 
     def upsert_conversation(self, conversation: ConversationRow) -> Optional[ConversationRow]:
         """
         Create a new conversation if it does not exist, otherwise update the existing conversation.
         """
         with self.Session() as sess:
             with sess.begin():
                 # Conversation exists if conversation.id is not None
                 if conversation.id is None:
                     values_to_insert: Dict[str, Any] = {
                         "user_id": conversation.user_id,
                         "user_persona": conversation.user_persona,
                         "user_data": conversation.user_data,
-                        "history": conversation.history.model_dump(include={"chat_history", "llm_history", "references"}),
+                        "history": conversation.history.model_dump(
+                            include={"chat_history", "llm_history", "references"}
+                        ),
                         "usage_data": conversation.usage_data,
                     }
                     if conversation.name is not None:
                         values_to_insert["name"] = conversation.name
 
                     insert_stmt = postgresql.insert(self.table).values(**values_to_insert)
                     result = sess.execute(insert_stmt)
@@ -129,33 +136,39 @@
                     if conversation.name is not None:
                         values_to_update["name"] = conversation.name
                     if conversation.user_persona is not None:
                         values_to_update["user_persona"] = conversation.user_persona
                     if conversation.user_data is not None:
                         values_to_update["user_data"] = conversation.user_data
                     if conversation.history is not None:
-                        values_to_update["history"] = conversation.history.model_dump(include={"chat_history", "llm_history", "references"})
+                        values_to_update["history"] = conversation.history.model_dump(
+                            include={"chat_history", "llm_history", "references"}
+                        )
                     if conversation.usage_data is not None:
                         values_to_update["usage_data"] = conversation.usage_data
 
-                    update_stmt = self.table.update()\
-                        .where(self.table.c.id == conversation.id)\
-                        .values(**values_to_update)
+                    update_stmt = (
+                        self.table.update().where(self.table.c.id == conversation.id).values(**values_to_update)
+                    )
                     sess.execute(update_stmt)
         return self.read_conversation(conversation_id=conversation.id, user_id=conversation.user_id)
 
     def end_conversation(self, conversation_id: int, user_id: str) -> None:
         with self.Session() as sess:
             with sess.begin():
-                existing_row: Optional[Row[Any]] = self._read_conversation(session=sess, conversation_id=conversation_id, user_id=user_id)
+                existing_row: Optional[Row[Any]] = self._read_conversation(
+                    session=sess, conversation_id=conversation_id, user_id=user_id
+                )
                 # Check if conversation exists in the database
                 if existing_row is not None:
-                    stmt = self.table.update() \
-                        .where(self.table.c.id == conversation_id) \
-                        .where(self.table.c.user_id == user_id) \
+                    stmt = (
+                        self.table.update()
+                        .where(self.table.c.id == conversation_id)
+                        .where(self.table.c.user_id == user_id)
                         .values(is_active=False)
+                    )
                     sess.execute(stmt)
 
     def delete(self) -> None:
         if self.table_exists():
             logger.debug(f"Deleting table: {self.table_name}")
             self.table.drop(self.db_engine)
```

### Comparing `phidata-2.0.0.dev7/phi/utils/common.py` & `phidata-2.0.0.dev8/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/defaults.py` & `phidata-2.0.0.dev8/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/filesystem.py` & `phidata-2.0.0.dev8/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/git.py` & `phidata-2.0.0.dev8/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/json_io.py` & `phidata-2.0.0.dev8/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/load_env.py` & `phidata-2.0.0.dev8/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/log.py` & `phidata-2.0.0.dev8/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/pickle.py` & `phidata-2.0.0.dev8/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/py_io.py` & `phidata-2.0.0.dev8/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/pyproject.py` & `phidata-2.0.0.dev8/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/resource_filter.py` & `phidata-2.0.0.dev8/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/utils/yaml_io.py` & `phidata-2.0.0.dev8/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/vectordb/base.py` & `phidata-2.0.0.dev8/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/vectordb/pgvector/pgvector.py` & `phidata-2.0.0.dev8/phi/vectordb/pgvector/pgvector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/workspace/config.py` & `phidata-2.0.0.dev8/phi/workspace/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,18 +144,22 @@
     def set_local_env(self) -> None:
         from os import environ
 
         from phi.constants import (
             SCRIPTS_DIR_ENV_VAR,
             STORAGE_DIR_ENV_VAR,
             WORKFLOWS_DIR_ENV_VAR,
+            WORKSPACE_NAME_ENV_VAR,
             WORKSPACE_ROOT_ENV_VAR,
             WORKSPACE_DIR_ENV_VAR,
         )
 
+        if self.ws_name is not None:
+            environ[WORKSPACE_NAME_ENV_VAR] = str(self.ws_name)
+
         if self.ws_root_path is not None:
             environ[WORKSPACE_ROOT_ENV_VAR] = str(self.ws_root_path)
 
             workspace_dir_path: Optional[Path] = self.workspace_dir_path
             if workspace_dir_path is not None:
                 environ[WORKSPACE_DIR_ENV_VAR] = str(workspace_dir_path)
```

### Comparing `phidata-2.0.0.dev7/phi/workspace/helpers.py` & `phidata-2.0.0.dev8/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/workspace/operator.py` & `phidata-2.0.0.dev8/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phi/workspace/settings.py` & `phidata-2.0.0.dev8/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/airflow/operators/empty.py` & `phidata-2.0.0.dev8/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_base.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_flower.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_manager.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_scheduler.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_webserver.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/airflow/airflow_worker.py` & `phidata-2.0.0.dev8/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/alertmanager/alertmanager.py` & `phidata-2.0.0.dev8/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/amundsen/frontend.py` & `phidata-2.0.0.dev8/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/amundsen/metadata.py` & `phidata-2.0.0.dev8/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/amundsen/search.py` & `phidata-2.0.0.dev8/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/assistant/assistant.py` & `phidata-2.0.0.dev8/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/aws_app.py` & `phidata-2.0.0.dev8/phidata/app/aws_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/base_app.py` & `phidata-2.0.0.dev8/phidata/app/base_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/cadvisor/cadvisor.py` & `phidata-2.0.0.dev8/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/databox/databox.py` & `phidata-2.0.0.dev8/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/db/base_db.py` & `phidata-2.0.0.dev8/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/django/django_app.py` & `phidata-2.0.0.dev8/phidata/app/django/django_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/django/django_backup.py` & `phidata-2.0.0.dev8/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/docker_app.py` & `phidata-2.0.0.dev8/phidata/app/docker_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/elastic/elastic_app.py` & `phidata-2.0.0.dev8/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/elasticsearch/elasticsearch.py` & `phidata-2.0.0.dev8/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/fastapi/fastapi_server.py` & `phidata-2.0.0.dev8/phidata/app/fastapi/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/grafana/grafana.py` & `phidata-2.0.0.dev8/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/group.py` & `phidata-2.0.0.dev8/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter.py` & `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_hub.py` & `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/jupyter/jupyter_lab.py` & `phidata-2.0.0.dev8/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/k8s/app.py` & `phidata-2.0.0.dev8/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/k8s/dir.py` & `phidata-2.0.0.dev8/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/k8s/url.py` & `phidata-2.0.0.dev8/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/k8s_app.py` & `phidata-2.0.0.dev8/phidata/app/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/mysql/mysql_db.py` & `phidata-2.0.0.dev8/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/neo4j/neo4j.py` & `phidata-2.0.0.dev8/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/nodeexporter/nodeexporter.py` & `phidata-2.0.0.dev8/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/phidata_app.py` & `phidata-2.0.0.dev8/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/postgres/postgres_db.py` & `phidata-2.0.0.dev8/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/prometheus/prometheus.py` & `phidata-2.0.0.dev8/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/qdrant/qdrant.py` & `phidata-2.0.0.dev8/phidata/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/redis/redis.py` & `phidata-2.0.0.dev8/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/redis/stack.py` & `phidata-2.0.0.dev8/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/server/api_server.py` & `phidata-2.0.0.dev8/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/server/server_base.py` & `phidata-2.0.0.dev8/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/spark/spark_base.py` & `phidata-2.0.0.dev8/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/spark/spark_driver.py` & `phidata-2.0.0.dev8/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/spark/spark_worker.py` & `phidata-2.0.0.dev8/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/streamlit/streamlit_app.py` & `phidata-2.0.0.dev8/phidata/app/streamlit/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/superset/superset_base.py` & `phidata-2.0.0.dev8/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/superset/superset_init.py` & `phidata-2.0.0.dev8/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/superset/superset_webserver.py` & `phidata-2.0.0.dev8/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/superset/superset_worker.py` & `phidata-2.0.0.dev8/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/superset/superset_worker_beat.py` & `phidata-2.0.0.dev8/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/traefik/crds.py` & `phidata-2.0.0.dev8/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/traefik/ingress_route.py` & `phidata-2.0.0.dev8/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/app/traefik/router.py` & `phidata-2.0.0.dev8/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/asset/aws/aws_asset.py` & `phidata-2.0.0.dev8/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/asset/data_asset.py` & `phidata-2.0.0.dev8/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/asset/local/file.py` & `phidata-2.0.0.dev8/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/asset/local/local_asset.py` & `phidata-2.0.0.dev8/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/api_client.py` & `phidata-2.0.0.dev8/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/athena/query.py` & `phidata-2.0.0.dev8/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/config.py` & `phidata-2.0.0.dev8/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/create/iam/eks_admin_role.py` & `phidata-2.0.0.dev8/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/create/iam/role.py` & `phidata-2.0.0.dev8/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/driver.py` & `phidata-2.0.0.dev8/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/enums/manager_status.py` & `phidata-2.0.0.dev8/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/manager.py` & `phidata-2.0.0.dev8/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/acm/certificate.py` & `phidata-2.0.0.dev8/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/athena/query.py` & `phidata-2.0.0.dev8/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/base.py` & `phidata-2.0.0.dev8/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/cloudformation/stack.py` & `phidata-2.0.0.dev8/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ec2/security_group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ec2/subnet.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ec2/volume.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ecs/cluster.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ecs/container.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ecs/service.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ecs/task_definition.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/ecs/volume.py` & `phidata-2.0.0.dev8/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/eks/addon.py` & `phidata-2.0.0.dev8/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/eks/cluster.py` & `phidata-2.0.0.dev8/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/eks/fargate_profile.py` & `phidata-2.0.0.dev8/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/eks/kubeconfig.py` & `phidata-2.0.0.dev8/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/eks/node_group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/elasticache/cluster.py` & `phidata-2.0.0.dev8/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/elb/listener.py` & `phidata-2.0.0.dev8/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/elb/load_balancer.py` & `phidata-2.0.0.dev8/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/elb/target_group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/emr/cluster.py` & `phidata-2.0.0.dev8/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/glue/crawler.py` & `phidata-2.0.0.dev8/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/iam/group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/iam/policy.py` & `phidata-2.0.0.dev8/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/iam/role.py` & `phidata-2.0.0.dev8/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_cluster.py` & `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_instance.py` & `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-2.0.0.dev8/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/s3/bucket.py` & `phidata-2.0.0.dev8/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/secret/manager.py` & `phidata-2.0.0.dev8/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/secret/reader.py` & `phidata-2.0.0.dev8/phidata/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/types.py` & `phidata-2.0.0.dev8/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/resource/utils.py` & `phidata-2.0.0.dev8/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/s3/csv_dataset.py` & `phidata-2.0.0.dev8/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/s3/dataset.py` & `phidata-2.0.0.dev8/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/s3/dataset_base.py` & `phidata-2.0.0.dev8/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/s3/object.py` & `phidata-2.0.0.dev8/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/aws/worker.py` & `phidata-2.0.0.dev8/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/base.py` & `phidata-2.0.0.dev8/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/checks/check.py` & `phidata-2.0.0.dev8/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/checks/not_empty.py` & `phidata-2.0.0.dev8/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/constants.py` & `phidata-2.0.0.dev8/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/decorators/timer.py` & `phidata-2.0.0.dev8/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/decorators/validate_env.py` & `phidata-2.0.0.dev8/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/api_client.py` & `phidata-2.0.0.dev8/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/args.py` & `phidata-2.0.0.dev8/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/config.py` & `phidata-2.0.0.dev8/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/enums.py` & `phidata-2.0.0.dev8/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/manager.py` & `phidata-2.0.0.dev8/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/base.py` & `phidata-2.0.0.dev8/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/container.py` & `phidata-2.0.0.dev8/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/group.py` & `phidata-2.0.0.dev8/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/image.py` & `phidata-2.0.0.dev8/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/network.py` & `phidata-2.0.0.dev8/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/types.py` & `phidata-2.0.0.dev8/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/utils.py` & `phidata-2.0.0.dev8/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/resource/volume.py` & `phidata-2.0.0.dev8/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/utils/container.py` & `phidata-2.0.0.dev8/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/docker/worker.py` & `phidata-2.0.0.dev8/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/infra/args.py` & `phidata-2.0.0.dev8/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/infra/config.py` & `phidata-2.0.0.dev8/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/infra/resource.py` & `phidata-2.0.0.dev8/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/api_client.py` & `phidata-2.0.0.dev8/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/args.py` & `phidata-2.0.0.dev8/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/config.py` & `phidata-2.0.0.dev8/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev8/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/apps/v1/deployment.py` & `phidata-2.0.0.dev8/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/common/port.py` & `phidata-2.0.0.dev8/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/config_map.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/container.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/namespace.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/secret.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/service_account.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/core/v1/volume.py` & `phidata-2.0.0.dev8/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-2.0.0.dev8/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/group.py` & `phidata-2.0.0.dev8/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/kubeconfig.py` & `phidata-2.0.0.dev8/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev8/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev8/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev8/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/enums/api_version.py` & `phidata-2.0.0.dev8/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/enums/kind.py` & `phidata-2.0.0.dev8/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/enums/manager_status.py` & `phidata-2.0.0.dev8/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/enums/pv.py` & `phidata-2.0.0.dev8/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/manager.py` & `phidata-2.0.0.dev8/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/base.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/config_map.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/container.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/namespace.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/secret.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/service_account.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/toleration.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/group.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/kubeconfig.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/types.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/resource/utils.py` & `phidata-2.0.0.dev8/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/utils/pod.py` & `phidata-2.0.0.dev8/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/k8s/worker.py` & `phidata-2.0.0.dev8/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/agent.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/chain.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/connection.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/loader.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/query.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/llm/duckdb/tool.py` & `phidata-2.0.0.dev8/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/product/data_product.py` & `phidata-2.0.0.dev8/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/local/csv.py` & `phidata-2.0.0.dev8/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/local/local_table.py` & `phidata-2.0.0.dev8/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/local/parquet.py` & `phidata-2.0.0.dev8/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/s3/csv.py` & `phidata-2.0.0.dev8/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/s3/parquet.py` & `phidata-2.0.0.dev8/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/s3/s3_table.py` & `phidata-2.0.0.dev8/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/sql/postgres.py` & `phidata-2.0.0.dev8/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/table/sql/sql_table.py` & `phidata-2.0.0.dev8/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/aws/athena/run_query.py` & `phidata-2.0.0.dev8/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/aws/emr/create_cluster.py` & `phidata-2.0.0.dev8/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/aws/emr/delete_cluster.py` & `phidata-2.0.0.dev8/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/aws/glue/start_crawler.py` & `phidata-2.0.0.dev8/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/decorator.py` & `phidata-2.0.0.dev8/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/download/s3/to_file.py` & `phidata-2.0.0.dev8/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/download/url/to_file.py` & `phidata-2.0.0.dev8/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/download/url/to_s3.py` & `phidata-2.0.0.dev8/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/download/url/to_sql.py` & `phidata-2.0.0.dev8/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/plot/sql/query.py` & `phidata-2.0.0.dev8/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/python_task.py` & `phidata-2.0.0.dev8/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/run/sql/query.py` & `phidata-2.0.0.dev8/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/task.py` & `phidata-2.0.0.dev8/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/task_relatives.py` & `phidata-2.0.0.dev8/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/upload/file/to_s3.py` & `phidata-2.0.0.dev8/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/task/upload/file/to_sql.py` & `phidata-2.0.0.dev8/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/types/airflow.py` & `phidata-2.0.0.dev8/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/types/context.py` & `phidata-2.0.0.dev8/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/types/phidata_runtime.py` & `phidata-2.0.0.dev8/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/cli_console.py` & `phidata-2.0.0.dev8/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/common.py` & `phidata-2.0.0.dev8/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/compare.py` & `phidata-2.0.0.dev8/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/context.py` & `phidata-2.0.0.dev8/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/dttm.py` & `phidata-2.0.0.dev8/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/enums.py` & `phidata-2.0.0.dev8/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/env_file.py` & `phidata-2.0.0.dev8/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/env_var.py` & `phidata-2.0.0.dev8/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/filesystem.py` & `phidata-2.0.0.dev8/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/get_python_objects_from_module.py` & `phidata-2.0.0.dev8/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/json_io.py` & `phidata-2.0.0.dev8/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/k8s.py` & `phidata-2.0.0.dev8/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/log.py` & `phidata-2.0.0.dev8/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/print_table.py` & `phidata-2.0.0.dev8/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/workspace_path.py` & `phidata-2.0.0.dev8/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/utils/yaml_io.py` & `phidata-2.0.0.dev8/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/workflow/decorator.py` & `phidata-2.0.0.dev8/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/workflow/workflow.py` & `phidata-2.0.0.dev8/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/workflow/workflow_relatives.py` & `phidata-2.0.0.dev8/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/workspace/config.py` & `phidata-2.0.0.dev8/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata/workspace/settings.py` & `phidata-2.0.0.dev8/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/phidata.egg-info/PKG-INFO` & `phidata-2.0.0.dev8/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev7
+Version: 2.0.0.dev8
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
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev7 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev8 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev7/phidata.egg-info/SOURCES.txt` & `phidata-2.0.0.dev8/phidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev7/pyproject.toml` & `phidata-2.0.0.dev8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.0.0.dev7"
+version = "2.0.0.dev8"
 description = "A toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```

