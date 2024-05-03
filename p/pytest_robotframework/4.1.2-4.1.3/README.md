# Comparing `tmp/pytest_robotframework-4.1.2.tar.gz` & `tmp/pytest_robotframework-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_robotframework-4.1.2.tar", last modified: Fri Mar 29 04:21:12 2024, max compression
+gzip compressed data, was "pytest_robotframework-4.1.3.tar", last modified: Fri May  3 05:52:59 2024, max compression
```

## Comparing `pytest_robotframework-4.1.2.tar` & `pytest_robotframework-4.1.3.tar`

### file list

```diff
@@ -1,261 +1,262 @@
--rw-r--r--   0        0        0     1067 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/LICENSE
--rw-r--r--   0        0        0    17528 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/README.md
--rw-r--r--   0        0        0     8067 2024-03-29 04:21:12.436873 pytest_robotframework-4.1.2/pyproject.toml
--rw-r--r--   0        0        0    28503 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/__init__.py
--rw-r--r--   0        0        0      559 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/cringe_globals.py
--rw-r--r--   0        0        0      921 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/errors.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/__init__.py
--rw-r--r--   0        0        0      230 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/exception_getter.py
--rw-r--r--   0        0        0    24784 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/plugin.py
--rw-r--r--   0        0        0     5008 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/robot_file_support.py
--rw-r--r--   0        0        0     1258 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/xdist_utils.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/__init__.py
--rw-r--r--   0        0        0     4528 2024-03-29 04:20:53.772783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/library.py
--rw-r--r--   0        0        0    25889 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
--rw-r--r--   0        0        0     9078 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/utils.py
--rw-r--r--   0        0        0     2045 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/pytest_robotframework/_internal/utils.py
--rw-r--r--   0        0        0     3240 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/pytest_robotframework/hooks.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/pytest_robotframework/py.typed
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/scripts/__init__.py
--rw-r--r--   0        0        0      177 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/scripts/clear_pycache.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/__init__.py
--rw-r--r--   0        0        0    13843 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/conftest.py
--rw-r--r--   0        0        0      230 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/__init__.py
--rw-r--r--   0        0        0      104 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_ansi.py
--rw-r--r--   0        0        0      186 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
--rw-r--r--   0        0        0      296 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
--rw-r--r--   0        0        0      105 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_fails.py
--rw-r--r--   0        0        0      105 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
--rw-r--r--   0        0        0      195 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_fails_with_description.py
--rw-r--r--   0        0        0      196 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
--rw-r--r--   0        0        0      175 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
--rw-r--r--   0        0        0      105 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_passes.py
--rw-r--r--   0        0        0      435 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
--rw-r--r--   0        0        0      253 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
--rw-r--r--   0        0        0      359 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
--rw-r--r--   0        0        0      292 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
--rw-r--r--   0        0        0       80 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
--rw-r--r--   0        0        0       57 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
--rw-r--r--   0        0        0      536 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
--rw-r--r--   0        0        0       67 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
--rw-r--r--   0        0        0       67 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
--rw-r--r--   0        0        0      163 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_class_has_separate_suite.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_class_separate_files/__init__.py
--rw-r--r--   0        0        0      121 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
--rw-r--r--   0        0        0      121 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
--rw-r--r--   0        0        0        8 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
--rw-r--r--   0        0        0       57 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
--rw-r--r--   0        0        0        8 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
--rw-r--r--   0        0        0       57 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
--rw-r--r--   0        0        0       87 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
--rw-r--r--   0        0        0      130 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment.py
--rw-r--r--   0        0        0      148 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_and_second_test.py
--rw-r--r--   0        0        0      130 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_exitonerror.py
--rw-r--r--   0        0        0      171 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_setup/__init__.py
--rw-r--r--   0        0        0      142 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_setup/conftest.py
--rw-r--r--   0        0        0      106 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
--rw-r--r--   0        0        0      145 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
--rw-r--r--   0        0        0      106 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
--rw-r--r--   0        0        0      163 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_fixture.py
--rw-r--r--   0        0        0      625 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_fixture_scope.py
--rw-r--r--   0        0        0      225 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
--rw-r--r--   0        0        0      152 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
--rw-r--r--   0        0        0       82 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_invalid_fixture.py
--rw-r--r--   0        0        0      243 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
--rw-r--r--   0        0        0      218 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_args.py
--rw-r--r--   0        0        0      554 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
--rw-r--r--   0        0        0      542 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
--rw-r--r--   0        0        0      468 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
--rw-r--r--   0        0        0      171 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
--rw-r--r--   0        0        0      148 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_docstring.py
--rw-r--r--   0        0        0      178 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
--rw-r--r--   0        0        0      445 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
--rw-r--r--   0        0        0      275 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_try_except.py
--rw-r--r--   0        0        0       85 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_names.py
--rw-r--r--   0        0        0      273 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_raises.py
--rw-r--r--   0        0        0      166 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keywordify_context_manager.py
--rw-r--r--   0        0        0      127 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keywordify_function.py
--rw-r--r--   0        0        0      280 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
--rw-r--r--   0        0        0      527 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
--rw-r--r--   0        0        0      597 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
--rw-r--r--   0        0        0      105 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
--rw-r--r--   0        0        0       77 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_module_docstring.py
--rw-r--r--   0        0        0       62 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_multiple_runs.py
--rw-r--r--   0        0        0      186 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_nested_class.py
--rw-r--r--   0        0        0      188 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_nested_keyword_that_fails.py
--rw-r--r--   0        0        0      107 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
--rw-r--r--   0        0        0      107 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
--rw-r--r--   0        0        0      126 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_nested_suites/test_top_level.py
--rw-r--r--   0        0        0       63 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
--rw-r--r--   0        0        0       92 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_one_test_fails.py
--rw-r--r--   0        0        0       73 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_one_test_passes.py
--rw-r--r--   0        0        0      162 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_one_test_skipped.py
--rw-r--r--   0        0        0      100 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_parameterized_tags.py
--rw-r--r--   0        0        0      207 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_parametrize.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.776783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
--rw-r--r--   0        0        0      185 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
--rw-r--r--   0        0        0       72 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
--rw-r--r--   0        0        0      398 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
--rw-r--r--   0        0        0       67 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
--rw-r--r--   0        0        0      471 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
--rw-r--r--   0        0        0       67 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
--rw-r--r--   0        0        0      296 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_args.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
--rw-r--r--   0        0        0       34 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
--rw-r--r--   0        0        0      262 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
--rw-r--r--   0        0        0      119 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
--rw-r--r--   0        0        0      175 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
--rw-r--r--   0        0        0      221 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
--rw-r--r--   0        0        0      235 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
--rw-r--r--   0        0        0      222 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
--rw-r--r--   0        0        0      630 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
--rw-r--r--   0        0        0       62 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
--rw-r--r--   0        0        0      498 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_variable.py
--rw-r--r--   0        0        0      498 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
--rw-r--r--   0        0        0      322 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
--rw-r--r--   0        0        0      236 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_set_log_level.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_fails/__init__.py
--rw-r--r--   0        0        0       90 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_passes/__init__.py
--rw-r--r--   0        0        0      116 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_passes/conftest.py
--rw-r--r--   0        0        0      116 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_skipped/__init__.py
--rw-r--r--   0        0        0      101 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_setup_skipped/test_foo.py
--rw-r--r--   0        0        0      305 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_suite_variables.py
--rw-r--r--   0        0        0      313 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_suite_variables_with_slash.py
--rw-r--r--   0        0        0      107 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
--rw-r--r--   0        0        0       94 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_tags.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_fails/__init__.py
--rw-r--r--   0        0        0       93 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_fails/conftest.py
--rw-r--r--   0        0        0       73 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_fails/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_passes/__init__.py
--rw-r--r--   0        0        0      119 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_passes/conftest.py
--rw-r--r--   0        0        0      115 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_passes/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_skipped/__init__.py
--rw-r--r--   0        0        0      104 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_skipped/conftest.py
--rw-r--r--   0        0        0       73 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
--rw-r--r--   0        0        0       78 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_test_case_docstring.py
--rw-r--r--   0        0        0       80 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_trace_ricing.py
--rw-r--r--   0        0        0      106 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_traceback.py
--rw-r--r--   0        0        0      108 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
--rw-r--r--   0        0        0       77 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
--rw-r--r--   0        0        0       62 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
--rw-r--r--   0        0        0       62 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       64 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       83 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
--rw-r--r--   0        0        0       63 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
--rw-r--r--   0        0        0       82 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
--rw-r--r--   0        0        0      121 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_unittest_class.py
--rw-r--r--   0        0        0      311 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_variables_list.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
--rw-r--r--   0        0        0      303 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
--rw-r--r--   0        0        0      222 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
--rw-r--r--   0        0        0       57 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xdist_n_0.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails/__init__.py
--rw-r--r--   0        0        0      133 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails/test_foo.py
--rw-r--r--   0        0        0       28 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails/tox.ini
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
--rw-r--r--   0        0        0      118 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes/__init__.py
--rw-r--r--   0        0        0      123 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes/test_foo.py
--rw-r--r--   0        0        0       28 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes/tox.ini
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
--rw-r--r--   0        0        0      107 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
--rw-r--r--   0        0        0       28 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
--rw-r--r--   0        0        0       36 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
--rw-r--r--   0        0        0       36 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
--rw-r--r--   0        0        0       44 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file/__init__.py
--rw-r--r--   0        0        0       40 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file/foo.robot
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file_nested/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
--rw-r--r--   0        0        0       40 2024-03-29 04:20:53.780783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
--rw-r--r--   0        0        0       40 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
--rw-r--r--   0        0        0      151 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator/foo.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
--rw-r--r--   0        0        0       71 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
--rw-r--r--   0        0        0      468 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
--rw-r--r--   0        0        0      162 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
--rw-r--r--   0        0        0       62 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_line_number.robot
--rw-r--r--   0        0        0      517 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
--rw-r--r--   0        0        0       40 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
--rw-r--r--   0        0        0       71 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
--rw-r--r--   0        0        0      160 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
--rw-r--r--   0        0        0       40 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_one_test_fails.robot
--rw-r--r--   0        0        0       36 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_one_test_passes.robot
--rw-r--r--   0        0        0       32 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_one_test_skipped.robot
--rw-r--r--   0        0        0       61 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
--rw-r--r--   0        0        0       34 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
--rw-r--r--   0        0        0       95 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
--rw-r--r--   0        0        0      115 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_setup_fails.robot
--rw-r--r--   0        0        0      111 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_setup_passes.robot
--rw-r--r--   0        0        0      107 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_setup_skipped.robot
--rw-r--r--   0        0        0      163 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_setup_with_args.robot
--rw-r--r--   0        0        0       96 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags.robot
--rw-r--r--   0        0        0      100 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags_in_settings.robot
--rw-r--r--   0        0        0        0 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
--rw-r--r--   0        0        0      722 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
--rw-r--r--   0        0        0       93 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
--rw-r--r--   0        0        0      119 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_teardown_fails.robot
--rw-r--r--   0        0        0      115 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_teardown_passes.robot
--rw-r--r--   0        0        0      111 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_teardown_skipped.robot
--rw-r--r--   0        0        0       36 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
--rw-r--r--   0        0        0       54 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
--rw-r--r--   0        0        0       54 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
--rw-r--r--   0        0        0       36 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
--rw-r--r--   0        0        0       55 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
--rw-r--r--   0        0        0       57 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
--rw-r--r--   0        0        0      874 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/test_common.py
--rw-r--r--   0        0        0    32434 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/test_python.py
--rw-r--r--   0        0        0    10361 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/test_robot.py
--rw-r--r--   0        0        0     1286 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/test_robot_utils.py
--rw-r--r--   0        0        0     1776 2024-03-29 04:20:53.784783 pytest_robotframework-4.1.2/tests/type_tests.py
--rw-r--r--   0        0        0    18071 1970-01-01 00:00:00.000000 pytest_robotframework-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-03 05:52:44.964870 pytest_robotframework-4.1.3/LICENSE
+-rw-r--r--   0        0        0    17497 2024-05-03 05:52:44.964870 pytest_robotframework-4.1.3/README.md
+-rw-r--r--   0        0        0     8038 2024-05-03 05:52:59.076973 pytest_robotframework-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0    28503 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/cringe_globals.py
+-rw-r--r--   0        0        0      921 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/exception_getter.py
+-rw-r--r--   0        0        0    24868 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/plugin.py
+-rw-r--r--   0        0        0     5008 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/robot_file_support.py
+-rw-r--r--   0        0        0     1181 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/xdist_utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/__init__.py
+-rw-r--r--   0        0        0     4528 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/library.py
+-rw-r--r--   0        0        0    25889 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py
+-rw-r--r--   0        0        0     9198 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/utils.py
+-rw-r--r--   0        0        0     2045 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/_internal/utils.py
+-rw-r--r--   0        0        0     3240 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/pytest_robotframework/py.typed
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/scripts/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/scripts/clear_pycache.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    13843 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/conftest.py
+-rw-r--r--   0        0        0      230 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_ansi.py
+-rw-r--r--   0        0        0      186 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_as_keyword_args_and_kwargs.py
+-rw-r--r--   0        0        0      296 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_as_keyword_context_manager_try_except.py
+-rw-r--r--   0        0        0      105 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_fails.py
+-rw-r--r--   0        0        0      105 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_fails_with_assertion_hook.py
+-rw-r--r--   0        0        0      195 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_fails_with_description.py
+-rw-r--r--   0        0        0      196 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_fails_with_fail_message_hide_assert.py
+-rw-r--r--   0        0        0      175 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_pass_hook_multiple_tests.py
+-rw-r--r--   0        0        0      105 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_passes.py
+-rw-r--r--   0        0        0      435 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_passes_custom_messages.py
+-rw-r--r--   0        0        0      253 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_passes_hide_assert.py
+-rw-r--r--   0        0        0      359 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_passes_hide_asserts_context_manager.py
+-rw-r--r--   0        0        0      292 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_passes_show_assert_when_no_assertions_in_robot_log.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/conftest.py
+-rw-r--r--   0        0        0       57 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_assertion_rewritten_in_conftest_when_assertion_hook_enabled/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator/__init__.py
+-rw-r--r--   0        0        0      536 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_class_has_separate_suite.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_class_separate_files/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_class_separate_files/test_suite1.py
+-rw-r--r--   0        0        0      121 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_class_separate_files/test_suite2.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_collect_only_nested_suites/asdf/test_foo.py
+-rw-r--r--   0        0        0        8 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/config/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_and_cwd_in_different_location/tests/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_in_different_location/__init__.py
+-rw-r--r--   0        0        0        8 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_in_different_location/asdf/tox.ini
+-rw-r--r--   0        0        0       57 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_config_file_in_different_location/test_asdf.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_bar.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_correct_items_collected_when_collect_only/test_foo.py
+-rw-r--r--   0        0        0       87 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_doesnt_run_when_collecting.py
+-rw-r--r--   0        0        0      130 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment.py
+-rw-r--r--   0        0        0      148 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_and_second_test.py
+-rw-r--r--   0        0        0      130 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_exitonerror.py
+-rw-r--r--   0        0        0      171 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_exitonerror_multiple_tests.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_setup/__init__.py
+-rw-r--r--   0        0        0      142 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_setup/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_setup/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_teardown/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_teardown/conftest.py
+-rw-r--r--   0        0        0      106 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_error_moment_teardown/test_foo.py
+-rw-r--r--   0        0        0      163 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_fixture.py
+-rw-r--r--   0        0        0      625 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_fixture_scope.py
+-rw-r--r--   0        0        0      225 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_full_stack_keyword_context_manager.py
+-rw-r--r--   0        0        0      152 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_full_stack_keyword_decorator.py
+-rw-r--r--   0        0        0       82 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_invalid_fixture.py
+-rw-r--r--   0        0        0      243 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_and_pytest_raises.py
+-rw-r--r--   0        0        0      218 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_args.py
+-rw-r--r--   0        0        0      554 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py
+-rw-r--r--   0        0        0      542 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py
+-rw-r--r--   0        0        0      468 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_exit.py
+-rw-r--r--   0        0        0      171 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_custom_name_and_tags.py
+-rw-r--r--   0        0        0      148 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_docstring.py
+-rw-r--r--   0        0        0      178 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_docstring_on_next_line.py
+-rw-r--r--   0        0        0      445 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_returns_context_manager_that_isnt_used.py
+-rw-r--r--   0        0        0      275 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_try_except.py
+-rw-r--r--   0        0        0       85 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_names.py
+-rw-r--r--   0        0        0      273 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_raises.py
+-rw-r--r--   0        0        0      166 2024-05-03 05:52:44.968870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keywordify_context_manager.py
+-rw-r--r--   0        0        0      127 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keywordify_function.py
+-rw-r--r--   0        0        0      280 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keywordify_keyword_inside_context_manager.py
+-rw-r--r--   0        0        0      527 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_calls_log_file/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_not_run_during_collection/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py
+-rw-r--r--   0        0        0      105 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_not_run_during_collection/test_foo.py
+-rw-r--r--   0        0        0       77 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_module_docstring.py
+-rw-r--r--   0        0        0       62 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_multiple_runs.py
+-rw-r--r--   0        0        0      186 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_nested_class.py
+-rw-r--r--   0        0        0      188 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_nested_keyword_that_fails.py
+-rw-r--r--   0        0        0      107 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_nested_suites/suite1/suite2/test_asdf.py
+-rw-r--r--   0        0        0      107 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_nested_suites/suite1/suite3/test_asdf2.py
+-rw-r--r--   0        0        0      126 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_nested_suites/test_top_level.py
+-rw-r--r--   0        0        0       63 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_no_tests_found_when_tests_exist.py
+-rw-r--r--   0        0        0       92 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_one_test_fails.py
+-rw-r--r--   0        0        0       73 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_one_test_passes.py
+-rw-r--r--   0        0        0      162 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_one_test_skipped.py
+-rw-r--r--   0        0        0      100 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_parameterized_tags.py
+-rw-r--r--   0        0        0      207 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_parametrize.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/a/test_c.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_hook_in_different_suite/b/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_item_hook/foo/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/conftest.py
+-rw-r--r--   0        0        0       67 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_pytest_runtest_protocol_session_hook/test_foo.py
+-rw-r--r--   0        0        0      296 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_python_file_doesnt_get_parsed_as_robot_file.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_args.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_keyword_in_python_test/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_keyword_in_python_test/bar/bar.resource
+-rw-r--r--   0        0        0      262 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_keyword_in_python_test/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/conftest.py
+-rw-r--r--   0        0        0      221 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_args_hook_collect_only/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook/conftest.py
+-rw-r--r--   0        0        0      222 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py
+-rw-r--r--   0        0        0       62 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/test_foo.py
+-rw-r--r--   0        0        0      498 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_variable.py
+-rw-r--r--   0        0        0      498 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_options_variable_merge_listeners/test_foo.py
+-rw-r--r--   0        0        0      236 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_set_log_level.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_fails/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_passes/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_passes/conftest.py
+-rw-r--r--   0        0        0      116 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_skipped/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_setup_skipped/test_foo.py
+-rw-r--r--   0        0        0      305 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_suite_variables.py
+-rw-r--r--   0        0        0      313 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_suite_variables_with_slash.py
+-rw-r--r--   0        0        0      107 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_suites/suite1/test_asdf.py
+-rw-r--r--   0        0        0       94 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_tags.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_fails/__init__.py
+-rw-r--r--   0        0        0       93 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_fails/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_fails/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_passes/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_passes/conftest.py
+-rw-r--r--   0        0        0      115 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_passes/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_skipped/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_skipped/conftest.py
+-rw-r--r--   0        0        0       73 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_teardown_skipped/test_foo.py
+-rw-r--r--   0        0        0       78 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_test_case_docstring.py
+-rw-r--r--   0        0        0       80 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_trace_ricing.py
+-rw-r--r--   0        0        0      106 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_traceback.py
+-rw-r--r--   0        0        0      108 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_one_fail_one_pass.py
+-rw-r--r--   0        0        0       77 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_specified_by_full_path.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_bar.py
+-rw-r--r--   0        0        0       62 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_specified_by_full_path_in_different_files/test_foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       83 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_two_files_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_one.py
+-rw-r--r--   0        0        0       82 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_two_tests_with_same_name_one_fail_one_pass/test_two.py
+-rw-r--r--   0        0        0      121 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_unittest_class.py
+-rw-r--r--   0        0        0      311 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_variables_list.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_one.py
+-rw-r--r--   0        0        0      222 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_variables_not_in_scope_in_other_suites/test_two.py
+-rw-r--r--   0        0        0       57 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xdist_n_0.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-03 05:52:44.972870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails_no_reason/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_fails_no_reason/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes/__init__.py
+-rw-r--r--   0        0        0      123 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes/tox.ini
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes_no_reason/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes_no_reason/test_foo.py
+-rw-r--r--   0        0        0       28 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_python/test_xfail_passes_no_reason/tox.ini
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_collect_only_nested_suites/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_collect_only_nested_suites/foo.robot
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/bar.robot
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_correct_items_collected_when_collect_only/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/bar/asdf.robot
+-rw-r--r--   0        0        0       36 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_doesnt_run_tests_outside_path/foo/asdf.robot
+-rw-r--r--   0        0        0       44 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_doesnt_run_when_collecting.robot
+-rw-r--r--   0        0        0       99 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_fails_when_import_error_and_exit_on_error.robot
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file_nested/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file_nested/foo/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file_nested/foo/bar.robot
+-rw-r--r--   0        0        0       40 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_init_file_nested/foo/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator/bar.robot
+-rw-r--r--   0        0        0      151 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator/foo.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/bar.robot
+-rw-r--r--   0        0        0      468 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_decorator_and_other_decorator/foo.py
+-rw-r--r--   0        0        0      162 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_keyword_with_conflicting_name.robot
+-rw-r--r--   0        0        0       62 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_line_number.robot
+-rw-r--r--   0        0        0      517 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_listener_calls_log_file/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_listener_calls_log_file/foo.robot
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_nested_keyword_that_fails/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_nested_keyword_that_fails/bar.robot
+-rw-r--r--   0        0        0      160 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_nested_keyword_that_fails/foo.py
+-rw-r--r--   0        0        0       40 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_no_tests_found_when_tests_exist.robot
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_one_test_fails.robot
+-rw-r--r--   0        0        0       36 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_one_test_passes.robot
+-rw-r--r--   0        0        0       32 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_one_test_skipped.robot
+-rw-r--r--   0        0        0       61 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_parameterized_tags/foo.robot
+-rw-r--r--   0        0        0       34 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_parameterized_tags/tox.ini
+-rw-r--r--   0        0        0       95 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_run_keyword_and_ignore_error.robot
+-rw-r--r--   0        0        0      115 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_setup_fails.robot
+-rw-r--r--   0        0        0      111 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_setup_passes.robot
+-rw-r--r--   0        0        0      107 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_setup_skipped.robot
+-rw-r--r--   0        0        0      163 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_setup_with_args.robot
+-rw-r--r--   0        0        0       96 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags.robot
+-rw-r--r--   0        0        0      100 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags_in_settings.robot
+-rw-r--r--   0        0        0        0 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags_with_kwargs/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py
+-rw-r--r--   0        0        0       93 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags_with_kwargs/test_tags_with_kwargs.robot
+-rw-r--r--   0        0        0      119 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_teardown_fails.robot
+-rw-r--r--   0        0        0      115 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_teardown_passes.robot
+-rw-r--r--   0        0        0      111 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_teardown_skipped.robot
+-rw-r--r--   0        0        0       36 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_two_files_run_one_test/bar.robot
+-rw-r--r--   0        0        0       54 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_two_files_run_one_test/foo.robot
+-rw-r--r--   0        0        0       54 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/asdf/foo.robot
+-rw-r--r--   0        0        0       36 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_two_files_run_test_from_second_suite/fdsa/bar.robot
+-rw-r--r--   0        0        0       55 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_two_tests_one_fail_one_pass.robot
+-rw-r--r--   0        0        0       57 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_warning_on_unknown_tag.robot
+-rw-r--r--   0        0        0      874 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/test_common.py
+-rw-r--r--   0        0        0    32434 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/test_python.py
+-rw-r--r--   0        0        0    10564 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/test_robot.py
+-rw-r--r--   0        0        0     1286 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/test_robot_utils.py
+-rw-r--r--   0        0        0     1776 2024-05-03 05:52:44.976870 pytest_robotframework-4.1.3/tests/type_tests.py
+-rw-r--r--   0        0        0    18040 1970-01-01 00:00:00.000000 pytest_robotframework-4.1.3/PKG-INFO
```

### Comparing `pytest_robotframework-4.1.2/LICENSE` & `pytest_robotframework-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/README.md` & `pytest_robotframework-4.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -391,19 +391,20 @@
 
 # IDE integration
 
 ## vscode
 
 vscode's builtin python plugin should discover both your python and robot tests by default, and show run buttons next to them:
 
-![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/411233d0-a0d6-4fca-9701-0503b534bd46)
+![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/d81278cc-1574-4360-be3c-29805b47dec6)
+![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/cce2fc08-806f-4b0e-85b9-42be677871ab)
 
-if you use the [robotframework-lsp](https://github.com/robocorp/robotframework-lsp) extension, you'll see duplicated tests on `.robot` files because you have two extensions that can discover them. to fix this, set `robot.testView.enabled` to `false` in vscode's settings.
+### running `.robot` tests
 
-(note: at the time of writing, this option is not yet in the latest version of the extension, so for now you'll need to install [this build](https://github.com/DetachHead/robotframework-lsp/releases/tag/asdf))
+if you still intend to use `.robot` files with pytest-robotframework, we recommend using the [robotcode](https://github.com/d-biehl/robotcode) extension and setting `robotcode.testExplorer.enabled` to `false` in `.vscode/settings.json`. this will prevent the tests from being duplicated in the test explorer.
 
 ## pycharm
 
 pycharm currently does not support pytest plugins for non-python files. see [this issue](https://youtrack.jetbrains.com/issue/PY-63110/use-pytest-collect-only-to-collect-pytest-tests)
 
 # compatibility
```

### Comparing `pytest_robotframework-4.1.2/pyproject.toml` & `pytest_robotframework-4.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest_robotframework"
-version = "4.1.2"
+version = "4.1.3"
 description = "a pytest plugin that can run both python and robotframework tests while generating robot reports for them"
 authors = [
     { name = "DetachHead", email = "detachhead@users.noreply.github.com" },
 ]
 dependencies = [
     "pytest<9,>=7",
     "robotframework<8.0.0,>=6.1",
@@ -20,15 +20,15 @@
 [project.urls]
 repository = "https://github.com/detachhead/pytest-robotframework"
 
 [project.entry-points.pytest11]
 robotframework = "pytest_robotframework._internal.pytest.plugin"
 
 [tool.pyprojectx]
-pdm = "pdm==2.12.4"
+pdm = "pdm==2.15.1"
 
 [tool.pdm.scripts]
 update = "pdm update"
 refresh_lockfile = "pdm lock --update-reuse"
 test = "pytest -n auto"
 pylint = "pylint pytest_robotframework tests"
 robocop = "robocop"
@@ -52,24 +52,25 @@
 composite = [
     "ruff check --fix",
     "ruff format",
 ]
 
 [tool.pdm.dev-dependencies]
 lint = [
-    "basedpyright>=1.6.0",
-    "pylint>=3.0.0a7",
+    "basedpyright>=1.10.1",
+    "pylint@git+https://github.com/pylint-dev/pylint@e5e6ca713b3e8ce8037ca8bd2d39154b1df016e7",
     "ruff>=0.2.0",
     "robotframework-robocop>=4.1.0",
     "robotframework-tidy>=4.5.0",
 ]
 test = [
     "lxml>=4.9.3",
     "lxml-stubs>=0.4.0",
     "pytest-xdist>=3.5.0",
+    "pytest-github-actions-annotate-failures>=0.2.0",
 ]
 docs = [
     "pdoc>=14.1.0",
 ]
 
 [tool.ruff]
 unsafe-fixes = true
@@ -210,30 +211,27 @@
 ]
 enable = [
     "useless-suppression",
     "access-member-before-definition",
     "assignment-from-none",
     "dict-iter-missing-items",
     "invalid-bool-returned",
-    "invalid-bytes-returned",
     "invalid-getnewargs-ex-returned",
     "invalid-getnewargs-returned",
     "invalid-index-returned",
     "invalid-length-hint-returned",
-    "invalid-length-returned",
     "invalid-slice-index",
     "invalid-slice-step",
     "invalid-slots",
     "invalid-slots-object",
     "invalid-unicode-codec",
     "logging-format-truncated",
     "logging-unsupported-format",
     "method-hidden",
     "modified-iterating-dict",
-    "modified-iterating-set",
     "potential-index-error",
     "relative-beyond-top-level",
     "abstract-method",
     "arguments-out-of-order",
     "attribute-defined-outside-init",
     "confusing-with-statement",
     "deprecated-decorator",
@@ -247,26 +245,24 @@
     "overlapping-except",
     "preferred-module",
     "raising-format-tuple",
     "redefined-outer-name",
     "redefined-slots-in-subclass",
     "redundant-returns-doc",
     "redundant-yields-doc",
-    "self-cls-assignment",
     "shallow-copy-environ",
     "useless-param-doc",
     "useless-parent-delegation",
     "useless-type-doc",
     "using-constant-test",
     "bad-file-encoding",
     "dict-init-mutate",
     "use-implicit-booleaness-not-comparison",
     "chained-comparison",
     "confusing-consecutive-elif",
-    "consider-using-augmented-assign",
     "consider-using-join",
     "consider-using-max-builtin",
     "consider-using-min-builtin",
     "consider-using-namedtuple-or-dataclass",
     "consider-using-tuple",
     "simplifiable-condition",
     "simplify-boolean-expression",
```

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/__init__.py` & `pytest_robotframework-4.1.3/pytest_robotframework/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/cringe_globals.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/cringe_globals.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/errors.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/errors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/plugin.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,22 +250,22 @@
             RobotFramework().parse_arguments(  # pyright:ignore[reportUnknownMemberType]
                 # i don't think this is actually used here, but we send it the correct paths
                 # just to be safe
                 _get_pytest_collection_paths(session)
             )[0],
         ),
     )
-
-    result = cast(RobotOptions, options)
+    # https://github.com/DetachHead/basedpyright#note-about-casting-with-typeddicts
+    result = cast(RobotOptions, options)  # pyright:ignore[reportInvalidCast]
     session.config.hook.pytest_robot_modify_options(options=result, session=session)
     session.stash[_robot_args_key] = result
     return result
 
 
-def _run_robot(session: Session, robot_options: InternalRobotOptions) -> int:
+def _run_robot(session: Session, robot_options: InternalRobotOptions):
     """runs robot with the specified `robot_options`"""
     robot_options = merge_robot_options(
         # user-specified options:
         _get_robot_args(session),
         # collect or run test specific options:
         robot_options,
         # options that always need to be set:
@@ -289,15 +289,20 @@
                 **robot_options,
             ),
         )
 
     robot_errors = report_robot_errors(session)
     if robot_errors:
         raise Exception(robot_errors)
-    return exit_code
+    if exit_code and not session.testsfailed:
+        raise Exception(
+            f"pytest-robotframework detected that robot failed with exit code {exit_code} despite"
+            + " no tests failing. this was may have been caused by a robot error that occurred"
+            + " before any tests started."
+        )
 
 
 def _robot_collect(session: Session):
     """runs robot in "collection" mode, meaning it won't actually run any tests or output any result
     files. this is only used to set `session.stash[collected_robot_tests_key]` which is then used in
     `_internal.pytest.robot_file_support` during collectionto create `RobotItem`s for tests located
     in `.robot` files
@@ -306,20 +311,15 @@
         "report": None,
         "output": None,
         "log": None,
         "exitonerror": True,
         "prerunmodifier": [RobotSuiteCollector(session)],
         "listener": None,
     }
-    exit_code = _run_robot(session, robot_options)
-    if exit_code:
-        # robot should never fail during collection because we prevent it from running any tests, so
-        # any failure would mean one of our suite visitors or something messed up, or it tried to
-        # run tests
-        raise InternalError(f"robot failed during collection ({exit_code=})")
+    _run_robot(session, robot_options)
 
 
 def _robot_run_tests(session: Session, xdist_item: Item | None = None):
     """
     runs robot either on an individual item or on every item in the session.
 
     :param xdist_item: if provided, only runs robot for this item.
```

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/robot_file_support.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/robot_file_support.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/pytest/xdist_utils.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/pytest/xdist_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,18 +26,15 @@
     )
 
 
 def worker_id(session: Session) -> str | None:
     xdist = get_xdist()
     if xdist is None:
         return None
-    result = cast(
-        str,
-        xdist.get_xdist_worker_id(session),  # pyright:ignore[reportUnknownMemberType]
-    )
+    result = xdist.get_xdist_worker_id(session)
     return None if result == "master" else result
 
 
 def is_xdist_worker(session: Session) -> bool:
     """checks whether the test is running in xdist mode (`-n` argument), since we need special
     handling to support it"""
     return worker_id(session) is not None
```

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/library.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/library.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/listeners_and_suite_visitors.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/robot/utils.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/robot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,16 +237,16 @@
 
 
 def cli_defaults(settings_class: Callable[[dict[str, object]], _BaseSettings]) -> RobotOptions:
     # need to reset outputdir because if anything from robot gets imported before pytest runs, then
     # the cwd gets updated, robot will still run with the outdated cwd.
     # we set it in this wacky way to make sure it never overrides user preferences
     _BaseSettings._cli_opts["OutputDir"] = ("outputdir", ".")  # pyright:ignore[reportUnknownMemberType,reportPrivateUsage]
-
-    return cast(
+    # https://github.com/DetachHead/basedpyright#note-about-casting-with-typeddicts
+    return cast(  # pyright:ignore[reportInvalidCast]
         RobotOptions,
         dict(
             # instantiate the class because _BaseSettings.__init__ adds any additional opts
             # that the subclass may have defined (using _extra_cli_opts)
             settings_class(  # pyright:ignore[reportUnknownArgumentType,reportUnknownMemberType]
                 {}
             )._cli_opts.values()  # pyright:ignore[reportPrivateUsage]
```

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/_internal/utils.py` & `pytest_robotframework-4.1.3/pytest_robotframework/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/pytest_robotframework/hooks.py` & `pytest_robotframework-4.1.3/pytest_robotframework/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/conftest.py` & `pytest_robotframework-4.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_catch_errors_decorator_with_non_instance_method/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_fixture_scope.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_fixture_scope.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_doesnt_suppress.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_keyword_decorator_context_manager_that_raises_in_body_and_exit.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_listener_not_run_during_collection/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_python/test_robot_modify_options_hook_listener_instance/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_listener_calls_log_file/Listener.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py` & `pytest_robotframework-4.1.3/tests/fixtures/test_robot/test_tags_with_kwargs/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/test_common.py` & `pytest_robotframework-4.1.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/test_python.py` & `pytest_robotframework-4.1.3/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/test_robot.py` & `pytest_robotframework-4.1.3/tests/test_robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     xml = output_xml()
     assert xml.xpath(".//test[@name='Foo']/tag[.='m1']")
     assert xml.xpath(".//test[@name='Bar']/tag[.='m1']")
 
 
 def test_warning_on_unknown_tag(pr: PytestRobotTester):
     result = pr.run_pytest("--strict-markers", "-m", "m1")
-    result.assert_outcomes(errors=pr.xdist if pr.xdist else 1)
+    result.assert_outcomes(errors=pr.xdist or 1)
     assert result.ret == ExitCode.TESTS_FAILED
     assert "'m1' not found in `markers` configuration option" in result.outlines
 
 
 def test_parameterized_tags(pr: PytestRobotTester):
     markers: list[Mark] | None = None
 
@@ -283,7 +283,12 @@
     pr.run_and_assert_result("-o", "enable_assertion_pass_hook=true", subprocess=True, failed=1)
     pr.assert_log_file_exists()
     xml = output_xml()
     assert xpath(xml, "//kw[@name='Bar']/kw[@name='Baz']/msg[@level='FAIL' and .='asdf']")
     # make sure the error was only logged once, since the exception gets re-raised after the
     # keyword is over we want to make sure it's not printed multiple times
     assert xpath(xml, "//msg[@level='FAIL']")
+
+
+def test_fails_when_import_error_and_exit_on_error(pr: PytestRobotTester):
+    pr.run_and_assert_assert_pytest_result("--robot-exitonerror", exit_code=ExitCode.INTERNAL_ERROR)
+    assert_robot_total_stats(failed=1)
```

### Comparing `pytest_robotframework-4.1.2/tests/test_robot_utils.py` & `pytest_robotframework-4.1.3/tests/test_robot_utils.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/tests/type_tests.py` & `pytest_robotframework-4.1.3/tests/type_tests.py`

 * *Files identical despite different names*

### Comparing `pytest_robotframework-4.1.2/PKG-INFO` & `pytest_robotframework-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_robotframework
-Version: 4.1.2
+Version: 4.1.3
 Summary: a pytest plugin that can run both python and robotframework tests while generating robot reports for them
 Author-Email: DetachHead <detachhead@users.noreply.github.com>
 License: MIT
 Project-URL: Repository, https://github.com/detachhead/pytest-robotframework
 Requires-Python: <4.0,>=3.8
 Requires-Dist: pytest<9,>=7
 Requires-Dist: robotframework<8.0.0,>=6.1
@@ -405,19 +405,20 @@
 
 # IDE integration
 
 ## vscode
 
 vscode's builtin python plugin should discover both your python and robot tests by default, and show run buttons next to them:
 
-![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/411233d0-a0d6-4fca-9701-0503b534bd46)
+![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/d81278cc-1574-4360-be3c-29805b47dec6)
+![image](https://github.com/DetachHead/pytest-robotframework/assets/57028336/cce2fc08-806f-4b0e-85b9-42be677871ab)
 
-if you use the [robotframework-lsp](https://github.com/robocorp/robotframework-lsp) extension, you'll see duplicated tests on `.robot` files because you have two extensions that can discover them. to fix this, set `robot.testView.enabled` to `false` in vscode's settings.
+### running `.robot` tests
 
-(note: at the time of writing, this option is not yet in the latest version of the extension, so for now you'll need to install [this build](https://github.com/DetachHead/robotframework-lsp/releases/tag/asdf))
+if you still intend to use `.robot` files with pytest-robotframework, we recommend using the [robotcode](https://github.com/d-biehl/robotcode) extension and setting `robotcode.testExplorer.enabled` to `false` in `.vscode/settings.json`. this will prevent the tests from being duplicated in the test explorer.
 
 ## pycharm
 
 pycharm currently does not support pytest plugins for non-python files. see [this issue](https://youtrack.jetbrains.com/issue/PY-63110/use-pytest-collect-only-to-collect-pytest-tests)
 
 # compatibility
```

