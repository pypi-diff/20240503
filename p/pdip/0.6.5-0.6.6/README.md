# Comparing `tmp/pdip-0.6.5.tar.gz` & `tmp/pdip-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdip-0.6.5.tar", last modified: Sat Mar 11 21:23:32 2023, max compression
+gzip compressed data, was "pdip-0.6.6.tar", last modified: Mon Mar 13 00:46:29 2023, max compression
```

## Comparing `pdip-0.6.5.tar` & `pdip-0.6.6.tar`

### file list

```diff
@@ -1,568 +1,568 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.949189 pdip-0.6.5/
--rw-rw-rw-   0        0        0     1097 2021-12-24 11:05:16.000000 pdip-0.6.5/LICENSE
--rw-rw-rw-   0        0        0     1330 2023-03-11 21:23:32.950188 pdip-0.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.282780 pdip-0.6.5/pdip/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.441783 pdip-0.6.5/pdip/api/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.498370 pdip-0.6.5/pdip/api/app/
--rw-rw-rw-   0        0        0       48 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/app/__init__.py
--rw-rw-rw-   0        0        0     1941 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/app/flask_app_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.667785 pdip-0.6.5/pdip/api/base/
--rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/base/__init__.py
--rw-rw-rw-   0        0        0     3736 2023-03-11 21:16:51.000000 pdip-0.6.5/pdip/api/base/controller_base.py
--rw-rw-rw-   0        0        0     4506 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/base/endpoint_base.py
--rw-rw-rw-   0        0        0     8789 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/api/base/endpoint_wrapper.py
--rw-rw-rw-   0        0        0      172 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/base/resource_base.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.783784 pdip-0.6.5/pdip/api/converter/
--rw-rw-rw-   0        0        0       49 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/converter/__init__.py
--rw-rw-rw-   0        0        0     3284 2022-01-17 05:17:17.000000 pdip-0.6.5/pdip/api/converter/request_converter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.829784 pdip-0.6.5/pdip/api/decorators/
--rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/decorators/__init__.py
--rw-rw-rw-   0        0        0      240 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/decorators/controller_base.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.884784 pdip-0.6.5/pdip/api/handlers/
--rw-rw-rw-   0        0        0       88 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/handlers/__init__.py
--rw-rw-rw-   0        0        0     3755 2022-01-23 16:31:36.000000 pdip-0.6.5/pdip/api/handlers/error_handlers.py
--rw-rw-rw-   0        0        0     1515 2022-02-13 20:47:19.000000 pdip-0.6.5/pdip/api/handlers/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.949782 pdip-0.6.5/pdip/api/request_parameter/
--rw-rw-rw-   0        0        0       97 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/request_parameter/__init__.py
--rw-rw-rw-   0        0        0      124 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/request_parameter/order_by_parameter.py
--rw-rw-rw-   0        0        0      129 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/request_parameter/paging_parameter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.044783 pdip-0.6.5/pdip/api/specifications/
--rw-rw-rw-   0        0        0      113 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/api/specifications/__init__.py
--rw-rw-rw-   0        0        0     1492 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/specifications/order_by_specification.py
--rw-rw-rw-   0        0        0     1252 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/api/specifications/paging_specification.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.106786 pdip-0.6.5/pdip/base/
--rw-rw-rw-   0        0        0       22 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/base/__init__.py
--rw-rw-rw-   0        0        0     1677 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/base/pdi.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.164784 pdip-0.6.5/pdip/configuration/
--rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/__init__.py
--rw-rw-rw-   0        0        0     5060 2023-03-04 01:10:13.000000 pdip-0.6.5/pdip/configuration/config_manager.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.228785 pdip-0.6.5/pdip/configuration/models/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.418784 pdip-0.6.5/pdip/configuration/models/api/
--rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/api/__init__.py
--rw-rw-rw-   0        0        0      334 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/api/api_config.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.557905 pdip-0.6.5/pdip/configuration/models/application/
--rw-rw-rw-   0        0        0       51 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/application/__init__.py
--rw-rw-rw-   0        0        0      271 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/application/application_config.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.645786 pdip-0.6.5/pdip/configuration/models/aps/
--rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/aps/__init__.py
--rw-rw-rw-   0        0        0      380 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/aps/aps_config.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.734786 pdip-0.6.5/pdip/configuration/models/base/
--rw-rw-rw-   0        0        0      236 2023-03-04 00:45:05.000000 pdip-0.6.5/pdip/configuration/models/base/__init__.py
--rw-rw-rw-   0        0        0       87 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/base/base_config.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.800785 pdip-0.6.5/pdip/configuration/models/database/
--rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/database/__init__.py
--rw-rw-rw-   0        0        0      450 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/models/database/database_config.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:24.889784 pdip-0.6.5/pdip/configuration/services/
--rw-rw-rw-   0        0        0       99 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/services/__init__.py
--rw-rw-rw-   0        0        0      482 2022-01-04 10:22:25.000000 pdip-0.6.5/pdip/configuration/services/config_parameter_base.py
--rw-rw-rw-   0        0        0     1051 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/configuration/services/config_service.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.114787 pdip-0.6.5/pdip/cqrs/
--rw-rw-rw-   0        0        0      301 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/__init__.py
--rw-rw-rw-   0        0        0      162 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/command_query_base.py
--rw-rw-rw-   0        0        0      331 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/command_query_handler_base.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.255786 pdip-0.6.5/pdip/cqrs/decorators/
--rw-rw-rw-   0        0        0      117 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/decorators/__init__.py
--rw-rw-rw-   0        0        0      861 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/decorators/cls_to_dict.py
--rw-rw-rw-   0        0        0      277 2023-03-11 19:32:52.000000 pdip-0.6.5/pdip/cqrs/decorators/dto_class.py
--rw-rw-rw-   0        0        0      281 2023-03-11 19:32:52.000000 pdip-0.6.5/pdip/cqrs/decorators/request_class.py
--rw-rw-rw-   0        0        0      282 2023-03-11 19:32:52.000000 pdip-0.6.5/pdip/cqrs/decorators/response_class.py
--rw-rw-rw-   0        0        0     1586 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/cqrs/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.313791 pdip-0.6.5/pdip/cqrs/generator/
--rw-rw-rw-   0        0        0       66 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.515786 pdip-0.6.5/pdip/cqrs/generator/domain/
--rw-rw-rw-   0        0        0      187 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/domain/__init__.py
--rw-rw-rw-   0        0        0      126 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/domain/dao_generate_config.py
--rw-rw-rw-   0        0        0      241 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/domain/generate_config.py
--rw-rw-rw-   0        0        0      167 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/domain/generator.py
--rw-rw-rw-   0        0        0      198 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/domain/query_generate_config.py
--rw-rw-rw-   0        0        0    12142 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/generator/query_generator.py
--rw-rw-rw-   0        0        0      223 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/icommand.py
--rw-rw-rw-   0        0        0      361 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/icommand_handler.py
--rw-rw-rw-   0        0        0      221 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/iquery.py
--rw-rw-rw-   0        0        0      354 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cqrs/iquery_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.593783 pdip-0.6.5/pdip/cryptography/
--rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cryptography/__init__.py
--rw-rw-rw-   0        0        0     1058 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/cryptography/crypto_service.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.613782 pdip-0.6.5/pdip/data/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.662786 pdip-0.6.5/pdip/data/base/
--rw-rw-rw-   0        0        0       62 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/base/__init__.py
--rw-rw-rw-   0        0        0     2757 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/base/database_session_manager.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.729784 pdip-0.6.5/pdip/data/decorators/
--rw-rw-rw-   0        0        0       53 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/decorators/__init__.py
--rw-rw-rw-   0        0        0      633 2022-01-06 10:48:22.000000 pdip-0.6.5/pdip/data/decorators/transaction_handler.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.794788 pdip-0.6.5/pdip/data/domain/
--rw-rw-rw-   0        0        0       65 2023-03-05 19:14:44.000000 pdip-0.6.5/pdip/data/domain/__init__.py
--rw-rw-rw-   0        0        0     1184 2023-03-05 19:37:01.000000 pdip-0.6.5/pdip/data/domain/entity.py
--rw-rw-rw-   0        0        0      908 2023-03-11 19:15:56.000000 pdip-0.6.5/pdip/data/domain/entity_base.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.834784 pdip-0.6.5/pdip/data/domain/types/
--rw-rw-rw-   0        0        0     1154 2023-03-05 19:38:59.000000 pdip-0.6.5/pdip/data/domain/types/GUID.py
--rw-rw-rw-   0        0        0       22 2023-03-05 19:37:56.000000 pdip-0.6.5/pdip/data/domain/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:25.907786 pdip-0.6.5/pdip/data/repository/
--rw-rw-rw-   0        0        0       89 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/data/repository/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-03-04 02:13:24.000000 pdip-0.6.5/pdip/data/repository/repository.py
--rw-rw-rw-   0        0        0     2031 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/repository/repository_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.095790 pdip-0.6.5/pdip/data/seed/
--rw-rw-rw-   0        0        0       61 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/data/seed/__init__.py
--rw-rw-rw-   0        0        0      115 2022-02-13 20:47:19.000000 pdip-0.6.5/pdip/data/seed/seed.py
--rw-rw-rw-   0        0        0     1478 2022-01-06 19:04:14.000000 pdip-0.6.5/pdip/data/seed/seed_runner.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.198784 pdip-0.6.5/pdip/delivery/
--rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/delivery/__init__.py
--rw-rw-rw-   0        0        0     4042 2022-01-05 12:49:30.000000 pdip-0.6.5/pdip/delivery/email_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.265785 pdip-0.6.5/pdip/dependency/
--rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/dependency/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.326790 pdip-0.6.5/pdip/dependency/container/
--rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/dependency/container/__init__.py
--rw-rw-rw-   0        0        0      945 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/dependency/container/dependency_container.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.407785 pdip-0.6.5/pdip/dependency/provider/
--rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/dependency/provider/__init__.py
--rw-rw-rw-   0        0        0     4253 2023-03-11 21:13:04.000000 pdip-0.6.5/pdip/dependency/provider/api_provider.py
--rw-rw-rw-   0        0        0     6454 2023-02-07 09:16:03.000000 pdip-0.6.5/pdip/dependency/provider/service_provider.py
--rw-rw-rw-   0        0        0      159 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/dependency/scopes.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.538130 pdip-0.6.5/pdip/exceptions/
--rw-rw-rw-   0        0        0      268 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/exceptions/__init__.py
--rw-rw-rw-   0        0        0       58 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/exceptions/incompatible_adapter_exception.py
--rw-rw-rw-   0        0        0      148 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/exceptions/not_supported_feature_exception.py
--rw-rw-rw-   0        0        0       50 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/exceptions/operational_exception.py
--rw-rw-rw-   0        0        0       52 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/exceptions/required_class_exception.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.582131 pdip-0.6.5/pdip/html/
--rw-rw-rw-   0        0        0       68 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/html/__init__.py
--rw-rw-rw-   0        0        0     9512 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/html/html_template_service.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.617132 pdip-0.6.5/pdip/integrator/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.670131 pdip-0.6.5/pdip/integrator/base/
--rw-rw-rw-   0        0        0       36 2022-01-16 21:11:05.000000 pdip-0.6.5/pdip/integrator/base/__init__.py
--rw-rw-rw-   0        0        0     2233 2022-01-25 06:29:38.000000 pdip-0.6.5/pdip/integrator/base/integrator.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.702129 pdip-0.6.5/pdip/integrator/connection/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.793131 pdip-0.6.5/pdip/integrator/connection/base/
--rw-rw-rw-   0        0        0      128 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/base/__init__.py
--rw-rw-rw-   0        0        0      668 2022-02-26 08:17:26.000000 pdip-0.6.5/pdip/integrator/connection/base/connection_source_adapter.py
--rw-rw-rw-   0        0        0      576 2022-02-13 16:45:52.000000 pdip-0.6.5/pdip/integrator/connection/base/connection_target_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.832129 pdip-0.6.5/pdip/integrator/connection/domain/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.862132 pdip-0.6.5/pdip/integrator/connection/domain/authentication/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.924131 pdip-0.6.5/pdip/integrator/connection/domain/authentication/basic/
--rw-rw-rw-   0        0        0       76 2022-01-24 06:37:02.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/basic/__init__.py
--rw-rw-rw-   0        0        0      137 2022-02-10 22:06:47.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/basic/connection_basic_authentication.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:26.988133 pdip-0.6.5/pdip/integrator/connection/domain/authentication/kerberos/
--rw-rw-rw-   0        0        0       61 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/kerberos/__init__.py
--rw-rw-rw-   0        0        0      218 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/kerberos/kerberos_authentication.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.040130 pdip-0.6.5/pdip/integrator/connection/domain/authentication/mechanism/
--rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/mechanism/__init__.py
--rw-rw-rw-   0        0        0      144 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/mechanism/mechanism_types.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.241130 pdip-0.6.5/pdip/integrator/connection/domain/authentication/type/
--rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/type/__init__.py
--rw-rw-rw-   0        0        0      134 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/authentication/type/authentication_types.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.333130 pdip-0.6.5/pdip/integrator/connection/domain/base/
--rw-rw-rw-   0        0        0       42 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/domain/base/__init__.py
--rw-rw-rw-   0        0        0      263 2022-02-10 14:11:07.000000 pdip-0.6.5/pdip/integrator/connection/domain/base/column.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.437132 pdip-0.6.5/pdip/integrator/connection/domain/enums/
--rw-rw-rw-   0        0        0       92 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      154 2022-01-12 17:12:09.000000 pdip-0.6.5/pdip/integrator/connection/domain/enums/connection_types.py
--rw-rw-rw-   0        0        0      212 2022-01-12 17:12:09.000000 pdip-0.6.5/pdip/integrator/connection/domain/enums/connector_types.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.466131 pdip-0.6.5/pdip/integrator/connection/domain/server/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.515131 pdip-0.6.5/pdip/integrator/connection/domain/server/base/
--rw-rw-rw-   0        0        0       49 2022-01-24 06:37:02.000000 pdip-0.6.5/pdip/integrator/connection/domain/server/base/__init__.py
--rw-rw-rw-   0        0        0      120 2022-01-23 16:31:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/server/base/connection_server.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.564130 pdip-0.6.5/pdip/integrator/connection/domain/task/
--rw-rw-rw-   0        0        0       44 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/task/__init__.py
--rw-rw-rw-   0        0        0      406 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/task/data_queue_task.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.587133 pdip-0.6.5/pdip/integrator/connection/domain/types/
--rw-rw-rw-   0        0        0        0 2022-02-10 16:14:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.606131 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/
--rw-rw-rw-   0        0        0        0 2022-02-10 15:34:05.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.646129 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/base/
--rw-rw-rw-   0        0        0       45 2022-02-10 16:15:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/base/__init__.py
--rw-rw-rw-   0        0        0      337 2022-02-13 09:04:59.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/base/big_data.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.674129 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/
--rw-rw-rw-   0        0        0        0 2022-02-13 09:03:54.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.746131 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/base/
--rw-rw-rw-   0        0        0       79 2022-02-10 16:17:31.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      902 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.865131 pdip-0.6.5/pdip/integrator/connection/domain/types/inmemory/
--rw-rw-rw-   0        0        0       81 2022-01-14 16:08:59.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/inmemory/__init__.py
--rw-rw-rw-   0        0        0      346 2022-01-14 19:09:21.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/inmemory/in_memory_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.897130 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/
--rw-rw-rw-   0        0        0        0 2022-02-10 15:34:05.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.947130 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/base/
--rw-rw-rw-   0        0        0       36 2022-02-10 16:15:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/base/__init__.py
--rw-rw-rw-   0        0        0      325 2022-02-10 21:50:35.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/base/sql.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:27.967129 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/
--rw-rw-rw-   0        0        0        2 2022-02-10 16:15:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.028129 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/base/
--rw-rw-rw-   0        0        0       70 2022-02-10 16:16:53.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      855 2022-02-10 21:44:31.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.064132 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.170133 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/base/
--rw-rw-rw-   0        0        0       51 2022-02-10 16:15:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/base/__init__.py
--rw-rw-rw-   0        0        0      314 2022-02-13 09:08:12.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/base/web_service.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.197130 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/
--rw-rw-rw-   0        0        0        0 2022-02-10 16:12:02.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.272131 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/base/
--rw-rw-rw-   0        0        0       85 2022-02-10 16:15:36.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/base/__init__.py
--rw-rw-rw-   0        0        0      572 2022-02-13 09:07:55.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.383133 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/soap/
--rw-rw-rw-   0        0        0       51 2022-02-10 15:34:05.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/soap/__init__.py
--rw-rw-rw-   0        0        0       99 2022-01-12 08:01:00.000000 pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/soap/soap_configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.452131 pdip-0.6.5/pdip/integrator/connection/factories/
--rw-rw-rw-   0        0        0      158 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/factories/__init__.py
--rw-rw-rw-   0        0        0     3095 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/factories/connection_source_adapter_factory.py
--rw-rw-rw-   0        0        0     3466 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/factories/connection_target_adapter_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.471133 pdip-0.6.5/pdip/integrator/connection/types/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.491129 pdip-0.6.5/pdip/integrator/connection/types/bigdata/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.508128 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.544132 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/source/
--rw-rw-rw-   0        0        0       59 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     4642 2022-02-10 06:03:24.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.590132 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/target/
--rw-rw-rw-   0        0        0       59 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     4589 2022-02-13 16:45:52.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.789130 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/
--rw-rw-rw-   0        0        0      282 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/__init__.py
--rw-rw-rw-   0        0        0      458 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_connector.py
--rw-rw-rw-   0        0        0     9560 2022-07-06 08:14:23.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_context.py
--rw-rw-rw-   0        0        0     2014 2022-07-05 16:29:28.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py
--rw-rw-rw-   0        0        0     1842 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py
--rw-rw-rw-   0        0        0     1450 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_policy.py
--rw-rw-rw-   0        0        0     2238 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.825131 pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.892142 pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/impala/
--rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/impala/__init__.py
--rw-rw-rw-   0        0        0     3597 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.916131 pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.961129 pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/impala/
--rw-rw-rw-   0        0        0       43 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/impala/__init__.py
--rw-rw-rw-   0        0        0     5185 2022-07-06 06:15:58.000000 pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:28.984130 pdip-0.6.5/pdip/integrator/connection/types/file/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.031132 pdip-0.6.5/pdip/integrator/connection/types/file/adapters/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/file/adapters/__init__.py
--rw-rw-rw-   0        0        0     8832 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/file/adapters/file_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.116133 pdip-0.6.5/pdip/integrator/connection/types/file/base/
--rw-rw-rw-   0        0        0      123 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/file/base/__init__.py
--rw-rw-rw-   0        0        0     1061 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/file/base/file_connector.py
--rw-rw-rw-   0        0        0     3837 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/file/base/file_context.py
--rw-rw-rw-   0        0        0     1938 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/file/base/file_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.135128 pdip-0.6.5/pdip/integrator/connection/types/file/connectors/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/file/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.179128 pdip-0.6.5/pdip/integrator/connection/types/file/connectors/csv/
--rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/file/connectors/csv/__init__.py
--rw-rw-rw-   0        0        0     3384 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.200131 pdip-0.6.5/pdip/integrator/connection/types/inmemory/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.309660 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/
--rw-rw-rw-   0        0        0      196 2022-01-12 13:27:34.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/__init__.py
--rw-rw-rw-   0        0        0     1273 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py
--rw-rw-rw-   0        0        0     4465 2022-01-12 13:27:34.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_context.py
--rw-rw-rw-   0        0        0     1056 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py
--rw-rw-rw-   0        0        0     1361 2022-02-13 09:02:58.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.335661 pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.375660 pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/sqlite/
--rw-rw-rw-   0        0        0       48 2022-01-14 19:08:48.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1523 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.397660 pdip-0.6.5/pdip/integrator/connection/types/queue/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.436660 pdip-0.6.5/pdip/integrator/connection/types/queue/adapters/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/adapters/__init__.py
--rw-rw-rw-   0        0        0     4288 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/adapters/queue_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.518659 pdip-0.6.5/pdip/integrator/connection/types/queue/base/
--rw-rw-rw-   0        0        0      129 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/base/__init__.py
--rw-rw-rw-   0        0        0     1094 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_connector.py
--rw-rw-rw-   0        0        0     2257 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_context.py
--rw-rw-rw-   0        0        0     2016 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.565662 pdip-0.6.5/pdip/integrator/connection/types/queue/connectors/
--rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/connectors/__init__.py
--rw-rw-rw-   0        0        0     6970 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/queue/connectors/kafka_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.590661 pdip-0.6.5/pdip/integrator/connection/types/sql/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.612660 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.660658 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/source/
--rw-rw-rw-   0        0        0       50 2022-02-01 21:03:35.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     3820 2022-02-13 18:58:01.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.713659 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/target/
--rw-rw-rw-   0        0        0       50 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     3672 2022-02-13 16:45:52.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.840663 pdip-0.6.5/pdip/integrator/connection/types/sql/base/
--rw-rw-rw-   0        0        0      228 2022-02-09 09:53:08.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/__init__.py
--rw-rw-rw-   0        0        0      478 2022-01-16 15:29:03.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_connector.py
--rw-rw-rw-   0        0        0     9467 2022-07-05 16:48:59.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_context.py
--rw-rw-rw-   0        0        0     2014 2022-07-05 15:56:01.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_dialect.py
--rw-rw-rw-   0        0        0     1797 2022-02-10 06:36:41.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_iterator.py
--rw-rw-rw-   0        0        0     1980 2022-02-10 21:51:34.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_policy.py
--rw-rw-rw-   0        0        0     3756 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.861661 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.896660 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mssql/
--rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mssql/__init__.py
--rw-rw-rw-   0        0        0     3340 2022-02-10 21:51:34.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.940664 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mysql/
--rw-rw-rw-   0        0        0       45 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mysql/__init__.py
--rw-rw-rw-   0        0        0     2113 2022-02-10 21:51:34.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:29.984661 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/oracle/
--rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/oracle/__init__.py
--rw-rw-rw-   0        0        0     2640 2022-02-10 21:51:34.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.031659 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/postgresql/
--rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/postgresql/__init__.py
--rw-rw-rw-   0        0        0     2123 2022-02-10 21:46:01.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.055666 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.110663 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mssql/
--rw-rw-rw-   0        0        0       41 2022-01-16 13:08:14.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mssql/__init__.py
--rw-rw-rw-   0        0        0     5467 2022-07-05 15:58:22.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.166660 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mysql/
--rw-rw-rw-   0        0        0       41 2022-01-16 16:08:55.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     5129 2022-02-13 19:24:19.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.230659 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/oracle/
--rw-rw-rw-   0        0        0       43 2022-01-16 16:08:55.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/oracle/__init__.py
--rw-rw-rw-   0        0        0     5434 2022-02-13 19:24:19.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.271662 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/postgresql/
--rw-rw-rw-   0        0        0       51 2022-01-16 16:08:56.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/postgresql/__init__.py
--rw-rw-rw-   0        0        0     5225 2022-02-13 19:24:18.000000 pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.293661 pdip-0.6.5/pdip/integrator/connection/types/webservice/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.319661 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.364906 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/source/
--rw-rw-rw-   0        0        0       65 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/source/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.465661 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/target/
--rw-rw-rw-   0        0        0       65 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/target/__init__.py
--rw-rw-rw-   0        0        0     3434 2022-07-05 16:44:50.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.648664 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/
--rw-rw-rw-   0        0        0      212 2022-01-12 07:24:26.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/__init__.py
--rw-rw-rw-   0        0        0      540 2022-01-12 07:24:26.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_connector.py
--rw-rw-rw-   0        0        0     1779 2022-02-13 20:47:39.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_context.py
--rw-rw-rw-   0        0        0     1061 2022-02-13 20:47:39.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_policy.py
--rw-rw-rw-   0        0        0     1991 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_provider.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.666658 pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.706663 pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/soap/
--rw-rw-rw-   0        0        0       43 2022-01-12 08:15:22.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/soap/__init__.py
--rw-rw-rw-   0        0        0     2122 2022-02-13 09:09:10.000000 pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.741663 pdip-0.6.5/pdip/integrator/domain/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.799659 pdip-0.6.5/pdip/integrator/domain/enums/
--rw-rw-rw-   0        0        0       39 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      437 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/domain/enums/events.py
--rw-rw-rw-   0        0        0      120 2021-10-31 17:47:11.000000 pdip-0.6.5/pdip/integrator/domain/enums/status_types.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.817660 pdip-0.6.5/pdip/integrator/event/
--rw-rw-rw-   0        0        0        0 2022-01-16 20:52:28.000000 pdip-0.6.5/pdip/integrator/event/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.890658 pdip-0.6.5/pdip/integrator/event/base/
--rw-rw-rw-   0        0        0      216 2022-01-16 21:27:09.000000 pdip-0.6.5/pdip/integrator/event/base/__init__.py
--rw-rw-rw-   0        0        0     3100 2022-01-16 21:11:05.000000 pdip-0.6.5/pdip/integrator/event/base/default_integrator_event_manager.py
--rw-rw-rw-   0        0        0     1250 2022-01-16 21:11:05.000000 pdip-0.6.5/pdip/integrator/event/base/integrator_event_manager.py
--rw-rw-rw-   0        0        0     1029 2022-02-04 03:16:01.000000 pdip-0.6.5/pdip/integrator/event/base/integrator_event_manager_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.905661 pdip-0.6.5/pdip/integrator/execution/
--rw-rw-rw-   0        0        0        0 2022-01-16 20:11:55.000000 pdip-0.6.5/pdip/integrator/execution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.918657 pdip-0.6.5/pdip/integrator/execution/base/
--rw-rw-rw-   0        0        0        2 2022-01-16 23:22:14.000000 pdip-0.6.5/pdip/integrator/execution/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.947658 pdip-0.6.5/pdip/integrator/execution/domain/
--rw-rw-rw-   0        0        0      284 2022-01-16 20:23:45.000000 pdip-0.6.5/pdip/integrator/execution/domain/__init__.py
--rw-rw-rw-   0        0        0     1080 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/execution/domain/execution.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.963658 pdip-0.6.5/pdip/integrator/initializer/
--rw-rw-rw-   0        0        0        0 2022-01-16 20:57:53.000000 pdip-0.6.5/pdip/integrator/initializer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:30.991662 pdip-0.6.5/pdip/integrator/initializer/base/
--rw-rw-rw-   0        0        0       38 2022-01-16 23:22:14.000000 pdip-0.6.5/pdip/integrator/initializer/base/__init__.py
--rw-rw-rw-   0        0        0       60 2022-01-16 22:25:18.000000 pdip-0.6.5/pdip/integrator/initializer/base/initializer.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.004658 pdip-0.6.5/pdip/integrator/initializer/execution/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.072661 pdip-0.6.5/pdip/integrator/initializer/execution/base/
--rw-rw-rw-   0        0        0      129 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/base/__init__.py
--rw-rw-rw-   0        0        0     1457 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/base/default_execution_initializer.py
--rw-rw-rw-   0        0        0      386 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/base/execution_initializer.py
--rw-rw-rw-   0        0        0     1013 2022-02-04 03:16:01.000000 pdip-0.6.5/pdip/integrator/initializer/execution/base/execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.141661 pdip-0.6.5/pdip/integrator/initializer/execution/integration/
--rw-rw-rw-   0        0        0      327 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/integration/__init__.py
--rw-rw-rw-   0        0        0      533 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py
--rw-rw-rw-   0        0        0      331 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer.py
--rw-rw-rw-   0        0        0     1217 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.215658 pdip-0.6.5/pdip/integrator/initializer/execution/operation/
--rw-rw-rw-   0        0        0      258 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/operation/__init__.py
--rw-rw-rw-   0        0        0      431 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/operation/default_operation_execution_initializer.py
--rw-rw-rw-   0        0        0      275 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/execution/operation/operation_execution_initializer.py
--rw-rw-rw-   0        0        0     1127 2022-02-04 03:16:01.000000 pdip-0.6.5/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.293658 pdip-0.6.5/pdip/integrator/initializer/integrator/
--rw-rw-rw-   0        0        0      207 2022-01-17 01:06:27.000000 pdip-0.6.5/pdip/integrator/initializer/integrator/__init__.py
--rw-rw-rw-   0        0        0     3286 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/initializer/integrator/default_integrator_initializer.py
--rw-rw-rw-   0        0        0      469 2022-01-25 06:28:03.000000 pdip-0.6.5/pdip/integrator/initializer/integrator/integrator_initializer.py
--rw-rw-rw-   0        0        0     1019 2022-02-04 03:16:01.000000 pdip-0.6.5/pdip/integrator/initializer/integrator/integrator_initializer_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.307657 pdip-0.6.5/pdip/integrator/integration/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.333658 pdip-0.6.5/pdip/integrator/integration/base/
--rw-rw-rw-   0        0        0       57 2022-01-16 23:22:14.000000 pdip-0.6.5/pdip/integrator/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3845 2022-02-13 16:15:29.000000 pdip-0.6.5/pdip/integrator/integration/base/integration_execution.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.347658 pdip-0.6.5/pdip/integrator/integration/domain/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/integration/domain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.373659 pdip-0.6.5/pdip/integrator/integration/domain/base/
--rw-rw-rw-   0        0        0       94 2022-02-10 15:34:05.000000 pdip-0.6.5/pdip/integrator/integration/domain/base/__init__.py
--rw-rw-rw-   0        0        0     1031 2022-02-13 20:47:39.000000 pdip-0.6.5/pdip/integrator/integration/domain/base/integration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.402658 pdip-0.6.5/pdip/integrator/integration/domain/enums/
--rw-rw-rw-   0        0        0       49 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/integration/domain/enums/__init__.py
--rw-rw-rw-   0        0        0      114 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/domain/enums/integration_types.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.416657 pdip-0.6.5/pdip/integrator/integration/types/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.459662 pdip-0.6.5/pdip/integrator/integration/types/base/
--rw-rw-rw-   0        0        0      121 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/base/__init__.py
--rw-rw-rw-   0        0        0      728 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/base/integration_adapter.py
--rw-rw-rw-   0        0        0     1845 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/base/integration_adapter_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.474658 pdip-0.6.5/pdip/integrator/integration/types/source/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/source/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.504661 pdip-0.6.5/pdip/integrator/integration/types/source/base/
--rw-rw-rw-   0        0        0       51 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/integration/types/source/base/__init__.py
--rw-rw-rw-   0        0        0     5127 2022-02-26 13:30:17.000000 pdip-0.6.5/pdip/integrator/integration/types/source/base/source_integration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.518659 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.549657 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/base/
--rw-rw-rw-   0        0        0       69 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/base/__init__.py
--rw-rw-rw-   0        0        0     6664 2022-02-13 17:38:52.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.564664 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/
--rw-rw-rw-   0        0        0        0 2022-02-13 17:38:52.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.593658 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/base/
--rw-rw-rw-   0        0        0      101 2022-02-13 17:38:52.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/base/__init__.py
--rw-rw-rw-   0        0        0      537 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.634661 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/factories/
--rw-rw-rw-   0        0        0       99 2022-02-13 20:47:39.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/factories/__init__.py
--rw-rw-rw-   0        0        0     1723 2022-02-26 08:16:34.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.656659 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/
--rw-rw-rw-   0        0        0        0 2022-02-13 17:30:21.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.694660 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/
--rw-rw-rw-   0        0        0       70 2022-02-13 17:38:52.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/__init__.py
--rw-rw-rw-   0        0        0    18820 2022-02-13 17:40:40.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.711661 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/
--rw-rw-rw-   0        0        0        0 2022-02-13 17:30:21.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.743658 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/
--rw-rw-rw-   0        0        0       83 2022-02-26 08:16:34.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/__init__.py
--rw-rw-rw-   0        0        0     7431 2022-02-28 06:09:14.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.760660 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/
--rw-rw-rw-   0        0        0        0 2022-02-26 07:23:54.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.789660 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/
--rw-rw-rw-   0        0        0       56 2022-02-28 06:09:14.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/__init__.py
--rw-rw-rw-   0        0        0     4368 2022-02-26 08:27:28.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.821659 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/
--rw-rw-rw-   0        0        0       58 2022-02-28 06:09:14.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/__init__.py
--rw-rw-rw-   0        0        0     8709 2022-02-26 09:01:27.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.836658 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/
--rw-rw-rw-   0        0        0        0 2022-02-26 07:23:54.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.883659 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/
--rw-rw-rw-   0        0        0      105 2022-02-26 07:36:10.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/__init__.py
--rw-rw-rw-   0        0        0     7222 2022-02-26 08:16:34.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py
--rw-rw-rw-   0        0        0     3887 2022-02-26 08:16:34.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.928660 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/
--rw-rw-rw-   0        0        0       74 2022-02-13 22:42:38.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/__init__.py
--rw-rw-rw-   0        0        0      144 2022-02-13 22:42:38.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_info.py
--rw-rw-rw-   0        0        0      304 2022-02-13 22:42:37.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_task.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.962660 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/
--rw-rw-rw-   0        0        0       75 2022-02-26 07:36:10.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/__init__.py
--rw-rw-rw-   0        0        0      438 2022-02-26 07:36:10.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/parallel_session_broker_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:31.978659 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/
--rw-rw-rw-   0        0        0      166 2022-02-13 20:47:39.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.024661 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/
--rw-rw-rw-   0        0        0       81 2022-02-13 17:38:52.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/__init__.py
--rw-rw-rw-   0        0        0     3917 2022-02-13 17:41:31.000000 pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.048660 pdip-0.6.5/pdip/integrator/integration/types/target/
--rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/target/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.095660 pdip-0.6.5/pdip/integrator/integration/types/target/base/
--rw-rw-rw-   0        0        0       51 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/target/base/__init__.py
--rw-rw-rw-   0        0        0     2684 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/integration/types/target/base/target_integration.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.115661 pdip-0.6.5/pdip/integrator/operation/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/operation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.143657 pdip-0.6.5/pdip/integrator/operation/base/
--rw-rw-rw-   0        0        0       53 2022-01-16 23:22:14.000000 pdip-0.6.5/pdip/integrator/operation/base/__init__.py
--rw-rw-rw-   0        0        0     2325 2022-02-01 21:03:36.000000 pdip-0.6.5/pdip/integrator/operation/base/operation_execution.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.175661 pdip-0.6.5/pdip/integrator/operation/domain/
--rw-rw-rw-   0        0        0       64 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/integrator/operation/domain/__init__.py
--rw-rw-rw-   0        0        0      808 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/operation/domain/operation.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.192658 pdip-0.6.5/pdip/integrator/pubsub/
--rw-rw-rw-   0        0        0        0 2022-01-02 19:32:28.000000 pdip-0.6.5/pdip/integrator/pubsub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.264659 pdip-0.6.5/pdip/integrator/pubsub/base/
--rw-rw-rw-   0        0        0      183 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/pubsub/base/__init__.py
--rw-rw-rw-   0        0        0      342 2022-01-03 13:30:44.000000 pdip-0.6.5/pdip/integrator/pubsub/base/channel_queue.py
--rw-rw-rw-   0        0        0     1529 2022-01-06 18:31:38.000000 pdip-0.6.5/pdip/integrator/pubsub/base/event_listener.py
--rw-rw-rw-   0        0        0     3040 2022-02-13 22:42:38.000000 pdip-0.6.5/pdip/integrator/pubsub/base/message_broker.py
--rw-rw-rw-   0        0        0     1302 2022-02-13 22:42:38.000000 pdip-0.6.5/pdip/integrator/pubsub/base/message_broker_worker.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.295189 pdip-0.6.5/pdip/integrator/pubsub/domain/
--rw-rw-rw-   0        0        0       34 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/pubsub/domain/__init__.py
--rw-rw-rw-   0        0        0      168 2022-01-05 01:38:23.000000 pdip-0.6.5/pdip/integrator/pubsub/domain/message.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.327186 pdip-0.6.5/pdip/integrator/pubsub/publisher/
--rw-rw-rw-   0        0        0       34 2022-02-13 20:47:19.000000 pdip-0.6.5/pdip/integrator/pubsub/publisher/__init__.py
--rw-rw-rw-   0        0        0      252 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/integrator/pubsub/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.343187 pdip-0.6.5/pdip/integrator/pubsub/subscriber/
--rw-rw-rw-   0        0        0        0 2022-01-01 12:02:58.000000 pdip-0.6.5/pdip/integrator/pubsub/subscriber/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.383185 pdip-0.6.5/pdip/io/
--rw-rw-rw-   0        0        0       82 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/io/__init__.py
--rw-rw-rw-   0        0        0     1011 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/io/file_manager.py
--rw-rw-rw-   0        0        0     1326 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/io/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.396187 pdip-0.6.5/pdip/json/
--rw-rw-rw-   0        0        0      320 2023-03-11 19:32:52.000000 pdip-0.6.5/pdip/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.441188 pdip-0.6.5/pdip/json/base/
--rw-rw-rw-   0        0        0        0 2023-03-11 19:22:26.000000 pdip-0.6.5/pdip/json/base/__init__.py
--rw-rw-rw-   0        0        0     3786 2023-03-11 19:32:52.000000 pdip-0.6.5/pdip/json/base/base_converter.py
--rw-rw-rw-   0        0        0     1037 2023-03-11 20:00:23.000000 pdip-0.6.5/pdip/json/base/json_convert.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.508186 pdip-0.6.5/pdip/json/encoders/
--rw-rw-rw-   0        0        0        0 2023-03-11 19:20:44.000000 pdip-0.6.5/pdip/json/encoders/__init__.py
--rw-rw-rw-   0        0        0      311 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/json/encoders/date_time_encoder.py
--rw-rw-rw-   0        0        0      734 2023-03-11 19:20:16.000000 pdip-0.6.5/pdip/json/encoders/mutliple_json_encoders.py
--rw-rw-rw-   0        0        0      272 2023-03-11 19:20:17.000000 pdip-0.6.5/pdip/json/encoders/uuid_encoder.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.533188 pdip-0.6.5/pdip/json/parsers/
--rw-rw-rw-   0        0        0        0 2023-03-11 19:21:45.000000 pdip-0.6.5/pdip/json/parsers/__init__.py
--rw-rw-rw-   0        0        0      528 2022-01-12 10:33:46.000000 pdip-0.6.5/pdip/json/parsers/date_time_parser.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.562188 pdip-0.6.5/pdip/logging/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.614186 pdip-0.6.5/pdip/logging/domain/
--rw-rw-rw-   0        0        0       31 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/domain/__init__.py
--rw-rw-rw-   0        0        0      499 2022-01-04 08:12:15.000000 pdip-0.6.5/pdip/logging/domain/log_data.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.632187 pdip-0.6.5/pdip/logging/loggers/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.666187 pdip-0.6.5/pdip/logging/loggers/base/
--rw-rw-rw-   0        0        0       30 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/loggers/base/__init__.py
--rw-rw-rw-   0        0        0     1015 2022-02-13 20:47:19.000000 pdip-0.6.5/pdip/logging/loggers/base/ilogger.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.698186 pdip-0.6.5/pdip/logging/loggers/console/
--rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/loggers/console/__init__.py
--rw-rw-rw-   0        0        0     1881 2022-01-03 21:37:05.000000 pdip-0.6.5/pdip/logging/loggers/console/console_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.729186 pdip-0.6.5/pdip/logging/loggers/file/
--rw-rw-rw-   0        0        0       37 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/loggers/file/__init__.py
--rw-rw-rw-   0        0        0     1977 2022-02-13 20:47:18.000000 pdip-0.6.5/pdip/logging/loggers/file/file_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.759185 pdip-0.6.5/pdip/logging/loggers/sql/
--rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/logging/loggers/sql/__init__.py
--rw-rw-rw-   0        0        0     4728 2023-03-05 19:19:52.000000 pdip-0.6.5/pdip/logging/loggers/sql/sql_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.774187 pdip-0.6.5/pdip/processing/
--rw-rw-rw-   0        0        0       65 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.816187 pdip-0.6.5/pdip/processing/base/
--rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/base/__init__.py
--rw-rw-rw-   0        0        0     7549 2022-02-13 20:47:40.000000 pdip-0.6.5/pdip/processing/base/process_manager.py
--rw-rw-rw-   0        0        0     2430 2022-02-13 20:27:25.000000 pdip-0.6.5/pdip/processing/base/subprocess.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.843184 pdip-0.6.5/pdip/processing/factories/
--rw-rw-rw-   0        0        0       60 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/factories/__init__.py
--rw-rw-rw-   0        0        0      418 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/factories/process_manager_factory.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.884185 pdip-0.6.5/pdip/processing/models/
--rw-rw-rw-   0        0        0       78 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/models/__init__.py
--rw-rw-rw-   0        0        0      348 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/models/process_info.py
--rw-rw-rw-   0        0        0      776 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/processing/models/process_task.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:32.938188 pdip-0.6.5/pdip/utils/
--rw-rw-rw-   0        0        0      106 2021-12-24 11:05:16.000000 pdip-0.6.5/pdip/utils/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-03-11 21:00:07.000000 pdip-0.6.5/pdip/utils/module_finder.py
--rw-rw-rw-   0        0        0     1531 2023-03-05 21:22:19.000000 pdip-0.6.5/pdip/utils/type_checker.py
--rw-rw-rw-   0        0        0     2936 2023-02-07 07:53:51.000000 pdip-0.6.5/pdip/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-11 21:23:23.416783 pdip-0.6.5/pdip.egg-info/
--rw-rw-rw-   0        0        0     1330 2023-03-11 21:23:20.000000 pdip-0.6.5/pdip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    21251 2023-03-11 21:23:21.000000 pdip-0.6.5/pdip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 21:23:20.000000 pdip-0.6.5/pdip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-11 21:23:20.000000 pdip-0.6.5/pdip.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-03-11 21:23:20.000000 pdip-0.6.5/pdip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-11 21:23:20.000000 pdip-0.6.5/pdip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2023-03-11 21:23:32.960187 pdip-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2190 2023-03-11 21:22:43.000000 pdip-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:29.147218 pdip-0.6.6/
+-rw-rw-rw-   0        0        0     1097 2021-12-24 11:05:16.000000 pdip-0.6.6/LICENSE
+-rw-rw-rw-   0        0        0     1330 2023-03-13 00:46:29.160225 pdip-0.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-13 00:45:59.915104 pdip-0.6.6/pdip/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:00.531101 pdip-0.6.6/pdip/api/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:00.800103 pdip-0.6.6/pdip/api/app/
+-rw-rw-rw-   0        0        0       48 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/app/__init__.py
+-rw-rw-rw-   0        0        0     1941 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/app/flask_app_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:00.988101 pdip-0.6.6/pdip/api/base/
+-rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/base/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-03-11 21:16:51.000000 pdip-0.6.6/pdip/api/base/controller_base.py
+-rw-rw-rw-   0        0        0     4506 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/base/endpoint_base.py
+-rw-rw-rw-   0        0        0     8789 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/api/base/endpoint_wrapper.py
+-rw-rw-rw-   0        0        0      172 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/base/resource_base.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.225106 pdip-0.6.6/pdip/api/converter/
+-rw-rw-rw-   0        0        0       49 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/converter/__init__.py
+-rw-rw-rw-   0        0        0     3284 2022-01-17 05:17:17.000000 pdip-0.6.6/pdip/api/converter/request_converter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.350104 pdip-0.6.6/pdip/api/decorators/
+-rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/decorators/__init__.py
+-rw-rw-rw-   0        0        0      240 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/decorators/controller_base.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.480104 pdip-0.6.6/pdip/api/handlers/
+-rw-rw-rw-   0        0        0       88 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3755 2022-01-23 16:31:36.000000 pdip-0.6.6/pdip/api/handlers/error_handlers.py
+-rw-rw-rw-   0        0        0     1515 2022-02-13 20:47:19.000000 pdip-0.6.6/pdip/api/handlers/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.629116 pdip-0.6.6/pdip/api/request_parameter/
+-rw-rw-rw-   0        0        0       97 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/request_parameter/__init__.py
+-rw-rw-rw-   0        0        0      124 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/request_parameter/order_by_parameter.py
+-rw-rw-rw-   0        0        0      129 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/request_parameter/paging_parameter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.765107 pdip-0.6.6/pdip/api/specifications/
+-rw-rw-rw-   0        0        0      113 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/api/specifications/__init__.py
+-rw-rw-rw-   0        0        0     1492 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/specifications/order_by_specification.py
+-rw-rw-rw-   0        0        0     1252 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/api/specifications/paging_specification.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.871106 pdip-0.6.6/pdip/base/
+-rw-rw-rw-   0        0        0       22 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/base/__init__.py
+-rw-rw-rw-   0        0        0     1677 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/base/pdi.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:01.979106 pdip-0.6.6/pdip/configuration/
+-rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/__init__.py
+-rw-rw-rw-   0        0        0     5060 2023-03-04 01:10:13.000000 pdip-0.6.6/pdip/configuration/config_manager.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.021105 pdip-0.6.6/pdip/configuration/models/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.122110 pdip-0.6.6/pdip/configuration/models/api/
+-rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/api/__init__.py
+-rw-rw-rw-   0        0        0      334 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/api/api_config.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.221109 pdip-0.6.6/pdip/configuration/models/application/
+-rw-rw-rw-   0        0        0       51 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/application/__init__.py
+-rw-rw-rw-   0        0        0      271 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/application/application_config.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.374101 pdip-0.6.6/pdip/configuration/models/aps/
+-rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/aps/__init__.py
+-rw-rw-rw-   0        0        0      380 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/aps/aps_config.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.535110 pdip-0.6.6/pdip/configuration/models/base/
+-rw-rw-rw-   0        0        0      236 2023-03-04 00:45:05.000000 pdip-0.6.6/pdip/configuration/models/base/__init__.py
+-rw-rw-rw-   0        0        0       87 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/base/base_config.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.664107 pdip-0.6.6/pdip/configuration/models/database/
+-rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/database/__init__.py
+-rw-rw-rw-   0        0        0      450 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/models/database/database_config.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:02.855111 pdip-0.6.6/pdip/configuration/services/
+-rw-rw-rw-   0        0        0       99 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/services/__init__.py
+-rw-rw-rw-   0        0        0      482 2022-01-04 10:22:25.000000 pdip-0.6.6/pdip/configuration/services/config_parameter_base.py
+-rw-rw-rw-   0        0        0     1051 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/configuration/services/config_service.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:03.307107 pdip-0.6.6/pdip/cqrs/
+-rw-rw-rw-   0        0        0      301 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/__init__.py
+-rw-rw-rw-   0        0        0      162 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/command_query_base.py
+-rw-rw-rw-   0        0        0      331 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/command_query_handler_base.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:03.699107 pdip-0.6.6/pdip/cqrs/decorators/
+-rw-rw-rw-   0        0        0      117 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/decorators/__init__.py
+-rw-rw-rw-   0        0        0      861 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/decorators/cls_to_dict.py
+-rw-rw-rw-   0        0        0      277 2023-03-11 19:32:52.000000 pdip-0.6.6/pdip/cqrs/decorators/dto_class.py
+-rw-rw-rw-   0        0        0      281 2023-03-11 19:32:52.000000 pdip-0.6.6/pdip/cqrs/decorators/request_class.py
+-rw-rw-rw-   0        0        0      282 2023-03-11 19:32:52.000000 pdip-0.6.6/pdip/cqrs/decorators/response_class.py
+-rw-rw-rw-   0        0        0     1586 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/cqrs/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:03.879114 pdip-0.6.6/pdip/cqrs/generator/
+-rw-rw-rw-   0        0        0       66 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.220110 pdip-0.6.6/pdip/cqrs/generator/domain/
+-rw-rw-rw-   0        0        0      187 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/domain/__init__.py
+-rw-rw-rw-   0        0        0      126 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/domain/dao_generate_config.py
+-rw-rw-rw-   0        0        0      241 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/domain/generate_config.py
+-rw-rw-rw-   0        0        0      167 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/domain/generator.py
+-rw-rw-rw-   0        0        0      198 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/domain/query_generate_config.py
+-rw-rw-rw-   0        0        0    12142 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/generator/query_generator.py
+-rw-rw-rw-   0        0        0      223 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/icommand.py
+-rw-rw-rw-   0        0        0      361 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/icommand_handler.py
+-rw-rw-rw-   0        0        0      221 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/iquery.py
+-rw-rw-rw-   0        0        0      354 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cqrs/iquery_handler.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.343113 pdip-0.6.6/pdip/cryptography/
+-rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     1058 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/cryptography/crypto_service.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.485118 pdip-0.6.6/pdip/data/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.570111 pdip-0.6.6/pdip/data/base/
+-rw-rw-rw-   0        0        0       62 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/base/__init__.py
+-rw-rw-rw-   0        0        0     2757 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/base/database_session_manager.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.699115 pdip-0.6.6/pdip/data/decorators/
+-rw-rw-rw-   0        0        0       53 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/decorators/__init__.py
+-rw-rw-rw-   0        0        0      633 2022-01-06 10:48:22.000000 pdip-0.6.6/pdip/data/decorators/transaction_handler.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.812111 pdip-0.6.6/pdip/data/domain/
+-rw-rw-rw-   0        0        0       65 2023-03-05 19:14:44.000000 pdip-0.6.6/pdip/data/domain/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-03-12 14:17:54.000000 pdip-0.6.6/pdip/data/domain/entity.py
+-rw-rw-rw-   0        0        0      908 2023-03-11 19:15:56.000000 pdip-0.6.6/pdip/data/domain/entity_base.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:05.895113 pdip-0.6.6/pdip/data/domain/types/
+-rw-rw-rw-   0        0        0     1154 2023-03-05 19:38:59.000000 pdip-0.6.6/pdip/data/domain/types/GUID.py
+-rw-rw-rw-   0        0        0       22 2023-03-05 19:37:56.000000 pdip-0.6.6/pdip/data/domain/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.179111 pdip-0.6.6/pdip/data/repository/
+-rw-rw-rw-   0        0        0       89 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/data/repository/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-03-04 02:13:24.000000 pdip-0.6.6/pdip/data/repository/repository.py
+-rw-rw-rw-   0        0        0     2031 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/repository/repository_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.304113 pdip-0.6.6/pdip/data/seed/
+-rw-rw-rw-   0        0        0       61 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/data/seed/__init__.py
+-rw-rw-rw-   0        0        0      115 2022-02-13 20:47:19.000000 pdip-0.6.6/pdip/data/seed/seed.py
+-rw-rw-rw-   0        0        0     1478 2022-01-06 19:04:14.000000 pdip-0.6.6/pdip/data/seed/seed_runner.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.482114 pdip-0.6.6/pdip/delivery/
+-rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/delivery/__init__.py
+-rw-rw-rw-   0        0        0     4042 2022-01-05 12:49:30.000000 pdip-0.6.6/pdip/delivery/email_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.575125 pdip-0.6.6/pdip/dependency/
+-rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/dependency/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.667115 pdip-0.6.6/pdip/dependency/container/
+-rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/dependency/container/__init__.py
+-rw-rw-rw-   0        0        0      945 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/dependency/container/dependency_container.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.803113 pdip-0.6.6/pdip/dependency/provider/
+-rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/dependency/provider/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-03-11 21:13:04.000000 pdip-0.6.6/pdip/dependency/provider/api_provider.py
+-rw-rw-rw-   0        0        0     6454 2023-02-07 09:16:03.000000 pdip-0.6.6/pdip/dependency/provider/service_provider.py
+-rw-rw-rw-   0        0        0      159 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/dependency/scopes.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:06.952117 pdip-0.6.6/pdip/exceptions/
+-rw-rw-rw-   0        0        0      268 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       58 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/exceptions/incompatible_adapter_exception.py
+-rw-rw-rw-   0        0        0      148 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/exceptions/not_supported_feature_exception.py
+-rw-rw-rw-   0        0        0       50 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/exceptions/operational_exception.py
+-rw-rw-rw-   0        0        0       52 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/exceptions/required_class_exception.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.026112 pdip-0.6.6/pdip/html/
+-rw-rw-rw-   0        0        0       68 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/html/__init__.py
+-rw-rw-rw-   0        0        0     9512 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/html/html_template_service.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.067113 pdip-0.6.6/pdip/integrator/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.133113 pdip-0.6.6/pdip/integrator/base/
+-rw-rw-rw-   0        0        0       36 2022-01-16 21:11:05.000000 pdip-0.6.6/pdip/integrator/base/__init__.py
+-rw-rw-rw-   0        0        0     2233 2022-01-25 06:29:38.000000 pdip-0.6.6/pdip/integrator/base/integrator.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.175113 pdip-0.6.6/pdip/integrator/connection/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.281113 pdip-0.6.6/pdip/integrator/connection/base/
+-rw-rw-rw-   0        0        0      128 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/base/__init__.py
+-rw-rw-rw-   0        0        0      668 2022-02-26 08:17:26.000000 pdip-0.6.6/pdip/integrator/connection/base/connection_source_adapter.py
+-rw-rw-rw-   0        0        0      576 2022-02-13 16:45:52.000000 pdip-0.6.6/pdip/integrator/connection/base/connection_target_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.317111 pdip-0.6.6/pdip/integrator/connection/domain/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.355113 pdip-0.6.6/pdip/integrator/connection/domain/authentication/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.420114 pdip-0.6.6/pdip/integrator/connection/domain/authentication/basic/
+-rw-rw-rw-   0        0        0       76 2022-01-24 06:37:02.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/basic/__init__.py
+-rw-rw-rw-   0        0        0      137 2022-02-10 22:06:47.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/basic/connection_basic_authentication.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.481116 pdip-0.6.6/pdip/integrator/connection/domain/authentication/kerberos/
+-rw-rw-rw-   0        0        0       61 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/kerberos/__init__.py
+-rw-rw-rw-   0        0        0      218 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/kerberos/kerberos_authentication.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.539112 pdip-0.6.6/pdip/integrator/connection/domain/authentication/mechanism/
+-rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/mechanism/__init__.py
+-rw-rw-rw-   0        0        0      144 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/mechanism/mechanism_types.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.640115 pdip-0.6.6/pdip/integrator/connection/domain/authentication/type/
+-rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/type/__init__.py
+-rw-rw-rw-   0        0        0      134 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/authentication/type/authentication_types.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.703117 pdip-0.6.6/pdip/integrator/connection/domain/base/
+-rw-rw-rw-   0        0        0       42 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/domain/base/__init__.py
+-rw-rw-rw-   0        0        0      263 2022-02-10 14:11:07.000000 pdip-0.6.6/pdip/integrator/connection/domain/base/column.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.823112 pdip-0.6.6/pdip/integrator/connection/domain/enums/
+-rw-rw-rw-   0        0        0       92 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      154 2022-01-12 17:12:09.000000 pdip-0.6.6/pdip/integrator/connection/domain/enums/connection_types.py
+-rw-rw-rw-   0        0        0      212 2022-01-12 17:12:09.000000 pdip-0.6.6/pdip/integrator/connection/domain/enums/connector_types.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.862117 pdip-0.6.6/pdip/integrator/connection/domain/server/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:07.922117 pdip-0.6.6/pdip/integrator/connection/domain/server/base/
+-rw-rw-rw-   0        0        0       49 2022-01-24 06:37:02.000000 pdip-0.6.6/pdip/integrator/connection/domain/server/base/__init__.py
+-rw-rw-rw-   0        0        0      120 2022-01-23 16:31:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/server/base/connection_server.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.004114 pdip-0.6.6/pdip/integrator/connection/domain/task/
+-rw-rw-rw-   0        0        0       44 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/task/__init__.py
+-rw-rw-rw-   0        0        0      406 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/task/data_queue_task.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.031112 pdip-0.6.6/pdip/integrator/connection/domain/types/
+-rw-rw-rw-   0        0        0        0 2022-02-10 16:14:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.062117 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/
+-rw-rw-rw-   0        0        0        0 2022-02-10 15:34:05.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.147137 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/base/
+-rw-rw-rw-   0        0        0       45 2022-02-10 16:15:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/base/__init__.py
+-rw-rw-rw-   0        0        0      337 2022-02-13 09:04:59.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/base/big_data.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.221122 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/
+-rw-rw-rw-   0        0        0        0 2022-02-13 09:03:54.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.311115 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/base/
+-rw-rw-rw-   0        0        0       79 2022-02-10 16:17:31.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      902 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.467118 pdip-0.6.6/pdip/integrator/connection/domain/types/inmemory/
+-rw-rw-rw-   0        0        0       81 2022-01-14 16:08:59.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/inmemory/__init__.py
+-rw-rw-rw-   0        0        0      346 2022-01-14 19:09:21.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/inmemory/in_memory_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.531121 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/
+-rw-rw-rw-   0        0        0        0 2022-02-10 15:34:05.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.720113 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/base/
+-rw-rw-rw-   0        0        0       36 2022-02-10 16:15:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/base/__init__.py
+-rw-rw-rw-   0        0        0      325 2022-02-10 21:50:35.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/base/sql.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.794117 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/
+-rw-rw-rw-   0        0        0        2 2022-02-10 16:15:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.911123 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/base/
+-rw-rw-rw-   0        0        0       70 2022-02-10 16:16:53.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      855 2022-02-10 21:44:31.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:08.998120 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.306116 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/base/
+-rw-rw-rw-   0        0        0       51 2022-02-10 16:15:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/base/__init__.py
+-rw-rw-rw-   0        0        0      314 2022-02-13 09:08:12.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/base/web_service.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.456122 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/
+-rw-rw-rw-   0        0        0        0 2022-02-10 16:12:02.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.580119 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/base/
+-rw-rw-rw-   0        0        0       85 2022-02-10 16:15:36.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/base/__init__.py
+-rw-rw-rw-   0        0        0      572 2022-02-13 09:07:55.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.678119 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/soap/
+-rw-rw-rw-   0        0        0       51 2022-02-10 15:34:05.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/soap/__init__.py
+-rw-rw-rw-   0        0        0       99 2022-01-12 08:01:00.000000 pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/soap/soap_configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.803117 pdip-0.6.6/pdip/integrator/connection/factories/
+-rw-rw-rw-   0        0        0      158 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/factories/__init__.py
+-rw-rw-rw-   0        0        0     3095 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/factories/connection_source_adapter_factory.py
+-rw-rw-rw-   0        0        0     3466 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/factories/connection_target_adapter_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.845124 pdip-0.6.6/pdip/integrator/connection/types/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.874117 pdip-0.6.6/pdip/integrator/connection/types/bigdata/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.905115 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:09.972118 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/source/
+-rw-rw-rw-   0        0        0       59 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     4642 2022-02-10 06:03:24.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:10.141131 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/target/
+-rw-rw-rw-   0        0        0       59 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     4589 2022-02-13 16:45:52.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:10.682125 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/
+-rw-rw-rw-   0        0        0      282 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/__init__.py
+-rw-rw-rw-   0        0        0      458 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_connector.py
+-rw-rw-rw-   0        0        0     9560 2022-07-06 08:14:23.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_context.py
+-rw-rw-rw-   0        0        0     2014 2022-07-05 16:29:28.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py
+-rw-rw-rw-   0        0        0     1842 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py
+-rw-rw-rw-   0        0        0     1450 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_policy.py
+-rw-rw-rw-   0        0        0     2238 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:10.758118 pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:10.838119 pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/impala/
+-rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/impala/__init__.py
+-rw-rw-rw-   0        0        0     3597 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:10.885122 pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:11.087121 pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/impala/
+-rw-rw-rw-   0        0        0       43 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/impala/__init__.py
+-rw-rw-rw-   0        0        0     5185 2022-07-06 06:15:58.000000 pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:11.229122 pdip-0.6.6/pdip/integrator/connection/types/file/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:11.323117 pdip-0.6.6/pdip/integrator/connection/types/file/adapters/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/file/adapters/__init__.py
+-rw-rw-rw-   0        0        0     8832 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/file/adapters/file_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:11.942119 pdip-0.6.6/pdip/integrator/connection/types/file/base/
+-rw-rw-rw-   0        0        0      123 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/file/base/__init__.py
+-rw-rw-rw-   0        0        0     1061 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/file/base/file_connector.py
+-rw-rw-rw-   0        0        0     3837 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/file/base/file_context.py
+-rw-rw-rw-   0        0        0     1938 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/file/base/file_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:12.152122 pdip-0.6.6/pdip/integrator/connection/types/file/connectors/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/file/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:12.374121 pdip-0.6.6/pdip/integrator/connection/types/file/connectors/csv/
+-rw-rw-rw-   0        0        0       41 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/file/connectors/csv/__init__.py
+-rw-rw-rw-   0        0        0     3384 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:12.484124 pdip-0.6.6/pdip/integrator/connection/types/inmemory/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:12.970644 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/
+-rw-rw-rw-   0        0        0      196 2022-01-12 13:27:34.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/__init__.py
+-rw-rw-rw-   0        0        0     1273 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py
+-rw-rw-rw-   0        0        0     4465 2022-01-12 13:27:34.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_context.py
+-rw-rw-rw-   0        0        0     1056 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py
+-rw-rw-rw-   0        0        0     1361 2022-02-13 09:02:58.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:13.018647 pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:13.306656 pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/sqlite/
+-rw-rw-rw-   0        0        0       48 2022-01-14 19:08:48.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1523 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:13.457648 pdip-0.6.6/pdip/integrator/connection/types/queue/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:13.554650 pdip-0.6.6/pdip/integrator/connection/types/queue/adapters/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4288 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/adapters/queue_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:13.921649 pdip-0.6.6/pdip/integrator/connection/types/queue/base/
+-rw-rw-rw-   0        0        0      129 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/base/__init__.py
+-rw-rw-rw-   0        0        0     1094 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_connector.py
+-rw-rw-rw-   0        0        0     2257 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_context.py
+-rw-rw-rw-   0        0        0     2016 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:14.266648 pdip-0.6.6/pdip/integrator/connection/types/queue/connectors/
+-rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/connectors/__init__.py
+-rw-rw-rw-   0        0        0     6970 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/queue/connectors/kafka_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:14.385653 pdip-0.6.6/pdip/integrator/connection/types/sql/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:14.484647 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:14.676659 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/source/
+-rw-rw-rw-   0        0        0       50 2022-02-01 21:03:35.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     3820 2022-02-13 18:58:01.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:14.935647 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/target/
+-rw-rw-rw-   0        0        0       50 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     3672 2022-02-13 16:45:52.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:15.929201 pdip-0.6.6/pdip/integrator/connection/types/sql/base/
+-rw-rw-rw-   0        0        0      228 2022-02-09 09:53:08.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/__init__.py
+-rw-rw-rw-   0        0        0      478 2022-01-16 15:29:03.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_connector.py
+-rw-rw-rw-   0        0        0     9467 2022-07-05 16:48:59.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_context.py
+-rw-rw-rw-   0        0        0     2014 2022-07-05 15:56:01.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_dialect.py
+-rw-rw-rw-   0        0        0     1797 2022-02-10 06:36:41.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_iterator.py
+-rw-rw-rw-   0        0        0     1980 2022-02-10 21:51:34.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_policy.py
+-rw-rw-rw-   0        0        0     3756 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:15.973198 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.071199 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mssql/
+-rw-rw-rw-   0        0        0       45 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mssql/__init__.py
+-rw-rw-rw-   0        0        0     3340 2022-02-10 21:51:34.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.168199 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mysql/
+-rw-rw-rw-   0        0        0       45 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mysql/__init__.py
+-rw-rw-rw-   0        0        0     2113 2022-02-10 21:51:34.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.447203 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/oracle/
+-rw-rw-rw-   0        0        0       47 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/oracle/__init__.py
+-rw-rw-rw-   0        0        0     2640 2022-02-10 21:51:34.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.705206 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/postgresql/
+-rw-rw-rw-   0        0        0       55 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/postgresql/__init__.py
+-rw-rw-rw-   0        0        0     2123 2022-02-10 21:46:01.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.787203 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:16.975206 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mssql/
+-rw-rw-rw-   0        0        0       41 2022-01-16 13:08:14.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mssql/__init__.py
+-rw-rw-rw-   0        0        0     5467 2022-07-05 15:58:22.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.235204 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mysql/
+-rw-rw-rw-   0        0        0       41 2022-01-16 16:08:55.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     5129 2022-02-13 19:24:19.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.391198 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/oracle/
+-rw-rw-rw-   0        0        0       43 2022-01-16 16:08:55.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/oracle/__init__.py
+-rw-rw-rw-   0        0        0     5434 2022-02-13 19:24:19.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.568202 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/postgresql/
+-rw-rw-rw-   0        0        0       51 2022-01-16 16:08:56.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/postgresql/__init__.py
+-rw-rw-rw-   0        0        0     5225 2022-02-13 19:24:18.000000 pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.634200 pdip-0.6.6/pdip/integrator/connection/types/webservice/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.706202 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:17.839203 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/source/
+-rw-rw-rw-   0        0        0       65 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/source/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:18.049201 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/target/
+-rw-rw-rw-   0        0        0       65 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/target/__init__.py
+-rw-rw-rw-   0        0        0     3434 2022-07-05 16:44:50.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:18.588202 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/
+-rw-rw-rw-   0        0        0      212 2022-01-12 07:24:26.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/__init__.py
+-rw-rw-rw-   0        0        0      540 2022-01-12 07:24:26.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_connector.py
+-rw-rw-rw-   0        0        0     1779 2022-02-13 20:47:39.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_context.py
+-rw-rw-rw-   0        0        0     1061 2022-02-13 20:47:39.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_policy.py
+-rw-rw-rw-   0        0        0     1991 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_provider.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:18.691202 pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:18.842204 pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/soap/
+-rw-rw-rw-   0        0        0       43 2022-01-12 08:15:22.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/soap/__init__.py
+-rw-rw-rw-   0        0        0     2122 2022-02-13 09:09:10.000000 pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.001206 pdip-0.6.6/pdip/integrator/domain/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.206207 pdip-0.6.6/pdip/integrator/domain/enums/
+-rw-rw-rw-   0        0        0       39 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      437 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/domain/enums/events.py
+-rw-rw-rw-   0        0        0      120 2021-10-31 17:47:11.000000 pdip-0.6.6/pdip/integrator/domain/enums/status_types.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.360206 pdip-0.6.6/pdip/integrator/event/
+-rw-rw-rw-   0        0        0        0 2022-01-16 20:52:28.000000 pdip-0.6.6/pdip/integrator/event/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.803215 pdip-0.6.6/pdip/integrator/event/base/
+-rw-rw-rw-   0        0        0      216 2022-01-16 21:27:09.000000 pdip-0.6.6/pdip/integrator/event/base/__init__.py
+-rw-rw-rw-   0        0        0     3100 2022-01-16 21:11:05.000000 pdip-0.6.6/pdip/integrator/event/base/default_integrator_event_manager.py
+-rw-rw-rw-   0        0        0     1250 2022-01-16 21:11:05.000000 pdip-0.6.6/pdip/integrator/event/base/integrator_event_manager.py
+-rw-rw-rw-   0        0        0     1029 2022-02-04 03:16:01.000000 pdip-0.6.6/pdip/integrator/event/base/integrator_event_manager_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.870210 pdip-0.6.6/pdip/integrator/execution/
+-rw-rw-rw-   0        0        0        0 2022-01-16 20:11:55.000000 pdip-0.6.6/pdip/integrator/execution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:19.931212 pdip-0.6.6/pdip/integrator/execution/base/
+-rw-rw-rw-   0        0        0        2 2022-01-16 23:22:14.000000 pdip-0.6.6/pdip/integrator/execution/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.039206 pdip-0.6.6/pdip/integrator/execution/domain/
+-rw-rw-rw-   0        0        0      284 2022-01-16 20:23:45.000000 pdip-0.6.6/pdip/integrator/execution/domain/__init__.py
+-rw-rw-rw-   0        0        0     1080 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/execution/domain/execution.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.092208 pdip-0.6.6/pdip/integrator/initializer/
+-rw-rw-rw-   0        0        0        0 2022-01-16 20:57:53.000000 pdip-0.6.6/pdip/integrator/initializer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.204211 pdip-0.6.6/pdip/integrator/initializer/base/
+-rw-rw-rw-   0        0        0       38 2022-01-16 23:22:14.000000 pdip-0.6.6/pdip/integrator/initializer/base/__init__.py
+-rw-rw-rw-   0        0        0       60 2022-01-16 22:25:18.000000 pdip-0.6.6/pdip/integrator/initializer/base/initializer.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.256209 pdip-0.6.6/pdip/integrator/initializer/execution/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.497209 pdip-0.6.6/pdip/integrator/initializer/execution/base/
+-rw-rw-rw-   0        0        0      129 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/base/__init__.py
+-rw-rw-rw-   0        0        0     1457 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/base/default_execution_initializer.py
+-rw-rw-rw-   0        0        0      386 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/base/execution_initializer.py
+-rw-rw-rw-   0        0        0     1013 2022-02-04 03:16:01.000000 pdip-0.6.6/pdip/integrator/initializer/execution/base/execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:20.753207 pdip-0.6.6/pdip/integrator/initializer/execution/integration/
+-rw-rw-rw-   0        0        0      327 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/integration/__init__.py
+-rw-rw-rw-   0        0        0      533 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py
+-rw-rw-rw-   0        0        0      331 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer.py
+-rw-rw-rw-   0        0        0     1217 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.274211 pdip-0.6.6/pdip/integrator/initializer/execution/operation/
+-rw-rw-rw-   0        0        0      258 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/operation/__init__.py
+-rw-rw-rw-   0        0        0      431 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/operation/default_operation_execution_initializer.py
+-rw-rw-rw-   0        0        0      275 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/execution/operation/operation_execution_initializer.py
+-rw-rw-rw-   0        0        0     1127 2022-02-04 03:16:01.000000 pdip-0.6.6/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.557209 pdip-0.6.6/pdip/integrator/initializer/integrator/
+-rw-rw-rw-   0        0        0      207 2022-01-17 01:06:27.000000 pdip-0.6.6/pdip/integrator/initializer/integrator/__init__.py
+-rw-rw-rw-   0        0        0     3286 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/initializer/integrator/default_integrator_initializer.py
+-rw-rw-rw-   0        0        0      469 2022-01-25 06:28:03.000000 pdip-0.6.6/pdip/integrator/initializer/integrator/integrator_initializer.py
+-rw-rw-rw-   0        0        0     1019 2022-02-04 03:16:01.000000 pdip-0.6.6/pdip/integrator/initializer/integrator/integrator_initializer_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.601208 pdip-0.6.6/pdip/integrator/integration/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.707213 pdip-0.6.6/pdip/integrator/integration/base/
+-rw-rw-rw-   0        0        0       57 2022-01-16 23:22:14.000000 pdip-0.6.6/pdip/integrator/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3845 2022-02-13 16:15:29.000000 pdip-0.6.6/pdip/integrator/integration/base/integration_execution.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.820214 pdip-0.6.6/pdip/integrator/integration/domain/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/integration/domain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:21.909209 pdip-0.6.6/pdip/integrator/integration/domain/base/
+-rw-rw-rw-   0        0        0       94 2022-02-10 15:34:05.000000 pdip-0.6.6/pdip/integrator/integration/domain/base/__init__.py
+-rw-rw-rw-   0        0        0     1031 2022-02-13 20:47:39.000000 pdip-0.6.6/pdip/integrator/integration/domain/base/integration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.137213 pdip-0.6.6/pdip/integrator/integration/domain/enums/
+-rw-rw-rw-   0        0        0       49 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/integration/domain/enums/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/domain/enums/integration_types.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.183209 pdip-0.6.6/pdip/integrator/integration/types/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.485210 pdip-0.6.6/pdip/integrator/integration/types/base/
+-rw-rw-rw-   0        0        0      121 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/base/__init__.py
+-rw-rw-rw-   0        0        0      728 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/base/integration_adapter.py
+-rw-rw-rw-   0        0        0     1845 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/base/integration_adapter_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.564210 pdip-0.6.6/pdip/integrator/integration/types/source/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/source/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.653217 pdip-0.6.6/pdip/integrator/integration/types/source/base/
+-rw-rw-rw-   0        0        0       51 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/integration/types/source/base/__init__.py
+-rw-rw-rw-   0        0        0     5127 2022-02-26 13:30:17.000000 pdip-0.6.6/pdip/integrator/integration/types/source/base/source_integration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.701211 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.799211 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/base/
+-rw-rw-rw-   0        0        0       69 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/base/__init__.py
+-rw-rw-rw-   0        0        0     6664 2022-02-13 17:38:52.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.845208 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/
+-rw-rw-rw-   0        0        0        0 2022-02-13 17:38:52.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:22.983214 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/base/
+-rw-rw-rw-   0        0        0      101 2022-02-13 17:38:52.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/base/__init__.py
+-rw-rw-rw-   0        0        0      537 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.167212 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/factories/
+-rw-rw-rw-   0        0        0       99 2022-02-13 20:47:39.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/factories/__init__.py
+-rw-rw-rw-   0        0        0     1723 2022-02-26 08:16:34.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.231210 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/
+-rw-rw-rw-   0        0        0        0 2022-02-13 17:30:21.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.340211 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/
+-rw-rw-rw-   0        0        0       70 2022-02-13 17:38:52.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/__init__.py
+-rw-rw-rw-   0        0        0    18820 2022-02-13 17:40:40.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.416212 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/
+-rw-rw-rw-   0        0        0        0 2022-02-13 17:30:21.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.516216 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/
+-rw-rw-rw-   0        0        0       83 2022-02-26 08:16:34.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/__init__.py
+-rw-rw-rw-   0        0        0     7431 2022-02-28 06:09:14.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:23.619210 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/
+-rw-rw-rw-   0        0        0        0 2022-02-26 07:23:54.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:24.721218 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/
+-rw-rw-rw-   0        0        0       56 2022-02-28 06:09:14.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/__init__.py
+-rw-rw-rw-   0        0        0     4368 2022-02-26 08:27:28.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:24.838214 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/
+-rw-rw-rw-   0        0        0       58 2022-02-28 06:09:14.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/__init__.py
+-rw-rw-rw-   0        0        0     8709 2022-02-26 09:01:27.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:24.935212 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/
+-rw-rw-rw-   0        0        0        0 2022-02-26 07:23:54.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.122214 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/
+-rw-rw-rw-   0        0        0      105 2022-02-26 07:36:10.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/__init__.py
+-rw-rw-rw-   0        0        0     7222 2022-02-26 08:16:34.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py
+-rw-rw-rw-   0        0        0     3887 2022-02-26 08:16:34.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.283216 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/
+-rw-rw-rw-   0        0        0       74 2022-02-13 22:42:38.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/__init__.py
+-rw-rw-rw-   0        0        0      144 2022-02-13 22:42:38.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_info.py
+-rw-rw-rw-   0        0        0      304 2022-02-13 22:42:37.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/domain/thread_task.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.451213 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/
+-rw-rw-rw-   0        0        0       75 2022-02-26 07:36:10.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/__init__.py
+-rw-rw-rw-   0        0        0      438 2022-02-26 07:36:10.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/factories/parallel_session_broker_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.505214 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/
+-rw-rw-rw-   0        0        0      166 2022-02-13 20:47:39.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.594213 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/
+-rw-rw-rw-   0        0        0       81 2022-02-13 17:38:52.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/__init__.py
+-rw-rw-rw-   0        0        0     3917 2022-02-13 17:41:31.000000 pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.663214 pdip-0.6.6/pdip/integrator/integration/types/target/
+-rw-rw-rw-   0        0        0        0 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/target/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.821220 pdip-0.6.6/pdip/integrator/integration/types/target/base/
+-rw-rw-rw-   0        0        0       51 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/target/base/__init__.py
+-rw-rw-rw-   0        0        0     2684 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/integration/types/target/base/target_integration.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:25.892213 pdip-0.6.6/pdip/integrator/operation/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/operation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.005217 pdip-0.6.6/pdip/integrator/operation/base/
+-rw-rw-rw-   0        0        0       53 2022-01-16 23:22:14.000000 pdip-0.6.6/pdip/integrator/operation/base/__init__.py
+-rw-rw-rw-   0        0        0     2325 2022-02-01 21:03:36.000000 pdip-0.6.6/pdip/integrator/operation/base/operation_execution.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.197215 pdip-0.6.6/pdip/integrator/operation/domain/
+-rw-rw-rw-   0        0        0       64 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/integrator/operation/domain/__init__.py
+-rw-rw-rw-   0        0        0      808 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/operation/domain/operation.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.242214 pdip-0.6.6/pdip/integrator/pubsub/
+-rw-rw-rw-   0        0        0        0 2022-01-02 19:32:28.000000 pdip-0.6.6/pdip/integrator/pubsub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.541220 pdip-0.6.6/pdip/integrator/pubsub/base/
+-rw-rw-rw-   0        0        0      183 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/pubsub/base/__init__.py
+-rw-rw-rw-   0        0        0      342 2022-01-03 13:30:44.000000 pdip-0.6.6/pdip/integrator/pubsub/base/channel_queue.py
+-rw-rw-rw-   0        0        0     1529 2022-01-06 18:31:38.000000 pdip-0.6.6/pdip/integrator/pubsub/base/event_listener.py
+-rw-rw-rw-   0        0        0     3040 2022-02-13 22:42:38.000000 pdip-0.6.6/pdip/integrator/pubsub/base/message_broker.py
+-rw-rw-rw-   0        0        0     1302 2022-02-13 22:42:38.000000 pdip-0.6.6/pdip/integrator/pubsub/base/message_broker_worker.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.635214 pdip-0.6.6/pdip/integrator/pubsub/domain/
+-rw-rw-rw-   0        0        0       34 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/pubsub/domain/__init__.py
+-rw-rw-rw-   0        0        0      168 2022-01-05 01:38:23.000000 pdip-0.6.6/pdip/integrator/pubsub/domain/message.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.726216 pdip-0.6.6/pdip/integrator/pubsub/publisher/
+-rw-rw-rw-   0        0        0       34 2022-02-13 20:47:19.000000 pdip-0.6.6/pdip/integrator/pubsub/publisher/__init__.py
+-rw-rw-rw-   0        0        0      252 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/integrator/pubsub/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.789213 pdip-0.6.6/pdip/integrator/pubsub/subscriber/
+-rw-rw-rw-   0        0        0        0 2022-01-01 12:02:58.000000 pdip-0.6.6/pdip/integrator/pubsub/subscriber/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:26.962216 pdip-0.6.6/pdip/io/
+-rw-rw-rw-   0        0        0       82 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/io/__init__.py
+-rw-rw-rw-   0        0        0     1011 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/io/file_manager.py
+-rw-rw-rw-   0        0        0     1326 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/io/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.018214 pdip-0.6.6/pdip/json/
+-rw-rw-rw-   0        0        0      320 2023-03-11 19:32:52.000000 pdip-0.6.6/pdip/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.292215 pdip-0.6.6/pdip/json/base/
+-rw-rw-rw-   0        0        0        0 2023-03-11 19:22:26.000000 pdip-0.6.6/pdip/json/base/__init__.py
+-rw-rw-rw-   0        0        0     3786 2023-03-11 19:32:52.000000 pdip-0.6.6/pdip/json/base/base_converter.py
+-rw-rw-rw-   0        0        0     1037 2023-03-11 20:00:23.000000 pdip-0.6.6/pdip/json/base/json_convert.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.530219 pdip-0.6.6/pdip/json/encoders/
+-rw-rw-rw-   0        0        0        0 2023-03-11 19:20:44.000000 pdip-0.6.6/pdip/json/encoders/__init__.py
+-rw-rw-rw-   0        0        0      311 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/json/encoders/date_time_encoder.py
+-rw-rw-rw-   0        0        0      734 2023-03-11 19:20:16.000000 pdip-0.6.6/pdip/json/encoders/mutliple_json_encoders.py
+-rw-rw-rw-   0        0        0      272 2023-03-11 19:20:17.000000 pdip-0.6.6/pdip/json/encoders/uuid_encoder.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.656218 pdip-0.6.6/pdip/json/parsers/
+-rw-rw-rw-   0        0        0        0 2023-03-11 19:21:45.000000 pdip-0.6.6/pdip/json/parsers/__init__.py
+-rw-rw-rw-   0        0        0      528 2022-01-12 10:33:46.000000 pdip-0.6.6/pdip/json/parsers/date_time_parser.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.691217 pdip-0.6.6/pdip/logging/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.771215 pdip-0.6.6/pdip/logging/domain/
+-rw-rw-rw-   0        0        0       31 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/domain/__init__.py
+-rw-rw-rw-   0        0        0      499 2022-01-04 08:12:15.000000 pdip-0.6.6/pdip/logging/domain/log_data.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.827219 pdip-0.6.6/pdip/logging/loggers/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:27.922217 pdip-0.6.6/pdip/logging/loggers/base/
+-rw-rw-rw-   0        0        0       30 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/loggers/base/__init__.py
+-rw-rw-rw-   0        0        0     1015 2022-02-13 20:47:19.000000 pdip-0.6.6/pdip/logging/loggers/base/ilogger.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.079216 pdip-0.6.6/pdip/logging/loggers/console/
+-rw-rw-rw-   0        0        0       43 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/loggers/console/__init__.py
+-rw-rw-rw-   0        0        0     1881 2022-01-03 21:37:05.000000 pdip-0.6.6/pdip/logging/loggers/console/console_logger.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.217217 pdip-0.6.6/pdip/logging/loggers/file/
+-rw-rw-rw-   0        0        0       37 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/loggers/file/__init__.py
+-rw-rw-rw-   0        0        0     1977 2022-02-13 20:47:18.000000 pdip-0.6.6/pdip/logging/loggers/file/file_logger.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.350220 pdip-0.6.6/pdip/logging/loggers/sql/
+-rw-rw-rw-   0        0        0       35 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/logging/loggers/sql/__init__.py
+-rw-rw-rw-   0        0        0     4728 2023-03-05 19:19:52.000000 pdip-0.6.6/pdip/logging/loggers/sql/sql_logger.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.392223 pdip-0.6.6/pdip/processing/
+-rw-rw-rw-   0        0        0       65 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.570218 pdip-0.6.6/pdip/processing/base/
+-rw-rw-rw-   0        0        0        0 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/base/__init__.py
+-rw-rw-rw-   0        0        0     7549 2022-02-13 20:47:40.000000 pdip-0.6.6/pdip/processing/base/process_manager.py
+-rw-rw-rw-   0        0        0     2430 2022-02-13 20:27:25.000000 pdip-0.6.6/pdip/processing/base/subprocess.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.727220 pdip-0.6.6/pdip/processing/factories/
+-rw-rw-rw-   0        0        0       60 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/factories/__init__.py
+-rw-rw-rw-   0        0        0      418 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/factories/process_manager_factory.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:28.884224 pdip-0.6.6/pdip/processing/models/
+-rw-rw-rw-   0        0        0       78 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/models/__init__.py
+-rw-rw-rw-   0        0        0      348 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/models/process_info.py
+-rw-rw-rw-   0        0        0      776 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/processing/models/process_task.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:29.115218 pdip-0.6.6/pdip/utils/
+-rw-rw-rw-   0        0        0      106 2021-12-24 11:05:16.000000 pdip-0.6.6/pdip/utils/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-03-11 21:00:07.000000 pdip-0.6.6/pdip/utils/module_finder.py
+-rw-rw-rw-   0        0        0     1531 2023-03-05 21:22:19.000000 pdip-0.6.6/pdip/utils/type_checker.py
+-rw-rw-rw-   0        0        0     2936 2023-02-07 07:53:51.000000 pdip-0.6.6/pdip/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-13 00:46:00.371108 pdip-0.6.6/pdip.egg-info/
+-rw-rw-rw-   0        0        0     1330 2023-03-13 00:45:53.000000 pdip-0.6.6/pdip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    21251 2023-03-13 00:45:55.000000 pdip-0.6.6/pdip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-13 00:45:53.000000 pdip-0.6.6/pdip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-13 00:45:53.000000 pdip-0.6.6/pdip.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      206 2023-03-13 00:45:53.000000 pdip-0.6.6/pdip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-03-13 00:45:53.000000 pdip-0.6.6/pdip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-03-13 00:46:29.238217 pdip-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     2190 2023-03-13 00:43:30.000000 pdip-0.6.6/setup.py
```

### Comparing `pdip-0.6.5/LICENSE` & `pdip-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/PKG-INFO` & `pdip-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdip
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Data Integrator infrastructures package
 Home-page: https://github.com/ahmetcagriakca/pdip
-Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.5.tar.gz
+Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.6.tar.gz
 Author: Ahmet Çağrı AKCA
 Author-email: ahmetcagriakca@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/issues
 Project-URL: Source, https://github.com/ahmetcagriakca/pdip
 Keywords: PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pdip Version: 0.6.5 Summary: Python Data Integrator
+Metadata-Version: 2.1 Name: pdip Version: 0.6.6 Summary: Python Data Integrator
 infrastructures package Home-page: https://github.com/ahmetcagriakca/pdip
 Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/
-v0.6.5.tar.gz Author: Ahmet ÃaÄrÄ± AKCA Author-email:
+v0.6.6.tar.gz Author: Ahmet ÃaÄrÄ± AKCA Author-email:
 ahmetcagriakca@gmail.com License: MIT Project-URL: Bug Reports, https://
 github.com/ahmetcagriakca/pdip/issues Project-URL: Source, https://github.com/
 ahmetcagriakca/pdip Keywords:
 PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `pdip-0.6.5/pdip/api/app/flask_app_wrapper.py` & `pdip-0.6.6/pdip/api/app/flask_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/base/controller_base.py` & `pdip-0.6.6/pdip/api/base/controller_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/base/endpoint_base.py` & `pdip-0.6.6/pdip/api/base/endpoint_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/base/endpoint_wrapper.py` & `pdip-0.6.6/pdip/api/base/endpoint_wrapper.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/converter/request_converter.py` & `pdip-0.6.6/pdip/api/converter/request_converter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/handlers/error_handlers.py` & `pdip-0.6.6/pdip/api/handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/handlers/request_handler.py` & `pdip-0.6.6/pdip/api/handlers/request_handler.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/specifications/order_by_specification.py` & `pdip-0.6.6/pdip/api/specifications/order_by_specification.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/api/specifications/paging_specification.py` & `pdip-0.6.6/pdip/api/specifications/paging_specification.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/base/pdi.py` & `pdip-0.6.6/pdip/base/pdi.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/configuration/config_manager.py` & `pdip-0.6.6/pdip/configuration/config_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/configuration/services/config_service.py` & `pdip-0.6.6/pdip/configuration/services/config_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/cqrs/decorators/cls_to_dict.py` & `pdip-0.6.6/pdip/cqrs/decorators/cls_to_dict.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/cqrs/dispatcher.py` & `pdip-0.6.6/pdip/cqrs/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/cqrs/generator/query_generator.py` & `pdip-0.6.6/pdip/cqrs/generator/query_generator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/cryptography/crypto_service.py` & `pdip-0.6.6/pdip/cryptography/crypto_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/base/database_session_manager.py` & `pdip-0.6.6/pdip/data/base/database_session_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/decorators/transaction_handler.py` & `pdip-0.6.6/pdip/data/decorators/transaction_handler.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/domain/entity.py` & `pdip-0.6.6/pdip/data/domain/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from .types import GUID
 
 
 class Entity(EntityBase):
     Id = Column(
         GUID(),
         primary_key=True,
-        default=str(uuid.uuid4())
+        default=lambda: str(uuid.uuid4())
     )
 
     @declared_attr
     def CreateUserId(cls):
         return Column(GUID(), index=False, unique=False, nullable=False,
-                      default=uuid.UUID("00000000-0000-0000-0000-000000000000"))
+                      default=lambda: uuid.UUID("00000000-0000-0000-0000-000000000000"))
 
     @declared_attr
     def CreateUserTime(cls):
-        return Column(DateTime, index=False, unique=False, nullable=False, default=datetime.now)
+        return Column(DateTime, index=False, unique=False, nullable=False, default=lambda: datetime.now)
 
     @declared_attr
     def UpdateUserId(cls):
         return Column(GUID(), index=False, unique=False, nullable=True)
 
     @declared_attr
     def UpdateUserTime(cls):
```

### Comparing `pdip-0.6.5/pdip/data/domain/entity_base.py` & `pdip-0.6.6/pdip/data/domain/entity_base.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/domain/types/GUID.py` & `pdip-0.6.6/pdip/data/domain/types/GUID.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/repository/repository.py` & `pdip-0.6.6/pdip/data/repository/repository.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/repository/repository_provider.py` & `pdip-0.6.6/pdip/data/repository/repository_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/data/seed/seed_runner.py` & `pdip-0.6.6/pdip/data/seed/seed_runner.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/delivery/email_provider.py` & `pdip-0.6.6/pdip/delivery/email_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/dependency/container/dependency_container.py` & `pdip-0.6.6/pdip/dependency/container/dependency_container.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/dependency/provider/api_provider.py` & `pdip-0.6.6/pdip/dependency/provider/api_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/dependency/provider/service_provider.py` & `pdip-0.6.6/pdip/dependency/provider/service_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/html/html_template_service.py` & `pdip-0.6.6/pdip/html/html_template_service.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/base/integrator.py` & `pdip-0.6.6/pdip/integrator/base/integrator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/base/connection_source_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/base/connection_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/base/connection_target_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/base/connection_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py` & `pdip-0.6.6/pdip/integrator/connection/domain/types/bigdata/configuration/base/big_data_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py` & `pdip-0.6.6/pdip/integrator/connection/domain/types/sql/configuration/base/sql_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py` & `pdip-0.6.6/pdip/integrator/connection/domain/types/webservice/configuration/base/web_service_connection_configuration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/factories/connection_source_adapter_factory.py` & `pdip-0.6.6/pdip/integrator/connection/factories/connection_source_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/factories/connection_target_adapter_factory.py` & `pdip-0.6.6/pdip/integrator/connection/factories/connection_target_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/source/big_data_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/adapters/target/big_data_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_iterator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_policy.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/base/big_data_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/base/big_data_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/connectors/impala/impala_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/bigdata/dialects/impala/impala_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/file/adapters/file_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/file/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/file/base/file_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/file/base/file_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/file/base/file_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/file/base/file_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/file/base/file_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/file/base/file_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/file/connectors/csv/csv_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py` & `pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/inmemory/base/in_memory_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/inmemory/connectors/sqlite/sq_lite_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/queue/adapters/queue_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/queue/adapters/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/queue/base/queue_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/queue/base/queue_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/queue/connectors/kafka_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/queue/connectors/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/source/sql_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/adapters/target/sql_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_iterator.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_iterator.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_policy.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/base/sql_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/base/sql_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/oracle/oracle_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/connectors/postgresql/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mssql/mssql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/mysql/mysql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/oracle/oracle_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py` & `pdip-0.6.6/pdip/integrator/connection/types/sql/dialects/postgresql/postgresql_dialect.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/source/web_service_source_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/adapters/target/web_service_target_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_context.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_context.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_policy.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_policy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/base/web_service_provider.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/base/web_service_provider.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py` & `pdip-0.6.6/pdip/integrator/connection/types/webservice/connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/event/base/default_integrator_event_manager.py` & `pdip-0.6.6/pdip/integrator/event/base/default_integrator_event_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/event/base/integrator_event_manager.py` & `pdip-0.6.6/pdip/integrator/event/base/integrator_event_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/event/base/integrator_event_manager_factory.py` & `pdip-0.6.6/pdip/integrator/event/base/integrator_event_manager_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/execution/domain/execution.py` & `pdip-0.6.6/pdip/integrator/execution/domain/execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/execution/base/default_execution_initializer.py` & `pdip-0.6.6/pdip/integrator/initializer/execution/base/default_execution_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/execution/base/execution_initializer_factory.py` & `pdip-0.6.6/pdip/integrator/initializer/execution/base/execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py` & `pdip-0.6.6/pdip/integrator/initializer/execution/integration/default_operation_integration_execution_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py` & `pdip-0.6.6/pdip/integrator/initializer/execution/integration/operation_integration_execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py` & `pdip-0.6.6/pdip/integrator/initializer/execution/operation/operation_execution_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/integrator/default_integrator_initializer.py` & `pdip-0.6.6/pdip/integrator/initializer/integrator/default_integrator_initializer.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/initializer/integrator/integrator_initializer_factory.py` & `pdip-0.6.6/pdip/integrator/initializer/integrator/integrator_initializer_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/base/integration_execution.py` & `pdip-0.6.6/pdip/integrator/integration/base/integration_execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/domain/base/integration.py` & `pdip-0.6.6/pdip/integrator/integration/domain/base/integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/base/integration_adapter.py` & `pdip-0.6.6/pdip/integrator/integration/types/base/integration_adapter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/base/integration_adapter_factory.py` & `pdip-0.6.6/pdip/integrator/integration/types/base/integration_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/source/base/source_integration.py` & `pdip-0.6.6/pdip/integrator/integration/types/source/base/source_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/base/source_to_target_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/base/integration_source_to_target_execute_strategy.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/factories/integration_execute_strategy_factory.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelold/base/parallel_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/base/parallel_thread_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/source/source_read_operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/operation/target/target_write_operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_session_broker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/parallelthread/threading/base/parallel_worker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py` & `pdip-0.6.6/pdip/integrator/integration/types/sourcetotarget/strategies/singleprocess/base/single_process_integration_execute.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/integration/types/target/base/target_integration.py` & `pdip-0.6.6/pdip/integrator/integration/types/target/base/target_integration.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/operation/base/operation_execution.py` & `pdip-0.6.6/pdip/integrator/operation/base/operation_execution.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/operation/domain/operation.py` & `pdip-0.6.6/pdip/integrator/operation/domain/operation.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/pubsub/base/event_listener.py` & `pdip-0.6.6/pdip/integrator/pubsub/base/event_listener.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/pubsub/base/message_broker.py` & `pdip-0.6.6/pdip/integrator/pubsub/base/message_broker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/integrator/pubsub/base/message_broker_worker.py` & `pdip-0.6.6/pdip/integrator/pubsub/base/message_broker_worker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/io/file_manager.py` & `pdip-0.6.6/pdip/io/file_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/io/folder_manager.py` & `pdip-0.6.6/pdip/io/folder_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/json/base/base_converter.py` & `pdip-0.6.6/pdip/json/base/base_converter.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/json/base/json_convert.py` & `pdip-0.6.6/pdip/json/base/json_convert.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/json/encoders/mutliple_json_encoders.py` & `pdip-0.6.6/pdip/json/encoders/mutliple_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/json/parsers/date_time_parser.py` & `pdip-0.6.6/pdip/json/parsers/date_time_parser.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/logging/loggers/base/ilogger.py` & `pdip-0.6.6/pdip/logging/loggers/base/ilogger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/logging/loggers/console/console_logger.py` & `pdip-0.6.6/pdip/logging/loggers/console/console_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/logging/loggers/file/file_logger.py` & `pdip-0.6.6/pdip/logging/loggers/file/file_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/logging/loggers/sql/sql_logger.py` & `pdip-0.6.6/pdip/logging/loggers/sql/sql_logger.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/processing/base/process_manager.py` & `pdip-0.6.6/pdip/processing/base/process_manager.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/processing/base/subprocess.py` & `pdip-0.6.6/pdip/processing/base/subprocess.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/processing/models/process_task.py` & `pdip-0.6.6/pdip/processing/models/process_task.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/utils/module_finder.py` & `pdip-0.6.6/pdip/utils/module_finder.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/utils/type_checker.py` & `pdip-0.6.6/pdip/utils/type_checker.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip/utils/utils.py` & `pdip-0.6.6/pdip/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/pdip.egg-info/PKG-INFO` & `pdip-0.6.6/pdip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdip
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python Data Integrator infrastructures package
 Home-page: https://github.com/ahmetcagriakca/pdip
-Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.5.tar.gz
+Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/v0.6.6.tar.gz
 Author: Ahmet Çağrı AKCA
 Author-email: ahmetcagriakca@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/ahmetcagriakca/pdip/issues
 Project-URL: Source, https://github.com/ahmetcagriakca/pdip
 Keywords: PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pdip Version: 0.6.5 Summary: Python Data Integrator
+Metadata-Version: 2.1 Name: pdip Version: 0.6.6 Summary: Python Data Integrator
 infrastructures package Home-page: https://github.com/ahmetcagriakca/pdip
 Download-URL: https://github.com/ahmetcagriakca/pdip/archive/refs/tags/
-v0.6.5.tar.gz Author: Ahmet ÃaÄrÄ± AKCA Author-email:
+v0.6.6.tar.gz Author: Ahmet ÃaÄrÄ± AKCA Author-email:
 ahmetcagriakca@gmail.com License: MIT Project-URL: Bug Reports, https://
 github.com/ahmetcagriakca/pdip/issues Project-URL: Source, https://github.com/
 ahmetcagriakca/pdip Keywords:
 PDI,API,ETL,PROCESS,MULTIPROCESS,IO,CQRS,MSSQL,ORACLE,POSTGRES,MYSQL,CSV
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `pdip-0.6.5/pdip.egg-info/SOURCES.txt` & `pdip-0.6.6/pdip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdip-0.6.5/setup.py` & `pdip-0.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 here = Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
-env_version = getenv('PYPI_PACKAGE_VERSION', default='0.6.5')
+env_version = getenv('PYPI_PACKAGE_VERSION', default='0.6.6')
 version = env_version.replace('v', '')
 setup(
     name='pdip',
     version=f'{version}',
     description='Python Data Integrator infrastructures package',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

