# Comparing `tmp/logfire-0.28.3.tar.gz` & `tmp/logfire-0.29.0.tar.gz`

## Comparing `logfire-0.28.3.tar` & `logfire-0.29.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 logfire-0.28.3/Makefile
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    54491 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/config.py
--rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/constants.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    53273 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/main.py
--rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 logfire-0.28.3/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/__init__.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_backfill.py
--rw-r--r--   0        0        0    44869 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_configure.py
--rw-r--r--   0        0        0    24220 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_formatter.py
--rw-r--r--   0        0        0    45084 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0    67482 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_logfire.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_loguru.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_no_production.py
--rw-r--r--   0        0        0    53664 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_structlog.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    40124 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    42460 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.28.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.28.3/LICENSE
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 logfire-0.28.3/README.md
--rw-r--r--   0        0        0     8345 2020-02-02 00:00:00.000000 logfire-0.28.3/pyproject.toml
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 logfire-0.28.3/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.29.0/Makefile
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    54920 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    12882 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    53273 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    17685 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0    11380 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/openai.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    18711 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 logfire-0.29.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/__init__.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    18741 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    44869 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    51315 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_configure.py
+-rw-r--r--   0        0        0    24810 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45507 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0    67482 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_loguru.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    53664 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     7334 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    40300 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    42320 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.29.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.29.0/LICENSE
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 logfire-0.29.0/README.md
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 logfire-0.29.0/pyproject.toml
+-rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 logfire-0.29.0/PKG-INFO
```

### Comparing `logfire-0.28.3/Makefile` & `logfire-0.29.0/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 .PHONY: test  # Run the tests
 test:
 	rye run coverage run -m pytest
 
 .PHONY: testcov  # Run tests and generate a coverage report
 testcov: test
 	@echo "building coverage html"
-	@rye run coverage html
+	@rye run coverage html --show-contexts
 
 .PHONY: docs  # Build the documentation
 docs:
 	rye run docs
 
 .PHONY: docs-serve  # Build and serve the documentation
 docs-serve:
```

### Comparing `logfire-0.28.3/logfire/__init__.py` & `logfire-0.29.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/propagate.py` & `logfire-0.29.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/testing.py` & `logfire-0.29.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/ast_utils.py` & `logfire-0.29.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/async_.py` & `logfire-0.29.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/auth.py` & `logfire-0.29.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/backfill.py` & `logfire-0.29.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/cli.py` & `logfire-0.29.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/config.py` & `logfire-0.29.0/logfire/_internal/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from .collect_system_info import collect_package_info
 from .config_params import ParamManager, PydanticPluginRecordValues
 from .constants import (
     DEFAULT_FALLBACK_FILE_NAME,
     OTLP_MAX_BODY_SIZE,
     RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS,
     SUPPRESS_INSTRUMENTATION_CONTEXT_KEY,
+    LevelName,
 )
 from .exporters.console import (
     ConsoleColorsValues,
     IndentedConsoleSpanExporter,
     ShowParentsConsoleSpanExporter,
     SimpleConsoleSpanExporter,
 )
@@ -97,15 +98,22 @@
 class ConsoleOptions:
     """Options for controlling console output."""
 
     colors: ConsoleColorsValues = 'auto'
     span_style: Literal['simple', 'indented', 'show-parents'] = 'show-parents'
     """How spans are shown in the console."""
     include_timestamps: bool = True
+    """Whether to include timestamps in the console output."""
     verbose: bool = False
+    """Whether to show verbose output.
+
+    It includes the filename, log level, and line number.
+    """
+    min_log_level: LevelName = 'info'
+    """The minimum log level to show in the console."""
 
 
 @dataclass
 class PydanticPlugin:
     """Options for the Pydantic plugin."""
 
     record: PydanticPluginRecordValues = 'off'
@@ -364,14 +372,15 @@
             self.console = False
         else:
             self.console = ConsoleOptions(
                 colors=param_manager.load_param('console_colors'),
                 span_style=param_manager.load_param('console_span_style'),
                 include_timestamps=param_manager.load_param('console_include_timestamp'),
                 verbose=param_manager.load_param('console_verbose'),
+                min_log_level=param_manager.load_param('console_min_log_level'),
             )
 
         if isinstance(pydantic_plugin, dict):
             # This is particularly for deserializing from a dict as in executors.py
             pydantic_plugin = PydanticPlugin(**pydantic_plugin)  # type: ignore
         self.pydantic_plugin = pydantic_plugin or param_manager.pydantic_plugin
         self.fast_shutdown = fast_shutdown
@@ -582,14 +591,15 @@
                     exporter_cls = ShowParentsConsoleSpanExporter
                 add_span_processor(
                     SimpleSpanProcessor(
                         exporter_cls(
                             colors=self.console.colors,
                             include_timestamp=self.console.include_timestamps,
                             verbose=self.console.verbose,
+                            min_log_level=self.console.min_log_level,
                         ),
                     )
                 )
 
             metric_readers = self.metric_readers
 
             if (self.send_to_logfire == 'if-token-present' and self.token is not None) or self.send_to_logfire is True:
```

### Comparing `logfire-0.28.3/logfire/_internal/config_params.py` & `logfire-0.29.0/logfire/_internal/config_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_ENDPOINT, OTEL_SERVICE_NAME
 from typing_extensions import get_args, get_origin
 
 from logfire.exceptions import LogfireConfigError
 
 from . import config
-from .constants import LOGFIRE_BASE_URL
+from .constants import LOGFIRE_BASE_URL, LevelName
 from .exporters.console import ConsoleColorsValues
 from .utils import read_toml_file
 
 try:
     import opentelemetry.instrumentation.system_metrics  # noqa: F401 # type: ignore
 
     COLLECT_SYSTEM_METRICS_DEFAULT = True
@@ -77,14 +77,16 @@
 * `'indented'`: Spans are shown as a tree, indented based on how many parents they have.
 * `'show-parents'`: Spans are shown intended, when spans are interleaved parent spans are printed again to
   give the best context."""
 CONSOLE_INCLUDE_TIMESTAMP = ConfigParam(env_vars=['LOGFIRE_CONSOLE_INCLUDE_TIMESTAMP'], allow_file_config=True, default=True, tp=bool)
 """Whether to include the timestamp in the console."""
 CONSOLE_VERBOSE = ConfigParam(env_vars=['LOGFIRE_CONSOLE_VERBOSE'], allow_file_config=True, default=False, tp=bool)
 """Whether to log in verbose mode in the console."""
+CONSOLE_MIN_LOG_LEVEL = ConfigParam(env_vars=['LOGFIRE_CONSOLE_MIN_LOG_LEVEL'], allow_file_config=True, default='info', tp=LevelName)
+"""Minimum log level to show in the console."""
 PYDANTIC_PLUGIN_RECORD = ConfigParam(env_vars=['LOGFIRE_PYDANTIC_PLUGIN_RECORD'], allow_file_config=True, default='off', tp=PydanticPluginRecordValues)
 """Whether instrument Pydantic validation.."""
 PYDANTIC_PLUGIN_INCLUDE = ConfigParam(env_vars=['LOGFIRE_PYDANTIC_PLUGIN_INCLUDE'], allow_file_config=True, default=set(), tp=Set[str])
 """Set of items that should be included in Logfire Pydantic plugin instrumentation."""
 PYDANTIC_PLUGIN_EXCLUDE = ConfigParam(env_vars=['LOGFIRE_PYDANTIC_PLUGIN_EXCLUDE'], allow_file_config=True, default=set(), tp=Set[str])
 """Set of items that should be excluded from Logfire Pydantic plugin instrumentation."""
 TRACE_SAMPLE_RATE = ConfigParam(env_vars=['LOGFIRE_TRACE_SAMPLE_RATE', 'OTEL_TRACES_SAMPLER_ARG'], allow_file_config=True, default=1.0, tp=float)
@@ -103,14 +105,15 @@
     'data_dir': CREDENTIALS_DIR,
     'collect_system_metrics': COLLECT_SYSTEM_METRICS,
     'console': CONSOLE,
     'console_colors': CONSOLE_COLORS,
     'console_span_style': CONSOLE_SPAN_STYLE,
     'console_include_timestamp': CONSOLE_INCLUDE_TIMESTAMP,
     'console_verbose': CONSOLE_VERBOSE,
+    'console_min_log_level': CONSOLE_MIN_LOG_LEVEL,
     'pydantic_plugin_record': PYDANTIC_PLUGIN_RECORD,
     'pydantic_plugin_include': PYDANTIC_PLUGIN_INCLUDE,
     'pydantic_plugin_exclude': PYDANTIC_PLUGIN_EXCLUDE,
 }
 
 
 @dataclass
```

### Comparing `logfire-0.28.3/logfire/_internal/constants.py` & `logfire-0.29.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/formatter.py` & `logfire-0.29.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/instrument.py` & `logfire-0.29.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/json_encoder.py` & `logfire-0.29.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/json_formatter.py` & `logfire-0.29.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/json_schema.py` & `logfire-0.29.0/logfire/_internal/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     if obj_type in {list, tuple, set, frozenset, deque}:
         return _array_schema(obj, seen)
     elif isinstance(obj, Mapping):
         return _mapping_schema(obj, seen)
     elif is_sqlalchemy(obj):
         return _sqlalchemy_schema(obj, seen)
-    elif dataclasses.is_dataclass(obj):
+    elif dataclasses.is_dataclass(obj) and not isinstance(obj, type):
         return _dataclass_schema(obj, seen)
     elif is_attrs(obj):
         return _attrs_schema(obj, seen)
 
     global _type_to_schema
     _type_to_schema = _type_to_schema or type_to_schema()
     for base in obj_type.__mro__[:-1]:
```

### Comparing `logfire-0.28.3/logfire/_internal/json_types.py` & `logfire-0.29.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/main.py` & `logfire-0.29.0/logfire/_internal/main.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/metrics.py` & `logfire-0.29.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/scrubbing.py` & `logfire-0.29.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/stack_info.py` & `logfire-0.29.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/tracer.py` & `logfire-0.29.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/utils.py` & `logfire-0.29.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/auto_trace/__init__.py` & `logfire-0.29.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.29.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.29.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/auto_trace/types.py` & `logfire-0.29.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/exporters/console.py` & `logfire-0.29.0/logfire/_internal/exporters/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     ATTRIBUTES_PENDING_SPAN_REAL_PARENT_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     DISABLE_CONSOLE_KEY,
     LEVEL_NUMBERS,
     NUMBER_TO_LEVEL,
     ONE_SECOND_IN_NANOSECONDS,
+    LevelName,
 )
 from ..json_formatter import json_args_value_formatter
 
 ConsoleColorsValues = Literal['auto', 'always', 'never']
+_INFO_LEVEL = LEVEL_NUMBERS['info']
 _WARN_LEVEL = LEVEL_NUMBERS['warn']
 _ERROR_LEVEL = LEVEL_NUMBERS['error']
 
 # A list of (text, style) pairs that can be passed to rich's `Text.assemble`.
 # When logging without colors, just the text is used in a plain `print`.
 TextParts = List[Tuple[str, str]]
 
@@ -52,14 +54,15 @@
 
     def __init__(
         self,
         output: TextIO | None = None,
         colors: ConsoleColorsValues = 'auto',
         include_timestamp: bool = True,
         verbose: bool = False,
+        min_log_level: LevelName = 'info',
     ) -> None:
         self._output = output or sys.stdout
         if colors == 'auto':
             force_terminal = None
         else:
             force_terminal = colors == 'always'
         self._console = Console(
@@ -74,18 +77,23 @@
             # Use plain `print` to `self._output` instead of rich when we don't need colors
             self._console = None
 
         self._include_timestamp = include_timestamp
         # timestamp len('12:34:56.789') 12 + space (1)
         self._timestamp_indent = 13 if include_timestamp else 0
         self._verbose = verbose
+        self._min_log_level_num = LEVEL_NUMBERS[min_log_level]
 
     def export(self, spans: Sequence[ReadableSpan]) -> SpanExportResult:
         """Export the spans to the console."""
         for span in spans:
+            if span.attributes:  # pragma: no branch
+                log_level: int = span.attributes.get(ATTRIBUTES_LOG_LEVEL_NUM_KEY, _INFO_LEVEL)  # type: ignore
+                if log_level < self._min_log_level_num:
+                    continue
             self._log_span(span)
 
         return SpanExportResult.SUCCESS
 
     def _log_span(self, span: ReadableSpan) -> None:
         """Print a summary of the span, this method can be overridden to customize how spans are displayed.
 
@@ -261,16 +269,17 @@
 
     def __init__(
         self,
         output: TextIO | None = None,
         colors: ConsoleColorsValues = 'auto',
         include_timestamp: bool = True,
         verbose: bool = False,
+        min_log_level: LevelName = 'info',
     ) -> None:
-        super().__init__(output, colors, include_timestamp, verbose)
+        super().__init__(output, colors, include_timestamp, verbose, min_log_level)
         # lookup from span ID to indent level
         self._indent_level: dict[int, int] = {}
 
     def _log_span(self, span: ReadableSpan) -> None:
         """Get the span indent based on `self._indent_level`, then print the span with that indent."""
         attributes = span.attributes or {}
         span_type = attributes.get(ATTRIBUTES_SPAN_TYPE_KEY, 'span')
@@ -308,16 +317,17 @@
 
     def __init__(
         self,
         output: TextIO | None = None,
         colors: ConsoleColorsValues = 'auto',
         include_timestamp: bool = True,
         verbose: bool = False,
+        min_log_level: LevelName = 'info',
     ) -> None:
-        super().__init__(output, colors, include_timestamp, verbose)
+        super().__init__(output, colors, include_timestamp, verbose, min_log_level)
 
         # lookup from span_id to `(indent, span message, parent id)`
         self._span_history: dict[int, tuple[int, str, int]] = {}
         # current open span ids
         self._span_stack: list[int] = []
 
     def _log_span(self, span: ReadableSpan) -> None:
```

### Comparing `logfire-0.28.3/logfire/_internal/exporters/fallback.py` & `logfire-0.29.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/exporters/file.py` & `logfire-0.29.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/exporters/otlp.py` & `logfire-0.29.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.29.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from urllib.parse import parse_qs, urlparse
 
 from opentelemetry import context
 from opentelemetry.sdk.trace import ReadableSpan, Span, SpanProcessor
+from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.semconv.trace import SpanAttributes
 
 from ..constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     PENDING_SPAN_NAME_SUFFIX,
@@ -31,80 +32,79 @@
     def on_start(
         self,
         span: Span,
         parent_context: context.Context | None = None,
     ) -> None:
         if context.get_value('suppress_instrumentation'):  # pragma: no cover
             return
+        _set_log_level_on_asgi_send_receive_spans(span)
         self.processor.on_start(span, parent_context)
 
     def on_end(self, span: ReadableSpan) -> None:
         if context.get_value('suppress_instrumentation'):  # pragma: no cover
             return
         span_dict = span_to_dict(span)
-        _tweak_asgi_send_recieve_spans(span_dict)
+        _tweak_asgi_send_receive_spans(span_dict)
         _tweak_http_spans(span_dict)
         self.scrubber.scrub_span(span_dict)
         span = ReadableSpan(**span_dict)
         self.processor.on_end(span)
 
     def shutdown(self) -> None:
         self.processor.shutdown()
 
     def force_flush(self, timeout_millis: int = 30000) -> bool:
         return self.processor.force_flush(timeout_millis)  # pragma: no cover
 
 
-def _tweak_asgi_send_recieve_spans(span: ReadableSpanDict):
-    """Make the name/message/level of spans generated by OTEL's ASGI middleware more useful.
+def _set_log_level_on_asgi_send_receive_spans(span: Span) -> None:
+    """Set the log level of ASGI send/receive spans to debug.
+
+    If a span doesn't have a level set, it defaults to 'info'. This is too high for ASGI send/receive spans,
+    which are generated for every request and are not particularly interesting.
+    """
+    if _is_asgi_send_receive_span(span.name, span.instrumentation_scope):
+        span.set_attributes(log_level_attributes('debug'))
+
+
+def _tweak_asgi_send_receive_spans(span: ReadableSpanDict) -> None:
+    """Make the name/message of spans generated by OTEL's ASGI middleware more useful.
 
     For example, a single request will typically generate two 'send' spans with the same message,
     e.g. 'GET /foo http send'. This function may add part of the ASGI event type to the name to make it more useful,
     so instead it shows e.g. 'http send response.start' and 'http send response.body'.
-
-    The log level of these spans is also set to debug, as they are not usually interesting to the user.
     """
-    instrumentation_scope = span['instrumentation_scope']
-    if not (instrumentation_scope and instrumentation_scope.name == 'opentelemetry.instrumentation.asgi'):
-        return
-
-    if not (name := span['name']).endswith(
-        (
-            ' http send',
-            ' http receive',
-            ' websocket send',
-            ' websocket receive',
-        )
-    ):
-        return
-
-    attributes = span['attributes']
-    # The attribute name should be `asgi.event.type` after this is merged and released:
-    # https://github.com/open-telemetry/opentelemetry-python-contrib/pull/2300
-    typ = attributes.get('asgi.event.type') or attributes.get('type')
-    if not (
-        isinstance(typ, str)
-        and typ.startswith(('http.', 'websocket.'))
-        and attributes.get(ATTRIBUTES_MESSAGE_KEY) == name
-    ):  # pragma: no cover
-        return
-
-    # Strip the 'http.' or 'websocket.' prefix from the event type and add it to the span name.
-    if typ in ('websocket.send', 'websocket.receive'):
-        # No point in adding anything in this case, otherwise it'd say e.g. 'websocket send send'.
-        # No other event types in https://asgi.readthedocs.io/en/latest/specs/www.html are redundant like this.
-        new_name = name
-    else:
-        span['name'] = new_name = f'{name} {typ.split(".", 1)[1]}'
-
-    span['attributes'] = {
-        **attributes,
-        ATTRIBUTES_MESSAGE_KEY: new_name,
-        **log_level_attributes('debug'),
-    }
+    name = span['name']
+    if _is_asgi_send_receive_span(name, span['instrumentation_scope']):
+        attributes = span['attributes']
+        # The attribute name should be `asgi.event.type` after this is merged and released:
+        # https://github.com/open-telemetry/opentelemetry-python-contrib/pull/2300
+        typ = attributes.get('asgi.event.type') or attributes.get('type')
+        if not (
+            isinstance(typ, str)
+            and typ.startswith(('http.', 'websocket.'))
+            and attributes.get(ATTRIBUTES_MESSAGE_KEY) == name
+        ):  # pragma: no cover
+            return
+
+        # Strip the 'http.' or 'websocket.' prefix from the event type and add it to the span name.
+        if typ in ('websocket.send', 'websocket.receive'):
+            # No point in adding anything in this case, otherwise it'd say e.g. 'websocket send send'.
+            # No other event types in https://asgi.readthedocs.io/en/latest/specs/www.html are redundant like this.
+            new_name = name
+        else:
+            span['name'] = new_name = f'{name} {typ.split(".", 1)[1]}'
+
+        span['attributes'] = {**attributes, ATTRIBUTES_MESSAGE_KEY: new_name}
+
+
+def _is_asgi_send_receive_span(name: str, instrumentation_scope: InstrumentationScope | None) -> bool:
+    return (
+        instrumentation_scope is not None and instrumentation_scope.name == 'opentelemetry.instrumentation.asgi'
+    ) and (name.endswith((' http send', ' http receive', ' websocket send', ' websocket receive')))
 
 
 def _tweak_http_spans(span: ReadableSpanDict):
     """Tweak spans from HTTP instrumentations, particularly the span name and message.
 
     Also derives `http.target` from `http.url` if needed.
```

### Comparing `logfire-0.28.3/logfire/_internal/exporters/remove_pending.py` & `logfire-0.29.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/exporters/wrapper.py` & `logfire-0.29.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/integrations/executors.py` & `logfire-0.29.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/integrations/fastapi.py` & `logfire-0.29.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/_internal/integrations/openai.py` & `logfire-0.29.0/logfire/_internal/integrations/openai.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,54 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, ContextManager, Iterator, NamedTuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncIterator,
+    Callable,
+    ContextManager,
+    Generic,
+    Iterator,
+    NamedTuple,
+    TypeVar,
+    cast,
+)
 
 import openai
+from openai._legacy_response import LegacyAPIResponse
+from openai.types.chat.chat_completion import ChatCompletion
+from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
+from openai.types.completion import Completion
+from openai.types.create_embedding_response import CreateEmbeddingResponse
+from openai.types.images_response import ImagesResponse
 from opentelemetry import context
 
 if TYPE_CHECKING:
     from openai._models import FinalRequestOptions
     from openai._streaming import AsyncStream, Stream
-    from openai.types.chat.chat_completion import ChatCompletion
-    from openai.types.completion import Completion
-    from openai.types.create_embedding_response import CreateEmbeddingResponse
-    from openai.types.images_response import ImagesResponse
-    from typing_extensions import LiteralString
+    from openai._types import ResponseT
+    from typing_extensions import LiteralString, TypedDict, Unpack
 
     from ..main import Logfire, LogfireSpan
 
+    # The following typevars are used to use a generic type in the `OpenAIRequest` TypedDict for the sync and async flavors
+    _AsyncStreamT = TypeVar('_AsyncStreamT', bound=AsyncStream[Any])
+    _StreamT = TypeVar('_StreamT', bound=Stream[Any])
+
+    _ResponseType = TypeVar('_ResponseType')
+    _StreamType = TypeVar('_StreamType')
+
+    class OpenAIRequest(TypedDict, Generic[_ResponseType, _StreamType]):
+        cast_to: type[_ResponseType]
+        options: FinalRequestOptions
+        remaining_retries: int | None
+        stream: bool
+        stream_cls: type[_StreamType] | None
+
 
 __all__ = ('instrument_openai',)
 
 
 def instrument_openai(
     logfire: Logfire, client: openai.OpenAI | openai.AsyncOpenAI, suppress_otel: bool
 ) -> ContextManager[None]:
@@ -55,190 +83,188 @@
 STEAMING_MSG_TEMPLATE: LiteralString = 'streaming response from {request_data[model]!r}'
 
 
 def instrument_openai_sync(logfire_openai: Logfire, openai_client: openai.OpenAI, suppress_otel: bool) -> None:
     # WARNING: this method is vey similar to `instrument_openai_async` below, any changes here should be reflected there
     openai_client._original_request_method = original_request_method = openai_client._request  # type: ignore
 
-    def instrumented_openai_request(**kwargs: Any) -> Any:
+    def instrumented_openai_request(**kwargs: Unpack[OpenAIRequest[ResponseT, _StreamT]]) -> ResponseT | _StreamT:
         if context.get_value('suppress_instrumentation'):
             return original_request_method(**kwargs)
 
-        options: FinalRequestOptions | None = kwargs.get('options')
+        options = kwargs['options']
         try:
-            message_template, span_data, on_response, content_from_stream = get_endpoint_config(options)
+            message_template, span_data, content_from_stream = get_endpoint_config(options)
         except ValueError as exc:
             logfire_openai.warn('Unable to instrument OpenAI API call: {error}', error=str(exc), kwargs=kwargs)
             return original_request_method(**kwargs)
 
         span_data['async'] = False
-        stream = bool(kwargs.get('stream'))
+        stream = kwargs['stream']
 
         if stream and content_from_stream:
-            stream_cls: type[Stream] | None = kwargs.get('stream_cls')  # type: ignore[reportMissingTypeArgument]
+            stream_cls = kwargs['stream_cls']
             assert stream_cls is not None, 'Expected `stream_cls` when streaming'
 
             class LogfireInstrumentedStream(stream_cls):
                 def __stream__(self) -> Iterator[Any]:
                     content: list[str] = []
                     with logfire_openai.span(STEAMING_MSG_TEMPLATE, **span_data) as stream_span:
                         with maybe_suppress_instrumentation(suppress_otel):
-                            for chunk in super().__stream__():  # type: ignore
+                            for chunk in super().__stream__():
                                 chunk_content = content_from_stream(chunk)
                                 if chunk_content is not None:
                                     content.append(chunk_content)
                                 yield chunk
                             stream_span.set_attribute(
                                 'response_data',
                                 {'combined_chunk_content': ''.join(content), 'chunk_count': len(content)},
                             )
 
-            kwargs['stream_cls'] = LogfireInstrumentedStream
+            kwargs['stream_cls'] = LogfireInstrumentedStream  # type: ignore
 
         with logfire_openai.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
                     return original_request_method(**kwargs)
                 else:
-                    response = original_request_method(**kwargs)
-                    on_response(response, span)
+                    response = on_response(original_request_method(**kwargs), span)
                     return response
 
     openai_client._request = instrumented_openai_request  # type: ignore
 
 
 def instrument_openai_async(logfire_openai: Logfire, openai_client: openai.AsyncOpenAI, suppress_otel: bool) -> None:
     # WARNING: this method is vey similar to `instrument_openai_sync` above, any changes here should be reflected there
     openai_client._original_request_method = original_request_method = openai_client._request  # type: ignore
 
-    async def instrumented_openai_request(**kwargs: Any) -> Any:
+    async def instrumented_openai_request(
+        **kwargs: Unpack[OpenAIRequest[ResponseT, _AsyncStreamT]],
+    ) -> ResponseT | _AsyncStreamT:
         if context.get_value('suppress_instrumentation'):
             return await original_request_method(**kwargs)
 
-        options: FinalRequestOptions | None = kwargs.get('options')
+        options = kwargs['options']
         try:
-            message_template, span_data, on_response, content_from_stream = get_endpoint_config(options)
+            message_template, span_data, content_from_stream = get_endpoint_config(options)
         except ValueError as exc:
             logfire_openai.warn('Unable to instrument OpenAI API call: {error}', error=str(exc), kwargs=kwargs)
             return await original_request_method(**kwargs)
 
         span_data['async'] = True
-        stream = bool(kwargs.get('stream'))
+        stream = kwargs['stream']
 
         if stream and content_from_stream:
-            stream_cls: type[AsyncStream] | None = kwargs.get('stream_cls')  # type: ignore[reportMissingTypeArgument]
+            stream_cls = kwargs['stream_cls']
             assert stream_cls is not None, 'Expected `stream_cls` when streaming'
 
             class LogfireInstrumentedStream(stream_cls):
                 async def __stream__(self) -> AsyncIterator[Any]:
                     content: list[str] = []
                     with logfire_openai.span(STEAMING_MSG_TEMPLATE, **span_data) as stream_span:
                         with maybe_suppress_instrumentation(suppress_otel):
-                            async for chunk in super().__stream__():  # type: ignore
+                            async for chunk in super().__stream__():
                                 chunk_content = content_from_stream(chunk)
                                 if chunk_content is not None:
                                     content.append(chunk_content)
                                 yield chunk
                             stream_span.set_attribute(
                                 'response_data',
                                 {'combined_chunk_content': ''.join(content), 'chunk_count': len(content)},
                             )
 
-            kwargs['stream_cls'] = LogfireInstrumentedStream
+            kwargs['stream_cls'] = LogfireInstrumentedStream  # type: ignore
 
         with logfire_openai.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
                     return await original_request_method(**kwargs)
                 else:
-                    response = await original_request_method(**kwargs)
-                    on_response(response, span)
+                    response = on_response(await original_request_method(**kwargs), span)
                     return response
 
     openai_client._request = instrumented_openai_request  # type: ignore
 
 
 class EndpointConfig(NamedTuple):
     message_template: LiteralString
     span_data: dict[str, Any]
-    on_response: Callable[[Any, LogfireSpan], None]
     content_from_stream: Callable[[Any], str | None] | None
 
 
-def get_endpoint_config(options: FinalRequestOptions | None) -> EndpointConfig:
-    if options is None:
-        raise ValueError('`options` is required')
+def get_endpoint_config(options: FinalRequestOptions) -> EndpointConfig:
     url = options.url
     json_data = options.json_data
     if not isinstance(json_data, dict):
         raise ValueError('Expected `options.json_data` to be a dictionary')
     if 'model' not in json_data:
         # all OpenAI API calls have a model AFAIK
         raise ValueError('`model` not found in request data')
 
     if url == '/chat/completions':
         return EndpointConfig(
             message_template='Chat Completion with {request_data[model]!r}',
             span_data={'request_data': json_data},
-            on_response=on_chat_response,
-            content_from_stream=lambda chunk: chunk.choices[0].delta.content if chunk and chunk.choices else None,
+            content_from_stream=content_from_chat_completions,
         )
     elif url == '/completions':
         return EndpointConfig(
             message_template='Completion with {request_data[model]!r}',
             span_data={'request_data': json_data},
-            on_response=on_completion_response,
-            content_from_stream=lambda chunk: chunk.choices[0].text if chunk and chunk.choices else None,
+            content_from_stream=content_from_completions,
         )
     elif url == '/embeddings':
         return EndpointConfig(
             message_template='Embedding Creation with {request_data[model]!r}',
             span_data={'request_data': json_data},
-            on_response=on_embedding_response,
             content_from_stream=None,
         )
     elif url == '/images/generations':
         return EndpointConfig(
             message_template='Image Generation with {request_data[model]!r}',
             span_data={'request_data': json_data},
-            on_response=on_image_response,
             content_from_stream=None,
         )
     else:
         raise ValueError(f'Unknown OpenAI API endpoint: `{url}`')
 
 
-def on_chat_response(response: ChatCompletion, span: LogfireSpan) -> None:
-    span.set_attribute(
-        'response_data',
-        {
-            'message': response.choices[0].message,
-            'usage': response.usage,
-        },
-    )
-
-
-def on_completion_response(response: Completion, span: LogfireSpan) -> None:
-    first_choice = response.choices[0]
-    span.set_attribute(
-        'response_data',
-        {
-            'finish_reason': first_choice.finish_reason,
-            'text': first_choice.text,
-            'usage': response.usage,
-        },
-    )
-
-
-def on_embedding_response(response: CreateEmbeddingResponse, span: LogfireSpan) -> None:
-    span.set_attribute('response_data', {'usage': response.usage})
-
-
-def on_image_response(response: ImagesResponse, span: LogfireSpan) -> None:
-    span.set_attribute('response_data', {'images': response.data})
+def content_from_completions(chunk: Completion | None) -> str | None:
+    if chunk and chunk.choices:
+        return chunk.choices[0].text
+    return None  # pragma: no cover
+
+
+def content_from_chat_completions(chunk: ChatCompletionChunk | None) -> str | None:
+    if chunk and chunk.choices:
+        return chunk.choices[0].delta.content
+    return None
+
+
+def on_response(response: ResponseT, span: LogfireSpan) -> ResponseT:
+    if isinstance(response, LegacyAPIResponse):  # pragma: no cover
+        on_response(response.parse(), span)  # type: ignore
+        return cast('ResponseT', response)
+
+    if isinstance(response, ChatCompletion):
+        span.set_attribute(
+            'response_data',
+            {'message': response.choices[0].message, 'usage': response.usage},
+        )
+    elif isinstance(response, Completion):
+        first_choice = response.choices[0]
+        span.set_attribute(
+            'response_data',
+            {'finish_reason': first_choice.finish_reason, 'text': first_choice.text, 'usage': response.usage},
+        )
+    elif isinstance(response, CreateEmbeddingResponse):
+        span.set_attribute('response_data', {'usage': response.usage})
+    elif isinstance(response, ImagesResponse):  # pragma: no branch
+        span.set_attribute('response_data', {'images': response.data})
+    return response
 
 
 @contextmanager
 def maybe_suppress_instrumentation(suppress: bool) -> Iterator[None]:
     if suppress:
         new_context = context.set_value('suppress_instrumentation', True)
         token = context.attach(new_context)
```

### Comparing `logfire-0.28.3/logfire/_internal/integrations/psycopg.py` & `logfire-0.29.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/integrations/logging.py` & `logfire-0.29.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/integrations/loguru.py` & `logfire-0.29.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/integrations/pydantic.py` & `logfire-0.29.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/logfire/integrations/structlog.py` & `logfire-0.29.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/conftest.py` & `logfire-0.29.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_auto_trace.py` & `logfire-0.29.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_backfill.py` & `logfire-0.29.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_cli.py` & `logfire-0.29.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_collect_package_resources.py` & `logfire-0.29.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_configure.py` & `logfire-0.29.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_console_exporter.py` & `logfire-0.29.0/tests/test_console_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: reportPrivateUsage=false
 from __future__ import annotations
 
 import io
 
 import pytest
+from inline_snapshot import snapshot
 from opentelemetry import trace
 from opentelemetry.sdk.trace import ReadableSpan
 
 import logfire
 from logfire import ConsoleOptions
 from logfire._internal.exporters.console import (
     IndentedConsoleSpanExporter,
@@ -594,28 +595,28 @@
             },
             events=None,
             resource=None,
         ),
     ]
 
     out = io.StringIO()
-    SimpleConsoleSpanExporter(output=out, colors='never').export(spans)  # type: ignore
+    SimpleConsoleSpanExporter(output=out, colors='never', min_log_level='trace').export(spans)  # type: ignore
     # insert_assert(out.getvalue().splitlines())
     assert out.getvalue().splitlines() == [
         '00:00:01.000 trace message',
         '00:00:02.000 debug message',
         '00:00:03.000 info message',
         '00:00:04.000 notice message',
         '00:00:05.000 warn message',
         '00:00:06.000 error message',
         '00:00:07.000 fatal message',
     ]
 
     out = io.StringIO()
-    SimpleConsoleSpanExporter(output=out, colors='never', verbose=True).export(spans)  # type: ignore
+    SimpleConsoleSpanExporter(output=out, colors='never', verbose=True, min_log_level='trace').export(spans)  # type: ignore
     # insert_assert(out.getvalue().splitlines())
     assert out.getvalue().splitlines() == [
         '00:00:01.000 trace message',
         '             │ test_console_exporter.py:123 trace',
         '00:00:02.000 debug message',
         '             │ test_console_exporter.py:123 debug',
         '00:00:03.000 info message',
@@ -627,26 +628,39 @@
         '00:00:06.000 error message',
         '             │ test_console_exporter.py:123 error',
         '00:00:07.000 fatal message',
         '             │ test_console_exporter.py:123 fatal',
     ]
 
     out = io.StringIO()
-    SimpleConsoleSpanExporter(output=out, colors='always').export(spans)  # type: ignore
+    SimpleConsoleSpanExporter(output=out, colors='always', min_log_level='trace').export(spans)  # type: ignore
     # insert_assert(out.getvalue().splitlines())
     assert out.getvalue().splitlines() == [
         '\x1b[32m00:00:01.000\x1b[0m trace message',
         '\x1b[32m00:00:02.000\x1b[0m debug message',
         '\x1b[32m00:00:03.000\x1b[0m info message',
         '\x1b[32m00:00:04.000\x1b[0m notice message',
         '\x1b[32m00:00:05.000\x1b[0m \x1b[33mwarn message\x1b[0m',
         '\x1b[32m00:00:06.000\x1b[0m \x1b[31merror message\x1b[0m',
         '\x1b[32m00:00:07.000\x1b[0m \x1b[31mfatal message\x1b[0m',
     ]
 
+    out = io.StringIO()
+    # The `min_log_level` is set to 'info' by default, so only 'info' and higher levels are logged.
+    SimpleConsoleSpanExporter(output=out).export(spans)  # type: ignore
+    assert out.getvalue().splitlines() == snapshot(
+        [
+            '00:00:03.000 info message',
+            '00:00:04.000 notice message',
+            '00:00:05.000 warn message',
+            '00:00:06.000 error message',
+            '00:00:07.000 fatal message',
+        ]
+    )
+
 
 def test_console_logging_to_stdout(capsys: pytest.CaptureFixture[str]):
     # This is essentially a basic integration test, the other tests using an exporter
     # missed that console logging had stopped working entirely for spans.
 
     logfire.configure(
         send_to_logfire=False,
```

### Comparing `logfire-0.28.3/tests/test_formatter.py` & `logfire-0.29.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_json_args.py` & `logfire-0.29.0/tests/test_json_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,14 +805,27 @@
                     },
                     'type': 'object',
                 },
                 'type': 'array',
             },
             id='dict_of_types_in_list',
         ),
+        pytest.param(
+            [MyDataclass],
+            "[<class 'tests.test_json_args.MyDataclass'>]",
+            '["<class \'tests.test_json_args.MyDataclass\'>"]',
+            {
+                'items': {
+                    'type': 'object',
+                    'x-python-datatype': 'unknown',
+                },
+                'type': 'array',
+            },
+            id='list_of_dataclass_type',
+        ),
     ],
 )
 def test_log_non_scalar_args(
     exporter: TestExporter,
     value: Any,
     value_repr: str,
     value_json: str,
```

### Comparing `logfire-0.28.3/tests/test_json_args_formatting.py` & `logfire-0.29.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_logfire.py` & `logfire-0.29.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_loguru.py` & `logfire-0.29.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_metrics.py` & `logfire-0.29.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_no_production.py` & `logfire-0.29.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_pydantic_plugin.py` & `logfire-0.29.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_sampling.py` & `logfire-0.29.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_secret_scrubbing.py` & `logfire-0.29.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_slow_async_callbacks.py` & `logfire-0.29.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_source_code_extraction.py` & `logfire-0.29.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_stdlib_logging.py` & `logfire-0.29.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_structlog.py` & `logfire-0.29.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_testing.py` & `logfire-0.29.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/test_utils.py` & `logfire-0.29.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/utils.py` & `logfire-0.29.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/exporters/test_fallback_exporter.py` & `logfire-0.29.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/exporters/test_file_exporter.py` & `logfire-0.29.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/exporters/test_otlp_session.py` & `logfire-0.29.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/exporters/test_remove_pending.py` & `logfire-0.29.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.29.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.29.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_asgi.py` & `logfire-0.29.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_django.py` & `logfire-0.29.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_fastapi.py` & `logfire-0.29.0/tests/otel_integrations/test_fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
                 'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'start_time': 4000000000,
                 'end_time': 4000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
                     'logfire.msg': 'GET /with_path_param/{param} http send',
+                    'logfire.level_num': 5,
                     'logfire.pending_parent_id': '0000000000000001',
                 },
             },
             {
                 'name': 'GET /with_path_param/{param} http send response.start',
                 'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
@@ -256,14 +257,15 @@
                 'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'start_time': 6000000000,
                 'end_time': 6000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
                     'logfire.msg': 'GET /with_path_param/{param} http send',
+                    'logfire.level_num': 5,
                     'logfire.pending_parent_id': '0000000000000001',
                 },
             },
             {
                 'name': 'GET /with_path_param/{param} http send response.body',
                 'context': {'trace_id': 1, 'span_id': 7, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
@@ -417,14 +419,15 @@
                 'context': {'trace_id': 1, 'span_id': 9, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
                 'start_time': 6000000000,
                 'end_time': 6000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000003',
+                    'logfire.level_num': 5,
                     'logfire.msg': 'GET / http send',
                 },
             },
             {
                 'name': 'GET / http send response.start',
                 'context': {'trace_id': 1, 'span_id': 8, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
@@ -443,14 +446,15 @@
                 'context': {'trace_id': 1, 'span_id': 11, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
                 'start_time': 8000000000,
                 'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000003',
+                    'logfire.level_num': 5,
                     'logfire.msg': 'GET / http send',
                 },
             },
             {
                 'name': 'GET / http send response.body',
                 'context': {'trace_id': 1, 'span_id': 10, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
```

### Comparing `logfire-0.28.3/tests/otel_integrations/test_flask.py` & `logfire-0.29.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_httpx.py` & `logfire-0.29.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_openai.py` & `logfire-0.29.0/tests/otel_integrations/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -886,19 +886,14 @@
                     'logfire.json_schema': IsStr(),
                 },
             }
         ]
     )
 
 
-def test_get_endpoint_config_none():
-    with pytest.raises(ValueError, match='`options` is required'):
-        get_endpoint_config(None)
-
-
 def test_get_endpoint_config_json_not_dict():
     with pytest.raises(ValueError, match='Expected `options.json_data` to be a dictionary'):
         get_endpoint_config(FinalRequestOptions(method='POST', url='...'))
 
 
 def test_get_endpoint_config_unknown_url():
     with pytest.raises(ValueError, match='Unknown OpenAI API endpoint: `/foobar/`'):
```

### Comparing `logfire-0.28.3/tests/otel_integrations/test_psycopg.py` & `logfire-0.29.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_requests.py` & `logfire-0.29.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.29.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_starlette.py` & `logfire-0.29.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/test_wsgi.py` & `logfire-0.29.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.29.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.29.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/LICENSE` & `logfire-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/README.md` & `logfire-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.28.3/pyproject.toml` & `logfire-0.29.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.28.3"
+version = "0.29.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
@@ -138,20 +138,15 @@
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["logfire"]
 
 [tool.hatch.build.targets.sdist]
-include = [
-    "/README.md",
-    "/Makefile",
-    "/logfire",
-    "/tests",
-]
+include = ["/README.md", "/Makefile", "/logfire", "/tests"]
 
 # https://beta.ruff.rs/docs/configuration/
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 extend-select = [
@@ -217,14 +212,16 @@
     "ignore:The 'app' shortcut is now deprecated.*:DeprecationWarning:httpx*:",
 ]
 DJANGO_SETTINGS_MODULE = "tests.otel_integrations.django_test_project.django_test_site.settings"
 
 # https://coverage.readthedocs.io/en/latest/config.html#run
 [tool.coverage.run]
 branch = true
+# Use this to get the tests that are covering the code. This is disabled by default because it can be slow.
+# dynamic_context = "test_function"
 
 # https://coverage.readthedocs.io/en/latest/config.html#report
 [tool.coverage.report]
 skip_covered = true
 show_missing = true
 ignore_errors = true
 precision = 2
```

### Comparing `logfire-0.28.3/PKG-INFO` & `logfire-0.29.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.28.3
+Version: 0.29.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

