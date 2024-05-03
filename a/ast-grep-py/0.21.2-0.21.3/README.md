# Comparing `tmp/ast_grep_py-0.21.2.tar.gz` & `tmp/ast_grep_py-0.21.3.tar.gz`

## Comparing `ast_grep_py-0.21.2.tar` & `ast_grep_py-0.21.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0     1001      127      693 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    14735 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    14742 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17980 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127      683 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     6091 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5213 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     7993 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    17323 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     7584 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    18996 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5226 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    16017 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    12633 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127    10865 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    11211 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127     2219 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1142 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13416 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3410 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2157 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/language/src/swift.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.21.2/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7731 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61091 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/Cargo.lock
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 ast_grep_py-0.21.2/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.21.2/pyproject.toml
--rw-r--r--   0     1001      127     1933 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1356 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1459 2024-05-02 06:42:51.000000 ast_grep_py-0.21.2/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.21.2/PKG-INFO
+-rw-r--r--   0     1001      127     2219 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1142 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13416 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3410 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2157 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/language/src/swift.rs
+-rw-r--r--   0     1001      127      683 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     6091 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5213 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     7993 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    17323 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     7584 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    18996 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5226 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    16017 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    12633 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127    10865 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    10708 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127      693 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15050 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    17980 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/core/src/traversal.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61091 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/Cargo.lock
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/pyproject.toml
+-rw-r--r--   0     1001      127     1933 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1356 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1459 2024-05-03 04:28:23.000000 ast_grep_py-0.21.3/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.21.3/PKG-INFO
```

### Comparing `ast_grep_py-0.21.2/crates/core/Cargo.toml` & `ast_grep_py-0.21.3/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/language.rs` & `ast_grep_py-0.21.3/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/lib.rs` & `ast_grep_py-0.21.3/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/match_tree.rs` & `ast_grep_py-0.21.3/crates/core/src/match_tree.rs`

 * *Files 5% similar despite different names*

```diff
@@ -289,20 +289,26 @@
     }
     cand_children.next();
     cand_children.peek()?;
   }
 }
 
 pub fn does_node_match_exactly<D: Doc>(goal: &Node<D>, candidate: &Node<D>) -> bool {
+  // return true if goal and candidate are the same node
+  if goal.node_id() == candidate.node_id() {
+    return true;
+  }
+  // gh issue #1087, we make pattern matching a little bit more permissive
+  // compare node text if at least one node is leaf
+  if goal.is_named_leaf() || candidate.is_named_leaf() {
+    return goal.text() == candidate.text();
+  }
   if goal.kind_id() != candidate.kind_id() {
     return false;
   }
-  if goal.is_named_leaf() {
-    return goal.text() == candidate.text();
-  }
   let goal_children = goal.children();
   let cand_children = candidate.children();
   if goal_children.len() != cand_children.len() {
     return false;
   }
   goal_children
     .zip(cand_children)
@@ -496,8 +502,13 @@
   fn test_ellipsis_end() {
     let end = test_end(
       "import {$$$A, B, $$$C} from 'a'",
       "import {A, B, C} from 'a'",
     );
     assert_eq!(end.expect("must match"), 25);
   }
+
+  #[test]
+  fn test_gh_1087() {
+    test_match("($P) => $F($P)", "(x) => bar(x)");
+  }
 }
```

### Comparing `ast_grep_py-0.21.2/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.21.3/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.21.3/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.21.3/crates/core/src/matcher/pattern.rs`

 * *Files 1% similar despite different names*

```diff
@@ -510,8 +510,19 @@
   }
 
   #[test]
   fn test_extract_duplicate_meta_var() {
     let vars = defined_vars("var $A = $A");
     assert_eq!(vars, ["A"]);
   }
+
+  #[test]
+  fn test_contextual_pattern_vars() {
+    let pattern = Pattern::contextual("<div ref={$A}/>", "jsx_attribute", Tsx).expect("correct");
+    assert_eq!(pattern.defined_vars(), ["A"].into_iter().collect());
+  }
+
+  #[test]
+  fn test_gh_1087() {
+    test_match("($P) => $F($P)", "(x) => bar(x)");
+  }
 }
```

### Comparing `ast_grep_py-0.21.2/crates/core/src/matcher/text.rs` & `ast_grep_py-0.21.3/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/matcher.rs` & `ast_grep_py-0.21.3/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/meta_var.rs` & `ast_grep_py-0.21.3/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/node.rs` & `ast_grep_py-0.21.3/crates/core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/ops.rs` & `ast_grep_py-0.21.3/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/pinned.rs` & `ast_grep_py-0.21.3/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.21.3/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.21.3/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/replacer/template.rs` & `ast_grep_py-0.21.3/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/replacer.rs` & `ast_grep_py-0.21.3/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/source.rs` & `ast_grep_py-0.21.3/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/core/src/traversal.rs` & `ast_grep_py-0.21.3/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/Cargo.toml` & `ast_grep_py-0.21.3/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/check_var.rs` & `ast_grep_py-0.21.3/crates/config/src/check_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/combined.rs` & `ast_grep_py-0.21.3/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/fixer.rs` & `ast_grep_py-0.21.3/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/lib.rs` & `ast_grep_py-0.21.3/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/maybe.rs` & `ast_grep_py-0.21.3/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.21.3/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule/mod.rs` & `ast_grep_py-0.21.3/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.21.3/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.21.3/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.21.3/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule_collection.rs` & `ast_grep_py-0.21.3/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule_config.rs` & `ast_grep_py-0.21.3/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/rule_core.rs` & `ast_grep_py-0.21.3/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/transform/mod.rs` & `ast_grep_py-0.21.3/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.21.3/crates/config/src/transform/rewrite.rs`

 * *Files 6% similar despite different names*

```diff
@@ -140,91 +140,82 @@
 mod test {
   use super::*;
   use crate::from_str;
   use crate::rule::DeserializeEnv;
   use crate::rule_core::SerializableRuleCore;
   use crate::test::TypeScript;
   use crate::GlobalRules;
+  use std::collections::HashSet;
 
   fn apply_transformation(
     rewrite: Rewrite,
     src: &str,
     pat: &str,
     rewriters: GlobalRules<TypeScript>,
   ) -> String {
-    let grep = TypeScript::Tsx.ast_grep(src);
-    let root = grep.root();
-    let mut nm = root.find(pat).expect("should find");
-    let before_vars: Vec<_> = nm.get_env().get_matched_variables().collect();
-    let env = nm.get_env_mut();
-    let enclosing = env.clone();
-    let mut ctx = Ctx {
-      lang: &TypeScript::Tsx,
-      transforms: &Default::default(),
-      env,
-      rewriters,
-      enclosing_env: &enclosing,
-    };
-    let after_vars: Vec<_> = ctx.env.get_matched_variables().collect();
-    assert_eq!(
-      before_vars, after_vars,
-      "rewrite should not write back to env"
-    );
-    rewrite.compute(&mut ctx).expect("should have transforms")
+    compute_rewritten(src, pat, rewrite, rewriters).expect("should have transforms")
   }
+
   macro_rules! str_vec {
     ( $($a: expr),* ) => { vec![ $($a.to_string()),* ] };
   }
 
-  fn make_rewriter(pairs: &[(&str, &str)]) -> GlobalRules<TypeScript> {
+  fn make_rewriters(pairs: &[(&str, &str)]) -> GlobalRules<TypeScript> {
+    make_rewriters_with_rewriter(pairs, Default::default())
+  }
+
+  fn make_rewriters_with_rewriter(
+    pairs: &[(&str, &str)],
+    vars: HashSet<&str>,
+  ) -> GlobalRules<TypeScript> {
     let rewriters = GlobalRules::default();
     for (key, ser) in pairs {
       let serialized: SerializableRuleCore = from_str(ser).unwrap();
       let env = DeserializeEnv::new(TypeScript::Tsx).with_rewriters(&rewriters);
-      let rule = serialized.get_rewriter(env, &Default::default()).unwrap();
+      let rule = serialized.get_rewriter(env, &vars).unwrap();
       rewriters.insert(key, rule).unwrap();
     }
     rewriters
   }
 
   #[test]
   fn test_perform_one_rewrite() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["rewrite"],
       join_by: None,
     };
-    let rewriters = make_rewriter(&[("rewrite", "{rule: {kind: number}, fix: '810'}")]);
+    let rewriters = make_rewriters(&[("rewrite", "{rule: {kind: number}, fix: '810'}")]);
     let ret = apply_transformation(rewrite, "log(t(1, 2, 3))", "log($A)", rewriters);
     assert_eq!(ret, "t(810, 810, 810)");
   }
 
   #[test]
   fn test_perform_multiple_rewriters() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re1", "re2"],
       join_by: None,
     };
-    let rewriters = make_rewriter(&[
+    let rewriters = make_rewriters(&[
       ("re1", "{rule: {regex: '^1$'}, fix: '810'}"),
       ("re2", "{rule: {regex: '^2$'}, fix: '1919'}"),
     ]);
     let ret = apply_transformation(rewrite, "log(t(1, 2, 3))", "log($A)", rewriters);
     assert_eq!(ret, "t(810, 1919, 3)");
   }
 
   #[test]
   fn test_ignore_unused_rewriters() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re1"],
       join_by: None,
     };
-    let rewriters = make_rewriter(&[
+    let rewriters = make_rewriters(&[
       ("ignored", "{rule: {regex: '^2$'}, fix: '1919'}"),
       ("re1", "{rule: {kind: number}, fix: '810'}"),
     ]);
     let ret = apply_transformation(rewrite, "log(t(1, 2, 3))", "log($A)", rewriters);
     assert_eq!(ret, "t(810, 810, 810)");
   }
 
@@ -232,15 +223,15 @@
   fn test_rewriters_order() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re2", "re1"],
       join_by: None,
     };
     // first match wins the rewrite
-    let rewriters = make_rewriter(&[
+    let rewriters = make_rewriters(&[
       ("re2", "{rule: {regex: '^2$'}, fix: '1919'}"),
       ("re1", "{rule: {kind: number}, fix: '810'}"),
     ]);
     let ret = apply_transformation(rewrite, "log(t(1, 2, 3))", "log($A)", rewriters);
     assert_eq!(ret, "t(810, 1919, 810)");
   }
 
@@ -248,30 +239,30 @@
   fn test_rewriters_overlapping() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re1", "re2"],
       join_by: None,
     };
     // parent node wins fix, even if rule comes later
-    let rewriters = make_rewriter(&[
+    let rewriters = make_rewriters(&[
       ("re1", "{rule: {kind: number}, fix: '810'}"),
       ("re2", "{rule: {kind: array}, fix: '1919'}"),
     ]);
     let ret = apply_transformation(rewrite, "[1, 2, 3]", "$A", rewriters);
     assert_eq!(ret, "1919");
   }
 
   #[test]
   fn test_rewriters_join_by() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re1"],
       join_by: Some(" + ".into()),
     };
-    let rewriters = make_rewriter(&[("re1", "{rule: {kind: number}, fix: '810'}")]);
+    let rewriters = make_rewriters(&[("re1", "{rule: {kind: number}, fix: '810'}")]);
     let ret = apply_transformation(rewrite, "log(t(1, 2, 3))", "log($A)", rewriters);
     assert_eq!(ret, "810 + 810 + 810");
   }
 
   #[test]
   fn test_recursive_rewriters() {
     let rewrite = Rewrite {
@@ -284,27 +275,27 @@
 transform:
   D:
     rewrite:
       source: $$$C
       rewriters: [re1]
 fix: $D
     "#;
-    let rewriters = make_rewriter(&[("re1", rule)]);
+    let rewriters = make_rewriters(&[("re1", rule)]);
     let ret = apply_transformation(rewrite, "[1, [2, [3, [4]]]]", "$A", rewriters);
     assert_eq!(ret, "1, 2, 3, 4");
   }
 
   #[test]
   fn test_should_inherit_match_env() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re"],
       join_by: None,
     };
-    let rewriters = make_rewriter(&[("re", "{rule: {pattern: $C}, fix: '123'}")]);
+    let rewriters = make_rewriters(&[("re", "{rule: {pattern: $C}, fix: '123'}")]);
     let ret = apply_transformation(rewrite.clone(), "[1, 2]", "[$A, $B]", rewriters.clone());
     assert_eq!(ret, "123");
     let ret = apply_transformation(rewrite.clone(), "[1, 1]", "[$A, $C]", rewriters.clone());
     assert_eq!(ret, "123");
     // should not match $C so no rewrite
     let ret = apply_transformation(rewrite, "[1, 2]", "[$A, $C]", rewriters);
     assert_eq!(ret, "1");
@@ -313,55 +304,54 @@
   #[test]
   fn test_node_not_found() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re"],
       join_by: None,
     };
-    let rewriters = make_rewriter(&[("re", "{rule: {pattern: $B}, fix: '123'}")]);
-    let grep = TypeScript::Tsx.ast_grep("[1, 2]");
-    let root = grep.root();
-    let mut nm = root.find("[$B, $C]").expect("should find");
-    let env = nm.get_env_mut();
-    let enclosing = env.clone();
-    let mut ctx = Ctx {
-      lang: &TypeScript::Tsx,
-      transforms: &Default::default(),
-      env,
-      rewriters,
-      enclosing_env: &enclosing,
-    };
-    let ret = rewrite.compute(&mut ctx);
+    let rewriters = make_rewriters(&[("re", "{rule: {pattern: $B}, fix: '123'}")]);
+    let ret = compute_rewritten("[1, 2]", "[$B, $C]", rewrite, rewriters);
     assert_eq!(ret, None);
   }
 
   #[test]
   fn test_rewrite_use_enclosing_env() {
     let rewrite = Rewrite {
       source: "$A".into(),
       rewriters: str_vec!["re"],
       join_by: None,
     };
-    let rewriters = GlobalRules::default();
-    let serialized: SerializableRuleCore =
-      from_str("{rule: {pattern: $B}, fix: '$B == $C'}").unwrap();
-    let env = DeserializeEnv::new(TypeScript::Tsx).with_rewriters(&rewriters);
-    let mut vars = std::collections::HashSet::new();
+    let mut vars = HashSet::new();
     vars.insert("C");
-    let rule = serialized.get_rewriter(env, &vars).unwrap();
-    rewriters.insert("re", rule).unwrap();
-    let grep = TypeScript::Tsx.ast_grep("[1, 2]");
+    let rewriters =
+      make_rewriters_with_rewriter(&[("re", "{rule: {pattern: $B}, fix: '$B == $C'}")], vars);
+    let ret = apply_transformation(rewrite, "[1, 2]", "[$A, $C]", rewriters);
+    assert_eq!(ret, "1 == 2");
+  }
+
+  fn compute_rewritten(
+    src: &str,
+    pat: &str,
+    rewrite: Rewrite,
+    rewriters: GlobalRules<TypeScript>,
+  ) -> Option<String> {
+    let grep = TypeScript::Tsx.ast_grep(src);
     let root = grep.root();
-    let mut nm = root.find("[$A, $C]").expect("should find");
+    let mut nm = root.find(pat).expect("should find");
+    let before_vars: Vec<_> = nm.get_env().get_matched_variables().collect();
     let env = nm.get_env_mut();
     let enclosing = env.clone();
     let mut ctx = Ctx {
       lang: &TypeScript::Tsx,
       transforms: &Default::default(),
       env,
       rewriters,
       enclosing_env: &enclosing,
     };
-    let ret = rewrite.compute(&mut ctx);
-    assert_eq!(ret, Some("1 == 2".into()));
+    let after_vars: Vec<_> = ctx.env.get_matched_variables().collect();
+    assert_eq!(
+      before_vars, after_vars,
+      "rewrite should not write back to env"
+    );
+    rewrite.compute(&mut ctx)
   }
 }
```

### Comparing `ast_grep_py-0.21.2/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.21.3/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/Cargo.toml` & `ast_grep_py-0.21.3/crates/language/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/bash.rs` & `ast_grep_py-0.21.3/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/cpp.rs` & `ast_grep_py-0.21.3/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/csharp.rs` & `ast_grep_py-0.21.3/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/css.rs` & `ast_grep_py-0.21.3/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/elixir.rs` & `ast_grep_py-0.21.3/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/go.rs` & `ast_grep_py-0.21.3/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/html.rs` & `ast_grep_py-0.21.3/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/json.rs` & `ast_grep_py-0.21.3/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/kotlin.rs` & `ast_grep_py-0.21.3/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/lib.rs` & `ast_grep_py-0.21.3/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/lua.rs` & `ast_grep_py-0.21.3/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/parsers.rs` & `ast_grep_py-0.21.3/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/python.rs` & `ast_grep_py-0.21.3/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/ruby.rs` & `ast_grep_py-0.21.3/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/rust.rs` & `ast_grep_py-0.21.3/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/scala.rs` & `ast_grep_py-0.21.3/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/language/src/swift.rs` & `ast_grep_py-0.21.3/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/Cargo.toml` & `ast_grep_py-0.21.3/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/README.md` & `ast_grep_py-0.21.3/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.21.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/src/lib.rs` & `ast_grep_py-0.21.3/crates/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.21.3/crates/pyo3/src/py_node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/src/range.rs` & `ast_grep_py-0.21.3/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.21.3/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.21.3/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.21.3/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.21.3/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.21.3/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/Cargo.lock` & `ast_grep_py-0.21.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -139,15 +139,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -155,38 +155,38 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
@@ -208,29 +208,29 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -240,15 +240,15 @@
  "tree-sitter-html",
  "tree-sitter-javascript",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
@@ -306,15 +306,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.21.2"
+version = "0.21.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
```

### Comparing `ast_grep_py-0.21.2/Cargo.toml` & `ast_grep_py-0.21.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.21.2"
+version = "0.21.3"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
-rust-version = "1.63"
+rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.21.2" }
-ast-grep-config = { path = "crates/config", version = "0.21.2" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.21.2" }
-ast-grep-language = { path = "crates/language", version = "0.21.2" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.21.2" }
+ast-grep-core = { path = "crates/core", version = "0.21.3" }
+ast-grep-config = { path = "crates/config", version = "0.21.3" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.21.3" }
+ast-grep-language = { path = "crates/language", version = "0.21.3" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.21.3" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0", features = ["derive"] }
 tree-sitter = { version = "0.9.2", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
```

### Comparing `ast_grep_py-0.21.2/pyproject.toml` & `ast_grep_py-0.21.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.21.2"
+version = "0.21.3"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.21.2/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.21.3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/ast_grep_py/__init__.py` & `ast_grep_py-0.21.3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/README.md` & `ast_grep_py-0.21.3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.21.2/PKG-INFO` & `ast_grep_py-0.21.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.21.2
+Version: 0.21.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

