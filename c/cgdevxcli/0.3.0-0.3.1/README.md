# Comparing `tmp/cgdevxcli-0.3.0.tar.gz` & `tmp/cgdevxcli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgdevxcli-0.3.0.tar", max compression
+gzip compressed data, was "cgdevxcli-0.3.1.tar", max compression
```

## Comparing `cgdevxcli-0.3.0.tar` & `cgdevxcli-0.3.1.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     2645 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/README.md
--rw-r--r--   0        0        0      497 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/.flake8
--rw-r--r--   0        0        0       83 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/__init__.py
--rw-r--r--   0        0        0      366 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/__main__.py
--rw-r--r--   0        0        0     1217 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/build.py
--rw-r--r--   0        0        0     7224 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/README.md
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/__init__.py
--rw-r--r--   0        0        0     6138 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/destroy.py
--rw-r--r--   0        0        0    48324 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/setup.py
--rw-r--r--   0        0        0     7816 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/README.md
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/__init__.py
--rw-r--r--   0        0        0    15215 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/bootstrap.py
--rw-r--r--   0        0        0     4398 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/create.py
--rw-r--r--   0        0        0     8962 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/delete.py
--rw-r--r--   0        0        0      235 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/commands/workload/workload.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/const/__init__.py
--rw-r--r--   0        0        0      903 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/const/common_path.py
--rw-r--r--   0        0        0     1007 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/const/const.py
--rw-r--r--   0        0        0      247 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/const/namespaces.py
--rw-r--r--   0        0        0      767 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/const/parameter_names.py
--rw-r--r--   0        0        0     1006 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/custom_excpetions.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.122632 cgdevxcli-0.3.0/cli/common/enums/__init__.py
--rw-r--r--   0        0        0      787 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/enums/cloud_providers.py
--rw-r--r--   0        0        0      799 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/enums/dns_registrars.py
--rw-r--r--   0        0        0      263 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/enums/git_plans.py
--rw-r--r--   0        0        0      788 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/enums/git_providers.py
--rw-r--r--   0        0        0     1779 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/logging_config.py
--rw-r--r--   0        0        0      830 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/retry_decorator.py
--rw-r--r--   0        0        0      307 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/singleton_metaclass.py
--rw-r--r--   0        0        0     3574 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/state_store.py
--rw-r--r--   0        0        0     1258 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/tracing_decorator.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/utils/__init__.py
--rw-r--r--   0        0        0    12697 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/utils/command_utils.py
--rw-r--r--   0        0        0      314 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/utils/generators.py
--rw-r--r--   0        0        0      187 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/common/utils/os_utils.py
--rw-r--r--   0        0        0      532 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/README.md
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/aws/__init__.py
--rw-r--r--   0        0        0     6482 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/aws/aws_manager.py
--rw-r--r--   0        0        0    11353 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/aws/aws_sdk.py
--rw-r--r--   0        0        0      932 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/aws/aws_session_manager.py
--rw-r--r--   0        0        0     5126 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/aws/iam_permissions.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/azure/__init__.py
--rw-r--r--   0        0        0    11546 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/azure/azure_manager.py
--rw-r--r--   0        0        0    25095 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/azure/azure_sdk.py
--rw-r--r--   0        0        0     5846 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/azure/iam_permissions.py
--rw-r--r--   0        0        0     4460 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/cloud/cloud_provider_manager.py
--rw-r--r--   0        0        0     6504 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dependency_manager.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/azure_dns/__init__.py
--rw-r--r--   0        0        0     1819 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/azure_dns/azure_dns.py
--rw-r--r--   0        0        0     2049 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/dns_provider_manager.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/route53/__init__.py
--rw-r--r--   0        0        0     1788 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/dns/route53/route53.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/config_builder.py
--rw-r--r--   0        0        0     6622 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/delivery_service_manager.py
--rw-r--r--   0        0        0    21428 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/k8s.py
--rw-r--r--   0        0        0     2150 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/kctl_wrapper.py
--rw-r--r--   0        0        0      461 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/k8s/kubeconfig.yaml
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/keys/__init__.py
--rw-r--r--   0        0        0     2156 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/keys/key_manager.py
--rw-r--r--   0        0        0     9269 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/platform_gitops.py
--rw-r--r--   0        0        0     6121 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/platform_template_manager.py
--rw-r--r--   0        0        0    15527 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/tf_wrapper.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/__init__.py
--rw-r--r--   0        0        0     2025 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/git_provider_manager.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/github/__init__.py
--rw-r--r--   0        0        0     5614 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/github/github_manager.py
--rw-r--r--   0        0        0        0 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/gitlab/__init__.py
--rw-r--r--   0        0        0     7767 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/vcs/gitlab/gitlab_manager.py
--rw-r--r--   0        0        0    12262 2024-04-18 22:03:27.126633 cgdevxcli-0.3.0/cli/services/wl_template_manager.py
--rw-r--r--   0        0        0     1226 2024-04-18 22:03:40.746824 cgdevxcli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4020 1970-01-01 00:00:00.000000 cgdevxcli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2645 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/README.md
+-rw-r--r--   0        0        0      497 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/.flake8
+-rw-r--r--   0        0        0       83 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/__main__.py
+-rw-r--r--   0        0        0     1217 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/build.py
+-rw-r--r--   0        0        0     7224 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/commands/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6387 2024-05-03 12:23:17.048450 cgdevxcli-0.3.1/cli/commands/destroy.py
+-rw-r--r--   0        0        0    48822 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/setup.py
+-rw-r--r--   0        0        0     7955 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/__init__.py
+-rw-r--r--   0        0        0    15465 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/bootstrap.py
+-rw-r--r--   0        0        0     4384 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/create.py
+-rw-r--r--   0        0        0    10397 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/delete.py
+-rw-r--r--   0        0        0      235 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/commands/workload/workload.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/const/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/const/common_path.py
+-rw-r--r--   0        0        0     1007 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/const/const.py
+-rw-r--r--   0        0        0      247 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/const/namespaces.py
+-rw-r--r--   0        0        0      767 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/const/parameter_names.py
+-rw-r--r--   0        0        0     1006 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/custom_excpetions.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/enums/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/enums/cloud_providers.py
+-rw-r--r--   0        0        0      799 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/enums/dns_registrars.py
+-rw-r--r--   0        0        0      263 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/enums/git_plans.py
+-rw-r--r--   0        0        0      788 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/enums/git_providers.py
+-rw-r--r--   0        0        0     1779 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/logging_config.py
+-rw-r--r--   0        0        0      830 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/retry_decorator.py
+-rw-r--r--   0        0        0      307 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/singleton_metaclass.py
+-rw-r--r--   0        0        0     3574 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/state_store.py
+-rw-r--r--   0        0        0     1258 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/tracing_decorator.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/utils/__init__.py
+-rw-r--r--   0        0        0    12697 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/utils/command_utils.py
+-rw-r--r--   0        0        0      314 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/utils/generators.py
+-rw-r--r--   0        0        0     3564 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/utils/k8s_utils.py
+-rw-r--r--   0        0        0      187 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/common/utils/os_utils.py
+-rw-r--r--   0        0        0      532 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/aws/__init__.py
+-rw-r--r--   0        0        0     6585 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/aws/aws_manager.py
+-rw-r--r--   0        0        0    11353 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/aws/aws_sdk.py
+-rw-r--r--   0        0        0      932 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/aws/aws_session_manager.py
+-rw-r--r--   0        0        0     5126 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/aws/iam_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/azure/__init__.py
+-rw-r--r--   0        0        0    11650 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/azure/azure_manager.py
+-rw-r--r--   0        0        0    25095 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/azure/azure_sdk.py
+-rw-r--r--   0        0        0     5846 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/azure/iam_permissions.py
+-rw-r--r--   0        0        0     4683 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/cloud/cloud_provider_manager.py
+-rw-r--r--   0        0        0     6504 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dependency_manager.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/azure_dns/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/azure_dns/azure_dns.py
+-rw-r--r--   0        0        0     2049 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/dns_provider_manager.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/route53/__init__.py
+-rw-r--r--   0        0        0     1788 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/dns/route53/route53.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/__init__.py
+-rw-r--r--   0        0        0     1271 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/config_builder.py
+-rw-r--r--   0        0        0     6622 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/delivery_service_manager.py
+-rw-r--r--   0        0        0    21428 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/k8s.py
+-rw-r--r--   0        0        0     2150 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/kctl_wrapper.py
+-rw-r--r--   0        0        0      461 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/k8s/kubeconfig.yaml
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/keys/__init__.py
+-rw-r--r--   0        0        0     2156 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/keys/key_manager.py
+-rw-r--r--   0        0        0    10006 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/platform_gitops.py
+-rw-r--r--   0        0        0     6121 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/platform_template_manager.py
+-rw-r--r--   0        0        0    15527 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/tf_wrapper.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/git_provider_manager.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/github/__init__.py
+-rw-r--r--   0        0        0     5614 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/github/github_manager.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/gitlab/__init__.py
+-rw-r--r--   0        0        0     7767 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/vcs/gitlab/gitlab_manager.py
+-rw-r--r--   0        0        0    12262 2024-05-03 12:23:17.052450 cgdevxcli-0.3.1/cli/services/wl_template_manager.py
+-rw-r--r--   0        0        0     1202 2024-05-03 12:23:34.916429 cgdevxcli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 cgdevxcli-0.3.1/PKG-INFO
```

### Comparing `cgdevxcli-0.3.0/README.md` & `cgdevxcli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/build.py` & `cgdevxcli-0.3.1/cli/build.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/commands/README.md` & `cgdevxcli-0.3.1/cli/commands/README.md`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/commands/destroy.py` & `cgdevxcli-0.3.1/cli/commands/destroy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import shutil
 import time
 
 import click
-import portforward
 import urllib3
 from git import InvalidGitRepositoryError
 
 from common.const.common_path import LOCAL_TF_FOLDER_VCS, LOCAL_TF_FOLDER_HOSTING_PROVIDER, LOCAL_FOLDER
 from common.const.namespaces import ARGOCD_NAMESPACE
-from common.const.parameter_names import GIT_ACCESS_TOKEN, GIT_ORGANIZATION_NAME
 from common.logging_config import configure_logging
 from common.state_store import StateStore
 from common.utils.command_utils import init_cloud_provider, prepare_cloud_provider_auth_env_vars, set_envs, unset_envs, \
     wait, init_git_provider, check_installation_presence, prepare_git_provider_env_vars
+from common.utils.k8s_utils import get_kr8s_pod_instance_by_name, find_pod_by_name_fragment
 from services.k8s.delivery_service_manager import DeliveryServiceManager, get_argocd_token, delete_application
 from services.k8s.k8s import KubeClient
 from services.platform_gitops import PlatformGitOpsRepo
 from services.tf_wrapper import TfWrapper
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -97,20 +96,26 @@
             # delete app
             cd_man.delete_app("ingress-nginx-components")
             cd_man.delete_app("ingress-nginx")
             cd_man.delete_app("github-runner-components")
             cd_man.delete_app("actions-runner-controller-components")
         except Exception as e:
             pass
-
         try:
-            with portforward.forward(ARGOCD_NAMESPACE, "argocd-server", 8080, 8080,
-                                     config_path=p.internals["KCTL_CONFIG_PATH"], waiting=3,
-                                     log_level=portforward.LogLevel.ERROR):
-
+            k8s_pod = find_pod_by_name_fragment(
+                kube_config_path=p.internals["KCTL_CONFIG_PATH"],
+                name_fragment="argocd-server",
+                namespace=ARGOCD_NAMESPACE
+            )
+            kr8s_pod = get_kr8s_pod_instance_by_name(
+                pod_name=k8s_pod.metadata.name,
+                namespace=ARGOCD_NAMESPACE,
+                kubeconfig=p.internals["KCTL_CONFIG_PATH"]
+            )
+            with kr8s_pod.portforward(remote_port=8080, local_port=8080):
                 argocd_token = get_argocd_token(p.internals["ARGOCD_USER"], p.internals["ARGOCD_PASSWORD"])
                 delete_application(registry_app_name, argocd_token)
 
             # need to wait here
             wait(300)
         except Exception as e:
             # suppress exception and continue without deleting ArgoCD app
```

### Comparing `cgdevxcli-0.3.0/cli/commands/setup.py` & `cgdevxcli-0.3.1/cli/commands/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import time
 import webbrowser
 
 import click
 import hvac
-import portforward
 import yaml
 from alive_progress import alive_bar
 
 from common.const.common_path import LOCAL_TF_FOLDER_VCS, LOCAL_TF_FOLDER_HOSTING_PROVIDER, \
     LOCAL_TF_FOLDER_SECRETS_MANAGER, LOCAL_TF_FOLDER_USERS, LOCAL_TF_FOLDER_CORE_SERVICES
 from common.const.const import GITOPS_REPOSITORY_URL, GITOPS_REPOSITORY_BRANCH, KUBECTL_VERSION, PLATFORM_USER_NAME, \
     TERRAFORM_VERSION, GITHUB_TF_REQUIRED_PROVIDER_VERSION, GITLAB_TF_REQUIRED_PROVIDER_VERSION
@@ -24,14 +23,15 @@
 from common.enums.git_providers import GitProviders
 from common.logging_config import configure_logging
 from common.state_store import StateStore
 from common.tracing_decorator import trace
 from common.utils.command_utils import init_cloud_provider, init_git_provider, prepare_cloud_provider_auth_env_vars, \
     set_envs, unset_envs, wait, wait_http_endpoint_readiness, prepare_git_provider_env_vars
 from common.utils.generators import random_string_generator
+from common.utils.k8s_utils import find_pod_by_name_fragment, get_kr8s_pod_instance_by_name
 from services.cloud.cloud_provider_manager import CloudProviderManager
 from services.dependency_manager import DependencyManager
 from services.dns.dns_provider_manager import DNSManager
 from services.k8s.config_builder import create_k8s_config, write_k8s_config
 from services.k8s.delivery_service_manager import DeliveryServiceManager, get_argocd_token
 from services.k8s.k8s import KubeClient, write_ca_cert
 from services.k8s.kctl_wrapper import KctlWrapper
@@ -256,14 +256,16 @@
         p.parameters["<K8S_ROLE_MAPPING>"] = cloud_man.create_k8s_cluster_role_mapping_snippet()
 
         p.fragments["# <ADDITIONAL_LABELS>"] = cloud_man.create_additional_labels()
         p.fragments["# <BASE_ADDITIONAL_ANNOTATIONS>"] = cloud_man.create_additional_labels()
         p.fragments["# <INGRESS_ANNOTATIONS>"] = cloud_man.create_ingress_annotations()
         p.fragments["# <SIDECAR_ANNOTATION>"] = cloud_man.create_sidecar_annotation()
 
+        p.fragments["# <KUBECOST_CLOUD_PROVIDER_CONFIGURATION>"] = cloud_man.create_kubecost_annotation()
+
         # dns zone info for external dns
         dns_zone_name, is_dns_zone_private = dns_man.get_domain_zone(p.parameters["<DOMAIN_NAME>"])
         p.internals["DNS_ZONE_NAME"] = dns_zone_name
         p.internals["DNS_ZONE_IS_PRIVATE"] = is_dns_zone_private
 
         p.fragments["# <EXTERNAL_DNS_ADDITIONAL_CONFIGURATION>"] = cloud_man.create_external_secrets_config(
             location=dns_zone_name, is_private=is_dns_zone_private)
@@ -552,21 +554,29 @@
 
             # argocd pods are ready, get and set credentials
             argo_pas = kube_client.get_secret(ARGOCD_NAMESPACE, "argocd-initial-admin-secret")
             p.internals["ARGOCD_USER"] = "admin"
             p.internals["ARGOCD_PASSWORD"] = argo_pas
 
             # get argocd auth token
-            with portforward.forward(ARGOCD_NAMESPACE, "argocd-server", 8080, 8080,
-                                     config_path=p.internals["KCTL_CONFIG_PATH"], waiting=3,
-                                     log_level=portforward.LogLevel.ERROR):
+            k8s_pod = find_pod_by_name_fragment(
+                kube_config_path=p.internals["KCTL_CONFIG_PATH"],
+                name_fragment="argocd-server",
+                namespace=ARGOCD_NAMESPACE
+            )
+            kr8s_pod = get_kr8s_pod_instance_by_name(
+                pod_name=k8s_pod.metadata.name,
+                namespace=ARGOCD_NAMESPACE,
+                kubeconfig=p.internals["KCTL_CONFIG_PATH"]
+            )
+            with kr8s_pod.portforward(remote_port=8080, local_port=8080):
+                # Make an API request to the forwarded port
                 argocd_token = get_argocd_token(p.internals["ARGOCD_USER"], p.internals["ARGOCD_PASSWORD"])
                 p.internals["ARGOCD_TOKEN"] = argocd_token
             bar()
-
             # create argocd "core" project
             # TODO: explicitly whitelist project repositories
             cd_man.create_project(argocd_core_project_name, [
                 p.parameters["<GIT_REPOSITORY_GIT_URL>"],
                 "https://charts.jetstack.io",
                 "https://kubernetes-sigs.github.io/external-dns",
                 "*"
```

### Comparing `cgdevxcli-0.3.0/cli/commands/workload/README.md` & `cgdevxcli-0.3.1/cli/commands/workload/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,26 +111,27 @@
 comments section.
 
 `workload delete` command deletes all the configuration generated by `workload create` [command](#create):
 
 When executed with `--destroy-resources` flag it will also destroy all the resources created for a specific workload.
 Please note that workload GitOps repository name should match one for workload.
 When executing with `--destroy-resources` flag enabled it **must** be executed by cluster owner.
-Under the hood, it will execute tf destroy locally, and tf state storage is protected and accessible only by the owner. 
+Under the hood, it will execute tf destroy locally, and tf state storage is protected and accessible only by the owner.
 
 
 > **NOTE!**: this process is irreversible
 
 `workload delete` command could be executed using arguments, or environment variables.
 
 **Arguments**:
 
 | Name (short, full)                        | Type                                    | Description                                       |
 |-------------------------------------------|-----------------------------------------|---------------------------------------------------|
-| -wl, --workload-name                      | TEXT                                    | Workload name                                     |
+| -wl, --workload-names                     | TEXT                                    | Workload name(s), could be multiple args          |
+| --all                                     | Flag                                    | Destroy all existing workloads                    |
 | -wldr, --destroy-resources                | Flag                                    | Destroy workload resources                        |
 | -wlgrn, --workload-gitops-repository-name | TEXT                                    | Name for Workload GitOps repository               |
 | --verbosity                               | [DEBUG, INFO, WARNING, ERROR, CRITICAL] | Set the logging verbosity level, default CRITICAL |
 
 > **Note!**: For all names use kebab-case.
 
 **Command snippet**
```

### Comparing `cgdevxcli-0.3.0/cli/commands/workload/bootstrap.py` & `cgdevxcli-0.3.1/cli/commands/workload/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,16 @@
         git_organisation_name = state_store.parameters["<GIT_ORGANIZATION_NAME>"]
         cluster_name = state_store.parameters["<PRIMARY_CLUSTER_NAME>"]
         cloud_account = state_store.internals["CLOUD_ACCOUNT"]
         domain_name = state_store.parameters["<DOMAIN_NAME>"]
         cloud_region = state_store.parameters["<CLOUD_REGION>"]
         owner_email = state_store.parameters["<OWNER_EMAIL>"]
         ci_iam_role_rn = state_store.parameters["<CI_IAM_ROLE_RN>"]
+        artifact_store = state_store.parameters["<CLOUD_BINARY_ARTIFACTS_STORE>"]
+        ci_ingress_url = state_store.parameters["<CI_INGRESS_URL>"]
 
 
         click.echo("1/11: Configuration loaded.")
     except KeyError as e:
         error_message = f'Configuration loading failed due to missing key: {e}. ' \
                         'Please verify the state store configuration and ensure all required keys are present. ' \
                         'Review the documentation for the necessary configuration keys and try again.'
@@ -175,14 +177,15 @@
         "<REGISTRY_GCR_PROXY>": gcr_proxy,
         "<REGISTRY_K8S_GCR_PROXY>": k8s_gcr_proxy,
         "<REGISTRY_QUAY_PROXY>": quay_proxy,
         "<WL_REPO_NAME>": wl_repo_name,
         "<WL_GITOPS_REPO_NAME>": wl_gitops_repo_name,
         "<GIT_ORGANIZATION_NAME>": git_organisation_name,
         "<GIT_RUNNER_GROUP_NAME>": git_runner_group_name,
+        "<CI_INGRESS_URL>": ci_ingress_url,
     }
 
     wl_gitops_params = {
         "<WL_NAME>": wl_name,
         "<WL_SERVICE_NAME>": wl_svc_name,
         "<WL_SERVICE_URL>": f'{wl_svc_name}.{wl_name}.{cc_cluster_fqdn}',
         "<WL_SERVICE_IMAGE>": f'{registry_url}/{wl_name}/{wl_svc_name}',
@@ -210,15 +213,16 @@
         "<CLOUD_REGION>": cloud_region,
         "<OWNER_EMAIL>": owner_email,
         "<REGISTRY_URL>": registry_url,
         "<CI_IAM_ROLE_RN>": ci_iam_role_rn,
         "<CLOUD_ACCOUNT>": cloud_account,
         "<WL_IAM_ROLE_RN>": construct_wl_iam_role(
             state_store.cloud_provider, cloud_account, cluster_name, wl_name, wl_svc_name
-        )
+        ),
+      "<CLOUD_BINARY_ARTIFACTS_STORE>": artifact_store
     }
 
     # set cloud provider specific params
     cloud_provider = state_store.parameters["<CLOUD_PROVIDER>"]
     if cloud_provider == CloudProviders.AWS:
         wl_gitops_params["<CLUSTER_OIDC_PROVIDER_ARN>"] = state_store.parameters["<CC_CLUSTER_OIDC_PROVIDER>"]
     elif cloud_provider == CloudProviders.Azure:
```

### Comparing `cgdevxcli-0.3.0/cli/commands/workload/create.py` & `cgdevxcli-0.3.1/cli/commands/workload/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import click
 from git import InvalidGitRepositoryError
 
 from common.const.const import GITOPS_REPOSITORY_MAIN_BRANCH, WL_PR_BRANCH_NAME_PREFIX
 from common.custom_excpetions import GitBranchAlreadyExists, PullRequestCreationError
 from common.logging_config import configure_logging, logger
 from common.state_store import StateStore
-from common.utils.command_utils import str_to_kebab, check_installation_presence, \
+from common.utils.command_utils import check_installation_presence, \
     initialize_gitops_repository, create_and_setup_branch, create_and_open_pull_request, preprocess_workload_names
 from services.platform_gitops import PlatformGitOpsRepo
 
 
 @click.command()
 @click.option('--workload-name', '-wl', 'wl_name', help='Workload name', type=click.STRING, prompt=True)
 @click.option(
```

### Comparing `cgdevxcli-0.3.0/cli/commands/workload/delete.py` & `cgdevxcli-0.3.1/cli/commands/workload/delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 import os
 import shutil
 import time
+from datetime import datetime
+from typing import List
 
 import click
 from git import InvalidGitRepositoryError
 
 from common.const.common_path import LOCAL_WORKLOAD_TEMP_FOLDER
-from common.const.const import GITOPS_REPOSITORY_MAIN_BRANCH, WL_PR_BRANCH_NAME_PREFIX, WL_GITOPS_REPOSITORY_BRANCH, \
-    WL_GITOPS_REPOSITORY_URL
+from common.const.const import GITOPS_REPOSITORY_MAIN_BRANCH, WL_PR_BRANCH_NAME_PREFIX
 from common.const.parameter_names import GIT_ACCESS_TOKEN, GIT_ORGANIZATION_NAME
 from common.custom_excpetions import GitBranchAlreadyExists, PullRequestCreationError
 from common.logging_config import configure_logging, logger
 from common.state_store import StateStore
-from common.utils.command_utils import str_to_kebab, prepare_cloud_provider_auth_env_vars, set_envs, \
-    check_installation_presence, initialize_gitops_repository, create_and_setup_branch, \
-    create_and_open_pull_request, preprocess_workload_names
+from common.utils.command_utils import prepare_cloud_provider_auth_env_vars, set_envs, \
+  check_installation_presence, initialize_gitops_repository, create_and_setup_branch, \
+  create_and_open_pull_request, preprocess_workload_names
 from services.platform_gitops import PlatformGitOpsRepo
 from services.tf_wrapper import TfWrapper
 from services.wl_template_manager import WorkloadManager
 
 
 @click.command()
-@click.option('--workload-name', '-wl', 'wl_name', help='Workload name', type=click.STRING, prompt=True)
+@click.option(
+    '--workload-names',
+    '-wl',
+    'wl_names',
+    help='Workload names',
+    type=click.STRING,
+    multiple=True
+)
+@click.option(
+    '--all',
+    'delete_all',
+    is_flag=True,
+    help='Delete all workloads',
+    default=False
+)
 @click.option(
     '--workload-gitops-repository-name',
     '-wlgrn',
     'wl_gitops_repo_name',
     help='Workload GitOps repository name',
     type=click.STRING
 )
@@ -34,149 +49,151 @@
     '-wldr',
     'destroy_resources',
     help='Destroy workload resources',
     is_flag=True,
     default=False
 )
 @click.option(
-    '--workload-gitops-template-url',
-    '-wlgu',
-    'wl_gitops_template_url',
-    help='Workload GitOps repository template',
-    type=click.STRING,
-    default=WL_GITOPS_REPOSITORY_URL
-)
-@click.option(
-    '--workload-gitops-template-branch',
-    '-wlgb',
-    'wl_gitops_template_branch',
-    help='Workload GitOps repository template branch',
-    type=click.STRING,
-    default=WL_GITOPS_REPOSITORY_BRANCH
-)
-@click.option(
     '--verbosity',
     type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'], case_sensitive=False),
     default='CRITICAL',
     help='Set the verbosity level (DEBUG, INFO, WARNING, ERROR, CRITICAL)'
 )
 def delete(
-        wl_name: str, wl_gitops_repo_name: str, destroy_resources: bool, wl_gitops_template_url: str,
-        wl_gitops_template_branch: str, verbosity: str
+        wl_names: List[str],
+        delete_all: bool,
+        wl_gitops_repo_name: str,
+        destroy_resources: bool,
+        verbosity: str
 ):
     """
     Deletes all the workload boilerplate, including optionally destroying associated resources.
 
     This command performs a series of steps to remove a workload and its configurations from the GitOps repository.
     It optionally destroys the resources defined in the workload's Infrastructure as Code (IaC).
 
     Args:
-        wl_name (str): Name of the workload to be deleted.
+        wl_names (List[str]): Names of the workloads to be deleted. Ignored if delete_all is True
+        delete_all (bool): If set to True, all workloads will be deleted, ignoring wl_names.
         wl_gitops_repo_name (str): Name of the GitOps repository associated with the workload.
         destroy_resources (bool): Flag indicating whether to destroy resources defined in the workload's IaC.
-        wl_gitops_template_url (str): URL of the GitOps repository template.
-        wl_gitops_template_branch (str): Branch of the GitOps repository template.
-        main_branch (str): Main branch name of the GitOps repository.
         verbosity (str): Logging level.
 
     Raises:
         click.ClickException: If any error occurs during the deletion process.
     """
-    click.confirm(f'This will delete the workload "{wl_name}". Please confirm to continue', abort=True)
+    # Set up global logger
+    configure_logging(verbosity=verbosity)
+
+    state_store: StateStore = StateStore()
+
+    try:
+        git_man, gor = initialize_gitops_repository(state_store=state_store, logger=logger)
+    except InvalidGitRepositoryError:
+        raise click.ClickException("GitOps repo does not exist")
+    click.echo(f"GitOps repository initialized.")
+
+    if delete_all:
+        wl_names = gor.list_workloads()
+    if len(wl_names) == 0:
+        raise click.ClickException("There are no workloads to be deleted")
+
+    click.confirm(f"This will delete the workloads \"{', '.join(wl_names)}\". Please confirm to continue", abort=True)
     destroy_resources = destroy_resources and click.confirm(
-        "This will delete all the resources defined in workload IaC. Please confirm to continue"
+        "This will delete all the resources defined in workloads IaC. Please confirm to continue"
     )
+
     # Determine the total number of steps
-    logging_total_steps = 7 if destroy_resources else 6
+    logging_total_steps = 6 if destroy_resources else 5
     func_start_time = time.time()
 
-    branch_name = f"{WL_PR_BRANCH_NAME_PREFIX}{wl_name}-destroy"
+    branch_name = _generate_destroy_branch_name()
     click.echo("Initializing workload deletion process...")
-    state_store: StateStore = StateStore()
+
     click.echo(f"1/{logging_total_steps}: State store initialized.")
 
-    # Set up global logger
-    configure_logging(verbosity=verbosity)
     check_installation_presence()
     click.echo(f"2/{logging_total_steps}: Logging and installation checked.")
 
-    wl_name, wl_repo_name, wl_gitops_repo_name = preprocess_workload_names(
-        logger=logger,
-        wl_name=wl_name,
-        wl_gitops_repo_name=wl_gitops_repo_name,
-    )
-    click.echo(f"3/{logging_total_steps}: Workload names processed.")
-    try:
-        git_man, gor = initialize_gitops_repository(state_store=state_store, logger=logger)
-    except InvalidGitRepositoryError:
-        raise click.ClickException("GitOps repo does not exist")
-    click.echo(f"4/{logging_total_steps}: GitOps repository initialized.")
-
     try:
         create_and_setup_branch(gor=gor, branch_name=branch_name, logger=logger)
     except GitBranchAlreadyExists as e:
         raise click.ClickException(str(e))
 
-    # Optionally destroy resources
-    if destroy_resources:
-        # to destroy workload resources, we need to clone workload gitops repo
-        # and call tf destroy while pointing to remote state
-        wl_gitops_manager = WorkloadManager(
-            org_name=state_store.parameters["<GIT_ORGANIZATION_NAME>"],
-            repo_name=wl_gitops_repo_name,
-            key_path=state_store.internals["DEFAULT_SSH_PRIVATE_KEY_PATH"],
-            template_url=wl_gitops_template_url,
-            template_branch=wl_gitops_template_branch
+    for index, wl_name in enumerate(wl_names):
+        wl_name, wl_repo_name, wl_gitops_repo_name = preprocess_workload_names(
+            logger=logger,
+            wl_name=wl_name,
+            wl_gitops_repo_name=wl_gitops_repo_name,
         )
+        click.echo(f"3.{index}/{logging_total_steps}: Workload names processed.")
 
-        wl_gitops_repo_folder = wl_gitops_manager.clone_wl()
-
-        _set_tf_env_vars_for_tf(state_store=state_store)
-
-        destroy_all_tf_resources(repo_folder=wl_gitops_repo_folder)
-
-        # remove temp folder
-        shutil.rmtree(LOCAL_WORKLOAD_TEMP_FOLDER)
-
-        click.echo(f"5/{logging_total_steps}: Workload resources destroyed.")
+        # Optionally destroy resources
+        if destroy_resources:
+            # to destroy workload resources, we need to clone workload gitops repo
+            # and call tf destroy while pointing to remote state
+            wl_gitops_manager = WorkloadManager(
+                org_name=state_store.parameters["<GIT_ORGANIZATION_NAME>"],
+                repo_name=wl_gitops_repo_name,
+                key_path=state_store.internals["DEFAULT_SSH_PRIVATE_KEY_PATH"]
+            )
+
+            wl_gitops_repo_folder = wl_gitops_manager.clone_wl()
+
+            _set_tf_env_vars_for_tf(state_store=state_store)
+
+            destroy_all_tf_resources(repo_folder=wl_gitops_repo_folder)
+
+            # remove temp folder
+            shutil.rmtree(LOCAL_WORKLOAD_TEMP_FOLDER)
+
+            click.echo(f"4.{index}/{logging_total_steps}: Workload \"{wl_name}\" resources destroyed.")
+
+        commit_message = f"Remove secrets, groups, repository structure for workload \"{wl_name}\""
+        _remove_workload_and_commit(wl_name=wl_name, gor=gor, commit_message=commit_message)
+        click.echo(
+            f"{5 if destroy_resources else 4}.{index}/{logging_total_steps}: "
+            f"Workload \"{wl_name}\" removed and changes committed."
+        )
 
-    _remove_workload_and_commit(wl_name=wl_name, gor=gor)
-    click.echo(f"{6 if destroy_resources else 5}/{logging_total_steps}: Workload removed and changes committed.")
     try:
         create_and_open_pull_request(
             gor=gor,
             state_store=state_store,
-            title=f"Remove {wl_name}",
+            title=f"Remove {wl_names}",
             body="Remove default secrets, groups and repository structure.",
             branch_name=branch_name,
             main_branch=GITOPS_REPOSITORY_MAIN_BRANCH,
             logger=logger
         )
     except PullRequestCreationError as e:
         raise click.ClickException(str(e))
 
-    click.echo(f"{7 if destroy_resources else 6}/{logging_total_steps}: Pull request created and opened.")
+    click.echo(f"{6 if destroy_resources else 5}/{logging_total_steps}: Pull request created and opened.")
 
     gor.switch_to_branch()
     gor.delete_branch(branch_name)
 
-    click.echo(f"Deleting workload GitOps code completed in {time.time() - func_start_time:.2f} seconds.")
+    click.echo(f"Deleting workloads GitOps code completed in {time.time() - func_start_time:.2f} seconds.")
 
 
-def _remove_workload_and_commit(gor: PlatformGitOpsRepo, wl_name: str) -> None:
+def _remove_workload_and_commit(gor: PlatformGitOpsRepo, wl_name: str, commit_message: str) -> None:
     """
-    Remove the workload to the GitOps repository and commit changes.
+    Remove the workload from the GitOps repository and commit the changes.
 
     Parameters:
-        gor: PlatformGitOpsRepo class instance.
-        wl_name (str): Name of the workload.
+        gor (PlatformGitOpsRepo): An instance of the PlatformGitOpsRepo class.
+        wl_name (str): The name of the workload to be removed.
+        commit_message (str): The commit message to be used when committing the changes to the repository.
+
+    The function removes the specified workload and commits the changes with the provided commit message.
     """
     gor.rm_workload(wl_name=wl_name)
-    gor.upload_changes()
-    logger.info("Workload added and committed to the repository.")
+    gor.upload_changes(commit_message)
+    logger.info(f"Workload removed and committed to the repository with message: {commit_message}")
 
 
 def _set_tf_env_vars_for_tf(state_store: StateStore) -> None:
     """
     Set environment variables required for Terraform operations.
 
     Args:
@@ -222,7 +239,33 @@
         tf_directory=os.path.join(repo_folder, "terraform", "secrets"),
         resource_description="WL secrets"
     )
     _destroy_tf_resources(
         tf_directory=os.path.join(repo_folder, "terraform", "infrastructure"),
         resource_description="WL cloud resources"
     )
+
+
+def _generate_destroy_branch_name(
+        git_folder_prefix: str = WL_PR_BRANCH_NAME_PREFIX, wl_destroy_prefix: str = "workload_destroy_"
+) -> str:
+    """
+    Generate a unique branch name for destroying workloads, incorporating the current date and time.
+
+    Parameters:
+        git_folder_prefix (str): The prefix to use for the branch name, which is related to the git folder, defaulting
+        to WL_PR_BRANCH_NAME_PREFIX.
+        wl_destroy_prefix (str): The prefix to add before "destroy" and the timestamp, defaulting to "workload_destroy_"
+
+    Returns:
+        str: The generated branch name, which concatenates the git folder prefix, workload destroy prefix,
+        and the current date and time.
+
+    This function constructs a branch name intended to be unique and descriptive, facilitating the identification of
+    the branch's purpose and the time of its creation.
+    """
+    current_time = datetime.now().strftime("%Y%m%d_%H%M%S")
+    branch_name = f"{git_folder_prefix}{wl_destroy_prefix}{current_time}"
+
+    logger.info(f"Generated branch name: {branch_name}")
+
+    return branch_name
```

### Comparing `cgdevxcli-0.3.0/cli/common/const/common_path.py` & `cgdevxcli-0.3.1/cli/common/const/common_path.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/const/const.py` & `cgdevxcli-0.3.1/cli/common/const/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 STATE_PARAMS = "params"
 STATE_FRAGMENTS = "fragments"
 STATE_CHECKPOINTS = "checkpoints"
 FALLBACK_AUTHOR_NAME = "cgdevx-bot"
 PLATFORM_USER_NAME = "cgdevx-bot"
 FALLBACK_AUTHOR_EMAIL = "cg-devx-automation@cloudgeometry.io"
 ARGOCD_REGISTRY_APP_PATH = "gitops-pipelines/delivery/clusters/cc-cluster/core-services"
-KUBECTL_VERSION = "1.27.4"
+KUBECTL_VERSION = "1.29.4"
 TERRAFORM_VERSION = "1.6.4"
 GITLAB_TF_REQUIRED_PROVIDER_VERSION = "16.7.0"
 GITHUB_TF_REQUIRED_PROVIDER_VERSION = "5.42.0"
 GITOPS_REPOSITORY_MAIN_BRANCH = "main"
 WL_REPOSITORY_URL = "git@github.com:CloudGeometry/cg-devx-wl-template.git"
 WL_REPOSITORY_BRANCH = "main"
 WL_PR_BRANCH_NAME_PREFIX = "feature/"
```

### Comparing `cgdevxcli-0.3.0/cli/common/const/parameter_names.py` & `cgdevxcli-0.3.1/cli/common/const/parameter_names.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/custom_excpetions.py` & `cgdevxcli-0.3.1/cli/common/custom_excpetions.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/enums/cloud_providers.py` & `cgdevxcli-0.3.1/cli/common/enums/cloud_providers.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/enums/dns_registrars.py` & `cgdevxcli-0.3.1/cli/common/enums/dns_registrars.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/enums/git_providers.py` & `cgdevxcli-0.3.1/cli/common/enums/git_providers.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/logging_config.py` & `cgdevxcli-0.3.1/cli/common/logging_config.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/retry_decorator.py` & `cgdevxcli-0.3.1/cli/common/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/state_store.py` & `cgdevxcli-0.3.1/cli/common/state_store.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/tracing_decorator.py` & `cgdevxcli-0.3.1/cli/common/tracing_decorator.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/common/utils/command_utils.py` & `cgdevxcli-0.3.1/cli/common/utils/command_utils.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/README.md` & `cgdevxcli-0.3.1/cli/services/README.md`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/aws/aws_manager.py` & `cgdevxcli-0.3.1/cli/services/cloud/aws/aws_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,7 +180,11 @@
     def create_iac_pr_automation_config_snippet(self):
         return '''# aws specific section
       # ----'''
 
     @trace()
     def create_autoscaler_snippet(self, cluster_name: str, node_groups=[]):
         return '''awsRegion: <CLOUD_REGION>'''
+
+    @trace()
+    def create_kubecost_annotation(self):
+        return '''amazon-web-services: true'''
```

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/aws/aws_sdk.py` & `cgdevxcli-0.3.1/cli/services/cloud/aws/aws_sdk.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/aws/aws_session_manager.py` & `cgdevxcli-0.3.1/cli/services/cloud/aws/aws_session_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/aws/iam_permissions.py` & `cgdevxcli-0.3.1/cli/services/cloud/aws/iam_permissions.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/azure/azure_manager.py` & `cgdevxcli-0.3.1/cli/services/cloud/azure/azure_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,7 +273,11 @@
         return '''# azure specific section
       ARM_USE_AKS_WORKLOAD_IDENTITY       = true,
       ARM_USE_CLI                         = false,
       ARM_SUBSCRIPTION_ID                 = "<AZ_SUBSCRIPTION_ID>",
       ARM_CLIENT_ID                       = "<IAC_PR_AUTOMATION_IAM_ROLE_RN>",
       ARM_ACCESS_KEY                      = var.tf_backend_storage_access_key,
       # ----'''
+
+    @trace()
+    def create_kubecost_annotation(self):
+        return '''azure-cloud-services: true'''
```

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/azure/azure_sdk.py` & `cgdevxcli-0.3.1/cli/services/cloud/azure/azure_sdk.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/azure/iam_permissions.py` & `cgdevxcli-0.3.1/cli/services/cloud/azure/iam_permissions.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/cloud/cloud_provider_manager.py` & `cgdevxcli-0.3.1/cli/services/cloud/cloud_provider_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,7 +159,15 @@
     @abstractmethod
     def create_iac_pr_automation_config_snippet(self):
         """
         Creates Cloud Provider specific configuration section for Atlantis
         :return: Atlantis configuration section
         """
         pass
+
+    @abstractmethod
+    def create_kubecost_annotation(self):
+        """
+        Creates Cloud Provider specific configuration section for KubeCost
+        :return: KubeCost configuration section
+        """
+        pass
```

### Comparing `cgdevxcli-0.3.0/cli/services/dependency_manager.py` & `cgdevxcli-0.3.1/cli/services/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/dns/azure_dns/azure_dns.py` & `cgdevxcli-0.3.1/cli/services/dns/azure_dns/azure_dns.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/dns/dns_provider_manager.py` & `cgdevxcli-0.3.1/cli/services/dns/dns_provider_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/dns/route53/route53.py` & `cgdevxcli-0.3.1/cli/services/dns/route53/route53.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/k8s/config_builder.py` & `cgdevxcli-0.3.1/cli/services/k8s/config_builder.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/k8s/delivery_service_manager.py` & `cgdevxcli-0.3.1/cli/services/k8s/delivery_service_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/k8s/k8s.py` & `cgdevxcli-0.3.1/cli/services/k8s/k8s.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/k8s/kctl_wrapper.py` & `cgdevxcli-0.3.1/cli/services/k8s/kctl_wrapper.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/keys/key_manager.py` & `cgdevxcli-0.3.1/cli/services/keys/key_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/platform_gitops.py` & `cgdevxcli-0.3.1/cli/services/platform_gitops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import shutil
-from typing import Optional
+from typing import Optional, List
 
 from ghrepo import GHRepo
 from git import InvalidGitRepositoryError, Repo, Actor, NoSuchPathError
 
 from common.const.common_path import LOCAL_GITOPS_FOLDER, LOCAL_TF_FOLDER_VCS, LOCAL_TF_FOLDER_SECRETS_MANAGER, \
     LOCAL_TF_FOLDER_CORE_SERVICES, LOCAL_CC_CLUSTER_WORKLOAD_FOLDER, LOCAL_TF_FOLDER_HOSTING_PROVIDER
 from common.const.const import FALLBACK_AUTHOR_NAME, FALLBACK_AUTHOR_EMAIL
@@ -91,22 +91,22 @@
 
         :param branch_name: Branch name
         """
         current = self._repo.create_head(branch_name)
         current.checkout()
 
     @trace()
-    def upload_changes(self):
+    def upload_changes(self, message: Optional[str] = "initial") -> None:
         """
         Commit all the changes to an active branch
         """
         with self._repo.git.custom_environment(GIT_SSH_COMMAND=self._ssh_cmd):
             self._repo.git.add(all=True)
             author = Actor(name=self._author_name, email=self._author_email)
-            self._repo.index.commit("initial", author=author, committer=author)
+            self._repo.index.commit(message, author=author, committer=author)
 
             self._repo.remotes.origin.push(self._repo.active_branch.name)
 
     @trace()
     def switch_to_branch(self, branch_name: str = "main"):
         """
         Switch to an existing branch in the platform GitOps repository
@@ -234,7 +234,25 @@
             vcs_tf_vars = json.load(file)
 
         if wl_name in vcs_tf_vars["workloads"]:
             del vcs_tf_vars["workloads"][wl_name]
 
             with open(tf_module_path / "terraform.tfvars.json", "w") as file:
                 file.write(json.dumps(vcs_tf_vars, indent=2))
+
+    @staticmethod
+    @trace()
+    def list_workloads() -> List[str]:
+        """
+        List all workloads defined in the platform GitOps repository.
+
+        :return: A list of workload names.
+        """
+        try:
+            with open(os.path.join(LOCAL_TF_FOLDER_VCS, "terraform.tfvars.json"), "r") as file:
+                tf_vars = json.load(file)
+            workloads = tf_vars.get("workloads", {}).keys()
+            logger.info(f"Found {len(workloads)} workloads: {list(workloads)}")
+            return list(workloads)
+        except FileNotFoundError:
+            logger.error(f"Could not find the Terraform variables file at {LOCAL_TF_FOLDER_VCS}")
+            return []
```

### Comparing `cgdevxcli-0.3.0/cli/services/platform_template_manager.py` & `cgdevxcli-0.3.1/cli/services/platform_template_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/tf_wrapper.py` & `cgdevxcli-0.3.1/cli/services/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/vcs/git_provider_manager.py` & `cgdevxcli-0.3.1/cli/services/vcs/git_provider_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/vcs/github/github_manager.py` & `cgdevxcli-0.3.1/cli/services/vcs/github/github_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/vcs/gitlab/gitlab_manager.py` & `cgdevxcli-0.3.1/cli/services/vcs/gitlab/gitlab_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/cli/services/wl_template_manager.py` & `cgdevxcli-0.3.1/cli/services/wl_template_manager.py`

 * *Files identical despite different names*

### Comparing `cgdevxcli-0.3.0/pyproject.toml` & `cgdevxcli-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "cgdevxcli"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Alexander Ulyanov <alexu@cloudgeometry.io>", "Mikhail Turetskii <mturetsky@cloudgeometry.io>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.scripts]
 cgdevxcli = "cli.__main__:entry_point"
 build = "cli.build:install"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.13"
 click = "8.1.7"
 cloup = "3.0.2"
 PyInstaller = "5.13.2"
 awscli = "1.29.56"
 boto3 = "1.28.56"
 configparser = "6.0.0"
 pyyaml = "6.0.1"
@@ -30,22 +30,20 @@
 azure-mgmt-storage = "^21.1.0"
 azure-mgmt-subscription = "^3.1.1"
 azure-mgmt-compute = "^30.5.0"
 gcloud = "0.18.3"
 gitpython = "3.1.32"
 ghrepo = "0.7.0"
 dnspython = "2.4.2"
-httpx = "0.25.0"
 hvac = "1.2.1"
-portforward = "^0.6.0"
 alive-progress = "^3.1.5"
+kr8s = "^0.14.2"
 
 [tool.poetry.dev-dependencies]
 flake8 = "6.1.0"
 flake8-class-attributes-order = "0.1.3"
 flake8-docstrings = "1.7.0"
 pydocstyle = "6.3.0"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cgdevxcli-0.3.0/PKG-INFO` & `cgdevxcli-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: cgdevxcli
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Alexander Ulyanov
 Author-email: alexu@cloudgeometry.io
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyInstaller (==5.13.2)
 Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
 Requires-Dist: awscli (==1.29.56)
 Requires-Dist: azure-identity (==1.14.0)
 Requires-Dist: azure-mgmt-authorization (>=4.0.0,<5.0.0)
 Requires-Dist: azure-mgmt-compute (>=30.5.0,<31.0.0)
 Requires-Dist: azure-mgmt-containerservice (>=26.0.0,<27.0.0)
@@ -24,18 +26,17 @@
 Requires-Dist: click (==8.1.7)
 Requires-Dist: cloup (==3.0.2)
 Requires-Dist: configparser (==6.0.0)
 Requires-Dist: dnspython (==2.4.2)
 Requires-Dist: gcloud (==0.18.3)
 Requires-Dist: ghrepo (==0.7.0)
 Requires-Dist: gitpython (==3.1.32)
-Requires-Dist: httpx (==0.25.0)
 Requires-Dist: hvac (==1.2.1)
+Requires-Dist: kr8s (>=0.14.2,<0.15.0)
 Requires-Dist: kubernetes (==27.2.0)
-Requires-Dist: portforward (>=0.6.0,<0.7.0)
 Requires-Dist: pyyaml (==6.0.1)
 Description-Content-Type: text/markdown
 
 # CG DevX CLI
 
 CG DevX CLI simplifies initial setup of CG DevX reference architecture.
 The setup process is intended to be executed from an operator's machine and will create a local folder containing tools,
```

