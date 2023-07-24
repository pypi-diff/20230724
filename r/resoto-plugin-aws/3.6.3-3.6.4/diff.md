# Comparing `tmp/resoto-plugin-aws-3.6.3.tar.gz` & `tmp/resoto-plugin-aws-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.6.3.tar", last modified: Mon Jul 24 12:16:22 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.6.4.tar", last modified: Mon Jul 24 18:32:45 2023, max compression
```

## Comparing `resoto-plugin-aws-3.6.3.tar` & `resoto-plugin-aws-3.6.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.963933 resoto-plugin-aws-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 12:16:22.963933 resoto-plugin-aws-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.927932 resoto-plugin-aws-3.6.3/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.931933 resoto-plugin-aws-3.6.3/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.943933 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    19802 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   122318 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.931933 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:11:24.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 12:16:22.000000 resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 12:16:22.963933 resoto-plugin-aws-3.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.947933 resoto-plugin-aws-3.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:16:22.963933 resoto-plugin-aws-3.6.3/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 12:10:50.000000 resoto-plugin-aws-3.6.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.654960 resoto-plugin-aws-3.6.4/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16289 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.658961 resoto-plugin-aws-3.6.4/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.662961 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27876 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19802 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122318 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78300 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22914 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31557 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234332 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13590 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.658961 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:27:43.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-24 18:32:45.000000 resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.662961 resoto-plugin-aws-3.6.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:32:45.666961 resoto-plugin-aws-3.6.4/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-24 18:27:03.000000 resoto-plugin-aws-3.6.4/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.6.3/PKG-INFO` & `resoto-plugin-aws-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.3
+Version: 3.6.4
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.3/README.md` & `resoto-plugin-aws-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/pyproject.toml` & `resoto-plugin-aws-3.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws"
-version = "3.6.3"
+version = "3.6.4"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.3",
+    "resotolib==3.6.4",
     "resotodata",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,31 +452,61 @@
         raise interesting_exception
     else:
         raise botocore.exceptions.NoCredentialsError()
 
 
 def set_account_names(accounts: List[AwsAccount]) -> None:
     def set_account_name(account: AwsAccount) -> None:
-        try:
-            account_aliases = (
-                aws_session(account=account.id, role=account.role, profile=account.profile, partition=account.partition)
-                .client("iam")
-                .list_account_aliases()
-                .get("AccountAliases", [])
-            )
-            if len(account_aliases) > 0:
-                account.name = account_aliases[0]
-        except Exception:
-            pass
+        def set_name_from_account_alias() -> bool:
+            try:
+                account_aliases = (
+                    aws_session(
+                        account=account.id, role=account.role, profile=account.profile, partition=account.partition
+                    )
+                    .client("iam")
+                    .list_account_aliases()
+                    .get("AccountAliases", [])
+                )
+                if len(account_aliases) > 0:
+                    account.name = account_aliases[0]
+                    log.debug(f"Set name for {account.kdname} from account alias")
+                    return True
+            except Exception:
+                pass
+            return False
+
+        def set_name_from_org() -> bool:
+            try:
+                scrape_org_role_arn = Config.aws.scrape_org_role_arn
+                if scrape_org_role_arn is not None and len(str(scrape_org_role_arn).strip()) == 0:
+                    scrape_org_role_arn = None
+                account_name = (
+                    aws_session(profile=account.profile, partition=account.partition, role_arn=scrape_org_role_arn)
+                    .client("organizations")
+                    .describe_account(AccountId=account.id)["Account"]["Name"]
+                )
+                account.name = account_name
+                log.debug(f"Set name for {account.kdname} from organization")
+                return True
+            except Exception:
+                pass
+            return False
+
+        if Config.aws.prefer_account_alias_as_name:
+            if not set_name_from_account_alias():
+                set_name_from_org()
+        else:
+            if not set_name_from_org():
+                set_name_from_account_alias()
 
     if len(accounts) == 0:
         return
 
     max_workers = len(accounts) if len(accounts) < Config.aws.account_pool_size else Config.aws.account_pool_size
-    with futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+    with futures.ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix="aws_account_name_finder") as executor:
         executor.map(set_account_name, accounts)
 
 
 def get_accounts(core_feedback: CoreFeedback) -> List[AwsAccount]:
     accounts = []
     profiles: Sequence[Optional[str]] = [None]
     config: AwsConfig = Config.aws
```

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,22 @@
     scrape_org_role_arn: Optional[str] = field(
         default=None,
         metadata={
             "description": "Role ARN to assume when listing AWS org accounts. If set to null Resoto will use the"
             " default credentials it was started with to call organizations:ListAccounts"
         },
     )
+    prefer_account_alias_as_name: bool = field(
+        default=True,
+        metadata={
+            "description": "Prefer the account alias as the account name instead of organization."
+            " If set to false, Resoto will try to use the organization name. If scrape_org_role_arn is defined,"
+            " the role will be assumed when calling organizations:DescribeAccount."
+        },
+    )
     fork_process: bool = field(
         default=True,
         metadata={
             "description": "Fork collector process instead of using threads. "
             "Recommended if you want to scrape many accounts in parallel."
         },
     )
```

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.6.3
+Version: 3.6.4
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-3.6.3/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.6.4/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/__init__.py` & `resoto-plugin-aws-3.6.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/aws_client_test.py` & `resoto-plugin-aws-3.6.4/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/collector_test.py` & `resoto-plugin-aws-3.6.4/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/configuration_test.py` & `resoto-plugin-aws-3.6.4/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/graphbuilder_test.py` & `resoto-plugin-aws-3.6.4/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/__init__.py` & `resoto-plugin-aws-3.6.4/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.6.4/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/athena_test.py` & `resoto-plugin-aws-3.6.4/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.6.4/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/base_test.py` & `resoto-plugin-aws-3.6.4/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.6.4/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.6.4/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.6.4/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.6.4/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/cognito_test.py` & `resoto-plugin-aws-3.6.4/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.6.4/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/ec2_test.py` & `resoto-plugin-aws-3.6.4/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/ecs_test.py` & `resoto-plugin-aws-3.6.4/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/eks_test.py` & `resoto-plugin-aws-3.6.4/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.6.4/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.6.4/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/elb_test.py` & `resoto-plugin-aws-3.6.4/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.6.4/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/glacier_test.py` & `resoto-plugin-aws-3.6.4/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/iam_test.py` & `resoto-plugin-aws-3.6.4/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.6.4/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/kms_test.py` & `resoto-plugin-aws-3.6.4/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/lambda_test.py` & `resoto-plugin-aws-3.6.4/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/pricing_test.py` & `resoto-plugin-aws-3.6.4/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/rds_test.py` & `resoto-plugin-aws-3.6.4/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/redshift_test.py` & `resoto-plugin-aws-3.6.4/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/route53_test.py` & `resoto-plugin-aws-3.6.4/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/s3_test.py` & `resoto-plugin-aws-3.6.4/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.6.4/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.6.4/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/sns_test.py` & `resoto-plugin-aws-3.6.4/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/resources/sqs_test.py` & `resoto-plugin-aws-3.6.4/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.6.3/test/test_utils.py` & `resoto-plugin-aws-3.6.4/test/test_utils.py`

 * *Files identical despite different names*

