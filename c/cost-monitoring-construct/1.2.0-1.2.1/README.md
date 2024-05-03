# Comparing `tmp/cost-monitoring-construct-1.2.0.tar.gz` & `tmp/cost-monitoring-construct-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-monitoring-construct-1.2.0.tar", last modified: Mon Apr 29 12:52:43 2024, max compression
+gzip compressed data, was "cost-monitoring-construct-1.2.1.tar", last modified: Fri May  3 07:23:16 2024, max compression
```

## Comparing `cost-monitoring-construct-1.2.0.tar` & `cost-monitoring-construct-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.756587 cost-monitoring-construct-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/
--rw-r--r--   0 runner    (1001) docker     (127)    70040 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77521 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:52:30.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:52:43.760587 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 12:52:43.000000 cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/
+-rw-r--r--   0 runner    (1001) docker     (127)    71512 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79038 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:23:02.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:23:16.020007 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-03 07:23:15.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 07:23:15.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:23:15.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 07:23:15.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 07:23:15.000000 cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/top_level.txt
```

### Comparing `cost-monitoring-construct-1.2.0/LICENSE` & `cost-monitoring-construct-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-monitoring-construct-1.2.0/PKG-INFO` & `cost-monitoring-construct-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.2.0
+Version: 1.2.1
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,54 +24,56 @@
 
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
-# How to use Cost Monitoring Construct?
+## How to use Cost Monitoring Construct?
 
 To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
 
 For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
 
-# Why do you need it?
+## Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
-# How does Cost Monitoring Construct work?
+## How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
 
 Cost Monitoring Construct provides the following features:
 
 * **Cost dashboard:** Displays your current costs and usage, broken down by application's name, region, and etc. Allows you to see how much you are spending on each application and where you might be able to reduce costs.
 * **Budgets:** Allows you to set budgets for each applications. It will automatically set up alerts to notify you when your actual costs exceed your budgeted costs. It also continues to track the cost and sending alert if an application continues to cost drastically.
 * **Integration:** Integrates with various tools and monitoring services, such as AWS Cost Explorer and Datadog.
 
-# What is it useful for?
+> [!WARNING]
+> ApplicationCostMonitoring uses AWS Tags to track resources' usages. You must [activate](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/activating-tags.html) your chosen tag key (`cm:application` by default) under Cost Allocation Tags. The tag key will appear in the AWS console up to 24 hours after at least one AWS resource has been created with that tag.
+
+## What is it useful for?
 
 Cost Monitoring Construct is useful for anyone who uses AWS and wants to keep their costs under control. It is particularly useful for:
 
 * **Startups and small businesses:** Cost Monitoring Construct can help startups and small businesses to keep their costs under control during the early stages of growth.
 * **Large enterprises:** Cost Monitoring Construct can help large enterprises to optimize their cloud usage and reduce costs across multiple teams and departments.
 * **Developers:** Cost Monitoring Construct can help developers to track their usage and costs across multiple projects and services.
 
-# What is this *not* useful for?
+## What is this *not* useful for?
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
-# Which programming languages Cost Monitoring Construct supports?
+## Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
 * [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [Python](https://pypi.org/project/cost-monitoring-construct/)
 * [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
 * [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
-> **✏️ Note**
->
+> [!NOTE]
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cost-monitoring-construct-1.2.0/README.md` & `cost-monitoring-construct-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
-# How to use Cost Monitoring Construct?
+## How to use Cost Monitoring Construct?
 
 To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
 
 For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
 
-# Why do you need it?
+## Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
-# How does Cost Monitoring Construct work?
+## How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
 
 Cost Monitoring Construct provides the following features:
 
 * **Cost dashboard:** Displays your current costs and usage, broken down by application's name, region, and etc. Allows you to see how much you are spending on each application and where you might be able to reduce costs.
 * **Budgets:** Allows you to set budgets for each applications. It will automatically set up alerts to notify you when your actual costs exceed your budgeted costs. It also continues to track the cost and sending alert if an application continues to cost drastically.
 * **Integration:** Integrates with various tools and monitoring services, such as AWS Cost Explorer and Datadog.
 
-# What is it useful for?
+> [!WARNING]
+> ApplicationCostMonitoring uses AWS Tags to track resources' usages. You must [activate](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/activating-tags.html) your chosen tag key (`cm:application` by default) under Cost Allocation Tags. The tag key will appear in the AWS console up to 24 hours after at least one AWS resource has been created with that tag.
+
+## What is it useful for?
 
 Cost Monitoring Construct is useful for anyone who uses AWS and wants to keep their costs under control. It is particularly useful for:
 
 * **Startups and small businesses:** Cost Monitoring Construct can help startups and small businesses to keep their costs under control during the early stages of growth.
 * **Large enterprises:** Cost Monitoring Construct can help large enterprises to optimize their cloud usage and reduce costs across multiple teams and departments.
 * **Developers:** Cost Monitoring Construct can help developers to track their usage and costs across multiple projects and services.
 
-# What is this *not* useful for?
+## What is this *not* useful for?
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
-# Which programming languages Cost Monitoring Construct supports?
+## Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
 * [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [Python](https://pypi.org/project/cost-monitoring-construct/)
 * [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
 * [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
-> **✏️ Note**
->
+> [!NOTE]
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cost-monitoring-construct-1.2.0/setup.py` & `cost-monitoring-construct-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cost-monitoring-construct",
-    "version": "1.2.0",
+    "version": "1.2.1",
     "description": "A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage",
     "license": "Apache-2.0",
     "url": "https://github.com/DataChefHQ/cost-monitoring-construct.git",
     "long_description_content_type": "text/markdown",
     "author": "DataChef<support@datachef.co>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cost_monitoring_construct",
         "cost_monitoring_construct._jsii"
     ],
     "package_data": {
         "cost_monitoring_construct._jsii": [
-            "cost-monitoring-construct@1.2.0.jsii.tgz"
+            "cost-monitoring-construct@1.2.1.jsii.tgz"
         ],
         "cost_monitoring_construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct/__init__.py` & `cost-monitoring-construct-1.2.1/src/cost_monitoring_construct/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 '''
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
-# How to use Cost Monitoring Construct?
+## How to use Cost Monitoring Construct?
 
 To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
 
 For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
 
-# Why do you need it?
+## Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
-# How does Cost Monitoring Construct work?
+## How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
 
 Cost Monitoring Construct provides the following features:
 
 * **Cost dashboard:** Displays your current costs and usage, broken down by application's name, region, and etc. Allows you to see how much you are spending on each application and where you might be able to reduce costs.
 * **Budgets:** Allows you to set budgets for each applications. It will automatically set up alerts to notify you when your actual costs exceed your budgeted costs. It also continues to track the cost and sending alert if an application continues to cost drastically.
 * **Integration:** Integrates with various tools and monitoring services, such as AWS Cost Explorer and Datadog.
 
-# What is it useful for?
+> [!WARNING]
+> ApplicationCostMonitoring uses AWS Tags to track resources' usages. You must [activate](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/activating-tags.html) your chosen tag key (`cm:application` by default) under Cost Allocation Tags. The tag key will appear in the AWS console up to 24 hours after at least one AWS resource has been created with that tag.
+
+## What is it useful for?
 
 Cost Monitoring Construct is useful for anyone who uses AWS and wants to keep their costs under control. It is particularly useful for:
 
 * **Startups and small businesses:** Cost Monitoring Construct can help startups and small businesses to keep their costs under control during the early stages of growth.
 * **Large enterprises:** Cost Monitoring Construct can help large enterprises to optimize their cloud usage and reduce costs across multiple teams and departments.
 * **Developers:** Cost Monitoring Construct can help developers to track their usage and costs across multiple projects and services.
 
-# What is this *not* useful for?
+## What is this *not* useful for?
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
-# Which programming languages Cost Monitoring Construct supports?
+## Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
 * [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [Python](https://pypi.org/project/cost-monitoring-construct/)
 * [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
 * [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
-> **✏️ Note**
->
+> [!NOTE]
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
 '''
 import abc
 import builtins
 import datetime
@@ -1002,16 +1004,15 @@
         '''Default Application CostMonitoring class that implements daily and monthly budgets.
 
         :param stack: - default stack to track its resources and it will be used to define Budget resources in it.
         :param props: -
 
         Example::
 
-            .com'
-            ]
+            .com']
             });
             
             budgetStratgy.monitor();
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__361ff8775d5ca30a358315f98c5b27b9eb15f57051ae67ebfad4c5e0c037aedf)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
@@ -1195,84 +1196,95 @@
         monthly_limit_in_dollars: jsii.Number,
         other_stacks_included_in_budget: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.Stack]] = None,
         default_topic: typing.Optional[builtins.str] = None,
         subscribers: typing.Optional[typing.Sequence[builtins.str]] = None,
         cost_allocation_tag: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param application_name: -
-        :param monthly_limit_in_dollars: -
-        :param other_stacks_included_in_budget: -
-        :param default_topic: -
-        :param subscribers: -
-        :param cost_allocation_tag: -
+        :param application_name: - the name of application to label resources with it.
+        :param monthly_limit_in_dollars: - montly limit in US Dollors.
+        :param other_stacks_included_in_budget: - optional other stack to track their resources alog with the default stack.
+        :param default_topic: - default SNS topic name. Only if provided, the BudgetStratgy creates an SNS topic and send notifications to it.
+        :param subscribers: - list of email address that the CostMonitoring will use to send alerts to.
+        :param cost_allocation_tag: - Tag key used to track resources' expenditure. Only if provided, it will be used to tag the application resources. Defaults to ``cm:application``
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__016611925949da4facbba95bcddcf14217d235eea769e2db3a3d240c6ca86d73)
             check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
             check_type(argname="argument monthly_limit_in_dollars", value=monthly_limit_in_dollars, expected_type=type_hints["monthly_limit_in_dollars"])
             check_type(argname="argument other_stacks_included_in_budget", value=other_stacks_included_in_budget, expected_type=type_hints["other_stacks_included_in_budget"])
             check_type(argname="argument default_topic", value=default_topic, expected_type=type_hints["default_topic"])
             check_type(argname="argument subscribers", value=subscribers, expected_type=type_hints["subscribers"])
             check_type(argname="argument cost_allocation_tag", value=cost_allocation_tag, expected_type=type_hints["cost_allocation_tag"])
         jsii.create(self.__class__, self, [application_name, monthly_limit_in_dollars, other_stacks_included_in_budget, default_topic, subscribers, cost_allocation_tag])
 
     @builtins.property
     @jsii.member(jsii_name="applicationName")
     def application_name(self) -> builtins.str:
+        '''- the name of application to label resources with it.'''
         return typing.cast(builtins.str, jsii.get(self, "applicationName"))
 
     @application_name.setter
     def application_name(self, value: builtins.str) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4fd4ce542700b2deac40811890f4429d90eac081bd29d08415e6ce8667697422)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationName", value)
 
     @builtins.property
     @jsii.member(jsii_name="monthlyLimitInDollars")
     def monthly_limit_in_dollars(self) -> jsii.Number:
+        '''- montly limit in US Dollors.'''
         return typing.cast(jsii.Number, jsii.get(self, "monthlyLimitInDollars"))
 
     @monthly_limit_in_dollars.setter
     def monthly_limit_in_dollars(self, value: jsii.Number) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__57b7dbe15daa64f31317dedf1362713156a13c2d526b10bae05bb824fb1852b5)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "monthlyLimitInDollars", value)
 
     @builtins.property
     @jsii.member(jsii_name="costAllocationTag")
     def cost_allocation_tag(self) -> typing.Optional[builtins.str]:
+        '''- Tag key used to track resources' expenditure.
+
+        Only if provided, it will be used to tag the application resources. Defaults to ``cm:application``
+        '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "costAllocationTag"))
 
     @cost_allocation_tag.setter
     def cost_allocation_tag(self, value: typing.Optional[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3bd683e50b33baeaf6f59fc99784ce52773a612c0f5a480e422ab4972f7f6e2b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "costAllocationTag", value)
 
     @builtins.property
     @jsii.member(jsii_name="defaultTopic")
     def default_topic(self) -> typing.Optional[builtins.str]:
+        '''- default SNS topic name.
+
+        Only if provided, the BudgetStratgy creates an SNS topic and send notifications to it.
+        '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "defaultTopic"))
 
     @default_topic.setter
     def default_topic(self, value: typing.Optional[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a36b5adee3e84bbffda1fbfb9801304b1780cd8ef3dc089586a0aeee043a09a7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultTopic", value)
 
     @builtins.property
     @jsii.member(jsii_name="otherStacksIncludedInBudget")
     def other_stacks_included_in_budget(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]]:
+        '''- optional other stack to track their resources alog with the default stack.'''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]], jsii.get(self, "otherStacksIncludedInBudget"))
 
     @other_stacks_included_in_budget.setter
     def other_stacks_included_in_budget(
         self,
         value: typing.Optional[typing.List[_aws_cdk_ceddda9d.Stack]],
     ) -> None:
@@ -1280,14 +1292,15 @@
             type_hints = typing.get_type_hints(_typecheckingstub__27ca7aaaa6cac405f55855e5078ed65603a6f03c771242fe182f13cf406a81a0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "otherStacksIncludedInBudget", value)
 
     @builtins.property
     @jsii.member(jsii_name="subscribers")
     def subscribers(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''- list of email address that the CostMonitoring will use to send alerts to.'''
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "subscribers"))
 
     @subscribers.setter
     def subscribers(self, value: typing.Optional[typing.List[builtins.str]]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bac5a7c82099fee82a0b4f1e50169bd023e5de76ee7c699ab88840159ea951e2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/PKG-INFO` & `cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-monitoring-construct
-Version: 1.2.0
+Version: 1.2.1
 Summary: A CDK construct that helps track applications' costs separately and receive alerts in case of unpredicted resource usage
 Home-page: https://github.com/DataChefHQ/cost-monitoring-construct.git
 Author: DataChef<support@datachef.co>
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataChefHQ/cost-monitoring-construct.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,54 +24,56 @@
 
 # What is Cost Monitoring Construct?
 
 Cost Monitoring Construct is a CDK library that helps monitor costs for AWS cloud infrastructure resources, such as virtual machines, storage, and network traffic. It allows you to set budgets and alerts to ensure that you don't overspend on your cloud resources.
 
 With the Cost Monitoring Construct, you can share the responsibility of cost management between developers and business holders. This is achieved through the creation of meaningful reports that enable the business team to make informed decisions. Additionally, the Construct generates boilerplate code that can be used to apply these decisions in practice, making it easier to stay on top of your budget.
 
-# How to use Cost Monitoring Construct?
+## How to use Cost Monitoring Construct?
 
 To use Cost Monitoring Construct, all you need is to have the AWS CDK installed and set up. Once you have that, you can install the package from the repository of your choice.
 
 For more information on using this Construct in TypeScript checkout the [TypeScript documentation](docs/typescript.md). You can also check the typescript example from [sample folder](https://github.com/DataChefHQ/cost-monitoring-construct/tree/main/sample) on the GitHub repository.
 
-# Why do you need it?
+## Why do you need it?
 
 Cloud services can get very expensive, very quickly, especially if you are not careful with your usage. Cost Monitoring Construct helps you to keep an eye on your cloud infrastructure costs so that you can stay within budget. By setting budgets and defining alert strategies, you can take proactive steps to reduce costs before they become a problem.
 
-# How does Cost Monitoring Construct work?
+## How does Cost Monitoring Construct work?
 
 Cost Monitoring Construct uses AWS Tagging practice to track resources related to an specific application, creates proper alert with respect to the defined budget limit and provide overview dashbords. The tool is highly customizable and allows you to customize it to your budgeting strategy based on your specific needs.
 
 Cost Monitoring Construct provides the following features:
 
 * **Cost dashboard:** Displays your current costs and usage, broken down by application's name, region, and etc. Allows you to see how much you are spending on each application and where you might be able to reduce costs.
 * **Budgets:** Allows you to set budgets for each applications. It will automatically set up alerts to notify you when your actual costs exceed your budgeted costs. It also continues to track the cost and sending alert if an application continues to cost drastically.
 * **Integration:** Integrates with various tools and monitoring services, such as AWS Cost Explorer and Datadog.
 
-# What is it useful for?
+> [!WARNING]
+> ApplicationCostMonitoring uses AWS Tags to track resources' usages. You must [activate](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/activating-tags.html) your chosen tag key (`cm:application` by default) under Cost Allocation Tags. The tag key will appear in the AWS console up to 24 hours after at least one AWS resource has been created with that tag.
+
+## What is it useful for?
 
 Cost Monitoring Construct is useful for anyone who uses AWS and wants to keep their costs under control. It is particularly useful for:
 
 * **Startups and small businesses:** Cost Monitoring Construct can help startups and small businesses to keep their costs under control during the early stages of growth.
 * **Large enterprises:** Cost Monitoring Construct can help large enterprises to optimize their cloud usage and reduce costs across multiple teams and departments.
 * **Developers:** Cost Monitoring Construct can help developers to track their usage and costs across multiple projects and services.
 
-# What is this *not* useful for?
+## What is this *not* useful for?
 
 The Cost Monitoring Construct is not a magical tool that can solve all of your cloud cost problems. In spite of the fact that it can bring clarity and help you to identify areas where you can reduce costs, you must make the necessary decisions about your infrastructure on your own.
 
-# Which programming languages Cost Monitoring Construct supports?
+## Which programming languages Cost Monitoring Construct supports?
 
 Cost Monitoring Construct has been developed using JSII technolgy to provide interfaces for different modern programming languages. Currently, it supports the following languages:
 
 * [TypeScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [JavaScript](https://www.npmjs.com/package/cost-monitoring-construct)
 * [Python](https://pypi.org/project/cost-monitoring-construct/)
 * [.NET](https://www.nuget.org/packages/DataChef.CostMonitoringConstruct)
 * [Java](https://central.sonatype.com/artifact/co.datachef/costmonitoringconstruct/1.1.0/versions)
 
-> **✏️ Note**
->
+> [!NOTE]
 > Go will be supported soon but for now you can build it from the source.
 
 If you have any questions or need help with Cost Monitoring Construct, you can reach out to our support team at [support@datachef.co](mailto:support@datachef.co).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cost-monitoring-construct-1.2.0/src/cost_monitoring_construct.egg-info/SOURCES.txt` & `cost-monitoring-construct-1.2.1/src/cost_monitoring_construct.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cost_monitoring_construct/py.typed
 src/cost_monitoring_construct.egg-info/PKG-INFO
 src/cost_monitoring_construct.egg-info/SOURCES.txt
 src/cost_monitoring_construct.egg-info/dependency_links.txt
 src/cost_monitoring_construct.egg-info/requires.txt
 src/cost_monitoring_construct.egg-info/top_level.txt
 src/cost_monitoring_construct/_jsii/__init__.py
-src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.0.jsii.tgz
+src/cost_monitoring_construct/_jsii/cost-monitoring-construct@1.2.1.jsii.tgz
```

