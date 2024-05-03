# Comparing `tmp/boto_formatter-1.0.0.tar.gz` & `tmp/boto_formatter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Abhijit\AWS\GIT-Publishing\repository\boto-formatter\dist\.tmp-4gtf46ed\boto_formatter-1.0.0.tar", last modified: Thu Feb 16 22:14:32 2023, max compression
+gzip compressed data, was "boto_formatter-2.0.0.tar", last modified: Fri May  3 01:29:24 2024, max compression
```

## Comparing `boto_formatter-1.0.0.tar` & `boto_formatter-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.969120 boto_formatter-1.0.0/
--rw-rw-rw-   0        0        0      960 2023-02-10 22:02:20.000000 boto_formatter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      150 2023-01-25 15:35:24.000000 boto_formatter-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11442 2023-02-16 22:14:32.966129 boto_formatter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10910 2023-02-14 18:42:26.000000 boto_formatter-1.0.0/README.md
--rw-rw-rw-   0        0        0      614 2023-02-10 22:30:30.000000 boto_formatter-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-16 22:14:32.971136 boto_formatter-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.513340 boto_formatter-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.585465 boto_formatter-1.0.0/src/boto_formatter/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 boto_formatter-1.0.0/src/boto_formatter/__init__.py
--rw-rw-rw-   0        0        0     7563 2023-01-31 02:56:16.000000 boto_formatter-1.0.0/src/boto_formatter/core_formatter.py
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.652227 boto_formatter-1.0.0/src/boto_formatter/json_util/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 boto_formatter-1.0.0/src/boto_formatter/json_util/__init__.py
--rw-rw-rw-   0        0        0    10769 2023-01-30 03:32:28.000000 boto_formatter-1.0.0/src/boto_formatter/json_util/json_util.py
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.674627 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/__init__.py
--rw-rw-rw-   0        0        0     5848 2022-12-29 03:55:50.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_config.py
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.955579 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/
--rw-rw-rw-   0        0        0        0 2022-08-09 21:49:41.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
--rw-rw-rw-   0        0        0     1086 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/apigateway.json
--rw-rw-rw-   0        0        0     2104 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/budgets.json
--rw-rw-rw-   0        0        0    10697 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudfront.json
--rw-rw-rw-   0        0        0      623 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
--rw-rw-rw-   0        0        0     1350 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
--rw-rw-rw-   0        0        0      643 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/codecommit.json
--rw-rw-rw-   0        0        0       73 2023-01-27 22:09:30.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
--rw-rw-rw-   0        0        0      555 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/dynamodb.json
--rw-rw-rw-   0        0        0    34336 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/ec2.json
--rw-rw-rw-   0        0        0     1510 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/ecs.json
--rw-rw-rw-   0        0        0     1464 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/efs.json
--rw-rw-rw-   0        0        0     3576 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/eks.json
--rw-rw-rw-   0        0        0     4475 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/elasticache.json
--rw-rw-rw-   0        0        0     1594 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/elbv2.json
--rw-rw-rw-   0        0        0     1795 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
--rw-rw-rw-   0        0        0     5490 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/emr.json
--rw-rw-rw-   0        0        0     7276 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/iam.json
--rw-rw-rw-   0        0        0      585 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/kms.json
--rw-rw-rw-   0        0        0     3425 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/lambda.json
--rw-rw-rw-   0        0        0     1447 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/organizations.json
--rw-rw-rw-   0        0        0    17897 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/rds.json
--rw-rw-rw-   0        0        0     2630 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
--rw-rw-rw-   0        0        0     7405 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift.json
--rw-rw-rw-   0        0        0     3129 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/route53.json
--rw-rw-rw-   0        0        0     1753 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/route53domains.json
--rw-rw-rw-   0        0        0     2526 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/s3.json
--rw-rw-rw-   0        0        0     1212 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/sns.json
--rw-rw-rw-   0        0        0      548 2023-01-31 18:54:37.000000 boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/sqs.json
--rw-rw-rw-   0        0        0     7408 2023-01-31 03:03:40.000000 boto_formatter-1.0.0/src/boto_formatter/service_formatter.py
-drwxrwxrwx   0        0        0        0 2023-02-16 22:14:32.632735 boto_formatter-1.0.0/src/boto_formatter.egg-info/
--rw-rw-rw-   0        0        0    11442 2023-02-16 22:14:32.000000 boto_formatter-1.0.0/src/boto_formatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2023-02-16 22:14:32.000000 boto_formatter-1.0.0/src/boto_formatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 22:14:32.000000 boto_formatter-1.0.0/src/boto_formatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-16 22:14:32.000000 boto_formatter-1.0.0/src/boto_formatter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.778849 boto_formatter-2.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.613073 boto_formatter-2.0.0/.venv/
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.613714 boto_formatter-2.0.0/.venv/Lib/
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.614230 boto_formatter-2.0.0/.venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.632699 boto_formatter-2.0.0/.venv/Lib/site-packages/boto_formatter-2.0.0.dist-info/
+-rw-rw-rw-   0        0        0       84 2024-05-03 01:28:55.000000 boto_formatter-2.0.0/.venv/Lib/site-packages/boto_formatter-2.0.0.dist-info/direct_url.json
+-rw-rw-rw-   0        0        0      945 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      147 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    47943 2024-05-03 01:29:24.775536 boto_formatter-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    46912 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/README.md
+-rw-rw-rw-   0        0        0      592 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 01:29:24.779850 boto_formatter-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.616459 boto_formatter-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.645678 boto_formatter-2.0.0/src/boto_formatter/
+-rw-rw-rw-   0        0        0        0 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/__init__.py
+-rw-rw-rw-   0        0        0    23537 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/boto_magic_formatter.py
+-rw-rw-rw-   0        0        0     7384 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/core_formatter.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.662573 boto_formatter-2.0.0/src/boto_formatter/json_util/
+-rw-rw-rw-   0        0        0        0 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/json_util/__init__.py
+-rw-rw-rw-   0        0        0    10623 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/json_util/json_util.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.667222 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/
+-rw-rw-rw-   0        0        0        0 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.765439 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/
+-rw-rw-rw-   0        0        0     4119 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
+-rw-rw-rw-   0        0        0      752 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/account.json
+-rw-rw-rw-   0        0        0     1434 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/acm.json
+-rw-rw-rw-   0        0        0     2292 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/amp.json
+-rw-rw-rw-   0        0        0     1257 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/apigateway.json
+-rw-rw-rw-   0        0        0     2589 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/budgets.json
+-rw-rw-rw-   0        0        0     1150 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cleanrooms.json
+-rw-rw-rw-   0        0        0     2290 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudformation.json
+-rw-rw-rw-   0        0        0    11045 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudfront.json
+-rw-rw-rw-   0        0        0      794 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
+-rw-rw-rw-   0        0        0     1692 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
+-rw-rw-rw-   0        0        0      814 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/codecommit.json
+-rw-rw-rw-   0        0        0      726 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/dynamodb.json
+-rw-rw-rw-   0        0        0    37267 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/ec2.json
+-rw-rw-rw-   0        0        0     2772 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/ecs.json
+-rw-rw-rw-   0        0        0     1635 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/efs.json
+-rw-rw-rw-   0        0        0     4746 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/eks.json
+-rw-rw-rw-   0        0        0     4646 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/elasticache.json
+-rw-rw-rw-   0        0        0     1765 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/elbv2.json
+-rw-rw-rw-   0        0        0     2504 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/emr-serverless.json
+-rw-rw-rw-   0        0        0     6531 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/emr.json
+-rw-rw-rw-   0        0        0    10370 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/iam.json
+-rw-rw-rw-   0        0        0      756 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/kms.json
+-rw-rw-rw-   0        0        0     3767 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/lambda.json
+-rw-rw-rw-   0        0        0     2114 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/organizations.json
+-rw-rw-rw-   0        0        0    18752 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/rds.json
+-rw-rw-rw-   0        0        0     2972 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
+-rw-rw-rw-   0        0        0     7576 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift.json
+-rw-rw-rw-   0        0        0     1376 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/resourcegroupstaggingapi.json
+-rw-rw-rw-   0        0        0     5171 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/route53.json
+-rw-rw-rw-   0        0        0     2093 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/route53domains.json
+-rw-rw-rw-   0        0        0    10235 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/s3.json
+-rw-rw-rw-   0        0        0     4338 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sagemaker.json
+-rw-rw-rw-   0        0        0     1554 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sns.json
+-rw-rw-rw-   0        0        0      719 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sqs.json
+-rw-rw-rw-   0        0        0     1643 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/ssm.json
+-rw-rw-rw-   0        0        0     7238 2024-05-03 00:33:18.000000 boto_formatter-2.0.0/src/boto_formatter/service_formatter.py
+drwxrwxrwx   0        0        0        0 2024-05-03 01:29:24.772535 boto_formatter-2.0.0/src/boto_formatter.egg-info/
+-rw-rw-rw-   0        0        0    47943 2024-05-03 01:29:24.000000 boto_formatter-2.0.0/src/boto_formatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3064 2024-05-03 01:29:24.000000 boto_formatter-2.0.0/src/boto_formatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 01:29:24.000000 boto_formatter-2.0.0/src/boto_formatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 01:29:24.000000 boto_formatter-2.0.0/src/boto_formatter.egg-info/top_level.txt
```

### Comparing `boto_formatter-1.0.0/LICENSE` & `boto_formatter-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-MIT No Attribution
-
-Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+MIT No Attribution
+
+Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/core_formatter.py` & `boto_formatter-2.0.0/src/boto_formatter/core_formatter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-import logging
-from sys import modules
-import os
-import boto_formatter.json_util.json_util as json_util
-from boto_formatter.service_config_mgr.service_config import ServiceConfig
-
-
-# Set up our logger
-logging.basicConfig(level=logging.ERROR)
-logger = logging.getLogger()
-
-
-def boto_response_formatter(service_name, function_name, **kwargs):
-    """
-     boto core response formatter
-    :param service_name: example lambda, s3
-    :param function_name: example list_functions
-    :param format_type: json or csv
-    :param output_to: print or file
-    :param output_path: file output path
-    :param pagination: result is generated through pagination
-    :param required_only: format result for required only columns
-    :return: formatted response
-    """
-    required_only = None  # Default is none if required only fields
-    format_type = None  # Options are json or csv. Default is json
-    output_to = None  # Options are print or file. Default is print
-    output_path = None  # Default is none, user can provide custom path
-    prefix_columns = None
-    pagination = None
-
-    # FORMAT_1 : JSON single record
-    # FORMAT_2 : JSON contains List of JSON
-    # FORMAT_3 : JSON contains List of Strings
-    COMMON_FORMAT = "FORMAT_2"
-
-    # default type is json. Supported types are json,csv
-    if "format_type" in kwargs:
-        format_type = kwargs["format_type"].lower()
-    # output_to default is None. Supported options are cmd,file,s3
-    if "output_to" in kwargs:
-        output_to = kwargs["output_to"]
-    # output_to default is None. Supported options are complete file path or S3 path
-    if "output_path" in kwargs:
-        output_path = kwargs["output_path"]
-    if "prefix_columns" in kwargs:
-        prefix_columns = kwargs["prefix_columns"]
-    if "pagination" in kwargs:
-        pagination = True
-    if "required_only" in kwargs:
-        required_only = "Yes"
-
-    def format_decorator(f):
-
-        def wrapped(*args, **kwargs):
-            response = f(*args, **kwargs)
-            # If output_path is not provided set as invoking function directory path
-            func_dir_path = None
-            try:
-                func_dir_path = os.path.dirname(
-                    os.path.abspath(modules[f.__module__].__file__))
-            except AttributeError as err:
-                logger.error(err)
-                logger.debug(
-                    "running from command prompt")
-                func_dir_path = os.getcwd()
-
-            logger.debug("Function directory Path : {}".format(func_dir_path))
-            json_config = None
-            result = None
-            function_config = ServiceConfig.get_service_function_details(
-                service_name, function_name)
-
-            json_config = function_config["json_response"]
-            response_format = function_config["response_format"]
-            # Some columns breaks as comma so for csv format put required only condition
-
-            result = __process_service_func_response(
-                function_config, json_config, format_type, required_only, response, prefix_columns, pagination)
-            # default result is in flatten json format.
-            if format_type:
-                result = __format_ouput(result, format_type)
-            if output_to:
-                result = __ouput_to(service_name, function_name,
-                                    result, output_to, format_type,
-                                    output_path, func_dir_path, response_format)
-            return result
-        return wrapped
-    return format_decorator
-
-
-def __process_service_func_response(function_config, json_config, format_type, required_only, response, prefix_columns, pagination):
-    """
-    :param function_config : function defined in service_config.json
-    :param json_config: reference response
-    :param format_type: csv,json
-    :param required_only: if present filter the result for required onlydata
-    :param response : response of base function
-    :prefix_columns : Addtional prefix columns to print
-    :pagination :if present json list is part of pagination
-    :return: formatted list of flattend JSON objects
-    """
-    response_format = function_config["response_format"]
-    result_keys = None
-    result = []
-    if "result_keys" in function_config.keys():
-        result_keys = function_config["result_keys"]
-    # Come columns breaks in csv format so added this condition to exclued these columns
-    if required_only is None and format_type is not None:
-        if "csv_enforced_required_only" in function_config.keys() and format_type == "csv":
-            required_only = "Yes"
-    # FORMAT_1 : JSON single record
-    # FORMAT_2 : JSON contains List of JSON
-    # FORMAT_3 : JSON contains List of Strings
-    if response_format == "FORMAT_2":
-        # if pagination then get extended loop
-        if pagination:
-            for obj in response:
-                result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
-                    obj, result_keys), required_only, prefix_columns))
-        else:
-            result = json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
-                response, result_keys), required_only, prefix_columns)
-
-    elif response_format == "FORMAT_1":
-        result = json_util.format_json_object(json_config, response)
-
-    elif response_format == "FORMAT_3":
-        if pagination:
-            for obj in response:
-                result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
-                    obj, result_keys), required_only, prefix_columns))
-        else:
-            result = json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
-                response, result_keys), required_only, prefix_columns)
-    return result
-
-
-def __format_ouput(result, format_type):
-    """
-    :param result : Flatten JSON list
-    :param format_type: currently supported only csv
-    :return: formatted list of comma seperated string
-    """
-    if format_type == "csv":
-        return json_util.get_csv_data(result)
-    else:
-        return result
-
-
-def __ouput_to(service_name, function_name, result, output_to, format_type, output_path, func_dir_path, response_format):
-    """
-    :param service_name :service_name like s3, lambda
-    :param function_name: function name like list_buckets
-    :param function_name: processed result
-    :param format_type: csv or json
-    :param output_path: user provided output_path to save file
-    :param func_dir_path: invoking file directory path
-    :response_format:FORMAT_1,FORMAT_2,FORMAT_3
-    :return: formatted list of comma seperated string
-    """
-    if output_to == "print":
-        return json_util.print_csv_response(result)
-    elif output_to == "file" or output_to == "s3":
-        if output_path is None:
-            output_path = func_dir_path
-            logging.debug("Directory Path : {}".format(output_path))
-        if format_type:
-            file_path = None
-            if format_type == "csv":
-                file_path = json_util.save_csv(
-                    result, service_name, function_name, output_path)
-            else:
-                file_path = json_util.save_json(
-                    result, service_name, function_name, output_path)
-
-        return file_path
-    else:
-        return result
+import logging
+from sys import modules
+import os
+import boto_formatter.json_util.json_util as json_util
+from boto_formatter.service_config_mgr.service_config import ServiceConfig
+
+
+# Set up our logger
+logging.basicConfig(level=logging.ERROR)
+logger = logging.getLogger()
+
+
+def boto_response_formatter(service_name, function_name, **kwargs):
+    """
+     boto core response formatter
+    :param service_name: example lambda, s3
+    :param function_name: example list_functions
+    :param format_type: json or csv
+    :param output_to: print or file
+    :param output_path: file output path
+    :param pagination: result is generated through pagination
+    :param required_only: format result for required only columns
+    :return: formatted response
+    """
+    required_only = None  # Default is none if required only fields
+    format_type = None  # Options are json or csv. Default is json
+    output_to = None  # Options are print or file. Default is print
+    output_path = None  # Default is none, user can provide custom path
+    prefix_columns = None
+    pagination = None
+
+    # FORMAT_1 : JSON single record
+    # FORMAT_2 : JSON contains List of JSON
+    # FORMAT_3 : JSON contains List of Strings
+    COMMON_FORMAT = "FORMAT_2"
+
+    # default type is json. Supported types are json,csv
+    if "format_type" in kwargs:
+        format_type = kwargs["format_type"].lower()
+    # output_to default is None. Supported options are cmd,file,s3
+    if "output_to" in kwargs:
+        output_to = kwargs["output_to"]
+    # output_to default is None. Supported options are complete file path or S3 path
+    if "output_path" in kwargs:
+        output_path = kwargs["output_path"]
+    if "prefix_columns" in kwargs:
+        prefix_columns = kwargs["prefix_columns"]
+    if "pagination" in kwargs:
+        pagination = True
+    if "required_only" in kwargs:
+        required_only = "Yes"
+
+    def format_decorator(f):
+
+        def wrapped(*args, **kwargs):
+            response = f(*args, **kwargs)
+            # If output_path is not provided set as invoking function directory path
+            func_dir_path = None
+            try:
+                func_dir_path = os.path.dirname(
+                    os.path.abspath(modules[f.__module__].__file__))
+            except AttributeError as err:
+                logger.error(err)
+                logger.debug(
+                    "running from command prompt")
+                func_dir_path = os.getcwd()
+
+            logger.debug("Function directory Path : {}".format(func_dir_path))
+            json_config = None
+            result = None
+            function_config = ServiceConfig.get_service_function_details(
+                service_name, function_name)
+
+            json_config = function_config["json_response"]
+            response_format = function_config["response_format"]
+            # Some columns breaks as comma so for csv format put required only condition
+
+            result = __process_service_func_response(
+                function_config, json_config, format_type, required_only, response, prefix_columns, pagination)
+            # default result is in flatten json format.
+            if format_type:
+                result = __format_ouput(result, format_type)
+            if output_to:
+                result = __ouput_to(service_name, function_name,
+                                    result, output_to, format_type,
+                                    output_path, func_dir_path, response_format)
+            return result
+        return wrapped
+    return format_decorator
+
+
+def __process_service_func_response(function_config, json_config, format_type, required_only, response, prefix_columns, pagination):
+    """
+    :param function_config : function defined in service_config.json
+    :param json_config: reference response
+    :param format_type: csv,json
+    :param required_only: if present filter the result for required onlydata
+    :param response : response of base function
+    :prefix_columns : Addtional prefix columns to print
+    :pagination :if present json list is part of pagination
+    :return: formatted list of flattend JSON objects
+    """
+    response_format = function_config["response_format"]
+    result_keys = None
+    result = []
+    if "result_keys" in function_config.keys():
+        result_keys = function_config["result_keys"]
+    # Come columns breaks in csv format so added this condition to exclued these columns
+    if required_only is None and format_type is not None:
+        if "csv_enforced_required_only" in function_config.keys() and format_type == "csv":
+            required_only = "Yes"
+    # FORMAT_1 : JSON single record
+    # FORMAT_2 : JSON contains List of JSON
+    # FORMAT_3 : JSON contains List of Strings
+    if response_format == "FORMAT_2":
+        # if pagination then get extended loop
+        if pagination:
+            for obj in response:
+                result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
+                    obj, result_keys), required_only, prefix_columns))
+        else:
+            result = json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
+                response, result_keys), required_only, prefix_columns)
+
+    elif response_format == "FORMAT_1":
+        result = json_util.format_json_object(json_config, response)
+
+    elif response_format == "FORMAT_3":
+        if pagination:
+            for obj in response:
+                result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
+                    obj, result_keys), required_only, prefix_columns))
+        else:
+            result = json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
+                response, result_keys), required_only, prefix_columns)
+    return result
+
+
+def __format_ouput(result, format_type):
+    """
+    :param result : Flatten JSON list
+    :param format_type: currently supported only csv
+    :return: formatted list of comma seperated string
+    """
+    if format_type == "csv":
+        return json_util.get_csv_data(result)
+    else:
+        return result
+
+
+def __ouput_to(service_name, function_name, result, output_to, format_type, output_path, func_dir_path, response_format):
+    """
+    :param service_name :service_name like s3, lambda
+    :param function_name: function name like list_buckets
+    :param function_name: processed result
+    :param format_type: csv or json
+    :param output_path: user provided output_path to save file
+    :param func_dir_path: invoking file directory path
+    :response_format:FORMAT_1,FORMAT_2,FORMAT_3
+    :return: formatted list of comma seperated string
+    """
+    if output_to == "print":
+        return json_util.print_csv_response(result)
+    elif output_to == "file" or output_to == "s3":
+        if output_path is None:
+            output_path = func_dir_path
+            logging.debug("Directory Path : {}".format(output_path))
+        if format_type:
+            file_path = None
+            if format_type == "csv":
+                file_path = json_util.save_csv(
+                    result, service_name, function_name, output_path)
+            else:
+                file_path = json_util.save_json(
+                    result, service_name, function_name, output_path)
+
+        return file_path
+    else:
+        return result
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/json_util/json_util.py` & `boto_formatter-2.0.0/src/boto_formatter/json_util/json_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,290 +1,292 @@
-"""
-This is general JSON utility
-
-"""
-import datetime
-import os
-import json
-import logging
-logger = logging.getLogger()
-logger.setLevel(logging.ERROR)
-
-
-def flatten_json(y):
-    """
-     Flatten JSON 
-    :param json to be flatten
-    :return: flattend json
-    """
-    output = {}
-
-    def flatten(x, name=''):
-        if type(x) is dict:
-            for a in x:
-                flatten(x[a], name + a + '_')
-        elif type(x) is list:
-            i = 0
-            for a in x:
-                flatten(a, name + str(i) + '_')
-                i += 1
-        else:
-            output[name[:-1]] = x
-    flatten(y)
-    return output
-
-
-def format_response_for_result_keys(json_object_list, result_keys):
-    """
-    Iterate over result keys in JSON to get appropriate List
-    :param json_object_list -JSON object which contains result_key(or Keys)
-    :param result_keys  - List of Keys to be search in JSON
-    :return: List of JSON objects
-    """
-    """"""
-    try:
-        for result_key in result_keys:
-            if len(json_object_list) > 0:
-                json_object_list = json_object_list[result_key]
-    except KeyError as err:
-        # This is to handle when pagination iterate even though there is no record
-        json_object_list = []
-        logger.debug(err)
-        #logger.error(err)
-        #raise ValueError(
-        #    "Result Keys {} not found in provided JSON. Decorator service/function is not matching with boto function".format(result_keys))
-    except TypeError as err:
-        logger.error(err)
-        raise ValueError(
-            "Result List returned by boto3 function is not in correct format or decorator service/function is not matching with boto function")
-    return json_object_list
-
-
-def format_json_list(json_config, json_object_list, required_only, prefix_columns=None):
-    """
-    Prior : 
-    Filter Result Keys
-    Append addtional columns
-    Compare all objects in JSON List with reference json(json_config) and generate list
-    1. Iterate each object in List
-    2. Flatten the object
-    3. Get Keys of reference JSON
-    4. Iterate over reference JSON keys and generate result row
-    5. Update result rows with not found keys (Extra Columns)
-    :param json_config -reference json
-    :param json_object_list  - json list that need to be formatted
-    :param required_only  - if interest is only in required only attributes
-    :param prefix_columns  -if addtional prefix columns you want to add in response
-    :return: return json object list formatted in line with json_config
-    """
-    result_json_list = []
-    json_config_keys = json_config.keys()
-    First_record = True
-    # 1 Take each object in list
-    # 1 Outer Loop
-    # if json_object_list is zero size loop will not execute
-    for json_object_raw in json_object_list:
-        # 2 Flatten the object
-        json_object = flatten_json(json_object_raw)
-        result_row = {}
-        keys_present_list = []
-        # 3 Append Prefix columns values like Account, Region
-        if prefix_columns:
-            for prefix_column_header in prefix_columns.keys():
-                result_row[prefix_column_header] = prefix_columns[prefix_column_header]
-        # 4. Get keys of reference JSON
-        json_object_keys = json_object.keys()
-        # 5 Go Through All the keys of reference JSON
-        for json_config_key in json_config_keys:
-            if json_config_key in json_object_keys:
-                result_row[json_config_key] = str(json_object[json_config_key])
-                keys_present_list.append(json_config_key)
-            else:
-                result_row[json_config_key] = ""
-        # 6. Append Extra Cloumns as pipe seprated Key/Value
-        # If required_only is selected don't need extra columns
-        if not required_only:
-            extra_rows = [
-                i for i in json_object_keys if i not in keys_present_list]
-            for extra_row_key in extra_rows:
-                result_row[extra_row_key] = "{}|{}".format(
-                    extra_row_key, json_object[extra_row_key])
-        # 7 None of key matches for first row raise and exception as it's not valid JSON
-        if First_record:
-            if len(keys_present_list) == 0:
-                raise ValueError(
-                    "Zero record keys are matching. Check the JSON result is appropriate format")
-        First_record = False
-        result_json_list.append(result_row)
-    return result_json_list
-
-
-def format_str_list(json_config, json_object_list, required_only, prefix_columns=None):
-    """
-    Prior : 
-    Filter Result Keys
-    Append addtional columns
-     Iterate each string and convert to JSON 
-
-    :param json_config -reference json
-    :param json_object_list  - json list that need to be formatted
-    :param required_only  - if interest is only in required only attributes
-    :param prefix_columns  -if addtional prefix columns you want to add in response
-    :return: return json object list formatted in line with json_config
-    """
-    result_json_list = []
-    #Ensure first Key is present
-    column_key = list(json_config.keys())[0]
-    # 1 Take each string in list
-    # 1 Outer Loop
-    # if json_object_list is zero size loop will not execute
-    for str_obj in json_object_list:
-        result_row = {}
-        # 2 Append Prefix columns values like Account, Region
-        if prefix_columns:
-            for prefix_column_header in prefix_columns.keys():
-                result_row[prefix_column_header] = prefix_columns[prefix_column_header]
-        # 3. Ensure first Key is present
-        result_row[column_key] = str_obj
-        result_json_list.append(result_row)
-    return result_json_list
-
-
-
-def format_json_object(json_config, json_object_raw):
-    """
-    Compare Json_object with reference json(json_config) and generate JSON Object
-    1. Flatten the object
-    2. Get Keys of reference JSON
-    3. Iterate over reference JSON keys and generate result row
-    4. Update result rows with not found keys (Extra Columns)
-    :param json_config -reference json
-    :param json_object_raw  - json object to be formatted
-    :return: return json object formated in line with json_config
-    """
-    json_config_keys = json_config.keys()
-    # 2 Flatten the object
-    json_object = flatten_json(json_object_raw)
-    result_row = {}
-    keys_present_list = []
-    # 3. Get keys of reference JSON
-    json_object_keys = json_object.keys()
-    # 4 Go Through All the keys of reference JSON
-    for json_config_key in json_config_keys:
-        if json_config_key in json_object_keys:
-            result_row[json_config_key] = str(json_object[json_config_key])
-            keys_present_list.append(json_config_key)
-        else:
-            result_row[json_config_key] = ""
-    # 5. Append Extra Cloumns as pipe seprated Key/Value
-    extra_rows = [i for i in json_object_keys if i not in keys_present_list]
-    for extra_row_key in extra_rows:
-        result_row[extra_row_key] = "{}|{}".format(
-            extra_row_key, json_object[extra_row_key])
-
-    return result_row
-
-
-def get_csv_data(result_json_list):
-    """
-    :param flattend json object list
-    :return: list of comma seperated string
-    """
-    csv_data = []
-    if len(result_json_list) > 0:
-        logger.debug(result_json_list)
-        csv_data.append(",".join(result_json_list[0].keys()))
-        for json_obj in result_json_list:
-            csv_data.append(",".join(json_obj.values()))
-    return csv_data
-
-
-def print_csv_response(csv_data):
-    """
-    :param list of comma seperated string
-    :return: None
-    """
-    for csv_value in csv_data:
-        print(csv_value)
-
-
-def get_output_path():
-    """
-    :return: output_path
-    """
-    dir_path = os.path.dirname(os.path.abspath(__file__))
-    return dir_path
-
-
-def get_file_path(service_name, function_name, dir_path, file_type):
-    """
-     Generate file path based on service_name and function_name
-    :param service_name like s3, lambda
-    :param function_name like list_buckets
-    :return: None
-    """
-    if not os.path.exists(dir_path):
-        ValueError("Invalid Path to store the file  {}".format(dir_path))
-    current_date = datetime.datetime.now().strftime("%d_%m_%Y_%H_%M_%S")
-    file_name = "{}_{}_{}.{}".format(
-        service_name, function_name, current_date, file_type)
-    output_path = os.path.join(dir_path, "output")
-    logger.info("Output directory path {} ".format(output_path))
-    if not os.path.exists(output_path):
-        os.mkdir(output_path)
-    file_path = os.path.join(output_path, file_name)
-    logger.info("File Path {}".format(file_path))
-    return file_path
-
-
-def save_csv(csv_data, service_name, function_name, dir_path):
-    """
-     save file as .csv
-    :param csv_data data in list of comma seperated strings
-    :param service_name like s3, lambda
-    :param function_name like list_buckets
-    :return: None
-    """
-    file_full_path = None
-    if len(csv_data) > 0:
-        file_full_path = get_file_path(
-            service_name, function_name, dir_path, "csv")
-        f = open(file_full_path, "w")
-        for row in csv_data:
-            f.write(row + "\n")
-        print("RESULT : File is generated at location {} ".format(file_full_path))
-    else:
-        print("RESULT : No records . ")
-    return file_full_path
-
-
-def save_json(json_data, service_name, function_name, dir_path=None):
-    """
-     save file as .json
-    :param json_data json formatted data
-    :param service_name like s3, lambda
-    :param function_name like list_buckets
-    :return: None
-    """
-    file_full_path = None
-    if len(json_data) > 0:
-        json_data_list = dict()
-        json_data_list["result"] = json_data
-        file_full_path = get_file_path(
-            service_name, function_name, dir_path, "json")
-        json_data_list = json.dumps(json_data_list, indent=4, default=str)
-        # Writing to sample.json
-        with open(file_full_path, "w") as outfile:
-            outfile.write(json_data_list)
-        print("RESULT : File is generated at location {} ".format(file_full_path))
-    else:
-        print("RESULT : No records . ")
-    return file_full_path
-
-
-def save_file(json_data, service_name, function_name, dir_path=None):
-    file_full_path = get_file_path(
-        service_name, function_name, dir_path, "json")
-    # Writing to sample.json
-    with open(file_full_path, "w") as outfile:
-        outfile.write(json_data)
-    print("RESULT : File is generated at location {} ".format(file_full_path))
+"""
+This is general JSON utility
+
+"""
+import datetime
+import os
+import json
+import logging
+logger = logging.getLogger()
+logger.setLevel(logging.ERROR)
+
+
+def flatten_json(y):
+    """
+     Flatten JSON 
+    :param json to be flatten
+    :return: flattend json
+    """
+    output = {}
+
+    def flatten(x, name=''):
+        if type(x) is dict:
+            for a in x:
+                flatten(x[a], name + a + '_')
+        elif type(x) is list:
+            i = 0
+            for a in x:
+                flatten(a, name + str(i) + '_')
+                i += 1
+        else:
+            output[name[:-1]] = x
+    flatten(y)
+    return output
+
+
+def format_response_for_result_keys(json_object_list, result_keys):
+    """
+    Iterate over result keys in JSON to get appropriate List
+    :param json_object_list -JSON object which contains result_key(or Keys)
+    :param result_keys  - List of Keys to be search in JSON
+    :return: List of JSON objects
+    """
+    """"""
+    try:
+        for result_key in result_keys:
+            if len(json_object_list) > 0:
+                json_object_list = json_object_list[result_key]
+    except KeyError as err:
+        # This is to handle when pagination iterate even though there is no record
+        json_object_list = []
+        logger.debug(err)
+        #logger.error(err)
+        #raise ValueError(
+        #    "Result Keys {} not found in provided JSON. Decorator service/function is not matching with boto function".format(result_keys))
+    except TypeError as err:
+        logger.error(err)
+        raise ValueError(
+            "Result List returned by boto3 function is not in correct format or decorator service/function is not matching with boto function")
+    return json_object_list
+
+
+def format_json_list(json_config, json_object_list, required_only, prefix_columns=None):
+    """
+    Prior : 
+    Filter Result Keys
+    Append addtional columns
+    Compare all objects in JSON List with reference json(json_config) and generate list
+    1. Iterate each object in List
+    2. Flatten the object
+    3. Get Keys of reference JSON
+    4. Iterate over reference JSON keys and generate result row
+    5. Update result rows with not found keys (Extra Columns)
+    :param json_config -reference json
+    :param json_object_list  - json list that need to be formatted
+    :param required_only  - if interest is only in required only attributes
+    :param prefix_columns  -if addtional prefix columns you want to add in response
+    :return: return json object list formatted in line with json_config
+    """
+    result_json_list = []
+    json_config_keys = json_config.keys()
+    First_record = True
+    # 1 Take each object in list
+    # 1 Outer Loop
+    # if json_object_list is zero size loop will not execute
+    for json_object_raw in json_object_list:
+        # 2 Flatten the object
+        json_object = flatten_json(json_object_raw)
+        result_row = {}
+        keys_present_list = []
+        # 3 Append Prefix columns values like Account, Region
+        if prefix_columns:
+            for prefix_column_header in prefix_columns.keys():
+                result_row[prefix_column_header] = prefix_columns[prefix_column_header]
+        # 4. Get keys of reference JSON
+        json_object_keys = json_object.keys()
+        # 5 Go Through All the keys of reference JSON
+        for json_config_key in json_config_keys:
+            if json_config_key in json_object_keys:
+                result_row[json_config_key] = str(json_object[json_config_key])
+                keys_present_list.append(json_config_key)
+            else:
+                result_row[json_config_key] = ""
+        # 6. Append Extra Cloumns as pipe seprated Key/Value
+        # If required_only is selected don't need extra columns
+        if not required_only:
+            extra_rows = [
+                i for i in json_object_keys if i not in keys_present_list]
+            for extra_row_key in extra_rows:
+                result_row[extra_row_key] = "{}|{}".format(
+                    extra_row_key, json_object[extra_row_key])
+        # 7 None of key matches for first row raise and exception as it's not valid JSON
+        if First_record:
+            if len(keys_present_list) == 0:
+                raise ValueError(
+                    "Zero record keys are matching. Check the JSON result is appropriate format")
+        First_record = False
+        result_json_list.append(result_row)
+    return result_json_list
+
+
+def format_str_list(json_config, json_object_list, required_only, prefix_columns=None):
+    """
+    Prior : 
+    Filter Result Keys
+    Append addtional columns
+     Iterate each string and convert to JSON 
+
+    :param json_config -reference json
+    :param json_object_list  - json list that need to be formatted
+    :param required_only  - if interest is only in required only attributes
+    :param prefix_columns  -if addtional prefix columns you want to add in response
+    :return: return json object list formatted in line with json_config
+    """
+    result_json_list = []
+    #Ensure first Key is present
+    column_key = list(json_config.keys())[0]
+    # 1 Take each string in list
+    # 1 Outer Loop
+    # if json_object_list is zero size loop will not execute
+    for str_obj in json_object_list:
+        result_row = {}
+        # 2 Append Prefix columns values like Account, Region
+        if prefix_columns:
+            for prefix_column_header in prefix_columns.keys():
+                result_row[prefix_column_header] = prefix_columns[prefix_column_header]
+        # 3. Ensure first Key is present
+        result_row[column_key] = str_obj
+        result_json_list.append(result_row)
+    return result_json_list
+
+
+
+def format_json_object(json_config, json_object_raw):
+    """
+    Compare Json_object with reference json(json_config) and generate JSON Object
+    1. Flatten the object
+    2. Get Keys of reference JSON
+    3. Iterate over reference JSON keys and generate result row
+    4. Update result rows with not found keys (Extra Columns)
+    :param json_config -reference json
+    :param json_object_raw  - json object to be formatted
+    :return: return json object formated in line with json_config
+    """
+    json_config_keys = json_config.keys()
+    # 2 Flatten the object
+    json_object = flatten_json(json_object_raw)
+    result_row = {}
+    keys_present_list = []
+    # 3. Get keys of reference JSON
+    json_object_keys = json_object.keys()
+    # 4 Go Through All the keys of reference JSON
+    for json_config_key in json_config_keys:
+        if json_config_key in json_object_keys:
+            result_row[json_config_key] = str(json_object[json_config_key])
+            keys_present_list.append(json_config_key)
+        else:
+            result_row[json_config_key] = ""
+    # 5. Append Extra Cloumns as pipe seprated Key/Value
+    extra_rows = [i for i in json_object_keys if i not in keys_present_list]
+    for extra_row_key in extra_rows:
+        result_row[extra_row_key] = "{}|{}".format(
+            extra_row_key, json_object[extra_row_key])
+
+    return result_row
+
+
+def get_csv_data(result_json_list):
+    """
+    :param flattend json object list
+    :return: list of comma seperated string
+    """
+    csv_data = []
+    if len(result_json_list) > 0:
+        logger.debug(result_json_list)
+        csv_data.append(",".join(result_json_list[0].keys()))
+        for json_obj in result_json_list:
+            csv_data.append(",".join(replace_breaking_comma(json_obj.values())))
+    return csv_data
+
+def replace_breaking_comma(json_obj_values):
+    return [obj_value.replace(',', '/n') for obj_value in json_obj_values]
+
+def print_csv_response(csv_data):
+    """
+    :param list of comma seperated string
+    :return: None
+    """
+    for csv_value in csv_data:
+        print(csv_value)
+
+
+def get_output_path():
+    """
+    :return: output_path
+    """
+    dir_path = os.path.dirname(os.path.abspath(__file__))
+    return dir_path
+
+
+def get_file_path(service_name, function_name, dir_path, file_type):
+    """
+     Generate file path based on service_name and function_name
+    :param service_name like s3, lambda
+    :param function_name like list_buckets
+    :return: None
+    """
+    if not os.path.exists(dir_path):
+        ValueError("Invalid Path to store the file  {}".format(dir_path))
+    current_date = datetime.datetime.now().strftime("%d_%m_%Y_%H_%M_%S")
+    file_name = "{}_{}_{}.{}".format(
+        service_name, function_name, current_date, file_type)
+    output_path = os.path.join(dir_path, "output")
+    logger.info("Output directory path {} ".format(output_path))
+    if not os.path.exists(output_path):
+        os.mkdir(output_path)
+    file_path = os.path.join(output_path, file_name)
+    logger.info("File Path {}".format(file_path))
+    return file_path
+
+
+def save_csv(csv_data, service_name, function_name, dir_path):
+    """
+     save file as .csv
+    :param csv_data data in list of comma seperated strings
+    :param service_name like s3, lambda
+    :param function_name like list_buckets
+    :return: None
+    """
+    file_full_path = None
+    if len(csv_data) > 0:
+        file_full_path = get_file_path(
+            service_name, function_name, dir_path, "csv")
+        f = open(file_full_path, "w")
+        for row in csv_data:
+            f.write(row + "\n")
+        print("RESULT : File is generated at location {} ".format(file_full_path))
+    else:
+        print("RESULT : No records . ")
+    return file_full_path
+
+
+def save_json(json_data, service_name, function_name, dir_path=None):
+    """
+     save file as .json
+    :param json_data json formatted data
+    :param service_name like s3, lambda
+    :param function_name like list_buckets
+    :return: None
+    """
+    file_full_path = None
+    if len(json_data) > 0:
+        json_data_list = dict()
+        json_data_list["result"] = json_data
+        file_full_path = get_file_path(
+            service_name, function_name, dir_path, "json")
+        json_data_list = json.dumps(json_data_list, indent=4, default=str)
+        # Writing to sample.json
+        with open(file_full_path, "w") as outfile:
+            outfile.write(json_data_list)
+        print("RESULT : File is generated at location {} ".format(file_full_path))
+    else:
+        print("RESULT : No records . ")
+    return file_full_path
+
+
+def save_file(json_data, service_name, function_name, dir_path=None):
+    file_full_path = get_file_path(
+        service_name, function_name, dir_path, "json")
+    # Writing to sample.json
+    with open(file_full_path, "w") as outfile:
+        outfile.write(json_data)
+    print("RESULT : File is generated at location {} ".format(file_full_path))
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/efs.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{0: {'function_name': 'describe_file_systems', 'function_description': 'Returns "*

 * *                "the description of a specific Amazon EFS file system ', 'is_regional': 'Y', "*

 * *                "'pagination_support': 'Y', 'result_keys': ['FileSystems'], 'json_response': "*

 * *                "{replace: OrderedDict([('OwnerId', 'string'), ('CreationToken', 'string'), "*

 * *                "('FileSystemId', 'string'), ('FileSystemArn', 'string'), ('CreationTime', ''), "*

 * *                "('LifeCycleSta […]*

```diff
@@ -1,58 +1,44 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Retrieves a list of analyzers.",
-            "function_name": "list_analyzers",
+            "function_description": "Returns the description of a specific Amazon EFS file system ",
+            "function_name": "describe_file_systems",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "arn": "string",
-                "createdAt": "",
-                "lastResourceAnalyzed": "string",
-                "lastResourceAnalyzedAt": "",
-                "name": "string",
-                "status": "",
-                "statusReason_code": "",
-                "tags_string": "string",
-                "type": ""
+                "AvailabilityZoneId": "string",
+                "AvailabilityZoneName": "string",
+                "CreationTime": "",
+                "CreationToken": "string",
+                "Encrypted": "",
+                "FileSystemArn": "string",
+                "FileSystemId": "string",
+                "KmsKeyId": "string",
+                "LifeCycleState": "",
+                "Name": "string",
+                "NumberOfMountTargets": "",
+                "OwnerId": "string",
+                "PerformanceMode": "",
+                "ProvisionedThroughputInMibps": "",
+                "SizeInBytes_Timestamp": "",
+                "SizeInBytes_Value": "",
+                "SizeInBytes_ValueInIA": "",
+                "SizeInBytes_ValueInStandard": "",
+                "Tags_0_Key": "string",
+                "Tags_0_Value": "string",
+                "ThroughputMode": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "analyzers"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "Returns information about the access key IDs associated with the specified IAM user",
-            "function_name": "list_findings",
-            "function_type": "list",
-            "is_regional": "No",
-            "json_response": {
-                "action_0": "string",
-                "analyzedAt": "",
-                "condition_string": "string",
-                "createdAt": "",
-                "error": "string",
-                "id": "string",
-                "isPublic": "string",
-                "principal_string": "string",
-                "resource": "string",
-                "resourceOwnerAccount": "string",
-                "resourceType": "",
-                "sources_0_detail_accessPointAccount": "string",
-                "sources_0_detail_accessPointArn": "string",
-                "sources_0_type": "",
-                "status": "",
-                "updatedAt": ""
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "findings"
-            ]
+                "FileSystems"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "accessanalyzer"
+    "service_name": "efs"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/apigateway.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/apigateway.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "List All Rest APIs",
             "function_name": "get_rest_apis",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "apiKeySource": "",
                 "binaryMediaTypes_0": "",
                 "createdDate": "",
                 "description": "",
                 "disableExecuteApiEndpoint": "",
                 "endpointConfiguration_types_0": "",
@@ -18,16 +21,17 @@
                 "minimumCompressionSize": "",
                 "name": "required",
                 "policy": "",
                 "tags_string": "",
                 "version": "",
                 "warnings_0": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "items"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "apigateway"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/budgets.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/budgets.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8928571428571428%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'N', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_global_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': '', 'pagination_attributes': "*

 * *                "[OrderedDict([('attribute_name', 'AccountId'), ('attribute_value', 'default'), "*

 * *                "('is_visible', 'N'), ('display_prompt', ''), ('type', 'str')])]}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Lists all the buedgets",
             "function_name": "describe_budgets",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "AutoAdjustData_AutoAdjustType": "",
                 "AutoAdjustData_HistoricalOptions_BudgetAdjustmentPeriod": "",
                 "AutoAdjustData_HistoricalOptions_LookBackAvailablePeriods": "",
                 "AutoAdjustData_LastAutoAdjustTime": "",
                 "BudgetLimit_Amount": "string",
                 "BudgetLimit_Unit": "string",
@@ -34,16 +37,26 @@
                 "LastUpdatedTime": "",
                 "PlannedBudgetLimits_string_Amount": "string",
                 "PlannedBudgetLimits_string_Unit": "string",
                 "TimePeriod_End": "",
                 "TimePeriod_Start": "",
                 "TimeUnit": ""
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "AccountId",
+                    "attribute_value": "default",
+                    "display_prompt": "",
+                    "is_visible": "N",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Budgets"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "budgets"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudfront.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudfront.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}, 1: {'is_regional': 'Y', 'pagination_support': 'N', "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_regional_no_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': ''}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "List CloudFront distributions",
             "function_name": "list_distributions",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "ARN": "string",
                 "AliasICPRecordals_0_CNAME": "string",
                 "AliasICPRecordals_0_ICPRecordalStatus": "",
                 "Aliases_Items_0": "string",
                 "Aliases_Quantity": "",
                 "CacheBehaviors_Items_0_AllowedMethods_CachedMethods_Items_0": "",
@@ -137,40 +140,45 @@
                 "ViewerCertificate_CertificateSource": "",
                 "ViewerCertificate_CloudFrontDefaultCertificate": "",
                 "ViewerCertificate_IAMCertificateId": "string",
                 "ViewerCertificate_MinimumProtocolVersion": "",
                 "ViewerCertificate_SSLSupportMethod": "",
                 "WebACLId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "DistributionList",
                 "Items"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Gets a list of all CloudFront functions in your Amazon Web Services account",
             "function_name": "list_functions",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_no_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "FunctionConfig_Comment": "string",
                 "FunctionConfig_Runtime": "",
                 "FunctionMetadata_CreatedTime": "",
                 "FunctionMetadata_FunctionARN": "string",
                 "FunctionMetadata_LastModifiedTime": "",
                 "FunctionMetadata_Stage": "",
                 "Name": "string",
                 "Status": "string"
             },
-            "pagination_support": "No",
+            "pagination_support": "N",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "FunctionList",
                 "Items"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "cloudfront"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudtrail.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudtrail.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}}"}*

```diff
@@ -1,22 +1,26 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Lists trails ",
             "function_name": "list_trails",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "HomeRegion": "string",
                 "Name": "string",
                 "TrailARN": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Trails"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "cloudtrail"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudwatch.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/kms.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_keys', 'function_description': 'Gets a list of all "*

 * *                "KMS keys.', 'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['Keys'], 'json_response': {replace: OrderedDict([('KeyId', 'string'), ('KeyArn', "*

 * *                "'string')])}, 'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': ''}, delete: [0]}",*

 * * "'service_name'": "'kms'"}*

```diff
@@ -1,41 +1,25 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "List of the dashboards for your account ",
-            "function_name": "list_dashboards",
+            "function_description": "Gets a list of all KMS keys.",
+            "function_name": "list_keys",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "DashboardArn": "string",
-                "DashboardName": "string",
-                "LastModified": "string",
-                "Size": "string"
+                "KeyArn": "string",
+                "KeyId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "DashboardEntries"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "List the specified metrics",
-            "function_name": "list_metrics",
-            "function_type": "list",
-            "is_regional": "Yes",
-            "json_response": {
-                "Dimensions_0_Name": "string",
-                "Dimensions_0_Value": "string",
-                "MetricName": "string",
-                "Namespace": "string"
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "Metrics"
-            ]
+                "Keys"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "cloudwatch"
+    "service_name": "kms"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/codecommit.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/dynamodb.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6057692307692308%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_tables', 'function_description': 'Returns a list of "*

 * *                "tables', 'response_format': 'FORMAT_3', 'is_regional': 'Y', 'pagination_support': "*

 * *                "'Y', 'result_keys': ['TableNames'], 'json_response': {replace: "*

 * *                "OrderedDict([('TableName', '')])}, 'is_multi_account_support': 'Y', 'implclass': "*

 * *                "'_regional_paginate', 'implfunction': 'process', 'validation_functions': ''}}",*

 * * "'service_name'": "'dynamodb'"}*

```diff
@@ -1,21 +1,24 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Gets information about one or more repositories.",
-            "function_name": "list_repositories",
+            "function_description": "Returns a list of tables",
+            "function_name": "list_tables",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "repositoryId": "string",
-                "repositoryName": "string"
+                "TableName": ""
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_3",
             "result_keys": [
-                "repositories"
-            ]
+                "TableNames"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "codecommit"
+    "service_name": "dynamodb"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/dynamodb.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sqs.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6153846153846154%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_queues', 'function_description': 'Returns a list of "*

 * *                "queues', 'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['QueueUrls'], 'json_response': {replace: OrderedDict([('QueueUrl', '')])}, "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': ''}}",*

 * * "'service_name'": "'sqs'"}*

```diff
@@ -1,20 +1,24 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Returns a list of tables",
-            "function_name": "list_tables",
+            "function_description": "Returns a list of queues",
+            "function_name": "list_queues",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "TableName": ""
+                "QueueUrl": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_3",
             "result_keys": [
-                "TableNames"
-            ]
+                "QueueUrls"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "dynamodb"
+    "service_name": "sqs"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/ec2.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/ec2.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9029761904761905%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'N', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_no_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}, 1: {'is_regional': 'Y', 'pagination_support': 'Y', "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': ''}, 2: {'is_regional': 'Y', "*

 * *                "'pagination_support':  […]*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Describes the specified Elastic IP addresses",
             "function_name": "describe_addresses",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_no_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AllocationId": "string",
                 "AssociationId": "string",
                 "CarrierIp": "string",
                 "CustomerOwnedIp": "string",
                 "CustomerOwnedIpv4Pool": "string",
                 "Domain": "",
@@ -19,26 +22,30 @@
                 "NetworkInterfaceOwnerId": "string",
                 "PrivateIpAddress": "string",
                 "PublicIp": "string",
                 "PublicIpv4Pool": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string"
             },
-            "pagination_support": "No",
+            "pagination_support": "N",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Addresses"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List VPCFlow logs",
             "function_name": "describe_flow_logs",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "CreationTime": "",
                 "DeliverCrossAccountRole": "string",
                 "DeliverLogsErrorMessage": "string",
                 "DeliverLogsPermissionArn": "string",
                 "DeliverLogsStatus": "string",
                 "DestinationOptions_FileFormat": "",
@@ -52,26 +59,30 @@
                 "LogGroupName": "string",
                 "MaxAggregationInterval": "",
                 "ResourceId": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "TrafficType": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "FlowLogs"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List All Ec2 instances",
             "function_name": "describe_instances",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Groups_0_GroupId": "string",
                 "Groups_0_GroupName": "string",
                 "Instances_0_AmiLaunchIndex": "",
                 "Instances_0_Architecture": "",
                 "Instances_0_BlockDeviceMappings_0_DeviceName": "string",
                 "Instances_0_BlockDeviceMappings_0_Ebs_AttachTime": "",
@@ -192,26 +203,30 @@
                 "Instances_0_Tags_0_Value": "string",
                 "Instances_0_TpmSupport": "string",
                 "Instances_0_UsageOperation": "string",
                 "Instances_0_UsageOperationUpdateTime": "",
                 "Instances_0_VirtualizationType": "",
                 "Instances_0_VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Reservations"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Descirbe Network ACL",
             "function_name": "describe_network_acls",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Associations_0_NetworkAclAssociationId": "string",
                 "Associations_0_NetworkAclId": "string",
                 "Associations_0_SubnetId": "string",
                 "Entries_0_CidrBlock": "string",
                 "Entries_0_Egress": "",
                 "Entries_0_IcmpTypeCode_Code": "",
@@ -225,26 +240,30 @@
                 "IsDefault": "",
                 "NetworkAclId": "string",
                 "OwnerId": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "NetworkAcls"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Descirbe Route Tables",
             "function_name": "describe_route_tables",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Associations_0_AssociationState_State": "",
                 "Associations_0_AssociationState_StatusMessage": "string",
                 "Associations_0_GatewayId": "string",
                 "Associations_0_Main": "",
                 "Associations_0_RouteTableAssociationId": "string",
                 "Associations_0_RouteTableId": "string",
@@ -268,26 +287,30 @@
                 "Routes_0_State": "",
                 "Routes_0_TransitGatewayId": "string",
                 "Routes_0_VpcPeeringConnectionId": "",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "RouteTables"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List All Security Groups",
             "function_name": "describe_security_groups",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Description": "string",
                 "GroupId": "string",
                 "GroupName": "string",
                 "IpPermissionsEgress_0_FromPort": "",
                 "IpPermissionsEgress_0_IpProtocol": "string",
                 "IpPermissionsEgress_0_IpRanges_0_CidrIp": "string",
@@ -321,26 +344,30 @@
                 "IpPermissions_0_UserIdGroupPairs_0_VpcId": "string",
                 "IpPermissions_0_UserIdGroupPairs_0_VpcPeeringConnectionId": "string",
                 "OwnerId": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "SecurityGroups"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List All Security Groups Rules",
             "function_name": "describe_security_group_rules",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "CidrIpv4": "string",
                 "CidrIpv6": "string",
                 "Description": "string",
                 "FromPort": "",
                 "GroupId": "string",
                 "GroupOwnerId": "string",
@@ -353,26 +380,30 @@
                 "ReferencedGroupInfo_VpcId": "string",
                 "ReferencedGroupInfo_VpcPeeringConnectionId": "string",
                 "SecurityGroupRuleId": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "ToPort": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "SecurityGroupRules"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Describe Snapshot",
             "function_name": "describe_snapshots",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "DataEncryptionKeyId": "string",
                 "Description": "string",
                 "Encrypted": "",
                 "KmsKeyId": "string",
                 "OutpostArn": "string",
                 "OwnerAlias": "string",
@@ -385,26 +416,41 @@
                 "StateMessage": "string",
                 "StorageTier": "",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VolumeId": "string",
                 "VolumeSize": ""
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "OwnerIds",
+                    "attribute_value": [
+                        "self"
+                    ],
+                    "display_prompt": "",
+                    "is_visible": "N",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Snapshots"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Descirbe Route Tables",
             "function_name": "describe_subnets",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AssignIpv6AddressOnCreation": "",
                 "AvailabilityZone": "string",
                 "AvailabilityZoneId": "string",
                 "AvailableIpAddressCount": "",
                 "CidrBlock": "string",
                 "CustomerOwnedIpv4Pool": "string",
@@ -426,26 +472,30 @@
                 "State": "",
                 "SubnetArn": "string",
                 "SubnetId": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Subnets"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List All transit_gateways",
             "function_name": "describe_transit_gateways",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "CreationTime": "",
                 "Description": "string",
                 "Options_AmazonSideAsn": "",
                 "Options_AssociationDefaultRouteTableId": "string",
                 "Options_AutoAcceptSharedAttachments": "",
                 "Options_DefaultRouteTableAssociation": "",
@@ -458,26 +508,30 @@
                 "OwnerId": "",
                 "State": "",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "TransitGatewayArn": "string",
                 "TransitGatewayId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "TransitGateways"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Descirbe Volumes",
             "function_name": "describe_volumes",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Attachments_0_AttachTime": "",
                 "Attachments_0_DeleteOnTermination": "",
                 "Attachments_0_Device": "string",
                 "Attachments_0_InstanceId": "string",
                 "Attachments_0_State": "",
                 "Attachments_0_VolumeId": "string",
@@ -494,26 +548,30 @@
                 "State": "",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "Throughput": "",
                 "VolumeId": "string",
                 "VolumeType": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Volumes"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Descirbe VPCs",
             "function_name": "describe_vpcs",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "CidrBlock": "string",
                 "CidrBlockAssociationSet_0_AssociationId": "string",
                 "CidrBlockAssociationSet_0_CidrBlock": "string",
                 "CidrBlockAssociationSet_0_CidrBlockState_State": "",
                 "CidrBlockAssociationSet_0_CidrBlockState_StatusMessage": "string",
                 "DhcpOptionsId": "string",
@@ -527,27 +585,31 @@
                 "IsDefault": "",
                 "OwnerId": "string",
                 "State": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Vpcs"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "csv_enforced_required_only": "Yes",
+            "csv_enforced_required_only": "Y",
             "function_description": "List VPC endpoints",
             "function_name": "describe_vpc_endpoints",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "CreationTimestamp": "",
                 "DnsEntries_0_DnsName": "string",
                 "DnsEntries_0_HostedZoneId": "string",
                 "DnsOptions_DnsRecordIpType": "",
                 "Groups_0_GroupId": "string",
                 "Groups_0_GroupName": "string",
@@ -564,26 +626,30 @@
                 "SubnetIds_0": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcEndpointId": "string",
                 "VpcEndpointType": "",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "VpcEndpoints"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List vpc peering connections Snapshot",
             "function_name": "describe_vpc_peering_connections",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AccepterVpcInfo_CidrBlock": "string",
                 "AccepterVpcInfo_CidrBlockSet_0_CidrBlock": "string",
                 "AccepterVpcInfo_Ipv6CidrBlockSet_0_Ipv6CidrBlock": "string",
                 "AccepterVpcInfo_OwnerId": "string",
                 "AccepterVpcInfo_PeeringOptions_AllowDnsResolutionFromRemoteVpc": "",
                 "AccepterVpcInfo_PeeringOptions_AllowEgressFromLocalClassicLinkToRemoteVpc": "",
@@ -602,26 +668,30 @@
                 "RequesterVpcInfo_VpcId": "string",
                 "Status_Code": "",
                 "Status_Message": "string",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "VpcPeeringConnectionId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "VpcPeeringConnections"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List VPCFlow logs",
             "function_name": "describe_vpn_connections",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_no_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "Category": "string",
                 "CoreNetworkArn": "string",
                 "CoreNetworkAttachmentArn": "string",
                 "CustomerGatewayConfiguration": "string",
                 "CustomerGatewayId": "string",
                 "GatewayAssociationState": "",
@@ -669,16 +739,17 @@
                 "VgwTelemetry_0_LastStatusChange": "",
                 "VgwTelemetry_0_OutsideIpAddress": "string",
                 "VgwTelemetry_0_Status": "",
                 "VgwTelemetry_0_StatusMessage": "",
                 "VpnConnectionId": "string",
                 "VpnGatewayId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "N",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "VpnConnections"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "ec2"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/ecs.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sns.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5705128205128205%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_subscriptions', 'function_description': 'List "*

 * *                "subscriptions', 'response_format': 'FORMAT_2', 'is_regional': 'Y', "*

 * *                "'pagination_support': 'Y', 'result_keys': ['Subscriptions'], 'json_response': "*

 * *                "{replace: OrderedDict([('SubscriptionArn', 'string'), ('Owner', 'string'), "*

 * *                "('Protocol', 'string'), ('Endpoint', 'string'), ('TopicArn', 'string')])}, "*

 * *                "'is_multi_account_support': 'Y' […]*

```diff
@@ -1,50 +1,47 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "List ECS Clusters",
-            "function_name": "list_clusters",
+            "function_description": "List subscriptions",
+            "function_name": "list_subscriptions",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "clusterArns": ""
+                "Endpoint": "string",
+                "Owner": "string",
+                "Protocol": "string",
+                "SubscriptionArn": "string",
+                "TopicArn": "string"
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "clusterArns"
-            ]
+                "Subscriptions"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "List ECS services",
-            "function_name": "list_services",
+            "function_description": "Returns a list of topics",
+            "function_name": "list_topics",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "ServiceArn": ""
+                "TopicArn": "string"
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "serviceArns"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "List Tasks",
-            "function_name": "list_tasks",
-            "function_type": "list",
-            "is_regional": "Yes",
-            "json_response": {
-                "taskArn": ""
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
-            "result_keys": [
-                "taskArns"
-            ]
+                "Topics"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "ecs"
+    "service_name": "sns"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/efs.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cloudwatch.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{1: {'function_name': 'list_metrics', 'function_description': 'List the specified "*

 * *                "metrics', 'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['Metrics'], 'json_response': {replace: OrderedDict([('Namespace', 'string'), "*

 * *                "('MetricName', 'string'), ('Dimensions_0_Name', 'string'), ('Dimensions_0_Value', "*

 * *                "'string')])}, 'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'imp […]*

```diff
@@ -1,40 +1,49 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Returns the description of a specific Amazon EFS file system ",
-            "function_name": "describe_file_systems",
+            "function_description": "List of the dashboards for your account ",
+            "function_name": "list_dashboards",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "AvailabilityZoneId": "string",
-                "AvailabilityZoneName": "string",
-                "CreationTime": "",
-                "CreationToken": "string",
-                "Encrypted": "",
-                "FileSystemArn": "string",
-                "FileSystemId": "string",
-                "KmsKeyId": "string",
-                "LifeCycleState": "",
-                "Name": "string",
-                "NumberOfMountTargets": "",
-                "OwnerId": "string",
-                "PerformanceMode": "",
-                "ProvisionedThroughputInMibps": "",
-                "SizeInBytes_Timestamp": "",
-                "SizeInBytes_Value": "",
-                "SizeInBytes_ValueInIA": "",
-                "SizeInBytes_ValueInStandard": "",
-                "Tags_0_Key": "string",
-                "Tags_0_Value": "string",
-                "ThroughputMode": ""
+                "DashboardArn": "string",
+                "DashboardName": "string",
+                "LastModified": "string",
+                "Size": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "FileSystems"
-            ]
+                "DashboardEntries"
+            ],
+            "validation_functions": ""
+        },
+        {
+            "boto_session_type": "client",
+            "function_description": "List the specified metrics",
+            "function_name": "list_metrics",
+            "function_type": "list",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
+            "json_response": {
+                "Dimensions_0_Name": "string",
+                "Dimensions_0_Value": "string",
+                "MetricName": "string",
+                "Namespace": "string"
+            },
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
+            "result_keys": [
+                "Metrics"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "efs"
+    "service_name": "cloudwatch"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/eks.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/sagemaker.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5615384615384615%*

 * *Differences: {"'functions'": "{2: {'function_name': 'list_models', 'function_description': 'Lists the Images. "*

 * *                "', 'response_format': 'FORMAT_2', 'function_type': 'list', 'is_regional': 'Y', "*

 * *                "'pagination_support': 'Y', 'result_keys': ['Models'], 'json_response': {replace: "*

 * *                "OrderedDict([('ModelName', 'string'), ('ModelArn', 'string'), ('CreationTime', "*

 * *                "'')])}, 'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'impl […]*

```diff
@@ -1,87 +1,124 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "List EKS Clusters",
-            "function_name": "describe_cluster",
-            "function_type": "object",
-            "is_regional": "Yes",
+            "function_description": "Lists the domains. ",
+            "function_name": "list_domains",
+            "function_type": "list",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
+            "json_response": {
+                "CreationTime": "",
+                "DomainArn": "string",
+                "DomainId": "string",
+                "DomainName": "string",
+                "LastModifiedTime": "",
+                "Status": "",
+                "Url": "string"
+            },
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
+            "result_keys": [
+                "Domains"
+            ],
+            "validation_functions": ""
+        },
+        {
+            "boto_session_type": "client",
+            "function_description": "Lists the Images. ",
+            "function_name": "list_images",
+            "function_type": "list",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
+            "json_response": {
+                "CreationTime": "",
+                "Description": "string",
+                "DisplayName": "string",
+                "FailureReason": "string",
+                "ImageArn": "string",
+                "ImageName": "string",
+                "ImageStatus": "",
+                "LastModifiedTime": ""
+            },
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
+            "result_keys": [
+                "Images"
+            ],
+            "validation_functions": ""
+        },
+        {
+            "boto_session_type": "client",
+            "function_description": "Lists the Images. ",
+            "function_name": "list_models",
+            "function_type": "list",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "arn": "string",
-                "certificateAuthority_data": "string",
-                "clientRequestToken": "string",
-                "connectorConfig_activationCode": "string",
-                "connectorConfig_activationExpiry": "",
-                "connectorConfig_activationId": "string",
-                "connectorConfig_provider": "string",
-                "connectorConfig_roleArn": "string",
-                "createdAt": "",
-                "encryptionConfig_0_provider_keyArn": "string",
-                "encryptionConfig_0_resources_0": "string",
-                "endpoint": "string",
-                "health_issues_0_code": "",
-                "health_issues_0_message": "string",
-                "health_issues_0_resourceIds_0": "string",
-                "id": "string",
-                "identity_oidc_issuer": "string",
-                "kubernetesNetworkConfig_ipFamily": "",
-                "kubernetesNetworkConfig_serviceIpv4Cidr": "string",
-                "kubernetesNetworkConfig_serviceIpv6Cidr": "string",
-                "logging_clusterLogging_0_enabled": "",
-                "logging_clusterLogging_0_types_0": "",
-                "name": "string",
-                "outpostConfig_controlPlaneInstanceType": "string",
-                "outpostConfig_controlPlanePlacement_groupName": "string",
-                "outpostConfig_outpostArns_0": "string",
-                "platformVersion": "string",
-                "resourcesVpcConfig_clusterSecurityGroupId": "string",
-                "resourcesVpcConfig_endpointPrivateAccess": "",
-                "resourcesVpcConfig_endpointPublicAccess": "",
-                "resourcesVpcConfig_publicAccessCidrs_0": "string",
-                "resourcesVpcConfig_securityGroupIds_0": "string",
-                "resourcesVpcConfig_subnetIds_0": "string",
-                "resourcesVpcConfig_vpcId": "string",
-                "roleArn": "string",
-                "status": "",
-                "tags_string": "string",
-                "version": "string"
+                "CreationTime": "",
+                "ModelArn": "string",
+                "ModelName": "string"
             },
-            "pagination_support": "No",
-            "response_format": "FORMAT_1",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "cluster"
-            ]
+                "Models"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "List EKS Clusters",
-            "function_name": "list_clusters",
+            "function_description": "Lists the Projects. ",
+            "function_name": "list_projects",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_no_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "cluster": ""
+                "CreationTime": "",
+                "ProjectArn": "string",
+                "ProjectDescription": "string",
+                "ProjectId": "string",
+                "ProjectName": "string",
+                "ProjectStatus": ""
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "N",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "clusters"
-            ]
+                "ProjectSummaryList"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "List Farget profiles",
-            "function_name": "list_fargate_profiles",
+            "function_description": "Lists user profiles. ",
+            "function_name": "list_user_profiles",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "fargateProfileName": ""
+                "CreationTime": "",
+                "DomainId": "string",
+                "LastModifiedTime": "",
+                "Status": "",
+                "UserProfileName": "string"
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "fargateProfileNames"
-            ]
+                "UserProfiles"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "eks"
+    "service_name": "sagemaker"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/elasticache.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/elasticache.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Provisioned cluster",
             "function_name": "describe_cache_clusters",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "ARN": "string",
                 "AtRestEncryptionEnabled": "",
                 "AuthTokenEnabled": "",
                 "AuthTokenLastModifiedDate": "",
                 "AutoMinorVersionUpgrade": "",
                 "CacheClusterCreateTime": "",
@@ -68,16 +71,17 @@
                 "SecurityGroups_0_SecurityGroupId": "string",
                 "SecurityGroups_0_Status": "string",
                 "SnapshotRetentionLimit": "",
                 "SnapshotWindow": "string",
                 "TransitEncryptionEnabled": "",
                 "TransitEncryptionMode": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "CacheClusters"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "elasticache"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/elbv2.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/elbv2.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "All of your load balancers.",
             "function_name": "describe_load_balancers",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AvailabilityZones_0_LoadBalancerAddresses_0_AllocationId": "string",
                 "AvailabilityZones_0_LoadBalancerAddresses_0_IPv6Address": "string",
                 "AvailabilityZones_0_LoadBalancerAddresses_0_IpAddress": "string",
                 "AvailabilityZones_0_LoadBalancerAddresses_0_PrivateIPv4Address": "string",
                 "AvailabilityZones_0_OutpostId": "string",
                 "AvailabilityZones_0_SubnetId": "string",
@@ -24,16 +27,17 @@
                 "Scheme": "",
                 "SecurityGroups_0": "string",
                 "State_Code": "",
                 "State_Reason": "string",
                 "Type": "",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "LoadBalancers"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "elbv2"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/emr-serverless.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/emr-serverless.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8983516483516484%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}, 1: {'is_regional': 'Y', 'pagination_support': 'Y', "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': '', 'pagination_attributes': "*

 * *                "[OrderedDict([('attribute […]*

```diff
@@ -1,55 +1,72 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Lists applications",
             "function_name": "list_applications",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "architecture": "",
                 "arn": "string",
                 "createdAt": "",
                 "id": "string",
                 "name": "string",
                 "releaseLabel": "string",
                 "state": "",
                 "stateDetails": "string",
                 "type": "string",
                 "updatedAt": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "applications"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists job runs",
             "function_name": "list_job_runs",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "applicationId": "string",
                 "arn": "string",
                 "createdAt": "string",
                 "createdBy": "string",
                 "executionRole": "string",
                 "id": "string",
                 "name": "string",
                 "releaseLabel": "string",
                 "state": "",
                 "stateDetails": "string",
                 "type": "string",
                 "updatedAt": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "applicationId",
+                    "attribute_value": "",
+                    "display_prompt": "The ID of the application for which to list the job run",
+                    "is_visible": "Y",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "jobRuns"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "emr-serverless"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/iam.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/iam.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8975274725274724%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'N', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_global_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}, 1: {'is_regional': 'N', 'pagination_support': 'Y', "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_global_paginate', 'implfunction': "*

 * *                "'process', 'validation_functions': ''}, 2: {'is_regional': 'N', "*

 * *                "'pagination_support': 'Y', 'i […]*

```diff
@@ -1,150 +1,225 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Lists the IAM users ",
             "function_name": "list_users",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "Arn": "string",
                 "CreateDate": "string",
                 "PasswordLastUsed": "string",
                 "Path": "string",
                 "PermissionsBoundary_PermissionsBoundaryArn": "string",
                 "PermissionsBoundary_PermissionsBoundaryType": "PermissionsBoundaryPolicy",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "UserId": "string",
                 "UserName": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Users"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Returns information about the access key IDs associated with the specified IAM user",
             "function_name": "list_access_keys",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "AccessKeyId": "required",
                 "CreateDate": "required",
                 "Status": "required",
                 "UserName": "required"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "AccessKeyMetadata"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists the account alias associated with the Amazon Web Services account ",
             "function_name": "list_account_aliases",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "AccountAliase": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_3",
             "result_keys": [
                 "AccountAliases"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists all managed policies that are attached to the specified IAM group",
             "function_name": "list_attached_group_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "PolicyArn": "required",
                 "PolicyName": "required"
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "GroupName",
+                    "attribute_value": "",
+                    "display_prompt": "Group Name",
+                    "is_visible": "Y",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "AttachedPolicies"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists all managed policies that are attached to the specified IAM role",
             "function_name": "list_attached_role_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "PolicyArn": "required",
                 "PolicyName": "required"
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "RoleName",
+                    "attribute_value": "",
+                    "display_prompt": "Role Name",
+                    "is_visible": "Y",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "AttachedPolicies"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists all managed policies that are attached to the specified IAM role",
             "function_name": "list_attached_user_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "PolicyArn": "required",
                 "PolicyName": "required"
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "UserName",
+                    "attribute_value": "",
+                    "display_prompt": "User Name",
+                    "is_visible": "Y",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "AttachedPolicies"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists all managed policies that are attached to the specified IAM role",
             "function_name": "list_group_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "PolicyName": ""
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "GroupName",
+                    "attribute_value": "",
+                    "display_prompt": "Group Name",
+                    "is_visible": "Y",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_3",
             "result_keys": [
                 "PolicyNames"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Lists all managed policies that are attached to the specified IAM role",
             "function_name": "list_groups",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
-                "Groups": " "
+                "Arn": "",
+                "CreateDate": "",
+                "GroupId": "",
+                "GroupName": "",
+                "Path": ""
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
                 "Groups"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "List All the IAM Polices",
             "function_name": "list_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "Arn": "required",
                 "AttachmentCount": "string",
                 "CreateDate": "required",
                 "DefaultVersionId": "string",
                 "Description": "string",
                 "IsAttachable": "string",
@@ -152,26 +227,30 @@
                 "PermissionsBoundaryUsageCount": "string",
                 "PolicyId": "required",
                 "PolicyName": "required",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "UpdateDate": "required"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Policies"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Roles",
             "function_name": "list_roles",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
                 "Arn": "required",
                 "AssumeRolePolicyDocument": "string",
                 "CreateDate": "string",
                 "Description": "string",
                 "MaxSessionDuration": "string",
                 "Path": "string",
@@ -180,16 +259,17 @@
                 "RoleId": "required",
                 "RoleLastUsed_LastUsedDate": "string",
                 "RoleLastUsed_Region": "string",
                 "RoleName": "required",
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Roles"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "iam"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/kms.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/account.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6153846153846154%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_regions', 'function_description': 'list_regions', "*

 * *                "'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': ['Regions'], "*

 * *                "'json_response': {replace: OrderedDict([('RegionName', ''), ('RegionOptStatus', "*

 * *                "'')])}, 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': '', 'is_multi_account_support': 'Y'}}",*

 * * "'service_name'": "'account'"}*

```diff
@@ -1,21 +1,25 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Gets a list of all KMS keys.",
-            "function_name": "list_keys",
+            "function_description": "list_regions",
+            "function_name": "list_regions",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "KeyArn": "string",
-                "KeyId": "string"
+                "RegionName": "",
+                "RegionOptStatus": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Keys"
-            ]
+                "Regions"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "kms"
+    "service_name": "account"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/lambda.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6153846153846154%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_namespaces', 'function_description': 'List Name "*

 * *                "spaces', 'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['namespaces'], 'json_response': {replace: OrderedDict([('adminUsername', "*

 * *                "'string'), ('creationDate', 'string'), ('dbName', 'string'), "*

 * *                "('defaultIamRoleArn', 'string'), ('iamRoles_0', 'string'), ('kmsKeyId', "*

 * *                "'string'), ('logExports_0', ''), ('namespaceAr […]*

```diff
@@ -1,85 +1,74 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "List Lambda Functions",
-            "function_name": "list_functions",
+            "function_description": "List Name spaces",
+            "function_name": "list_namespaces",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "Architectures_0": "",
-                "CodeSha256": "",
-                "CodeSize": "",
-                "DeadLetterConfig_TargetArn": "0",
-                "Description": "",
-                "Environment_Error_ErrorCode": "",
-                "Environment_Error_Message": "",
-                "Environment_Variables_string": "0",
-                "EphemeralStorage_Size": "",
-                "FileSystemConfigs_0_Arn": "string",
-                "FileSystemConfigs_0_LocalMountPath": "string",
-                "FunctionArn": "required",
-                "FunctionName": "required",
-                "Handler": "string",
-                "ImageConfigResponse_Error_ErrorCode": "string",
-                "ImageConfigResponse_Error_Message": "string",
-                "ImageConfigResponse_ImageConfig_Command_0": "string",
-                "ImageConfigResponse_ImageConfig_EntryPoint_0": "string",
-                "ImageConfigResponse_ImageConfig_WorkingDirectory": "string",
-                "KMSKeyArn": "string",
-                "LastModified": "",
-                "LastUpdateStatus": "",
-                "LastUpdateStatusReason": "",
-                "LastUpdateStatusReasonCode": "",
-                "Layers_0_Arn": "",
-                "Layers_0_CodeSize": "",
-                "Layers_0_SigningJobArn": "",
-                "Layers_0_SigningProfileVersionArn": "",
-                "MasterArn": "",
-                "MemorySize": "",
-                "PackageType": "",
-                "RevisionId": "",
-                "Role": "string",
-                "Runtime": "string",
-                "SigningJobArn": "string",
-                "SigningProfileVersionArn": "string",
-                "State": "string",
-                "StateReason": "string",
-                "StateReasonCode": "",
-                "Timeout": "",
-                "TracingConfig_Mode": "",
-                "Version": "",
-                "VpcConfig_SecurityGroupIds_0": "0",
-                "VpcConfig_SubnetIds_0": "0",
-                "VpcConfig_VpcId": "string"
+                "adminUsername": "string",
+                "creationDate": "string",
+                "dbName": "string",
+                "defaultIamRoleArn": "string",
+                "iamRoles_0": "string",
+                "kmsKeyId": "string",
+                "logExports_0": "",
+                "namespaceArn": "string",
+                "namespaceId": "string",
+                "namespaceName": "string",
+                "status": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Functions"
-            ]
+                "namespaces"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "List Layers",
-            "function_name": "list_layers",
+            "function_description": "List work groups",
+            "function_name": "list_workgroups",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "LatestMatchingVersion_CompatibleRuntimes_0": "",
-                "LatestMatchingVersion_CreatedDate": "",
-                "LatestMatchingVersion_Description": "",
-                "LatestMatchingVersion_LayerVersionArn": "",
-                "LatestMatchingVersion_Version": "",
-                "LayerArn": "required",
-                "LayerName": "required"
+                "baseCapacity": "",
+                "configParameters_0_parameterKey": "string",
+                "configParameters_0_parameterValue": "string",
+                "creationDate": "string",
+                "endpoint_address": "string",
+                "endpoint_port": "",
+                "endpoint_vpcEndpoints_0_networkInterfaces_0_availabilityZone": "string",
+                "endpoint_vpcEndpoints_0_networkInterfaces_0_networkInterfaceId": "string",
+                "endpoint_vpcEndpoints_0_networkInterfaces_0_privateIpAddress": "string",
+                "endpoint_vpcEndpoints_0_networkInterfaces_0_subnetId": "string",
+                "endpoint_vpcEndpoints_0_vpcEndpointId": "string",
+                "endpoint_vpcEndpoints_0_vpcId": "string",
+                "enhancedVpcRouting": "string",
+                "namespaceName": "string",
+                "port": "",
+                "publiclyAccessible": "string",
+                "securityGroupIds_0": "string",
+                "status": "",
+                "subnetIds_0": "string",
+                "workgroupArn": "string",
+                "workgroupId": "string",
+                "workgroupName": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Layers"
-            ]
+                "workgroups"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "lambda"
+    "service_name": "redshift-serverless"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/organizations.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/cleanrooms.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_collaborations', 'function_description': 'Lists "*

 * *                "collaborations the caller owns is active in or has been invited to.', "*

 * *                "'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['collaborationList'], 'json_response': {replace: OrderedDict([('id', 'string'), "*

 * *                "('arn', 'string'), ('name', 'string'), ('creatorAccountId', 'string'), "*

 * *                "('creatorDisplayName', 'string'), ('crea […]*

```diff
@@ -1,46 +1,33 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "List accounts in Organization",
-            "function_name": "list_accounts",
+            "function_description": "Lists collaborations the caller owns is active in or has been invited to.",
+            "function_name": "list_collaborations",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "Arn": "string",
-                "Email": "string",
-                "Id": "string",
-                "JoinedMethod": "",
-                "JoinedTimestamp": "",
-                "Name": "string",
-                "Status": ""
+                "arn": "string",
+                "createTime": "",
+                "creatorAccountId": "string",
+                "creatorDisplayName": "string",
+                "id": "string",
+                "memberStatus": "",
+                "membershipArn": "string",
+                "membershipId": "string",
+                "name": "string",
+                "updateTime": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Accounts"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "List Policies in  Organization",
-            "function_name": "list_policies",
-            "function_type": "list",
-            "is_regional": "No",
-            "json_response": {
-                "Arn": "string",
-                "AwsManaged": "",
-                "Description": "string",
-                "Id": "string",
-                "Name": "string",
-                "Type": ""
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "Policies"
-            ]
+                "collaborationList"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "organizations"
+    "service_name": "cleanrooms"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/rds.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/rds.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}, 1: {'is_regional': 'Y', 'pagination_support': 'Y', "*

 * *                "'is_multi_account_support': 'Y', 'implclass': '_regional_paginate', "*

 * *                "'implfunction': 'process', 'validation_functions': ''}, 2: {'is_regional': 'Y', "*

 * *                "'pagination_support': 'Y' […]*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Amazon Aurora DB clusters",
             "function_name": "describe_db_clusters",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "ActivityStreamKinesisStreamName": "string",
                 "ActivityStreamKmsKeyId": "string",
                 "ActivityStreamMode": "",
                 "ActivityStreamStatus": "",
                 "AllocatedStorage": "",
                 "AssociatedRoles_0_FeatureName": "string",
@@ -102,26 +105,30 @@
                 "StorageEncrypted": "",
                 "StorageType": "string",
                 "TagList_0_Key": "string",
                 "TagList_0_Value": "string",
                 "VpcSecurityGroups_0_Status": "string",
                 "VpcSecurityGroups_0_VpcSecurityGroupId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "DBClusters"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Provisioned RDS instances",
             "function_name": "describe_db_instances",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "ActivityStreamEngineNativeAuditFieldsIncluded": " ",
                 "ActivityStreamKinesisStreamName": "string",
                 "ActivityStreamKmsKeyId": "string",
                 "ActivityStreamMode": "",
                 "ActivityStreamPolicyStatus": "",
                 "ActivityStreamStatus": "",
@@ -246,51 +253,59 @@
                 "TagList_0_Key": "string",
                 "TagList_0_Value": "string",
                 "TdeCredentialArn": "string",
                 "Timezone": "string",
                 "VpcSecurityGroups_0_Status": "string",
                 "VpcSecurityGroups_0_VpcSecurityGroupId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "DBInstances"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Returns a list of DBSecurityGroup descriptions",
             "function_name": "describe_db_security_groups",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "DBSecurityGroupArn": "string",
                 "DBSecurityGroupDescription": "string",
                 "DBSecurityGroupName": "string",
                 "EC2SecurityGroups_0_EC2SecurityGroupId": "string",
                 "EC2SecurityGroups_0_EC2SecurityGroupName": "string",
                 "EC2SecurityGroups_0_EC2SecurityGroupOwnerId": "string",
                 "EC2SecurityGroups_0_Status": "string",
                 "IPRanges_0_CIDRIP": "string",
                 "IPRanges_0_Status": "string",
                 "OwnerId": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "DBSecurityGroups"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Returns information about DB snapshots.",
             "function_name": "describe_db_snapshots",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AllocatedStorage": "",
                 "AvailabilityZone": "string",
                 "DBInstanceIdentifier": "string",
                 "DBSnapshotArn": "string",
                 "DBSnapshotIdentifier": "string",
                 "DbiResourceId": "string",
@@ -320,26 +335,30 @@
                 "StorageType": "string",
                 "TagList_0_Key": "string",
                 "TagList_0_Value": "string",
                 "TdeCredentialArn": "string",
                 "Timezone": "string",
                 "VpcId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "DBSnapshots"
-            ]
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
             "function_description": "Aurora global database clusters",
             "function_name": "describe_global_clusters",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "DatabaseName": "string",
                 "DeletionProtection": "",
                 "Engine": "string",
                 "EngineVersion": "string",
                 "FailoverState_FromDbClusterArn": "string",
                 "FailoverState_Status": "",
@@ -350,16 +369,17 @@
                 "GlobalClusterMembers_0_GlobalWriteForwardingStatus": "",
                 "GlobalClusterMembers_0_IsWriter": "",
                 "GlobalClusterMembers_0_Readers_0": "string",
                 "GlobalClusterResourceId": "string",
                 "Status": "string",
                 "StorageEncrypted": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "GlobalClusters"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "rds"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/redshift.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9038461538461539%*

 * *Differences: {"'functions'": "{0: {'is_regional': 'Y', 'pagination_support': 'Y', 'is_multi_account_support': "*

 * *                "'Y', 'implclass': '_regional_paginate', 'implfunction': 'process', "*

 * *                "'validation_functions': ''}}"}*

```diff
@@ -1,15 +1,18 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
             "function_description": "Amazon Redshift returns all clusters ",
             "function_name": "describe_clusters",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
                 "AllowVersionUpgrade": "string",
                 "AquaConfiguration_AquaConfigurationStatus": "",
                 "AquaConfiguration_AquaStatus": "",
                 "AutomatedSnapshotRetentionPeriod": "string",
                 "AvailabilityZone": "string",
                 "AvailabilityZoneRelocationStatus": "string",
@@ -111,16 +114,17 @@
                 "Tags_0_Key": "string",
                 "Tags_0_Value": "string",
                 "TotalStorageCapacityInMegaBytes": "String ",
                 "VpcId": "string",
                 "VpcSecurityGroups_0_Status": "string",
                 "VpcSecurityGroups_0_VpcSecurityGroupId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
                 "Clusters"
-            ]
+            ],
+            "validation_functions": ""
         }
     ],
     "service_name": "redshift"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/route53.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/amp.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_scrapers', 'function_description': 'PrometheusService "*

 * *                ":The ListScrapers operation lists all of the scrapers in your account', "*

 * *                "'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': ['scrapers'], "*

 * *                "'json_response': {replace: OrderedDict([('alias', 'string'), ('arn', 'string'), "*

 * *                "('createdAt', ''), ('destination_ampConfiguration_workspaceArn', 'string'), "*

 * *                "('lastModified […]*

```diff
@@ -1,79 +1,61 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Returns a paginated list of CIDR collections in the Amazon Web Services account (metadata only)",
-            "function_name": "list_cidr_blocks",
+            "function_description": "PrometheusService :The ListScrapers operation lists all of the scrapers in your account",
+            "function_name": "list_scrapers",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "Arn": "string",
-                "Id": "string",
-                "Name": "string",
-                "Version": ""
+                "alias": "string",
+                "arn": "string",
+                "createdAt": "",
+                "destination_ampConfiguration_workspaceArn": "string",
+                "lastModifiedAt": "",
+                "roleArn": "",
+                "scraperId": "",
+                "source_eksConfiguration_clusterArn": "",
+                "source_eksConfiguration_securityGroupIds_0": "",
+                "source_eksConfiguration_subnetIds_0": "",
+                "statusReason": "",
+                "status_statusCode": "",
+                "tags_string": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "CidrCollections"
-            ]
+                "scrapers"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "Retrieves a list of the public and private hosted zones that are associated with the current Amazon Web Services account",
-            "function_name": "list_hosted_zones",
+            "function_description": "Lists all of the Amazon Managed Service for Prometheus workspaces in your account",
+            "function_name": "list_workspaces",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "CallerReference": "string",
-                "Config_Comment": "string",
-                "Config_PrivateZone": "",
-                "Id": "string",
-                "LinkedService_Description": "string",
-                "LinkedService_ServicePrincipal": "string",
-                "Name": "string",
-                "ResourceRecordSetCount": ""
+                "alias": "string",
+                "arn": "string",
+                "createdAt": "",
+                "kmsKeyArn": "string",
+                "status_statusCode": "",
+                "tags_string": "string",
+                "workspaceId": "string"
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "HostedZones"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "Retrieves a list of the public and private hosted zones that are associated with the current Amazon Web Services account",
-            "function_name": "list_hosted_zones_by_vpc",
-            "function_type": "list",
-            "is_regional": "No",
-            "json_response": {
-                "HostedZoneId": "string",
-                "Name": "string",
-                "Owner_OwningAccount": "string",
-                "Owner_OwningService": "string"
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "HostedZoneSummaries"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "Gets a list of the VPCs that were created by other accounts and that can be associated with a specified hosted zone because youve submitted one or more CreateVPCAssociationAuthorization requests.",
-            "function_name": "list_vpc_association_authorizations",
-            "function_type": "list",
-            "is_regional": "No",
-            "json_response": {
-                "VPCId": "string",
-                "VPCRegion": ""
-            },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "VPCs"
-            ]
+                "workspaces"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "route53"
+    "service_name": "amp"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/route53domains.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/organizations.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6115427541208791%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_accounts', 'function_description': 'List accounts in "*

 * *                "Organization', 'is_regional': 'N', 'pagination_support': 'Y', 'result_keys': "*

 * *                "['Accounts'], 'json_response': {replace: OrderedDict([('Id', 'string'), ('Arn', "*

 * *                "'string'), ('Email', 'string'), ('Name', 'string'), ('Status', ''), "*

 * *                "('JoinedMethod', ''), ('JoinedTimestamp', '')])}, 'is_multi_account_support': "*

 * *                "'N', 'implclass' […]*

```diff
@@ -1,48 +1,63 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Domain names registered with Amazon Route 53 ",
-            "function_name": "list_domains",
+            "function_description": "List accounts in Organization",
+            "function_name": "list_accounts",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "N",
+            "is_regional": "N",
             "json_response": {
-                "AutoRenew": "string",
-                "DomainName": "string",
-                "Expiry": "string",
-                "TransferLock": "string"
+                "Arn": "string",
+                "Email": "string",
+                "Id": "string",
+                "JoinedMethod": "",
+                "JoinedTimestamp": "",
+                "Name": "string",
+                "Status": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Domains"
-            ]
+                "Accounts"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "Lists the following prices for either all the TLDs supported by Route 53",
-            "function_name": "list_prices",
+            "function_description": "List Policies in  Organization",
+            "function_name": "list_policies",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "N",
+            "is_regional": "N",
             "json_response": {
-                "ChangeOwnershipPrice_Currency": "string",
-                "ChangeOwnershipPrice_Price": "",
+                "Arn": "string",
+                "AwsManaged": "",
+                "Description": "string",
+                "Id": "string",
                 "Name": "string",
-                "RegistrationPrice_Currency": "string",
-                "RegistrationPrice_Price": "",
-                "RenewalPrice_Currency": "string",
-                "RenewalPrice_Price": "",
-                "RestorationPrice_Currency": "string",
-                "RestorationPrice_Price": "",
-                "TransferPrice_Currency": "string",
-                "TransferPrice_Price": ""
+                "Type": ""
             },
-            "pagination_support": "Yes",
+            "pagination_attributes": [
+                {
+                    "attribute_name": "Filter",
+                    "attribute_value": "SERVICE_CONTROL_POLICY",
+                    "display_prompt": "",
+                    "is_visible": "N",
+                    "type": "str"
+                }
+            ],
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Prices"
-            ]
+                "Policies"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "route53domains"
+    "service_name": "organizations"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/s3.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/route53domains.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5576923076923077%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_domains', 'function_description': 'Domain names "*

 * *                "registered with Amazon Route 53 ', 'is_regional': 'N', 'pagination_support': 'Y', "*

 * *                "'result_keys': ['Domains'], 'json_response': {replace: "*

 * *                "OrderedDict([('DomainName', 'string'), ('AutoRenew', 'string'), ('TransferLock', "*

 * *                "'string'), ('Expiry', 'string')])}, 'is_multi_account_support': 'Y', 'implclass': "*

 * *                "'_global_paginate', 'imp […]*

```diff
@@ -1,77 +1,56 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "create bucket",
-            "function_name": "create_bucket",
-            "function_type": "create",
-            "is_regional": "No",
-            "json_response": {
-                "Location": "string"
-            },
-            "pagination_support": "No",
-            "response_format": "FORMAT_1"
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "list buckets",
-            "function_name": "list_buckets",
-            "function_type": "list",
-            "is_regional": "Yes",
-            "json_response": {
-                "CreationDate": "required",
-                "Name": "required"
-            },
-            "pagination_support": "No",
-            "response_format": "FORMAT_2",
-            "result_keys": [
-                "Buckets"
-            ]
-        },
-        {
-            "boto_session_type": "client",
-            "function_description": "list buckets",
-            "function_name": "list_multipart_uploads",
+            "function_description": "Domain names registered with Amazon Route 53 ",
+            "function_name": "list_domains",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
-                "ChecksumAlgorithm_0": "string",
-                "ETag": "string",
-                "Key": "required",
-                "LastModified": "required",
-                "Owner_DisplayName": "string",
-                "Owner_ID": "string",
-                "Size": "123",
-                "StorageClass": "required"
+                "AutoRenew": "string",
+                "DomainName": "string",
+                "Expiry": "string",
+                "TransferLock": "string"
             },
-            "pagination_support": "No",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Uploads"
-            ]
+                "Domains"
+            ],
+            "validation_functions": ""
         },
         {
             "boto_session_type": "client",
-            "function_description": "List Objects",
-            "function_name": "list_objects_v2",
+            "function_description": "Lists the following prices for either all the TLDs supported by Route 53",
+            "function_name": "list_prices",
             "function_type": "list",
-            "is_regional": "No",
+            "implclass": "_global_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "N",
             "json_response": {
-                "ChecksumAlgorithm_0": "",
-                "ETag": "string",
-                "Key": "string",
-                "LastModified": "",
-                "Owner_DisplayName": "string",
-                "Owner_ID": "string",
-                "Size": "",
-                "StorageClass": ""
+                "ChangeOwnershipPrice_Currency": "string",
+                "ChangeOwnershipPrice_Price": "",
+                "Name": "string",
+                "RegistrationPrice_Currency": "string",
+                "RegistrationPrice_Price": "",
+                "RenewalPrice_Currency": "string",
+                "RenewalPrice_Price": "",
+                "RestorationPrice_Currency": "string",
+                "RestorationPrice_Price": "",
+                "TransferPrice_Currency": "string",
+                "TransferPrice_Price": ""
             },
-            "pagination_support": "Yes",
+            "pagination_support": "Y",
             "response_format": "FORMAT_2",
             "result_keys": [
-                "Contents"
-            ]
+                "Prices"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "s3"
+    "service_name": "route53domains"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_config_mgr/service_configs/sqs.json` & `boto_formatter-2.0.0/src/boto_formatter/service_config_mgr/service_configs/codecommit.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6057692307692308%*

 * *Differences: {"'functions'": "{0: {'function_name': 'list_repositories', 'function_description': 'Gets "*

 * *                "information about one or more repositories.', 'response_format': 'FORMAT_2', "*

 * *                "'is_regional': 'Y', 'pagination_support': 'Y', 'result_keys': ['repositories'], "*

 * *                "'json_response': {replace: OrderedDict([('repositoryName', 'string'), "*

 * *                "('repositoryId', 'string')])}, 'is_multi_account_support': 'Y', 'implclass': "*

 * *                "'_regional_paginate', ' […]*

```diff
@@ -1,20 +1,25 @@
 {
     "functions": [
         {
             "boto_session_type": "client",
-            "function_description": "Returns a list of queues",
-            "function_name": "list_queues",
+            "function_description": "Gets information about one or more repositories.",
+            "function_name": "list_repositories",
             "function_type": "list",
-            "is_regional": "Yes",
+            "implclass": "_regional_paginate",
+            "implfunction": "process",
+            "is_multi_account_support": "Y",
+            "is_regional": "Y",
             "json_response": {
-                "QueueUrl": ""
+                "repositoryId": "string",
+                "repositoryName": "string"
             },
-            "pagination_support": "Yes",
-            "response_format": "FORMAT_3",
+            "pagination_support": "Y",
+            "response_format": "FORMAT_2",
             "result_keys": [
-                "QueueUrls"
-            ]
+                "repositories"
+            ],
+            "validation_functions": ""
         }
     ],
-    "service_name": "sqs"
+    "service_name": "codecommit"
 }
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter/service_formatter.py` & `boto_formatter-2.0.0/src/boto_formatter/service_formatter.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-
-import logging
-from sys import modules
-import os
-import boto_formatter.json_util.json_util as json_util
-from boto_formatter.service_config_mgr.service_config import ServiceConfig
-import time
-
-
-# Set up our logger
-logging.basicConfig(level=logging.ERROR)
-logger = logging.getLogger()
-
-
-def service_response_formatter(service_name, function_name, response, attributes=None):
-    """
-     service_response_formatter
-    :param service_name: example lambda, s3
-    :param function_name: example list_functions
-    :param response: list of json objects
-    :param attributes: format_type,output_to,output_path,pagination,required_only
-    :return: formatted response
-    """
-    format_type = None  # Options are json or csv. Default is json
-    output_to = None  # Options are print or file. Default is print
-    output_path = None  # Default is none, user can provide custom path
-    pagination = False
-    required_only = None  # Default is none if required only fields
-    # default type is json. Supported types are json,csv
-    if attributes is not None:
-        if "format_type" in attributes:
-            format_type = attributes["format_type"]
-        # output_to default is None. Supported options are cmd,file,s3
-        if "output_to" in attributes:
-            output_to = attributes["output_to"]
-        # output_to default is None. Supported options are complete file path or S3 path
-        if "output_path" in attributes:
-            output_path = attributes["output_path"]
-        if "pagination" in attributes:
-            if attributes["pagination"] == "True":
-                pagination = True
-        if "required_only" in attributes:
-            required_only = True
-    if output_path is None:
-        output_path = os.getcwd()
-    json_config = None
-    result = None
-    function_config = ServiceConfig.get_service_function_details(
-        service_name, function_name)
-    json_config = function_config["json_response"]
-    response_format = function_config["response_format"]
-    # Some columns breaks as comma so for csv format put required only condition
-
-    start_time = time.time()
-    result = __process_response(
-        function_config, json_config, format_type, required_only, response, pagination)
-    logger.debug("Flattening JSON took--- %s seconds ---" %
-                 (time.time() - start_time))
-    if format_type:
-        result = __format_ouput(result, format_type)
-    if output_to:
-        result = __ouput_to(service_name, function_name,
-                            result, output_to, format_type,
-                            output_path, response_format)
-    return result
-
-
-def __process_response(function_config, json_config, format_type, required_only, response, pagination):
-    """
-    :param function_config : function defined in service_config.json
-    :param json_config: reference response
-    :param required_only: if present filter the result for required onlydata
-    :param response : List of Json object
-    :pagination :if present json list is part of pagination
-    :return: formatted list of flattend JSON objects
-    """
-    response_format = function_config["response_format"]
-    result_keys = None
-    final_result = []
-    if "result_keys" in function_config.keys():
-        result_keys = function_config["result_keys"]
-    if required_only is None and format_type is not None:
-        if "csv_enforced_required_only" in function_config.keys() and format_type == "csv":
-            required_only = "Yes"
-    # FORMAT_1 : JSON single record
-    # FORMAT_2 : JSON contains List of JSON
-    # FORMAT_3 : JSON contains List of Strings
-    if response_format == "FORMAT_2":
-        # if pagination then get extended loop
-        if pagination:
-            for item in response:
-                result = item["result"]
-                prefix_columns = None
-                # prefix_colums work differently in service_formatter and core_formatter
-                if "prefix_columns" in item.keys():
-                    prefix_columns = item["prefix_columns"]
-                for obj in result:
-                    final_result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
-                        obj, result_keys), required_only, prefix_columns))
-        else:
-            for item in response:
-                result = item["result"]
-                prefix_columns = None
-                if "prefix_columns" in item.keys():
-                    prefix_columns = item["prefix_columns"]
-                final_result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
-                    result, result_keys), required_only, prefix_columns))
-    elif response_format == "FORMAT_1":
-        final_result = json_util.format_json_object(json_config, response)
-
-    elif response_format == "FORMAT_3":
-        # if pagination then get extended loop
-        if pagination:
-            for item in response:
-                result = item["result"]
-                prefix_columns = None
-                # prefix_colums work differently in service_formatter and core_formatter
-                if "prefix_columns" in item.keys():
-                    prefix_columns = item["prefix_columns"]
-                for obj in result:
-                    final_result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
-                        obj, result_keys), required_only, prefix_columns))
-        else:
-            for item in response:
-                result = item["result"]
-                prefix_columns = None
-                if "prefix_columns" in item.keys():
-                    prefix_columns = item["prefix_columns"]
-                final_result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
-                    result, result_keys), required_only, prefix_columns))
-
-    return final_result
-
-
-def __format_ouput(result, format_type):
-    """
-    :param result : Flatten JSON list
-    :param format_type: currently supported only csv
-    :return: formatted list of comma seperated string
-    """
-    if format_type == "csv":
-        return json_util.get_csv_data(result)
-    else:
-        return result
-
-
-def __ouput_to(service_name, function_name, result, output_to, format_type, output_path, response_format):
-    """
-    :param service_name :service_name like s3, lambda
-    :param function_name: function name like list_buckets
-    :param function_name: processed result
-    :param format_type: csv or json
-    :param output_path: user provided output_path to save file
-    :response_format:FORMAT_1,FORMAT_2,FORMAT_3
-    :return: formatted list of comma seperated string
-    """
-    if output_to == "print":
-        return json_util.print_csv_response(result)
-    elif output_to == "file" or output_to == "s3":
-        if format_type:
-            file_path = None
-            if format_type == "csv":
-                file_path = json_util.save_csv(
-                    result, service_name, function_name, output_path)
-            else:
-                file_path = json_util.save_json(
-                    result, service_name, function_name, output_path)
-        return file_path
-    else:
-        return result
+
+import logging
+from sys import modules
+import os
+import boto_formatter.json_util.json_util as json_util
+from boto_formatter.service_config_mgr.service_config import ServiceConfig
+import time
+
+
+# Set up our logger
+logging.basicConfig(level=logging.ERROR)
+logger = logging.getLogger()
+
+
+def service_response_formatter(service_name, function_name, response, attributes=None):
+    """
+     service_response_formatter
+    :param service_name: example lambda, s3
+    :param function_name: example list_functions
+    :param response: list of json objects
+    :param attributes: format_type,output_to,output_path,pagination,required_only
+    :return: formatted response
+    """
+    format_type = None  # Options are json or csv. Default is json
+    output_to = None  # Options are print or file. Default is print
+    output_path = None  # Default is none, user can provide custom path
+    pagination = False
+    required_only = None  # Default is none if required only fields
+    # default type is json. Supported types are json,csv
+    if attributes is not None:
+        if "format_type" in attributes:
+            format_type = attributes["format_type"]
+        # output_to default is None. Supported options are cmd,file,s3
+        if "output_to" in attributes:
+            output_to = attributes["output_to"]
+        # output_to default is None. Supported options are complete file path or S3 path
+        if "output_path" in attributes:
+            output_path = attributes["output_path"]
+        if "pagination" in attributes:
+            if attributes["pagination"] == "True":
+                pagination = True
+        if "required_only" in attributes:
+            required_only = True
+    if output_path is None:
+        output_path = os.getcwd()
+    json_config = None
+    result = None
+    function_config = ServiceConfig.get_service_function_details(
+        service_name, function_name)
+    json_config = function_config["json_response"]
+    response_format = function_config["response_format"]
+    # Some columns breaks as comma so for csv format put required only condition
+
+    start_time = time.time()
+    result = __process_response(
+        function_config, json_config, format_type, required_only, response, pagination)
+    logger.debug("Flattening JSON took--- %s seconds ---" %
+                 (time.time() - start_time))
+    if format_type:
+        result = __format_ouput(result, format_type)
+    if output_to:
+        result = __ouput_to(service_name, function_name,
+                            result, output_to, format_type,
+                            output_path, response_format)
+    return result
+
+
+def __process_response(function_config, json_config, format_type, required_only, response, pagination):
+    """
+    :param function_config : function defined in service_config.json
+    :param json_config: reference response
+    :param required_only: if present filter the result for required onlydata
+    :param response : List of Json object
+    :pagination :if present json list is part of pagination
+    :return: formatted list of flattend JSON objects
+    """
+    response_format = function_config["response_format"]
+    result_keys = None
+    final_result = []
+    if "result_keys" in function_config.keys():
+        result_keys = function_config["result_keys"]
+    if required_only is None and format_type is not None:
+        if "csv_enforced_required_only" in function_config.keys() and format_type == "csv":
+            required_only = "Yes"
+    # FORMAT_1 : JSON single record
+    # FORMAT_2 : JSON contains List of JSON
+    # FORMAT_3 : JSON contains List of Strings
+    if response_format == "FORMAT_2":
+        # if pagination then get extended loop
+        if pagination:
+            for item in response:
+                result = item["result"]
+                prefix_columns = None
+                # prefix_colums work differently in service_formatter and core_formatter
+                if "prefix_columns" in item.keys():
+                    prefix_columns = item["prefix_columns"]
+                for obj in result:
+                    final_result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
+                        obj, result_keys), required_only, prefix_columns))
+        else:
+            for item in response:
+                result = item["result"]
+                prefix_columns = None
+                if "prefix_columns" in item.keys():
+                    prefix_columns = item["prefix_columns"]
+                final_result.extend(json_util.format_json_list(json_config, json_util.format_response_for_result_keys(
+                    result, result_keys), required_only, prefix_columns))
+    elif response_format == "FORMAT_1":
+        final_result = json_util.format_json_object(json_config, response)
+
+    elif response_format == "FORMAT_3":
+        # if pagination then get extended loop
+        if pagination:
+            for item in response:
+                result = item["result"]
+                prefix_columns = None
+                # prefix_colums work differently in service_formatter and core_formatter
+                if "prefix_columns" in item.keys():
+                    prefix_columns = item["prefix_columns"]
+                for obj in result:
+                    final_result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
+                        obj, result_keys), required_only, prefix_columns))
+        else:
+            for item in response:
+                result = item["result"]
+                prefix_columns = None
+                if "prefix_columns" in item.keys():
+                    prefix_columns = item["prefix_columns"]
+                final_result.extend(json_util.format_str_list(json_config, json_util.format_response_for_result_keys(
+                    result, result_keys), required_only, prefix_columns))
+
+    return final_result
+
+
+def __format_ouput(result, format_type):
+    """
+    :param result : Flatten JSON list
+    :param format_type: currently supported only csv
+    :return: formatted list of comma seperated string
+    """
+    if format_type == "csv":
+        return json_util.get_csv_data(result)
+    else:
+        return result
+
+
+def __ouput_to(service_name, function_name, result, output_to, format_type, output_path, response_format):
+    """
+    :param service_name :service_name like s3, lambda
+    :param function_name: function name like list_buckets
+    :param function_name: processed result
+    :param format_type: csv or json
+    :param output_path: user provided output_path to save file
+    :response_format:FORMAT_1,FORMAT_2,FORMAT_3
+    :return: formatted list of comma seperated string
+    """
+    if output_to == "print":
+        return json_util.print_csv_response(result)
+    elif output_to == "file" or output_to == "s3":
+        if format_type:
+            file_path = None
+            if format_type == "csv":
+                file_path = json_util.save_csv(
+                    result, service_name, function_name, output_path)
+            else:
+                file_path = json_util.save_json(
+                    result, service_name, function_name, output_path)
+        return file_path
+    else:
+        return result
```

### Comparing `boto_formatter-1.0.0/src/boto_formatter.egg-info/SOURCES.txt` & `boto_formatter-2.0.0/src/boto_formatter.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+.venv/Lib/site-packages/boto_formatter-2.0.0.dist-info/direct_url.json
 src/boto_formatter/__init__.py
+src/boto_formatter/boto_magic_formatter.py
 src/boto_formatter/core_formatter.py
 src/boto_formatter/service_formatter.py
 src/boto_formatter.egg-info/PKG-INFO
 src/boto_formatter.egg-info/SOURCES.txt
 src/boto_formatter.egg-info/dependency_links.txt
 src/boto_formatter.egg-info/top_level.txt
 src/boto_formatter/json_util/__init__.py
 src/boto_formatter/json_util/json_util.py
 src/boto_formatter/service_config_mgr/__init__.py
 src/boto_formatter/service_config_mgr/service_config.py
-src/boto_formatter/service_config_mgr/service_configs/__init__.py
 src/boto_formatter/service_config_mgr/service_configs/accessanalyzer.json
+src/boto_formatter/service_config_mgr/service_configs/account.json
+src/boto_formatter/service_config_mgr/service_configs/acm.json
+src/boto_formatter/service_config_mgr/service_configs/amp.json
 src/boto_formatter/service_config_mgr/service_configs/apigateway.json
 src/boto_formatter/service_config_mgr/service_configs/budgets.json
+src/boto_formatter/service_config_mgr/service_configs/cleanrooms.json
+src/boto_formatter/service_config_mgr/service_configs/cloudformation.json
 src/boto_formatter/service_config_mgr/service_configs/cloudfront.json
 src/boto_formatter/service_config_mgr/service_configs/cloudtrail.json
 src/boto_formatter/service_config_mgr/service_configs/cloudwatch.json
 src/boto_formatter/service_config_mgr/service_configs/codecommit.json
-src/boto_formatter/service_config_mgr/service_configs/describe_cache_clusters.json
 src/boto_formatter/service_config_mgr/service_configs/dynamodb.json
 src/boto_formatter/service_config_mgr/service_configs/ec2.json
 src/boto_formatter/service_config_mgr/service_configs/ecs.json
 src/boto_formatter/service_config_mgr/service_configs/efs.json
 src/boto_formatter/service_config_mgr/service_configs/eks.json
 src/boto_formatter/service_config_mgr/service_configs/elasticache.json
 src/boto_formatter/service_config_mgr/service_configs/elbv2.json
@@ -34,12 +39,15 @@
 src/boto_formatter/service_config_mgr/service_configs/iam.json
 src/boto_formatter/service_config_mgr/service_configs/kms.json
 src/boto_formatter/service_config_mgr/service_configs/lambda.json
 src/boto_formatter/service_config_mgr/service_configs/organizations.json
 src/boto_formatter/service_config_mgr/service_configs/rds.json
 src/boto_formatter/service_config_mgr/service_configs/redshift-serverless.json
 src/boto_formatter/service_config_mgr/service_configs/redshift.json
+src/boto_formatter/service_config_mgr/service_configs/resourcegroupstaggingapi.json
 src/boto_formatter/service_config_mgr/service_configs/route53.json
 src/boto_formatter/service_config_mgr/service_configs/route53domains.json
 src/boto_formatter/service_config_mgr/service_configs/s3.json
+src/boto_formatter/service_config_mgr/service_configs/sagemaker.json
 src/boto_formatter/service_config_mgr/service_configs/sns.json
-src/boto_formatter/service_config_mgr/service_configs/sqs.json
+src/boto_formatter/service_config_mgr/service_configs/sqs.json
+src/boto_formatter/service_config_mgr/service_configs/ssm.json
```

