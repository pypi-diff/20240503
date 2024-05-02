# Comparing `tmp/mubble-1.0.0.tar.gz` & `tmp/mubble-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mubble-1.0.0.tar", max compression
+gzip compressed data, was "mubble-1.1.0.tar", max compression
```

## Comparing `mubble-1.0.0.tar` & `mubble-1.1.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     2957 2024-01-31 01:59:07.727926 mubble-1.0.0/mubble/__init__.py
--rw-r--r--   0        0        0      246 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/api/__init__.py
--rw-r--r--   0        0        0     1526 2024-01-31 02:19:30.748665 mubble-1.0.0/mubble/api/abc.py
--rw-r--r--   0        0        0     1964 2024-01-31 02:20:25.756446 mubble-1.0.0/mubble/api/api.py
--rw-r--r--   0        0        0      390 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/api/error.py
--rw-r--r--   0        0        0      480 2024-01-31 01:59:32.309553 mubble-1.0.0/mubble/api/response.py
--rw-r--r--   0        0        0     1550 2024-01-31 01:59:08.099595 mubble-1.0.0/mubble/bot/__init__.py
--rw-r--r--   0        0        0     2187 2024-01-31 01:59:29.990346 mubble-1.0.0/mubble/bot/bot.py
--rw-r--r--   0        0        0      295 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/cute_types/__init__.py
--rw-r--r--   0        0        0     1105 2024-01-31 01:59:32.258492 mubble-1.0.0/mubble/bot/cute_types/base.py
--rw-r--r--   0        0        0     2552 2024-01-31 01:59:32.239145 mubble-1.0.0/mubble/bot/cute_types/callback_query.py
--rw-r--r--   0        0        0     1334 2024-01-31 01:59:32.154609 mubble-1.0.0/mubble/bot/cute_types/inline_query.py
--rw-r--r--   0        0        0     5802 2024-01-31 01:59:32.139762 mubble-1.0.0/mubble/bot/cute_types/message.py
--rw-r--r--   0        0        0      525 2024-01-31 01:59:31.969134 mubble-1.0.0/mubble/bot/cute_types/update.py
--rw-r--r--   0        0        0     1312 2024-01-31 01:59:08.108597 mubble-1.0.0/mubble/bot/dispatch/__init__.py
--rw-r--r--   0        0        0      439 2024-01-31 01:59:30.201957 mubble-1.0.0/mubble/bot/dispatch/abc.py
--rw-r--r--   0        0        0     2539 2024-01-31 01:59:30.196367 mubble-1.0.0/mubble/bot/dispatch/composition.py
--rw-r--r--   0        0        0     2031 2024-01-31 01:59:30.050630 mubble-1.0.0/mubble/bot/dispatch/context.py
--rw-r--r--   0        0        0     3798 2024-01-31 01:59:30.118280 mubble-1.0.0/mubble/bot/dispatch/dispatch.py
--rw-r--r--   0        0        0      169 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/handler/__init__.py
--rw-r--r--   0        0        0      567 2024-01-31 01:59:30.231279 mubble-1.0.0/mubble/bot/dispatch/handler/abc.py
--rw-r--r--   0        0        0     2074 2024-01-31 01:59:30.343244 mubble-1.0.0/mubble/bot/dispatch/handler/func.py
--rw-r--r--   0        0        0     1399 2024-01-31 01:59:30.274884 mubble-1.0.0/mubble/bot/dispatch/handler/message_reply.py
--rw-r--r--   0        0        0       61 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/middleware/__init__.py
--rw-r--r--   0        0        0      411 2024-01-31 02:30:53.146152 mubble-1.0.0/mubble/bot/dispatch/middleware/abc.py
--rw-r--r--   0        0        0     2225 2024-01-31 01:59:30.082619 mubble-1.0.0/mubble/bot/dispatch/process.py
--rw-r--r--   0        0        0      447 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/return_manager/__init__.py
--rw-r--r--   0        0        0     3206 2024-01-31 01:59:30.945317 mubble-1.0.0/mubble/bot/dispatch/return_manager/abc.py
--rw-r--r--   0        0        0      610 2024-01-31 01:59:30.757937 mubble-1.0.0/mubble/bot/dispatch/return_manager/callback_query.py
--rw-r--r--   0        0        0      433 2024-01-31 01:59:30.777824 mubble-1.0.0/mubble/bot/dispatch/return_manager/inline_query.py
--rw-r--r--   0        0        0      818 2024-01-31 01:59:30.802584 mubble-1.0.0/mubble/bot/dispatch/return_manager/message.py
--rw-r--r--   0        0        0      379 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/view/__init__.py
--rw-r--r--   0        0        0     4481 2024-01-31 01:59:30.744615 mubble-1.0.0/mubble/bot/dispatch/view/abc.py
--rw-r--r--   0        0        0     1197 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/view/box.py
--rw-r--r--   0        0        0      682 2024-01-31 01:59:30.581705 mubble-1.0.0/mubble/bot/dispatch/view/callback_query.py
--rw-r--r--   0        0        0      509 2024-01-31 01:59:30.559505 mubble-1.0.0/mubble/bot/dispatch/view/inline_query.py
--rw-r--r--   0        0        0      480 2024-01-31 01:59:30.553014 mubble-1.0.0/mubble/bot/dispatch/view/message.py
--rw-r--r--   0        0        0      190 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/dispatch/waiter_machine/__init__.py
--rw-r--r--   0        0        0     3393 2024-01-31 01:59:30.541923 mubble-1.0.0/mubble/bot/dispatch/waiter_machine/machine.py
--rw-r--r--   0        0        0     2486 2024-01-31 01:59:30.451351 mubble-1.0.0/mubble/bot/dispatch/waiter_machine/middleware.py
--rw-r--r--   0        0        0     1086 2024-01-31 01:59:30.357222 mubble-1.0.0/mubble/bot/dispatch/waiter_machine/short_state.py
--rw-r--r--   0        0        0       94 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/polling/__init__.py
--rw-r--r--   0        0        0      434 2024-01-31 01:59:31.961063 mubble-1.0.0/mubble/bot/polling/abc.py
--rw-r--r--   0        0        0     4328 2024-01-31 01:59:31.949322 mubble-1.0.0/mubble/bot/polling/polling.py
--rw-r--r--   0        0        0     1938 2024-01-31 02:11:10.830407 mubble-1.0.0/mubble/bot/rules/__init__.py
--rw-r--r--   0        0        0     3611 2024-01-31 01:59:31.756443 mubble-1.0.0/mubble/bot/rules/abc.py
--rw-r--r--   0        0        0      231 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/rules/adapter/__init__.py
--rw-r--r--   0        0        0      536 2024-01-31 01:59:31.813207 mubble-1.0.0/mubble/bot/rules/adapter/abc.py
--rw-r--r--   0        0        0       73 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/rules/adapter/errors.py
--rw-r--r--   0        0        0     1176 2024-01-31 01:59:31.803498 mubble-1.0.0/mubble/bot/rules/adapter/event.py
--rw-r--r--   0        0        0      619 2024-01-31 01:59:31.767812 mubble-1.0.0/mubble/bot/rules/adapter/raw_update.py
--rw-r--r--   0        0        0     5637 2024-01-31 02:09:43.271792 mubble-1.0.0/mubble/bot/rules/callback_data.py
--rw-r--r--   0        0        0     3317 2024-01-31 02:17:55.846104 mubble-1.0.0/mubble/bot/rules/command.py
--rw-r--r--   0        0        0      932 2024-01-31 01:59:31.476298 mubble-1.0.0/mubble/bot/rules/enum_text.py
--rw-r--r--   0        0        0      697 2024-01-31 01:59:31.438401 mubble-1.0.0/mubble/bot/rules/func.py
--rw-r--r--   0        0        0      707 2024-01-31 01:59:31.208521 mubble-1.0.0/mubble/bot/rules/fuzzy.py
--rw-r--r--   0        0        0      975 2024-01-31 01:59:31.427263 mubble-1.0.0/mubble/bot/rules/inline.py
--rw-r--r--   0        0        0      526 2024-01-31 01:59:31.415900 mubble-1.0.0/mubble/bot/rules/integer.py
--rw-r--r--   0        0        0     4416 2024-01-31 01:59:31.251003 mubble-1.0.0/mubble/bot/rules/is_from.py
--rw-r--r--   0        0        0     1054 2024-01-31 01:59:31.396015 mubble-1.0.0/mubble/bot/rules/markup.py
--rw-r--r--   0        0        0      483 2024-01-31 01:59:31.263004 mubble-1.0.0/mubble/bot/rules/mention.py
--rw-r--r--   0        0        0     1048 2024-01-31 01:59:31.378114 mubble-1.0.0/mubble/bot/rules/message_entities.py
--rw-r--r--   0        0        0     1165 2024-01-31 01:59:31.363300 mubble-1.0.0/mubble/bot/rules/regex.py
--rw-r--r--   0        0        0     2087 2024-01-31 01:59:31.289821 mubble-1.0.0/mubble/bot/rules/rule_enum.py
--rw-r--r--   0        0        0     1186 2024-01-31 01:59:31.346143 mubble-1.0.0/mubble/bot/rules/start.py
--rw-r--r--   0        0        0     1137 2024-01-31 01:59:31.306207 mubble-1.0.0/mubble/bot/rules/text.py
--rw-r--r--   0        0        0      148 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/bot/scenario/__init__.py
--rw-r--r--   0        0        0      526 2024-01-31 01:59:31.196267 mubble-1.0.0/mubble/bot/scenario/abc.py
--rw-r--r--   0        0        0     3917 2024-01-31 01:59:31.182843 mubble-1.0.0/mubble/bot/scenario/checkbox.py
--rw-r--r--   0        0        0     1429 2024-01-31 01:59:30.981202 mubble-1.0.0/mubble/bot/scenario/choice.py
--rw-r--r--   0        0        0      130 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/client/__init__.py
--rw-r--r--   0        0        0     1177 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/client/abc.py
--rw-r--r--   0        0        0     3605 2024-01-31 01:59:32.293717 mubble-1.0.0/mubble/client/aiohttp.py
--rw-r--r--   0        0        0     7521 2024-01-31 01:59:26.461431 mubble-1.0.0/mubble/model.py
--rw-r--r--   0        0        0     7409 2024-01-31 01:59:26.403514 mubble-1.0.0/mubble/modules.py
--rw-r--r--   0        0        0      239 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/msgspec_json.py
--rw-r--r--   0        0        0      706 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/node/__init__.py
--rw-r--r--   0        0        0     2508 2024-01-31 01:59:29.933461 mubble-1.0.0/mubble/node/attachment.py
--rw-r--r--   0        0        0     2221 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/node/base.py
--rw-r--r--   0        0        0     2216 2024-01-31 01:59:29.863234 mubble-1.0.0/mubble/node/composer.py
--rw-r--r--   0        0        0      636 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/node/container.py
--rw-r--r--   0        0        0      410 2024-01-31 01:59:29.762804 mubble-1.0.0/mubble/node/message.py
--rw-r--r--   0        0        0     1705 2024-01-31 01:59:29.750594 mubble-1.0.0/mubble/node/rule.py
--rw-r--r--   0        0        0      863 2024-01-31 01:59:29.698732 mubble-1.0.0/mubble/node/source.py
--rw-r--r--   0        0        0      303 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/node/text.py
--rw-r--r--   0        0        0       57 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/node/tools/__init__.py
--rw-r--r--   0        0        0     1014 2024-01-31 01:59:29.970657 mubble-1.0.0/mubble/node/tools/generator.py
--rw-r--r--   0        0        0      248 2024-01-31 01:59:29.663595 mubble-1.0.0/mubble/node/update.py
--rw-r--r--   0        0        0      130 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/option/__init__.py
--rw-r--r--   0        0        0     1024 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/option/msgspec_option.py
--rw-r--r--   0        0        0     2351 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/option/option.py
--rw-r--r--   0        0        0     4929 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/result.py
--rw-r--r--   0        0        0       39 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/rules.py
--rw-r--r--   0        0        0     2678 2024-01-31 01:59:07.968357 mubble-1.0.0/mubble/tools/__init__.py
--rw-r--r--   0        0        0     1748 2024-01-31 01:59:28.327688 mubble-1.0.0/mubble/tools/buttons.py
--rw-r--r--   0        0        0      155 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/error_handler/__init__.py
--rw-r--r--   0        0        0      747 2024-01-31 01:59:29.655983 mubble-1.0.0/mubble/tools/error_handler/abc.py
--rw-r--r--   0        0        0     5367 2024-01-31 01:59:29.644723 mubble-1.0.0/mubble/tools/error_handler/error_handler.py
--rw-r--r--   0        0        0     1459 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/formatting/__init__.py
--rw-r--r--   0        0        0     8494 2024-01-31 01:59:29.505250 mubble-1.0.0/mubble/tools/formatting/html.py
--rw-r--r--   0        0        0      852 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/formatting/links.py
--rw-r--r--   0        0        0     2302 2024-01-31 01:59:29.215716 mubble-1.0.0/mubble/tools/formatting/spec_html_formats.py
--rw-r--r--   0        0        0      267 2024-01-31 01:59:28.640028 mubble-1.0.0/mubble/tools/global_context/__init__.py
--rw-r--r--   0        0        0     1628 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/global_context/abc.py
--rw-r--r--   0        0        0    13884 2024-01-31 01:59:29.149193 mubble-1.0.0/mubble/tools/global_context/global_context.py
--rw-r--r--   0        0        0      597 2024-01-31 01:59:28.652029 mubble-1.0.0/mubble/tools/global_context/mubble_ctx.py
--rw-r--r--   0        0        0      288 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/i18n/__init__.py
--rw-r--r--   0        0        0      637 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/i18n/base.py
--rw-r--r--   0        0        0       82 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/i18n/middleware/__init__.py
--rw-r--r--   0        0        0      670 2024-01-31 01:59:28.636032 mubble-1.0.0/mubble/tools/i18n/middleware/base.py
--rw-r--r--   0        0        0     1609 2024-01-31 01:59:28.619143 mubble-1.0.0/mubble/tools/i18n/simple.py
--rw-r--r--   0        0        0      156 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/kb_set/__init__.py
--rw-r--r--   0        0        0      243 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/kb_set/base.py
--rw-r--r--   0        0        0     2042 2024-01-31 01:59:28.596551 mubble-1.0.0/mubble/tools/kb_set/yaml.py
--rw-r--r--   0        0        0     3646 2024-01-31 01:59:28.246828 mubble-1.0.0/mubble/tools/keyboard.py
--rw-r--r--   0        0        0      143 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/loop_wrapper/__init__.py
--rw-r--r--   0        0        0      405 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/loop_wrapper/abc.py
--rw-r--r--   0        0        0     4273 2024-01-31 01:59:28.449523 mubble-1.0.0/mubble/tools/loop_wrapper/loop_wrapper.py
--rw-r--r--   0        0        0     1796 2024-01-31 01:59:28.126025 mubble-1.0.0/mubble/tools/magic.py
--rw-r--r--   0        0        0       92 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/tools/parse_mode.py
--rw-r--r--   0        0        0       68 2024-01-31 01:59:26.404513 mubble-1.0.0/mubble/types/__init__.py
--rw-r--r--   0        0        0    18789 2024-01-30 20:58:47.000000 mubble-1.0.0/mubble/types/enums.py
--rw-r--r--   0        0        0   178844 2024-01-31 01:59:27.999972 mubble-1.0.0/mubble/types/methods.py
--rw-r--r--   0        0        0   199436 2024-01-31 01:59:26.890806 mubble-1.0.0/mubble/types/objects.py
--rw-r--r--   0        0        0      612 2024-01-31 02:07:46.772890 mubble-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3191 2024-01-31 02:18:27.247405 mubble-1.0.0/README.md
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 mubble-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3548 2024-05-02 22:55:28.226035 mubble-1.1.0/mubble/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/api/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-02 22:54:23.849867 mubble-1.1.0/mubble/api/abc.py
+-rw-r--r--   0        0        0     2422 2024-05-02 22:54:23.963848 mubble-1.1.0/mubble/api/api.py
+-rw-r--r--   0        0        0      425 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/api/error.py
+-rw-r--r--   0        0        0      481 2024-05-02 22:54:23.963848 mubble-1.1.0/mubble/api/response.py
+-rw-r--r--   0        0        0     1550 2024-05-02 22:55:28.682678 mubble-1.1.0/mubble/bot/__init__.py
+-rw-r--r--   0        0        0     2451 2024-05-02 22:55:28.834481 mubble-1.1.0/mubble/bot/bot.py
+-rw-r--r--   0        0        0      295 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/cute_types/__init__.py
+-rw-r--r--   0        0        0     4532 2024-05-02 22:54:23.983849 mubble-1.1.0/mubble/bot/cute_types/base.py
+-rw-r--r--   0        0        0    20250 2024-05-02 22:54:23.983849 mubble-1.1.0/mubble/bot/cute_types/callback_query.py
+-rw-r--r--   0        0        0     2456 2024-05-02 23:05:07.158195 mubble-1.1.0/mubble/bot/cute_types/inline_query.py
+-rw-r--r--   0        0        0   140740 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/cute_types/message.py
+-rw-r--r--   0        0        0      737 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/cute_types/update.py
+-rw-r--r--   0        0        0    16339 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/cute_types/utils.py
+-rw-r--r--   0        0        0     1312 2024-05-02 22:55:28.965892 mubble-1.1.0/mubble/bot/dispatch/__init__.py
+-rw-r--r--   0        0        0      447 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/dispatch/abc.py
+-rw-r--r--   0        0        0     2943 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/dispatch/composition.py
+-rw-r--r--   0        0        0     2317 2024-05-02 22:54:24.126618 mubble-1.1.0/mubble/bot/dispatch/context.py
+-rw-r--r--   0        0        0     5031 2024-05-02 22:55:28.892548 mubble-1.1.0/mubble/bot/dispatch/dispatch.py
+-rw-r--r--   0        0        0      169 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/handler/__init__.py
+-rw-r--r--   0        0        0      549 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/handler/abc.py
+-rw-r--r--   0        0        0     2329 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/handler/func.py
+-rw-r--r--   0        0        0     1787 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/handler/message_reply.py
+-rw-r--r--   0        0        0       61 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/middleware/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/middleware/abc.py
+-rw-r--r--   0        0        0     2273 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/process.py
+-rw-r--r--   0        0        0      447 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/return_manager/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/return_manager/abc.py
+-rw-r--r--   0        0        0      646 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/return_manager/callback_query.py
+-rw-r--r--   0        0        0      474 2024-05-02 22:54:24.127612 mubble-1.1.0/mubble/bot/dispatch/return_manager/inline_query.py
+-rw-r--r--   0        0        0     1124 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/return_manager/message.py
+-rw-r--r--   0        0        0      379 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/view/__init__.py
+-rw-r--r--   0        0        0     5504 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/view/abc.py
+-rw-r--r--   0        0        0     1252 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/view/box.py
+-rw-r--r--   0        0        0      626 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/view/callback_query.py
+-rw-r--r--   0        0        0      521 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/view/inline_query.py
+-rw-r--r--   0        0        0      488 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/view/message.py
+-rw-r--r--   0        0        0      190 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/dispatch/waiter_machine/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/waiter_machine/machine.py
+-rw-r--r--   0        0        0     2531 2024-05-02 22:54:24.145801 mubble-1.1.0/mubble/bot/dispatch/waiter_machine/middleware.py
+-rw-r--r--   0        0        0     1180 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/dispatch/waiter_machine/short_state.py
+-rw-r--r--   0        0        0       94 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/polling/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/polling/abc.py
+-rw-r--r--   0        0        0     4687 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/polling/polling.py
+-rw-r--r--   0        0        0     2111 2024-05-02 22:58:24.697586 mubble-1.1.0/mubble/bot/rules/__init__.py
+-rw-r--r--   0        0        0     3641 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/abc.py
+-rw-r--r--   0        0        0      231 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/rules/adapter/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-02 22:54:24.832675 mubble-1.1.0/mubble/bot/rules/adapter/abc.py
+-rw-r--r--   0        0        0       73 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/rules/adapter/errors.py
+-rw-r--r--   0        0        0     1674 2024-05-02 22:54:24.832675 mubble-1.1.0/mubble/bot/rules/adapter/event.py
+-rw-r--r--   0        0        0      727 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/bot/rules/adapter/raw_update.py
+-rw-r--r--   0        0        0     5565 2024-05-02 22:59:21.110587 mubble-1.1.0/mubble/bot/rules/callback_data.py
+-rw-r--r--   0        0        0     3300 2024-05-02 23:03:05.687459 mubble-1.1.0/mubble/bot/rules/command.py
+-rw-r--r--   0        0        0      896 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/enum_text.py
+-rw-r--r--   0        0        0      697 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/func.py
+-rw-r--r--   0        0        0      707 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/fuzzy.py
+-rw-r--r--   0        0        0     1925 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/inline.py
+-rw-r--r--   0        0        0      526 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/integer.py
+-rw-r--r--   0        0        0     5238 2024-05-02 22:54:24.142577 mubble-1.1.0/mubble/bot/rules/is_from.py
+-rw-r--r--   0        0        0     1090 2024-05-02 22:55:28.682678 mubble-1.1.0/mubble/bot/rules/markup.py
+-rw-r--r--   0        0        0      483 2024-05-02 22:54:24.809615 mubble-1.1.0/mubble/bot/rules/mention.py
+-rw-r--r--   0        0        0     1081 2024-05-02 22:59:56.078140 mubble-1.1.0/mubble/bot/rules/message_entities.py
+-rw-r--r--   0        0        0     1186 2024-05-02 22:54:24.811616 mubble-1.1.0/mubble/bot/rules/regex.py
+-rw-r--r--   0        0        0     2078 2024-05-02 22:54:24.811616 mubble-1.1.0/mubble/bot/rules/rule_enum.py
+-rw-r--r--   0        0        0     1173 2024-05-02 22:54:24.832675 mubble-1.1.0/mubble/bot/rules/start.py
+-rw-r--r--   0        0        0     1140 2024-05-02 23:00:45.378324 mubble-1.1.0/mubble/bot/rules/text.py
+-rw-r--r--   0        0        0      166 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/bot/scenario/__init__.py
+-rw-r--r--   0        0        0      459 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/bot/scenario/abc.py
+-rw-r--r--   0        0        0     4167 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/bot/scenario/checkbox.py
+-rw-r--r--   0        0        0     1427 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/bot/scenario/choice.py
+-rw-r--r--   0        0        0      104 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/client/__init__.py
+-rw-r--r--   0        0        0     1611 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/client/abc.py
+-rw-r--r--   0        0        0     4137 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/client/aiohttp.py
+-rw-r--r--   0        0        0     4670 2024-05-02 22:54:23.837867 mubble-1.1.0/mubble/model.py
+-rw-r--r--   0        0        0     7822 2024-05-02 22:55:28.316667 mubble-1.1.0/mubble/modules.py
+-rw-r--r--   0        0        0      226 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/msgspec_json.py
+-rw-r--r--   0        0        0     8214 2024-05-02 23:06:26.577443 mubble-1.1.0/mubble/msgspec_utils.py
+-rw-r--r--   0        0        0      706 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/node/__init__.py
+-rw-r--r--   0        0        0     2507 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/attachment.py
+-rw-r--r--   0        0        0     2220 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/node/base.py
+-rw-r--r--   0        0        0     2230 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/composer.py
+-rw-r--r--   0        0        0      636 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/node/container.py
+-rw-r--r--   0        0        0      410 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/message.py
+-rw-r--r--   0        0        0     1699 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/rule.py
+-rw-r--r--   0        0        0      726 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/source.py
+-rw-r--r--   0        0        0      303 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/node/text.py
+-rw-r--r--   0        0        0       57 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/node/tools/__init__.py
+-rw-r--r--   0        0        0     1015 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/tools/generator.py
+-rw-r--r--   0        0        0      248 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/node/update.py
+-rw-r--r--   0        0        0       39 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/rules.py
+-rw-r--r--   0        0        0     2894 2024-05-02 22:55:28.349624 mubble-1.1.0/mubble/tools/__init__.py
+-rw-r--r--   0        0        0     2415 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/tools/buttons.py
+-rw-r--r--   0        0        0      207 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/error_handler/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-02 22:54:24.979912 mubble-1.1.0/mubble/tools/error_handler/abc.py
+-rw-r--r--   0        0        0      188 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/error_handler/error.py
+-rw-r--r--   0        0        0     5972 2024-05-02 22:54:24.979912 mubble-1.1.0/mubble/tools/error_handler/error_handler.py
+-rw-r--r--   0        0        0     1609 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/formatting/__init__.py
+-rw-r--r--   0        0        0     8570 2024-05-02 22:54:24.979912 mubble-1.1.0/mubble/tools/formatting/html.py
+-rw-r--r--   0        0        0     1334 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/formatting/links.py
+-rw-r--r--   0        0        0     2742 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/formatting/spec_html_formats.py
+-rw-r--r--   0        0        0      267 2024-05-02 22:55:28.681678 mubble-1.1.0/mubble/tools/global_context/__init__.py
+-rw-r--r--   0        0        0     1644 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/global_context/abc.py
+-rw-r--r--   0        0        0    13937 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/global_context/global_context.py
+-rw-r--r--   0        0        0      597 2024-05-02 22:55:28.357622 mubble-1.1.0/mubble/tools/global_context/mubble_ctx.py
+-rw-r--r--   0        0        0      288 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/i18n/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/i18n/base.py
+-rw-r--r--   0        0        0       82 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/i18n/middleware/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/i18n/middleware/base.py
+-rw-r--r--   0        0        0     1609 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/i18n/simple.py
+-rw-r--r--   0        0        0      156 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/kb_set/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/kb_set/base.py
+-rw-r--r--   0        0        0     2022 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/kb_set/yaml.py
+-rw-r--r--   0        0        0     3728 2024-05-02 22:54:24.956100 mubble-1.1.0/mubble/tools/keyboard.py
+-rw-r--r--   0        0        0      165 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/loop_wrapper/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/loop_wrapper/abc.py
+-rw-r--r--   0        0        0     5697 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/tools/loop_wrapper/loop_wrapper.py
+-rw-r--r--   0        0        0     1851 2024-05-02 22:54:24.979912 mubble-1.1.0/mubble/tools/magic.py
+-rw-r--r--   0        0        0       92 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/tools/parse_mode.py
+-rw-r--r--   0        0        0       68 2024-05-02 22:54:24.980901 mubble-1.1.0/mubble/types/__init__.py
+-rw-r--r--   0        0        0    18330 2024-04-27 19:57:12.000000 mubble-1.1.0/mubble/types/enums.py
+-rw-r--r--   0        0        0   186365 2024-05-02 22:54:24.982910 mubble-1.1.0/mubble/types/methods.py
+-rw-r--r--   0        0        0   214788 2024-05-02 22:54:25.054911 mubble-1.1.0/mubble/types/objects.py
+-rw-r--r--   0        0        0     1012 2024-05-02 22:54:23.837867 mubble-1.1.0/mubble/verification_utils.py
+-rw-r--r--   0        0        0      638 2024-05-02 23:10:23.559656 mubble-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3514 2024-01-31 03:49:49.005545 mubble-1.1.0/README.md
+-rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 mubble-1.1.0/PKG-INFO
```

### Comparing `mubble-1.0.0/mubble/__init__.py` & `mubble-1.1.0/mubble/bot/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,76 @@
-from .api import ABCAPI, API, APIError, APIResponse, Token
-from .bot import (
+from .bot import Mubble
+from .cute_types import (
+    BaseCute,
+    CallbackQueryCute,
+    InlineQueryCute,
+    MessageCute,
+    UpdateCute,
+)
+from .dispatch import (
     ABCDispatch,
     ABCHandler,
     ABCMiddleware,
-    ABCPolling,
     ABCReturnManager,
-    ABCRule,
-    ABCScenario,
     ABCStateView,
     ABCView,
-    BaseCute,
     BaseReturnManager,
     BaseStateView,
     BaseView,
-    CallbackQueryCute,
     CallbackQueryReturnManager,
     CallbackQueryView,
-    Checkbox,
+    CompositionDispatch,
+    Context,
     Dispatch,
     FuncHandler,
-    InlineQueryCute,
     InlineQueryReturnManager,
-    MessageCute,
+    Manager,
     MessageReplyHandler,
     MessageReturnManager,
-    MessageRule,
     MessageView,
-    Polling,
-    SingleChoice,
-    Mubble,
     ViewBox,
     WaiterMachine,
     register_manager,
 )
-from .client import ABCClient, AiohttpClient
-from .model import Model, decoder, encoder
-from .modules import logger
-from .option import Nothing, NothingType, Option, Some
-from .result import Error, Ok, Result
-from .tools import (
-    ABCGlobalContext,
-    ABCLoopWrapper,
-    ABCTranslator,
-    ABCTranslatorMiddleware,
-    AnyMarkup,
-    Button,
-    CtxVar,
-    DelayedTask,
-    FormatString,
-    GlobalContext,
-    HTMLFormatter,
-    I18nEnum,
-    InlineButton,
-    InlineKeyboard,
-    Keyboard,
-    KeyboardSetBase,
-    KeyboardSetYAML,
-    LoopWrapper,
-    ParseMode,
-    RowButtons,
-    SimpleI18n,
-    SimpleTranslator,
-    ctx_var,
-    keyboard_remove,
-    magic_bundle,
-)
-
-Message = MessageCute
-CallbackQuery = CallbackQueryCute
-InlineQuery = InlineQueryCute
-Bot = Mubble
-
+from .polling import ABCPolling, Polling
+from .rules import ABCRule, CallbackQueryRule, MessageRule
+from .scenario import ABCScenario, Checkbox, SingleChoice
 
 __all__ = (
-    "ABCAPI",
-    "ABCClient",
     "ABCDispatch",
-    "ABCGlobalContext",
     "ABCHandler",
-    "ABCLoopWrapper",
     "ABCMiddleware",
     "ABCPolling",
     "ABCReturnManager",
     "ABCRule",
     "ABCScenario",
     "ABCStateView",
-    "ABCTranslator",
-    "ABCTranslatorMiddleware",
     "ABCView",
-    "API",
-    "APIError",
-    "APIResponse",
-    "AiohttpClient",
-    "AnyMarkup",
     "BaseCute",
     "BaseReturnManager",
     "BaseStateView",
     "BaseView",
-    "Bot",
-    "Button",
-    "CallbackQuery",
     "CallbackQueryCute",
     "CallbackQueryReturnManager",
+    "CallbackQueryRule",
     "CallbackQueryView",
     "Checkbox",
-    "CtxVar",
-    "DelayedTask",
+    "CompositionDispatch",
+    "Context",
     "Dispatch",
-    "Error",
-    "FormatString",
     "FuncHandler",
-    "GlobalContext",
-    "HTMLFormatter",
-    "I18nEnum",
-    "InlineButton",
-    "InlineKeyboard",
-    "InlineQuery",
     "InlineQueryCute",
     "InlineQueryReturnManager",
-    "Keyboard",
-    "KeyboardSetBase",
-    "KeyboardSetYAML",
-    "LoopWrapper",
-    "Message",
+    "Manager",
     "MessageCute",
     "MessageReplyHandler",
     "MessageReturnManager",
     "MessageRule",
     "MessageView",
-    "Model",
-    "Nothing",
-    "NothingType",
-    "Ok",
-    "Option",
-    "ParseMode",
     "Polling",
-    "Result",
-    "RowButtons",
-    "SimpleI18n",
-    "SimpleTranslator",
     "SingleChoice",
-    "Some",
     "Mubble",
-    "Token",
+    "UpdateCute",
     "ViewBox",
     "WaiterMachine",
-    "ctx_var",
-    "decoder",
-    "encoder",
-    "keyboard_remove",
-    "logger",
-    "magic_bundle",
     "register_manager",
 )
```

### Comparing `mubble-1.0.0/mubble/api/abc.py` & `mubble-1.1.0/mubble/api/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import pathlib
 import typing
 from abc import ABC, abstractmethod
 
 import msgspec
 from envparse import env
+from fntypes.result import Result
 
 from mubble.api.error import APIError
 from mubble.client import ABCClient
-from mubble.result import Result
 
 from .error import InvalidTokenError
 
 
 class Token(str):
     def __new__(cls, token: str) -> typing.Self:
         if token.count(":") != 1 or not token.split(":")[0].isdigit():
-            raise InvalidTokenError(
-                "Invalid token, it should look like this '123:abc'."
-            )
+            raise InvalidTokenError("Invalid token, it should look like this '123:ABC'.")
         return super().__new__(cls, token)
+    
+    def __repr__(self) -> str:
+        return f"<Token: {self.bot_id}:{''.join(self.split(':')[-1])[:6]}...>"
 
     @classmethod
     def from_env(
         cls,
         var_name: str = "BOT_TOKEN",
         *,
         is_read: bool = False,
@@ -40,23 +41,25 @@
 class ABCAPI(ABC):
     http: ABCClient
 
     @abstractmethod
     async def request(
         self,
         method: str,
-        data: dict | None = None,
-    ) -> Result[list | dict | bool, APIError]:
+        data: dict[str, typing.Any] | None = None,
+        files: dict[str, tuple[str, bytes]] | None = None,
+    ) -> Result[list[typing.Any] | dict[str, typing.Any] | bool, APIError]:
         pass
 
     @abstractmethod
     async def request_raw(
         self,
         method: str,
-        data: dict | None = None,
+        data: dict[str, typing.Any] | None = None,
+        files: dict[str, tuple[str, bytes]] | None = None,
     ) -> Result[msgspec.Raw, APIError]:
         pass
 
     @property
     @abstractmethod
     def request_url(self) -> str:
         pass
```

### Comparing `mubble-1.0.0/mubble/api/api.py` & `mubble-1.1.0/mubble/api/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 import typing
 
 import msgspec
+from fntypes.result import Error, Ok, Result
 
 from mubble.api.response import APIResponse
 from mubble.client import ABCClient, AiohttpClient
-from mubble.model import convert, decoder
-from mubble.result import Error, Ok, Result
+from mubble.model import DataConverter, decoder
 from mubble.types.methods import APIMethods
 
 from .abc import ABCAPI, APIError, Token
 
 
-def compose_data(client: ABCClient, data: dict[str, typing.Any]) -> typing.Any:
-    data = {k: convert(v) for k, v in data.items()}
-    if any(isinstance(v, tuple) for v in data.values()):
-        data = client.get_form(data)
-    return data
+def compose_data(
+    client: ABCClient,
+    data: dict[str, typing.Any],
+    files: dict[str, tuple[str, bytes]],
+) -> typing.Any:
+    converter = DataConverter(files=files.copy())
+    return client.get_form(
+        data={k: converter(v) for k, v in data.items()},
+        files=converter.files,
+    )
 
 
 class API(ABCAPI, APIMethods):
-    API_URL: typing.ClassVar[str] = "https://api.telegram.org/"
+    """Bot API with available API methods."""
 
-    def __init__(self, token: Token, *, http: ABCClient | None = None):
+    API_URL = "https://api.telegram.org/"
+
+    def __init__(self, token: Token, *, http: ABCClient | None = None) -> None:
         self.token = token
         self.http = http or AiohttpClient()
         super().__init__(self)
+    
+    def __repr__(self) -> str:
+        return "<{}: token={!r}, http={!r}>".format(
+            self.__class__.__name__,
+            self.token,
+            self.http,
+        )
 
     @property
     def id(self) -> int:
         return self.token.bot_id
 
     @property
     def request_url(self) -> str:
         return self.API_URL + f"bot{self.token}/"
 
     async def request(
         self,
         method: str,
-        data: dict | None = None,
-    ) -> Result[dict | list | bool, APIError]:
-        data = compose_data(self.http, data or {})
-        response = await self.http.request_json(self.request_url + method, data=data)
-
+        data: dict[str, typing.Any] | None = None,
+        files: dict[str, tuple[str, bytes]] | None = None,
+    ) -> Result[dict[str, typing.Any] | list[typing.Any] | bool, APIError]:
+        response = await self.http.request_json(
+            url=self.request_url + method,
+            data=compose_data(self.http, data or {}, files or {})
+        )
         if response.get("ok"):
             assert "result" in response
             return Ok(response["result"])
-        
-        return Error(
-            APIError(
-                code=response.get("error_code", -1),
-                error=response.get("description"),
-            )
-        )
+        return Error(APIError(
+            code=response.get("error_code", 400),
+            error=response.get("description"),
+        ))
 
     async def request_raw(
         self,
         method: str,
         data: dict[str, typing.Any] | None = None,
+        files: dict[str, tuple[str, bytes]] | None = None,
     ) -> Result[msgspec.Raw, APIError]:
         response_bytes = await self.http.request_bytes(
-            self.request_url + method, data=compose_data(self.http, data or {})
+            url=self.request_url + method,
+            data=compose_data(self.http, data or {}, files or {}),
         )
-        
         return decoder.decode(response_bytes, type=APIResponse).to_result()
 
 
 __all__ = ("API",)
```

### Comparing `mubble-1.0.0/mubble/bot/__init__.py` & `mubble-1.1.0/mubble/bot/dispatch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,58 @@
-from .bot import Mubble
-from .cute_types import (
-    BaseCute,
-    CallbackQueryCute,
-    InlineQueryCute,
-    MessageCute,
-    UpdateCute,
-)
-from .dispatch import (
-    ABCDispatch,
-    ABCHandler,
-    ABCMiddleware,
+from .abc import ABCDispatch
+from .composition import CompositionDispatch
+from .context import Context
+from .dispatch import ABCRule, Dispatch, MubbleCtx
+from .handler import ABCHandler, FuncHandler, MessageReplyHandler
+from .middleware import ABCMiddleware
+from .process import check_rule, process_inner
+from .return_manager import (
     ABCReturnManager,
-    ABCStateView,
-    ABCView,
     BaseReturnManager,
-    BaseStateView,
-    BaseView,
     CallbackQueryReturnManager,
-    CallbackQueryView,
-    CompositionDispatch,
-    Context,
-    Dispatch,
-    FuncHandler,
     InlineQueryReturnManager,
     Manager,
-    MessageReplyHandler,
     MessageReturnManager,
+    register_manager,
+)
+from .view import (
+    ABCStateView,
+    ABCView,
+    BaseStateView,
+    BaseView,
+    CallbackQueryView,
+    InlineQueryView,
     MessageView,
     ViewBox,
-    WaiterMachine,
-    register_manager,
 )
-from .polling import ABCPolling, Polling
-from .rules import ABCRule, CallbackQueryRule, MessageRule
-from .scenario import ABCScenario, Checkbox, SingleChoice
+from .waiter_machine import WaiterMachine
 
 __all__ = (
     "ABCDispatch",
     "ABCHandler",
     "ABCMiddleware",
-    "ABCPolling",
     "ABCReturnManager",
     "ABCRule",
-    "ABCScenario",
     "ABCStateView",
     "ABCView",
-    "BaseCute",
     "BaseReturnManager",
     "BaseStateView",
     "BaseView",
-    "CallbackQueryCute",
     "CallbackQueryReturnManager",
-    "CallbackQueryRule",
     "CallbackQueryView",
-    "Checkbox",
     "CompositionDispatch",
     "Context",
     "Dispatch",
     "FuncHandler",
-    "InlineQueryCute",
     "InlineQueryReturnManager",
+    "InlineQueryView",
     "Manager",
-    "MessageCute",
     "MessageReplyHandler",
     "MessageReturnManager",
-    "MessageRule",
     "MessageView",
-    "Polling",
-    "SingleChoice",
-    "Mubble",
-    "UpdateCute",
+    "MubbleCtx",
     "ViewBox",
     "WaiterMachine",
+    "check_rule",
+    "process_inner",
     "register_manager",
 )
```

### Comparing `mubble-1.0.0/mubble/bot/bot.py` & `mubble-1.1.0/mubble/bot/bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,52 +8,59 @@
 
 DispatchT = typing.TypeVar("DispatchT", bound=ABCDispatch, default=Dispatch)
 PollingT = typing.TypeVar("PollingT", bound=ABCPolling, default=Polling)
 LoopWrapperT = typing.TypeVar("LoopWrapperT", bound=ABCLoopWrapper, default=LoopWrapper)
 
 
 class Mubble(typing.Generic[DispatchT, PollingT, LoopWrapperT]):
-    dispatch: DispatchT
-    polling: PollingT
-    loop_wrapper: LoopWrapperT
-
     def __init__(
         self,
         api: API,
         *,
         polling: PollingT | None = None,
         dispatch: DispatchT | None = None,
         loop_wrapper: LoopWrapperT | None = None,
-    ):
+    ) -> None:
         self.api = api
-        self.dispatch = dispatch or Dispatch()  # type: ignore
-        self.polling = polling or Polling(api)  # type: ignore
-        self.loop_wrapper = loop_wrapper or LoopWrapper()  # type: ignore
+        self.dispatch = typing.cast(DispatchT, dispatch or Dispatch())
+        self.polling = typing.cast(PollingT, polling or Polling(api))
+        self.loop_wrapper = typing.cast(LoopWrapperT, loop_wrapper or LoopWrapper())
+
+    def __repr__(self) -> str:
+        return "<{}: api={!r}, dispatch={!r}, polling={!r}, loop_wrapper={!r}>".format(
+            self.__class__.__name__,
+            self.api,
+            self.dispatch,
+            self.polling,
+            self.loop_wrapper,
+        )
 
     @property
     def on(self) -> DispatchT:
         return self.dispatch
 
     async def reset_webhook(self) -> None:
         if not (await self.api.get_webhook_info()).unwrap().url:
             return
         await self.api.delete_webhook()
 
-    async def run_polling(self, offset: int = 0, skip_updates: bool = False) -> None:
+    async def run_polling(self, *, offset: int = 0, skip_updates: bool = False) -> None:
         if skip_updates:
             logger.debug("Dropping pending updates")
             await self.reset_webhook()
             await self.api.delete_webhook(drop_pending_updates=True)
         self.polling.offset = offset
 
         async for updates in self.polling.listen():
             for update in updates:
                 logger.debug("Received update (update_id={})", update.update_id)
                 self.loop_wrapper.add_task(self.dispatch.feed(update, self.api))
 
-    def run_forever(self, offset: int = 0, skip_updates: bool = False) -> None:
+    def run_forever(self, *, offset: int = 0, skip_updates: bool = False) -> None:
         logger.debug("Running blocking polling (id={})", self.api.id)
-        self.loop_wrapper.add_task(self.run_polling(offset, skip_updates=skip_updates))
+        self.loop_wrapper.add_task(
+            self.run_polling(offset=offset, skip_updates=skip_updates)
+        )
         self.loop_wrapper.run_event_loop()
 
 
 __all__ = ("Mubble",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/composition.py` & `mubble-1.1.0/mubble/bot/dispatch/composition.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,56 +22,67 @@
     def __init__(self, func: typing.Callable, is_blocking: bool) -> None:
         self.func = func
         self.nodes = {
             name: parameter.annotation
             for name, parameter in inspect.signature(func).parameters.items()
         }
         self.is_blocking = is_blocking
-
+    
+    def __repr__(self) -> str:
+        return "<{}: for function={!r} with nodes={}>".format(
+            ("blocking " if self.is_blocking else "")
+            + self.__class__.__name__,
+            self.func.__name__,
+            self.nodes,
+        )
+    
     async def compose_nodes(self, update: UpdateCute) -> NodeCollection | None:
         nodes: dict[str, NodeSession] = {}
         for name, node_t in self.nodes.items():
             try:
                 nodes[name] = await compose_node(node_t, update)
-            except ComposeError as err:
+            except ComposeError:
                 await NodeCollection(nodes).close_all()
                 return None
         return NodeCollection(nodes)
-
-    async def __call__(self, **kwargs) -> typing.Any:
+    
+    async def __call__(self, **kwargs: typing.Any) -> typing.Any:
         return await self.func(**magic_bundle(self.func, kwargs, start_idx=0, bundle_ctx=False))  # type: ignore
 
 
 class CompositionDispatch(ABCDispatch):
     def __init__(self) -> None:
         self.compositions: list[Composition] = []
+    
+    def __repr__(self) -> str:
+        return "<{}: with compositions={!r}>".format(
+            self.__class__.__name__,
+            self.compositions,
+        )
 
     async def feed(self, event: Update, api: ABCAPI) -> bool:
         update = UpdateCute(**event.to_dict(), api=api)
         is_found = False
         for composition in self.compositions:
             nodes = await composition.compose_nodes(update)
             if nodes is not None:
                 result = await composition(**nodes.values())
                 await nodes.close_all(with_value=result)
                 if composition.is_blocking:
                     return True
                 is_found = True
         return is_found
-
+    
     def load(self, external: typing.Self):
         self.compositions.extend(external.compositions)
 
     def __call__(self, *container_nodes: type[Node], is_blocking: bool = True):
         def wrapper(func: typing.Callable):
             composition = Composition(func, is_blocking)
             if container_nodes:
-                composition.nodes["container"] = ContainerNode.link_nodes(
-                    list(container_nodes)
-                )
+                composition.nodes["container"] = ContainerNode.link_nodes(list(container_nodes))
             self.compositions.append(composition)
             return func
-
         return wrapper
 
 
 __all__ = ("Composition", "CompositionDispatch")
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/context.py` & `mubble-1.1.0/mubble/node/composer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-import enum
 import typing
 
-from mubble.types import Update
+from mubble.bot.cute_types import UpdateCute
+from mubble.node import Node
 
-Key: typing.TypeAlias = str | enum.Enum
-AnyValue: typing.TypeAlias = typing.Any
 
+class NodeSession:
+    def __init__(
+        self, 
+        value: typing.Any,
+        subnodes: dict[str, typing.Self],
+        generator: typing.AsyncGenerator[typing.Any, None] | None = None,
+    ):
+        self.value = value
+        self.subnodes = subnodes
+        self.generator = generator
+    
+    async def close(self, with_value: typing.Any | None = None) -> None:
+        for subnode in self.subnodes.values():
+            await subnode.close()
+        
+        if self.generator is None:
+            return
+        try:
+            await self.generator.asend(with_value)
+        except StopAsyncIteration:
+            self.generator = None
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {self.value}" + ("ACTIVE>" if self.generator else ">")
+
+
+class NodeCollection:
+    def __init__(self, sessions: dict[str, NodeSession]) -> None:
+        self.sessions = sessions
+
+    def values(self) -> dict[str, typing.Any]:
+        return {name: session.value for name, session in self.sessions.items()}
+    
+    async def close_all(self, with_value: typing.Any | None = None) -> None:
+        for session in self.sessions.values():
+            await session.close(with_value)
+
+
+async def compose_node(
+    node: type[Node],
+    update: UpdateCute,
+    ready_context: dict[str, NodeSession] | None = None,
+) -> NodeSession:
+    _node = node.as_node()
+    context = NodeCollection(ready_context.copy() if ready_context else {})
+
+    for name, subnode in _node.get_sub_nodes().items():
+        if subnode is UpdateCute:
+            context.sessions[name] = NodeSession(update, {})
+        else:
+            context.sessions[name] = await compose_node(subnode, update)
+
+    generator: typing.AsyncGenerator | None
+
+    if _node.is_generator():
+        generator = typing.cast(typing.AsyncGenerator, _node.compose(**context.values()))
+        value = await generator.asend(None)
+    else:
+        generator = None
+        value = await _node.compose(**context.values())  # type: ignore
+    
+    return NodeSession(value, context.sessions, generator)
 
-@typing.dataclass_transform(kw_only_default=True, order_default=True)
-class Context(dict[str, AnyValue]):
-    """Context class for rules and middlewares.
-    ```
-    class MyRule(ABCRule[T]):
-        adapter: ABCAdapter[Update, T] = RawUpdateAdapter()
 
-        async def check(self, event: T, ctx: Context) -> bool:
-            ctx.set("value", (await event.ctx_api.get_me()).unwrap())
-            return True
-    ```
-    """
-
-    raw_update: Update
-
-    def __init__(self, **kwargs: AnyValue) -> None:
-        cls_vars = vars(self.__class__)
-        defaults = {}
-        for k in self.__class__.__annotations__:
-            if k in cls_vars:
-                defaults[k] = cls_vars[k]
-                delattr(self.__class__, k)
-        dict.__init__(self, **defaults | kwargs)
-
-    def __setitem__(self, __key: Key, __value: AnyValue) -> None:
-        super().__setitem__(self.key_to_str(__key), __value)
-
-    def __getitem__(self, __key: Key) -> AnyValue:
-        return super().__getitem__(self.key_to_str(__key))
-
-    def __delitem__(self, __key: Key) -> None:
-        super().__delattr__(self.key_to_str(__key))
-
-    def __setattr__(self, __name: str, __value: AnyValue) -> None:
-        self.__setitem__(__name, __value)
-
-    def __getattr__(self, __name: str) -> AnyValue:
-        return self.__getitem__(__name)
-
-    def __delattr__(self, __name: str) -> None:
-        return self.__delitem__(__name)
-
-    @staticmethod
-    def key_to_str(key: Key) -> str:
-        return key if isinstance(key, str) else str(key.value)
-
-    def copy(self) -> typing.Self:
-        return self.__class__(**self)
-
-    def set(self, key: Key, value: AnyValue) -> None:
-        self[self.key_to_str(key)] = value
-
-    def get(self, key: Key) -> AnyValue:
-        return self[self.key_to_str(key)]
-
-    def delete(self, key: Key) -> None:
-        del self[self.key_to_str(key)]
-
-
-__all__ = ("Context",)
+__all__ = ("NodeCollection", "NodeSession", "compose_node")
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/handler/abc.py` & `mubble-1.1.0/mubble/bot/dispatch/handler/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,21 +7,17 @@
 from mubble.types import Update
 
 T = typing.TypeVar("T", bound=Model)
 
 
 class ABCHandler(ABC, typing.Generic[T]):
     is_blocking: bool
-    ctx: Context
 
     @abstractmethod
-    async def run(self, event: T) -> typing.Any:
+    async def check(self, api: ABCAPI, event: Update, ctx: Context | None = None) -> bool:
         pass
 
     @abstractmethod
-    async def check(
-        self, api: ABCAPI, event: Update, ctx: Context | None = None
-    ) -> bool:
+    async def run(self, event: T, ctx: Context) -> typing.Any:
         pass
 
-
 __all__ = ("ABCHandler",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/handler/func.py` & `mubble-1.1.0/mubble/bot/dispatch/handler/func.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import dataclasses
+
 import typing_extensions as typing
 
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types import BaseCute
 from mubble.bot.dispatch.context import Context
 from mubble.bot.dispatch.process import check_rule
 from mubble.modules import logger
@@ -9,58 +11,54 @@
 from mubble.types import Update
 
 from .abc import ABCHandler
 
 if typing.TYPE_CHECKING:
     from mubble.bot.rules import ABCRule
 
-F = typing.TypeVar(
-    "F", bound=typing.Callable[typing.Concatenate[typing.Any, ...], typing.Awaitable]
-)
+F = typing.TypeVar("F", bound=typing.Callable[typing.Concatenate[typing.Any, ...], typing.Awaitable[typing.Any]])
 EventT = typing.TypeVar("EventT", bound=BaseCute)
-ErrorHandlerT = typing.TypeVar(
-    "ErrorHandlerT", bound=ABCErrorHandler, default=ErrorHandler
-)
+ErrorHandlerT = typing.TypeVar("ErrorHandlerT", bound=ABCErrorHandler, default=ErrorHandler)
 
 
+@dataclasses.dataclass(repr=False)
 class FuncHandler(ABCHandler[EventT], typing.Generic[EventT, F, ErrorHandlerT]):
-    def __init__(
-        self,
-        func: F,
-        rules: list["ABCRule[EventT]"],
-        is_blocking: bool = True,
-        dataclass: type[typing.Any] | None = dict,
-        error_handler: ErrorHandlerT | None = None,
-    ):
-        self.func = func
-        self.is_blocking = is_blocking
-        self.rules = rules
-        self.dataclass = dataclass
-        self.error_handler: ErrorHandlerT = error_handler or ErrorHandler()  # type: ignore
-        self.ctx = Context()
-
-    @property
-    def on_error(self):
-        return self.error_handler.catch
-
-    async def check(
-        self, api: ABCAPI, event: Update, ctx: Context | None = None
-    ) -> bool:
+    func: F
+    rules: list["ABCRule[EventT]"]
+    _: dataclasses.KW_ONLY
+    is_blocking: bool = dataclasses.field(default=True)
+    dataclass: type[typing.Any] | None = dataclasses.field(default=dict)
+    error_handler: ErrorHandlerT = dataclasses.field(
+        default_factory=lambda: typing.cast(ErrorHandlerT, ErrorHandler()),
+    )
+    preset_context: Context = dataclasses.field(default_factory=lambda: Context())
+
+    def __repr__(self) -> str:
+        return "<{}: {}={!r} with rules={!r}, dataclass={!r}, error_handler={!r}>".format(
+            self.__class__.__name__,
+            "blocking function" if self.is_blocking else "function",
+            self.func.__name__,
+            self.rules,
+            self.dataclass,
+            self.error_handler,
+        )
+    
+    async def check(self, api: ABCAPI, event: Update, ctx: Context | None = None) -> bool:
         ctx = ctx or Context()
-        preset_ctx = self.ctx.copy()
-        self.ctx |= ctx
+        temp_ctx = ctx.copy()
+        temp_ctx |= self.preset_context
+
         for rule in self.rules:
-            if not await check_rule(api, rule, event, self.ctx):
+            if not await check_rule(api, rule, event, temp_ctx):
                 logger.debug("Rule {!r} failed!", rule)
-                self.ctx = preset_ctx
                 return False
+        
+        ctx |= temp_ctx
         return True
 
-    async def run(self, event: EventT) -> typing.Any:
+    async def run(self, event: EventT, ctx: Context) -> typing.Any:
         if self.dataclass is not None:
             event = self.dataclass(**event.to_dict())
-        return (
-            await self.error_handler.run(self.func, event, event.api, self.ctx)
-        ).unwrap()
+        return (await self.error_handler.run(self.func, event, event.api, ctx)).unwrap()
 
 
 __all__ = ("FuncHandler",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/handler/message_reply.py` & `mubble-1.1.0/mubble/bot/dispatch/handler/message_reply.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,47 +2,57 @@
 
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types import MessageCute
 from mubble.bot.dispatch.context import Context
 from mubble.bot.dispatch.process import check_rule
 from mubble.bot.rules.abc import ABCRule
 from mubble.modules import logger
-from mubble.option.option import Nothing
-from mubble.types.objects import Update
+from mubble.msgspec_utils import Nothing
+from mubble.types.objects import ReplyParameters, Update
 
 from .abc import ABCHandler
 
 
 class MessageReplyHandler(ABCHandler[MessageCute]):
     def __init__(
         self,
         text: str,
         *rules: ABCRule[MessageCute],
-        as_reply: bool = False,
         is_blocking: bool = True,
-    ):
+        as_reply: bool = False,
+    ) -> None:
         self.text = text
         self.rules = list(rules)
         self.as_reply = as_reply
         self.is_blocking = is_blocking
-        self.dataclass = MessageCute
-        self.ctx = Context()
+        self.preset_context = Context()
+    
+    def __repr__(self) -> str:
+        return "<{}: with rules={!r}, {}: {!r}>".format(
+            ("blocking " if self.is_blocking else "")
+            + self.__class__.__name__,
+            self.rules,
+            "answer text as reply" if self.as_reply else "answer text",
+            self.text,
+        )
 
-    async def check(
-        self, api: ABCAPI, event: Update, ctx: Context | None = None
-    ) -> bool:
+    async def check(self, api: ABCAPI, event: Update, ctx: Context | None = None) -> bool:
         ctx = ctx or Context()
-        self.ctx |= ctx
+        temp_ctx = ctx.copy()
+        temp_ctx |= self.preset_context
+
         for rule in self.rules:
-            if not await check_rule(api, rule, event, self.ctx):
+            if not await check_rule(api, rule, event, ctx):
                 logger.debug("Rule {!r} failed!", rule)
                 return False
+
+        ctx |= temp_ctx
         return True
 
-    async def run(self, event: MessageCute) -> typing.Any:
+    async def run(self, event: MessageCute, _: Context) -> typing.Any:
         await event.answer(
             text=self.text,
-            reply_to_message_id=(event.message_id if self.as_reply else Nothing),
+            reply_parameters=ReplyParameters(event.message_id) if self.as_reply else None,
         )
 
 
 __all__ = ("MessageReplyHandler",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/process.py` & `mubble-1.1.0/mubble/bot/dispatch/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import typing
 
+from fntypes.result import Error
+
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types import BaseCute
 from mubble.bot.dispatch.context import Context
 from mubble.modules import logger
-from mubble.result import Error
 from mubble.tools.i18n.base import I18nEnum
 from mubble.types import Update
 
 from .middleware.abc import ABCMiddleware
 from .return_manager.abc import ABCReturnManager
 
 if typing.TYPE_CHECKING:
     from mubble.bot.dispatch.handler.abc import ABCHandler
     from mubble.bot.rules.abc import ABCRule
 
 T = typing.TypeVar("T", bound=BaseCute)
-_ = typing.Any
+_: typing.TypeAlias = typing.Any
 
 
 async def process_inner(
     event: T,
     raw_event: Update,
     middlewares: list[ABCMiddleware[T]],
     handlers: list["ABCHandler[T]"],
@@ -31,23 +32,25 @@
 
     for middleware in middlewares:
         if await middleware.pre(event, ctx) is False:
             return False
 
     found = False
     responses = []
+    ctx_copy = ctx.copy()
+
     for handler in handlers:
         if await handler.check(event.api, raw_event, ctx):
             found = True
-            handler.ctx |= ctx
-            response = await handler.run(event)
+            response = await handler.run(event, ctx)
             responses.append(response)
             await return_manager.run(response, event, ctx)
             if handler.is_blocking:
                 break
+            ctx = ctx_copy
 
     for middleware in middlewares:
         await middleware.post(event, responses, ctx)
 
     return found
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/return_manager/abc.py` & `mubble-1.1.0/mubble/bot/dispatch/return_manager/abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return tuple(typing.get_origin(x) or x for x in typing.get_args(t))
     return None
 
 
 def register_manager(return_type: type | types.UnionType):
     def wrapper(func: typing.Callable[..., typing.Awaitable]):
         return Manager(get_union_types(return_type) or (return_type,), func)  # type: ignore
-
+    
     return wrapper
 
 
 @dataclasses.dataclass(frozen=True)
 class Manager:
     types: tuple[type, ...]
     callback: typing.Callable[..., typing.Awaitable]
@@ -39,65 +39,60 @@
 class ABCReturnManager(ABC, typing.Generic[EventT]):
     @abstractmethod
     async def run(self, response: typing.Any, event: EventT, ctx: Context) -> None:
         pass
 
 
 class BaseReturnManager(ABCReturnManager[EventT]):
+    def __repr__(self) -> str:
+        return "<{}: {}>".format(
+            self.__class__.__name__,
+            ", ".join(x.callback.__name__ + "=" + repr(x) for x in self.managers),
+        )
+
     @property
     def managers(self) -> list[Manager]:
         return [
             manager
             for manager in (vars(BaseReturnManager) | vars(self.__class__)).values()
             if isinstance(manager, Manager)
         ]
 
     @register_manager(Context)
     @staticmethod
     async def ctx_manager(value: Context, event: EventT, ctx: Context) -> None:
         """Basic manager for returning context from handler."""
-
+        
         ctx.update(value)
-
+    
     async def run(self, response: typing.Any, event: EventT, ctx: Context) -> None:
         for manager in self.managers:
-            if typing.Any in manager.types or any(
-                type(response) is x for x in manager.types
-            ):
+            if typing.Any in manager.types or any(type(response) is x for x in manager.types):
                 await manager(response, event, ctx)
-
+    
     @typing.overload
-    def register_manager(
-        self, return_type: type[T]
-    ) -> typing.Callable[
+    def register_manager(self, return_type: type[T]) -> typing.Callable[
         [typing.Callable[[T, EventT, Context], typing.Awaitable]], Manager
     ]:
         ...
-
+    
     @typing.overload
-    def register_manager(
-        self, return_type: tuple[type[T], ...]
-    ) -> typing.Callable[
+    def register_manager(self, return_type: tuple[type[T], ...]) -> typing.Callable[
         [typing.Callable[[tuple[T, ...], EventT, Context], typing.Awaitable]], Manager
     ]:
         ...
 
-    def register_manager(
-        self, return_type: type[T] | tuple[type[T], ...]
-    ) -> typing.Callable[
-        [typing.Callable[[T | tuple[T, ...], EventT, Context], typing.Awaitable]],
-        Manager,
+    def register_manager(self, return_type: type[T] | tuple[type[T], ...]) -> typing.Callable[
+        [typing.Callable[[T | tuple[T, ...], EventT, Context], typing.Awaitable]], Manager
     ]:
-        def wrapper(
-            func: typing.Callable[[T, EventT, Context], typing.Awaitable]
-        ) -> Manager:
+        def wrapper(func: typing.Callable[[T, EventT, Context], typing.Awaitable]) -> Manager:
             manager = Manager(get_union_types(return_type) or (return_type,), func)  # type: ignore
             setattr(self.__class__, func.__name__, manager)
             return manager
-
+        
         return wrapper
 
 
 __all__ = (
     "ABCReturnManager",
     "BaseReturnManager",
     "Manager",
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/return_manager/callback_query.py` & `mubble-1.1.0/mubble/bot/dispatch/return_manager/callback_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import typing
+
 from mubble.bot.cute_types import CallbackQueryCute
 from mubble.bot.dispatch.context import Context
 
 from .abc import BaseReturnManager, register_manager
 
 
 class CallbackQueryReturnManager(BaseReturnManager[CallbackQueryCute]):
     @register_manager(str)
     @staticmethod
     async def str_manager(value: str, event: CallbackQueryCute, ctx: Context) -> None:
         await event.answer(value)
-
+    
     @register_manager(dict)
     @staticmethod
-    async def dict_manager(value: dict, event: CallbackQueryCute, ctx: Context) -> None:
+    async def dict_manager(value: dict[str, typing.Any], event: CallbackQueryCute, ctx: Context) -> None:
         await event.answer(**value)
 
 
 __all__ = ("CallbackQueryReturnManager",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/return_manager/message.py` & `mubble-1.1.0/mubble/bot/dispatch/return_manager/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import typing
+
 from mubble.bot.cute_types import MessageCute
 from mubble.bot.dispatch.context import Context
+from mubble.tools.formatting import HTMLFormatter
 
 from .abc import BaseReturnManager, register_manager
 
 
-class MessageReturnManager(BaseReturnManager[MessageCute]):
+class MessageReturnManager(BaseReturnManager[MessageCute]):  
     @register_manager(str)
     @staticmethod
     async def str_manager(value: str, event: MessageCute, ctx: Context) -> None:
         await event.answer(value)
-
+    
     @register_manager(list | tuple)
     @staticmethod
-    async def seq_manager(
-        value: list[str] | tuple[str, ...], event: MessageCute, ctx: Context
-    ) -> None:
+    async def seq_manager(value: list[str] | tuple[str, ...], event: MessageCute, ctx: Context) -> None:
         for message in value:
             await event.answer(message)
-
+    
     @register_manager(dict)
     @staticmethod
-    async def dict_manager(value: dict, event: MessageCute, ctx: Context) -> None:
+    async def dict_manager(value: dict[str, typing.Any], event: MessageCute, ctx: Context) -> None:
         await event.answer(**value)
 
+    @register_manager(HTMLFormatter)
+    @staticmethod
+    async def htmlformatter_manager(value: HTMLFormatter, event: MessageCute, ctx: Context) -> None:
+        await event.answer(value, parse_mode=HTMLFormatter.PARSE_MODE)
+
 
 __all__ = ("MessageReturnManager",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/view/abc.py` & `mubble-1.1.0/mubble/bot/dispatch/view/abc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 import typing
 from abc import ABC, abstractmethod
 
+from fntypes.co import Nothing, Some
+
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types.base import BaseCute
 from mubble.bot.dispatch.handler.abc import ABCHandler
-from mubble.bot.dispatch.handler.func import ErrorHandlerT, FuncHandler
+from mubble.bot.dispatch.handler.func import FuncHandler
 from mubble.bot.dispatch.middleware.abc import ABCMiddleware
 from mubble.bot.dispatch.process import process_inner
 from mubble.bot.dispatch.return_manager.abc import ABCReturnManager
 from mubble.bot.rules.abc import ABCRule
 from mubble.model import Model
-from mubble.option.option import Nothing, NothingType, Option, Some
+from mubble.msgspec_utils import Option
+from mubble.tools.error_handler.error_handler import ABCErrorHandler, ErrorHandler
 from mubble.types.objects import Update
 
 EventType = typing.TypeVar("EventType", bound=BaseCute)
+ErrorHandlerT = typing.TypeVar("ErrorHandlerT", bound=ABCErrorHandler)
+MiddlewareT = typing.TypeVar("MiddlewareT", bound=ABCMiddleware)
+
+FuncType: typing.TypeAlias = typing.Callable[
+    typing.Concatenate[EventType, ...],
+    typing.Coroutine[typing.Any, typing.Any, typing.Any],
+]
 
 
 class ABCView(ABC):
     @abstractmethod
     async def check(self, event: Update) -> bool:
         pass
 
@@ -53,84 +63,107 @@
         for base in cls.__dict__.get("__orig_bases__", ()):
             if issubclass(typing.get_origin(base) or base, ABCView):
                 for generic_type in typing.get_args(base):
                     if issubclass(
                         typing.get_origin(generic_type) or generic_type, BaseCute
                     ):
                         return Some(generic_type)
-        return Nothing
+        return Nothing()
 
     @classmethod
-    def get_event_raw(cls, update: Update) -> Option[Model]:
-        match cls.get_event_type():
-            case Some(event_type):
-                for field in update.__struct_fields__:
-                    event_raw = getattr(update, field)
-                    if isinstance(event_raw, Some | NothingType):
-                        event_raw = event_raw.unwrap_or_none()
-                    if event_raw is not None and issubclass(
-                        event_type, event_raw.__class__
-                    ):
-                        return Some(event_raw)
-        return Nothing
+    def get_raw_event(cls, update: Update) -> Option[Model]:
+        match update.update_type:
+            case Some(update_type):
+                return getattr(update, update_type.value)
+            case _:
+                return Nothing()
+    
+    @typing.overload
+    def __call__(
+        self,
+        *rules: ABCRule[EventType],
+    ) -> typing.Callable[[FuncType[EventType]], FuncHandler[EventType, FuncType[EventType], ErrorHandler]]:
+        ...
+    
+    @typing.overload
+    def __call__(
+        self,
+        *rules: ABCRule[EventType],
+        error_handler: ErrorHandlerT,
+        is_blocking: bool = True,
+    ) -> typing.Callable[[FuncType[EventType]], FuncHandler[EventType, FuncType[EventType], ErrorHandlerT]]:
+        ...
 
+    @typing.overload
     def __call__(
         self,
         *rules: ABCRule[EventType],
+        error_handler: typing.Literal[None] = None,
+        is_blocking: bool = True,
+    ) -> typing.Callable[[FuncType[EventType]], FuncHandler[EventType, FuncType[EventType], ErrorHandler]]:
+        ...
+
+    def __call__(  # type: ignore
+        self,
+        *rules: ABCRule[EventType],
+        error_handler: ABCErrorHandler | None = None,
         is_blocking: bool = True,
-        error_handler: ErrorHandlerT | None = None,
     ):
-        def wrapper(
-            func: typing.Callable[
-                typing.Concatenate[EventType, ...],
-                typing.Coroutine,
-            ]
-        ):
+        def wrapper(func: FuncType[EventType]):
             func_handler = FuncHandler(
                 func,
                 [*self.auto_rules, *rules],
-                is_blocking,
+                is_blocking=is_blocking,
                 dataclass=None,
-                error_handler=error_handler,
             )
             self.handlers.append(func_handler)
             return func_handler
 
         return wrapper
 
     def register_middleware(self, *args: typing.Any, **kwargs: typing.Any):
-        def wrapper(cls: type[ABCMiddleware[EventType]]):
+        def wrapper(cls: type[MiddlewareT]) -> type[MiddlewareT]:
             self.middlewares.append(cls(*args, **kwargs))
             return cls
 
         return wrapper
 
     async def check(self, event: Update) -> bool:
-        return bool(self.get_event_raw(event))
+        match self.get_raw_event(event):
+            case Some(e) if issubclass(
+                self.get_event_type().expect(
+                    "{!r} has no event type in generic.".format(self.__class__.__name__),
+                ),
+                e.__class__,
+            ):
+                return True
+            case _:
+                return False
 
     async def process(self, event: Update, api: ABCAPI) -> bool:
-        event_raw = self.get_event_raw(event).unwrap()
-        event_type = self.get_event_type().unwrap()
         return await process_inner(
-            event_type(**event_raw.to_dict(), api=api),
+            self.get_event_type()
+            .unwrap()
+            .from_update(
+                update=self.get_raw_event(event).unwrap(),
+                bound_api=api,
+            ),
             event,
             self.middlewares,
             self.handlers,
             self.return_manager,
         )
 
     def load(self, external: typing.Self) -> None:
         self.auto_rules.extend(external.auto_rules)
         self.handlers.extend(external.handlers)
         self.middlewares.extend(external.middlewares)
 
 
-class BaseStateView(
-    ABCStateView[EventType], BaseView[EventType], ABC, typing.Generic[EventType]
-):
+class BaseStateView(ABCStateView[EventType], BaseView[EventType], ABC, typing.Generic[EventType]):
     @abstractmethod
     def get_state_key(self, event: EventType) -> int | None:
         pass
 
 
 __all__ = (
     "ABCView",
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/view/box.py` & `mubble-1.1.0/mubble/bot/dispatch/view/box.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,26 @@
     "InlineQueryViewT", bound=ABCView, default=InlineQueryView
 )
 MessageViewT = typing.TypeVar("MessageViewT", bound=ABCView, default=MessageView)
 
 
 @dataclasses.dataclass(kw_only=True)
 class ViewBox(typing.Generic[CallbackQueryViewT, InlineQueryViewT, MessageViewT]):
-    callback_query: CallbackQueryViewT = dataclasses.field(  # type: ignore
-        default_factory=lambda: CallbackQueryView(),
+    callback_query: CallbackQueryViewT = dataclasses.field(
+        default_factory=lambda: typing.cast(CallbackQueryViewT, CallbackQueryView()),
     )
-    inline_query: InlineQueryViewT = dataclasses.field(  # type: ignore
-        default_factory=lambda: InlineQueryView(),
+    inline_query: InlineQueryViewT = dataclasses.field(
+        default_factory=lambda: typing.cast(InlineQueryViewT, InlineQueryView()),
     )
-    message: MessageViewT = dataclasses.field(  # type: ignore
-        default_factory=lambda: MessageView(),
+    message: MessageViewT = dataclasses.field(
+        default_factory=lambda: typing.cast(MessageViewT, MessageView()),
     )
 
     def get_views(self) -> dict[str, ABCView]:
         return {
-            name: view for name, view in self.__dict__.items()
+            name: view
+            for name, view in self.__dict__.items()
             if isinstance(view, ABCView)
         }
 
 
 __all__ = ("ViewBox",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/view/callback_query.py` & `mubble-1.1.0/mubble/bot/dispatch/view/callback_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
+from fntypes.option import Some
+
 from mubble.bot.cute_types import CallbackQueryCute
 from mubble.bot.dispatch.return_manager import CallbackQueryReturnManager
-from mubble.option.option import Some
 
 from .abc import BaseStateView
 
 
 class CallbackQueryView(BaseStateView[CallbackQueryCute]):
-    def __init__(self):
+    def __init__(self) -> None:
         self.auto_rules = []
         self.handlers = []
         self.middlewares = []
         self.return_manager = CallbackQueryReturnManager()
 
     def get_state_key(self, event: CallbackQueryCute) -> int | None:
-        match event.message:
-            case Some(message):
-                return message.message_id
-            case _:
-                return None
+        return event.message.map(lambda variative: variative.v.message_id).unwrap_or_none()
 
 
 __all__ = ("CallbackQueryView",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/waiter_machine/machine.py` & `mubble-1.1.0/mubble/bot/dispatch/waiter_machine/machine.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,20 +15,26 @@
 if typing.TYPE_CHECKING:
     from mubble.bot.dispatch.view.abc import ABCStateView, BaseStateView
 
 
 class WaiterMachine:
     def __init__(self) -> None:
         self.storage: Storage = {}
+    
+    def __repr__(self) -> str:
+        return "<{}: storage={!r}>".format(
+            self.__class__.__name__,
+            self.storage,
+        )
 
     async def drop(
         self,
         state_view: "ABCStateView[EventModel]",
         id: Identificator,
-        **context,
+        **context: typing.Any,
     ) -> None:
         view_name = state_view.__class__.__name__
         if view_name not in self.storage:
             raise LookupError("No record of view {!r} found".format(view_name))
 
         short_state = self.storage[view_name].pop(id, None)
         if not short_state:
@@ -37,15 +43,15 @@
                     id,
                     view_name,
                 )
             )
 
         waiters = typing.cast(
             typing.Iterable[asyncio.Future[typing.Any]],
-            short_state.event._waiters,  # type: ignore
+            short_state.event._waiters  # type: ignore
         )
         for future in waiters:
             future.cancel()
 
         await self.call_behaviour(
             state_view,
             short_state.on_drop_behaviour,
@@ -56,34 +62,34 @@
     async def wait(
         self,
         state_view: "BaseStateView[EventModel]",
         linked: EventModel | tuple[ABCAPI, Identificator],
         *rules: ABCRule[EventModel],
         default: Behaviour = None,
         on_drop: Behaviour = None,
-        expiration: datetime.timedelta | int | None = None,
+        expiration: datetime.timedelta | int | float | None = None,
     ) -> tuple[EventModel, Context]:
-        if isinstance(expiration, int):
+        if isinstance(expiration, int | float):
             expiration = datetime.timedelta(seconds=expiration)
 
         api: ABCAPI
         key: Identificator
         event = asyncio.Event()
         if isinstance(linked, tuple):
             api, key = linked
         else:
             api, key = linked.ctx_api, state_view.get_state_key(linked)  # type: ignore
             if not key:
                 raise RuntimeError("Unable to get state key.")
 
         short_state = ShortState(
             key,
-            ctx_api=api,
-            event=event,
-            rules=rules,
+            api,
+            event,
+            rules,
             expiration=expiration,
             default_behaviour=default,
             on_drop_behaviour=on_drop,
         )
 
         view_name = state_view.__class__.__name__
         if view_name not in self.storage:
@@ -100,17 +106,17 @@
         return e, ctx
 
     async def call_behaviour(
         self,
         view: "ABCStateView[EventModel]",
         behaviour: Behaviour,
         event: asyncio.Event | EventModel,
-        **context,
+        **context: typing.Any,
     ) -> None:
         if behaviour is None:
             return
         # TODO: add behaviour check
         # TODO: support view as a behaviour
-        await behaviour.run(event)
+        await behaviour.run(event, context)  # type: ignore
 
 
 __all__ = ("WaiterMachine",)
```

### Comparing `mubble-1.0.0/mubble/bot/dispatch/waiter_machine/middleware.py` & `mubble-1.1.0/mubble/bot/dispatch/waiter_machine/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,47 +34,45 @@
         if view_name not in self.machine.storage:
             return True
 
         key = self.view.get_state_key(event)
         if key is None:
             raise RuntimeError("Unable to get state key.")
 
-        short_state: typing.Optional["ShortState"] = self.machine.storage[
-            view_name
-        ].get(key)
+        short_state: typing.Optional["ShortState[EventType]"] = self.machine.storage[view_name].get(key)
         if not short_state:
             return True
 
         if (
-            short_state.expiration is not None
-            and datetime.datetime.now() >= short_state.expiration
+            short_state.expiration_date is not None
+            and datetime.datetime.now() >= short_state.expiration_date
         ):
             await self.machine.drop(self.view, short_state.key)
             return True
-
+        
         handler = FuncHandler(
-            self.pass_runtime, list(short_state.rules), dataclass=None
+            self.pass_runtime,
+            list(short_state.rules),
+            dataclass=None,
         )
-        handler.ctx.set("short_state", short_state)
+        handler.preset_context.set("short_state", short_state)
         result = await handler.check(event.ctx_api, ctx.raw_update, ctx)
 
         if result is True:
-            await handler.run(event)
+            await handler.run(event, ctx)
 
         elif short_state.default_behaviour is not None:
             await self.machine.call_behaviour(
                 self.view,
                 short_state.default_behaviour,
                 event,
-                **handler.ctx,
+                **handler.preset_context,
             )
 
         return False
 
-    async def pass_runtime(
-        self, event: EventType, short_state: "ShortState[EventType]", ctx: Context
-    ) -> None:
+    async def pass_runtime(self, event: EventType, short_state: "ShortState[EventType]", ctx: Context) -> None:
         setattr(short_state.event, "context", (event, ctx))
         short_state.event.set()
 
 
 __all__ = ("WaiterMiddleware",)
```

### Comparing `mubble-1.0.0/mubble/bot/polling/polling.py` & `mubble-1.1.0/mubble/bot/polling/polling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 import typing
 
 import aiohttp
+import msgspec
+from fntypes.result import Error, Ok
 
 from mubble.api.abc import ABCAPI
 from mubble.api.error import InvalidTokenError
 from mubble.bot.polling.abc import ABCPolling
-from mubble.model import Raw, decoder
 from mubble.modules import logger
-from mubble.result import Error, Ok
+from mubble.msgspec_utils import decoder
 from mubble.types import Update, UpdateType
 
 
 class Polling(ABCPolling):
     def __init__(
         self,
         api: ABCAPI,
@@ -24,20 +25,32 @@
         exclude_updates: set[str | UpdateType] | None = None,
     ):
         self.api = api
         self.allowed_updates = self.get_allowed_updates(
             include_updates=include_updates,
             exclude_updates=exclude_updates,
         )
-        self.reconnection_timeout = (
-            5 if reconnection_timeout < 0 else reconnection_timeout
-        )
+        self.reconnection_timeout = 5 if reconnection_timeout < 0 else reconnection_timeout
         self.max_reconnetions = 10 if max_reconnetions < 0 else max_reconnetions
         self.offset = offset
         self._stop = False
+    
+    def __repr__(self) -> str:
+        return (
+            "<{}: with api={!r}, stopped={}, offset={}, allowed_updates={!r}, "
+            "max_reconnetions={}, reconnection_timeout={}>"
+        ).format(
+            self.__class__.__name__,
+            self.api,
+            self._stop,
+            self.offset,
+            self.allowed_updates,
+            self.max_reconnetions,
+            self.reconnection_timeout,
+        )
 
     def get_allowed_updates(
         self,
         *,
         include_updates: set[str | UpdateType] | None = None,
         exclude_updates: set[str | UpdateType] | None = None,
     ) -> list[str]:
@@ -54,15 +67,15 @@
         elif exclude_updates:
             allowed_updates = [x for x in allowed_updates if x not in exclude_updates]
         elif include_updates:
             allowed_updates = [x for x in allowed_updates if x in include_updates]
 
         return [x.value if isinstance(x, UpdateType) else x for x in allowed_updates]
 
-    async def get_updates(self) -> Raw | None:
+    async def get_updates(self) -> msgspec.Raw | None:
         raw_updates = await self.api.request_raw(
             "getUpdates",
             {"offset": self.offset, "allowed_updates": self.allowed_updates},
         )
         match raw_updates:
             case Ok(value):
                 return value
@@ -96,25 +109,21 @@
                         "Failed to reconnect to the server after {} attempts, polling stopping.",
                         self.max_reconnetions,
                     )
                     self.stop()
                     exit(9)
                 else:
                     logger.warning(
-                        "Server disconnected, waiting 5 seconds to reconnetion..."
+                        "Server disconnected, waiting 5 seconds to reconnetion...",
                     )
                     reconn_counter += 1
                     await asyncio.sleep(self.reconnection_timeout)
             except aiohttp.ClientConnectorError:
-                logger.error(
-                    "Client connection failed, polling stopping! "
-                    "Please, check your internet connection."
-                )
-                self.stop()
-                exit(3)
+                logger.error("Client connection failed, attempted to reconnect...")
+                await asyncio.sleep(self.reconnection_timeout)
             except BaseException as e:
                 logger.exception(e)
 
     def stop(self) -> None:
         self._stop = True
```

### Comparing `mubble-1.0.0/mubble/bot/rules/abc.py` & `mubble-1.1.0/mubble/bot/rules/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from mubble.bot.dispatch.process import check_rule
 from mubble.bot.rules.adapter import ABCAdapter, EventAdapter, RawUpdateAdapter
 from mubble.tools.i18n.base import ABCTranslator
 from mubble.tools.magic import cache_translation, get_cached_translation
 from mubble.types.objects import Update as UpdateObject
 
 T = typing.TypeVar("T", bound=BaseCute)
-Message = MessageCute
-Update = UpdateCute
+
+Message: typing.TypeAlias = MessageCute
+Update: typing.TypeAlias = UpdateCute
 
 
 def with_caching_translations(func):
     """Should be used as decorator for .translate method. Caches rule translations."""
 
-    async def wrapper(self: "ABCRule", translator: ABCTranslator):
+    async def wrapper(self: "ABCRule[typing.Any]", translator: ABCTranslator):
         if translation := get_cached_translation(self, translator.locale):
             return translation
         translation = await func(self, translator)
         cache_translation(self, translator.locale, translation)
         return translation
 
     return wrapper
@@ -55,15 +56,15 @@
 
     def __neg__(self) -> "ABCRule[T]":
         return NotRule(self)
 
     def __repr__(self) -> str:
         return "<rule: {!r}, adapter: {!r}>".format(
             self.__class__.__name__,
-            self.adapter.__class__.__name__,
+            self.adapter,
         )
 
     async def translate(self, translator: ABCTranslator) -> typing.Self:
         return self
 
 
 class AndRule(ABCRule[T]):
```

### Comparing `mubble-1.0.0/mubble/bot/rules/adapter/abc.py` & `mubble-1.1.0/mubble/bot/rules/adapter/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import abc
 import typing
 
+from fntypes.result import Result
+
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types import BaseCute
 from mubble.bot.rules.adapter.errors import AdapterError
 from mubble.model import Model
-from mubble.result import Result
 
 UpdateT = typing.TypeVar("UpdateT", bound=Model)
 CuteT = typing.TypeVar("CuteT", bound=BaseCute)
 
 
 class ABCAdapter(abc.ABC, typing.Generic[UpdateT, CuteT]):
     @abc.abstractmethod
```

### Comparing `mubble-1.0.0/mubble/bot/rules/adapter/event.py` & `mubble-1.1.0/mubble/bot/rules/adapter/event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 import typing
 
+from fntypes.result import Error, Ok, Result
+
 from mubble.api.abc import ABCAPI
 from mubble.bot.cute_types import BaseCute
 from mubble.bot.rules.adapter.abc import ABCAdapter
 from mubble.bot.rules.adapter.errors import AdapterError
-from mubble.option.option import Nothing
-from mubble.result import Error, Ok, Result
+from mubble.msgspec_utils import Nothing
 from mubble.types.objects import Model, Update
 
 EventT = typing.TypeVar("EventT", bound=Model)
 CuteT = typing.TypeVar("CuteT", bound=BaseCute)
 
 
 class EventAdapter(ABCAdapter[Update, CuteT]):
-    def __init__(self, event_name: str, model: type[CuteT]):
+    def __init__(self, event_name: str, model: type[CuteT]) -> None:
         self.event_name = event_name
         self.model = model
+    
+    def __repr__(self) -> str:
+        raw_update_type = Update.__annotations__.get(self.event_name, "Unknown")
+        raw_update_type = (
+            typing.get_args(raw_update_type)[0].__forward_arg__
+            if typing.get_args(raw_update_type)
+            else raw_update_type
+        )
+        return "<{}: adapt {} -> {}>".format(
+            self.__class__.__name__,
+            raw_update_type,
+            self.model.__name__,
+        )
 
     async def adapt(self, api: ABCAPI, update: Update) -> Result[CuteT, AdapterError]:
         update_dct = update.to_dict()
         if self.event_name not in update_dct:
             return Error(
-                AdapterError(f"Update is not of event type {self.event_name!r}.")
+                AdapterError(f"Update is not of event type {self.event_name!r}."),
             )
         if update_dct[self.event_name] is Nothing:
-            return Error(AdapterError(f"Update is not an {self.event_name!r}."))
+            return Error(
+                AdapterError(f"Update is not an {self.event_name!r}."),
+            )
         return Ok(
-            self.model.from_update(update_dct[self.event_name].unwrap(), bound_api=api)
+            self.model.from_update(update_dct[self.event_name].unwrap(), bound_api=api),
         )
 
 
 __all__ = ("EventAdapter",)
```

### Comparing `mubble-1.0.0/mubble/bot/rules/callback_data.py` & `mubble-1.1.0/mubble/bot/rules/callback_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,38 +10,24 @@
 from mubble.bot.rules.adapter import EventAdapter
 from mubble.model import decoder
 from mubble.tools.buttons import DataclassInstance
 
 from .abc import ABCRule
 from .markup import Markup, PatternLike, check_string
 
-if typing.TYPE_CHECKING:
-    T = typing.TypeVar("T")
-    Ref: typing.TypeAlias = typing.Annotated[T, ...]
-else:
-
-    class Ref:
-        def __class_getitem__(cls, code: str) -> typing.ForwardRef:
-            return typing.ForwardRef(code)
+T = typing.TypeVar("T")
 
-
-CallbackQuery = CallbackQueryCute
-Validator: typing.TypeAlias = typing.Callable[
-    [typing.Any], bool | typing.Awaitable[bool]
-]
+Ref: typing.TypeAlias = typing.Annotated[T, ...]
+CallbackQuery: typing.TypeAlias = CallbackQueryCute
+Validator: typing.TypeAlias = typing.Callable[[typing.Any], bool | typing.Awaitable[bool]]
 MapDict: typing.TypeAlias = dict[
-    str,
-    typing.Any | type[typing.Any] | Validator | list[Ref["MapDict"]] | Ref["MapDict"],
-]
-CallbackMap: typing.TypeAlias = list[
-    tuple[str, typing.Any | type | Validator | Ref["CallbackMap"]]
-]
-CallbackMapStrict: typing.TypeAlias = list[
-    tuple[str, Validator | Ref["CallbackMapStrict"]]
+    str, typing.Any | type[typing.Any] | Validator | list[Ref["MapDict"]] | Ref["MapDict"]
 ]
+CallbackMap: typing.TypeAlias = list[tuple[str, typing.Any | type | Validator | Ref["CallbackMap"]]]
+CallbackMapStrict: typing.TypeAlias = list[tuple[str, Validator | Ref["CallbackMapStrict"]]]
 
 
 class CallbackQueryRule(ABCRule[CallbackQuery], abc.ABC):
     adapter = EventAdapter("callback_query", CallbackQuery)
 
     @abc.abstractmethod
     async def check(self, event: CallbackQuery, ctx: Context) -> bool:
@@ -62,75 +48,75 @@
         self.mapping = self.transform_to_callbacks(
             self.transform_to_map(mapping),
         )
 
     @classmethod
     def transform_to_map(cls, mapping: MapDict) -> CallbackMap:
         """Transforms MapDict to CallbackMap."""
-
+        
         callback_map = []
-
+        
         for k, v in mapping.items():
             if isinstance(v, dict):
                 v = cls.transform_to_map(v)
             callback_map.append((k, v))
-
+        
         return callback_map
 
     @classmethod
     def transform_to_callbacks(cls, callback_map: CallbackMap) -> CallbackMapStrict:
         """Transforms `CallbackMap` to `CallbackMapStrict`."""
-
+        
         callback_map_result = []
 
         for key, value in callback_map:
             if isinstance(value, type):
                 validator = (lambda tp: lambda v: isinstance(v, tp))(value)
             elif isinstance(value, list):
                 validator = cls.transform_to_callbacks(value)
             elif not callable(value):
                 validator = (lambda val: lambda v: val == v)(value)
             else:
                 validator = value
             callback_map_result.append((key, validator))
-
+        
         return callback_map_result
 
     @staticmethod
     async def run_validator(value: typing.Any, validator: Validator) -> bool:
         """Run async or sync validator."""
-
+        
         with suppress(BaseException):
             result = validator(value)
             if inspect.isawaitable(result):
                 result = await result
             return result  # type: ignore
-
+        
         return False
-
+        
     @classmethod
     async def match(cls, callback_data: dict, callback_map: CallbackMapStrict) -> bool:
         """Matches callback_data with callback_map recursively."""
 
         for key, validator in callback_map:
             if key not in callback_data:
                 return False
-
+            
             if isinstance(validator, list):
                 if not (
                     isinstance(callback_data[key], dict)
                     and await cls.match(callback_data[key], validator)
                 ):
                     return False
-
+            
             elif not await cls.run_validator(callback_data[key], validator):
                 return False
 
         return True
-
+    
     async def check(self, event: CallbackQuery, ctx: Context) -> bool:
         callback_data = event.decode_callback_data().unwrap_or_none()
         if callback_data is None:
             return False
         if await self.match(callback_data, self.mapping):
             ctx.update(callback_data)
             return True
@@ -152,15 +138,15 @@
     async def check(self, event: CallbackQuery, ctx: Context) -> bool:
         return event.decode_callback_data().unwrap_or_none() == self.d
 
 
 class CallbackDataJsonModel(CallbackQueryDataRule):
     def __init__(self, model: type[msgspec.Struct] | type[DataclassInstance]):
         self.model = model
-
+        
     async def check(self, event: CallbackQuery, ctx: Context) -> bool:
         with suppress(BaseException):
             ctx.data = decoder.decode(event.data.unwrap().encode(), type=self.model)
             return True
         return False
```

### Comparing `mubble-1.0.0/mubble/bot/rules/command.py` & `mubble-1.1.0/mubble/bot/rules/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,46 +40,43 @@
         self.names = [names] if isinstance(names, str) else names
         self.arguments = arguments
         self.prefixes = prefixes
         self.separator = separator
         self.lazy = lazy
 
     def remove_prefix(self, text: str) -> str | None:
-        for prefix in self.prefixes:
-            if text.startswith(prefix):
-                return text.removeprefix(prefix)
-        return None
+        return next(
+            (
+                text.removeprefix(prefix)
+                for prefix in self.prefixes
+                if text.startswith(prefix)
+            ),
+            None,
+        )
 
     def parse_argument(
         self,
         arguments: list[Argument],
         data_s: str,
         new_s: str,
         s: str,
     ) -> dict | None:
         argument = arguments[0]
         data = argument.check(data_s)
-        if data is None and not argument.optional:
-            return None
-
         if data is None:
-            return self.parse_arguments(arguments[1:], s)
-
+            return self.parse_arguments(arguments[1:], s) if argument.optional else None
         with_argument = self.parse_arguments(arguments[1:], new_s)
         if with_argument is not None:
             return {argument.name: data, **with_argument}
 
-        if not argument.optional:
-            return None
-
-        return self.parse_arguments(arguments[1:], s)
+        return self.parse_arguments(arguments[1:], s) if argument.optional else None
 
     def parse_arguments(self, arguments: list[Argument], s: str) -> dict | None:
         if not arguments:
-            return {} if not s else None
+            return None if s else {}
 
         if self.lazy:
             return self.parse_argument(arguments, *single_split(s, self.separator), s)
 
         all_split = s.split(self.separator)
         for i in range(1, len(all_split) + 1):
             ctx = self.parse_argument(
```

### Comparing `mubble-1.0.0/mubble/bot/rules/enum_text.py` & `mubble-1.1.0/mubble/bot/rules/enum_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
+import enum
 import typing
-from enum import StrEnum
 
 from mubble.bot.dispatch.context import Context
 
 from .abc import Message
 from .text import TextMessageRule
 
-T = typing.TypeVar("T", bound=StrEnum, covariant=True)
+T = typing.TypeVar("T", bound=enum.Enum, covariant=True)
 
 
 class EnumTextRule(TextMessageRule, typing.Generic[T]):
     def __init__(self, enum_t: type[T], *, lower_case: bool = True) -> None:
         self.enum_t = enum_t
-        self.texts = list(
-            map(lambda x: x.value.lower() if lower_case else x.value, self.enum_t)
-        )
+        self.texts = list(map(lambda x: x.value.lower() if lower_case else x.value, self.enum_t))
 
     def find(self, s: str) -> T:
         for enumeration in self.enum_t:
             if enumeration.value.lower() == s:
                 return enumeration
         raise KeyError("Enumeration is undefined.")
 
     async def check(self, message: Message, ctx: Context) -> bool:
         text = message.text.unwrap().lower()
         if text not in self.texts:
             return False
-        ctx["enum_text"] = self.find(text)
+        ctx.enum_text = self.find(text)
         return True
```

### Comparing `mubble-1.0.0/mubble/bot/rules/func.py` & `mubble-1.1.0/mubble/bot/rules/func.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/bot/rules/fuzzy.py` & `mubble-1.1.0/mubble/bot/rules/fuzzy.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/bot/rules/integer.py` & `mubble-1.1.0/mubble/bot/rules/integer.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/bot/rules/markup.py` & `mubble-1.1.0/mubble/bot/rules/markup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import typing
+
 import vbml
 
 from mubble.bot.dispatch.context import Context
 from mubble.tools.global_context import MubbleCtx
 
 from .abc import Message
 from .text import TextMessageRule
 
-PatternLike = str | vbml.Pattern
+PatternLike: typing.TypeAlias = str | vbml.Pattern
 global_ctx = MubbleCtx()
 
 
 def check_string(patterns: list[vbml.Pattern], s: str, ctx: Context) -> bool:
     for pattern in patterns:
         match global_ctx.vbml_patcher.check(pattern, s):
             case None | False:
@@ -18,15 +20,15 @@
             case {**response}:
                 ctx |= response
         return True
     return False
 
 
 class Markup(TextMessageRule):
-    def __init__(self, patterns: PatternLike | list[PatternLike]):
+    def __init__(self, patterns: PatternLike | list[PatternLike], /):
         if not isinstance(patterns, list):
             patterns = [patterns]
         self.patterns = [
             vbml.Pattern(pattern) if isinstance(pattern, str) else pattern
             for pattern in patterns
         ]
```

### Comparing `mubble-1.0.0/mubble/bot/rules/message_entities.py` & `mubble-1.1.0/mubble/bot/rules/message_entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import typing
+
 from mubble.bot.dispatch.context import Context
 from mubble.types.enums import MessageEntityType
 from mubble.types.objects import MessageEntity
 
 from .abc import Message, MessageRule
 
-Entity = str | MessageEntityType
+Entity: typing.TypeAlias = str | MessageEntityType
 
 
 class HasEntities(MessageRule):
     async def check(self, message: Message, ctx: Context) -> bool:
         return bool(message.entities)
```

### Comparing `mubble-1.0.0/mubble/bot/rules/regex.py` & `mubble-1.1.0/mubble/bot/rules/regex.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 
 from mubble.bot.dispatch.context import Context
 
 from .abc import Message
 from .text import TextMessageRule
 
-PatternLike = str | typing.Pattern[str]
+PatternLike: typing.TypeAlias = str | typing.Pattern[str]
 
 
 class Regex(TextMessageRule):
     def __init__(self, regexp: PatternLike | list[PatternLike]):
         self.regexp: list[re.Pattern[str]] = []
         match regexp:
             case re.Pattern() as pattern:
@@ -26,13 +26,13 @@
     async def check(self, message: Message, ctx: Context) -> bool:
         for regexp in self.regexp:
             response = re.match(regexp, message.text.unwrap())
             if response is not None:
                 if matches := response.groupdict():
                     ctx |= matches
                 else:
-                    ctx |= {"matches": response.groups() or response.group()}
+                    ctx |= {"matches": response.groups() or (response.group(),)}
                 return True
         return False
 
 
 __all__ = ("Regex",)
```

### Comparing `mubble-1.0.0/mubble/bot/rules/rule_enum.py` & `mubble-1.1.0/mubble/bot/rules/rule_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from mubble.bot.dispatch.context import Context
 
 from .abc import ABCRule, T, Update, check_rule
 from .func import FuncRule
 
 
-@dataclasses.dataclass(unsafe_hash=True)
+@dataclasses.dataclass
 class RuleEnumState:
     name: str
     rule: ABCRule
     cls: type["RuleEnum"]
 
     def __eq__(self, other: typing.Self) -> bool:
         return self.cls == other.cls and self.name == other.name
@@ -39,23 +39,23 @@
                 self & FuncRule(lambda _, ctx: self.must_be_state(ctx, attribute)),
             )
             enum_lst.append(attribute)
 
         setattr(cls, "__enum__", enum_lst)
 
     @classmethod
-    def save_state(cls, ctx: dict, enum: RuleEnumState) -> None:
+    def save_state(cls, ctx: Context, enum: RuleEnumState) -> None:
         ctx.update({cls.__class__.__name__ + "_state": enum})
 
     @classmethod
-    def check_state(cls, ctx: dict) -> RuleEnumState | None:
+    def check_state(cls, ctx: Context) -> RuleEnumState | None:
         return ctx.get(cls.__class__.__name__ + "_state")
 
     @classmethod
-    def must_be_state(cls, ctx: dict, state: RuleEnumState) -> bool:
+    def must_be_state(cls, ctx: Context, state: RuleEnumState) -> bool:
         real_state = cls.check_state(ctx)
         if not real_state:
             return False
         return real_state == state
 
     async def check(self, event: Update, ctx: Context) -> bool:
         if self.check_state(ctx):
```

### Comparing `mubble-1.0.0/mubble/bot/rules/start.py` & `mubble-1.1.0/mubble/bot/rules/start.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 from .abc import MessageRule
 from .is_from import IsPrivate
 from .markup import Markup, Message
 from .message_entities import MessageEntities
 
 
 class StartCommand(
-    MessageRule,
-    requires=[
-        IsPrivate()
-        & MessageEntities(MessageEntityType.BOT_COMMAND)
+    MessageRule, requires=[
+        IsPrivate() & MessageEntities(MessageEntityType.BOT_COMMAND)
         & Markup(["/start <param>", "/start"]),
-    ],
+    ]
 ):
     def __init__(
         self,
         validator: typing.Callable[[str], typing.Any | None] | None = None,
         *,
         param_required: bool = False,
         alias: str | None = None,
```

### Comparing `mubble-1.0.0/mubble/bot/rules/text.py` & `mubble-1.1.0/mubble/bot/rules/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 
 class TextMessageRule(MessageRule, ABC, requires=[HasText()]):
     pass
 
 
 class Text(TextMessageRule):
-    def __init__(self, texts: str | list[str], ignore_case: bool = False):
+    def __init__(self, texts: str | list[str], *, ignore_case: bool = False) -> None:
         if not isinstance(texts, list):
             texts = [texts]
-        self.texts = texts if not ignore_case else list(map(str.lower, texts))
+        self.texts = list(map(str.lower, texts)) if ignore_case else texts
         self.ignore_case = ignore_case
 
     async def check(self, message: Message, ctx: Context) -> bool:
         text = message.text.unwrap()
-        return (text if not self.ignore_case else text.lower()) in self.texts
+        return (text.lower() if self.ignore_case else text) in self.texts
 
     @with_caching_translations
     async def translate(self, translator: ABCTranslator) -> "Text":
         return Text(
             texts=[translator.get(text) for text in self.texts],
             ignore_case=self.ignore_case,
         )
```

### Comparing `mubble-1.0.0/mubble/bot/scenario/checkbox.py` & `mubble-1.1.0/mubble/bot/scenario/checkbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import dataclasses
-import random
-import string
+import secrets
 import typing
 
 from mubble.bot.cute_types import CallbackQueryCute
 from mubble.bot.dispatch.waiter_machine import WaiterMachine
 from mubble.tools import InlineButton, InlineKeyboard
 from mubble.tools.parse_mode import ParseMode
 from mubble.types.objects import InlineKeyboardMarkup
@@ -21,67 +20,80 @@
     name: str
     is_picked: bool
     default_text: str
     picked_text: str
     code: str
 
 
-def random_code(length: int) -> str:
-    return "".join(random.choices(string.ascii_letters + string.digits, k=length))
-
-
 class Checkbox(ABCScenario[CallbackQueryCute]):
-    INVALID_CODE: typing.ClassVar[str] = "Invalid code"
-    CALLBACK_ANSWER: typing.ClassVar[str] = "Done"
-    PARSE_MODE: typing.ClassVar[str] = ParseMode.MARKDOWNV2
+    INVALID_CODE = "Invalid code"
+    CALLBACK_ANSWER = "Done"
+    PARSE_MODE = ParseMode.HTML
 
     def __init__(
         self,
         waiter_machine: WaiterMachine,
         chat_id: int,
         msg: str,
+        *,
         ready_text: str = "Ready",
         max_in_row: int = 3,
-    ):
+    ) -> None:
         self.chat_id = chat_id
         self.msg = msg
         self.choices: list[Choice] = []
         self.ready = ready_text
         self.max_in_row = max_in_row
-        self.random_code = random_code(16)
+        self.random_code = secrets.token_hex(8)
         self.waiter_machine = waiter_machine
+    
+    def __repr__(self) -> str:
+        return (
+            "<{}@{!r}: (choices={!r}, max_in_row={}) with waiter_machine={!r}, ready_text={!r} "
+            "for chat_id={} with message={!r}>"
+        ).format(
+            self.__class__.__name__,
+            self.random_code,
+            self.choices,
+            self.max_in_row,
+            self.waiter_machine,
+            self.ready,
+            self.chat_id,
+            self.msg,
+        )
 
     def get_markup(self) -> InlineKeyboardMarkup:
-        kb = InlineKeyboard(resize_keyboard=True)
+        kb = InlineKeyboard()
         choices = self.choices.copy()
         while choices:
             while len(kb.keyboard[-1]) < self.max_in_row and choices:
                 choice = choices.pop(0)
                 kb.add(
                     InlineButton(
                         text=choice.default_text
                         if not choice.is_picked
                         else choice.picked_text,
                         callback_data=self.random_code + "/" + choice.code,
                     )
                 )
             kb.row()
-
+        
         kb.add(InlineButton(self.ready, callback_data=self.random_code + "/ready"))
         return kb.get_markup()
 
     def add_option(
         self,
         name: str,
         default_text: str,
         picked_text: str,
+        *,
         is_picked: bool = False,
     ) -> typing.Self:
         self.choices.append(
-            Choice(name, is_picked, default_text, picked_text, random_code(16)),
+            Choice(name, is_picked, default_text, picked_text, secrets.token_hex(8)),
         )
         return self
 
     async def handle(self, cb: CallbackQueryCute) -> bool:
         code = cb.data.unwrap().replace(self.random_code + "/", "", 1)
         if code == "ready":
             return False
@@ -103,29 +115,28 @@
         self,
         api: "API",
         view: "BaseStateView[CallbackQueryCute]",
     ) -> tuple[dict[str, bool], int]:
         assert len(self.choices) > 1
         message = (
             await api.send_message(
-                self.chat_id,
+                chat_id=self.chat_id,
                 text=self.msg,
                 parse_mode=self.PARSE_MODE,
                 reply_markup=self.get_markup(),
             )
         ).unwrap()
-
+        
         while True:
-            q: CallbackQueryCute
             q, _ = await self.waiter_machine.wait(view, (api, message.message_id))
             should_continue = await self.handle(q)
             await q.answer(self.CALLBACK_ANSWER)
             if not should_continue:
                 break
-
+        
         return (
             {choice.name: choice.is_picked for choice in self.choices},
             message.message_id,
         )
 
 
-__all__ = ("Checkbox", "Choice", "random_code")
+__all__ = ("Checkbox", "Choice")
```

### Comparing `mubble-1.0.0/mubble/bot/scenario/choice.py` & `mubble-1.1.0/mubble/bot/scenario/choice.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,28 @@
         for choice in self.choices:
             choice.is_picked = False
 
         for i, choice in enumerate(self.choices):
             if choice.code == code:
                 self.choices[i].is_picked = True
                 await cb.ctx_api.edit_message_text(
-                    chat_id=cb.message.unwrap().chat.id,
-                    message_id=cb.message.unwrap().message_id,
+                    chat_id=cb.message.unwrap().v.chat.id,
+                    message_id=cb.message.unwrap().v.message_id,
                     text=self.msg,
                     parse_mode=self.PARSE_MODE,
                     reply_markup=self.get_markup(),
                 )
 
         return True
 
     async def wait(
         self,
         api: "API",
-        cb_view: "BaseStateView[CallbackQueryCute]",
+        view: "BaseStateView[CallbackQueryCute]",
     ) -> tuple[str, int]:
         if len([choice for choice in self.choices if choice.is_picked]) != 1:
             raise ValueError("Exactly one choice must be picked")
-        choices, m_id = await super().wait(api, cb_view)
+        choices, m_id = await super().wait(api, view)
         return list(choices.keys())[list(choices.values()).index(True)], m_id
 
 
 __all__ = ("SingleChoice",)
```

### Comparing `mubble-1.0.0/mubble/client/aiohttp.py` & `mubble-1.1.0/mubble/client/aiohttp.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,27 +14,35 @@
 
 class AiohttpClient(ABCClient):
     def __init__(
         self,
         session: ClientSession | None = None,
         json_processing_module: JSONModule | None = None,
         timeout: aiohttp.ClientTimeout | None = None,
-        **session_params,
-    ):
+        **session_params: typing.Any,
+    ) -> None:
         self.session = session
         self.json_processing_module = json_processing_module or json
         self.session_params = session_params
         self.timeout = timeout or aiohttp.ClientTimeout(total=0)
-
+    
+    def __repr__(self) -> str:
+        return "<{}: session={!r}, timeout={}, closed={}>".format(
+            self.__class__.__name__,
+            self.session,
+            self.timeout,
+            True if self.session is None else self.session.closed,
+        )
+    
     async def request_raw(
         self,
         url: str,
         method: str = "GET",
-        data: dict | None = None,
-        **kwargs,
+        data: dict[str, typing.Any] | None = None,
+        **kwargs: typing.Any,
     ) -> "ClientResponse":
         if not self.session:
             self.session = ClientSession(
                 connector=TCPConnector(
                     ssl=ssl.create_default_context(cafile=certifi.where())
                 ),
                 json_serialize=self.json_processing_module.dumps,
@@ -50,73 +58,77 @@
             await response.read()
             return response
 
     async def request_json(
         self,
         url: str,
         method: str = "GET",
-        data: dict | None = None,
-        **kwargs,
-    ) -> dict:
+        data: dict[str, typing.Any] | None = None,
+        **kwargs: typing.Any,
+    ) -> dict[str, typing.Any]:
         response = await self.request_raw(url, method, data, **kwargs)
         return await response.json(
             encoding="utf-8",
             loads=self.json_processing_module.loads,
             content_type=None,
         )
 
     async def request_text(
         self,
         url: str,
         method: str = "GET",
-        data: dict | aiohttp.FormData | None = None,
-        **kwargs,
+        data: dict[str, typing.Any] | aiohttp.FormData | None = None,
+        **kwargs: typing.Any,
     ) -> str:
         response = await self.request_raw(url, method, data, **kwargs)  # type: ignore
         return await response.text(encoding="utf-8")
 
     async def request_bytes(
         self,
         url: str,
         method: str = "GET",
-        data: dict | aiohttp.FormData | None = None,
-        **kwargs,
+        data: dict[str, typing.Any] | aiohttp.FormData | None = None,
+        **kwargs: typing.Any,
     ) -> bytes:
         response = await self.request_raw(url, method, data, **kwargs)  # type: ignore
         if response._body is None:
             await response.read()
         return response._body
 
     async def request_content(
         self,
         url: str,
         method: str = "GET",
-        data: dict | None = None,
-        **kwargs,
+        data: dict[str, typing.Any] | None = None,
+        **kwargs: typing.Any,
     ) -> bytes:
         response = await self.request_raw(url, method, data, **kwargs)
         return response._body
 
     async def close(self) -> None:
         if self.session and not self.session.closed:
             await self.session.close()
 
     @classmethod
-    def get_form(cls, data: dict) -> aiohttp.formdata.FormData:
+    def get_form(
+        cls,
+        data: dict[str, typing.Any],
+        files: dict[str, tuple[str, bytes]] | None = None,
+    ) -> aiohttp.formdata.FormData:
+        files = files or {}
         form = aiohttp.formdata.FormData(quote_fields=False)
         for k, v in data.items():
-            params = {}
-            if isinstance(v, tuple):
-                params["filename"], v = v[0], v[1]
-            else:
-                v = str(v)
-            form.add_field(k, v, **params)
+            form.add_field(k, str(v))
+        
+        for n, f in files.items():
+            form.add_field(n, f[1], filename=f[0])
+        
         return form
 
-    def __del__(self):
+    def __del__(self) -> None:
         if self.session and not self.session.closed:
             if self.session._connector is not None and self.session._connector_owner:
                 self.session._connector.close()
             self.session._connector = None
 
 
 __all__ = ("AiohttpClient",)
```

### Comparing `mubble-1.0.0/mubble/model.py` & `mubble-1.1.0/mubble/msgspec_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,274 +1,280 @@
 import typing
 
+import fntypes.option
 import msgspec
-from msgspec import Raw, ValidationError
+from fntypes.co import Error, Ok, Result, Variative
 
-from mubble.option import Nothing, NothingType, Option, Some
-from mubble.option.msgspec_option import Option as MsgspecOption
-from mubble.result import Error, Ok, Result
+if typing.TYPE_CHECKING:
+    from datetime import datetime
 
-T = typing.TypeVar("T")
+    from fntypes.option import Option
+else:
+    from datetime import datetime as dt
 
-DecHook = typing.Callable[[type[T], typing.Any], typing.Any]
-EncHook = typing.Callable[[T], typing.Any]
+    Value = typing.TypeVar("Value")
 
-if typing.TYPE_CHECKING:
-    from mubble.api.error import APIError
+    datetime = type("datetime", (dt,), {})
 
-    Union = typing.Union
-else:
-    Ts = typing.TypeVarTuple("Ts")
 
-    @typing.runtime_checkable
-    class _Union(typing.Protocol[*Ts]):
-        def __repr__(self) -> str:
-            ...
-
-    Union = _Union
-
-MODEL_CONFIG: typing.Final[dict[str, typing.Any]] = {
-    "omit_defaults": True,
-    "dict": True,
-    "rename": {"from_": "from"},
-}
+    class OptionMeta(type):
+        def __instancecheck__(self, __instance: typing.Any) -> bool:
+            return isinstance(__instance, fntypes.option.Some | fntypes.option.Nothing)
+
+
+    class Option(typing.Generic[Value], metaclass=OptionMeta):
+        pass
+
+T = typing.TypeVar("T")
+Ts = typing.TypeVarTuple("Ts")
+
+DecHook: typing.TypeAlias = typing.Callable[[type[T], typing.Any], object]
+EncHook: typing.TypeAlias = typing.Callable[[T], typing.Any]
+
+Nothing: typing.Final[fntypes.option.Nothing] = fntypes.option.Nothing()
 
 
 def get_origin(t: type[T]) -> type[T]:
     return typing.cast(T, typing.get_origin(t)) or t
 
 
 def repr_type(t: type) -> str:
     return getattr(t, "__name__", repr(get_origin(t)))
 
 
-def msgspec_convert(obj: typing.Any, t: type[T]) -> Result[T, ValidationError]:
+def msgspec_convert(obj: typing.Any, t: type[T]) -> Result[T, msgspec.ValidationError]:
     try:
         return Ok(decoder.convert(obj, type=t, strict=True))
-    except ValidationError as exc:
+    except msgspec.ValidationError as exc:
         return Error(exc)
 
 
-def option_enc_hook(obj: Option[typing.Any]) -> typing.Any | None:
-    return obj.value if isinstance(obj, Some) else None
-
-
-def option_dec_hook(tp: type, obj: typing.Any) -> typing.Any:
+def option_dec_hook(tp: type[Option[typing.Any]], obj: typing.Any) -> Option[typing.Any]:
     if obj is None:
         return Nothing
-    value_type = (typing.get_args(tp) or (typing.Any,))[0]
-    return msgspec_convert({"value": obj}, Some[value_type]).unwrap()
+    value_type, = typing.get_args(tp) or (typing.Any,)
+    return msgspec_convert({"value": obj}, fntypes.option.Some[value_type]).unwrap()
 
 
-def union_dec_hook(tp: type, obj: typing.Any) -> typing.Any:
+def variative_dec_hook(tp: type[Variative], obj: typing.Any) -> Variative:
     union_types = typing.get_args(tp)
-
+    
     if isinstance(obj, dict):
-        counter_fields = {
+        struct_fields_match_sums: dict[type[msgspec.Struct], int] = {
             m: sum(1 for k in obj if k in m.__struct_fields__)
             for m in union_types
-            if issubclass(m, Model)
+            if issubclass(get_origin(m), msgspec.Struct)
         }
-        union_types = tuple(t for t in union_types if t not in counter_fields)
+        union_types = tuple(t for t in union_types if t not in struct_fields_match_sums)
         reverse = False
 
-        if len(set(counter_fields.values())) != len(counter_fields.values()):
-            counter_fields = {m: len(m.__struct_fields__) for m in counter_fields}
+        if len(set(struct_fields_match_sums.values())) != len(struct_fields_match_sums.values()):
+            struct_fields_match_sums = {m: len(m.__struct_fields__) for m in struct_fields_match_sums}
             reverse = True
 
         union_types = (
-            *sorted(counter_fields, key=lambda k: counter_fields[k], reverse=reverse),
+            *sorted(struct_fields_match_sums, key=lambda k: struct_fields_match_sums[k], reverse=reverse),
             *union_types,
         )
-
+    
     for t in union_types:
         match msgspec_convert(obj, t):
             case Ok(value):
-                return value
+                return tp(value)
 
     raise TypeError(
         "Object of type `{}` does not belong to types `{}`".format(
-            repr_type(type(obj)),
+            repr_type(obj.__class__),
             " | ".join(map(repr_type, union_types)),
         )
     )
 
 
-@typing.overload
-def full_result(
-    result: Result[msgspec.Raw, "APIError"], full_t: type[T]
-) -> Result[T, "APIError"]:
-    ...
-
-
-@typing.overload
-def full_result(
-    result: Result[msgspec.Raw, "APIError"],
-    full_t: tuple[type[T], ...],
-) -> Result[T, "APIError"]:
-    ...
-
-
-def full_result(
-    result: Result[msgspec.Raw, "APIError"],
-    full_t: type[T] | tuple[type[T], ...],
-) -> Result[T, "APIError"]:
-    return result.map(lambda v: decoder.decode(v, type=full_t))  # type: ignore
-
-
-def convert(d: typing.Any, serialize: bool = True) -> typing.Any:
-    if isinstance(d, Model):
-        converted_dct = convert(d.to_dict(), serialize=False)
-        return encoder.encode(converted_dct) if serialize is True else converted_dct
-
-    if isinstance(d, dict):
-        return {
-            k: convert(v, serialize=serialize)
-            for k, v in d.items()
-            if v not in (None, Nothing)
-        }
-
-    if isinstance(d, list):
-        converted_lst = [convert(x, serialize=False) for x in d]
-        return encoder.encode(converted_lst) if serialize is True else converted_lst
-
-    return d
-
-
-def get_params(params: dict[str, typing.Any]) -> dict[str, typing.Any]:
-    return {
-        k: v.unwrap() if v and isinstance(v, Some) else v
-        for k, v in (
-            *params.items(),
-            *params.pop("other", {}).items(),
-        )
-        if k != "self" and v not in (None, Nothing)
-    }
-
-
-class Model(msgspec.Struct, **MODEL_CONFIG):
-    def to_dict(
-        self,
-        *,
-        exclude_fields: set[str] | None = None,
-    ):
-        exclude_fields = exclude_fields or set()
-        if "model_to_dict" not in self.__dict__:
-            self.__dict__["model_to_dict"] = msgspec.structs.asdict(self)
-        return {
-            key: value
-            for key, value in self.__dict__["model_to_dict"].items()
-            if key not in exclude_fields
-        }
-
-
 class Decoder:
+    """Class `Decoder` for `msgspec` module with decode hook
+    for objects with the specified type.
+    
+    ```
+    import enum
+
+    from datetime import datetime as dt
+
+    class Digit(enum.IntEnum):
+        ONE = 1
+        TWO = 2
+        THREE = 3
+
+    decoder = Encoder()
+    decoder.dec_hooks[dt] = lambda t, timestamp: t.fromtimestamp(timestamp)
+
+    decoder.dec_hook(dt, 1713354732)  #> datetime.datetime(2024, 4, 17, 14, 52, 12)
+    decoder.dec_hook(int, "123")  #> TypeError: Unknown type `int`. You can implement decode hook for this type.
+
+    decoder.convert("123", type=int, strict=False)  #> 123
+    decoder.convert(1, type=Digit)  #> <Digit.ONE: 1>
+
+    decoder.decode(b'{"digit":3}', type=dict[str, Digit])  #> {'digit': <Digit.THREE: 3>}
+    ```
+    """
+
     def __init__(self) -> None:
-        self.dec_hooks: dict[type, DecHook[typing.Any]] = {
-            MsgspecOption: option_dec_hook,
-            Union: union_dec_hook,  # type: ignore
+        self.dec_hooks: dict[typing.Any, DecHook[typing.Any]] = {
+            Option: option_dec_hook,
+            Variative: variative_dec_hook,
+            datetime: lambda t, obj: t.fromtimestamp(obj),
         }
+    
+    def __repr__(self) -> str:
+        return "<{}: dec_hooks={!r}>".format(
+            self.__class__.__name__,
+            self.dec_hooks,
+        )
 
-    def add_dec_hook(self, tp: type[T]):  # type: ignore
+    def add_dec_hook(self, t: T):  # type: ignore
         def decorator(func: DecHook[T]) -> DecHook[T]:
-            return self.dec_hooks.setdefault(get_origin(tp), func)
-
+            return self.dec_hooks.setdefault(get_origin(t), func)  # type: ignore
+        
         return decorator
-
-    def dec_hook(self, tp: type, obj: object) -> object:
-        origin_type = get_origin(tp)
+    
+    def dec_hook(self, tp: type[typing.Any], obj: object) -> object:
+        origin_type = t if isinstance((t := get_origin(tp)), type) else type(t)
         if origin_type not in self.dec_hooks:
             raise TypeError(
                 f"Unknown type `{repr_type(origin_type)}`. "
                 "You can implement decode hook for this type."
             )
         return self.dec_hooks[origin_type](tp, obj)
-
+    
     def convert(
         self,
         obj: object,
         *,
-        type: type["T"] = dict,
+        type: type[T] = dict,
         strict: bool = True,
         from_attributes: bool = False,
-        builtin_types: typing.Iterable[type] | None = None,
+        builtin_types: typing.Iterable[type[typing.Any]] | None = None,
         str_keys: bool = False,
-    ) -> "T":
+    ) -> T:
         return msgspec.convert(
             obj,
             type,
             strict=strict,
             from_attributes=from_attributes,
             dec_hook=self.dec_hook,
             builtin_types=builtin_types,
             str_keys=str_keys,
         )
+    
+    @typing.overload
+    def decode(self, buf: str | bytes) -> typing.Any:
+        ...
+    
+    @typing.overload
+    def decode(self, buf: str | bytes, *, strict: bool = True) -> typing.Any:
+        ...
 
+    @typing.overload
     def decode(
         self,
         buf: str | bytes,
         *,
-        type: type[T] = dict,
+        type: type[T],
+        strict: bool = True,
+    ) -> T:
+        ...
+
+    def decode(
+        self,
+        buf: str | bytes,
+        *,
+        type: type[T] = typing.Any,  # type: ignore
         strict: bool = True,
     ) -> T:
         return msgspec.json.decode(
             buf,
             type=type,
             strict=strict,
             dec_hook=self.dec_hook,
         )
 
 
 class Encoder:
+    """Class `Encoder` for `msgspec` module with encode hooks for objects.
+    
+    ```
+    from datetime import datetime as dt
+
+    encoder = Encoder()
+    encoder.enc_hooks[dt] = lambda d: int(d.timestamp())
+
+    encoder.enc_hook(dt.now())  #> 1713354732
+    encoder.enc_hook(123)  #> NotImplementedError: Not implemented encode hook for object of type `int`.
+
+    encoder.encode({'digit': Digit.ONE})  #> '{"digit":1}'
+    ```
+    """
+
     def __init__(self) -> None:
-        self.enc_hooks: dict[type, EncHook] = {
-            Some: option_enc_hook,
-            NothingType: option_enc_hook,
+        self.enc_hooks: dict[typing.Any, EncHook[typing.Any]] = {
+            fntypes.option.Some: lambda opt: opt.value,
+            fntypes.option.Nothing: lambda _: None,
+            Variative: lambda variative: variative.v,
+            datetime: lambda date: int(date.timestamp()),
         }
 
-    def add_dec_hook(self, tp: type[T]):  # type: ignore
-        def decorator(func: EncHook[T]) -> EncHook[T]:
-            return self.enc_hooks.setdefault(get_origin(tp), func)
+    def __repr__(self) -> str:
+        return "<{}: enc_hooks={!r}>".format(
+            self.__class__.__name__,
+            self.enc_hooks,
+        )
 
+    def add_dec_hook(self, t: type[T]):
+        def decorator(func: EncHook[T]) -> EncHook[T]:
+            encode_hook = self.enc_hooks.setdefault(get_origin(t), func)
+            return func if encode_hook is not func else encode_hook
+        
         return decorator
-
+    
     def enc_hook(self, obj: object) -> object:
-        origin_type = get_origin(type(obj))
+        origin_type = get_origin(obj.__class__)
         if origin_type not in self.enc_hooks:
             raise NotImplementedError(
                 "Not implemented encode hook for "
                 f"object of type `{repr_type(origin_type)}`."
             )
         return self.enc_hooks[origin_type](obj)
 
     @typing.overload
     def encode(self, obj: typing.Any) -> str:
         ...
+    
+    @typing.overload
+    def encode(self, obj: typing.Any, *, as_str: typing.Literal[True]) -> str:
+        ...
 
     @typing.overload
-    def encode(self, obj: typing.Any, *, as_str: bool = False) -> bytes:
+    def encode(self, obj: typing.Any, *, as_str: typing.Literal[False]) -> bytes:
         ...
 
     def encode(self, obj: typing.Any, *, as_str: bool = True) -> str | bytes:
         buf = msgspec.json.encode(obj, enc_hook=self.enc_hook)
         return buf.decode() if as_str else buf
 
 
 decoder: typing.Final[Decoder] = Decoder()
 encoder: typing.Final[Encoder] = Encoder()
 
 
 __all__ = (
     "Decoder",
     "Encoder",
-    "Model",
-    "Raw",
-    "convert",
-    "decoder",
-    "encoder",
-    "full_result",
+    "Option",
+    "Nothing",
     "get_origin",
-    "get_params",
-    "msgspec",
-    "msgspec_convert",
     "repr_type",
+    "msgspec_convert",
+    "option_dec_hook",
+    "variative_dec_hook",
+    "datetime",
+    "decoder",
+    "encoder",
 )
```

### Comparing `mubble-1.0.0/mubble/modules.py` & `mubble-1.1.0/mubble/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 import os
 import typing
 
 from choicelib import choice_in_order
 
 
+@typing.runtime_checkable
 class JSONModule(typing.Protocol):
-    def loads(self, s: str) -> dict | list:
-        ...
+    def loads(self, s: str | bytes) -> typing.Any: ...
 
-    def dumps(self, o: dict | list) -> str:
-        ...
+    def dumps(self, o: typing.Any) -> str: ...
 
 
+@typing.runtime_checkable
 class LoggerModule(typing.Protocol):
-    def debug(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def debug(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
-    def info(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def info(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
-    def warning(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def warning(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
-    def error(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def error(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
-    def critical(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def critical(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
-    def exception(self, __msg: object, *args: object, **kwargs: object):
-        ...
+    def exception(self, __msg: object, *args: object, **kwargs: object) -> None: ...
 
     def set_level(
         self,
         level: typing.Literal[
             "DEBUG",
             "INFO",
             "WARNING",
             "ERROR",
             "CRITICAL",
             "EXCEPTION",
         ],
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 logger: LoggerModule
 json: JSONModule = choice_in_order(
-    ["ujson", "hyperjson", "orjson"], do_import=True, default="mubble.msgspec_json"
+    ["orjson", "ujson", "hyperjson"], do_import=True, default="mubble.msgspec_json"
 )
 logging_module = choice_in_order(["loguru"], default="logging")
 logging_level = os.getenv("LOGGER_LEVEL", default="DEBUG").upper()
 
 if logging_module == "loguru":
     import os
     import sys
@@ -178,33 +171,44 @@
             return logging.Formatter(
                 LEVEL_FORMATS.get(record.levelname),
                 datefmt="%Y-%m-%d %H:%M:%S",
                 style="{",
             ).format(record)
 
     class LogMessage:
-        def __init__(self, fmt, args, kwargs):
+        def __init__(
+            self, fmt: typing.Any, args: typing.Any, kwargs: typing.Any
+        ) -> None:
             self.fmt = fmt
             self.args = args
             self.kwargs = kwargs
 
         def __str__(self) -> str:
             return self.fmt.format(*self.args, **self.kwargs)
 
     class MubbleLoggingStyleAdapter(logging.LoggerAdapter):
-        def __init__(self, logger, extra=None):
+        def __init__(
+            self,
+            logger: LoggerModule,
+            extra: dict[str, typing.Any] | None = None,
+        ) -> None:
             super().__init__(logger, extra or {})
 
-        def log(self, level, msg, *args, **kwargs):
+        def log(self, level: int, msg: object, *args: object, **kwargs: object) -> None:
             if self.isEnabledFor(level):
                 kwargs.setdefault("stacklevel", 2)
                 msg, args, kwargs = self.proc(msg, args, kwargs)
                 self.logger._log(level, msg, args, **kwargs)
 
-        def proc(self, msg, args, kwargs):
+        def proc(
+            self,
+            msg: object,
+            args: tuple[object, ...],
+            kwargs: dict[str, object],
+        ) -> tuple[LogMessage | object, tuple[object, ...], dict[str, object]]:
             log_kwargs = {
                 key: kwargs[key]
                 for key in inspect.getfullargspec(self.logger._log).args[1:]
                 if key in kwargs
             }
 
             if isinstance(msg, str):
```

### Comparing `mubble-1.0.0/mubble/node/__init__.py` & `mubble-1.1.0/mubble/node/__init__.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/node/attachment.py` & `mubble-1.1.0/mubble/node/attachment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 import dataclasses
 import typing
 
+from fntypes.option import Nothing
+
 import mubble.types
-from mubble.option import Nothing, Option
+from mubble.msgspec_utils import Option
 
 from .base import ComposeError, DataNode, ScalarNode
 from .message import MessageNode
 
 
 @dataclasses.dataclass
 class Attachment(DataNode):
     attachment_type: typing.Literal["audio", "document", "photo", "poll", "video"]
     _: dataclasses.KW_ONLY
-    audio: Option[mubble.types.Audio] = dataclasses.field(
-        default_factory=lambda: Nothing
-    )
-    document: Option[mubble.types.Document] = dataclasses.field(
-        default_factory=lambda: Nothing
-    )
-    photo: Option[list[mubble.types.PhotoSize]] = dataclasses.field(
-        default_factory=lambda: Nothing
-    )
-    poll: Option[mubble.types.Poll] = dataclasses.field(default_factory=lambda: Nothing)
-    video: Option[mubble.types.Video] = dataclasses.field(
-        default_factory=lambda: Nothing
-    )
+    audio: Option[mubble.types.Audio] = dataclasses.field(default_factory=lambda: Nothing())
+    document: Option[mubble.types.Document] = dataclasses.field(default_factory=lambda: Nothing())
+    photo: Option[list[mubble.types.PhotoSize]] = dataclasses.field(default_factory=lambda: Nothing())
+    poll: Option[mubble.types.Poll] = dataclasses.field(default_factory=lambda: Nothing())
+    video: Option[mubble.types.Video] = dataclasses.field(default_factory=lambda: Nothing())
 
     @classmethod
     async def compose(cls, message: MessageNode) -> "Attachment":
         for attachment_type in ("audio", "document", "photo", "poll", "video"):
-            if attachment := getattr(message, attachment_type, Nothing):
+            if (attachment := getattr(message, attachment_type, None)) is not None:
                 return cls(attachment_type, **{attachment_type: attachment})
         return cls.compose_error("No attachment found in message")
 
 
 @dataclasses.dataclass
 class Photo(DataNode):
     sizes: list[mubble.types.PhotoSize]
```

### Comparing `mubble-1.0.0/mubble/node/base.py` & `mubble-1.1.0/mubble/node/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import typing
 
 ComposeResult: typing.TypeAlias = typing.Coroutine[typing.Any, typing.Any, typing.Any] | typing.AsyncGenerator[typing.Any, None]
 
 
 class ComposeError(BaseException):
-    pass
+    ...
 
 
 class Node(abc.ABC):
     node: str = "node"
 
     @classmethod
     @abc.abstractmethod
```

### Comparing `mubble-1.0.0/mubble/node/container.py` & `mubble-1.1.0/mubble/node/container.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/node/rule.py` & `mubble-1.1.0/mubble/node/rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,37 +22,35 @@
             return cls.dataclass(**ctx)  # type: ignore
         except Exception as exc:
             raise ComposeError(f"Dataclass validation error: {exc}")
 
     @classmethod
     def as_node(cls) -> type[typing.Self]:
         return cls
-
+    
     @classmethod
     def get_sub_nodes(cls) -> dict:
         return {"update": UpdateNode}
 
     @classmethod
     def is_generator(cls) -> typing.Literal[False]:
         return False
 
     def __new__(cls, *rules: ABCRule) -> type[Node]:
         return type("_RuleNode", (cls,), {"dataclass": dict, "rules": rules})  # type: ignore
-
+    
     def __class_getitem__(cls, item: tuple[ABCRule, ...]) -> typing.Self:
         if not isinstance(item, tuple):
             item = (item,)
         return cls(*item)
-
+    
     @staticmethod
     def generate_dataclass(cls_: type["RuleContext"]):  # noqa: ANN205
-        return dataclasses.dataclass(
-            type(cls_.__name__, (object,), dict(cls_.__dict__))
-        )
-
+        return dataclasses.dataclass(type(cls_.__name__, (object,), dict(cls_.__dict__)))
+    
     def __init_subclass__(cls) -> None:
         if cls.__name__ == "_RuleNode":
             return
         cls.dataclass = cls.generate_dataclass(cls)
 
 
 __all__ = ("RuleContext",)
```

### Comparing `mubble-1.0.0/mubble/node/tools/generator.py` & `mubble-1.1.0/mubble/node/tools/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def error_on_none(value: T | None) -> T:
     if value is None:
         raise ComposeError
     return value
 
 
 def generate(
-    subnodes: tuple[type[Node], ...],
+    subnodes: tuple[type[Node], ...], 
     func: typing.Callable[..., typing.Any],
     casts: tuple[typing.Callable, ...] = (cast_false_to_none, error_on_none),
 ) -> type[ContainerNode]:
     async def compose(**kw: typing.Any) -> typing.Any:
         args = await ContainerNode.compose(**kw)
         result = func(*args)
         if inspect.isawaitable(result):
```

### Comparing `mubble-1.0.0/mubble/tools/__init__.py` & `mubble-1.1.0/mubble/tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from .error_handler import ABCErrorHandler, Catcher, ErrorHandler
+from .buttons import BaseButton
+from .error_handler import ABCErrorHandler, Catcher, CatcherError, ErrorHandler
 from .formatting import (
     BaseSpecFormat,
     ChannelBoostLink,
     FormatString,
     HTMLFormatter,
     InviteChatLink,
     Link,
     Mention,
     PreCode,
     ResolveDomain,
     SpecialFormat,
     StartBotLink,
     StartGroupLink,
     TgEmoji,
+    UserOpenMessage,
     block_quote,
     bold,
     channel_boost_link,
     code_inline,
     escape,
     get_channel_boost_link,
     get_invite_chat_link,
@@ -32,14 +34,16 @@
     resolve_domain,
     spoiler,
     start_bot_link,
     start_group_link,
     strike,
     tg_emoji,
     underline,
+    user_open_message,
+    user_open_message_link,
 )
 from .global_context import (
     ABCGlobalContext,
     CtxVar,
     GlobalContext,
     GlobalCtxVar,
     MubbleCtx,
@@ -57,31 +61,32 @@
 from .keyboard import (
     AnyMarkup,
     Button,
     InlineButton,
     InlineKeyboard,
     Keyboard,
     RowButtons,
-    keyboard_remove,
 )
-from .loop_wrapper import ABCLoopWrapper, DelayedTask, LoopWrapper
+from .loop_wrapper import ABCLoopWrapper, DelayedTask, Lifespan, LoopWrapper
 from .magic import magic_bundle, resolve_arg_names
 from .parse_mode import ParseMode
 
 __all__ = (
     "ABCErrorHandler",
     "ABCGlobalContext",
     "ABCI18n",
     "ABCLoopWrapper",
     "ABCTranslator",
     "ABCTranslatorMiddleware",
     "AnyMarkup",
+    "BaseButton",
     "BaseSpecFormat",
     "Button",
     "Catcher",
+    "CatcherError",
     "ChannelBoostLink",
     "CtxVar",
     "DelayedTask",
     "ErrorHandler",
     "FormatString",
     "GlobalContext",
     "GlobalCtxVar",
@@ -90,48 +95,51 @@
     "InlineButton",
     "InlineKeyboard",
     "InviteChatLink",
     "Keyboard",
     "KeyboardSetBase",
     "KeyboardSetYAML",
     "Link",
+    "Lifespan",
     "LoopWrapper",
     "Mention",
     "ParseMode",
     "PreCode",
     "ResolveDomain",
     "RowButtons",
     "SimpleI18n",
     "SimpleTranslator",
     "SpecialFormat",
     "StartBotLink",
     "StartGroupLink",
     "MubbleCtx",
     "TgEmoji",
+    "UserOpenMessage",
     "block_quote",
     "bold",
     "channel_boost_link",
     "code_inline",
     "ctx_var",
     "escape",
     "get_channel_boost_link",
     "get_invite_chat_link",
     "get_mention_link",
     "get_resolve_domain_link",
     "get_start_bot_link",
     "get_start_group_link",
     "invite_chat_link",
     "italic",
-    "keyboard_remove",
     "link",
     "magic_bundle",
     "mention",
     "pre_code",
     "resolve_arg_names",
     "resolve_domain",
     "spoiler",
     "start_bot_link",
     "start_group_link",
     "strike",
     "tg_emoji",
     "underline",
+    "user_open_message",
+    "user_open_message_link",
 )
```

### Comparing `mubble-1.0.0/mubble/tools/buttons.py` & `mubble-1.1.0/mubble/tools/buttons.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 import dataclasses
 import typing
 
 import msgspec
 
 from mubble.model import encoder
+from mubble.types import (
+    CallbackGame,
+    KeyboardButtonPollType,
+    KeyboardButtonRequestChat,
+    KeyboardButtonRequestUsers,
+    SwitchInlineQueryChosenChat,
+    WebAppInfo,
+)
+from mubble.types.objects import LoginUrl
 
 ButtonT = typing.TypeVar("ButtonT", bound="BaseButton")
 
 
+@typing.runtime_checkable
 class DataclassInstance(typing.Protocol):
     __dataclass_fields__: typing.ClassVar[dict[str, dataclasses.Field[typing.Any]]]
 
 
 @dataclasses.dataclass
 class BaseButton:
     def get_data(self) -> dict[str, typing.Any]:
@@ -36,35 +46,37 @@
 
 @dataclasses.dataclass
 class Button(BaseButton):
     text: str
     _: dataclasses.KW_ONLY
     request_contact: bool = False
     request_location: bool = False
-    request_poll: dict | None = None
-    web_app: dict | None = None
+    request_chat: dict[str, typing.Any] | KeyboardButtonRequestChat | None = None
+    request_user: dict[str, typing.Any] | KeyboardButtonRequestUsers | None = None
+    request_poll: dict[str, typing.Any] | KeyboardButtonPollType | None = None
+    web_app: dict[str, typing.Any] | WebAppInfo | None = None
 
 
 @dataclasses.dataclass
 class InlineButton(BaseButton):
     text: str
     _: dataclasses.KW_ONLY
     url: str | None = None
-    login_url: dict | None = None
+    login_url: dict[str, typing.Any] | LoginUrl | None = None
     pay: bool | None = None
-    callback_data: typing.Union[
-        str,
-        dict[str, typing.Any],
-        DataclassInstance,
-        msgspec.Struct,
-    ] | None = None
-    callback_game: dict | None = None
+    callback_data: (
+        str | dict[str, typing.Any] | DataclassInstance | msgspec.Struct | None
+    ) = None
+    callback_game: dict[str, typing.Any] | CallbackGame | None = None
     switch_inline_query: str | None = None
     switch_inline_query_current_chat: str | None = None
-    web_app: dict | None = None
+    switch_inline_query_chosen_chat: (
+        dict[str, typing.Any] | SwitchInlineQueryChosenChat | None
+    ) = None
+    web_app: dict[str, typing.Any] | WebAppInfo | None = None
 
 
 __all__ = (
     "BaseButton",
     "Button",
     "DataclassInstance",
     "InlineButton",
```

### Comparing `mubble-1.0.0/mubble/tools/error_handler/abc.py` & `mubble-1.1.0/mubble/tools/error_handler/abc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import typing
 from abc import ABC, abstractmethod
 
+from fntypes.result import Result
+
 from mubble.api import ABCAPI
 from mubble.bot.cute_types import BaseCute
 from mubble.bot.dispatch.context import Context
-from mubble.result import Result
 
 EventT = typing.TypeVar("EventT", bound=BaseCute)
 Handler = typing.Callable[typing.Concatenate[EventT, ...], typing.Awaitable[typing.Any]]
 
 
 class ABCErrorHandler(ABC, typing.Generic[EventT]):
     @abstractmethod
-    def catch(self) -> typing.Callable[[typing.Callable], typing.Callable]:
-        ...
+    def __call__(
+        self,
+        *args: typing.Any,
+        **kwargs: typing.Any,
+    ) -> typing.Callable[[typing.Callable[..., typing.Any]], typing.Callable[..., typing.Any]]:
+        """Decorator for registering callback as an error handler."""
 
     @abstractmethod
     async def run(
         self,
         handler: Handler[EventT],
         event: EventT,
         api: ABCAPI,
         ctx: Context,
     ) -> Result[typing.Any, typing.Any]:
-        ...
+        """Run error handler."""
 
 
 __all__ = ("ABCErrorHandler",)
```

### Comparing `mubble-1.0.0/mubble/tools/error_handler/error_handler.py` & `mubble-1.1.0/mubble/tools/error_handler/error_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,160 +1,175 @@
 import dataclasses
 import typing
 
+from fntypes.result import Error, Ok, Result
+
 from mubble.api import ABCAPI
 from mubble.bot.dispatch.context import Context
 from mubble.modules import logger
-from mubble.result import Error, Ok, Result
 from mubble.tools.magic import magic_bundle
 
 from .abc import ABCErrorHandler, EventT, Handler
+from .error import CatcherError
 
 F = typing.TypeVar("F", bound="FuncCatcher")
 ExceptionT = typing.TypeVar("ExceptionT", bound=BaseException, contravariant=True)
-FuncCatcher = typing.Callable[
-    typing.Concatenate[ExceptionT, ...], typing.Awaitable[typing.Any]
-]
+FuncCatcher = typing.Callable[typing.Concatenate[ExceptionT, ...], typing.Awaitable[typing.Any]]
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, repr=False)
 class Catcher(typing.Generic[EventT]):
-    func: FuncCatcher
+    func: FuncCatcher[BaseException]
     _: dataclasses.KW_ONLY
     exceptions: list[type[BaseException] | BaseException] = dataclasses.field(
-        default_factory=lambda: []
+        default_factory=lambda: [],
     )
     logging: bool = dataclasses.field(default=False)
     raise_exception: bool = dataclasses.field(default=False)
     ignore_errors: bool = dataclasses.field(default=False)
 
-    def match_exception(self, exception: BaseException) -> bool:
-        for exc in self.exceptions:
-            if isinstance(exc, type) and type(exception) == exc:
-                return True
-            if isinstance(exc, object) and type(exception) == type(exc):
-                return True if not exc.args else exc.args == exception.args
-        return False
+    def __repr__(self) -> str:
+        return "<Catcher: function={!r}, logging={}, raise_exception={}, ignore_errors={}>".format(
+            self.func.__name__,
+            self.logging,
+            self.raise_exception,
+            self.ignore_errors,
+        )
 
     async def __call__(
         self,
         handler: Handler[EventT],
         event: EventT,
         api: ABCAPI,
         ctx: Context,
-    ) -> Result[typing.Any, typing.Any]:
+    ) -> Result[typing.Any, BaseException]:
         try:
-            result = Ok(await handler(event, **magic_bundle(handler, ctx)))  # type: ignore
+            return Ok(await handler(event, **magic_bundle(handler, ctx)))  # type: ignore
         except BaseException as exc:
-            logger.debug(
-                "Exception {!r} occurred while running handler {!r}. Matching  "
-                "exceptions it with exception that can be caught by the catcher {!r}...",
-                exc.__class__.__name__,
-                handler.__name__,
-                self.func.__name__,
-            )
+            return await self.process_exception(api, event, ctx, exc, handler.__name__)
 
-            if self.match_exception(exc):
-                logger.debug(
-                    "Catcher {!r} caught an exception in handler {!r}, "
-                    "running catcher...".format(
-                        self.func.__name__,
-                        handler.__name__,
-                    )
+    async def process_exception(
+        self,
+        api: ABCAPI,
+        event: EventT,
+        ctx: Context,
+        exception: BaseException,
+        handler_name: str,
+    ) -> Result[typing.Any, BaseException]:
+        if self.match_exception(exception):
+            logger.debug(
+                "Catcher {!r} caught an exception in handler {!r}, "
+                "running catcher...".format(
+                    self.func.__name__,
+                    handler_name,
                 )
-                result = Ok(
-                    await self.func(
-                        exc,
-                        **magic_bundle(
-                            self.func,
-                            {"event": event, "api": api} | ctx,  # type: ignore
-                        ),
-                    )
+            )
+            return Ok(
+                await self.func(
+                    exception,
+                    **magic_bundle(self.func, {"event": event, "api": api} | ctx),  # type: ignore
                 )
-            else:
-                logger.debug("Failed to match exception {!r}!", exc.__class__.__name__)
-                result = Error(exc)
-
-        logger.debug(
-            "Catcher {!r} {} with result: {!r}",
-            self.func.__name__,
-            "completed" if result else "failed",
-            result,
-        )
-        return result
+            )
+        logger.debug("Failed to match exception {!r}!", exception.__class__.__name__)
+        return Error(exception)
+    
+    def match_exception(self, exception: BaseException) -> bool:
+        for exc in self.exceptions:
+            if isinstance(exc, type) and type(exception) is exc:
+                return True
+            if isinstance(exc, object) and type(exception) is type(exc):
+                return True if not exc.args else exc.args == exception.args
+        return False
 
 
 class ErrorHandler(ABCErrorHandler[EventT]):
-    def __init__(self, __catcher: Catcher[EventT] | None = None):
-        self.catcher = __catcher
-
+    def __init__(self, catcher: Catcher[EventT] | None = None, /) -> None:
+        self.catcher = catcher
+    
     def __repr__(self) -> str:
-        return f"<ErrorHandler: {self.catcher!r}>"
+        return (
+            "<ErrorHandler: exceptions_handled=[{}], catcher={!r}>".format(
+                ", ".join(
+                    e.__name__ if isinstance(e, type) else repr(e)
+                    for e in self.catcher.exceptions
+                ),
+                self.catcher,
+            )
+            if self.catcher is not None
+            else "<ErrorHandler: No catcher>"
+        )
 
-    def catch(
+    def __call__(
         self,
         *exceptions: type[BaseException] | BaseException,
         logging: bool = False,
         raise_exception: bool = False,
         ignore_errors: bool = False,
     ):
-        """Catch an exception while the handler is running.
+        """Register the catcher.
         :param logging: Error logging in stderr.
         :param raise_exception: Raise an exception if the catcher hasn't started.
-        :param ignore_errors: Ignore errors that may occur in the catcher.
+        :param ignore_errors: Ignore errors that may occur.
         """
 
         def decorator(func: F) -> F:
             if not self.catcher:
                 self.catcher = Catcher(
                     func,
                     exceptions=list(exceptions),
                     logging=logging,
                     raise_exception=raise_exception,
                     ignore_errors=ignore_errors,
                 )
             return func
-
         return decorator
+    
+    async def process(
+        self,
+        handler: Handler[EventT],
+        event: EventT,
+        api: ABCAPI,
+        ctx: Context,
+    ) -> Result[typing.Any, BaseException]:
+        assert self.catcher is not None
+
+        try:
+            return await self.catcher(handler, event, api, ctx)
+        except BaseException as exc:
+            return Error(CatcherError(
+                exc,
+                "Exception {!r} was occurred during the running catcher {!r}.".format(
+                    repr(exc), self.catcher.func.__name__
+                )
+            ))
+        
+    def process_catcher_error(self, error: CatcherError) -> Result[None, str]:
+        assert self.catcher is not None
+        
+        if self.catcher.raise_exception:
+            raise error.exc from None
+        if not self.catcher.ignore_errors:
+            return Error(error.error)
+        if self.catcher.logging:
+            logger.error(error.error)
+        
+        return Ok(None)
 
     async def run(
         self,
         handler: Handler[EventT],
         event: EventT,
         api: ABCAPI,
         ctx: Context,
     ) -> Result[typing.Any, typing.Any]:
         if not self.catcher:
             return Ok(await handler(event, **magic_bundle(handler, ctx)))  # type: ignore
-
-        ok_none = Ok(None)
-
-        try:
-            result = await self.catcher(handler, event, api, ctx)
-        except BaseException as e:
-            error_msg = (
-                "Exception {} was occurred during the running catcher {!r}.".format(
-                    repr(e.__class__.__name__)
-                    if not e.args
-                    else f"{e.__class__.__name__!r}: {str(e)!r}",
-                    self.catcher.func.__name__,
-                )
-            )
-            result = ok_none
-
-            if not self.catcher.ignore_errors:
-                return Error(error_msg)
-            if self.catcher.logging:
-                logger.error(error_msg)
-
-        if self.catcher.raise_exception and not result:
-            return result
-
-        if self.catcher.logging and not result:
-            logger.error(
-                "Catcher {!r} failed with error: {!r}",
-                self.catcher.func.__name__,
-                result.error,
-            )
-            return ok_none
-
-        return result or ok_none
+        
+        match await self.process(handler, event, api, ctx):
+            case Ok(_) as ok:
+                return ok
+            case Error(exc) as err:
+                if isinstance(exc, CatcherError):
+                    return self.process_catcher_error(exc)              
+                if self.catcher.ignore_errors:
+                    return Ok(None)
+                return err
```

### Comparing `mubble-1.0.0/mubble/tools/formatting/__init__.py` & `mubble-1.1.0/mubble/tools/formatting/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,35 +14,38 @@
     resolve_domain,
     spoiler,
     start_bot_link,
     start_group_link,
     strike,
     tg_emoji,
     underline,
+    user_open_message,
 )
 from .links import (
     get_channel_boost_link,
     get_invite_chat_link,
     get_mention_link,
     get_resolve_domain_link,
     get_start_bot_link,
     get_start_group_link,
+    user_open_message_link,
 )
 from .spec_html_formats import (
     BaseSpecFormat,
     ChannelBoostLink,
     InviteChatLink,
     Link,
     Mention,
     PreCode,
     ResolveDomain,
     SpecialFormat,
     StartBotLink,
     StartGroupLink,
     TgEmoji,
+    UserOpenMessage,
 )
 
 __all__ = (
     "BaseSpecFormat",
     "ChannelBoostLink",
     "FormatString",
     "HTMLFormatter",
@@ -51,14 +54,15 @@
     "Mention",
     "PreCode",
     "ResolveDomain",
     "SpecialFormat",
     "StartBotLink",
     "StartGroupLink",
     "TgEmoji",
+    "UserOpenMessage",
     "block_quote",
     "bold",
     "channel_boost_link",
     "code_inline",
     "escape",
     "get_channel_boost_link",
     "get_invite_chat_link",
@@ -74,8 +78,10 @@
     "resolve_domain",
     "spoiler",
     "start_bot_link",
     "start_group_link",
     "strike",
     "tg_emoji",
     "underline",
+    "user_open_message",
+    "user_open_message_link",
 )
```

### Comparing `mubble-1.0.0/mubble/tools/formatting/html.py` & `mubble-1.1.0/mubble/tools/formatting/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .links import (
     get_channel_boost_link,
     get_invite_chat_link,
     get_mention_link,
     get_resolve_domain_link,
     get_start_bot_link,
     get_start_group_link,
+    user_open_message_link,
 )
 from .spec_html_formats import SpecialFormat, is_spec_format
 
 TAG_FORMAT = "<{tag}{data}>{content}</{tag}>"
 QUOT_MARK = '"'
 
 
@@ -44,17 +45,15 @@
                 "Unknown format {!r} for object of type {!r}.".format(
                     fmt,
                     type(value).__name__,
                 )
             )
         return fmt
 
-    def get_spec_formatter(
-        self, value: SpecialFormat
-    ) -> typing.Callable[..., "TagFormat"]:
+    def get_spec_formatter(self, value: SpecialFormat) -> typing.Callable[..., "TagFormat"]:
         return globals()[value.__formatter_name__]
 
     def check_formats(self, value: typing.Any, fmts: list[str]) -> "TagFormat":
         if is_spec_format(value):
             value = value.string
 
         current_format = globals()[fmts.pop(0)](
@@ -197,19 +196,16 @@
     return TagFormat(string, tag="blockquote")
 
 
 def bold(string: str) -> TagFormat:
     return TagFormat(string, tag="b")
 
 
-def channel_boost_link(channel_username: str, string: str | None = None):
-    return link(
-        get_channel_boost_link(channel_username),
-        string or f"t.me/{channel_username}?boost",
-    )
+def channel_boost_link(channel_id: str | int, string: str | None = None):
+    return link(get_channel_boost_link(channel_id), string)
 
 
 def code_inline(string: str) -> TagFormat:
     return TagFormat(string, tag="code")
 
 
 def italic(string: str) -> TagFormat:
@@ -231,27 +227,20 @@
     return pre_code(TagFormat(string, tag="code", **{"class": f"language-{lang}"}))
 
 
 def spoiler(string: str) -> TagFormat:
     return TagFormat(string, tag="tg-spoiler")
 
 
-def start_bot_link(
-    bot_username: str, data: str, string: str | None = None
-) -> TagFormat:
-    return link(
-        get_start_bot_link(bot_username, data),
-        string or f"t.me/{bot_username}?start={data}",
-    )
+def start_bot_link(bot_id: str | int, data: str, string: str | None = None) -> TagFormat:
+    return link(get_start_bot_link(bot_id, data), string)
 
 
-def start_group_link(
-    bot_username: str, data: str, string: str | None = None
-) -> TagFormat:
-    return link(get_start_group_link(bot_username, data), string)
+def start_group_link(bot_id: str | int, data: str, string: str | None = None) -> TagFormat:
+    return link(get_start_group_link(bot_id, data), string)
 
 
 def strike(string: str) -> TagFormat:
     return TagFormat(string, tag="s")
 
 
 def mention(string: str, user_id: int) -> TagFormat:
@@ -276,14 +265,22 @@
     )
 
 
 def underline(string: str) -> TagFormat:
     return TagFormat(string, tag="u")
 
 
+def user_open_message(
+    user_id: int,
+    message: str | None = None,
+    string: str | None = None,
+) -> TagFormat:
+    return link(user_open_message_link(user_id, message), string)
+
+
 __all__ = (
     "FormatString",
     "HTMLFormatter",
     "SpecialFormat",
     "block_quote",
     "bold",
     "channel_boost_link",
@@ -303,8 +300,9 @@
     "resolve_domain",
     "spoiler",
     "start_bot_link",
     "start_group_link",
     "strike",
     "tg_emoji",
     "underline",
+    "user_open_message",
 )
```

### Comparing `mubble-1.0.0/mubble/tools/formatting/spec_html_formats.py` & `mubble-1.1.0/mubble/tools/formatting/spec_html_formats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,132 @@
 import dataclasses
 import typing
 
 from mubble.types.enums import ProgrammingLanguage
 
-SpecialFormat = typing.Union[
+SpecialFormat: typing.TypeAlias = typing.Union[
     "ChannelBoostLink",
-    "Mention",
+    "InviteChatLink",
     "Link",
+    "Mention",
     "PreCode",
-    "TgEmoji",
+    "ResolveDomain",
     "StartBotLink",
     "StartGroupLink",
-    "ResolveDomain",
-    "InviteChatLink",
+    "TgEmoji",
+    "UserOpenMessage",
 ]
 
 
 def is_spec_format(obj: typing.Any) -> typing.TypeGuard[SpecialFormat]:
     return (
         dataclasses.is_dataclass(obj)
         and hasattr(obj, "__formatter_name__")
         and isinstance(obj, BaseSpecFormat)
     )
 
 
 @dataclasses.dataclass(repr=False)
 class BaseSpecFormat:
-    __formatter_name__: typing.ClassVar[str]
+    __formatter_name__: typing.ClassVar[str] = dataclasses.field(init=False, repr=False)
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__!r}: {self.__formatter_name__!r}>"
+        return f"<Special formatter {self.__class__.__name__!r} -> {self.__formatter_name__!r}>"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class ChannelBoostLink(BaseSpecFormat):
     __formatter_name__ = "channel_boost_link"
 
-    channel_username: str
+    channel_id: str | int
     string: str | None = None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class InviteChatLink(BaseSpecFormat):
     __formatter_name__ = "invite_chat_link"
 
     invite_link: str
     string: str | None = None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class Mention(BaseSpecFormat):
     __formatter_name__ = "mention"
 
     string: str
     user_id: int
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class Link(BaseSpecFormat):
     __formatter_name__ = "link"
 
     href: str
     string: str | None = None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class PreCode(BaseSpecFormat):
     __formatter_name__ = "pre_code"
 
     string: str
     lang: str | ProgrammingLanguage | None = None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class TgEmoji(BaseSpecFormat):
     __formatter_name__ = "tg_emoji"
-
+    
     string: str
     emoji_id: int
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class StartBotLink(BaseSpecFormat):
     __formatter_name__ = "start_bot_link"
 
-    bot_username: str
+    bot_id: str | int
     data: str
     string: str | None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class StartGroupLink(BaseSpecFormat):
     __formatter_name__ = "start_group_link"
 
-    bot_username: str
+    bot_id: str | int
     data: str
     string: str | None = None
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(repr=False)
 class ResolveDomain(BaseSpecFormat):
     __formatter_name__ = "resolve_domain"
 
     username: str
     string: str | None = None
 
 
+@dataclasses.dataclass(repr=False)
+class UserOpenMessage(BaseSpecFormat):
+    __formatter_name__ = "user_open_message"
+
+    user_id: int
+    message: str | None = None
+    string: str | None = None
+
+
 __all__ = (
     "BaseSpecFormat",
     "ChannelBoostLink",
     "InviteChatLink",
     "Link",
     "Mention",
     "PreCode",
     "ResolveDomain",
     "SpecialFormat",
     "StartBotLink",
     "StartGroupLink",
     "TgEmoji",
+    "UserOpenMessage",
 )
```

### Comparing `mubble-1.0.0/mubble/tools/global_context/abc.py` & `mubble-1.1.0/mubble/tools/global_context/abc.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,17 @@
             self.name,
             repr(CtxVar(self.value, const=self.const)),
         )
 
     @classmethod
     def collect(cls, name: str, ctx_value: T | CtxVariable[T]) -> typing.Self:
         ctx_value = CtxVar(ctx_value) if not isinstance(ctx_value, CtxVar | GlobalCtxVar) else ctx_value
-        return cls(**dataclasses.asdict(ctx_value), name=name)  # type: ignore
+        params = ctx_value.__dict__
+        params["name"] = name
+        return cls(**params)
 
 
 class ABCGlobalContext(ABC, typing.Generic[T]):
     @abstractmethod
     def __getattr__(self, __name: str) -> typing.Any:
         pass
```

### Comparing `mubble-1.0.0/mubble/tools/global_context/global_context.py` & `mubble-1.1.0/mubble/tools/global_context/global_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import dataclasses
 from copy import deepcopy
 from functools import wraps
 
 import typing_extensions as typing
+from fntypes.co import Error, Nothing, Ok, Option, Result, Some
 
-from mubble.model import msgspec_convert
 from mubble.modules import logger
-from mubble.option import Nothing, Option, Some
-from mubble.result import Error, Ok, Result
+from mubble.msgspec_utils import msgspec_convert
 
 from .abc import ABCGlobalContext, CtxVar, CtxVariable, GlobalCtxVar
 
 T = typing.TypeVar("T")
 F = typing.TypeVar("F", bound=typing.Callable)
 CtxValueT = typing.TypeVar("CtxValueT", default=typing.Any)
 
 if typing.TYPE_CHECKING:
+
     _: typing.TypeAlias = None
 else:
+
     _ = lambda: None
 
 
 def type_check(value: object, value_type: type[T]) -> typing.TypeGuard[T]:
-    return True if value_type is object else bool(msgspec_convert(value, value_type))
+    if value_type in (typing.Any, object):
+        return True
+    match msgspec_convert(value, value_type):
+        case Ok(v):
+            return type(value) is type(v)
+        case Error(_):
+            return False
 
 
 def is_dunder(name: str) -> bool:
     return name.startswith("__") and name.endswith("__")
 
 
 def get_orig_class(obj: T) -> type[T]:
@@ -39,31 +46,31 @@
             "You cannot decorate a {!r} function with this decorator, only "
             "'__setattr__', __getattr__', '__delattr__' methods.".format(
                 func.__name__,
             )
         )
 
     @wraps(func)
-    def wrapper(self: "GlobalContext", __name: str, *args) -> typing.Any:
-        if self.is_root_attribute(__name) and __name in (
+    def wrapper(self: "GlobalContext", name: str, /, *args) -> typing.Any:
+        if self.is_root_attribute(name) and name in (
             self.__dict__ | self.__class__.__dict__
         ):
-            root_attr = self.get_root_attribute(__name).unwrap()
+            root_attr = self.get_root_attribute(name).unwrap()
             if all((not root_attr.can_be_rewritten, not root_attr.can_be_read)):
                 raise AttributeError(
-                    f"Unable to set, get, delete root attribute {__name!r}."
+                    f"Unable to set, get, delete root attribute {name!r}."
                 )
             if func.__name__ == "__setattr__" and not root_attr.can_be_rewritten:
-                raise AttributeError(f"Unable to set root attribute {__name!r}.")
+                raise AttributeError(f"Unable to set root attribute {name!r}.")
             if func.__name__ == "__getattr__" and not root_attr.can_be_read:
-                raise AttributeError(f"Unable to get root attribute {__name!r}.")
+                raise AttributeError(f"Unable to get root attribute {name!r}.")
             if func.__name__ == "__delattr__":
-                raise AttributeError(f"Unable to delete root attribute {__name!r}.")
+                raise AttributeError(f"Unable to delete root attribute {name!r}.")
 
-        return func(self, __name, *args)  # type: ignore
+        return func(self, name, *args)  # type: ignore
 
     return wrapper  # type: ignore
 
 
 def ctx_var(value: T, *, const: bool = False) -> T:
     """Example:
     ```
@@ -108,30 +115,28 @@
         return self._storage.copy()
 
     def set(self, name: str, ctx: "GlobalContext") -> None:
         self._storage.setdefault(name, ctx)
 
     def get(self, ctx_name: str) -> Option["GlobalContext"]:
         ctx = self._storage.get(ctx_name)
-        return Some(ctx) if ctx is not None else Nothing
+        return Some(ctx) if ctx is not None else Nothing()
 
     def delete(self, ctx_name: str) -> None:
         assert (
             self._storage.pop(ctx_name, None) is not None
         ), f"Context {ctx_name!r} is not defined in storage."
 
 
 @typing.dataclass_transform(
     kw_only_default=True,
     order_default=True,
     field_specifiers=(ctx_var,),
 )
-class GlobalContext(
-    ABCGlobalContext, typing.Generic[CtxValueT], dict[str, GlobalCtxVar[CtxValueT]]
-):
+class GlobalContext(ABCGlobalContext, typing.Generic[CtxValueT], dict[str, GlobalCtxVar[CtxValueT]]):
     """GlobalContext.
 
     ```
     ctx = GlobalContext()
     ctx["client"] = Client()
     ctx.address = CtxVar("128.0.0.7:8888", const=True)
 
@@ -190,24 +195,27 @@
         if not hasattr(self, "__ctx_name__"):
             self.__ctx_name__ = ctx_name
 
         if variables and not self:
             self.set_context_variables(variables)
 
     def __repr__(self) -> str:
-        return "<{!r} -> ({})>".format(
-            f"{self.__class__.__name__}@{self.ctx_name}",
+        return "<{} -> ({})>".format(
+            f"{self.__class__.__name__}@{self.ctx_name!r}",
             ", ".join(repr(var) for var in self),
         )
 
     def __eq__(self, __value: "GlobalContext") -> bool:
         """Returns True if the names of context stores
         that use self and __value instances are equivalent."""
 
-        return self.ctx_name == __value.ctx_name
+        return (
+            isinstance(__value, GlobalContext)
+            and self.__ctx_name__ == __value.__ctx_name__
+        )
 
     def __setitem__(self, __name: str, __value: CtxValueT | CtxVariable[CtxValueT]):
         if is_dunder(__name):
             raise NameError("Cannot set a context variable with dunder name.")
         var = self.get(__name)
         if var and var.unwrap().const:
             raise TypeError(
@@ -274,15 +282,15 @@
     def get_root_attribute(self, name: str) -> Option[RootAttr]:
         """Get root attribute by name."""
 
         if self.is_root_attribute(name):
             for rattr in self.__root_attributes__:
                 if rattr.name == name:
                     return Some(rattr)
-        return Nothing
+        return Nothing()
 
     def items(self) -> list[tuple[str, GlobalCtxVar[CtxValueT]]]:
         """Return context variables as set-like items."""
 
         return list(dict.items(self))
 
     def keys(self) -> list[str]:
@@ -299,93 +307,86 @@
         """Update context."""
 
         dict.update(dict(other.items()))
 
     def copy(self) -> typing.Self:
         """Copy context. Returns copied context without ctx_name."""
 
-        return self.__class__(**deepcopy(self.dict()))
+        return self.__class__(**self.dict())
 
     def dict(self) -> dict[str, GlobalCtxVar[CtxValueT]]:
         """Returns context as dict."""
 
-        return {name: var for name, var in self.items()}
+        return {name: deepcopy(var) for name, var in self.items()}
 
     @typing.overload
-    def pop(self, var_name: str) -> Option[GlobalCtxVar[CtxValueT]]:
-        ...
+    def pop(self, var_name: str) -> Option[GlobalCtxVar[CtxValueT]]: ...
 
     @typing.overload
     def pop(
         self,
         var_name: str,
         var_value_type: type[T],
-    ) -> Option[GlobalCtxVar[T]]:
-        ...
+    ) -> Option[GlobalCtxVar[T]]: ...
 
     def pop(
         self, var_name: str, var_value_type: type[T] = object
     ) -> Option[GlobalCtxVar[T]]:
-        """Pop context variable by name.
-        Returns Option[GlobalCtxVar[T]] object.
-        """
+        """Pop context variable by name."""
 
         val = self.get(var_name, var_value_type)
         if val:
             del self[var_name]
             return val
-        return Nothing
+        return Nothing()
 
     @typing.overload
-    def get(self, var_name: str) -> Option[GlobalCtxVar[CtxValueT]]:
-        ...
+    def get(self, var_name: str) -> Option[GlobalCtxVar[CtxValueT]]: ...
 
     @typing.overload
     def get(
         self,
         var_name: str,
         var_value_type: type[T],
-    ) -> Option[GlobalCtxVar[T]]:
-        ...
+    ) -> Option[GlobalCtxVar[T]]: ...
 
     def get(
         self,
         var_name: str,
         var_value_type: type[T] = object,
     ) -> Option[GlobalCtxVar[T]]:
-        """Get context variable by name.
-        Returns `GlobalCtxVar[value_type]` object."""
+        """Get context variable by name."""
 
         generic_types = typing.get_args(get_orig_class(self))
         if generic_types and var_value_type is object:
             var_value_type = generic_types[0]
         var = dict.get(self, var_name)
         if var is None:
-            return Nothing
+            return Nothing()
         assert type_check(
             var.value, var_value_type
         ), "Context variable value type of {!r} does not correspond to the expected type {!r}.".format(
             type(var.value).__name__,
-            getattr(var_value_type, "__name__")
-            if isinstance(var_value_type, type)
-            else repr(var_value_type),
+            (
+                getattr(var_value_type, "__name__")
+                if isinstance(var_value_type, type)
+                else repr(var_value_type)
+            ),
         )
         return Some(var)
 
     @typing.overload
-    def get_value(self, var_name: str) -> Option[CtxValueT]:
-        ...
+    def get_value(self, var_name: str) -> Option[CtxValueT]: ...
 
     @typing.overload
     def get_value(
         self,
         var_name: str,
         var_value_type: type[T],
-    ) -> Option[T]:
-        ...
+    ) -> Option[T]: ...
 
     def get_value(
         self,
         var_name: str,
         var_value_type: type[T] = object,
     ) -> Option[T]:
         """Get context variable value by name."""
@@ -394,16 +395,15 @@
 
     def rename(self, old_var_name: str, new_var_name: str) -> Result[_, str]:
         """Rename context variable."""
 
         var = self.get(old_var_name).unwrap()
         if var.const:
             return Error(
-                f"Unable to rename variable {old_var_name!r}, "
-                "because it's a constant."
+                f"Unable to rename variable {old_var_name!r}, " "because it's a constant."
             )
         del self[old_var_name]
         self[new_var_name] = var.value
         return Ok(_())
 
     def clear(self, *, include_consts: bool = False) -> None:
         """Clear context. If `include_consts = True`,
```

### Comparing `mubble-1.0.0/mubble/tools/global_context/mubble_ctx.py` & `mubble-1.1.0/mubble/tools/global_context/mubble_ctx.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/tools/i18n/base.py` & `mubble-1.1.0/mubble/tools/i18n/base.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/tools/i18n/middleware/base.py` & `mubble-1.1.0/mubble/tools/i18n/middleware/base.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/tools/i18n/simple.py` & `mubble-1.1.0/mubble/tools/i18n/simple.py`

 * *Files identical despite different names*

### Comparing `mubble-1.0.0/mubble/tools/kb_set/yaml.py` & `mubble-1.1.0/mubble/tools/kb_set/yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import yaml
 
 from mubble.tools.keyboard import InlineKeyboard, Keyboard
 
 from .base import KeyboardSetBase, KeyboardSetError
 
-PathLike = str | os.PathLike[str]
+PathLike: typing.TypeAlias = str | os.PathLike[str]
 
 
 class KeyboardSetYAML(KeyboardSetBase):
     __config__: PathLike
 
     @classmethod
     def load(cls) -> None:
@@ -31,17 +31,15 @@
         for name, hint in typing.get_type_hints(cls).items():
             g = re.match(r"(?:kb_|keyboard_)(.+)", name.lower())
             if not g:
                 continue
 
             short_name = g.group(1)
             if short_name not in config:
-                raise KeyboardSetError(
-                    f"Keyboard {short_name!r} is undefined in config."
-                )
+                raise KeyboardSetError(f"Keyboard {short_name!r} is undefined in config.")
 
             kb_config = config[short_name]
             if (
                 not isinstance(kb_config, dict)
                 or "buttons" not in kb_config
                 or not isinstance(kb_config["buttons"], list)
             ):
```

### Comparing `mubble-1.0.0/mubble/tools/keyboard.py` & `mubble-1.1.0/mubble/tools/keyboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,39 @@
 import dataclasses
 import typing
 from abc import ABC, abstractmethod
+from types import NoneType
 
-from mubble.option import Nothing, Some
-from mubble.option.msgspec_option import Option
+from fntypes.option import Nothing, Some
+
+from mubble.msgspec_utils import Option
 from mubble.types.objects import (
     InlineKeyboardMarkup,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .buttons import Button, ButtonT, InlineButton, RowButtons
 
-DictStrAny = dict[str, typing.Any]
-AnyMarkup = InlineKeyboardMarkup | ReplyKeyboardMarkup
-
-
-def keyboard_remove(*, selective: bool | None = None) -> ReplyKeyboardRemove:
-    return ReplyKeyboardRemove(
-        remove_keyboard=True,
-        selective=Nothing if selective is None else Some(selective),
-    )
+DictStrAny: typing.TypeAlias = dict[str, typing.Any]
+AnyMarkup: typing.TypeAlias = InlineKeyboardMarkup | ReplyKeyboardMarkup
 
 
 @dataclasses.dataclass
 class KeyboardModel:
     resize_keyboard: bool | Option[bool]
     one_time_keyboard: bool | Option[bool]
     selective: bool | Option[bool]
     is_persistent: bool | Option[bool]
-    keyboard: list[list[dict]]
+    keyboard: list[list[DictStrAny]]
 
 
-class ABCMarkup(ABC, KeyboardModel, typing.Generic[ButtonT]):
+class ABCMarkup(ABC, typing.Generic[ButtonT]):
     BUTTON: type[ButtonT]
-
-    def __init__(
-        self,
-        *,
-        resize_keyboard: bool = True,
-        one_time_keyboard: bool = False,
-        selective: bool = False,
-        is_persistent: bool = False,
-    ):
-        self.keyboard = [[]]
-        self.resize_keyboard = resize_keyboard
-        self.one_time_keyboard = one_time_keyboard
-        self.selective = selective
-        self.is_persistent = is_persistent
+    keyboard: list[list[DictStrAny]]
 
     @abstractmethod
     def dict(self) -> DictStrAny:
         pass
 
     @abstractmethod
     def get_markup(self) -> AnyMarkup:
@@ -60,15 +42,15 @@
     @classmethod
     def empty(cls) -> AnyMarkup:
         return cls().get_markup()
 
     def add(self, row_or_button: RowButtons[ButtonT] | ButtonT) -> typing.Self:
         if not len(self.keyboard):
             self.row()
-
+        
         if isinstance(row_or_button, RowButtons):
             self.keyboard[-1].extend(row_or_button.get_data())
             if row_or_button.auto_row:
                 self.row()
             return self
 
         self.keyboard[-1].append(row_or_button.get_data())
@@ -77,55 +59,70 @@
     def row(self) -> typing.Self:
         if len(self.keyboard) and not len(self.keyboard[-1]):
             raise RuntimeError("Last row is empty!")
 
         self.keyboard.append([])
         return self
 
-    def format(self, **format_data: typing.Dict[str, str]) -> "ABCMarkup":
+    def format(self, **format_data: str) -> typing.Self:
         copy_keyboard = self.__class__()
         for row in self.keyboard:
             for button in row:
                 copy_button = button.copy()
                 copy_button["text"] = copy_button["text"].format(**format_data)
                 copy_keyboard.add(self.BUTTON(**copy_button))
             copy_keyboard.row()
         return copy_keyboard
 
     def merge(self, other: typing.Self) -> typing.Self:
         self.keyboard.extend(other.keyboard)
         return self
 
 
-class Keyboard(ABCMarkup[Button]):
+@dataclasses.dataclass(kw_only=True)
+class Keyboard(ABCMarkup[Button], KeyboardModel):
     BUTTON = Button
 
+    keyboard: list[list[DictStrAny]] = dataclasses.field(
+        default_factory=lambda: [[]],
+        init=False,
+    )
+    resize_keyboard: bool = dataclasses.field(default=True)
+    one_time_keyboard: bool = dataclasses.field(default=False)
+    selective: bool = dataclasses.field(default=False)
+    is_persistent: bool = dataclasses.field(default=False)
+
     def dict(self) -> DictStrAny:
         self.keyboard = [row for row in self.keyboard if row]
         return {
             k: v.unwrap() if v and isinstance(v, Some) else v
             for k, v in self.__dict__.items()
-            if v not in (None, Nothing)
+            if type(v) not in (NoneType, Nothing)
         }
 
     def get_markup(self) -> ReplyKeyboardMarkup:
         return ReplyKeyboardMarkup(**self.dict())
 
+    def get_empty_markup(self, *, selective: bool = False) -> ReplyKeyboardRemove:
+        return ReplyKeyboardRemove(remove_keyboard=True, selective=Some(selective))
+
 
 class InlineKeyboard(ABCMarkup[InlineButton]):
     BUTTON = InlineButton
 
+    def __init__(self) -> None:
+        self.keyboard = [[]]
+
     def dict(self) -> DictStrAny:
         self.keyboard = [row for row in self.keyboard if row]
         return dict(inline_keyboard=self.keyboard)
 
     def get_markup(self) -> InlineKeyboardMarkup:
         return InlineKeyboardMarkup(**self.dict())
 
 
 __all__ = (
     "ABCMarkup",
     "InlineKeyboard",
     "Keyboard",
     "KeyboardModel",
-    "keyboard_remove",
 )
```

### Comparing `mubble-1.0.0/mubble/tools/magic.py` & `mubble-1.1.0/mubble/tools/magic.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 
 if typing.TYPE_CHECKING:
     from mubble.bot.rules.abc import ABCRule
 
     T = typing.TypeVar("T", bound=ABCRule)
 
-FuncType = types.FunctionType | typing.Callable
-TRANSLATIONS_KEY = "_translations"
+FuncType: typing.TypeAlias = types.FunctionType | typing.Callable[..., typing.Any]
+TRANSLATIONS_KEY: typing.Final[str] = "_translations"
 
 
 def resolve_arg_names(func: FuncType, start_idx: int = 1) -> tuple[str, ...]:
     return func.__code__.co_varnames[start_idx : func.__code__.co_argcount]
 
 
 def get_default_args(func: FuncType) -> dict[str, typing.Any]:
@@ -24,15 +24,15 @@
 def to_str(s: str | enum.Enum) -> str:
     if isinstance(s, enum.Enum):
         return str(s.value)
     return s
 
 
 def magic_bundle(
-    handler: FuncType,
+    handler: FuncType, 
     kw: dict[str | enum.Enum, typing.Any],
     *,
     start_idx: int = 1,
     bundle_ctx: bool = True,
 ) -> dict[str, typing.Any]:
     names = resolve_arg_names(handler, start_idx=start_idx)
     args = get_default_args(handler)
```

### Comparing `mubble-1.0.0/mubble/types/enums.py` & `mubble-1.1.0/mubble/types/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     SQL = "sql"
     F_SHARP = "fs"
     FORTRAN = "fortran"
     KOTLIN = "kotlin"
     HTML = "html"
     YAML = "yaml"
     JSON = "json"
+    MARKDOWN = "markdown"
+    MARKUP = "markup"
 
 
 class ChatAction(str, enum.Enum):
     """Type of ChatAction.
 
     Choose one, depending on what the user is about to receive:
     - typing for text messages,
@@ -61,16 +63,128 @@
     UPLOAD_DOCUMENT = "upload_document"
     CHOOSE_STICKER = "choose_sticker"
     FIND_LOCATION = "find_location"
     RECORD_VIDEO_NOTE = "record_video_note"
     UPLOAD_VIDEO_NOTE = "upload_video_note"
 
 
+class ReactionEmoji(str, enum.Enum):
+    """Type of ReactionEmoji.
+
+    Currently, it can be one of `👍`, `👎`, `❤`, `🔥`, `🥰`, `👏`,
+    `😁`, `🤔`, `🤯`, `😱`, `🤬`, `😢`, `🎉`, `🤩`, `🤮`, `💩`, `🙏`, `👌`, `🕊`, `🤡`, `🥱`,
+    `🥴`, `😍`, `🐳`, `❤‍🔥`, `🌚`, `🌭`, `💯`, `🤣`, `⚡`, `🍌`, `🏆`, `💔`, `🤨`, `😐`, `🍓`,
+    `🍾`, `💋`, `🖕`, `😈`, `😴`, `😭`, `🤓`, `👻`, `👨‍💻`, `👀`, `🎃`, `🙈`, `😇`, `😨`, `🤝`,
+    `✍`, `🤗`, `🫡`, `🎅`, `🎄`, `☃`, `💅`, `🤪`, `🗿`, `🆒`, `💘`, `🙉`, `🦄`, `😘`, `💊`,
+    `🙊`, `😎`, `👾`, `🤷‍♂`, `🤷`, `🤷‍♀`, `😡`.
+
+    Docs: https://core.telegram.org/bots/api#reactiontypeemoji"""
+
+    THUMBS_UP = "👍"
+    THUMBS_DOWN = "👎"
+    RED_HEART = "❤"
+    FIRE = "🔥"
+    SMILING_FACE_WITH_HEARTS = "🥰"
+    CLAPPING_HANDS = "👏"
+    BEAMING_FACE_WITH_SMILING_EYES = "😁"
+    THINKING_FACE = "🤔"
+    EXPLODING_HEAD = "🤯"
+    FACE_SCREAMING_IN_FEAR = "😱"
+    FACE_WITH_SYMBOLS_ON_MOUTH = "🤬"
+    CRYING_FACE = "😢"
+    PARTY_POPPER = "🎉"
+    STAR_STRUCK = "🤩"
+    FACE_VOMITING = "🤮"
+    PILE_OF_POO = "💩"
+    FOLDED_HANDS = "🙏"
+    OK_HAND = "👌"
+    DOVE = "🕊"
+    CLOWN_FACE = "🤡"
+    YAWNING_FACE = "🥱"
+    WOOZY_FACE = "🥴"
+    SMILING_FACE_WITH_HEART_EYES = "😍"
+    SPOUTING_WHALE = "🐳"
+    HEART_ON_FIRE = "❤‍🔥"
+    NEW_MOON_FACE = "🌚"
+    HOT_DOG = "🌭"
+    HUNDRED_POINTS = "💯"
+    ROLLING_ON_THE_FLOOR_LAUGHING = "🤣"
+    HIGH_VOLTAGE = "⚡"
+    BANANA = "🍌"
+    TROPHY = "🏆"
+    BROKEN_HEART = "💔"
+    FACE_WITH_RAISED_EYEBROW = "🤨"
+    NEUTRAL_FACE = "😐"
+    STRAWBERRY = "🍓"
+    BOTTLE_WITH_POPPING_CORK = "🍾"
+    KISS_MARK = "💋"
+    MIDDLE_FINGER = "🖕"
+    SMILING_FACE_WITH_HORNS = "😈"
+    SLEEPING_FACE = "😴"
+    LOUDLY_CRYING_FACE = "😭"
+    NERD_FACE = "🤓"
+    GHOST = "👻"
+    MAN_TECHNOLOGIST = "👨‍💻"
+    EYES = "👀"
+    JACK_O_LANTERN = "🎃"
+    SEE_NO_EVIL_MONKEY = "🙈"
+    SMILING_FACE_WITH_HALO = "😇"
+    FEARFUL_FACE = "😨"
+    HANDSHAKE = "🤝"
+    WRITING_HAND = "✍"
+    SMILING_FACE_WITH_OPEN_HANDS = "🤗"
+    SALUTING_FACE = "🫡"
+    SANTA_CLAUS = "🎅"
+    CHRISTMAS_TREE = "🎄"
+    SNOWMAN = "☃"
+    NAIL_POLISH = "💅"
+    ZANY_FACE = "🤪"
+    MOAI = "🗿"
+    COOL_BUTTON = "🆒"
+    HEART_WITH_ARROW = "💘"
+    HEAR_NO_EVIL_MONKEY = "🙉"
+    UNICORN = "🦄"
+    FACE_BLOWING_A_KISS = "😘"
+    PILL = "💊"
+    SPEAK_NO_EVIL_MONKEY = "🙊"
+    SMILING_FACE_WITH_SUNGLASSES = "😎"
+    ALIEN_MONSTER = "👾"
+    MAN_SHRUGGING = "🤷‍♂"
+    PERSON_SHRUGGING = "🤷"
+    WOMAN_SHRUGGING = "🤷‍♀"
+    ENRAGED_FACE = "😡"
+
+
+class DefaultAccentColor(int, enum.Enum):
+    """Type of DefaultAccentColor.
+
+    One of 7 possible user colors:
+    - Red
+    - Orange
+    - Purple
+    - Green
+    - Cyan
+    - Blue
+    - Pink
+
+    Docs: https://core.telegram.org/bots/api#accent-colors
+    """
+
+    RED = 0
+    ORANGE = 1
+    PURPLE = 2
+    GREEN = 3
+    CYAN = 4
+    BLUE = 5
+    PINK = 6
+
+
 class TopicIconColor(int, enum.Enum):
     """Type of TopicIconColor.
+
     Docs: https://github.com/telegramdesktop/tdesktop/blob/991fe491c5ae62705d77aa8fdd44a79caf639c45/Telegram/SourceFiles/data/data_forum_topic.cpp#L51-L56
     """
 
     BLUE = 0x6FB9F0
     YELLOW = 0xFFD67E
     VIOLET = 0xCB86DB
     GREEN = 0x8EEE98
@@ -109,14 +223,15 @@
     LOCATION = "location"
     NEW_CHAT_MEMBERS = "new_chat_members"
     LEFT_CHAT_MEMBER = "left_chat_member"
     NEW_CHAT_TITLE = "new_chat_title"
     NEW_CHAT_PHOTO = "new_chat_photo"
     DELETE_CHAT_PHOTO = "delete_chat_photo"
     GROUP_CHAT_CREATED = "group_chat_created"
+    BOOST_ADDED = "boost_added"
     SUPERGROUP_CHAT_CREATED = "supergroup_chat_created"
     CHANNEL_CHAT_CREATED = "channel_chat_created"
     MESSAGE_AUTO_DELETE_TIMER_CHANGED = "message_auto_delete_timer_changed"
     MIGRATE_TO_CHAT_ID = "migrate_to_chat_id"
     MIGRATE_FROM_CHAT_ID = "migrate_from_chat_id"
     PINNED_MESSAGE = "pinned_message"
     INVOICE = "invoice"
@@ -296,14 +411,18 @@
     POLL = "poll"
     POLL_ANSWER = "poll_answer"
     MY_CHAT_MEMBER = "my_chat_member"
     CHAT_MEMBER = "chat_member"
     CHAT_JOIN_REQUEST = "chat_join_request"
     CHAT_BOOST = "chat_boost"
     REMOVED_CHAT_BOOST = "removed_chat_boost"
+    BUSINESS_CONNECTION = "business_connection"
+    BUSINESS_MESSAGE = "business_message"
+    EDITED_BUSINESS_MESSAGE = "edited_business_message"
+    DELETE_BUSINESS_MESSAGE = "delete_business_messages"
 
 
 class BotCommandScopeType(str, enum.Enum):
     """Type of BotCommandScope.
     Represents the scope to which bot commands are applied."""
 
     DEFAULT = "default"
@@ -528,112 +647,13 @@
     RENTAL_AGREEMENT = "rental_agreement"
     PASSPORT_REGISTRATION = "passport_registration"
     TEMPORARY_REGISTRATION = "temporary_registration"
     PHONE_NUMBER = "phone_number"
     EMAIL = "email"
 
 
-class PassportElementErrorDataFieldType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the error, one of “personal_details”,
-    “passport”, “driver_license”, “identity_card”, “internal_passport”,
-    “address”"""
-
-    PERSONAL_DETAILS = "personal_details"
-    PASSPORT = "passport"
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-    INTERNAL_PASSPORT = "internal_passport"
-    ADDRESS = "address"
-
-
-class PassportElementErrorFrontSideType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the issue, one of “passport”,
-    “driver_license”, “identity_card”, “internal_passport”"""
-
-    PASSPORT = "passport"
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-    INTERNAL_PASSPORT = "internal_passport"
-
-
-class PassportElementErrorReverseSideType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the issue, one of “driver_license”,
-    “identity_card”"""
-
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-
-
-class PassportElementErrorSelfieType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the issue, one of “passport”,
-    “driver_license”, “identity_card”, “internal_passport”"""
-
-    PASSPORT = "passport"
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-    INTERNAL_PASSPORT = "internal_passport"
-
-
-class PassportElementErrorFileType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the issue, one of “utility_bill”,
-    “bank_statement”, “rental_agreement”, “passport_registration”,
-    “temporary_registration”"""
-
-    UTILITY_BILL = "utility_bill"
-    BANK_STATEMENT = "bank_statement"
-    RENTAL_AGREEMENT = "rental_agreement"
-    PASSPORT_REGISTRATION = "passport_registration"
-    TEMPORARY_REGISTRATION = "temporary_registration"
-
-
-class PassportElementErrorFilesType(str, enum.Enum):
-    """The section of the user's Telegram Passport which has the issue, one of “utility_bill”,
-    “bank_statement”, “rental_agreement”, “passport_registration”,
-    “temporary_registration”"""
-
-    UTILITY_BILL = "utility_bill"
-    BANK_STATEMENT = "bank_statement"
-    RENTAL_AGREEMENT = "rental_agreement"
-    PASSPORT_REGISTRATION = "passport_registration"
-    TEMPORARY_REGISTRATION = "temporary_registration"
-
-
-class PassportElementErrorTranslationFileType(str, enum.Enum):
-    """Type of element of the user's Telegram Passport which has the issue, one
-    of “passport”, “driver_license”, “identity_card”, “internal_passport”,
-    “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”,
-    “temporary_registration”"""
-
-    PASSPORT = "passport"
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-    INTERNAL_PASSPORT = "internal_passport"
-    UTILITY_BILL = "utility_bill"
-    BANK_STATEMENT = "bank_statement"
-    RENTAL_AGREEMENT = "rental_agreement"
-    PASSPORT_REGISTRATION = "passport_registration"
-    TEMPORARY_REGISTRATION = "temporary_registration"
-
-
-class PassportElementErrorTranslationFilesType(str, enum.Enum):
-    """Type of element of the user's Telegram Passport which has the issue, one
-    of “passport”, “driver_license”, “identity_card”, “internal_passport”,
-    “utility_bill”, “bank_statement”, “rental_agreement”, “passport_registration”,
-    “temporary_registration”"""
-
-    PASSPORT = "passport"
-    DRIVER_LICENSE = "driver_license"
-    IDENTITY_CARD = "identity_card"
-    INTERNAL_PASSPORT = "internal_passport"
-    UTILITY_BILL = "utility_bill"
-    BANK_STATEMENT = "bank_statement"
-    RENTAL_AGREEMENT = "rental_agreement"
-    PASSPORT_REGISTRATION = "passport_registration"
-    TEMPORARY_REGISTRATION = "temporary_registration"
-
-
 class StickerFormat(str, enum.Enum):
     """Format of the sticker."""
 
     STATIC = "static"
     ANIMATED = "animated"
     VIDEO = "video"
```

### Comparing `mubble-1.0.0/mubble/types/methods.py` & `mubble-1.1.0/mubble/types/methods.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,3724 +1,4332 @@
 import typing
 
+from fntypes.co import Result, Variative
+
 from mubble.api.error import APIError
 from mubble.model import full_result, get_params
-from mubble.option.msgspec_option import Option
-from mubble.option.option import Nothing
-from mubble.result import Result
-from mubble.types.objects import *
+from mubble.types.objects import *  # noqa: F403
 
 if typing.TYPE_CHECKING:
     from mubble.api.abc import ABCAPI
 
 
 class APIMethods:
+    """Telegram Bot API 7.2 methods, released `March 31, 2024`."""
+
     def __init__(self, api: "ABCAPI") -> None:
         self.api = api
 
     async def get_updates(
         self,
-        offset: int | Option[int] = Nothing,
-        limit: int | Option[int] = Nothing,
-        timeout: int | Option[int] = Nothing,
-        allowed_updates: list[str] | Option[list[str]] = Nothing,
+        offset: int | None = None,
+        limit: int | None = None,
+        timeout: int | None = None,
+        allowed_updates: list[str] | None = None,
         **other: typing.Any,
-    ) -> Result[list[Update], "APIError"]:
+    ) -> Result[list[Update], APIError]:
         """Method `getUpdates`, see the [documentation](https://core.telegram.org/bots/api#getupdates)
 
-        Use this method to receive incoming updates using long polling (wiki). Returns an Array of Update objects.
+        Use this method to receive incoming updates using long polling (wiki). 
+        Returns an Array of Update objects.
 
-        :param offset: Identifier of the first update to be returned. Must be greater by one than
-        the highest among the identifiers of previously received updates. By default,
-        updates starting with the earliest unconfirmed update are returned. An
-        update is considered confirmed as soon as getUpdates is called with an offset
-        higher than its update_id. The negative offset can be specified to retrieve
-        updates starting from -offset update from the end of the updates queue.
+        :param offset: Identifier of the first update to be returned. Must be greater by one than \
+        the highest among the identifiers of previously received updates. By default, \
+        updates starting with the earliest unconfirmed update are returned. An \
+        update is considered confirmed as soon as getUpdates is called with an offset \
+        higher than its update_id. The negative offset can be specified to retrieve \
+        updates starting from -offset update from the end of the updates queue. \
         All previous updates will be forgotten.
 
-        :param limit: Limits the number of updates to be retrieved. Values between 1-100 are accepted.
+        :param limit: Limits the number of updates to be retrieved. Values between 1-100 are accepted. \
         Defaults to 100.
 
-        :param timeout: Timeout in seconds for long polling. Defaults to 0, i.e. usual short polling.
-        Should be positive, short polling should be used for testing purposes only.
+        :param timeout: Timeout in seconds for long polling. Defaults to 0, i.e. usual short polling. \
+        Should be positive, short polling should be used for testing purposes only. \
 
-        :param allowed_updates: A JSON-serialized list of the update types you want your bot to receive.
-        For example, specify [`message`, `edited_channel_post`, `callback_query`]
-        to only receive updates of these types. See Update for a complete list of
-        available update types. Specify an empty list to receive all update types
-        except chat_member, message_reaction, and message_reaction_count
-        (default). If not specified, the previous setting will be used. Please
-        note that this parameter doesn't affect updates created before the call
-        to the getUpdates, so unwanted updates may be received for a short period
-        of time."""
+        :param allowed_updates: A JSON-serialized list of the update types you want your bot to receive. \
+        For example, specify [`message`, `edited_channel_post`, `callback_query`] \
+        to only receive updates of these types. See Update for a complete list of \
+        available update types. Specify an empty list to receive all update types \
+        except chat_member, message_reaction, and message_reaction_count \
+        (default). If not specified, the previous setting will be used. Please \
+        note that this parameter doesn't affect updates created before the call \
+        to the getUpdates, so unwanted updates may be received for a short period \
+        of time.
+        """
 
-        method_response = await self.api.request_raw("getUpdates", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "getUpdates",
+            get_params(locals()),
+        )
         return full_result(method_response, list[Update])
 
     async def set_webhook(
         self,
         url: str,
-        certificate: InputFile | Option[InputFile] = Nothing,
-        ip_address: str | Option[str] = Nothing,
-        max_connections: int | Option[int] = Nothing,
-        allowed_updates: list[str] | Option[list[str]] = Nothing,
-        drop_pending_updates: bool | Option[bool] = Nothing,
-        secret_token: str | Option[str] = Nothing,
+        certificate: InputFile | None = None,
+        ip_address: str | None = None,
+        max_connections: int | None = None,
+        allowed_updates: list[str] | None = None,
+        drop_pending_updates: bool | None = None,
+        secret_token: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setWebhook`, see the [documentation](https://core.telegram.org/bots/api#setwebhook)
 
-        Use this method to specify a URL and receive incoming updates via an outgoing webhook. Whenever there is an update for the bot, we will send an HTTPS POST request to the specified URL, containing a JSON-serialized Update. In case of an unsuccessful request, we will give up after a reasonable amount of attempts. Returns True on success.
-        If you'd like to make sure that the webhook was set by you, you can specify secret data in the parameter secret_token. If specified, the request will contain a header "X-Telegram-Bot-Api-Secret-Token" with the secret token as content.
+        Use this method to specify a URL and receive incoming updates via an outgoing 
+        webhook. Whenever there is an update for the bot, we will send an HTTPS POST 
+        request to the specified URL, containing a JSON-serialized Update. In 
+        case of an unsuccessful request, we will give up after a reasonable amount 
+        of attempts. Returns True on success. If you'd like to make sure that the 
+        webhook was set by you, you can specify secret data in the parameter secret_token. 
+        If specified, the request will contain a header "X-Telegram-Bot-Api-Secret-Token" 
+        with the secret token as content.
 
-        :param url: HTTPS URL to send updates to. Use an empty string to remove webhook integration
+        :param url: HTTPS URL to send updates to. Use an empty string to remove webhook integration. \
 
-        :param certificate: Upload your public key certificate so that the root certificate in use can
+        :param certificate: Upload your public key certificate so that the root certificate in use can \
         be checked. See our self-signed guide for details.
 
-        :param ip_address: The fixed IP address which will be used to send webhook requests instead
-        of the IP address resolved through DNS
+        :param ip_address: The fixed IP address which will be used to send webhook requests instead \
+        of the IP address resolved through DNS.
 
-        :param max_connections: The maximum allowed number of simultaneous HTTPS connections to the webhook
-        for update delivery, 1-100. Defaults to 40. Use lower values to limit the
-        load on your bot's server, and higher values to increase your bot's throughput.
-
-        :param allowed_updates: A JSON-serialized list of the update types you want your bot to receive.
-        For example, specify [`message`, `edited_channel_post`, `callback_query`]
-        to only receive updates of these types. See Update for a complete list of
-        available update types. Specify an empty list to receive all update types
-        except chat_member, message_reaction, and message_reaction_count
-        (default). If not specified, the previous setting will be used. Please
-        note that this parameter doesn't affect updates created before the call
-        to the setWebhook, so unwanted updates may be received for a short period
+        :param max_connections: The maximum allowed number of simultaneous HTTPS connections to the webhook \
+        for update delivery, 1-100. Defaults to 40. Use lower values to limit the \
+        load on your bot's server, and higher values to increase your bot's throughput. \
+
+        :param allowed_updates: A JSON-serialized list of the update types you want your bot to receive. \
+        For example, specify [`message`, `edited_channel_post`, `callback_query`] \
+        to only receive updates of these types. See Update for a complete list of \
+        available update types. Specify an empty list to receive all update types \
+        except chat_member, message_reaction, and message_reaction_count \
+        (default). If not specified, the previous setting will be used. Please \
+        note that this parameter doesn't affect updates created before the call \
+        to the setWebhook, so unwanted updates may be received for a short period \
         of time.
 
-        :param drop_pending_updates: Pass True to drop all pending updates
+        :param drop_pending_updates: Pass True to drop all pending updates.
 
-        :param secret_token: A secret token to be sent in a header `X-Telegram-Bot-Api-Secret-Token`
-        in every webhook request, 1-256 characters. Only characters A-Z, a-z,
-        0-9, _ and - are allowed. The header is useful to ensure that the request comes
-        from a webhook set by you."""
+        :param secret_token: A secret token to be sent in a header `X-Telegram-Bot-Api-Secret-Token` \
+        in every webhook request, 1-256 characters. Only characters A-Z, a-z, \
+        0-9, _ and - are allowed. The header is useful to ensure that the request comes \
+        from a webhook set by you.
+        """
 
-        method_response = await self.api.request_raw("setWebhook", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "setWebhook",
+            get_params(locals()),
+        )
         return full_result(method_response, bool)
 
     async def delete_webhook(
         self,
-        drop_pending_updates: bool | Option[bool] = Nothing,
+        drop_pending_updates: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteWebhook`, see the [documentation](https://core.telegram.org/bots/api#deletewebhook)
 
-        Use this method to remove webhook integration if you decide to switch back to getUpdates. Returns True on success.
+        Use this method to remove webhook integration if you decide to switch back
+        to getUpdates. Returns True on success.
 
-        :param drop_pending_updates: Pass True to drop all pending updates"""
+        :param drop_pending_updates: Pass True to drop all pending updates.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteWebhook", get_params(locals())
+            "deleteWebhook",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_webhook_info(
-        self,
-        **other: typing.Any,
-    ) -> Result[WebhookInfo, "APIError"]:
+        self, **other: typing.Any
+    ) -> Result[WebhookInfo, APIError]:
         """Method `getWebhookInfo`, see the [documentation](https://core.telegram.org/bots/api#getwebhookinfo)
 
-        Use this method to get current webhook status. Requires no parameters. On success, returns a WebhookInfo object. If the bot is using getUpdates, will return an object with the url field empty.
+        Use this method to get current webhook status. Requires no parameters.
+        On success, returns a WebhookInfo object. If the bot is using getUpdates,
+        will return an object with the url field empty.
         """
 
         method_response = await self.api.request_raw(
-            "getWebhookInfo", get_params(locals())
+            "getWebhookInfo",
+            get_params(locals()),
         )
         return full_result(method_response, WebhookInfo)
 
-    async def get_me(
-        self,
-        **other: typing.Any,
-    ) -> Result[User, "APIError"]:
+    async def get_me(self, **other: typing.Any) -> Result[User, APIError]:
         """Method `getMe`, see the [documentation](https://core.telegram.org/bots/api#getme)
 
-        A simple method for testing your bot's authentication token. Requires no parameters. Returns basic information about the bot in form of a User object.
+        A simple method for testing your bot's authentication token. Requires
+        no parameters. Returns basic information about the bot in form of a User
+        object.
         """
 
-        method_response = await self.api.request_raw("getMe", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "getMe",
+            get_params(locals()),
+        )
         return full_result(method_response, User)
 
-    async def log_out(
-        self,
-        **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    async def log_out(self, **other: typing.Any) -> Result[bool, APIError]:
         """Method `logOut`, see the [documentation](https://core.telegram.org/bots/api#logout)
 
-        Use this method to log out from the cloud Bot API server before launching the bot locally. You must log out the bot before running it locally, otherwise there is no guarantee that the bot will receive updates. After a successful call, you can immediately log in on a local server, but will not be able to log in back to the cloud Bot API server for 10 minutes. Returns True on success. Requires no parameters.
+        Use this method to log out from the cloud Bot API server before launching
+        the bot locally. You must log out the bot before running it locally, otherwise
+        there is no guarantee that the bot will receive updates. After a successful
+        call, you can immediately log in on a local server, but will not be able to
+        log in back to the cloud Bot API server for 10 minutes. Returns True on success.
+        Requires no parameters.
         """
 
-        method_response = await self.api.request_raw("logOut", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "logOut",
+            get_params(locals()),
+        )
         return full_result(method_response, bool)
 
-    async def close(
-        self,
-        **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    async def close(self, **other: typing.Any) -> Result[bool, APIError]:
         """Method `close`, see the [documentation](https://core.telegram.org/bots/api#close)
 
-        Use this method to close the bot instance before moving it from one local server to another. You need to delete the webhook before calling this method to ensure that the bot isn't launched again after server restart. The method will return error 429 in the first 10 minutes after the bot is launched. Returns True on success. Requires no parameters.
+        Use this method to close the bot instance before moving it from one local
+        server to another. You need to delete the webhook before calling this method
+        to ensure that the bot isn't launched again after server restart. The method
+        will return error 429 in the first 10 minutes after the bot is launched. Returns
+        True on success. Requires no parameters.
         """
 
-        method_response = await self.api.request_raw("close", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "close",
+            get_params(locals()),
+        )
         return full_result(method_response, bool)
 
     async def send_message(
         self,
         chat_id: int | str,
         text: str,
-        message_thread_id: int | Option[int] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        link_preview_options: LinkPreviewOptions | Option[LinkPreviewOptions] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        parse_mode: str | None = None,
+        entities: list[MessageEntity] | None = None,
+        link_preview_options: LinkPreviewOptions | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendMessage`, see the [documentation](https://core.telegram.org/bots/api#sendmessage)
 
         Use this method to send text messages. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param text: Text of the message to be sent, 1-4096 characters after entities parsing
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param parse_mode: Mode for parsing entities in the message text. See formatting options for
+        :param text: Text of the message to be sent, 1-4096 characters after entities parsing. \
+
+        :param parse_mode: Mode for parsing entities in the message text. See formatting options for \
         more details.
 
-        :param entities: A JSON-serialized list of special entities that appear in message text,
-        which can be specified instead of parse_mode
+        :param entities: A JSON-serialized list of special entities that appear in message text, \
+        which can be specified instead of parse_mode.
 
-        :param link_preview_options: Link preview generation options for the message
+        :param link_preview_options: Link preview generation options for the message.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendMessage", get_params(locals())
+            "sendMessage",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def forward_message(
         self,
         chat_id: int | str,
         from_chat_id: int | str,
         message_id: int,
-        message_thread_id: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `forwardMessage`, see the [documentation](https://core.telegram.org/bots/api#forwardmessage)
 
-        Use this method to forward messages of any kind. Service messages and messages with protected content can't be forwarded. On success, the sent Message is returned.
+        Use this method to forward messages of any kind. Service messages and messages 
+        with protected content can't be forwarded. On success, the sent Message 
+        is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param from_chat_id: Unique identifier for the chat where the original message was sent (or channel
-        username in the format @channelusername)
+        :param from_chat_id: Unique identifier for the chat where the original message was sent (or channel \
+        username in the format @channelusername).
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the forwarded message from forwarding and saving
+        :param protect_content: Protects the contents of the forwarded message from forwarding and saving. \
 
-        :param message_id: Message identifier in the chat specified in from_chat_id"""
+        :param message_id: Message identifier in the chat specified in from_chat_id.
+        """
 
         method_response = await self.api.request_raw(
-            "forwardMessage", get_params(locals())
+            "forwardMessage",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def forward_messages(
         self,
         chat_id: int | str,
         from_chat_id: int | str,
         message_ids: list[int],
-        message_thread_id: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
         **other: typing.Any,
-    ) -> Result[list[MessageId], "APIError"]:
+    ) -> Result[list[MessageId], APIError]:
         """Method `forwardMessages`, see the [documentation](https://core.telegram.org/bots/api#forwardmessages)
 
-        Use this method to forward multiple messages of any kind. If some of the specified messages can't be found or forwarded, they are skipped. Service messages and messages with protected content can't be forwarded. Album grouping is kept for forwarded messages. On success, an array of MessageId of the sent messages is returned.
-
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
-
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
-
-        :param from_chat_id: Unique identifier for the chat where the original messages were sent (or
-        channel username in the format @channelusername)
-
-        :param message_ids: Identifiers of 1-100 messages in the chat from_chat_id to forward. The
-        identifiers must be specified in a strictly increasing order.
+        Use this method to forward multiple messages of any kind. If some of the specified 
+        messages can't be found or forwarded, they are skipped. Service messages 
+        and messages with protected content can't be forwarded. Album grouping 
+        is kept for forwarded messages. On success, an array of MessageId of the 
+        sent messages is returned.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
+
+        :param from_chat_id: Unique identifier for the chat where the original messages were sent (or \
+        channel username in the format @channelusername).
+
+        :param message_ids: A JSON-serialized list of 1-100 identifiers of messages in the chat from_chat_id \
+        to forward. The identifiers must be specified in a strictly increasing \
+        order.
 
-        :param disable_notification: Sends the messages silently. Users will receive a notification with no
+        :param disable_notification: Sends the messages silently. Users will receive a notification with no \
         sound.
 
-        :param protect_content: Protects the contents of the forwarded messages from forwarding and saving
+        :param protect_content: Protects the contents of the forwarded messages from forwarding and saving. \
         """
 
         method_response = await self.api.request_raw(
-            "forwardMessages", get_params(locals())
+            "forwardMessages",
+            get_params(locals()),
         )
         return full_result(method_response, list[MessageId])
 
     async def copy_message(
         self,
         chat_id: int | str,
         from_chat_id: int | str,
         message_id: int,
-        message_thread_id: int | Option[int] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        message_thread_id: int | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[MessageId, "APIError"]:
+    ) -> Result[MessageId, APIError]:
         """Method `copyMessage`, see the [documentation](https://core.telegram.org/bots/api#copymessage)
 
-        Use this method to copy messages of any kind. Service messages, giveaway messages, giveaway winners messages, and invoice messages can't be copied. A quiz poll can be copied only if the value of the field correct_option_id is known to the bot. The method is analogous to the method forwardMessage, but the copied message doesn't have a link to the original message. Returns the MessageId of the sent message on success.
+        Use this method to copy messages of any kind. Service messages, giveaway 
+        messages, giveaway winners messages, and invoice messages can't be copied. 
+        A quiz poll can be copied only if the value of the field correct_option_id 
+        is known to the bot. The method is analogous to the method forwardMessage, 
+        but the copied message doesn't have a link to the original message. Returns 
+        the MessageId of the sent message on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param from_chat_id: Unique identifier for the chat where the original message was sent (or channel
-        username in the format @channelusername)
+        :param from_chat_id: Unique identifier for the chat where the original message was sent (or channel \
+        username in the format @channelusername).
 
-        :param message_id: Message identifier in the chat specified in from_chat_id
+        :param message_id: Message identifier in the chat specified in from_chat_id.
 
-        :param caption: New caption for media, 0-1024 characters after entities parsing. If not
-        specified, the original caption is kept
+        :param caption: New caption for media, 0-1024 characters after entities parsing. If not \
+        specified, the original caption is kept.
 
-        :param parse_mode: Mode for parsing entities in the new caption. See formatting options for
+        :param parse_mode: Mode for parsing entities in the new caption. See formatting options for \
         more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the new caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the new caption, \
+        which can be specified instead of parse_mode.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove reply keyboard \
+        or to force a reply from the user.
+        """
 
         method_response = await self.api.request_raw(
-            "copyMessage", get_params(locals())
+            "copyMessage",
+            get_params(locals()),
         )
         return full_result(method_response, MessageId)
 
     async def copy_messages(
         self,
         chat_id: int | str,
         from_chat_id: int | str,
         message_ids: list[int],
-        message_thread_id: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        remove_caption: bool | Option[bool] = Nothing,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        remove_caption: bool | None = None,
         **other: typing.Any,
-    ) -> Result[list[MessageId], "APIError"]:
+    ) -> Result[list[MessageId], APIError]:
         """Method `copyMessages`, see the [documentation](https://core.telegram.org/bots/api#copymessages)
 
-        Use this method to copy messages of any kind. If some of the specified messages can't be found or copied, they are skipped. Service messages, giveaway messages, giveaway winners messages, and invoice messages can't be copied. A quiz poll can be copied only if the value of the field correct_option_id is known to the bot. The method is analogous to the method forwardMessages, but the copied messages don't have a link to the original message. Album grouping is kept for copied messages. On success, an array of MessageId of the sent messages is returned.
-
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        Use this method to copy messages of any kind. If some of the specified messages 
+        can't be found or copied, they are skipped. Service messages, giveaway 
+        messages, giveaway winners messages, and invoice messages can't be copied. 
+        A quiz poll can be copied only if the value of the field correct_option_id 
+        is known to the bot. The method is analogous to the method forwardMessages, 
+        but the copied messages don't have a link to the original message. Album 
+        grouping is kept for copied messages. On success, an array of MessageId 
+        of the sent messages is returned.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param from_chat_id: Unique identifier for the chat where the original messages were sent (or \
+        channel username in the format @channelusername).
 
-        :param from_chat_id: Unique identifier for the chat where the original messages were sent (or
-        channel username in the format @channelusername)
+        :param message_ids: A JSON-serialized list of 1-100 identifiers of messages in the chat from_chat_id \
+        to copy. The identifiers must be specified in a strictly increasing order. \
 
-        :param message_ids: Identifiers of 1-100 messages in the chat from_chat_id to copy. The identifiers
-        must be specified in a strictly increasing order.
-
-        :param disable_notification: Sends the messages silently. Users will receive a notification with no
+        :param disable_notification: Sends the messages silently. Users will receive a notification with no \
         sound.
 
-        :param protect_content: Protects the contents of the sent messages from forwarding and saving
+        :param protect_content: Protects the contents of the sent messages from forwarding and saving. \
 
-        :param remove_caption: Pass True to copy the messages without their captions"""
+        :param remove_caption: Pass True to copy the messages without their captions.
+        """
 
         method_response = await self.api.request_raw(
-            "copyMessages", get_params(locals())
+            "copyMessages",
+            get_params(locals()),
         )
         return full_result(method_response, list[MessageId])
 
     async def send_photo(
         self,
         chat_id: int | str,
         photo: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        has_spoiler: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        has_spoiler: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendPhoto`, see the [documentation](https://core.telegram.org/bots/api#sendphoto)
 
         Use this method to send photos. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param photo: Photo to send. Pass a file_id as String to send a photo that exists on the Telegram
-        servers (recommended), pass an HTTP URL as a String for Telegram to get a
-        photo from the Internet, or upload a new photo using multipart/form-data.
-        The photo must be at most 10 MB in size. The photo's width and height must not
-        exceed 10000 in total. Width and height ratio must be at most 20. More information
-        on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param caption: Photo caption (may also be used when resending photos by file_id), 0-1024
-        characters after entities parsing
+        :param photo: Photo to send. Pass a file_id as String to send a photo that exists on the Telegram \
+        servers (recommended), pass an HTTP URL as a String for Telegram to get a \
+        photo from the Internet, or upload a new photo using multipart/form-data. \
+        The photo must be at most 10 MB in size. The photo's width and height must not \
+        exceed 10000 in total. Width and height ratio must be at most 20. More information \
+        on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param parse_mode: Mode for parsing entities in the photo caption. See formatting options
+        :param caption: Photo caption (may also be used when resending photos by file_id), 0-1024 \
+        characters after entities parsing.
+
+        :param parse_mode: Mode for parsing entities in the photo caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param has_spoiler: Pass True if the photo needs to be covered with a spoiler animation
+        :param has_spoiler: Pass True if the photo needs to be covered with a spoiler animation.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendPhoto", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendPhoto",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_audio(
         self,
         chat_id: int | str,
         audio: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        duration: int | Option[int] = Nothing,
-        performer: str | Option[str] = Nothing,
-        title: str | Option[str] = Nothing,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        duration: int | None = None,
+        performer: str | None = None,
+        title: str | None = None,
+        thumbnail: InputFile | str | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendAudio`, see the [documentation](https://core.telegram.org/bots/api#sendaudio)
 
-        Use this method to send audio files, if you want Telegram clients to display them in the music player. Your audio must be in the .MP3 or .M4A format. On success, the sent Message is returned. Bots can currently send audio files of up to 50 MB in size, this limit may be changed in the future.
-        For sending voice messages, use the sendVoice method instead.
+        Use this method to send audio files, if you want Telegram clients to display 
+        them in the music player. Your audio must be in the .MP3 or .M4A format. On 
+        success, the sent Message is returned. Bots can currently send audio files 
+        of up to 50 MB in size, this limit may be changed in the future. For sending 
+        voice messages, use the sendVoice method instead.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param audio: Audio file to send. Pass a file_id as String to send an audio file that exists
-        on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram
-        to get an audio file from the Internet, or upload a new one using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param caption: Audio caption, 0-1024 characters after entities parsing
+        :param audio: Audio file to send. Pass a file_id as String to send an audio file that exists \
+        on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram \
+        to get an audio file from the Internet, or upload a new one using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param parse_mode: Mode for parsing entities in the audio caption. See formatting options
+        :param caption: Audio caption, 0-1024 characters after entities parsing.
+
+        :param parse_mode: Mode for parsing entities in the audio caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param duration: Duration of the audio in seconds
+        :param duration: Duration of the audio in seconds.
 
-        :param performer: Performer
+        :param performer: Performer.
 
-        :param title: Track name
+        :param title: Track name.
 
-        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the
-        file is supported server-side. The thumbnail should be in JPEG format and
-        less than 200 kB in size. A thumbnail's width and height should not exceed
-        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails
-        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>`
-        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the \
+        file is supported server-side. The thumbnail should be in JPEG format and \
+        less than 200 kB in size. A thumbnail's width and height should not exceed \
+        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails \
+        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` \
+        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendAudio", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendAudio",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_document(
         self,
         chat_id: int | str,
         document: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        disable_content_type_detection: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        disable_content_type_detection: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendDocument`, see the [documentation](https://core.telegram.org/bots/api#senddocument)
 
-        Use this method to send general files. On success, the sent Message is returned. Bots can currently send files of any type of up to 50 MB in size, this limit may be changed in the future.
-
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
-
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
-
-        :param document: File to send. Pass a file_id as String to send a file that exists on the Telegram
-        servers (recommended), pass an HTTP URL as a String for Telegram to get a
-        file from the Internet, or upload a new one using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
-
-        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the
-        file is supported server-side. The thumbnail should be in JPEG format and
-        less than 200 kB in size. A thumbnail's width and height should not exceed
-        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails
-        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>`
-        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        Use this method to send general files. On success, the sent Message is returned. 
+        Bots can currently send files of any type of up to 50 MB in size, this limit 
+        may be changed in the future.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
+
+        :param document: File to send. Pass a file_id as String to send a file that exists on the Telegram \
+        servers (recommended), pass an HTTP URL as a String for Telegram to get a \
+        file from the Internet, or upload a new one using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
+
+        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the \
+        file is supported server-side. The thumbnail should be in JPEG format and \
+        less than 200 kB in size. A thumbnail's width and height should not exceed \
+        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails \
+        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` \
+        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param caption: Document caption (may also be used when resending documents by file_id),
-        0-1024 characters after entities parsing
+        :param caption: Document caption (may also be used when resending documents by file_id), \
+        0-1024 characters after entities parsing.
 
-        :param parse_mode: Mode for parsing entities in the document caption. See formatting options
+        :param parse_mode: Mode for parsing entities in the document caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param disable_content_type_detection: Disables automatic server-side content type detection for files uploaded
-        using multipart/form-data
+        :param disable_content_type_detection: Disables automatic server-side content type detection for files uploaded \
+        using multipart/form-data.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendDocument", get_params(locals())
+            "sendDocument",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def send_video(
         self,
         chat_id: int | str,
         video: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        duration: int | Option[int] = Nothing,
-        width: int | Option[int] = Nothing,
-        height: int | Option[int] = Nothing,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        has_spoiler: bool | Option[bool] = Nothing,
-        supports_streaming: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        duration: int | None = None,
+        width: int | None = None,
+        height: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        has_spoiler: bool | None = None,
+        supports_streaming: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendVideo`, see the [documentation](https://core.telegram.org/bots/api#sendvideo)
 
-        Use this method to send video files, Telegram clients support MPEG4 videos (other formats may be sent as Document). On success, the sent Message is returned. Bots can currently send video files of up to 50 MB in size, this limit may be changed in the future.
+        Use this method to send video files, Telegram clients support MPEG4 videos 
+        (other formats may be sent as Document). On success, the sent Message is 
+        returned. Bots can currently send video files of up to 50 MB in size, this 
+        limit may be changed in the future.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param video: Video to send. Pass a file_id as String to send a video that exists on the Telegram
-        servers (recommended), pass an HTTP URL as a String for Telegram to get a
-        video from the Internet, or upload a new video using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param video: Video to send. Pass a file_id as String to send a video that exists on the Telegram \
+        servers (recommended), pass an HTTP URL as a String for Telegram to get a \
+        video from the Internet, or upload a new video using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param duration: Duration of sent video in seconds
+        :param duration: Duration of sent video in seconds.
 
-        :param width: Video width
+        :param width: Video width.
 
-        :param height: Video height
+        :param height: Video height.
 
-        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the
-        file is supported server-side. The thumbnail should be in JPEG format and
-        less than 200 kB in size. A thumbnail's width and height should not exceed
-        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails
-        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>`
-        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the \
+        file is supported server-side. The thumbnail should be in JPEG format and \
+        less than 200 kB in size. A thumbnail's width and height should not exceed \
+        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails \
+        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` \
+        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param caption: Video caption (may also be used when resending videos by file_id), 0-1024
-        characters after entities parsing
+        :param caption: Video caption (may also be used when resending videos by file_id), 0-1024 \
+        characters after entities parsing.
 
-        :param parse_mode: Mode for parsing entities in the video caption. See formatting options
+        :param parse_mode: Mode for parsing entities in the video caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param has_spoiler: Pass True if the video needs to be covered with a spoiler animation
+        :param has_spoiler: Pass True if the video needs to be covered with a spoiler animation.
 
-        :param supports_streaming: Pass True if the uploaded video is suitable for streaming
+        :param supports_streaming: Pass True if the uploaded video is suitable for streaming.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendVideo", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendVideo",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_animation(
         self,
         chat_id: int | str,
         animation: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        duration: int | Option[int] = Nothing,
-        width: int | Option[int] = Nothing,
-        height: int | Option[int] = Nothing,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        has_spoiler: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        duration: int | None = None,
+        width: int | None = None,
+        height: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        has_spoiler: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendAnimation`, see the [documentation](https://core.telegram.org/bots/api#sendanimation)
 
-        Use this method to send animation files (GIF or H.264/MPEG-4 AVC video without sound). On success, the sent Message is returned. Bots can currently send animation files of up to 50 MB in size, this limit may be changed in the future.
+        Use this method to send animation files (GIF or H.264/MPEG-4 AVC video without 
+        sound). On success, the sent Message is returned. Bots can currently send 
+        animation files of up to 50 MB in size, this limit may be changed in the future.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param animation: Animation to send. Pass a file_id as String to send an animation that exists
-        on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram
-        to get an animation from the Internet, or upload a new animation using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param animation: Animation to send. Pass a file_id as String to send an animation that exists \
+        on the Telegram servers (recommended), pass an HTTP URL as a String for Telegram \
+        to get an animation from the Internet, or upload a new animation using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param duration: Duration of sent animation in seconds
+        :param duration: Duration of sent animation in seconds.
 
-        :param width: Animation width
+        :param width: Animation width.
 
-        :param height: Animation height
+        :param height: Animation height.
 
-        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the
-        file is supported server-side. The thumbnail should be in JPEG format and
-        less than 200 kB in size. A thumbnail's width and height should not exceed
-        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails
-        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>`
-        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the \
+        file is supported server-side. The thumbnail should be in JPEG format and \
+        less than 200 kB in size. A thumbnail's width and height should not exceed \
+        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails \
+        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` \
+        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param caption: Animation caption (may also be used when resending animation by file_id),
-        0-1024 characters after entities parsing
+        :param caption: Animation caption (may also be used when resending animation by file_id), \
+        0-1024 characters after entities parsing.
 
-        :param parse_mode: Mode for parsing entities in the animation caption. See formatting options
+        :param parse_mode: Mode for parsing entities in the animation caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param has_spoiler: Pass True if the animation needs to be covered with a spoiler animation
+        :param has_spoiler: Pass True if the animation needs to be covered with a spoiler animation. \
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendAnimation", get_params(locals())
+            "sendAnimation",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def send_voice(
         self,
         chat_id: int | str,
         voice: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        duration: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendVoice`, see the [documentation](https://core.telegram.org/bots/api#sendvoice)
 
-        Use this method to send audio files, if you want Telegram clients to display the file as a playable voice message. For this to work, your audio must be in an .OGG file encoded with OPUS (other formats may be sent as Audio or Document). On success, the sent Message is returned. Bots can currently send voice messages of up to 50 MB in size, this limit may be changed in the future.
+        Use this method to send audio files, if you want Telegram clients to display 
+        the file as a playable voice message. For this to work, your audio must be 
+        in an .OGG file encoded with OPUS (other formats may be sent as Audio or Document). 
+        On success, the sent Message is returned. Bots can currently send voice 
+        messages of up to 50 MB in size, this limit may be changed in the future.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param voice: Audio file to send. Pass a file_id as String to send a file that exists on the
-        Telegram servers (recommended), pass an HTTP URL as a String for Telegram
-        to get a file from the Internet, or upload a new one using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param voice: Audio file to send. Pass a file_id as String to send a file that exists on the \
+        Telegram servers (recommended), pass an HTTP URL as a String for Telegram \
+        to get a file from the Internet, or upload a new one using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param caption: Voice message caption, 0-1024 characters after entities parsing
+        :param caption: Voice message caption, 0-1024 characters after entities parsing.
 
-        :param parse_mode: Mode for parsing entities in the voice message caption. See formatting
+        :param parse_mode: Mode for parsing entities in the voice message caption. See formatting \
         options for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param duration: Duration of the voice message in seconds
+        :param duration: Duration of the voice message in seconds.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendVoice", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendVoice",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_video_note(
         self,
         chat_id: int | str,
         video_note: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        duration: int | Option[int] = Nothing,
-        length: int | Option[int] = Nothing,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        duration: int | None = None,
+        length: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendVideoNote`, see the [documentation](https://core.telegram.org/bots/api#sendvideonote)
 
-        As of v.4.0, Telegram clients support rounded square MPEG4 videos of up to 1 minute long. Use this method to send video messages. On success, the sent Message is returned.
+        As of v.4.0, Telegram clients support rounded square MPEG4 videos of up 
+        to 1 minute long. Use this method to send video messages. On success, the 
+        sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param video_note: Video note to send. Pass a file_id as String to send a video note that exists
-        on the Telegram servers (recommended) or upload a new video using multipart/form-data.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files.
-        Sending video notes by a URL is currently unsupported
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param duration: Duration of sent video in seconds
+        :param video_note: Video note to send. Pass a file_id as String to send a video note that exists \
+        on the Telegram servers (recommended) or upload a new video using multipart/form-data. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
+        Sending video notes by a URL is currently unsupported.
 
-        :param length: Video width and height, i.e. diameter of the video message
+        :param duration: Duration of sent video in seconds.
 
-        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the
-        file is supported server-side. The thumbnail should be in JPEG format and
-        less than 200 kB in size. A thumbnail's width and height should not exceed
-        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails
-        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>`
-        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>.
-        More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param length: Video width and height, i.e. diameter of the video message.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param thumbnail: Thumbnail of the file sent; can be ignored if thumbnail generation for the \
+        file is supported server-side. The thumbnail should be in JPEG format and \
+        less than 200 kB in size. A thumbnail's width and height should not exceed \
+        320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails \
+        can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` \
+        if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. \
+        More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param reply_parameters: Description of the message to reply to
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_parameters: Description of the message to reply to.
+
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendVideoNote", get_params(locals())
+            "sendVideoNote",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def send_media_group(
         self,
         chat_id: int | str,
-        media: list[InputMediaAudio]
-        | list[InputMediaDocument]
-        | list[InputMediaPhoto]
-        | list[InputMediaVideo],
-        message_thread_id: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
+        media: list[
+            InputMediaAudio | InputMediaDocument | InputMediaPhoto | InputMediaVideo
+        ],
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
         **other: typing.Any,
-    ) -> Result[list[Message], "APIError"]:
+    ) -> Result[list[Message], APIError]:
         """Method `sendMediaGroup`, see the [documentation](https://core.telegram.org/bots/api#sendmediagroup)
 
-        Use this method to send a group of photos, videos, documents or audios as an album. Documents and audio files can be only grouped in an album with messages of the same type. On success, an array of Messages that were sent is returned.
+        Use this method to send a group of photos, videos, documents or audios as 
+        an album. Documents and audio files can be only grouped in an album with messages 
+        of the same type. On success, an array of Messages that were sent is returned.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param media: A JSON-serialized array describing messages to be sent, must include 2-10
-        items
+        :param media: A JSON-serialized array describing messages to be sent, must include 2-10 \
+        items.
 
-        :param disable_notification: Sends messages silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends messages silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent messages from forwarding and saving
+        :param protect_content: Protects the contents of the sent messages from forwarding and saving. \
 
-        :param reply_parameters: Description of the message to reply to"""
+        :param reply_parameters: Description of the message to reply to.
+        """
 
         method_response = await self.api.request_raw(
-            "sendMediaGroup", get_params(locals())
+            "sendMediaGroup",
+            get_params(locals()),
         )
         return full_result(method_response, list[Message])
 
     async def send_location(
         self,
         chat_id: int | str,
         latitude: float,
         longitude: float,
-        message_thread_id: int | Option[int] = Nothing,
-        horizontal_accuracy: float | Option[float] = Nothing,
-        live_period: int | Option[int] = Nothing,
-        heading: int | Option[int] = Nothing,
-        proximity_alert_radius: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        horizontal_accuracy: float | None = None,
+        live_period: int | None = None,
+        heading: int | None = None,
+        proximity_alert_radius: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendLocation`, see the [documentation](https://core.telegram.org/bots/api#sendlocation)
 
         Use this method to send point on the map. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param latitude: Latitude of the location
+        :param latitude: Latitude of the location.
 
-        :param longitude: Longitude of the location
+        :param longitude: Longitude of the location.
 
-        :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500
+        :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500. \
 
-        :param live_period: Period in seconds for which the location will be updated (see Live Locations,
+        :param live_period: Period in seconds for which the location will be updated (see Live Locations, \
         should be between 60 and 86400.
 
-        :param heading: For live locations, a direction in which the user is moving, in degrees.
+        :param heading: For live locations, a direction in which the user is moving, in degrees. \
         Must be between 1 and 360 if specified.
 
-        :param proximity_alert_radius: For live locations, a maximum distance for proximity alerts about approaching
-        another chat member, in meters. Must be between 1 and 100000 if specified.
+        :param proximity_alert_radius: For live locations, a maximum distance for proximity alerts about approaching \
+        another chat member, in meters. Must be between 1 and 100000 if specified. \
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendLocation", get_params(locals())
+            "sendLocation",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def send_venue(
         self,
         chat_id: int | str,
         latitude: float,
         longitude: float,
         title: str,
         address: str,
-        message_thread_id: int | Option[int] = Nothing,
-        foursquare_id: str | Option[str] = Nothing,
-        foursquare_type: str | Option[str] = Nothing,
-        google_place_id: str | Option[str] = Nothing,
-        google_place_type: str | Option[str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        foursquare_id: str | None = None,
+        foursquare_type: str | None = None,
+        google_place_id: str | None = None,
+        google_place_type: str | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendVenue`, see the [documentation](https://core.telegram.org/bots/api#sendvenue)
 
-        Use this method to send information about a venue. On success, the sent Message is returned.
+        Use this method to send information about a venue. On success, the sent Message 
+        is returned.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param latitude: Latitude of the venue
+        :param latitude: Latitude of the venue.
 
-        :param longitude: Longitude of the venue
+        :param longitude: Longitude of the venue.
 
-        :param title: Name of the venue
+        :param title: Name of the venue.
 
-        :param address: Address of the venue
+        :param address: Address of the venue.
 
-        :param foursquare_id: Foursquare identifier of the venue
+        :param foursquare_id: Foursquare identifier of the venue.
 
-        :param foursquare_type: Foursquare type of the venue, if known. (For example, `arts_entertainment/default`,
-        `arts_entertainment/aquarium` or `food/icecream`.)
+        :param foursquare_type: Foursquare type of the venue, if known. (For example, `arts_entertainment/default`, \
+        `arts_entertainment/aquarium` or `food/icecream`.).
 
-        :param google_place_id: Google Places identifier of the venue
+        :param google_place_id: Google Places identifier of the venue.
 
-        :param google_place_type: Google Places type of the venue. (See supported types.)
+        :param google_place_type: Google Places type of the venue. (See supported types.).
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendVenue", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendVenue",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_contact(
         self,
         chat_id: int | str,
         phone_number: str,
         first_name: str,
-        message_thread_id: int | Option[int] = Nothing,
-        last_name: str | Option[str] = Nothing,
-        vcard: str | Option[str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        last_name: str | None = None,
+        vcard: str | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendContact`, see the [documentation](https://core.telegram.org/bots/api#sendcontact)
 
         Use this method to send phone contacts. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param phone_number: Contact's phone number
+        :param phone_number: Contact's phone number.
 
-        :param first_name: Contact's first name
+        :param first_name: Contact's first name.
 
-        :param last_name: Contact's last name
+        :param last_name: Contact's last name.
 
-        :param vcard: Additional data about the contact in the form of a vCard, 0-2048 bytes
+        :param vcard: Additional data about the contact in the form of a vCard, 0-2048 bytes.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendContact", get_params(locals())
+            "sendContact",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def send_poll(
         self,
         chat_id: int | str,
         question: str,
         options: list[str],
-        message_thread_id: int | Option[int] = Nothing,
-        is_anonymous: bool | Option[bool] = Nothing,
-        type: str | Option[str] = Nothing,
-        allows_multiple_answers: bool | Option[bool] = Nothing,
-        correct_option_id: int | Option[int] = Nothing,
-        explanation: str | Option[str] = Nothing,
-        explanation_parse_mode: str | Option[str] = Nothing,
-        explanation_entities: list[MessageEntity]
-        | Option[list[MessageEntity]] = Nothing,
-        open_period: int | Option[int] = Nothing,
-        close_date: int | Option[int] = Nothing,
-        is_closed: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        is_anonymous: bool | None = None,
+        type: typing.Literal["quiz", "regular"] | None = None,
+        allows_multiple_answers: bool | None = None,
+        correct_option_id: int | None = None,
+        explanation: str | None = None,
+        explanation_parse_mode: str | None = None,
+        explanation_entities: list[MessageEntity] | None = None,
+        open_period: int | None = None,
+        close_date: datetime | int | None = None,
+        is_closed: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendPoll`, see the [documentation](https://core.telegram.org/bots/api#sendpoll)
 
         Use this method to send a native poll. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param question: Poll question, 1-300 characters
+        :param question: Poll question, 1-300 characters.
 
-        :param options: A JSON-serialized list of answer options, 2-10 strings 1-100 characters
-        each
+        :param options: A JSON-serialized list of answer options, 2-10 strings 1-100 characters \
+        each.
 
-        :param is_anonymous: True, if the poll needs to be anonymous, defaults to True
+        :param is_anonymous: True, if the poll needs to be anonymous, defaults to True.
 
-        :param type: Poll type, `quiz` or `regular`, defaults to `regular`
+        :param type: Poll type, `quiz` or `regular`, defaults to `regular`.
 
-        :param allows_multiple_answers: True, if the poll allows multiple answers, ignored for polls in quiz mode,
-        defaults to False
+        :param allows_multiple_answers: True, if the poll allows multiple answers, ignored for polls in quiz mode, \
+        defaults to False.
 
-        :param correct_option_id: 0-based identifier of the correct answer option, required for polls in
-        quiz mode
+        :param correct_option_id: 0-based identifier of the correct answer option, required for polls in \
+        quiz mode.
 
-        :param explanation: Text that is shown when a user chooses an incorrect answer or taps on the lamp
-        icon in a quiz-style poll, 0-200 characters with at most 2 line feeds after
-        entities parsing
+        :param explanation: Text that is shown when a user chooses an incorrect answer or taps on the lamp \
+        icon in a quiz-style poll, 0-200 characters with at most 2 line feeds after \
+        entities parsing.
 
-        :param explanation_parse_mode: Mode for parsing entities in the explanation. See formatting options for
+        :param explanation_parse_mode: Mode for parsing entities in the explanation. See formatting options for \
         more details.
 
-        :param explanation_entities: A JSON-serialized list of special entities that appear in the poll explanation,
-        which can be specified instead of parse_mode
+        :param explanation_entities: A JSON-serialized list of special entities that appear in the poll explanation, \
+        which can be specified instead of parse_mode.
 
-        :param open_period: Amount of time in seconds the poll will be active after creation, 5-600.
+        :param open_period: Amount of time in seconds the poll will be active after creation, 5-600. \
         Can't be used together with close_date.
 
-        :param close_date: Point in time (Unix timestamp) when the poll will be automatically closed.
-        Must be at least 5 and no more than 600 seconds in the future. Can't be used
+        :param close_date: Point in time (Unix timestamp) when the poll will be automatically closed. \
+        Must be at least 5 and no more than 600 seconds in the future. Can't be used \
         together with open_period.
 
-        :param is_closed: Pass True if the poll needs to be immediately closed. This can be useful for
+        :param is_closed: Pass True if the poll needs to be immediately closed. This can be useful for \
         poll preview.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendPoll", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendPoll",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_dice(
         self,
         chat_id: int | str,
-        message_thread_id: int | Option[int] = Nothing,
-        emoji: str | Option[str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        emoji: DiceEmoji | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendDice`, see the [documentation](https://core.telegram.org/bots/api#senddice)
 
-        Use this method to send an animated emoji that will display a random value. On success, the sent Message is returned.
+        Use this method to send an animated emoji that will display a random value. 
+        On success, the sent Message is returned.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param emoji: Emoji on which the dice throw animation is based. Currently, must be one
-        of `🎲`, `🎯`, `🏀`, `⚽`, `🎳`, or `🎰`. Dice can have values 1-6 for `🎲`, `🎯` and
-        `🎳`, values 1-5 for `🏀` and `⚽`, and values 1-64 for `🎰`. Defaults to `🎲`
+        :param emoji: Emoji on which the dice throw animation is based. Currently, must be one \
+        of `🎲`, `🎯`, `🏀`, `⚽`, `🎳`, or `🎰`. Dice can have values 1-6 for `🎲`, `🎯` and \
+        `🎳`, values 1-5 for `🏀` and `⚽`, and values 1-64 for `🎰`. Defaults to `🎲`. \
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding
+        :param protect_content: Protects the contents of the sent message from forwarding.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove a reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendDice", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendDice",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def send_chat_action(
         self,
         chat_id: int | str,
-        action: str,
-        message_thread_id: int | Option[int] = Nothing,
+        action: ChatAction,
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `sendChatAction`, see the [documentation](https://core.telegram.org/bots/api#sendchataction)
 
-        Use this method when you need to tell the user that something is happening on the bot's side. The status is set for 5 seconds or less (when a message arrives from your bot, Telegram clients clear its typing status). Returns True on success.
-        We only recommend using this method when a response from the bot will take a noticeable amount of time to arrive.
-
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
-
-        :param message_thread_id: Unique identifier for the target message thread; supergroups only
-
-        :param action: Type of action to broadcast. Choose one, depending on what the user is about
-        to receive: typing for text messages, upload_photo for photos, record_video
-        or upload_video for videos, record_voice or upload_voice for voice notes,
-        upload_document for general files, choose_sticker for stickers, find_location
-        for location data, record_video_note or upload_video_note for video
-        notes."""
+        Use this method when you need to tell the user that something is happening 
+        on the bot's side. The status is set for 5 seconds or less (when a message arrives 
+        from your bot, Telegram clients clear its typing status). Returns True 
+        on success. We only recommend using this method when a response from the 
+        bot will take a noticeable amount of time to arrive.
+
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the action \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+
+        :param message_thread_id: Unique identifier for the target message thread; for supergroups only. \
+
+        :param action: Type of action to broadcast. Choose one, depending on what the user is about \
+        to receive: typing for text messages, upload_photo for photos, record_video \
+        or upload_video for videos, record_voice or upload_voice for voice notes, \
+        upload_document for general files, choose_sticker for stickers, find_location \
+        for location data, record_video_note or upload_video_note for video \
+        notes.
+        """
 
         method_response = await self.api.request_raw(
-            "sendChatAction", get_params(locals())
+            "sendChatAction",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_message_reaction(
         self,
         chat_id: int | str,
         message_id: int,
-        reaction: list[ReactionType] | Option[list[ReactionType]] = Nothing,
-        is_big: bool | Option[bool] = Nothing,
+        reaction: list[ReactionType] | None = None,
+        is_big: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMessageReaction`, see the [documentation](https://core.telegram.org/bots/api#setmessagereaction)
 
-        Use this method to change the chosen reactions on a message. Service messages can't be reacted to. Automatically forwarded messages from a channel to its discussion group have the same available reactions as messages in the channel. Returns True on success.
-
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
-
-        :param message_id: Identifier of the target message. If the message belongs to a media group,
-        the reaction is set to the first non-deleted message in the group instead.
-
-        :param reaction: New list of reaction types to set on the message. Currently, as non-premium
-        users, bots can set up to one reaction per message. A custom emoji reaction
-        can be used if it is either already present on the message or explicitly allowed
-        by chat administrators.
+        Use this method to change the chosen reactions on a message. Service messages 
+        can't be reacted to. Automatically forwarded messages from a channel to 
+        its discussion group have the same available reactions as messages in the 
+        channel. Returns True on success.
+
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+
+        :param message_id: Identifier of the target message. If the message belongs to a media group, \
+        the reaction is set to the first non-deleted message in the group instead. \
+
+        :param reaction: A JSON-serialized list of reaction types to set on the message. Currently, \
+        as non-premium users, bots can set up to one reaction per message. A custom \
+        emoji reaction can be used if it is either already present on the message \
+        or explicitly allowed by chat administrators.
 
-        :param is_big: Pass True to set the reaction with a big animation"""
+        :param is_big: Pass True to set the reaction with a big animation.
+        """
 
         method_response = await self.api.request_raw(
-            "setMessageReaction", get_params(locals())
+            "setMessageReaction",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_user_profile_photos(
         self,
         user_id: int,
-        offset: int | Option[int] = Nothing,
-        limit: int | Option[int] = Nothing,
+        offset: int | None = None,
+        limit: int | None = None,
         **other: typing.Any,
-    ) -> Result[UserProfilePhotos, "APIError"]:
+    ) -> Result[UserProfilePhotos, APIError]:
         """Method `getUserProfilePhotos`, see the [documentation](https://core.telegram.org/bots/api#getuserprofilephotos)
 
-        Use this method to get a list of profile pictures for a user. Returns a UserProfilePhotos object.
+        Use this method to get a list of profile pictures for a user. Returns a UserProfilePhotos 
+        object.
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param offset: Sequential number of the first photo to be returned. By default, all photos
+        :param offset: Sequential number of the first photo to be returned. By default, all photos \
         are returned.
 
-        :param limit: Limits the number of photos to be retrieved. Values between 1-100 are accepted.
-        Defaults to 100."""
+        :param limit: Limits the number of photos to be retrieved. Values between 1-100 are accepted. \
+        Defaults to 100.
+        """
 
         method_response = await self.api.request_raw(
-            "getUserProfilePhotos", get_params(locals())
+            "getUserProfilePhotos",
+            get_params(locals()),
         )
         return full_result(method_response, UserProfilePhotos)
 
     async def get_file(
         self,
         file_id: str,
         **other: typing.Any,
-    ) -> Result[File, "APIError"]:
+    ) -> Result[File, APIError]:
         """Method `getFile`, see the [documentation](https://core.telegram.org/bots/api#getfile)
 
-        Use this method to get basic information about a file and prepare it for downloading. For the moment, bots can download files of up to 20MB in size. On success, a File object is returned. The file can then be downloaded via the link https://api.telegram.org/file/bot<token>/<file_path>, where <file_path> is taken from the response. It is guaranteed that the link will be valid for at least 1 hour. When the link expires, a new one can be requested by calling getFile again.
-        Note: This function may not preserve the original file name and MIME type. You should save the file's MIME type and name (if available) when the File object is received.
+        Use this method to get basic information about a file and prepare it for downloading.
+        For the moment, bots can download files of up to 20MB in size. On success,
+        a File object is returned. The file can then be downloaded via the link https://api.telegram.org/file/bot<token>/<file_path>,
+        where <file_path> is taken from the response. It is guaranteed that the
+        link will be valid for at least 1 hour. When the link expires, a new one can
+        be requested by calling getFile again. Note: This function may not preserve
+        the original file name and MIME type. You should save the file's MIME type
+        and name (if available) when the File object is received.
 
-        :param file_id: File identifier to get information about"""
+        :param file_id: File identifier to get information about.
+        """
 
-        method_response = await self.api.request_raw("getFile", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "getFile",
+            get_params(locals()),
+        )
         return full_result(method_response, File)
 
     async def ban_chat_member(
         self,
         chat_id: int | str,
         user_id: int,
-        until_date: int | Option[int] = Nothing,
-        revoke_messages: bool | Option[bool] = Nothing,
+        until_date: datetime | int | None = None,
+        revoke_messages: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `banChatMember`, see the [documentation](https://core.telegram.org/bots/api#banchatmember)
 
-        Use this method to ban a user in a group, a supergroup or a channel. In the case of supergroups and channels, the user will not be able to return to the chat on their own using invite links, etc., unless unbanned first. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to ban a user in a group, a supergroup or a channel. In the case 
+        of supergroups and channels, the user will not be able to return to the chat 
+        on their own using invite links, etc., unless unbanned first. The bot must 
+        be an administrator in the chat for this to work and must have the appropriate 
+        administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target group or username of the target supergroup
-        or channel (in the format @channelusername)
+        :param chat_id: Unique identifier for the target group or username of the target supergroup \
+        or channel (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param until_date: Date when the user will be unbanned; Unix time. If user is banned for more
-        than 366 days or less than 30 seconds from the current time they are considered
+        :param until_date: Date when the user will be unbanned; Unix time. If user is banned for more \
+        than 366 days or less than 30 seconds from the current time they are considered \
         to be banned forever. Applied for supergroups and channels only.
 
-        :param revoke_messages: Pass True to delete all messages from the chat for the user that is being removed.
-        If False, the user will be able to see messages in the group that were sent
-        before the user was removed. Always True for supergroups and channels."""
+        :param revoke_messages: Pass True to delete all messages from the chat for the user that is being removed. \
+        If False, the user will be able to see messages in the group that were sent \
+        before the user was removed. Always True for supergroups and channels. \
+        """
 
         method_response = await self.api.request_raw(
-            "banChatMember", get_params(locals())
+            "banChatMember",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unban_chat_member(
         self,
         chat_id: int | str,
         user_id: int,
-        only_if_banned: bool | Option[bool] = Nothing,
+        only_if_banned: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unbanChatMember`, see the [documentation](https://core.telegram.org/bots/api#unbanchatmember)
 
-        Use this method to unban a previously banned user in a supergroup or channel. The user will not return to the group or channel automatically, but will be able to join via link, etc. The bot must be an administrator for this to work. By default, this method guarantees that after the call the user is not a member of the chat, but will be able to join it. So if the user is a member of the chat they will also be removed from the chat. If you don't want this, use the parameter only_if_banned. Returns True on success.
+        Use this method to unban a previously banned user in a supergroup or channel. 
+        The user will not return to the group or channel automatically, but will 
+        be able to join via link, etc. The bot must be an administrator for this to 
+        work. By default, this method guarantees that after the call the user is 
+        not a member of the chat, but will be able to join it. So if the user is a member 
+        of the chat they will also be removed from the chat. If you don't want this, 
+        use the parameter only_if_banned. Returns True on success.
 
-        :param chat_id: Unique identifier for the target group or username of the target supergroup
-        or channel (in the format @channelusername)
+        :param chat_id: Unique identifier for the target group or username of the target supergroup \
+        or channel (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param only_if_banned: Do nothing if the user is not banned"""
+        :param only_if_banned: Do nothing if the user is not banned.
+        """
 
         method_response = await self.api.request_raw(
-            "unbanChatMember", get_params(locals())
+            "unbanChatMember",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def restrict_chat_member(
         self,
         chat_id: int | str,
         user_id: int,
         permissions: ChatPermissions,
-        use_independent_chat_permissions: bool | Option[bool] = Nothing,
-        until_date: int | Option[int] = Nothing,
+        use_independent_chat_permissions: bool | None = None,
+        until_date: datetime | int | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `restrictChatMember`, see the [documentation](https://core.telegram.org/bots/api#restrictchatmember)
 
-        Use this method to restrict a user in a supergroup. The bot must be an administrator in the supergroup for this to work and must have the appropriate administrator rights. Pass True for all permissions to lift restrictions from a user. Returns True on success.
+        Use this method to restrict a user in a supergroup. The bot must be an administrator 
+        in the supergroup for this to work and must have the appropriate administrator 
+        rights. Pass True for all permissions to lift restrictions from a user. 
+        Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param permissions: A JSON-serialized object for new user permissions
+        :param permissions: A JSON-serialized object for new user permissions.
 
-        :param use_independent_chat_permissions: Pass True if chat permissions are set independently. Otherwise, the can_send_other_messages
-        and can_add_web_page_previews permissions will imply the can_send_messages,
-        can_send_audios, can_send_documents, can_send_photos, can_send_videos,
-        can_send_video_notes, and can_send_voice_notes permissions; the can_send_polls
+        :param use_independent_chat_permissions: Pass True if chat permissions are set independently. Otherwise, the can_send_other_messages \
+        and can_add_web_page_previews permissions will imply the can_send_messages, \
+        can_send_audios, can_send_documents, can_send_photos, can_send_videos, \
+        can_send_video_notes, and can_send_voice_notes permissions; the can_send_polls \
         permission will imply the can_send_messages permission.
 
-        :param until_date: Date when restrictions will be lifted for the user; Unix time. If user is
-        restricted for more than 366 days or less than 30 seconds from the current
-        time, they are considered to be restricted forever"""
+        :param until_date: Date when restrictions will be lifted for the user; Unix time. If user is \
+        restricted for more than 366 days or less than 30 seconds from the current \
+        time, they are considered to be restricted forever.
+        """
 
         method_response = await self.api.request_raw(
-            "restrictChatMember", get_params(locals())
+            "restrictChatMember",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def promote_chat_member(
         self,
         chat_id: int | str,
         user_id: int,
-        is_anonymous: bool | Option[bool] = Nothing,
-        can_manage_chat: bool | Option[bool] = Nothing,
-        can_delete_messages: bool | Option[bool] = Nothing,
-        can_manage_video_chats: bool | Option[bool] = Nothing,
-        can_restrict_members: bool | Option[bool] = Nothing,
-        can_promote_members: bool | Option[bool] = Nothing,
-        can_change_info: bool | Option[bool] = Nothing,
-        can_invite_users: bool | Option[bool] = Nothing,
-        can_post_messages: bool | Option[bool] = Nothing,
-        can_edit_messages: bool | Option[bool] = Nothing,
-        can_pin_messages: bool | Option[bool] = Nothing,
-        can_post_stories: bool | Option[bool] = Nothing,
-        can_edit_stories: bool | Option[bool] = Nothing,
-        can_delete_stories: bool | Option[bool] = Nothing,
-        can_manage_topics: bool | Option[bool] = Nothing,
+        is_anonymous: bool | None = None,
+        can_manage_chat: bool | None = None,
+        can_delete_messages: bool | None = None,
+        can_manage_video_chats: bool | None = None,
+        can_restrict_members: bool | None = None,
+        can_promote_members: bool | None = None,
+        can_change_info: bool | None = None,
+        can_invite_users: bool | None = None,
+        can_post_stories: bool | None = None,
+        can_edit_stories: bool | None = None,
+        can_delete_stories: bool | None = None,
+        can_post_messages: bool | None = None,
+        can_edit_messages: bool | None = None,
+        can_pin_messages: bool | None = None,
+        can_manage_topics: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `promoteChatMember`, see the [documentation](https://core.telegram.org/bots/api#promotechatmember)
 
-        Use this method to promote or demote a user in a supergroup or a channel. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Pass False for all boolean parameters to demote a user. Returns True on success.
+        Use this method to promote or demote a user in a supergroup or a channel. The 
+        bot must be an administrator in the chat for this to work and must have the 
+        appropriate administrator rights. Pass False for all boolean parameters 
+        to demote a user. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param is_anonymous: Pass True if the administrator's presence in the chat is hidden
+        :param is_anonymous: Pass True if the administrator's presence in the chat is hidden.
 
-        :param can_manage_chat: Pass True if the administrator can access the chat event log, boost list
-        in channels, see channel members, report spam messages, see anonymous
-        administrators in supergroups and ignore slow mode. Implied by any other
-        administrator privilege
+        :param can_manage_chat: Pass True if the administrator can access the chat event log, get boost list, \
+        see hidden supergroup and channel members, report spam messages and ignore \
+        slow mode. Implied by any other administrator privilege.
 
-        :param can_delete_messages: Pass True if the administrator can delete messages of other users
+        :param can_delete_messages: Pass True if the administrator can delete messages of other users.
 
-        :param can_manage_video_chats: Pass True if the administrator can manage video chats
+        :param can_manage_video_chats: Pass True if the administrator can manage video chats.
 
-        :param can_restrict_members: Pass True if the administrator can restrict, ban or unban chat members,
-        or access supergroup statistics
+        :param can_restrict_members: Pass True if the administrator can restrict, ban or unban chat members, \
+        or access supergroup statistics.
 
-        :param can_promote_members: Pass True if the administrator can add new administrators with a subset
-        of their own privileges or demote administrators that they have promoted,
-        directly or indirectly (promoted by administrators that were appointed
-        by him)
+        :param can_promote_members: Pass True if the administrator can add new administrators with a subset \
+        of their own privileges or demote administrators that they have promoted, \
+        directly or indirectly (promoted by administrators that were appointed \
+        by him).
 
-        :param can_change_info: Pass True if the administrator can change chat title, photo and other settings
+        :param can_change_info: Pass True if the administrator can change chat title, photo and other settings. \
 
-        :param can_invite_users: Pass True if the administrator can invite new users to the chat
+        :param can_invite_users: Pass True if the administrator can invite new users to the chat.
 
-        :param can_post_messages: Pass True if the administrator can post messages in the channel, or access
-        channel statistics; channels only
+        :param can_post_stories: Pass True if the administrator can post stories to the chat.
 
-        :param can_edit_messages: Pass True if the administrator can edit messages of other users and can pin
-        messages; channels only
+        :param can_edit_stories: Pass True if the administrator can edit stories posted by other users.
 
-        :param can_pin_messages: Pass True if the administrator can pin messages, supergroups only
+        :param can_delete_stories: Pass True if the administrator can delete stories posted by other users. \
 
-        :param can_post_stories: Pass True if the administrator can post stories in the channel; channels
-        only
+        :param can_post_messages: Pass True if the administrator can post messages in the channel, or access \
+        channel statistics; for channels only.
 
-        :param can_edit_stories: Pass True if the administrator can edit stories posted by other users; channels
-        only
+        :param can_edit_messages: Pass True if the administrator can edit messages of other users and can pin \
+        messages; for channels only.
 
-        :param can_delete_stories: Pass True if the administrator can delete stories posted by other users;
-        channels only
+        :param can_pin_messages: Pass True if the administrator can pin messages; for supergroups only. \
 
-        :param can_manage_topics: Pass True if the user is allowed to create, rename, close, and reopen forum
-        topics, supergroups only"""
+        :param can_manage_topics: Pass True if the user is allowed to create, rename, close, and reopen forum \
+        topics; for supergroups only.
+        """
 
         method_response = await self.api.request_raw(
-            "promoteChatMember", get_params(locals())
+            "promoteChatMember",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_chat_administrator_custom_title(
         self,
         chat_id: int | str,
         user_id: int,
         custom_title: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatAdministratorCustomTitle`, see the [documentation](https://core.telegram.org/bots/api#setchatadministratorcustomtitle)
 
-        Use this method to set a custom title for an administrator in a supergroup promoted by the bot. Returns True on success.
+        Use this method to set a custom title for an administrator in a supergroup 
+        promoted by the bot. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param user_id: Unique identifier of the target user
+        :param user_id: Unique identifier of the target user.
 
-        :param custom_title: New custom title for the administrator; 0-16 characters, emoji are not
-        allowed"""
+        :param custom_title: New custom title for the administrator; 0-16 characters, emoji are not \
+        allowed.
+        """
 
         method_response = await self.api.request_raw(
-            "setChatAdministratorCustomTitle", get_params(locals())
+            "setChatAdministratorCustomTitle",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def ban_chat_sender_chat(
         self,
         chat_id: int | str,
         sender_chat_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `banChatSenderChat`, see the [documentation](https://core.telegram.org/bots/api#banchatsenderchat)
 
-        Use this method to ban a channel chat in a supergroup or a channel. Until the chat is unbanned, the owner of the banned chat won't be able to send messages on behalf of any of their channels. The bot must be an administrator in the supergroup or channel for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to ban a channel chat in a supergroup or a channel. Until the 
+        chat is unbanned, the owner of the banned chat won't be able to send messages 
+        on behalf of any of their channels. The bot must be an administrator in the 
+        supergroup or channel for this to work and must have the appropriate administrator 
+        rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param sender_chat_id: Unique identifier of the target sender chat"""
+        :param sender_chat_id: Unique identifier of the target sender chat.
+        """
 
         method_response = await self.api.request_raw(
-            "banChatSenderChat", get_params(locals())
+            "banChatSenderChat",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unban_chat_sender_chat(
         self,
         chat_id: int | str,
         sender_chat_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unbanChatSenderChat`, see the [documentation](https://core.telegram.org/bots/api#unbanchatsenderchat)
 
-        Use this method to unban a previously banned channel chat in a supergroup or channel. The bot must be an administrator for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to unban a previously banned channel chat in a supergroup 
+        or channel. The bot must be an administrator for this to work and must have 
+        the appropriate administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param sender_chat_id: Unique identifier of the target sender chat"""
+        :param sender_chat_id: Unique identifier of the target sender chat.
+        """
 
         method_response = await self.api.request_raw(
-            "unbanChatSenderChat", get_params(locals())
+            "unbanChatSenderChat",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_chat_permissions(
         self,
         chat_id: int | str,
         permissions: ChatPermissions,
-        use_independent_chat_permissions: bool | Option[bool] = Nothing,
+        use_independent_chat_permissions: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatPermissions`, see the [documentation](https://core.telegram.org/bots/api#setchatpermissions)
 
-        Use this method to set default chat permissions for all members. The bot must be an administrator in the group or a supergroup for this to work and must have the can_restrict_members administrator rights. Returns True on success.
-
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
-
-        :param permissions: A JSON-serialized object for new default chat permissions
-
-        :param use_independent_chat_permissions: Pass True if chat permissions are set independently. Otherwise, the can_send_other_messages
-        and can_add_web_page_previews permissions will imply the can_send_messages,
-        can_send_audios, can_send_documents, can_send_photos, can_send_videos,
-        can_send_video_notes, and can_send_voice_notes permissions; the can_send_polls
-        permission will imply the can_send_messages permission."""
+        Use this method to set default chat permissions for all members. The bot 
+        must be an administrator in the group or a supergroup for this to work and 
+        must have the can_restrict_members administrator rights. Returns True 
+        on success.
+
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+
+        :param permissions: A JSON-serialized object for new default chat permissions.
+
+        :param use_independent_chat_permissions: Pass True if chat permissions are set independently. Otherwise, the can_send_other_messages \
+        and can_add_web_page_previews permissions will imply the can_send_messages, \
+        can_send_audios, can_send_documents, can_send_photos, can_send_videos, \
+        can_send_video_notes, and can_send_voice_notes permissions; the can_send_polls \
+        permission will imply the can_send_messages permission.
+        """
 
         method_response = await self.api.request_raw(
-            "setChatPermissions", get_params(locals())
+            "setChatPermissions",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def export_chat_invite_link(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[str, "APIError"]:
+    ) -> Result[str, APIError]:
         """Method `exportChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#exportchatinvitelink)
 
-        Use this method to generate a new primary invite link for a chat; any previously generated primary link is revoked. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns the new invite link as String on success.
+        Use this method to generate a new primary invite link for a chat; any previously 
+        generated primary link is revoked. The bot must be an administrator in the 
+        chat for this to work and must have the appropriate administrator rights. 
+        Returns the new invite link as String on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+        """
 
         method_response = await self.api.request_raw(
-            "exportChatInviteLink", get_params(locals())
+            "exportChatInviteLink",
+            get_params(locals()),
         )
         return full_result(method_response, str)
 
     async def create_chat_invite_link(
         self,
         chat_id: int | str,
-        name: str | Option[str] = Nothing,
-        expire_date: int | Option[int] = Nothing,
-        member_limit: int | Option[int] = Nothing,
-        creates_join_request: bool | Option[bool] = Nothing,
+        name: str | None = None,
+        expire_date: datetime | int | None = None,
+        member_limit: int | None = None,
+        creates_join_request: bool | None = None,
         **other: typing.Any,
-    ) -> Result[ChatInviteLink, "APIError"]:
+    ) -> Result[ChatInviteLink, APIError]:
         """Method `createChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#createchatinvitelink)
 
-        Use this method to create an additional invite link for a chat. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. The link can be revoked using the method revokeChatInviteLink. Returns the new invite link as ChatInviteLink object.
+        Use this method to create an additional invite link for a chat. The bot must 
+        be an administrator in the chat for this to work and must have the appropriate 
+        administrator rights. The link can be revoked using the method revokeChatInviteLink. 
+        Returns the new invite link as ChatInviteLink object.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param name: Invite link name; 0-32 characters
+        :param name: Invite link name; 0-32 characters.
 
-        :param expire_date: Point in time (Unix timestamp) when the link will expire
+        :param expire_date: Point in time (Unix timestamp) when the link will expire.
 
-        :param member_limit: The maximum number of users that can be members of the chat simultaneously
-        after joining the chat via this invite link; 1-99999
+        :param member_limit: The maximum number of users that can be members of the chat simultaneously \
+        after joining the chat via this invite link; 1-99999.
 
-        :param creates_join_request: True, if users joining the chat via the link need to be approved by chat administrators.
-        If True, member_limit can't be specified"""
+        :param creates_join_request: True, if users joining the chat via the link need to be approved by chat administrators. \
+        If True, member_limit can't be specified.
+        """
 
         method_response = await self.api.request_raw(
-            "createChatInviteLink", get_params(locals())
+            "createChatInviteLink",
+            get_params(locals()),
         )
         return full_result(method_response, ChatInviteLink)
 
     async def edit_chat_invite_link(
         self,
         chat_id: int | str,
         invite_link: str,
-        name: str | Option[str] = Nothing,
-        expire_date: int | Option[int] = Nothing,
-        member_limit: int | Option[int] = Nothing,
-        creates_join_request: bool | Option[bool] = Nothing,
+        name: str | None = None,
+        expire_date: datetime | int | None = None,
+        member_limit: int | None = None,
+        creates_join_request: bool | None = None,
         **other: typing.Any,
-    ) -> Result[ChatInviteLink, "APIError"]:
+    ) -> Result[ChatInviteLink, APIError]:
         """Method `editChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#editchatinvitelink)
 
-        Use this method to edit a non-primary invite link created by the bot. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns the edited invite link as a ChatInviteLink object.
+        Use this method to edit a non-primary invite link created by the bot. The 
+        bot must be an administrator in the chat for this to work and must have the 
+        appropriate administrator rights. Returns the edited invite link as a 
+        ChatInviteLink object.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param invite_link: The invite link to edit
+        :param invite_link: The invite link to edit.
 
-        :param name: Invite link name; 0-32 characters
+        :param name: Invite link name; 0-32 characters.
 
-        :param expire_date: Point in time (Unix timestamp) when the link will expire
+        :param expire_date: Point in time (Unix timestamp) when the link will expire.
 
-        :param member_limit: The maximum number of users that can be members of the chat simultaneously
-        after joining the chat via this invite link; 1-99999
+        :param member_limit: The maximum number of users that can be members of the chat simultaneously \
+        after joining the chat via this invite link; 1-99999.
 
-        :param creates_join_request: True, if users joining the chat via the link need to be approved by chat administrators.
-        If True, member_limit can't be specified"""
+        :param creates_join_request: True, if users joining the chat via the link need to be approved by chat administrators. \
+        If True, member_limit can't be specified.
+        """
 
         method_response = await self.api.request_raw(
-            "editChatInviteLink", get_params(locals())
+            "editChatInviteLink",
+            get_params(locals()),
         )
         return full_result(method_response, ChatInviteLink)
 
     async def revoke_chat_invite_link(
         self,
         chat_id: int | str,
         invite_link: str,
         **other: typing.Any,
-    ) -> Result[ChatInviteLink, "APIError"]:
+    ) -> Result[ChatInviteLink, APIError]:
         """Method `revokeChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#revokechatinvitelink)
 
-        Use this method to revoke an invite link created by the bot. If the primary link is revoked, a new link is automatically generated. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns the revoked invite link as ChatInviteLink object.
+        Use this method to revoke an invite link created by the bot. If the primary 
+        link is revoked, a new link is automatically generated. The bot must be an 
+        administrator in the chat for this to work and must have the appropriate 
+        administrator rights. Returns the revoked invite link as ChatInviteLink 
+        object.
 
-        :param chat_id: Unique identifier of the target chat or username of the target channel (in
-        the format @channelusername)
+        :param chat_id: Unique identifier of the target chat or username of the target channel (in \
+        the format @channelusername).
 
-        :param invite_link: The invite link to revoke"""
+        :param invite_link: The invite link to revoke.
+        """
 
         method_response = await self.api.request_raw(
-            "revokeChatInviteLink", get_params(locals())
+            "revokeChatInviteLink",
+            get_params(locals()),
         )
         return full_result(method_response, ChatInviteLink)
 
     async def approve_chat_join_request(
         self,
         chat_id: int | str,
         user_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `approveChatJoinRequest`, see the [documentation](https://core.telegram.org/bots/api#approvechatjoinrequest)
 
-        Use this method to approve a chat join request. The bot must be an administrator in the chat for this to work and must have the can_invite_users administrator right. Returns True on success.
+        Use this method to approve a chat join request. The bot must be an administrator 
+        in the chat for this to work and must have the can_invite_users administrator 
+        right. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user"""
+        :param user_id: Unique identifier of the target user.
+        """
 
         method_response = await self.api.request_raw(
-            "approveChatJoinRequest", get_params(locals())
+            "approveChatJoinRequest",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def decline_chat_join_request(
         self,
         chat_id: int | str,
         user_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `declineChatJoinRequest`, see the [documentation](https://core.telegram.org/bots/api#declinechatjoinrequest)
 
-        Use this method to decline a chat join request. The bot must be an administrator in the chat for this to work and must have the can_invite_users administrator right. Returns True on success.
+        Use this method to decline a chat join request. The bot must be an administrator 
+        in the chat for this to work and must have the can_invite_users administrator 
+        right. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user"""
+        :param user_id: Unique identifier of the target user.
+        """
 
         method_response = await self.api.request_raw(
-            "declineChatJoinRequest", get_params(locals())
+            "declineChatJoinRequest",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_chat_photo(
         self,
         chat_id: int | str,
         photo: InputFile,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatPhoto`, see the [documentation](https://core.telegram.org/bots/api#setchatphoto)
 
-        Use this method to set a new profile photo for the chat. Photos can't be changed for private chats. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to set a new profile photo for the chat. Photos can't be changed 
+        for private chats. The bot must be an administrator in the chat for this to 
+        work and must have the appropriate administrator rights. Returns True 
+        on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param photo: New chat photo, uploaded using multipart/form-data"""
+        :param photo: New chat photo, uploaded using multipart/form-data.
+        """
 
         method_response = await self.api.request_raw(
-            "setChatPhoto", get_params(locals())
+            "setChatPhoto",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_chat_photo(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteChatPhoto`, see the [documentation](https://core.telegram.org/bots/api#deletechatphoto)
 
-        Use this method to delete a chat photo. Photos can't be changed for private chats. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to delete a chat photo. Photos can't be changed for private 
+        chats. The bot must be an administrator in the chat for this to work and must 
+        have the appropriate administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+        """
 
         method_response = await self.api.request_raw(
-            "deleteChatPhoto", get_params(locals())
+            "deleteChatPhoto",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_chat_title(
         self,
         chat_id: int | str,
         title: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatTitle`, see the [documentation](https://core.telegram.org/bots/api#setchattitle)
 
-        Use this method to change the title of a chat. Titles can't be changed for private chats. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to change the title of a chat. Titles can't be changed for 
+        private chats. The bot must be an administrator in the chat for this to work 
+        and must have the appropriate administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param title: New chat title, 1-128 characters"""
+        :param title: New chat title, 1-128 characters.
+        """
 
         method_response = await self.api.request_raw(
-            "setChatTitle", get_params(locals())
+            "setChatTitle",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_chat_description(
         self,
         chat_id: int | str,
-        description: str | Option[str] = Nothing,
+        description: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatDescription`, see the [documentation](https://core.telegram.org/bots/api#setchatdescription)
 
-        Use this method to change the description of a group, a supergroup or a channel. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Returns True on success.
+        Use this method to change the description of a group, a supergroup or a channel. 
+        The bot must be an administrator in the chat for this to work and must have 
+        the appropriate administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param description: New chat description, 0-255 characters"""
+        :param description: New chat description, 0-255 characters.
+        """
 
         method_response = await self.api.request_raw(
-            "setChatDescription", get_params(locals())
+            "setChatDescription",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def pin_chat_message(
         self,
         chat_id: int | str,
         message_id: int,
-        disable_notification: bool | Option[bool] = Nothing,
+        disable_notification: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `pinChatMessage`, see the [documentation](https://core.telegram.org/bots/api#pinchatmessage)
 
-        Use this method to add a message to the list of pinned messages in a chat. If the chat is not a private chat, the bot must be an administrator in the chat for this to work and must have the 'can_pin_messages' administrator right in a supergroup or 'can_edit_messages' administrator right in a channel. Returns True on success.
+        Use this method to add a message to the list of pinned messages in a chat. If 
+        the chat is not a private chat, the bot must be an administrator in the chat 
+        for this to work and must have the 'can_pin_messages' administrator right 
+        in a supergroup or 'can_edit_messages' administrator right in a channel. 
+        Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_id: Identifier of a message to pin
+        :param message_id: Identifier of a message to pin.
 
-        :param disable_notification: Pass True if it is not necessary to send a notification to all chat members
-        about the new pinned message. Notifications are always disabled in channels
-        and private chats."""
+        :param disable_notification: Pass True if it is not necessary to send a notification to all chat members \
+        about the new pinned message. Notifications are always disabled in channels \
+        and private chats.
+        """
 
         method_response = await self.api.request_raw(
-            "pinChatMessage", get_params(locals())
+            "pinChatMessage",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unpin_chat_message(
         self,
         chat_id: int | str,
-        message_id: int | Option[int] = Nothing,
+        message_id: int | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unpinChatMessage`, see the [documentation](https://core.telegram.org/bots/api#unpinchatmessage)
 
-        Use this method to remove a message from the list of pinned messages in a chat. If the chat is not a private chat, the bot must be an administrator in the chat for this to work and must have the 'can_pin_messages' administrator right in a supergroup or 'can_edit_messages' administrator right in a channel. Returns True on success.
+        Use this method to remove a message from the list of pinned messages in a chat. 
+        If the chat is not a private chat, the bot must be an administrator in the chat 
+        for this to work and must have the 'can_pin_messages' administrator right 
+        in a supergroup or 'can_edit_messages' administrator right in a channel. 
+        Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_id: Identifier of a message to unpin. If not specified, the most recent pinned
-        message (by sending date) will be unpinned."""
+        :param message_id: Identifier of a message to unpin. If not specified, the most recent pinned \
+        message (by sending date) will be unpinned.
+        """
 
         method_response = await self.api.request_raw(
-            "unpinChatMessage", get_params(locals())
+            "unpinChatMessage",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unpin_all_chat_messages(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unpinAllChatMessages`, see the [documentation](https://core.telegram.org/bots/api#unpinallchatmessages)
 
-        Use this method to clear the list of pinned messages in a chat. If the chat is not a private chat, the bot must be an administrator in the chat for this to work and must have the 'can_pin_messages' administrator right in a supergroup or 'can_edit_messages' administrator right in a channel. Returns True on success.
+        Use this method to clear the list of pinned messages in a chat. If the chat 
+        is not a private chat, the bot must be an administrator in the chat for this 
+        to work and must have the 'can_pin_messages' administrator right in a supergroup 
+        or 'can_edit_messages' administrator right in a channel. Returns True 
+        on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
+        """
 
         method_response = await self.api.request_raw(
-            "unpinAllChatMessages", get_params(locals())
+            "unpinAllChatMessages",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def leave_chat(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `leaveChat`, see the [documentation](https://core.telegram.org/bots/api#leavechat)
 
-        Use this method for your bot to leave a group, supergroup or channel. Returns True on success.
+        Use this method for your bot to leave a group, supergroup or channel. Returns 
+        True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        or channel (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        or channel (in the format @channelusername).
+        """
 
-        method_response = await self.api.request_raw("leaveChat", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "leaveChat",
+            get_params(locals()),
+        )
         return full_result(method_response, bool)
 
     async def get_chat(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[Chat, "APIError"]:
+    ) -> Result[Chat, APIError]:
         """Method `getChat`, see the [documentation](https://core.telegram.org/bots/api#getchat)
 
-        Use this method to get up to date information about the chat. Returns a Chat object on success.
+        Use this method to get up to date information about the chat. Returns a Chat 
+        object on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        or channel (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        or channel (in the format @channelusername).
+        """
 
-        method_response = await self.api.request_raw("getChat", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "getChat",
+            get_params(locals()),
+        )
         return full_result(method_response, Chat)
 
     async def get_chat_administrators(
         self,
         chat_id: int | str,
         **other: typing.Any,
     ) -> Result[
         list[
-            ChatMemberOwner
-            | ChatMemberAdministrator
-            | ChatMemberMember
-            | ChatMemberRestricted
-            | ChatMemberLeft
-            | ChatMemberBanned
+            Variative[
+                ChatMemberOwner,
+                ChatMemberAdministrator,
+                ChatMemberMember,
+                ChatMemberRestricted,
+                ChatMemberLeft,
+                ChatMemberBanned,
+            ]
         ],
-        "APIError",
+        APIError,
     ]:
         """Method `getChatAdministrators`, see the [documentation](https://core.telegram.org/bots/api#getchatadministrators)
 
-        Use this method to get a list of administrators in a chat, which aren't bots. Returns an Array of ChatMember objects.
+        Use this method to get a list of administrators in a chat, which aren't bots. 
+        Returns an Array of ChatMember objects.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        or channel (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        or channel (in the format @channelusername).
+        """
 
         method_response = await self.api.request_raw(
-            "getChatAdministrators", get_params(locals())
+            "getChatAdministrators",
+            get_params(locals()),
         )
         return full_result(
             method_response,
             list[
-                ChatMemberOwner
-                | ChatMemberAdministrator
-                | ChatMemberMember
-                | ChatMemberRestricted
-                | ChatMemberLeft
-                | ChatMemberBanned
+                Variative[
+                    ChatMemberOwner,
+                    ChatMemberAdministrator,
+                    ChatMemberMember,
+                    ChatMemberRestricted,
+                    ChatMemberLeft,
+                    ChatMemberBanned,
+                ]
             ],
         )
 
     async def get_chat_member_count(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[int, "APIError"]:
+    ) -> Result[int, APIError]:
         """Method `getChatMemberCount`, see the [documentation](https://core.telegram.org/bots/api#getchatmembercount)
 
         Use this method to get the number of members in a chat. Returns Int on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        or channel (in the format @channelusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        or channel (in the format @channelusername).
+        """
 
         method_response = await self.api.request_raw(
-            "getChatMemberCount", get_params(locals())
+            "getChatMemberCount",
+            get_params(locals()),
         )
         return full_result(method_response, int)
 
     async def get_chat_member(
         self,
         chat_id: int | str,
         user_id: int,
         **other: typing.Any,
     ) -> Result[
-        ChatMemberOwner
-        | ChatMemberAdministrator
-        | ChatMemberMember
-        | ChatMemberRestricted
-        | ChatMemberLeft
-        | ChatMemberBanned,
-        "APIError",
+        Variative[
+            ChatMemberOwner,
+            ChatMemberAdministrator,
+            ChatMemberMember,
+            ChatMemberRestricted,
+            ChatMemberLeft,
+            ChatMemberBanned,
+        ],
+        APIError,
     ]:
         """Method `getChatMember`, see the [documentation](https://core.telegram.org/bots/api#getchatmember)
 
-        Use this method to get information about a member of a chat. The method is only guaranteed to work for other users if the bot is an administrator in the chat. Returns a ChatMember object on success.
+        Use this method to get information about a member of a chat. The method is 
+        only guaranteed to work for other users if the bot is an administrator in 
+        the chat. Returns a ChatMember object on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        or channel (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        or channel (in the format @channelusername).
 
-        :param user_id: Unique identifier of the target user"""
+        :param user_id: Unique identifier of the target user.
+        """
 
         method_response = await self.api.request_raw(
-            "getChatMember", get_params(locals())
+            "getChatMember",
+            get_params(locals()),
         )
         return full_result(
             method_response,
-            ChatMemberOwner
-            | ChatMemberAdministrator
-            | ChatMemberMember
-            | ChatMemberRestricted
-            | ChatMemberLeft
-            | ChatMemberBanned,
+            Variative[
+                ChatMemberOwner,
+                ChatMemberAdministrator,
+                ChatMemberMember,
+                ChatMemberRestricted,
+                ChatMemberLeft,
+                ChatMemberBanned,
+            ],
         )
 
     async def set_chat_sticker_set(
         self,
         chat_id: int | str,
         sticker_set_name: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatStickerSet`, see the [documentation](https://core.telegram.org/bots/api#setchatstickerset)
 
-        Use this method to set a new group sticker set for a supergroup. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Use the field can_set_sticker_set optionally returned in getChat requests to check if the bot can use this method. Returns True on success.
+        Use this method to set a new group sticker set for a supergroup. The bot must 
+        be an administrator in the chat for this to work and must have the appropriate 
+        administrator rights. Use the field can_set_sticker_set optionally 
+        returned in getChat requests to check if the bot can use this method. Returns 
+        True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param sticker_set_name: Name of the sticker set to be set as the group sticker set
+        :param sticker_set_name: Name of the sticker set to be set as the group sticker set.
         """
 
         method_response = await self.api.request_raw(
-            "setChatStickerSet", get_params(locals())
+            "setChatStickerSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_chat_sticker_set(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteChatStickerSet`, see the [documentation](https://core.telegram.org/bots/api#deletechatstickerset)
 
-        Use this method to delete a group sticker set from a supergroup. The bot must be an administrator in the chat for this to work and must have the appropriate administrator rights. Use the field can_set_sticker_set optionally returned in getChat requests to check if the bot can use this method. Returns True on success.
+        Use this method to delete a group sticker set from a supergroup. The bot must 
+        be an administrator in the chat for this to work and must have the appropriate 
+        administrator rights. Use the field can_set_sticker_set optionally 
+        returned in getChat requests to check if the bot can use this method. Returns 
+        True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "deleteChatStickerSet", get_params(locals())
+            "deleteChatStickerSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_forum_topic_icon_stickers(
-        self,
-        **other: typing.Any,
-    ) -> Result[list[Sticker], "APIError"]:
+        self, **other: typing.Any
+    ) -> Result[list[Sticker], APIError]:
         """Method `getForumTopicIconStickers`, see the [documentation](https://core.telegram.org/bots/api#getforumtopiciconstickers)
 
-        Use this method to get custom emoji stickers, which can be used as a forum topic icon by any user. Requires no parameters. Returns an Array of Sticker objects.
+        Use this method to get custom emoji stickers, which can be used as a forum
+        topic icon by any user. Requires no parameters. Returns an Array of Sticker
+        objects.
         """
 
         method_response = await self.api.request_raw(
-            "getForumTopicIconStickers", get_params(locals())
+            "getForumTopicIconStickers",
+            get_params(locals()),
         )
         return full_result(method_response, list[Sticker])
 
     async def create_forum_topic(
         self,
         chat_id: int | str,
         name: str,
-        icon_color: int | Option[int] = Nothing,
-        icon_custom_emoji_id: str | Option[str] = Nothing,
+        icon_color: TopicIconColor | None = None,
+        icon_custom_emoji_id: str | None = None,
         **other: typing.Any,
-    ) -> Result[ForumTopic, "APIError"]:
+    ) -> Result[ForumTopic, APIError]:
         """Method `createForumTopic`, see the [documentation](https://core.telegram.org/bots/api#createforumtopic)
 
-        Use this method to create a topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights. Returns information about the created topic as a ForumTopic object.
-
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        Use this method to create a topic in a forum supergroup chat. The bot must 
+        be an administrator in the chat for this to work and must have the can_manage_topics 
+        administrator rights. Returns information about the created topic as 
+        a ForumTopic object.
+
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+
+        :param name: Topic name, 1-128 characters.
+
+        :param icon_color: Color of the topic icon in RGB format. Currently, must be one of 7322096 (0x6FB9F0), \
+        16766590 (0xFFD67E), 13338331 (0xCB86DB), 9367192 (0x8EEE98), 16749490 \
+        (0xFF93B2), or 16478047 (0xFB6F5F).
 
-        :param name: Topic name, 1-128 characters
-
-        :param icon_color: Color of the topic icon in RGB format. Currently, must be one of 7322096 (0x6FB9F0),
-        16766590 (0xFFD67E), 13338331 (0xCB86DB), 9367192 (0x8EEE98), 16749490
-        (0xFF93B2), or 16478047 (0xFB6F5F)
-
-        :param icon_custom_emoji_id: Unique identifier of the custom emoji shown as the topic icon. Use getForumTopicIconStickers
-        to get all allowed custom emoji identifiers."""
+        :param icon_custom_emoji_id: Unique identifier of the custom emoji shown as the topic icon. Use getForumTopicIconStickers \
+        to get all allowed custom emoji identifiers.
+        """
 
         method_response = await self.api.request_raw(
-            "createForumTopic", get_params(locals())
+            "createForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, ForumTopic)
 
     async def edit_forum_topic(
         self,
         chat_id: int | str,
         message_thread_id: int,
-        name: str | Option[str] = Nothing,
-        icon_custom_emoji_id: str | Option[str] = Nothing,
+        name: str | None = None,
+        icon_custom_emoji_id: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `editForumTopic`, see the [documentation](https://core.telegram.org/bots/api#editforumtopic)
 
-        Use this method to edit name and icon of a topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have can_manage_topics administrator rights, unless it is the creator of the topic. Returns True on success.
-
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
-
-        :param message_thread_id: Unique identifier for the target message thread of the forum topic
-
-        :param name: New topic name, 0-128 characters. If not specified or empty, the current
-        name of the topic will be kept
-
-        :param icon_custom_emoji_id: New unique identifier of the custom emoji shown as the topic icon. Use getForumTopicIconStickers
-        to get all allowed custom emoji identifiers. Pass an empty string to remove
-        the icon. If not specified, the current icon will be kept"""
+        Use this method to edit name and icon of a topic in a forum supergroup chat. 
+        The bot must be an administrator in the chat for this to work and must have 
+        can_manage_topics administrator rights, unless it is the creator of the 
+        topic. Returns True on success.
+
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+
+        :param message_thread_id: Unique identifier for the target message thread of the forum topic.
+
+        :param name: New topic name, 0-128 characters. If not specified or empty, the current \
+        name of the topic will be kept.
+
+        :param icon_custom_emoji_id: New unique identifier of the custom emoji shown as the topic icon. Use getForumTopicIconStickers \
+        to get all allowed custom emoji identifiers. Pass an empty string to remove \
+        the icon. If not specified, the current icon will be kept.
+        """
 
         method_response = await self.api.request_raw(
-            "editForumTopic", get_params(locals())
+            "editForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def close_forum_topic(
         self,
         chat_id: int | str,
         message_thread_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `closeForumTopic`, see the [documentation](https://core.telegram.org/bots/api#closeforumtopic)
 
-        Use this method to close an open topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights, unless it is the creator of the topic. Returns True on success.
+        Use this method to close an open topic in a forum supergroup chat. The bot 
+        must be an administrator in the chat for this to work and must have the can_manage_topics 
+        administrator rights, unless it is the creator of the topic. Returns True 
+        on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param message_thread_id: Unique identifier for the target message thread of the forum topic
+        :param message_thread_id: Unique identifier for the target message thread of the forum topic.
         """
 
         method_response = await self.api.request_raw(
-            "closeForumTopic", get_params(locals())
+            "closeForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def reopen_forum_topic(
         self,
         chat_id: int | str,
         message_thread_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `reopenForumTopic`, see the [documentation](https://core.telegram.org/bots/api#reopenforumtopic)
 
-        Use this method to reopen a closed topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights, unless it is the creator of the topic. Returns True on success.
+        Use this method to reopen a closed topic in a forum supergroup chat. The bot 
+        must be an administrator in the chat for this to work and must have the can_manage_topics 
+        administrator rights, unless it is the creator of the topic. Returns True 
+        on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param message_thread_id: Unique identifier for the target message thread of the forum topic
+        :param message_thread_id: Unique identifier for the target message thread of the forum topic.
         """
 
         method_response = await self.api.request_raw(
-            "reopenForumTopic", get_params(locals())
+            "reopenForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_forum_topic(
         self,
         chat_id: int | str,
         message_thread_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteForumTopic`, see the [documentation](https://core.telegram.org/bots/api#deleteforumtopic)
 
-        Use this method to delete a forum topic along with all its messages in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_delete_messages administrator rights. Returns True on success.
+        Use this method to delete a forum topic along with all its messages in a forum 
+        supergroup chat. The bot must be an administrator in the chat for this to 
+        work and must have the can_delete_messages administrator rights. Returns 
+        True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param message_thread_id: Unique identifier for the target message thread of the forum topic
+        :param message_thread_id: Unique identifier for the target message thread of the forum topic.
         """
 
         method_response = await self.api.request_raw(
-            "deleteForumTopic", get_params(locals())
+            "deleteForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unpin_all_forum_topic_messages(
         self,
         chat_id: int | str,
         message_thread_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unpinAllForumTopicMessages`, see the [documentation](https://core.telegram.org/bots/api#unpinallforumtopicmessages)
 
-        Use this method to clear the list of pinned messages in a forum topic. The bot must be an administrator in the chat for this to work and must have the can_pin_messages administrator right in the supergroup. Returns True on success.
+        Use this method to clear the list of pinned messages in a forum topic. The 
+        bot must be an administrator in the chat for this to work and must have the 
+        can_pin_messages administrator right in the supergroup. Returns True 
+        on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param message_thread_id: Unique identifier for the target message thread of the forum topic
+        :param message_thread_id: Unique identifier for the target message thread of the forum topic.
         """
 
         method_response = await self.api.request_raw(
-            "unpinAllForumTopicMessages", get_params(locals())
+            "unpinAllForumTopicMessages",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def edit_general_forum_topic(
         self,
         chat_id: int | str,
         name: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `editGeneralForumTopic`, see the [documentation](https://core.telegram.org/bots/api#editgeneralforumtopic)
 
-        Use this method to edit the name of the 'General' topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have can_manage_topics administrator rights. Returns True on success.
+        Use this method to edit the name of the 'General' topic in a forum supergroup 
+        chat. The bot must be an administrator in the chat for this to work and must 
+        have can_manage_topics administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
 
-        :param name: New topic name, 1-128 characters"""
+        :param name: New topic name, 1-128 characters.
+        """
 
         method_response = await self.api.request_raw(
-            "editGeneralForumTopic", get_params(locals())
+            "editGeneralForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def close_general_forum_topic(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `closeGeneralForumTopic`, see the [documentation](https://core.telegram.org/bots/api#closegeneralforumtopic)
 
-        Use this method to close an open 'General' topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights. Returns True on success.
+        Use this method to close an open 'General' topic in a forum supergroup chat. 
+        The bot must be an administrator in the chat for this to work and must have 
+        the can_manage_topics administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "closeGeneralForumTopic", get_params(locals())
+            "closeGeneralForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def reopen_general_forum_topic(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `reopenGeneralForumTopic`, see the [documentation](https://core.telegram.org/bots/api#reopengeneralforumtopic)
 
-        Use this method to reopen a closed 'General' topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights. The topic will be automatically unhidden if it was hidden. Returns True on success.
+        Use this method to reopen a closed 'General' topic in a forum supergroup 
+        chat. The bot must be an administrator in the chat for this to work and must 
+        have the can_manage_topics administrator rights. The topic will be automatically 
+        unhidden if it was hidden. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "reopenGeneralForumTopic", get_params(locals())
+            "reopenGeneralForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def hide_general_forum_topic(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `hideGeneralForumTopic`, see the [documentation](https://core.telegram.org/bots/api#hidegeneralforumtopic)
 
-        Use this method to hide the 'General' topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights. The topic will be automatically closed if it was open. Returns True on success.
+        Use this method to hide the 'General' topic in a forum supergroup chat. The 
+        bot must be an administrator in the chat for this to work and must have the 
+        can_manage_topics administrator rights. The topic will be automatically 
+        closed if it was open. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "hideGeneralForumTopic", get_params(locals())
+            "hideGeneralForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unhide_general_forum_topic(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unhideGeneralForumTopic`, see the [documentation](https://core.telegram.org/bots/api#unhidegeneralforumtopic)
 
-        Use this method to unhide the 'General' topic in a forum supergroup chat. The bot must be an administrator in the chat for this to work and must have the can_manage_topics administrator rights. Returns True on success.
+        Use this method to unhide the 'General' topic in a forum supergroup chat. 
+        The bot must be an administrator in the chat for this to work and must have 
+        the can_manage_topics administrator rights. Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "unhideGeneralForumTopic", get_params(locals())
+            "unhideGeneralForumTopic",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def unpin_all_general_forum_topic_messages(
         self,
         chat_id: int | str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `unpinAllGeneralForumTopicMessages`, see the [documentation](https://core.telegram.org/bots/api#unpinallgeneralforumtopicmessages)
 
-        Use this method to clear the list of pinned messages in a General forum topic. The bot must be an administrator in the chat for this to work and must have the can_pin_messages administrator right in the supergroup. Returns True on success.
+        Use this method to clear the list of pinned messages in a General forum topic. 
+        The bot must be an administrator in the chat for this to work and must have 
+        the can_pin_messages administrator right in the supergroup. Returns 
+        True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target supergroup
-        (in the format @supergroupusername)"""
+        :param chat_id: Unique identifier for the target chat or username of the target supergroup \
+        (in the format @supergroupusername).
+        """
 
         method_response = await self.api.request_raw(
-            "unpinAllGeneralForumTopicMessages", get_params(locals())
+            "unpinAllGeneralForumTopicMessages",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def answer_callback_query(
         self,
         callback_query_id: str,
-        text: str | Option[str] = Nothing,
-        show_alert: bool | Option[bool] = Nothing,
-        url: str | Option[str] = Nothing,
-        cache_time: int | Option[int] = Nothing,
+        text: str | None = None,
+        show_alert: bool | None = None,
+        url: str | None = None,
+        cache_time: int | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `answerCallbackQuery`, see the [documentation](https://core.telegram.org/bots/api#answercallbackquery)
 
-        Use this method to send answers to callback queries sent from inline keyboards. The answer will be displayed to the user as a notification at the top of the chat screen or as an alert. On success, True is returned.
+        Use this method to send answers to callback queries sent from inline keyboards. 
+        The answer will be displayed to the user as a notification at the top of the 
+        chat screen or as an alert. On success, True is returned.
 
-        :param callback_query_id: Unique identifier for the query to be answered
+        :param callback_query_id: Unique identifier for the query to be answered.
 
-        :param text: Text of the notification. If not specified, nothing will be shown to the
-        user, 0-200 characters
+        :param text: Text of the notification. If not specified, nothing will be shown to the \
+        user, 0-200 characters.
 
-        :param show_alert: If True, an alert will be shown by the client instead of a notification at
+        :param show_alert: If True, an alert will be shown by the client instead of a notification at \
         the top of the chat screen. Defaults to false.
 
-        :param url: URL that will be opened by the user's client. If you have created a Game and
-        accepted the conditions via @BotFather, specify the URL that opens your
-        game - note that this will only work if the query comes from a callback_game
-        button. Otherwise, you may use links like t.me/your_bot?start=XXXX that
+        :param url: URL that will be opened by the user's client. If you have created a Game and \
+        accepted the conditions via @BotFather, specify the URL that opens your \
+        game - note that this will only work if the query comes from a callback_game \
+        button. Otherwise, you may use links like t.me/your_bot?start=XXXX that \
         open your bot with a parameter.
 
-        :param cache_time: The maximum amount of time in seconds that the result of the callback query
-        may be cached client-side. Telegram apps will support caching starting
-        in version 3.14. Defaults to 0."""
+        :param cache_time: The maximum amount of time in seconds that the result of the callback query \
+        may be cached client-side. Telegram apps will support caching starting \
+        in version 3.14. Defaults to 0.
+        """
 
         method_response = await self.api.request_raw(
-            "answerCallbackQuery", get_params(locals())
+            "answerCallbackQuery",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_user_chat_boosts(
         self,
         chat_id: int | str,
         user_id: int,
         **other: typing.Any,
-    ) -> Result[UserChatBoosts, "APIError"]:
+    ) -> Result[UserChatBoosts, APIError]:
         """Method `getUserChatBoosts`, see the [documentation](https://core.telegram.org/bots/api#getuserchatboosts)
 
-        Use this method to get the list of boosts added to a chat by a user. Requires administrator rights in the chat. Returns a UserChatBoosts object.
+        Use this method to get the list of boosts added to a chat by a user. Requires 
+        administrator rights in the chat. Returns a UserChatBoosts object.
 
-        :param chat_id: Unique identifier for the chat or username of the channel (in the format
-        @channelusername)
+        :param chat_id: Unique identifier for the chat or username of the channel (in the format \
+        @channelusername).
 
-        :param user_id: Unique identifier of the target user"""
+        :param user_id: Unique identifier of the target user.
+        """
 
         method_response = await self.api.request_raw(
-            "getUserChatBoosts", get_params(locals())
+            "getUserChatBoosts",
+            get_params(locals()),
         )
         return full_result(method_response, UserChatBoosts)
 
+    async def get_business_connection(
+        self,
+        business_connection_id: str,
+        **other: typing.Any,
+    ) -> Result[BusinessConnection, APIError]:
+        """Method `getBusinessConnection`, see the [documentation](https://core.telegram.org/bots/api#getbusinessconnection)
+
+        Use this method to get information about the connection of the bot with a
+        business account. Returns a BusinessConnection object on success.
+
+        :param business_connection_id: Unique identifier of the business connection.
+        """
+
+        method_response = await self.api.request_raw(
+            "getBusinessConnection",
+            get_params(locals()),
+        )
+        return full_result(method_response, BusinessConnection)
+
     async def set_my_commands(
         self,
         commands: list[BotCommand],
-        scope: BotCommandScope | Option[BotCommandScope] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMyCommands`, see the [documentation](https://core.telegram.org/bots/api#setmycommands)
 
-        Use this method to change the list of the bot's commands. See this manual for more details about bot commands. Returns True on success.
+        Use this method to change the list of the bot's commands. See this manual 
+        for more details about bot commands. Returns True on success.
 
-        :param commands: A JSON-serialized list of bot commands to be set as the list of the bot's commands.
+        :param commands: A JSON-serialized list of bot commands to be set as the list of the bot's commands. \
         At most 100 commands can be specified.
 
-        :param scope: A JSON-serialized object, describing scope of users for which the commands
+        :param scope: A JSON-serialized object, describing scope of users for which the commands \
         are relevant. Defaults to BotCommandScopeDefault.
 
-        :param language_code: A two-letter ISO 639-1 language code. If empty, commands will be applied
-        to all users from the given scope, for whose language there are no dedicated
-        commands"""
+        :param language_code: A two-letter ISO 639-1 language code. If empty, commands will be applied \
+        to all users from the given scope, for whose language there are no dedicated \
+        commands.
+        """
 
         method_response = await self.api.request_raw(
-            "setMyCommands", get_params(locals())
+            "setMyCommands",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_my_commands(
         self,
-        scope: BotCommandScope | Option[BotCommandScope] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteMyCommands`, see the [documentation](https://core.telegram.org/bots/api#deletemycommands)
 
-        Use this method to delete the list of the bot's commands for the given scope and user language. After deletion, higher level commands will be shown to affected users. Returns True on success.
+        Use this method to delete the list of the bot's commands for the given scope 
+        and user language. After deletion, higher level commands will be shown 
+        to affected users. Returns True on success.
 
-        :param scope: A JSON-serialized object, describing scope of users for which the commands
+        :param scope: A JSON-serialized object, describing scope of users for which the commands \
         are relevant. Defaults to BotCommandScopeDefault.
 
-        :param language_code: A two-letter ISO 639-1 language code. If empty, commands will be applied
-        to all users from the given scope, for whose language there are no dedicated
-        commands"""
+        :param language_code: A two-letter ISO 639-1 language code. If empty, commands will be applied \
+        to all users from the given scope, for whose language there are no dedicated \
+        commands.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteMyCommands", get_params(locals())
+            "deleteMyCommands",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_my_commands(
         self,
-        scope: BotCommandScope | Option[BotCommandScope] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[list[BotCommand], "APIError"]:
+    ) -> Result[list[BotCommand], APIError]:
         """Method `getMyCommands`, see the [documentation](https://core.telegram.org/bots/api#getmycommands)
 
-        Use this method to get the current list of the bot's commands for the given scope and user language. Returns an Array of BotCommand objects. If commands aren't set, an empty list is returned.
+        Use this method to get the current list of the bot's commands for the given 
+        scope and user language. Returns an Array of BotCommand objects. If commands 
+        aren't set, an empty list is returned.
 
-        :param scope: A JSON-serialized object, describing scope of users. Defaults to BotCommandScopeDefault.
+        :param scope: A JSON-serialized object, describing scope of users. Defaults to BotCommandScopeDefault. \
 
-        :param language_code: A two-letter ISO 639-1 language code or an empty string"""
+        :param language_code: A two-letter ISO 639-1 language code or an empty string.
+        """
 
         method_response = await self.api.request_raw(
-            "getMyCommands", get_params(locals())
+            "getMyCommands",
+            get_params(locals()),
         )
         return full_result(method_response, list[BotCommand])
 
     async def set_my_name(
         self,
-        name: str | Option[str] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        name: str | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMyName`, see the [documentation](https://core.telegram.org/bots/api#setmyname)
 
         Use this method to change the bot's name. Returns True on success.
 
-        :param name: New bot name; 0-64 characters. Pass an empty string to remove the dedicated
+        :param name: New bot name; 0-64 characters. Pass an empty string to remove the dedicated \
         name for the given language.
 
-        :param language_code: A two-letter ISO 639-1 language code. If empty, the name will be shown to
-        all users for whose language there is no dedicated name."""
+        :param language_code: A two-letter ISO 639-1 language code. If empty, the name will be shown to \
+        all users for whose language there is no dedicated name.
+        """
 
-        method_response = await self.api.request_raw("setMyName", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "setMyName",
+            get_params(locals()),
+        )
         return full_result(method_response, bool)
 
     async def get_my_name(
         self,
-        language_code: str | Option[str] = Nothing,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[BotName, "APIError"]:
+    ) -> Result[BotName, APIError]:
         """Method `getMyName`, see the [documentation](https://core.telegram.org/bots/api#getmyname)
 
-        Use this method to get the current bot name for the given user language. Returns BotName on success.
+        Use this method to get the current bot name for the given user language. Returns
+        BotName on success.
 
-        :param language_code: A two-letter ISO 639-1 language code or an empty string"""
+        :param language_code: A two-letter ISO 639-1 language code or an empty string.
+        """
 
-        method_response = await self.api.request_raw("getMyName", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "getMyName",
+            get_params(locals()),
+        )
         return full_result(method_response, BotName)
 
     async def set_my_description(
         self,
-        description: str | Option[str] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        description: str | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMyDescription`, see the [documentation](https://core.telegram.org/bots/api#setmydescription)
 
-        Use this method to change the bot's description, which is shown in the chat with the bot if the chat is empty. Returns True on success.
+        Use this method to change the bot's description, which is shown in the chat 
+        with the bot if the chat is empty. Returns True on success.
 
-        :param description: New bot description; 0-512 characters. Pass an empty string to remove the
+        :param description: New bot description; 0-512 characters. Pass an empty string to remove the \
         dedicated description for the given language.
 
-        :param language_code: A two-letter ISO 639-1 language code. If empty, the description will be
-        applied to all users for whose language there is no dedicated description."""
+        :param language_code: A two-letter ISO 639-1 language code. If empty, the description will be \
+        applied to all users for whose language there is no dedicated description. \
+        """
 
         method_response = await self.api.request_raw(
-            "setMyDescription", get_params(locals())
+            "setMyDescription",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_my_description(
         self,
-        language_code: str | Option[str] = Nothing,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[BotDescription, "APIError"]:
+    ) -> Result[BotDescription, APIError]:
         """Method `getMyDescription`, see the [documentation](https://core.telegram.org/bots/api#getmydescription)
 
-        Use this method to get the current bot description for the given user language. Returns BotDescription on success.
+        Use this method to get the current bot description for the given user language.
+        Returns BotDescription on success.
 
-        :param language_code: A two-letter ISO 639-1 language code or an empty string"""
+        :param language_code: A two-letter ISO 639-1 language code or an empty string.
+        """
 
         method_response = await self.api.request_raw(
-            "getMyDescription", get_params(locals())
+            "getMyDescription",
+            get_params(locals()),
         )
         return full_result(method_response, BotDescription)
 
     async def set_my_short_description(
         self,
-        short_description: str | Option[str] = Nothing,
-        language_code: str | Option[str] = Nothing,
+        short_description: str | None = None,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMyShortDescription`, see the [documentation](https://core.telegram.org/bots/api#setmyshortdescription)
 
-        Use this method to change the bot's short description, which is shown on the bot's profile page and is sent together with the link when users share the bot. Returns True on success.
+        Use this method to change the bot's short description, which is shown on 
+        the bot's profile page and is sent together with the link when users share 
+        the bot. Returns True on success.
 
-        :param short_description: New short description for the bot; 0-120 characters. Pass an empty string
+        :param short_description: New short description for the bot; 0-120 characters. Pass an empty string \
         to remove the dedicated short description for the given language.
 
-        :param language_code: A two-letter ISO 639-1 language code. If empty, the short description will
-        be applied to all users for whose language there is no dedicated short description.
+        :param language_code: A two-letter ISO 639-1 language code. If empty, the short description will \
+        be applied to all users for whose language there is no dedicated short description. \
         """
 
         method_response = await self.api.request_raw(
-            "setMyShortDescription", get_params(locals())
+            "setMyShortDescription",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_my_short_description(
         self,
-        language_code: str | Option[str] = Nothing,
+        language_code: str | None = None,
         **other: typing.Any,
-    ) -> Result[BotShortDescription, "APIError"]:
+    ) -> Result[BotShortDescription, APIError]:
         """Method `getMyShortDescription`, see the [documentation](https://core.telegram.org/bots/api#getmyshortdescription)
 
-        Use this method to get the current bot short description for the given user language. Returns BotShortDescription on success.
+        Use this method to get the current bot short description for the given user
+        language. Returns BotShortDescription on success.
 
-        :param language_code: A two-letter ISO 639-1 language code or an empty string"""
+        :param language_code: A two-letter ISO 639-1 language code or an empty string.
+        """
 
         method_response = await self.api.request_raw(
-            "getMyShortDescription", get_params(locals())
+            "getMyShortDescription",
+            get_params(locals()),
         )
         return full_result(method_response, BotShortDescription)
 
     async def set_chat_menu_button(
         self,
-        chat_id: int | Option[int] = Nothing,
-        menu_button: MenuButton | Option[MenuButton] = Nothing,
+        chat_id: int | None = None,
+        menu_button: MenuButton | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setChatMenuButton`, see the [documentation](https://core.telegram.org/bots/api#setchatmenubutton)
 
-        Use this method to change the bot's menu button in a private chat, or the default menu button. Returns True on success.
+        Use this method to change the bot's menu button in a private chat, or the default 
+        menu button. Returns True on success.
 
-        :param chat_id: Unique identifier for the target private chat. If not specified, default
-        bot's menu button will be changed
+        :param chat_id: Unique identifier for the target private chat. If not specified, default \
+        bot's menu button will be changed.
 
-        :param menu_button: A JSON-serialized object for the bot's new menu button. Defaults to MenuButtonDefault
+        :param menu_button: A JSON-serialized object for the bot's new menu button. Defaults to MenuButtonDefault. \
         """
 
         method_response = await self.api.request_raw(
-            "setChatMenuButton", get_params(locals())
+            "setChatMenuButton",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_chat_menu_button(
         self,
-        chat_id: int | Option[int] = Nothing,
+        chat_id: int | None = None,
         **other: typing.Any,
-    ) -> Result[MenuButtonCommands | MenuButtonWebApp | MenuButtonDefault, "APIError"]:
+    ) -> Result[
+        Variative[MenuButtonCommands, MenuButtonWebApp, MenuButtonDefault], APIError
+    ]:
         """Method `getChatMenuButton`, see the [documentation](https://core.telegram.org/bots/api#getchatmenubutton)
 
-        Use this method to get the current value of the bot's menu button in a private chat, or the default menu button. Returns MenuButton on success.
+        Use this method to get the current value of the bot's menu button in a private 
+        chat, or the default menu button. Returns MenuButton on success.
 
-        :param chat_id: Unique identifier for the target private chat. If not specified, default
-        bot's menu button will be returned"""
+        :param chat_id: Unique identifier for the target private chat. If not specified, default \
+        bot's menu button will be returned.
+        """
 
         method_response = await self.api.request_raw(
-            "getChatMenuButton", get_params(locals())
+            "getChatMenuButton",
+            get_params(locals()),
         )
         return full_result(
-            method_response, MenuButtonCommands | MenuButtonWebApp | MenuButtonDefault
+            method_response,
+            Variative[MenuButtonCommands, MenuButtonWebApp, MenuButtonDefault],
         )
 
     async def set_my_default_administrator_rights(
         self,
-        rights: ChatAdministratorRights | Option[ChatAdministratorRights] = Nothing,
-        for_channels: bool | Option[bool] = Nothing,
+        rights: ChatAdministratorRights | None = None,
+        for_channels: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setMyDefaultAdministratorRights`, see the [documentation](https://core.telegram.org/bots/api#setmydefaultadministratorrights)
 
-        Use this method to change the default administrator rights requested by the bot when it's added as an administrator to groups or channels. These rights will be suggested to users, but they are free to modify the list before adding the bot. Returns True on success.
+        Use this method to change the default administrator rights requested by 
+        the bot when it's added as an administrator to groups or channels. These 
+        rights will be suggested to users, but they are free to modify the list before 
+        adding the bot. Returns True on success.
 
-        :param rights: A JSON-serialized object describing new default administrator rights.
+        :param rights: A JSON-serialized object describing new default administrator rights. \
         If not specified, the default administrator rights will be cleared.
 
-        :param for_channels: Pass True to change the default administrator rights of the bot in channels.
-        Otherwise, the default administrator rights of the bot for groups and supergroups
-        will be changed."""
+        :param for_channels: Pass True to change the default administrator rights of the bot in channels. \
+        Otherwise, the default administrator rights of the bot for groups and supergroups \
+        will be changed.
+        """
 
         method_response = await self.api.request_raw(
-            "setMyDefaultAdministratorRights", get_params(locals())
+            "setMyDefaultAdministratorRights",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def get_my_default_administrator_rights(
         self,
-        for_channels: bool | Option[bool] = Nothing,
+        for_channels: bool | None = None,
         **other: typing.Any,
-    ) -> Result[ChatAdministratorRights, "APIError"]:
+    ) -> Result[ChatAdministratorRights, APIError]:
         """Method `getMyDefaultAdministratorRights`, see the [documentation](https://core.telegram.org/bots/api#getmydefaultadministratorrights)
 
-        Use this method to get the current default administrator rights of the bot. Returns ChatAdministratorRights on success.
+        Use this method to get the current default administrator rights of the bot. 
+        Returns ChatAdministratorRights on success.
 
-        :param for_channels: Pass True to get default administrator rights of the bot in channels. Otherwise,
-        default administrator rights of the bot for groups and supergroups will
-        be returned."""
+        :param for_channels: Pass True to get default administrator rights of the bot in channels. Otherwise, \
+        default administrator rights of the bot for groups and supergroups will \
+        be returned.
+        """
 
         method_response = await self.api.request_raw(
-            "getMyDefaultAdministratorRights", get_params(locals())
+            "getMyDefaultAdministratorRights",
+            get_params(locals()),
         )
         return full_result(method_response, ChatAdministratorRights)
 
     async def edit_message_text(
         self,
         text: str,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        link_preview_options: LinkPreviewOptions | Option[LinkPreviewOptions] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        parse_mode: str | None = None,
+        entities: list[MessageEntity] | None = None,
+        link_preview_options: LinkPreviewOptions | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `editMessageText`, see the [documentation](https://core.telegram.org/bots/api#editmessagetext)
 
-        Use this method to edit text and game messages. On success, if the edited message is not an inline message, the edited Message is returned, otherwise True is returned.
+        Use this method to edit text and game messages. On success, if the edited 
+        message is not an inline message, the edited Message is returned, otherwise 
+        True is returned.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        to edit
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        to edit.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param text: New text of the message, 1-4096 characters after entities parsing
+        :param text: New text of the message, 1-4096 characters after entities parsing.
 
-        :param parse_mode: Mode for parsing entities in the message text. See formatting options for
+        :param parse_mode: Mode for parsing entities in the message text. See formatting options for \
         more details.
 
-        :param entities: A JSON-serialized list of special entities that appear in message text,
-        which can be specified instead of parse_mode
+        :param entities: A JSON-serialized list of special entities that appear in message text, \
+        which can be specified instead of parse_mode.
 
-        :param link_preview_options: Link preview generation options for the message
+        :param link_preview_options: Link preview generation options for the message.
 
-        :param reply_markup: A JSON-serialized object for an inline keyboard."""
+        :param reply_markup: A JSON-serialized object for an inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "editMessageText", get_params(locals())
+            "editMessageText",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def edit_message_caption(
         self,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        caption: str | Option[str] = Nothing,
-        parse_mode: str | Option[str] = Nothing,
-        caption_entities: list[MessageEntity] | Option[list[MessageEntity]] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        caption: str | None = None,
+        parse_mode: str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `editMessageCaption`, see the [documentation](https://core.telegram.org/bots/api#editmessagecaption)
 
-        Use this method to edit captions of messages. On success, if the edited message is not an inline message, the edited Message is returned, otherwise True is returned.
+        Use this method to edit captions of messages. On success, if the edited message 
+        is not an inline message, the edited Message is returned, otherwise True 
+        is returned.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        to edit
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        to edit.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param caption: New caption of the message, 0-1024 characters after entities parsing
+        :param caption: New caption of the message, 0-1024 characters after entities parsing. \
 
-        :param parse_mode: Mode for parsing entities in the message caption. See formatting options
+        :param parse_mode: Mode for parsing entities in the message caption. See formatting options \
         for more details.
 
-        :param caption_entities: A JSON-serialized list of special entities that appear in the caption,
-        which can be specified instead of parse_mode
+        :param caption_entities: A JSON-serialized list of special entities that appear in the caption, \
+        which can be specified instead of parse_mode.
 
-        :param reply_markup: A JSON-serialized object for an inline keyboard."""
+        :param reply_markup: A JSON-serialized object for an inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "editMessageCaption", get_params(locals())
+            "editMessageCaption",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def edit_message_media(
         self,
         media: InputMedia,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `editMessageMedia`, see the [documentation](https://core.telegram.org/bots/api#editmessagemedia)
 
-        Use this method to edit animation, audio, document, photo, or video messages. If a message is part of a message album, then it can be edited only to an audio for audio albums, only to a document for document albums and to a photo or a video otherwise. When an inline message is edited, a new file can't be uploaded; use a previously uploaded file via its file_id or specify a URL. On success, if the edited message is not an inline message, the edited Message is returned, otherwise True is returned.
-
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        Use this method to edit animation, audio, document, photo, or video messages. 
+        If a message is part of a message album, then it can be edited only to an audio 
+        for audio albums, only to a document for document albums and to a photo or 
+        a video otherwise. When an inline message is edited, a new file can't be uploaded; 
+        use a previously uploaded file via its file_id or specify a URL. On success, 
+        if the edited message is not an inline message, the edited Message is returned, 
+        otherwise True is returned.
+
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
+
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        to edit.
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        to edit
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param media: A JSON-serialized object for a new media content of the message.
 
-        :param media: A JSON-serialized object for a new media content of the message
-
-        :param reply_markup: A JSON-serialized object for a new inline keyboard."""
+        :param reply_markup: A JSON-serialized object for a new inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "editMessageMedia", get_params(locals())
+            "editMessageMedia",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def edit_message_live_location(
         self,
         latitude: float,
         longitude: float,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        horizontal_accuracy: float | Option[float] = Nothing,
-        heading: int | Option[int] = Nothing,
-        proximity_alert_radius: int | Option[int] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        horizontal_accuracy: float | None = None,
+        heading: int | None = None,
+        proximity_alert_radius: int | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `editMessageLiveLocation`, see the [documentation](https://core.telegram.org/bots/api#editmessagelivelocation)
 
-        Use this method to edit live location messages. A location can be edited until its live_period expires or editing is explicitly disabled by a call to stopMessageLiveLocation. On success, if the edited message is not an inline message, the edited Message is returned, otherwise True is returned.
+        Use this method to edit live location messages. A location can be edited 
+        until its live_period expires or editing is explicitly disabled by a call 
+        to stopMessageLiveLocation. On success, if the edited message is not an 
+        inline message, the edited Message is returned, otherwise True is returned.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        to edit
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        to edit.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param latitude: Latitude of new location
+        :param latitude: Latitude of new location.
 
-        :param longitude: Longitude of new location
+        :param longitude: Longitude of new location.
 
-        :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500
+        :param horizontal_accuracy: The radius of uncertainty for the location, measured in meters; 0-1500. \
 
-        :param heading: Direction in which the user is moving, in degrees. Must be between 1 and 360
+        :param heading: Direction in which the user is moving, in degrees. Must be between 1 and 360 \
         if specified.
 
-        :param proximity_alert_radius: The maximum distance for proximity alerts about approaching another chat
+        :param proximity_alert_radius: The maximum distance for proximity alerts about approaching another chat \
         member, in meters. Must be between 1 and 100000 if specified.
 
-        :param reply_markup: A JSON-serialized object for a new inline keyboard."""
+        :param reply_markup: A JSON-serialized object for a new inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "editMessageLiveLocation", get_params(locals())
+            "editMessageLiveLocation",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def stop_message_live_location(
         self,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `stopMessageLiveLocation`, see the [documentation](https://core.telegram.org/bots/api#stopmessagelivelocation)
 
-        Use this method to stop updating a live location message before live_period expires. On success, if the message is not an inline message, the edited Message is returned, otherwise True is returned.
+        Use this method to stop updating a live location message before live_period 
+        expires. On success, if the message is not an inline message, the edited 
+        Message is returned, otherwise True is returned.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        with live location to stop
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        with live location to stop.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param reply_markup: A JSON-serialized object for a new inline keyboard."""
+        :param reply_markup: A JSON-serialized object for a new inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "stopMessageLiveLocation", get_params(locals())
+            "stopMessageLiveLocation",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def edit_message_reply_markup(
         self,
-        chat_id: int | str | Option[int | str] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        chat_id: int | str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `editMessageReplyMarkup`, see the [documentation](https://core.telegram.org/bots/api#editmessagereplymarkup)
 
-        Use this method to edit only the reply markup of messages. On success, if the edited message is not an inline message, the edited Message is returned, otherwise True is returned.
+        Use this method to edit only the reply markup of messages. On success, if 
+        the edited message is not an inline message, the edited Message is returned, 
+        otherwise True is returned.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat or username of the target channel (in the format @channelusername)
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat or username of the target channel (in the format @channelusername). \
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the message
-        to edit
+        :param message_id: Required if inline_message_id is not specified. Identifier of the message \
+        to edit.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
 
-        :param reply_markup: A JSON-serialized object for an inline keyboard."""
+        :param reply_markup: A JSON-serialized object for an inline keyboard.
+        """
 
         method_response = await self.api.request_raw(
-            "editMessageReplyMarkup", get_params(locals())
+            "editMessageReplyMarkup",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def stop_poll(
         self,
         chat_id: int | str,
         message_id: int,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Poll, "APIError"]:
+    ) -> Result[Poll, APIError]:
         """Method `stopPoll`, see the [documentation](https://core.telegram.org/bots/api#stoppoll)
 
-        Use this method to stop a poll which was sent by the bot. On success, the stopped Poll is returned.
+        Use this method to stop a poll which was sent by the bot. On success, the stopped 
+        Poll is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_id: Identifier of the original message with the poll
+        :param message_id: Identifier of the original message with the poll.
 
         :param reply_markup: A JSON-serialized object for a new message inline keyboard.
         """
 
-        method_response = await self.api.request_raw("stopPoll", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "stopPoll",
+            get_params(locals()),
+        )
         return full_result(method_response, Poll)
 
     async def delete_message(
         self,
         chat_id: int | str,
         message_id: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteMessage`, see the [documentation](https://core.telegram.org/bots/api#deletemessage)
 
-        Use this method to delete a message, including service messages, with the following limitations:
-        - A message can only be deleted if it was sent less than 48 hours ago.
-        - Service messages about a supergroup, channel, or forum topic creation can't be deleted.
-        - A dice message in a private chat can only be deleted if it was sent more than 24 hours ago.
-        - Bots can delete outgoing messages in private chats, groups, and supergroups.
-        - Bots can delete incoming messages in private chats.
-        - Bots granted can_post_messages permissions can delete outgoing messages in channels.
-        - If the bot is an administrator of a group, it can delete any message there.
-        - If the bot has can_delete_messages permission in a supergroup or a channel, it can delete any message there.
+        Use this method to delete a message, including service messages, with the 
+        following limitations: - A message can only be deleted if it was sent less 
+        than 48 hours ago. - Service messages about a supergroup, channel, or forum 
+        topic creation can't be deleted. - A dice message in a private chat can only 
+        be deleted if it was sent more than 24 hours ago. - Bots can delete outgoing 
+        messages in private chats, groups, and supergroups. - Bots can delete incoming 
+        messages in private chats. - Bots granted can_post_messages permissions 
+        can delete outgoing messages in channels. - If the bot is an administrator 
+        of a group, it can delete any message there. - If the bot has can_delete_messages 
+        permission in a supergroup or a channel, it can delete any message there. 
         Returns True on success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_id: Identifier of the message to delete"""
+        :param message_id: Identifier of the message to delete.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteMessage", get_params(locals())
+            "deleteMessage",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_messages(
         self,
         chat_id: int | str,
         message_ids: list[int],
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteMessages`, see the [documentation](https://core.telegram.org/bots/api#deletemessages)
 
-        Use this method to delete multiple messages simultaneously. If some of the specified messages can't be found, they are skipped. Returns True on success.
+        Use this method to delete multiple messages simultaneously. If some of 
+        the specified messages can't be found, they are skipped. Returns True on 
+        success.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_ids: Identifiers of 1-100 messages to delete. See deleteMessage for limitations
-        on which messages can be deleted"""
+        :param message_ids: A JSON-serialized list of 1-100 identifiers of messages to delete. See \
+        deleteMessage for limitations on which messages can be deleted.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteMessages", get_params(locals())
+            "deleteMessages",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def send_sticker(
         self,
         chat_id: int | str,
         sticker: InputFile | str,
-        message_thread_id: int | Option[int] = Nothing,
-        emoji: str | Option[str] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup
-        | ReplyKeyboardMarkup
-        | ReplyKeyboardRemove
-        | ForceReply
-        | Option[
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        emoji: str | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: (
             InlineKeyboardMarkup
             | ReplyKeyboardMarkup
             | ReplyKeyboardRemove
             | ForceReply
-        ] = Nothing,
+            | None
+        ) = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendSticker`, see the [documentation](https://core.telegram.org/bots/api#sendsticker)
 
-        Use this method to send static .WEBP, animated .TGS, or video .WEBM stickers. On success, the sent Message is returned.
+        Use this method to send static .WEBP, animated .TGS, or video .WEBM stickers. 
+        On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param sticker: Sticker to send. Pass a file_id as String to send a file that exists on the
-        Telegram servers (recommended), pass an HTTP URL as a String for Telegram
-        to get a .WEBP sticker from the Internet, or upload a new .WEBP or .TGS sticker
-        using multipart/form-data. More information on Sending Files: https://core.telegram.org/bots/api#sending-files.
-        Video stickers can only be sent by a file_id. Animated stickers can't be
-        sent via an HTTP URL.
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param emoji: Emoji associated with the sticker; only for just uploaded stickers
+        :param sticker: Sticker to send. Pass a file_id as String to send a file that exists on the \
+        Telegram servers (recommended), pass an HTTP URL as a String for Telegram \
+        to get a .WEBP sticker from the Internet, or upload a new .WEBP, .TGS, or .WEBM \
+        sticker using multipart/form-data. More information on Sending Files: \
+        https://core.telegram.org/bots/api#sending-files. Video and animated \
+        stickers can't be sent via an HTTP URL.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param emoji: Emoji associated with the sticker; only for just uploaded stickers.
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param reply_parameters: Description of the message to reply to
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_markup: Additional interface options. A JSON-serialized object for an inline
-        keyboard, custom reply keyboard, instructions to remove reply keyboard
-        or to force a reply from the user."""
+        :param reply_parameters: Description of the message to reply to.
+
+        :param reply_markup: Additional interface options. A JSON-serialized object for an inline \
+        keyboard, custom reply keyboard, instructions to remove reply keyboard \
+        or to force a reply from the user. Not supported for messages sent on behalf \
+        of a business account.
+        """
 
         method_response = await self.api.request_raw(
-            "sendSticker", get_params(locals())
+            "sendSticker",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def get_sticker_set(
         self,
         name: str,
         **other: typing.Any,
-    ) -> Result[StickerSet, "APIError"]:
+    ) -> Result[StickerSet, APIError]:
         """Method `getStickerSet`, see the [documentation](https://core.telegram.org/bots/api#getstickerset)
 
         Use this method to get a sticker set. On success, a StickerSet object is returned.
 
-        :param name: Name of the sticker set"""
+        :param name: Name of the sticker set.
+        """
 
         method_response = await self.api.request_raw(
-            "getStickerSet", get_params(locals())
+            "getStickerSet",
+            get_params(locals()),
         )
         return full_result(method_response, StickerSet)
 
     async def get_custom_emoji_stickers(
         self,
         custom_emoji_ids: list[str],
         **other: typing.Any,
-    ) -> Result[list[Sticker], "APIError"]:
+    ) -> Result[list[Sticker], APIError]:
         """Method `getCustomEmojiStickers`, see the [documentation](https://core.telegram.org/bots/api#getcustomemojistickers)
 
-        Use this method to get information about custom emoji stickers by their identifiers. Returns an Array of Sticker objects.
+        Use this method to get information about custom emoji stickers by their 
+        identifiers. Returns an Array of Sticker objects.
 
-        :param custom_emoji_ids: List of custom emoji identifiers. At most 200 custom emoji identifiers
-        can be specified."""
+        :param custom_emoji_ids: A JSON-serialized list of custom emoji identifiers. At most 200 custom \
+        emoji identifiers can be specified.
+        """
 
         method_response = await self.api.request_raw(
-            "getCustomEmojiStickers", get_params(locals())
+            "getCustomEmojiStickers",
+            get_params(locals()),
         )
         return full_result(method_response, list[Sticker])
 
     async def upload_sticker_file(
         self,
         user_id: int,
         sticker: InputFile,
-        sticker_format: str,
+        sticker_format: typing.Literal["static", "animated", "video"],
         **other: typing.Any,
-    ) -> Result[File, "APIError"]:
+    ) -> Result[File, APIError]:
         """Method `uploadStickerFile`, see the [documentation](https://core.telegram.org/bots/api#uploadstickerfile)
 
-        Use this method to upload a file with a sticker for later use in the createNewStickerSet and addStickerToSet methods (the file can be used multiple times). Returns the uploaded File on success.
+        Use this method to upload a file with a sticker for later use in the createNewStickerSet, 
+        addStickerToSet, or replaceStickerInSet methods (the file can be used 
+        multiple times). Returns the uploaded File on success.
 
-        :param user_id: User identifier of sticker file owner
+        :param user_id: User identifier of sticker file owner.
 
-        :param sticker: A file with the sticker in .WEBP, .PNG, .TGS, or .WEBM format. See https://core.telegram.org/stickers
-        for technical requirements. More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        :param sticker: A file with the sticker in .WEBP, .PNG, .TGS, or .WEBM format. See https://core.telegram.org/stickers \
+        for technical requirements. More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
 
-        :param sticker_format: Format of the sticker, must be one of `static`, `animated`, `video`
+        :param sticker_format: Format of the sticker, must be one of `static`, `animated`, `video`.
         """
 
         method_response = await self.api.request_raw(
-            "uploadStickerFile", get_params(locals())
+            "uploadStickerFile",
+            get_params(locals()),
         )
         return full_result(method_response, File)
 
     async def create_new_sticker_set(
         self,
         user_id: int,
         name: str,
         title: str,
         stickers: list[InputSticker],
-        sticker_format: str,
-        sticker_type: str | Option[str] = Nothing,
-        needs_repainting: bool | Option[bool] = Nothing,
+        sticker_type: typing.Literal["regular", "mask", "custom_emoji"] | None = None,
+        needs_repainting: bool | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `createNewStickerSet`, see the [documentation](https://core.telegram.org/bots/api#createnewstickerset)
 
-        Use this method to create a new sticker set owned by a user. The bot will be able to edit the sticker set thus created. Returns True on success.
+        Use this method to create a new sticker set owned by a user. The bot will be 
+        able to edit the sticker set thus created. Returns True on success.
 
-        :param user_id: User identifier of created sticker set owner
+        :param user_id: User identifier of created sticker set owner.
 
-        :param name: Short name of sticker set, to be used in t.me/addstickers/ URLs (e.g., animals).
-        Can contain only English letters, digits and underscores. Must begin with
-        a letter, can't contain consecutive underscores and must end in `_by_<bot_username>`.
+        :param name: Short name of sticker set, to be used in t.me/addstickers/ URLs (e.g., animals). \
+        Can contain only English letters, digits and underscores. Must begin with \
+        a letter, can't contain consecutive underscores and must end in `_by_<bot_username>`. \
         <bot_username> is case insensitive. 1-64 characters.
 
-        :param title: Sticker set title, 1-64 characters
+        :param title: Sticker set title, 1-64 characters.
 
-        :param stickers: A JSON-serialized list of 1-50 initial stickers to be added to the sticker
-        set
+        :param stickers: A JSON-serialized list of 1-50 initial stickers to be added to the sticker \
+        set.
 
-        :param sticker_format: Format of stickers in the set, must be one of `static`, `animated`, `video`
-
-        :param sticker_type: Type of stickers in the set, pass `regular`, `mask`, or `custom_emoji`.
+        :param sticker_type: Type of stickers in the set, pass `regular`, `mask`, or `custom_emoji`. \
         By default, a regular sticker set is created.
 
-        :param needs_repainting: Pass True if stickers in the sticker set must be repainted to the color of
-        text when used in messages, the accent color if used as emoji status, white
-        on chat photos, or another appropriate color based on context; for custom
-        emoji sticker sets only"""
+        :param needs_repainting: Pass True if stickers in the sticker set must be repainted to the color of \
+        text when used in messages, the accent color if used as emoji status, white \
+        on chat photos, or another appropriate color based on context; for custom \
+        emoji sticker sets only.
+        """
 
         method_response = await self.api.request_raw(
-            "createNewStickerSet", get_params(locals())
+            "createNewStickerSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def add_sticker_to_set(
         self,
         user_id: int,
         name: str,
         sticker: InputSticker,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `addStickerToSet`, see the [documentation](https://core.telegram.org/bots/api#addstickertoset)
 
-        Use this method to add a new sticker to a set created by the bot. The format of the added sticker must match the format of the other stickers in the set. Emoji sticker sets can have up to 200 stickers. Animated and video sticker sets can have up to 50 stickers. Static sticker sets can have up to 120 stickers. Returns True on success.
+        Use this method to add a new sticker to a set created by the bot. Emoji sticker 
+        sets can have up to 200 stickers. Other sticker sets can have up to 120 stickers. 
+        Returns True on success.
 
-        :param user_id: User identifier of sticker set owner
+        :param user_id: User identifier of sticker set owner.
 
-        :param name: Sticker set name
+        :param name: Sticker set name.
 
-        :param sticker: A JSON-serialized object with information about the added sticker. If
-        exactly the same sticker had already been added to the set, then the set isn't
-        changed."""
+        :param sticker: A JSON-serialized object with information about the added sticker. If \
+        exactly the same sticker had already been added to the set, then the set isn't \
+        changed.
+        """
 
         method_response = await self.api.request_raw(
-            "addStickerToSet", get_params(locals())
+            "addStickerToSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_position_in_set(
         self,
         sticker: str,
         position: int,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerPositionInSet`, see the [documentation](https://core.telegram.org/bots/api#setstickerpositioninset)
 
-        Use this method to move a sticker in a set created by the bot to a specific position. Returns True on success.
+        Use this method to move a sticker in a set created by the bot to a specific position.
+        Returns True on success.
 
-        :param sticker: File identifier of the sticker
+        :param sticker: File identifier of the sticker.
 
-        :param position: New sticker position in the set, zero-based"""
+        :param position: New sticker position in the set, zero-based.
+        """
 
         method_response = await self.api.request_raw(
-            "setStickerPositionInSet", get_params(locals())
+            "setStickerPositionInSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_sticker_from_set(
         self,
         sticker: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteStickerFromSet`, see the [documentation](https://core.telegram.org/bots/api#deletestickerfromset)
 
-        Use this method to delete a sticker from a set created by the bot. Returns True on success.
+        Use this method to delete a sticker from a set created by the bot. Returns
+        True on success.
 
-        :param sticker: File identifier of the sticker"""
+        :param sticker: File identifier of the sticker.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteStickerFromSet", get_params(locals())
+            "deleteStickerFromSet",
+            get_params(locals()),
+        )
+        return full_result(method_response, bool)
+
+    async def replace_sticker_in_set(
+        self,
+        user_id: int,
+        name: str,
+        old_sticker: str,
+        sticker: InputSticker,
+        **other: typing.Any,
+    ) -> Result[bool, APIError]:
+        """Method `replaceStickerInSet`, see the [documentation](https://core.telegram.org/bots/api#replacestickerinset)
+
+        Use this method to replace an existing sticker in a sticker set with a new 
+        one. The method is equivalent to calling deleteStickerFromSet, then addStickerToSet, 
+        then setStickerPositionInSet. Returns True on success.
+
+        :param user_id: User identifier of the sticker set owner.
+
+        :param name: Sticker set name.
+
+        :param old_sticker: File identifier of the replaced sticker.
+
+        :param sticker: A JSON-serialized object with information about the added sticker. If \
+        exactly the same sticker had already been added to the set, then the set remains \
+        unchanged.
+        """
+
+        method_response = await self.api.request_raw(
+            "replaceStickerInSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_emoji_list(
         self,
         sticker: str,
         emoji_list: list[str],
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerEmojiList`, see the [documentation](https://core.telegram.org/bots/api#setstickeremojilist)
 
-        Use this method to change the list of emoji assigned to a regular or custom emoji sticker. The sticker must belong to a sticker set created by the bot. Returns True on success.
+        Use this method to change the list of emoji assigned to a regular or custom
+        emoji sticker. The sticker must belong to a sticker set created by the bot.
+        Returns True on success.
 
-        :param sticker: File identifier of the sticker
+        :param sticker: File identifier of the sticker.
 
-        :param emoji_list: A JSON-serialized list of 1-20 emoji associated with the sticker
+        :param emoji_list: A JSON-serialized list of 1-20 emoji associated with the sticker.
         """
 
         method_response = await self.api.request_raw(
-            "setStickerEmojiList", get_params(locals())
+            "setStickerEmojiList",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_keywords(
         self,
         sticker: str,
-        keywords: list[str] | Option[list[str]] = Nothing,
+        keywords: list[str] | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerKeywords`, see the [documentation](https://core.telegram.org/bots/api#setstickerkeywords)
 
-        Use this method to change search keywords assigned to a regular or custom emoji sticker. The sticker must belong to a sticker set created by the bot. Returns True on success.
+        Use this method to change search keywords assigned to a regular or custom 
+        emoji sticker. The sticker must belong to a sticker set created by the bot. 
+        Returns True on success.
 
-        :param sticker: File identifier of the sticker
+        :param sticker: File identifier of the sticker.
 
-        :param keywords: A JSON-serialized list of 0-20 search keywords for the sticker with total
-        length of up to 64 characters"""
+        :param keywords: A JSON-serialized list of 0-20 search keywords for the sticker with total \
+        length of up to 64 characters.
+        """
 
         method_response = await self.api.request_raw(
-            "setStickerKeywords", get_params(locals())
+            "setStickerKeywords",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_mask_position(
         self,
         sticker: str,
-        mask_position: MaskPosition | Option[MaskPosition] = Nothing,
+        mask_position: MaskPosition | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerMaskPosition`, see the [documentation](https://core.telegram.org/bots/api#setstickermaskposition)
 
-        Use this method to change the mask position of a mask sticker. The sticker must belong to a sticker set that was created by the bot. Returns True on success.
+        Use this method to change the mask position of a mask sticker. The sticker 
+        must belong to a sticker set that was created by the bot. Returns True on success.
 
-        :param sticker: File identifier of the sticker
+        :param sticker: File identifier of the sticker.
 
-        :param mask_position: A JSON-serialized object with the position where the mask should be placed
-        on faces. Omit the parameter to remove the mask position."""
+        :param mask_position: A JSON-serialized object with the position where the mask should be placed \
+        on faces. Omit the parameter to remove the mask position.
+        """
 
         method_response = await self.api.request_raw(
-            "setStickerMaskPosition", get_params(locals())
+            "setStickerMaskPosition",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_set_title(
         self,
         name: str,
         title: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerSetTitle`, see the [documentation](https://core.telegram.org/bots/api#setstickersettitle)
 
-        Use this method to set the title of a created sticker set. Returns True on success.
+        Use this method to set the title of a created sticker set. Returns True on
+        success.
 
-        :param name: Sticker set name
+        :param name: Sticker set name.
 
-        :param title: Sticker set title, 1-64 characters"""
+        :param title: Sticker set title, 1-64 characters.
+        """
 
         method_response = await self.api.request_raw(
-            "setStickerSetTitle", get_params(locals())
+            "setStickerSetTitle",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: int,
-        thumbnail: InputFile | str | Option[InputFile | str] = Nothing,
+        format: str,
+        thumbnail: InputFile | str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setStickerSetThumbnail`, see the [documentation](https://core.telegram.org/bots/api#setstickersetthumbnail)
 
-        Use this method to set the thumbnail of a regular or mask sticker set. The format of the thumbnail file must match the format of the stickers in the set. Returns True on success.
-
-        :param name: Sticker set name
+        Use this method to set the thumbnail of a regular or mask sticker set. The 
+        format of the thumbnail file must match the format of the stickers in the 
+        set. Returns True on success.
+
+        :param name: Sticker set name.
+
+        :param user_id: User identifier of the sticker set owner.
+
+        :param thumbnail: A .WEBP or .PNG image with the thumbnail, must be up to 128 kilobytes in size \
+        and have a width and height of exactly 100px, or a .TGS animation with a thumbnail \
+        up to 32 kilobytes in size (see https://core.telegram.org/stickers#animated-sticker-requirements \
+        for animated sticker technical requirements), or a WEBM video with the \
+        thumbnail up to 32 kilobytes in size; see https://core.telegram.org/stickers#video-sticker-requirements \
+        for video sticker technical requirements. Pass a file_id as a String to \
+        send a file that already exists on the Telegram servers, pass an HTTP URL \
+        as a String for Telegram to get a file from the Internet, or upload a new one \
+        using multipart/form-data. More information on Sending Files: https://core.telegram.org/bots/api#sending-files. \
+        Animated and video sticker set thumbnails can't be uploaded via HTTP URL. \
+        If omitted, then the thumbnail is dropped and the first sticker is used as \
+        the thumbnail.
 
-        :param user_id: User identifier of the sticker set owner
-
-        :param thumbnail: A .WEBP or .PNG image with the thumbnail, must be up to 128 kilobytes in size
-        and have a width and height of exactly 100px, or a .TGS animation with a thumbnail
-        up to 32 kilobytes in size (see https://core.telegram.org/stickers#animated-sticker-requirements
-        for animated sticker technical requirements), or a WEBM video with the
-        thumbnail up to 32 kilobytes in size; see https://core.telegram.org/stickers#video-sticker-requirements
-        for video sticker technical requirements. Pass a file_id as a String to
-        send a file that already exists on the Telegram servers, pass an HTTP URL
-        as a String for Telegram to get a file from the Internet, or upload a new one
-        using multipart/form-data. More information on Sending Files: https://core.telegram.org/bots/api#sending-files.
-        Animated and video sticker set thumbnails can't be uploaded via HTTP URL.
-        If omitted, then the thumbnail is dropped and the first sticker is used as
-        the thumbnail."""
+        :param format: Format of the thumbnail, must be one of `static` for a .WEBP or .PNG image, \
+        `animated` for a .TGS animation, or `video` for a WEBM video.
+        """
 
         method_response = await self.api.request_raw(
-            "setStickerSetThumbnail", get_params(locals())
+            "setStickerSetThumbnail",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_custom_emoji_sticker_set_thumbnail(
         self,
         name: str,
-        custom_emoji_id: str | Option[str] = Nothing,
+        custom_emoji_id: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setCustomEmojiStickerSetThumbnail`, see the [documentation](https://core.telegram.org/bots/api#setcustomemojistickersetthumbnail)
 
-        Use this method to set the thumbnail of a custom emoji sticker set. Returns True on success.
+        Use this method to set the thumbnail of a custom emoji sticker set. Returns 
+        True on success.
 
-        :param name: Sticker set name
+        :param name: Sticker set name.
 
-        :param custom_emoji_id: Custom emoji identifier of a sticker from the sticker set; pass an empty
-        string to drop the thumbnail and use the first sticker as the thumbnail."""
+        :param custom_emoji_id: Custom emoji identifier of a sticker from the sticker set; pass an empty \
+        string to drop the thumbnail and use the first sticker as the thumbnail. \
+        """
 
         method_response = await self.api.request_raw(
-            "setCustomEmojiStickerSetThumbnail", get_params(locals())
+            "setCustomEmojiStickerSetThumbnail",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def delete_sticker_set(
         self,
         name: str,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `deleteStickerSet`, see the [documentation](https://core.telegram.org/bots/api#deletestickerset)
 
-        Use this method to delete a sticker set that was created by the bot. Returns True on success.
+        Use this method to delete a sticker set that was created by the bot. Returns
+        True on success.
 
-        :param name: Sticker set name"""
+        :param name: Sticker set name.
+        """
 
         method_response = await self.api.request_raw(
-            "deleteStickerSet", get_params(locals())
+            "deleteStickerSet",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def answer_inline_query(
         self,
         inline_query_id: str,
         results: list[InlineQueryResult],
-        cache_time: int | Option[int] = Nothing,
-        is_personal: bool | Option[bool] = Nothing,
-        next_offset: str | Option[str] = Nothing,
-        button: InlineQueryResultsButton | Option[InlineQueryResultsButton] = Nothing,
+        cache_time: int | None = None,
+        is_personal: bool | None = None,
+        next_offset: str | None = None,
+        button: InlineQueryResultsButton | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `answerInlineQuery`, see the [documentation](https://core.telegram.org/bots/api#answerinlinequery)
 
-        Use this method to send answers to an inline query. On success, True is returned.
+        Use this method to send answers to an inline query. On success, True is returned. 
         No more than 50 results per query are allowed.
 
-        :param inline_query_id: Unique identifier for the answered query
+        :param inline_query_id: Unique identifier for the answered query.
 
-        :param results: A JSON-serialized array of results for the inline query
+        :param results: A JSON-serialized array of results for the inline query.
 
-        :param cache_time: The maximum amount of time in seconds that the result of the inline query
+        :param cache_time: The maximum amount of time in seconds that the result of the inline query \
         may be cached on the server. Defaults to 300.
 
-        :param is_personal: Pass True if results may be cached on the server side only for the user that
-        sent the query. By default, results may be returned to any user who sends
+        :param is_personal: Pass True if results may be cached on the server side only for the user that \
+        sent the query. By default, results may be returned to any user who sends \
         the same query.
 
-        :param next_offset: Pass the offset that a client should send in the next query with the same text
-        to receive more results. Pass an empty string if there are no more results
-        or if you don't support pagination. Offset length can't exceed 64 bytes.
+        :param next_offset: Pass the offset that a client should send in the next query with the same text \
+        to receive more results. Pass an empty string if there are no more results \
+        or if you don't support pagination. Offset length can't exceed 64 bytes. \
 
-        :param button: A JSON-serialized object describing a button to be shown above inline query
-        results"""
+        :param button: A JSON-serialized object describing a button to be shown above inline query \
+        results.
+        """
 
         method_response = await self.api.request_raw(
-            "answerInlineQuery", get_params(locals())
+            "answerInlineQuery",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def answer_web_app_query(
         self,
         web_app_query_id: str,
         result: InlineQueryResult,
         **other: typing.Any,
-    ) -> Result[SentWebAppMessage, "APIError"]:
+    ) -> Result[SentWebAppMessage, APIError]:
         """Method `answerWebAppQuery`, see the [documentation](https://core.telegram.org/bots/api#answerwebappquery)
 
-        Use this method to set the result of an interaction with a Web App and send a corresponding message on behalf of the user to the chat from which the query originated. On success, a SentWebAppMessage object is returned.
+        Use this method to set the result of an interaction with a Web App and send
+        a corresponding message on behalf of the user to the chat from which the query
+        originated. On success, a SentWebAppMessage object is returned.
 
-        :param web_app_query_id: Unique identifier for the query to be answered
+        :param web_app_query_id: Unique identifier for the query to be answered.
 
-        :param result: A JSON-serialized object describing the message to be sent"""
+        :param result: A JSON-serialized object describing the message to be sent.
+        """
 
         method_response = await self.api.request_raw(
-            "answerWebAppQuery", get_params(locals())
+            "answerWebAppQuery",
+            get_params(locals()),
         )
         return full_result(method_response, SentWebAppMessage)
 
     async def send_invoice(
         self,
         chat_id: int | str,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: list[LabeledPrice],
-        message_thread_id: int | Option[int] = Nothing,
-        max_tip_amount: int | Option[int] = Nothing,
-        suggested_tip_amounts: list[int] | Option[list[int]] = Nothing,
-        start_parameter: str | Option[str] = Nothing,
-        provider_data: str | Option[str] = Nothing,
-        photo_url: str | Option[str] = Nothing,
-        photo_size: int | Option[int] = Nothing,
-        photo_width: int | Option[int] = Nothing,
-        photo_height: int | Option[int] = Nothing,
-        need_name: bool | Option[bool] = Nothing,
-        need_phone_number: bool | Option[bool] = Nothing,
-        need_email: bool | Option[bool] = Nothing,
-        need_shipping_address: bool | Option[bool] = Nothing,
-        send_phone_number_to_provider: bool | Option[bool] = Nothing,
-        send_email_to_provider: bool | Option[bool] = Nothing,
-        is_flexible: bool | Option[bool] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        message_thread_id: int | None = None,
+        max_tip_amount: int | None = None,
+        suggested_tip_amounts: list[int] | None = None,
+        start_parameter: str | None = None,
+        provider_data: str | None = None,
+        photo_url: str | None = None,
+        photo_size: int | None = None,
+        photo_width: int | None = None,
+        photo_height: int | None = None,
+        need_name: bool | None = None,
+        need_phone_number: bool | None = None,
+        need_email: bool | None = None,
+        need_shipping_address: bool | None = None,
+        send_phone_number_to_provider: bool | None = None,
+        send_email_to_provider: bool | None = None,
+        is_flexible: bool | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendInvoice`, see the [documentation](https://core.telegram.org/bots/api#sendinvoice)
 
         Use this method to send invoices. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat or username of the target channel
-        (in the format @channelusername)
+        :param chat_id: Unique identifier for the target chat or username of the target channel \
+        (in the format @channelusername).
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param title: Product name, 1-32 characters
+        :param title: Product name, 1-32 characters.
 
-        :param description: Product description, 1-255 characters
+        :param description: Product description, 1-255 characters.
 
-        :param payload: Bot-defined invoice payload, 1-128 bytes. This will not be displayed to
+        :param payload: Bot-defined invoice payload, 1-128 bytes. This will not be displayed to \
         the user, use for your internal processes.
 
-        :param provider_token: Payment provider token, obtained via @BotFather
+        :param provider_token: Payment provider token, obtained via @BotFather.
 
-        :param currency: Three-letter ISO 4217 currency code, see more on currencies
+        :param currency: Three-letter ISO 4217 currency code, see more on currencies.
 
-        :param prices: Price breakdown, a JSON-serialized list of components (e.g. product price,
-        tax, discount, delivery cost, delivery tax, bonus, etc.)
+        :param prices: Price breakdown, a JSON-serialized list of components (e.g. product price, \
+        tax, discount, delivery cost, delivery tax, bonus, etc.).
 
-        :param max_tip_amount: The maximum accepted amount for tips in the smallest units of the currency
-        (integer, not float/double). For example, for a maximum tip of US$ 1.45
-        pass max_tip_amount = 145. See the exp parameter in currencies.json, it
-        shows the number of digits past the decimal point for each currency (2 for
-        the majority of currencies). Defaults to 0
-
-        :param suggested_tip_amounts: A JSON-serialized array of suggested amounts of tips in the smallest units
-        of the currency (integer, not float/double). At most 4 suggested tip amounts
-        can be specified. The suggested tip amounts must be positive, passed in
+        :param max_tip_amount: The maximum accepted amount for tips in the smallest units of the currency \
+        (integer, not float/double). For example, for a maximum tip of US$ 1.45 \
+        pass max_tip_amount = 145. See the exp parameter in currencies.json, it \
+        shows the number of digits past the decimal point for each currency (2 for \
+        the majority of currencies). Defaults to 0.
+
+        :param suggested_tip_amounts: A JSON-serialized array of suggested amounts of tips in the smallest units \
+        of the currency (integer, not float/double). At most 4 suggested tip amounts \
+        can be specified. The suggested tip amounts must be positive, passed in \
         a strictly increased order and must not exceed max_tip_amount.
 
-        :param start_parameter: Unique deep-linking parameter. If left empty, forwarded copies of the
-        sent message will have a Pay button, allowing multiple users to pay directly
-        from the forwarded message, using the same invoice. If non-empty, forwarded
-        copies of the sent message will have a URL button with a deep link to the bot
-        (instead of a Pay button), with the value used as the start parameter
+        :param start_parameter: Unique deep-linking parameter. If left empty, forwarded copies of the \
+        sent message will have a Pay button, allowing multiple users to pay directly \
+        from the forwarded message, using the same invoice. If non-empty, forwarded \
+        copies of the sent message will have a URL button with a deep link to the bot \
+        (instead of a Pay button), with the value used as the start parameter.
 
-        :param provider_data: JSON-serialized data about the invoice, which will be shared with the payment
-        provider. A detailed description of required fields should be provided
+        :param provider_data: JSON-serialized data about the invoice, which will be shared with the payment \
+        provider. A detailed description of required fields should be provided \
         by the payment provider.
 
-        :param photo_url: URL of the product photo for the invoice. Can be a photo of the goods or a marketing
-        image for a service. People like it better when they see what they are paying
+        :param photo_url: URL of the product photo for the invoice. Can be a photo of the goods or a marketing \
+        image for a service. People like it better when they see what they are paying \
         for.
 
-        :param photo_size: Photo size in bytes
+        :param photo_size: Photo size in bytes.
 
-        :param photo_width: Photo width
+        :param photo_width: Photo width.
 
-        :param photo_height: Photo height
+        :param photo_height: Photo height.
 
-        :param need_name: Pass True if you require the user's full name to complete the order
+        :param need_name: Pass True if you require the user's full name to complete the order.
 
-        :param need_phone_number: Pass True if you require the user's phone number to complete the order
+        :param need_phone_number: Pass True if you require the user's phone number to complete the order.
 
-        :param need_email: Pass True if you require the user's email address to complete the order
+        :param need_email: Pass True if you require the user's email address to complete the order. \
 
-        :param need_shipping_address: Pass True if you require the user's shipping address to complete the order
+        :param need_shipping_address: Pass True if you require the user's shipping address to complete the order. \
 
-        :param send_phone_number_to_provider: Pass True if the user's phone number should be sent to provider
+        :param send_phone_number_to_provider: Pass True if the user's phone number should be sent to provider.
 
-        :param send_email_to_provider: Pass True if the user's email address should be sent to provider
+        :param send_email_to_provider: Pass True if the user's email address should be sent to provider.
 
-        :param is_flexible: Pass True if the final price depends on the shipping method
+        :param is_flexible: Pass True if the final price depends on the shipping method.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: A JSON-serialized object for an inline keyboard. If empty, one 'Pay total
-        price' button will be shown. If not empty, the first button must be a Pay button.
+        :param reply_markup: A JSON-serialized object for an inline keyboard. If empty, one 'Pay total \
+        price' button will be shown. If not empty, the first button must be a Pay button. \
         """
 
         method_response = await self.api.request_raw(
-            "sendInvoice", get_params(locals())
+            "sendInvoice",
+            get_params(locals()),
         )
         return full_result(method_response, Message)
 
     async def create_invoice_link(
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: list[LabeledPrice],
-        max_tip_amount: int | Option[int] = Nothing,
-        suggested_tip_amounts: list[int] | Option[list[int]] = Nothing,
-        provider_data: str | Option[str] = Nothing,
-        photo_url: str | Option[str] = Nothing,
-        photo_size: int | Option[int] = Nothing,
-        photo_width: int | Option[int] = Nothing,
-        photo_height: int | Option[int] = Nothing,
-        need_name: bool | Option[bool] = Nothing,
-        need_phone_number: bool | Option[bool] = Nothing,
-        need_email: bool | Option[bool] = Nothing,
-        need_shipping_address: bool | Option[bool] = Nothing,
-        send_phone_number_to_provider: bool | Option[bool] = Nothing,
-        send_email_to_provider: bool | Option[bool] = Nothing,
-        is_flexible: bool | Option[bool] = Nothing,
+        max_tip_amount: int | None = None,
+        suggested_tip_amounts: list[int] | None = None,
+        provider_data: str | None = None,
+        photo_url: str | None = None,
+        photo_size: int | None = None,
+        photo_width: int | None = None,
+        photo_height: int | None = None,
+        need_name: bool | None = None,
+        need_phone_number: bool | None = None,
+        need_email: bool | None = None,
+        need_shipping_address: bool | None = None,
+        send_phone_number_to_provider: bool | None = None,
+        send_email_to_provider: bool | None = None,
+        is_flexible: bool | None = None,
         **other: typing.Any,
-    ) -> Result[str, "APIError"]:
+    ) -> Result[str, APIError]:
         """Method `createInvoiceLink`, see the [documentation](https://core.telegram.org/bots/api#createinvoicelink)
 
-        Use this method to create a link for an invoice. Returns the created invoice link as String on success.
+        Use this method to create a link for an invoice. Returns the created invoice 
+        link as String on success.
 
-        :param title: Product name, 1-32 characters
+        :param title: Product name, 1-32 characters.
 
-        :param description: Product description, 1-255 characters
+        :param description: Product description, 1-255 characters.
 
-        :param payload: Bot-defined invoice payload, 1-128 bytes. This will not be displayed to
+        :param payload: Bot-defined invoice payload, 1-128 bytes. This will not be displayed to \
         the user, use for your internal processes.
 
-        :param provider_token: Payment provider token, obtained via BotFather
+        :param provider_token: Payment provider token, obtained via BotFather.
 
-        :param currency: Three-letter ISO 4217 currency code, see more on currencies
+        :param currency: Three-letter ISO 4217 currency code, see more on currencies.
 
-        :param prices: Price breakdown, a JSON-serialized list of components (e.g. product price,
-        tax, discount, delivery cost, delivery tax, bonus, etc.)
+        :param prices: Price breakdown, a JSON-serialized list of components (e.g. product price, \
+        tax, discount, delivery cost, delivery tax, bonus, etc.).
 
-        :param max_tip_amount: The maximum accepted amount for tips in the smallest units of the currency
-        (integer, not float/double). For example, for a maximum tip of US$ 1.45
-        pass max_tip_amount = 145. See the exp parameter in currencies.json, it
-        shows the number of digits past the decimal point for each currency (2 for
-        the majority of currencies). Defaults to 0
-
-        :param suggested_tip_amounts: A JSON-serialized array of suggested amounts of tips in the smallest units
-        of the currency (integer, not float/double). At most 4 suggested tip amounts
-        can be specified. The suggested tip amounts must be positive, passed in
+        :param max_tip_amount: The maximum accepted amount for tips in the smallest units of the currency \
+        (integer, not float/double). For example, for a maximum tip of US$ 1.45 \
+        pass max_tip_amount = 145. See the exp parameter in currencies.json, it \
+        shows the number of digits past the decimal point for each currency (2 for \
+        the majority of currencies). Defaults to 0.
+
+        :param suggested_tip_amounts: A JSON-serialized array of suggested amounts of tips in the smallest units \
+        of the currency (integer, not float/double). At most 4 suggested tip amounts \
+        can be specified. The suggested tip amounts must be positive, passed in \
         a strictly increased order and must not exceed max_tip_amount.
 
-        :param provider_data: JSON-serialized data about the invoice, which will be shared with the payment
-        provider. A detailed description of required fields should be provided
+        :param provider_data: JSON-serialized data about the invoice, which will be shared with the payment \
+        provider. A detailed description of required fields should be provided \
         by the payment provider.
 
-        :param photo_url: URL of the product photo for the invoice. Can be a photo of the goods or a marketing
+        :param photo_url: URL of the product photo for the invoice. Can be a photo of the goods or a marketing \
         image for a service.
 
-        :param photo_size: Photo size in bytes
+        :param photo_size: Photo size in bytes.
 
-        :param photo_width: Photo width
+        :param photo_width: Photo width.
 
-        :param photo_height: Photo height
+        :param photo_height: Photo height.
 
-        :param need_name: Pass True if you require the user's full name to complete the order
+        :param need_name: Pass True if you require the user's full name to complete the order.
 
-        :param need_phone_number: Pass True if you require the user's phone number to complete the order
+        :param need_phone_number: Pass True if you require the user's phone number to complete the order.
 
-        :param need_email: Pass True if you require the user's email address to complete the order
+        :param need_email: Pass True if you require the user's email address to complete the order. \
 
-        :param need_shipping_address: Pass True if you require the user's shipping address to complete the order
+        :param need_shipping_address: Pass True if you require the user's shipping address to complete the order. \
 
-        :param send_phone_number_to_provider: Pass True if the user's phone number should be sent to the provider
+        :param send_phone_number_to_provider: Pass True if the user's phone number should be sent to the provider.
 
-        :param send_email_to_provider: Pass True if the user's email address should be sent to the provider
+        :param send_email_to_provider: Pass True if the user's email address should be sent to the provider.
 
-        :param is_flexible: Pass True if the final price depends on the shipping method
+        :param is_flexible: Pass True if the final price depends on the shipping method.
         """
 
         method_response = await self.api.request_raw(
-            "createInvoiceLink", get_params(locals())
+            "createInvoiceLink",
+            get_params(locals()),
         )
         return full_result(method_response, str)
 
     async def answer_shipping_query(
         self,
         shipping_query_id: str,
         ok: bool,
-        shipping_options: list[ShippingOption] | Option[list[ShippingOption]] = Nothing,
-        error_message: str | Option[str] = Nothing,
+        shipping_options: list[ShippingOption] | None = None,
+        error_message: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `answerShippingQuery`, see the [documentation](https://core.telegram.org/bots/api#answershippingquery)
 
-        If you sent an invoice requesting a shipping address and the parameter is_flexible was specified, the Bot API will send an Update with a shipping_query field to the bot. Use this method to reply to shipping queries. On success, True is returned.
-
-        :param shipping_query_id: Unique identifier for the query to be answered
-
-        :param ok: Pass True if delivery to the specified address is possible and False if there
-        are any problems (for example, if delivery to the specified address is not
-        possible)
-
-        :param shipping_options: Required if ok is True. A JSON-serialized array of available shipping options.
-
-        :param error_message: Required if ok is False. Error message in human readable form that explains
-        why it is impossible to complete the order (e.g. `Sorry, delivery to your
-        desired address is unavailable'). Telegram will display this message
-        to the user."""
+        If you sent an invoice requesting a shipping address and the parameter is_flexible 
+        was specified, the Bot API will send an Update with a shipping_query field 
+        to the bot. Use this method to reply to shipping queries. On success, True 
+        is returned.
+
+        :param shipping_query_id: Unique identifier for the query to be answered.
+
+        :param ok: Pass True if delivery to the specified address is possible and False if there \
+        are any problems (for example, if delivery to the specified address is not \
+        possible).
+
+        :param shipping_options: Required if ok is True. A JSON-serialized array of available shipping options. \
+
+        :param error_message: Required if ok is False. Error message in human readable form that explains \
+        why it is impossible to complete the order (e.g. `Sorry, delivery to your \
+        desired address is unavailable'). Telegram will display this message \
+        to the user.
+        """
 
         method_response = await self.api.request_raw(
-            "answerShippingQuery", get_params(locals())
+            "answerShippingQuery",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def answer_pre_checkout_query(
         self,
         pre_checkout_query_id: str,
         ok: bool,
-        error_message: str | Option[str] = Nothing,
+        error_message: str | None = None,
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `answerPreCheckoutQuery`, see the [documentation](https://core.telegram.org/bots/api#answerprecheckoutquery)
 
-        Once the user has confirmed their payment and shipping details, the Bot API sends the final confirmation in the form of an Update with the field pre_checkout_query. Use this method to respond to such pre-checkout queries. On success, True is returned. Note: The Bot API must receive an answer within 10 seconds after the pre-checkout query was sent.
-
-        :param pre_checkout_query_id: Unique identifier for the query to be answered
-
-        :param ok: Specify True if everything is alright (goods are available, etc.) and the
-        bot is ready to proceed with the order. Use False if there are any problems.
-
-        :param error_message: Required if ok is False. Error message in human readable form that explains
-        the reason for failure to proceed with the checkout (e.g. `Sorry, somebody
-        just bought the last of our amazing black T-shirts while you were busy filling
-        out your payment details. Please choose a different color or garment!`).
-        Telegram will display this message to the user."""
+        Once the user has confirmed their payment and shipping details, the Bot 
+        API sends the final confirmation in the form of an Update with the field pre_checkout_query. 
+        Use this method to respond to such pre-checkout queries. On success, True 
+        is returned. Note: The Bot API must receive an answer within 10 seconds after 
+        the pre-checkout query was sent.
+
+        :param pre_checkout_query_id: Unique identifier for the query to be answered.
+
+        :param ok: Specify True if everything is alright (goods are available, etc.) and the \
+        bot is ready to proceed with the order. Use False if there are any problems. \
+
+        :param error_message: Required if ok is False. Error message in human readable form that explains \
+        the reason for failure to proceed with the checkout (e.g. `Sorry, somebody \
+        just bought the last of our amazing black T-shirts while you were busy filling \
+        out your payment details. Please choose a different color or garment!`). \
+        Telegram will display this message to the user.
+        """
 
         method_response = await self.api.request_raw(
-            "answerPreCheckoutQuery", get_params(locals())
+            "answerPreCheckoutQuery",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def set_passport_data_errors(
         self,
         user_id: int,
         errors: list[PassportElementError],
         **other: typing.Any,
-    ) -> Result[bool, "APIError"]:
+    ) -> Result[bool, APIError]:
         """Method `setPassportDataErrors`, see the [documentation](https://core.telegram.org/bots/api#setpassportdataerrors)
 
-        Informs a user that some of the Telegram Passport elements they provided contains errors. The user will not be able to re-submit their Passport to you until the errors are fixed (the contents of the field for which you returned the error must change). Returns True on success.
-        Use this if the data submitted by the user doesn't satisfy the standards your service requires for any reason. For example, if a birthday date seems invalid, a submitted document is blurry, a scan shows evidence of tampering, etc. Supply some details in the error message to make sure the user knows how to correct the issues.
+        Informs a user that some of the Telegram Passport elements they provided
+        contains errors. The user will not be able to re-submit their Passport to
+        you until the errors are fixed (the contents of the field for which you returned
+        the error must change). Returns True on success. Use this if the data submitted
+        by the user doesn't satisfy the standards your service requires for any
+        reason. For example, if a birthday date seems invalid, a submitted document
+        is blurry, a scan shows evidence of tampering, etc. Supply some details
+        in the error message to make sure the user knows how to correct the issues.
 
-        :param user_id: User identifier
+        :param user_id: User identifier.
 
-        :param errors: A JSON-serialized array describing the errors"""
+        :param errors: A JSON-serialized array describing the errors.
+        """
 
         method_response = await self.api.request_raw(
-            "setPassportDataErrors", get_params(locals())
+            "setPassportDataErrors",
+            get_params(locals()),
         )
         return full_result(method_response, bool)
 
     async def send_game(
         self,
         chat_id: int,
         game_short_name: str,
-        message_thread_id: int | Option[int] = Nothing,
-        disable_notification: bool | Option[bool] = Nothing,
-        protect_content: bool | Option[bool] = Nothing,
-        reply_parameters: ReplyParameters | Option[ReplyParameters] = Nothing,
-        reply_markup: InlineKeyboardMarkup | Option[InlineKeyboardMarkup] = Nothing,
+        business_connection_id: str | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        protect_content: bool | None = None,
+        reply_parameters: ReplyParameters | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **other: typing.Any,
-    ) -> Result[Message, "APIError"]:
+    ) -> Result[Message, APIError]:
         """Method `sendGame`, see the [documentation](https://core.telegram.org/bots/api#sendgame)
 
         Use this method to send a game. On success, the sent Message is returned.
 
-        :param chat_id: Unique identifier for the target chat
+        :param business_connection_id: Unique identifier of the business connection on behalf of which the message \
+        will be sent.
+
+        :param chat_id: Unique identifier for the target chat.
 
-        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for
-        forum supergroups only
+        :param message_thread_id: Unique identifier for the target message thread (topic) of the forum; for \
+        forum supergroups only.
 
-        :param game_short_name: Short name of the game, serves as the unique identifier for the game. Set
+        :param game_short_name: Short name of the game, serves as the unique identifier for the game. Set \
         up your games via @BotFather.
 
-        :param disable_notification: Sends the message silently. Users will receive a notification with no sound.
+        :param disable_notification: Sends the message silently. Users will receive a notification with no sound. \
 
-        :param protect_content: Protects the contents of the sent message from forwarding and saving
+        :param protect_content: Protects the contents of the sent message from forwarding and saving.
 
-        :param reply_parameters: Description of the message to reply to
+        :param reply_parameters: Description of the message to reply to.
 
-        :param reply_markup: A JSON-serialized object for an inline keyboard. If empty, one 'Play game_title'
-        button will be shown. If not empty, the first button must launch the game."""
+        :param reply_markup: A JSON-serialized object for an inline keyboard. If empty, one 'Play game_title' \
+        button will be shown. If not empty, the first button must launch the game. \
+        Not supported for messages sent on behalf of a business account.
+        """
 
-        method_response = await self.api.request_raw("sendGame", get_params(locals()))
+        method_response = await self.api.request_raw(
+            "sendGame",
+            get_params(locals()),
+        )
         return full_result(method_response, Message)
 
     async def set_game_score(
         self,
         user_id: int,
         score: int,
-        force: bool | Option[bool] = Nothing,
-        disable_edit_message: bool | Option[bool] = Nothing,
-        chat_id: int | Option[int] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
+        force: bool | None = None,
+        disable_edit_message: bool | None = None,
+        chat_id: int | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
         **other: typing.Any,
-    ) -> Result[Message | bool, "APIError"]:
+    ) -> Result[Variative[Message, bool], APIError]:
         """Method `setGameScore`, see the [documentation](https://core.telegram.org/bots/api#setgamescore)
 
-        Use this method to set the score of the specified user in a game message. On success, if the message is not an inline message, the Message is returned, otherwise True is returned. Returns an error, if the new score is not greater than the user's current score in the chat and force is False.
+        Use this method to set the score of the specified user in a game message. On 
+        success, if the message is not an inline message, the Message is returned, 
+        otherwise True is returned. Returns an error, if the new score is not greater 
+        than the user's current score in the chat and force is False.
 
-        :param user_id: User identifier
+        :param user_id: User identifier.
 
-        :param score: New score, must be non-negative
+        :param score: New score, must be non-negative.
 
-        :param force: Pass True if the high score is allowed to decrease. This can be useful when
-        fixing mistakes or banning cheaters
+        :param force: Pass True if the high score is allowed to decrease. This can be useful when \
+        fixing mistakes or banning cheaters.
 
-        :param disable_edit_message: Pass True if the game message should not be automatically edited to include
-        the current scoreboard
+        :param disable_edit_message: Pass True if the game message should not be automatically edited to include \
+        the current scoreboard.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat.
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the sent
-        message
+        :param message_id: Required if inline_message_id is not specified. Identifier of the sent \
+        message.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message"""
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
+        """
 
         method_response = await self.api.request_raw(
-            "setGameScore", get_params(locals())
+            "setGameScore",
+            get_params(locals()),
         )
-        return full_result(method_response, Message | bool)
+        return full_result(method_response, Variative[Message, bool])
 
     async def get_game_high_scores(
         self,
         user_id: int,
-        chat_id: int | Option[int] = Nothing,
-        message_id: int | Option[int] = Nothing,
-        inline_message_id: str | Option[str] = Nothing,
+        chat_id: int | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
         **other: typing.Any,
-    ) -> Result[list[GameHighScore], "APIError"]:
+    ) -> Result[list[GameHighScore], APIError]:
         """Method `getGameHighScores`, see the [documentation](https://core.telegram.org/bots/api#getgamehighscores)
 
-        Use this method to get data for high score tables. Will return the score of the specified user and several of their neighbors in a game. Returns an Array of GameHighScore objects.
+        Use this method to get data for high score tables. Will return the score of 
+        the specified user and several of their neighbors in a game. Returns an Array 
+        of GameHighScore objects.
 
-        :param user_id: Target user id
+        :param user_id: Target user id.
 
-        :param chat_id: Required if inline_message_id is not specified. Unique identifier for
-        the target chat
+        :param chat_id: Required if inline_message_id is not specified. Unique identifier for \
+        the target chat.
 
-        :param message_id: Required if inline_message_id is not specified. Identifier of the sent
-        message
+        :param message_id: Required if inline_message_id is not specified. Identifier of the sent \
+        message.
 
-        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the
-        inline message"""
+        :param inline_message_id: Required if chat_id and message_id are not specified. Identifier of the \
+        inline message.
+        """
 
         method_response = await self.api.request_raw(
-            "getGameHighScores", get_params(locals())
+            "getGameHighScores",
+            get_params(locals()),
         )
         return full_result(method_response, list[GameHighScore])
```

### Comparing `mubble-1.0.0/mubble/types/objects.py` & `mubble-1.1.0/mubble/types/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,105 +1,98 @@
 import typing
 
-from mubble.model import Model, Union
-from mubble.option.msgspec_option import Option
-from mubble.option.option import Nothing
-from mubble.types.enums import *
+from fntypes.co import Some, Variative
+
+from mubble.model import Model
+from mubble.msgspec_utils import Nothing, Option, datetime
+from mubble.types.enums import *  # noqa: F403
 
 
 class ReactionType(Model):
-    """Object `ReactionType`, see the [documentation](https://core.telegram.org/bots/api#reactiontype)
+    """Base object `ReactionType`, see the [documentation](https://core.telegram.org/bots/api#reactiontype).
 
     This object describes the type of a reaction. Currently, it can be one of
     - ReactionTypeEmoji
-    - ReactionTypeCustomEmoji"""
-
-    pass
+    - ReactionTypeCustomEmoji
+    """
 
 
 class PassportElementError(Model):
-    """Object `PassportElementError`, see the [documentation](https://core.telegram.org/bots/api#passportelementerror)
+    """Base object `PassportElementError`, see the [documentation](https://core.telegram.org/bots/api#passportelementerror).
 
     This object represents an error in the Telegram Passport element which was submitted that should be resolved by the user. It should be one of:
     - PassportElementErrorDataField
     - PassportElementErrorFrontSide
     - PassportElementErrorReverseSide
     - PassportElementErrorSelfie
     - PassportElementErrorFile
     - PassportElementErrorFiles
     - PassportElementErrorTranslationFile
     - PassportElementErrorTranslationFiles
-    - PassportElementErrorUnspecified"""
-
-    pass
+    - PassportElementErrorUnspecified
+    """
 
 
 class MessageOrigin(Model):
-    """Object `MessageOrigin`, see the [documentation](https://core.telegram.org/bots/api#messageorigin)
+    """Base object `MessageOrigin`, see the [documentation](https://core.telegram.org/bots/api#messageorigin).
 
     This object describes the origin of a message. It can be one of
     - MessageOriginUser
     - MessageOriginHiddenUser
     - MessageOriginChat
-    - MessageOriginChannel"""
-
-    pass
+    - MessageOriginChannel
+    """
 
 
 class MaybeInaccessibleMessage(Model):
-    """Object `MaybeInaccessibleMessage`, see the [documentation](https://core.telegram.org/bots/api#maybeinaccessiblemessage)
+    """Base object `MaybeInaccessibleMessage`, see the [documentation](https://core.telegram.org/bots/api#maybeinaccessiblemessage).
 
     This object describes a message that can be inaccessible to the bot. It can be one of
     - Message
-    - InaccessibleMessage"""
-
-    pass
+    - InaccessibleMessage
+    """
 
 
 class MenuButton(Model):
-    """Object `MenuButton`, see the [documentation](https://core.telegram.org/bots/api#menubutton)
+    """Base object `MenuButton`, see the [documentation](https://core.telegram.org/bots/api#menubutton).
 
     This object describes the bot's menu button in a private chat. It should be one of
     - MenuButtonCommands
     - MenuButtonWebApp
     - MenuButtonDefault
     If a menu button other than MenuButtonDefault is set for a private chat, then it is applied in the chat. Otherwise the default menu button is applied. By default, the menu button opens the list of bot commands.
     """
 
-    pass
-
 
 class InputMessageContent(Model):
-    """Object `InputMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputmessagecontent)
+    """Base object `InputMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputmessagecontent).
 
     This object represents the content of a message to be sent as a result of an inline query. Telegram clients currently support the following 5 types:
     - InputTextMessageContent
     - InputLocationMessageContent
     - InputVenueMessageContent
     - InputContactMessageContent
-    - InputInvoiceMessageContent"""
-
-    pass
+    - InputInvoiceMessageContent
+    """
 
 
 class InputMedia(Model):
-    """Object `InputMedia`, see the [documentation](https://core.telegram.org/bots/api#inputmedia)
+    """Base object `InputMedia`, see the [documentation](https://core.telegram.org/bots/api#inputmedia).
 
     This object represents the content of a media message to be sent. It should be one of
     - InputMediaAnimation
     - InputMediaDocument
     - InputMediaAudio
     - InputMediaPhoto
-    - InputMediaVideo"""
-
-    pass
+    - InputMediaVideo
+    """
 
 
 class InlineQueryResult(Model):
-    """Object `InlineQueryResult`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresult)
+    """Base object `InlineQueryResult`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresult).
 
     This object represents one result of an inline query. Telegram clients currently support results of the following 20 types:
     - InlineQueryResultCachedAudio
     - InlineQueryResultCachedDocument
     - InlineQueryResultCachedGif
     - InlineQueryResultCachedMpeg4Gif
     - InlineQueryResultCachedPhoto
@@ -117,62 +110,58 @@
     - InlineQueryResultPhoto
     - InlineQueryResultVenue
     - InlineQueryResultVideo
     - InlineQueryResultVoice
     Note: All URLs passed in inline query results will be available to end users and therefore must be assumed to be public.
     """
 
-    pass
-
 
 class ChatMember(Model):
-    """Object `ChatMember`, see the [documentation](https://core.telegram.org/bots/api#chatmember)
+    """Base object `ChatMember`, see the [documentation](https://core.telegram.org/bots/api#chatmember).
 
     This object contains information about one member of a chat. Currently, the following 6 types of chat members are supported:
     - ChatMemberOwner
     - ChatMemberAdministrator
     - ChatMemberMember
     - ChatMemberRestricted
     - ChatMemberLeft
-    - ChatMemberBanned"""
-
-    pass
+    - ChatMemberBanned
+    """
 
 
 class ChatBoostSource(Model):
-    """Object `ChatBoostSource`, see the [documentation](https://core.telegram.org/bots/api#chatboostsource)
+    """Base object `ChatBoostSource`, see the [documentation](https://core.telegram.org/bots/api#chatboostsource).
 
     This object describes the source of a chat boost. It can be one of
     - ChatBoostSourcePremium
     - ChatBoostSourceGiftCode
-    - ChatBoostSourceGiveaway"""
-
-    pass
+    - ChatBoostSourceGiveaway
+    """
 
 
 class BotCommandScope(Model):
-    """Object `BotCommandScope`, see the [documentation](https://core.telegram.org/bots/api#botcommandscope)
+    """Base object `BotCommandScope`, see the [documentation](https://core.telegram.org/bots/api#botcommandscope).
 
     This object represents the scope to which bot commands are applied. Currently, the following 7 scopes are supported:
     - BotCommandScopeDefault
     - BotCommandScopeAllPrivateChats
     - BotCommandScopeAllGroupChats
     - BotCommandScopeAllChatAdministrators
     - BotCommandScopeChat
     - BotCommandScopeChatAdministrators
-    - BotCommandScopeChatMember"""
-
-    pass
+    - BotCommandScopeChatMember
+    """
 
 
 class Update(Model):
-    """Object `Update`, see the [documentation](https://core.telegram.org/bots/api#update)
+    """Object `Update`, see the [documentation](https://core.telegram.org/bots/api#update).
 
     This object represents an incoming update.
-    At most one of the optional parameters can be present in any given update."""
+    At most one of the optional parameters can be present in any given update.
+    """
 
     update_id: int
     """The update's unique identifier. Update identifiers start from a certain 
     positive number and increase sequentially. This identifier becomes especially 
     handy if you're using webhooks, since it allows you to ignore repeated updates 
     or to restore the correct update sequence, should they get out of order. 
     If there are no new updates for at least a week, then identifier of the next 
@@ -191,48 +180,61 @@
     etc."""
 
     edited_channel_post: Option["Message"] = Nothing
     """Optional. New version of a channel post that is known to the bot and was edited. 
     This update may at times be triggered by changes to message fields that are 
     either unavailable or not actively used by your bot."""
 
+    business_connection: Option["BusinessConnection"] = Nothing
+    """Optional. The bot was connected to or disconnected from a business account, 
+    or a user edited an existing connection with the bot."""
+
+    business_message: Option["Message"] = Nothing
+    """Optional. New non-service message from a connected business account."""
+
+    edited_business_message: Option["Message"] = Nothing
+    """Optional. New version of a message from a connected business account."""
+
+    deleted_business_messages: Option["BusinessMessagesDeleted"] = Nothing
+    """Optional. Messages were deleted from a connected business account."""
+
     message_reaction: Option["MessageReactionUpdated"] = Nothing
     """Optional. A reaction to a message was changed by a user. The bot must be an 
     administrator in the chat and must explicitly specify `message_reaction` 
     in the list of allowed_updates to receive these updates. The update isn't 
     received for reactions set by bots."""
 
     message_reaction_count: Option["MessageReactionCountUpdated"] = Nothing
     """Optional. Reactions to a message with anonymous reactions were changed. 
     The bot must be an administrator in the chat and must explicitly specify 
     `message_reaction_count` in the list of allowed_updates to receive these 
     updates. The updates are grouped and can be sent with delay up to a few minutes."""
 
     inline_query: Option["InlineQuery"] = Nothing
-    """Optional. New incoming inline query"""
+    """Optional. New incoming inline query."""
 
     chosen_inline_result: Option["ChosenInlineResult"] = Nothing
     """Optional. The result of an inline query that was chosen by a user and sent 
     to their chat partner. Please see our documentation on the feedback collecting 
     for details on how to enable these updates for your bot."""
 
     callback_query: Option["CallbackQuery"] = Nothing
-    """Optional. New incoming callback query"""
+    """Optional. New incoming callback query."""
 
     shipping_query: Option["ShippingQuery"] = Nothing
     """Optional. New incoming shipping query. Only for invoices with flexible 
-    price"""
+    price."""
 
     pre_checkout_query: Option["PreCheckoutQuery"] = Nothing
     """Optional. New incoming pre-checkout query. Contains full information 
-    about checkout"""
+    about checkout."""
 
     poll: Option["Poll"] = Nothing
     """Optional. New poll state. Bots receive only updates about manually stopped 
-    polls and polls, which are sent by the bot"""
+    polls and polls, which are sent by the bot."""
 
     poll_answer: Option["PollAnswer"] = Nothing
     """Optional. A user changed their answer in a non-anonymous poll. Bots receive 
     new votes only in polls that were sent by the bot itself."""
 
     my_chat_member: Option["ChatMemberUpdated"] = Nothing
     """Optional. The bot's chat member status was updated in a chat. For private 
@@ -252,139 +254,188 @@
     """Optional. A chat boost was added or changed. The bot must be an administrator 
     in the chat to receive these updates."""
 
     removed_chat_boost: Option["ChatBoostRemoved"] = Nothing
     """Optional. A boost was removed from a chat. The bot must be an administrator 
     in the chat to receive these updates."""
 
+    @property
+    def update_type(self) -> Option[UpdateType]:
+        """Incoming update type."""
+
+        if update := next(
+            filter(
+                lambda x: bool(x[1]),
+                self.to_dict(exclude_fields={"update_id"}).items(),
+            ),
+            None,
+        ):
+            return Some(UpdateType(update[0]))
+        return Nothing
+
 
 class WebhookInfo(Model):
-    """Object `WebhookInfo`, see the [documentation](https://core.telegram.org/bots/api#webhookinfo)
+    """Object `WebhookInfo`, see the [documentation](https://core.telegram.org/bots/api#webhookinfo).
 
-    Describes the current status of a webhook."""
+    Describes the current status of a webhook.
+    """
 
     url: str
-    """Webhook URL, may be empty if webhook is not set up"""
+    """Webhook URL, may be empty if webhook is not set up."""
 
     has_custom_certificate: bool
-    """True, if a custom certificate was provided for webhook certificate checks"""
+    """True, if a custom certificate was provided for webhook certificate checks."""
 
     pending_update_count: int
-    """Number of updates awaiting delivery"""
+    """Number of updates awaiting delivery."""
 
     ip_address: Option[str] = Nothing
-    """Optional. Currently used webhook IP address"""
+    """Optional. Currently used webhook IP address."""
 
-    last_error_date: Option[int] = Nothing
+    last_error_date: Option[datetime] = Nothing
     """Optional. Unix time for the most recent error that happened when trying 
-    to deliver an update via webhook"""
+    to deliver an update via webhook."""
 
     last_error_message: Option[str] = Nothing
     """Optional. Error message in human-readable format for the most recent error 
-    that happened when trying to deliver an update via webhook"""
+    that happened when trying to deliver an update via webhook."""
 
-    last_synchronization_error_date: Option[int] = Nothing
+    last_synchronization_error_date: Option[datetime] = Nothing
     """Optional. Unix time of the most recent error that happened when trying to 
-    synchronize available updates with Telegram datacenters"""
+    synchronize available updates with Telegram datacenters."""
 
     max_connections: Option[int] = Nothing
     """Optional. The maximum allowed number of simultaneous HTTPS connections 
-    to the webhook for update delivery"""
+    to the webhook for update delivery."""
 
     allowed_updates: Option[list[str]] = Nothing
     """Optional. A list of update types the bot is subscribed to. Defaults to all 
-    update types except chat_member"""
+    update types except chat_member."""
 
 
 class User(Model):
-    """Object `User`, see the [documentation](https://core.telegram.org/bots/api#user)
+    """Object `User`, see the [documentation](https://core.telegram.org/bots/api#user).
 
-    This object represents a Telegram user or bot."""
+    This object represents a Telegram user or bot.
+    """
 
     id: int
     """Unique identifier for this user or bot. This number may have more than 32 
     significant bits and some programming languages may have difficulty/silent 
     defects in interpreting it. But it has at most 52 significant bits, so a 64-bit 
     integer or double-precision float type are safe for storing this identifier."""
 
     is_bot: bool
-    """True, if this user is a bot"""
+    """True, if this user is a bot."""
 
     first_name: str
-    """User's or bot's first name"""
+    """User's or bot's first name."""
 
     last_name: Option[str] = Nothing
-    """Optional. User's or bot's last name"""
+    """Optional. User's or bot's last name."""
 
     username: Option[str] = Nothing
-    """Optional. User's or bot's username"""
+    """Optional. User's or bot's username."""
 
     language_code: Option[str] = Nothing
-    """Optional. IETF language tag of the user's language"""
+    """Optional. IETF language tag of the user's language."""
 
     is_premium: Option[bool] = Nothing
-    """Optional. True, if this user is a Telegram Premium user"""
+    """Optional. True, if this user is a Telegram Premium user."""
 
     added_to_attachment_menu: Option[bool] = Nothing
-    """Optional. True, if this user added the bot to the attachment menu"""
+    """Optional. True, if this user added the bot to the attachment menu."""
 
     can_join_groups: Option[bool] = Nothing
     """Optional. True, if the bot can be invited to groups. Returned only in getMe."""
 
     can_read_all_group_messages: Option[bool] = Nothing
     """Optional. True, if privacy mode is disabled for the bot. Returned only in 
     getMe."""
 
     supports_inline_queries: Option[bool] = Nothing
     """Optional. True, if the bot supports inline queries. Returned only in getMe."""
 
+    can_connect_to_business: Option[bool] = Nothing
+    """Optional. True, if the bot can be connected to a Telegram Business account 
+    to receive its messages. Returned only in getMe."""
+
+    @property
+    def default_accent_color(self) -> DefaultAccentColor:
+        """User's or bot's accent color (non-premium)."""
+
+        return DefaultAccentColor(self.id % 7)
+
     @property
     def full_name(self) -> str:
-        """User's or bot's `first_name` + `last_name`."""
+        """User's or bot's full name (`first_name` + `last_name`)."""
 
         return self.first_name + self.last_name.map(lambda v: " " + v).unwrap_or("")
 
 
 class Chat(Model):
-    """Object `Chat`, see the [documentation](https://core.telegram.org/bots/api#chat)
+    """Object `Chat`, see the [documentation](https://core.telegram.org/bots/api#chat).
 
-    This object represents a chat."""
+    This object represents a chat.
+    """
 
     id: int
     """Unique identifier for this chat. This number may have more than 32 significant 
     bits and some programming languages may have difficulty/silent defects 
     in interpreting it. But it has at most 52 significant bits, so a signed 64-bit 
     integer or double-precision float type are safe for storing this identifier."""
 
     type: ChatType
-    """Type of chat, can be either `private`, `group`, `supergroup` or `channel`"""
+    """Type of chat, can be either `private`, `group`, `supergroup` or `channel`."""
 
     title: Option[str] = Nothing
-    """Optional. Title, for supergroups, channels and group chats"""
+    """Optional. Title, for supergroups, channels and group chats."""
 
     username: Option[str] = Nothing
-    """Optional. Username, for private chats, supergroups and channels if available"""
+    """Optional. Username, for private chats, supergroups and channels if available."""
 
     first_name: Option[str] = Nothing
-    """Optional. First name of the other party in a private chat"""
+    """Optional. First name of the other party in a private chat."""
 
     last_name: Option[str] = Nothing
-    """Optional. Last name of the other party in a private chat"""
+    """Optional. Last name of the other party in a private chat."""
 
     is_forum: Option[bool] = Nothing
-    """Optional. True, if the supergroup chat is a forum (has topics enabled)"""
+    """Optional. True, if the supergroup chat is a forum (has topics enabled)."""
 
     photo: Option["ChatPhoto"] = Nothing
     """Optional. Chat photo. Returned only in getChat."""
 
     active_usernames: Option[list[str]] = Nothing
     """Optional. If non-empty, the list of all active chat usernames; for private 
     chats, supergroups and channels. Returned only in getChat."""
 
-    available_reactions: Option[list["ReactionType"]] = Nothing
+    birthdate: Option["Birthdate"] = Nothing
+    """Optional. For private chats, the date of birth of the user. Returned only 
+    in getChat."""
+
+    business_intro: Option["BusinessIntro"] = Nothing
+    """Optional. For private chats with business accounts, the intro of the business. 
+    Returned only in getChat."""
+
+    business_location: Option["BusinessLocation"] = Nothing
+    """Optional. For private chats with business accounts, the location of the 
+    business. Returned only in getChat."""
+
+    business_opening_hours: Option["BusinessOpeningHours"] = Nothing
+    """Optional. For private chats with business accounts, the opening hours 
+    of the business. Returned only in getChat."""
+
+    personal_chat: Option["Chat"] = Nothing
+    """Optional. For private chats, the personal channel of the user. Returned 
+    only in getChat."""
+
+    available_reactions: Option[
+        list[Variative["ReactionTypeEmoji", "ReactionTypeCustomEmoji"]]
+    ] = Nothing
     """Optional. List of available reactions allowed in the chat. If omitted, 
     then all emoji reactions are allowed. Returned only in getChat."""
 
     accent_color_id: Option[int] = Nothing
     """Optional. Identifier of the accent color for the chat name and backgrounds 
     of the chat photo, reply header, and link preview. See accent colors for 
     more details. Returned only in getChat. Always returned in getChat."""
@@ -401,15 +452,15 @@
     """Optional. Custom emoji identifier of the emoji chosen by the chat for its 
     profile background. Returned only in getChat."""
 
     emoji_status_custom_emoji_id: Option[str] = Nothing
     """Optional. Custom emoji identifier of the emoji status of the chat or the 
     other party in a private chat. Returned only in getChat."""
 
-    emoji_status_expiration_date: Option[int] = Nothing
+    emoji_status_expiration_date: Option[datetime] = Nothing
     """Optional. Expiration date of the emoji status of the chat or the other party 
     in a private chat, in Unix time, if any. Returned only in getChat."""
 
     bio: Option[str] = Nothing
     """Optional. Bio of the other party in a private chat. Returned only in getChat."""
 
     has_private_forwards: Option[bool] = Nothing
@@ -443,16 +494,20 @@
 
     permissions: Option["ChatPermissions"] = Nothing
     """Optional. Default chat member permissions, for groups and supergroups. 
     Returned only in getChat."""
 
     slow_mode_delay: Option[int] = Nothing
     """Optional. For supergroups, the minimum allowed delay between consecutive 
-    messages sent by each unpriviledged user; in seconds. Returned only in 
-    getChat."""
+    messages sent by each unprivileged user; in seconds. Returned only in getChat."""
+
+    unrestrict_boost_count: Option[int] = Nothing
+    """Optional. For supergroups, the minimum number of boosts that a non-administrator 
+    user needs to add in order to ignore slow mode and chat permissions. Returned 
+    only in getChat."""
 
     message_auto_delete_time: Option[int] = Nothing
     """Optional. The time after which all messages sent to the chat will be automatically 
     deleted; in seconds. Returned only in getChat."""
 
     has_aggressive_anti_spam_enabled: Option[bool] = Nothing
     """Optional. True, if aggressive anti-spam checks are enabled in the supergroup. 
@@ -474,196 +529,231 @@
     """Optional. For supergroups, name of group sticker set. Returned only in 
     getChat."""
 
     can_set_sticker_set: Option[bool] = Nothing
     """Optional. True, if the bot can change the group sticker set. Returned only 
     in getChat."""
 
+    custom_emoji_sticker_set_name: Option[str] = Nothing
+    """Optional. For supergroups, the name of the group's custom emoji sticker 
+    set. Custom emoji from this set can be used by all users and bots in the group. 
+    Returned only in getChat."""
+
     linked_chat_id: Option[int] = Nothing
     """Optional. Unique identifier for the linked chat, i.e. the discussion group 
     identifier for a channel and vice versa; for supergroups and channel chats. 
     This identifier may be greater than 32 bits and some programming languages 
     may have difficulty/silent defects in interpreting it. But it is smaller 
     than 52 bits, so a signed 64 bit integer or double-precision float type are 
     safe for storing this identifier. Returned only in getChat."""
 
     location: Option["ChatLocation"] = Nothing
     """Optional. For supergroups, the location to which the supergroup is connected. 
     Returned only in getChat."""
 
+    @property
+    def full_name(self) -> Option[str]:
+        """Optional. Full name (`first_name` + `last_name`) of the
+        other party in a `private` chat."""
+
+        return self.first_name.map(lambda x: x + " " + self.last_name.unwrap_or(""))
+
 
 class Message(MaybeInaccessibleMessage):
-    """Object `Message`, see the [documentation](https://core.telegram.org/bots/api#message)
+    """Object `Message`, see the [documentation](https://core.telegram.org/bots/api#message).
 
-    This object represents a message."""
+    This object represents a message.
+    """
 
     message_id: int
-    """Unique message identifier inside this chat"""
+    """Unique message identifier inside this chat."""
 
-    date: int
+    date: datetime
     """Date the message was sent in Unix time. It is always a positive number, representing 
     a valid date."""
 
     chat: "Chat"
-    """Chat the message belongs to"""
+    """Chat the message belongs to."""
 
     message_thread_id: Option[int] = Nothing
     """Optional. Unique identifier of a message thread to which the message belongs; 
-    for supergroups only"""
+    for supergroups only."""
 
     from_: Option["User"] = Nothing
     """Optional. Sender of the message; empty for messages sent to channels. For 
     backward compatibility, the field contains a fake sender user in non-channel 
     chats, if the message was sent on behalf of a chat."""
 
     sender_chat: Option["Chat"] = Nothing
     """Optional. Sender of the message, sent on behalf of a chat. For example, the 
     channel itself for channel posts, the supergroup itself for messages from 
     anonymous group administrators, the linked channel for messages automatically 
     forwarded to the discussion group. For backward compatibility, the field 
     from contains a fake sender user in non-channel chats, if the message was 
     sent on behalf of a chat."""
 
+    sender_boost_count: Option[int] = Nothing
+    """Optional. If the sender of the message boosted the chat, the number of boosts 
+    added by the user."""
+
+    sender_business_bot: Option["User"] = Nothing
+    """Optional. The bot that actually sent the message on behalf of the business 
+    account. Available only for outgoing messages sent on behalf of the connected 
+    business account."""
+
+    business_connection_id: Option[str] = Nothing
+    """Optional. Unique identifier of the business connection from which the 
+    message was received. If non-empty, the message belongs to a chat of the 
+    corresponding business account that is independent from any potential 
+    bot chat which might share the same identifier."""
+
     forward_origin: Option[
-        Union[
+        Variative[
             "MessageOriginUser",
             "MessageOriginHiddenUser",
             "MessageOriginChat",
             "MessageOriginChannel",
         ]
     ] = Nothing
-    """Optional. Information about the original message for forwarded messages"""
+    """Optional. Information about the original message for forwarded messages."""
 
     is_topic_message: Option[bool] = Nothing
-    """Optional. True, if the message is sent to a forum topic"""
+    """Optional. True, if the message is sent to a forum topic."""
 
     is_automatic_forward: Option[bool] = Nothing
     """Optional. True, if the message is a channel post that was automatically 
-    forwarded to the connected discussion group"""
+    forwarded to the connected discussion group."""
 
     reply_to_message: Option["Message"] = Nothing
     """Optional. For replies in the same chat and message thread, the original 
     message. Note that the Message object in this field will not contain further 
     reply_to_message fields even if it itself is a reply."""
 
     external_reply: Option["ExternalReplyInfo"] = Nothing
     """Optional. Information about the message that is being replied to, which 
-    may come from another chat or forum topic"""
+    may come from another chat or forum topic."""
 
     quote: Option["TextQuote"] = Nothing
     """Optional. For replies that quote part of the original message, the quoted 
-    part of the message"""
+    part of the message."""
+
+    reply_to_story: Option["Story"] = Nothing
+    """Optional. For replies to a story, the original story."""
 
     via_bot: Option["User"] = Nothing
-    """Optional. Bot through which the message was sent"""
+    """Optional. Bot through which the message was sent."""
 
-    edit_date: Option[int] = Nothing
-    """Optional. Date the message was last edited in Unix time"""
+    edit_date: Option[datetime] = Nothing
+    """Optional. Date the message was last edited in Unix time."""
 
     has_protected_content: Option[bool] = Nothing
-    """Optional. True, if the message can't be forwarded"""
+    """Optional. True, if the message can't be forwarded."""
+
+    is_from_offline: Option[bool] = Nothing
+    """Optional. True, if the message was sent by an implicit action, for example, 
+    as an away or a greeting business message, or as a scheduled message."""
 
     media_group_id: Option[str] = Nothing
     """Optional. The unique identifier of a media message group this message belongs 
-    to"""
+    to."""
 
     author_signature: Option[str] = Nothing
     """Optional. Signature of the post author for messages in channels, or the 
-    custom title of an anonymous group administrator"""
+    custom title of an anonymous group administrator."""
 
     text: Option[str] = Nothing
-    """Optional. For text messages, the actual UTF-8 text of the message"""
+    """Optional. For text messages, the actual UTF-8 text of the message."""
 
     entities: Option[list["MessageEntity"]] = Nothing
     """Optional. For text messages, special entities like usernames, URLs, bot 
-    commands, etc. that appear in the text"""
+    commands, etc. that appear in the text."""
 
     link_preview_options: Option["LinkPreviewOptions"] = Nothing
     """Optional. Options used for link preview generation for the message, if 
-    it is a text message and link preview options were changed"""
+    it is a text message and link preview options were changed."""
 
     animation: Option["Animation"] = Nothing
     """Optional. Message is an animation, information about the animation. For 
     backward compatibility, when this field is set, the document field will 
-    also be set"""
+    also be set."""
 
     audio: Option["Audio"] = Nothing
-    """Optional. Message is an audio file, information about the file"""
+    """Optional. Message is an audio file, information about the file."""
 
     document: Option["Document"] = Nothing
-    """Optional. Message is a general file, information about the file"""
+    """Optional. Message is a general file, information about the file."""
 
     photo: Option[list["PhotoSize"]] = Nothing
-    """Optional. Message is a photo, available sizes of the photo"""
+    """Optional. Message is a photo, available sizes of the photo."""
 
     sticker: Option["Sticker"] = Nothing
-    """Optional. Message is a sticker, information about the sticker"""
+    """Optional. Message is a sticker, information about the sticker."""
 
     story: Option["Story"] = Nothing
-    """Optional. Message is a forwarded story"""
+    """Optional. Message is a forwarded story."""
 
     video: Option["Video"] = Nothing
-    """Optional. Message is a video, information about the video"""
+    """Optional. Message is a video, information about the video."""
 
     video_note: Option["VideoNote"] = Nothing
-    """Optional. Message is a video note, information about the video message"""
+    """Optional. Message is a video note, information about the video message."""
 
     voice: Option["Voice"] = Nothing
-    """Optional. Message is a voice message, information about the file"""
+    """Optional. Message is a voice message, information about the file."""
 
     caption: Option[str] = Nothing
     """Optional. Caption for the animation, audio, document, photo, video or 
-    voice"""
+    voice."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. For messages with a caption, special entities like usernames, 
-    URLs, bot commands, etc. that appear in the caption"""
+    URLs, bot commands, etc. that appear in the caption."""
 
     has_media_spoiler: Option[bool] = Nothing
-    """Optional. True, if the message media is covered by a spoiler animation"""
+    """Optional. True, if the message media is covered by a spoiler animation."""
 
     contact: Option["Contact"] = Nothing
-    """Optional. Message is a shared contact, information about the contact"""
+    """Optional. Message is a shared contact, information about the contact."""
 
     dice: Option["Dice"] = Nothing
-    """Optional. Message is a dice with random value"""
+    """Optional. Message is a dice with random value."""
 
     game: Option["Game"] = Nothing
     """Optional. Message is a game, information about the game. More about games: 
-    https://core.telegram.org/bots/api#games"""
+    https://core.telegram.org/bots/api#games."""
 
     poll: Option["Poll"] = Nothing
-    """Optional. Message is a native poll, information about the poll"""
+    """Optional. Message is a native poll, information about the poll."""
 
     venue: Option["Venue"] = Nothing
     """Optional. Message is a venue, information about the venue. For backward 
-    compatibility, when this field is set, the location field will also be set"""
+    compatibility, when this field is set, the location field will also be set."""
 
     location: Option["Location"] = Nothing
-    """Optional. Message is a shared location, information about the location"""
+    """Optional. Message is a shared location, information about the location."""
 
     new_chat_members: Option[list["User"]] = Nothing
     """Optional. New members that were added to the group or supergroup and information 
-    about them (the bot itself may be one of these members)"""
+    about them (the bot itself may be one of these members)."""
 
     left_chat_member: Option["User"] = Nothing
     """Optional. A member was removed from the group, information about them (this 
-    member may be the bot itself)"""
+    member may be the bot itself)."""
 
     new_chat_title: Option[str] = Nothing
-    """Optional. A chat title was changed to this value"""
+    """Optional. A chat title was changed to this value."""
 
     new_chat_photo: Option[list["PhotoSize"]] = Nothing
-    """Optional. A chat photo was change to this value"""
+    """Optional. A chat photo was change to this value."""
 
     delete_chat_photo: Option[bool] = Nothing
-    """Optional. Service message: the chat photo was deleted"""
+    """Optional. Service message: the chat photo was deleted."""
 
     group_chat_created: Option[bool] = Nothing
-    """Optional. Service message: the group has been created"""
+    """Optional. Service message: the group has been created."""
 
     supergroup_chat_created: Option[bool] = Nothing
     """Optional. Service message: the supergroup has been created. This field 
     can't be received in a message coming through updates, because bot can't 
     be a member of a supergroup when it is created. It can only be found in reply_to_message 
     if someone replies to a very first message in a directly created supergroup."""
 
@@ -671,15 +761,15 @@
     """Optional. Service message: the channel has been created. This field can't 
     be received in a message coming through updates, because bot can't be a member 
     of a channel when it is created. It can only be found in reply_to_message 
     if someone replies to a very first message in a channel."""
 
     message_auto_delete_timer_changed: Option["MessageAutoDeleteTimerChanged"] = Nothing
     """Optional. Service message: auto-delete timer settings changed in the 
-    chat"""
+    chat."""
 
     migrate_to_chat_id: Option[int] = Nothing
     """Optional. The group has been migrated to a supergroup with the specified 
     identifier. This number may have more than 32 significant bits and some 
     programming languages may have difficulty/silent defects in interpreting 
     it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this identifier."""
@@ -687,93 +777,96 @@
     migrate_from_chat_id: Option[int] = Nothing
     """Optional. The supergroup has been migrated from a group with the specified 
     identifier. This number may have more than 32 significant bits and some 
     programming languages may have difficulty/silent defects in interpreting 
     it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this identifier."""
 
-    pinned_message: Option[Union["Message", "InaccessibleMessage"]] = Nothing
+    pinned_message: Option[Variative["Message", "InaccessibleMessage"]] = Nothing
     """Optional. Specified message was pinned. Note that the Message object in 
     this field will not contain further reply_to_message fields even if it 
     itself is a reply."""
 
     invoice: Option["Invoice"] = Nothing
     """Optional. Message is an invoice for a payment, information about the invoice. 
-    More about payments: https://core.telegram.org/bots/api#payments"""
+    More about payments: https://core.telegram.org/bots/api#payments."""
 
     successful_payment: Option["SuccessfulPayment"] = Nothing
     """Optional. Message is a service message about a successful payment, information 
-    about the payment. More about payments: https://core.telegram.org/bots/api#payments"""
+    about the payment. More about payments: https://core.telegram.org/bots/api#payments."""
 
     users_shared: Option["UsersShared"] = Nothing
-    """Optional. Service message: users were shared with the bot"""
+    """Optional. Service message: users were shared with the bot."""
 
     chat_shared: Option["ChatShared"] = Nothing
-    """Optional. Service message: a chat was shared with the bot"""
+    """Optional. Service message: a chat was shared with the bot."""
 
     connected_website: Option[str] = Nothing
     """Optional. The domain name of the website on which the user has logged in. 
-    More about Telegram Login: https://core.telegram.org/widgets/login"""
+    More about Telegram Login: https://core.telegram.org/widgets/login."""
 
     write_access_allowed: Option["WriteAccessAllowed"] = Nothing
     """Optional. Service message: the user allowed the bot to write messages after 
     adding it to the attachment or side menu, launching a Web App from a link, 
-    or accepting an explicit request from a Web App sent by the method requestWriteAccess"""
+    or accepting an explicit request from a Web App sent by the method requestWriteAccess."""
 
     passport_data: Option["PassportData"] = Nothing
-    """Optional. Telegram Passport data"""
+    """Optional. Telegram Passport data."""
 
     proximity_alert_triggered: Option["ProximityAlertTriggered"] = Nothing
     """Optional. Service message. A user in the chat triggered another user's 
     proximity alert while sharing Live Location."""
 
+    boost_added: Option["ChatBoostAdded"] = Nothing
+    """Optional. Service message: user boosted the chat."""
+
     forum_topic_created: Option["ForumTopicCreated"] = Nothing
-    """Optional. Service message: forum topic created"""
+    """Optional. Service message: forum topic created."""
 
     forum_topic_edited: Option["ForumTopicEdited"] = Nothing
-    """Optional. Service message: forum topic edited"""
+    """Optional. Service message: forum topic edited."""
 
     forum_topic_closed: Option["ForumTopicClosed"] = Nothing
-    """Optional. Service message: forum topic closed"""
+    """Optional. Service message: forum topic closed."""
 
     forum_topic_reopened: Option["ForumTopicReopened"] = Nothing
-    """Optional. Service message: forum topic reopened"""
+    """Optional. Service message: forum topic reopened."""
 
     general_forum_topic_hidden: Option["GeneralForumTopicHidden"] = Nothing
-    """Optional. Service message: the 'General' forum topic hidden"""
+    """Optional. Service message: the 'General' forum topic hidden."""
 
     general_forum_topic_unhidden: Option["GeneralForumTopicUnhidden"] = Nothing
-    """Optional. Service message: the 'General' forum topic unhidden"""
+    """Optional. Service message: the 'General' forum topic unhidden."""
 
     giveaway_created: Option["GiveawayCreated"] = Nothing
-    """Optional. Service message: a scheduled giveaway was created"""
+    """Optional. Service message: a scheduled giveaway was created."""
 
     giveaway: Option["Giveaway"] = Nothing
-    """Optional. The message is a scheduled giveaway message"""
+    """Optional. The message is a scheduled giveaway message."""
 
     giveaway_winners: Option["GiveawayWinners"] = Nothing
-    """Optional. A giveaway with public winners was completed"""
+    """Optional. A giveaway with public winners was completed."""
 
     giveaway_completed: Option["GiveawayCompleted"] = Nothing
-    """Optional. Service message: a giveaway without public winners was completed"""
+    """Optional. Service message: a giveaway without public winners was completed."""
 
     video_chat_scheduled: Option["VideoChatScheduled"] = Nothing
-    """Optional. Service message: video chat scheduled"""
+    """Optional. Service message: video chat scheduled."""
 
     video_chat_started: Option["VideoChatStarted"] = Nothing
-    """Optional. Service message: video chat started"""
+    """Optional. Service message: video chat started."""
 
     video_chat_ended: Option["VideoChatEnded"] = Nothing
-    """Optional. Service message: video chat ended"""
+    """Optional. Service message: video chat ended."""
 
     video_chat_participants_invited: Option["VideoChatParticipantsInvited"] = Nothing
-    """Optional. Service message: new participants invited to a video chat"""
+    """Optional. Service message: new participants invited to a video chat."""
 
     web_app_data: Option["WebAppData"] = Nothing
-    """Optional. Service message: data sent by a Web App"""
+    """Optional. Service message: data sent by a Web App."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
     """Optional. Inline keyboard attached to the message. login_url buttons 
     are represented as ordinary url buttons."""
 
     @property
     def content_type(self) -> ContentType:
@@ -785,212 +878,236 @@
                 and getattr(self, content.value, Nothing) is not Nothing
             ):
                 return content
         return ContentType.UNKNOWN
 
     @property
     def from_user(self) -> "User":
-        """`from_user` instead of `from_.unwrap()`"""
+        """`from_user` instead of `from_.unwrap()`."""
 
         return self.from_.unwrap()
 
-    def __eq__(self, other: "Message") -> bool:
-        return self.message_id == other.message_id and self.chat.id == other.chat.id
+    @property
+    def chat_id(self) -> int:
+        """`chat_id` instead of `chat.id`."""
+
+        return self.chat.id
+
+    @property
+    def chat_title(self) -> str:
+        """Chat title, for `supergroups`, `channels` and `group` chats.
+        Full name, for `private` chat."""
+
+        return (
+            self.chat.full_name.unwrap()
+            if self.chat.type == ChatType.PRIVATE
+            else self.chat.title.unwrap()
+        )
+
+    def __eq__(self, other: typing.Any) -> bool:
+        return (
+            isinstance(other, self.__class__)
+            and self.message_id == other.message_id
+            and self.chat_id == other.chat_id
+        )
 
 
 class MessageId(Model):
-    """Object `MessageId`, see the [documentation](https://core.telegram.org/bots/api#messageid)
+    """Object `MessageId`, see the [documentation](https://core.telegram.org/bots/api#messageid).
 
-    This object represents a unique message identifier."""
+    This object represents a unique message identifier.
+    """
 
     message_id: int
-    """Unique message identifier"""
+    """Unique message identifier."""
 
 
 class InaccessibleMessage(MaybeInaccessibleMessage):
-    """Object `InaccessibleMessage`, see the [documentation](https://core.telegram.org/bots/api#inaccessiblemessage)
+    """Object `InaccessibleMessage`, see the [documentation](https://core.telegram.org/bots/api#inaccessiblemessage).
 
     This object describes a message that was deleted or is otherwise inaccessible to the bot.
     """
 
     chat: "Chat"
-    """Chat the message belonged to"""
+    """Chat the message belonged to."""
 
     message_id: int
-    """Unique message identifier inside the chat"""
+    """Unique message identifier inside the chat."""
 
     date: typing.Literal[0]
     """Always 0. The field can be used to differentiate regular and inaccessible 
     messages."""
 
 
 class MessageEntity(Model):
-    """Object `MessageEntity`, see the [documentation](https://core.telegram.org/bots/api#messageentity)
+    """Object `MessageEntity`, see the [documentation](https://core.telegram.org/bots/api#messageentity).
 
     This object represents one special entity in a text message. For example, hashtags, usernames, URLs, etc.
     """
 
     type: MessageEntityType
     """Type of the entity. Currently, can be `mention` (@username), `hashtag` 
     (#hashtag), `cashtag` ($USD), `bot_command` (/start@jobs_bot), `url` 
     (https://telegram.org), `email` (do-not-reply@telegram.org), `phone_number` 
     (+1-212-555-0123), `bold` (bold text), `italic` (italic text), `underline` 
     (underlined text), `strikethrough` (strikethrough text), `spoiler` 
     (spoiler message), `blockquote` (block quotation), `code` (monowidth 
     string), `pre` (monowidth block), `text_link` (for clickable text URLs), 
     `text_mention` (for users without usernames), `custom_emoji` (for inline 
-    custom emoji stickers)"""
+    custom emoji stickers)."""
 
     offset: int
-    """Offset in UTF-16 code units to the start of the entity"""
+    """Offset in UTF-16 code units to the start of the entity."""
 
     length: int
-    """Length of the entity in UTF-16 code units"""
+    """Length of the entity in UTF-16 code units."""
 
     url: Option[str] = Nothing
     """Optional. For `text_link` only, URL that will be opened after user taps 
-    on the text"""
+    on the text."""
 
     user: Option["User"] = Nothing
-    """Optional. For `text_mention` only, the mentioned user"""
+    """Optional. For `text_mention` only, the mentioned user."""
 
     language: Option[str] = Nothing
-    """Optional. For `pre` only, the programming language of the entity text"""
+    """Optional. For `pre` only, the programming language of the entity text."""
 
     custom_emoji_id: Option[str] = Nothing
     """Optional. For `custom_emoji` only, unique identifier of the custom emoji. 
-    Use getCustomEmojiStickers to get full information about the sticker"""
+    Use getCustomEmojiStickers to get full information about the sticker."""
 
 
 class TextQuote(Model):
-    """Object `TextQuote`, see the [documentation](https://core.telegram.org/bots/api#textquote)
+    """Object `TextQuote`, see the [documentation](https://core.telegram.org/bots/api#textquote).
 
     This object contains information about the quoted part of a message that is replied to by the given message.
     """
 
     text: str
-    """Text of the quoted part of a message that is replied to by the given message"""
+    """Text of the quoted part of a message that is replied to by the given message."""
 
     position: int
     """Approximate quote position in the original message in UTF-16 code units 
-    as specified by the sender"""
+    as specified by the sender."""
 
     entities: Option[list["MessageEntity"]] = Nothing
     """Optional. Special entities that appear in the quote. Currently, only bold, 
     italic, underline, strikethrough, spoiler, and custom_emoji entities 
     are kept in quotes."""
 
     is_manual: Option[bool] = Nothing
     """Optional. True, if the quote was chosen manually by the message sender. 
     Otherwise, the quote was added automatically by the server."""
 
 
 class ExternalReplyInfo(Model):
-    """Object `ExternalReplyInfo`, see the [documentation](https://core.telegram.org/bots/api#externalreplyinfo)
+    """Object `ExternalReplyInfo`, see the [documentation](https://core.telegram.org/bots/api#externalreplyinfo).
 
     This object contains information about a message that is being replied to, which may come from another chat or forum topic.
     """
 
-    origin: Union[
+    origin: Variative[
         "MessageOriginUser",
         "MessageOriginHiddenUser",
         "MessageOriginChat",
         "MessageOriginChannel",
     ]
-    """Origin of the message replied to by the given message"""
+    """Origin of the message replied to by the given message."""
 
     chat: Option["Chat"] = Nothing
     """Optional. Chat the original message belongs to. Available only if the chat 
     is a supergroup or a channel."""
 
     message_id: Option[int] = Nothing
     """Optional. Unique message identifier inside the original chat. Available 
     only if the original chat is a supergroup or a channel."""
 
     link_preview_options: Option["LinkPreviewOptions"] = Nothing
     """Optional. Options used for link preview generation for the original message, 
-    if it is a text message"""
+    if it is a text message."""
 
     animation: Option["Animation"] = Nothing
-    """Optional. Message is an animation, information about the animation"""
+    """Optional. Message is an animation, information about the animation."""
 
     audio: Option["Audio"] = Nothing
-    """Optional. Message is an audio file, information about the file"""
+    """Optional. Message is an audio file, information about the file."""
 
     document: Option["Document"] = Nothing
-    """Optional. Message is a general file, information about the file"""
+    """Optional. Message is a general file, information about the file."""
 
     photo: Option[list["PhotoSize"]] = Nothing
-    """Optional. Message is a photo, available sizes of the photo"""
+    """Optional. Message is a photo, available sizes of the photo."""
 
     sticker: Option["Sticker"] = Nothing
-    """Optional. Message is a sticker, information about the sticker"""
+    """Optional. Message is a sticker, information about the sticker."""
 
     story: Option["Story"] = Nothing
-    """Optional. Message is a forwarded story"""
+    """Optional. Message is a forwarded story."""
 
     video: Option["Video"] = Nothing
-    """Optional. Message is a video, information about the video"""
+    """Optional. Message is a video, information about the video."""
 
     video_note: Option["VideoNote"] = Nothing
-    """Optional. Message is a video note, information about the video message"""
+    """Optional. Message is a video note, information about the video message."""
 
     voice: Option["Voice"] = Nothing
-    """Optional. Message is a voice message, information about the file"""
+    """Optional. Message is a voice message, information about the file."""
 
     has_media_spoiler: Option[bool] = Nothing
-    """Optional. True, if the message media is covered by a spoiler animation"""
+    """Optional. True, if the message media is covered by a spoiler animation."""
 
     contact: Option["Contact"] = Nothing
-    """Optional. Message is a shared contact, information about the contact"""
+    """Optional. Message is a shared contact, information about the contact."""
 
     dice: Option["Dice"] = Nothing
-    """Optional. Message is a dice with random value"""
+    """Optional. Message is a dice with random value."""
 
     game: Option["Game"] = Nothing
     """Optional. Message is a game, information about the game. More about games: 
-    https://core.telegram.org/bots/api#games"""
+    https://core.telegram.org/bots/api#games."""
 
     giveaway: Option["Giveaway"] = Nothing
-    """Optional. Message is a scheduled giveaway, information about the giveaway"""
+    """Optional. Message is a scheduled giveaway, information about the giveaway."""
 
     giveaway_winners: Option["GiveawayWinners"] = Nothing
-    """Optional. A giveaway with public winners was completed"""
+    """Optional. A giveaway with public winners was completed."""
 
     invoice: Option["Invoice"] = Nothing
     """Optional. Message is an invoice for a payment, information about the invoice. 
-    More about payments: https://core.telegram.org/bots/api#payments"""
+    More about payments: https://core.telegram.org/bots/api#payments."""
 
     location: Option["Location"] = Nothing
-    """Optional. Message is a shared location, information about the location"""
+    """Optional. Message is a shared location, information about the location."""
 
     poll: Option["Poll"] = Nothing
-    """Optional. Message is a native poll, information about the poll"""
+    """Optional. Message is a native poll, information about the poll."""
 
     venue: Option["Venue"] = Nothing
-    """Optional. Message is a venue, information about the venue"""
+    """Optional. Message is a venue, information about the venue."""
 
 
 class ReplyParameters(Model):
-    """Object `ReplyParameters`, see the [documentation](https://core.telegram.org/bots/api#replyparameters)
+    """Object `ReplyParameters`, see the [documentation](https://core.telegram.org/bots/api#replyparameters).
 
-    Describes reply parameters for the message that is being sent."""
+    Describes reply parameters for the message that is being sent.
+    """
 
     message_id: int
     """Identifier of the message that will be replied to in the current chat, or 
-    in the chat chat_id if it is specified"""
+    in the chat chat_id if it is specified."""
 
-    chat_id: Option[int | str] = Nothing
+    chat_id: Option[Variative[int, str]] = Nothing
     """Optional. If the message to be replied to is from a different chat, unique 
-    identifier for the chat or username of the channel (in the format @channelusername)"""
+    identifier for the chat or username of the channel (in the format @channelusername). 
+    Not supported for messages sent on behalf of a business account."""
 
     allow_sending_without_reply: Option[bool] = Nothing
     """Optional. Pass True if the message should be sent even if the specified message 
-    to be replied to is not found; can be used only for replies in the same chat 
-    and forum topic."""
+    to be replied to is not found. Always False for replies in another chat or 
+    forum topic. Always True for messages sent on behalf of a business account."""
 
     quote: Option[str] = Nothing
     """Optional. Quoted part of the message to be replied to; 0-1024 characters 
     after entities parsing. The quote must be an exact substring of the message 
     to be replied to, including bold, italic, underline, strikethrough, spoiler, 
     and custom_emoji entities. The message will fail to send if the quote isn't 
     found in the original message."""
@@ -1000,443 +1117,461 @@
     for more details."""
 
     quote_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. A JSON-serialized list of special entities that appear in the 
     quote. It can be specified instead of quote_parse_mode."""
 
     quote_position: Option[int] = Nothing
-    """Optional. Position of the quote in the original message in UTF-16 code units"""
+    """Optional. Position of the quote in the original message in UTF-16 code units."""
 
 
 class MessageOriginUser(MessageOrigin):
-    """Object `MessageOriginUser`, see the [documentation](https://core.telegram.org/bots/api#messageoriginuser)
+    """Object `MessageOriginUser`, see the [documentation](https://core.telegram.org/bots/api#messageoriginuser).
 
-    The message was originally sent by a known user."""
+    The message was originally sent by a known user.
+    """
 
-    type: MessageOriginType
-    """Type of the message origin, always `user`"""
+    type: typing.Literal["user"]
+    """Type of the message origin, always `user`."""
 
-    date: int
-    """Date the message was sent originally in Unix time"""
+    date: datetime
+    """Date the message was sent originally in Unix time."""
 
     sender_user: "User"
-    """User that sent the message originally"""
+    """User that sent the message originally."""
 
 
 class MessageOriginHiddenUser(MessageOrigin):
-    """Object `MessageOriginHiddenUser`, see the [documentation](https://core.telegram.org/bots/api#messageoriginhiddenuser)
+    """Object `MessageOriginHiddenUser`, see the [documentation](https://core.telegram.org/bots/api#messageoriginhiddenuser).
 
-    The message was originally sent by an unknown user."""
+    The message was originally sent by an unknown user.
+    """
 
-    type: MessageOriginType
-    """Type of the message origin, always `hidden_user`"""
+    type: typing.Literal["hidden_user"]
+    """Type of the message origin, always `hidden_user`."""
 
-    date: int
-    """Date the message was sent originally in Unix time"""
+    date: datetime
+    """Date the message was sent originally in Unix time."""
 
     sender_user_name: str
-    """Name of the user that sent the message originally"""
+    """Name of the user that sent the message originally."""
 
 
 class MessageOriginChat(MessageOrigin):
-    """Object `MessageOriginChat`, see the [documentation](https://core.telegram.org/bots/api#messageoriginchat)
+    """Object `MessageOriginChat`, see the [documentation](https://core.telegram.org/bots/api#messageoriginchat).
 
-    The message was originally sent on behalf of a chat to a group chat."""
+    The message was originally sent on behalf of a chat to a group chat.
+    """
 
-    type: str
-    """Type of the message origin, always `chat`"""
+    type: typing.Literal["chat"]
+    """Type of the message origin, always `chat`."""
 
-    date: int
-    """Date the message was sent originally in Unix time"""
+    date: datetime
+    """Date the message was sent originally in Unix time."""
 
     sender_chat: "Chat"
-    """Chat that sent the message originally"""
+    """Chat that sent the message originally."""
 
     author_signature: Option[str] = Nothing
     """Optional. For messages originally sent by an anonymous chat administrator, 
-    original message author signature"""
+    original message author signature."""
 
 
 class MessageOriginChannel(MessageOrigin):
-    """Object `MessageOriginChannel`, see the [documentation](https://core.telegram.org/bots/api#messageoriginchannel)
+    """Object `MessageOriginChannel`, see the [documentation](https://core.telegram.org/bots/api#messageoriginchannel).
 
-    The message was originally sent to a channel chat."""
+    The message was originally sent to a channel chat.
+    """
 
-    type: str
-    """Type of the message origin, always `channel`"""
+    type: typing.Literal["channel"]
+    """Type of the message origin, always `channel`."""
 
-    date: int
-    """Date the message was sent originally in Unix time"""
+    date: datetime
+    """Date the message was sent originally in Unix time."""
 
     chat: "Chat"
-    """Channel chat to which the message was originally sent"""
+    """Channel chat to which the message was originally sent."""
 
     message_id: int
-    """Unique message identifier inside the chat"""
+    """Unique message identifier inside the chat."""
 
     author_signature: Option[str] = Nothing
-    """Optional. Signature of the original post author"""
+    """Optional. Signature of the original post author."""
 
 
 class PhotoSize(Model):
-    """Object `PhotoSize`, see the [documentation](https://core.telegram.org/bots/api#photosize)
+    """Object `PhotoSize`, see the [documentation](https://core.telegram.org/bots/api#photosize).
 
-    This object represents one size of a photo or a file / sticker thumbnail."""
+    This object represents one size of a photo or a file / sticker thumbnail.
+    """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     width: int
-    """Photo width"""
+    """Photo width."""
 
     height: int
-    """Photo height"""
+    """Photo height."""
 
     file_size: Option[int] = Nothing
-    """Optional. File size in bytes"""
+    """Optional. File size in bytes."""
 
 
 class Animation(Model):
-    """Object `Animation`, see the [documentation](https://core.telegram.org/bots/api#animation)
+    """Object `Animation`, see the [documentation](https://core.telegram.org/bots/api#animation).
 
     This object represents an animation file (GIF or H.264/MPEG-4 AVC video without sound).
     """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     width: int
-    """Video width as defined by sender"""
+    """Video width as defined by sender."""
 
     height: int
-    """Video height as defined by sender"""
+    """Video height as defined by sender."""
 
     duration: int
-    """Duration of the video in seconds as defined by sender"""
+    """Duration of the video in seconds as defined by sender."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Animation thumbnail as defined by sender"""
+    """Optional. Animation thumbnail as defined by sender."""
 
     file_name: Option[str] = Nothing
-    """Optional. Original animation filename as defined by sender"""
+    """Optional. Original animation filename as defined by sender."""
 
     mime_type: Option[str] = Nothing
-    """Optional. MIME type of the file as defined by sender"""
+    """Optional. MIME type of the file as defined by sender."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
     languages may have difficulty/silent defects in interpreting it. But 
     it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this value."""
 
 
 class Audio(Model):
-    """Object `Audio`, see the [documentation](https://core.telegram.org/bots/api#audio)
+    """Object `Audio`, see the [documentation](https://core.telegram.org/bots/api#audio).
 
     This object represents an audio file to be treated as music by the Telegram clients.
     """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     duration: int
-    """Duration of the audio in seconds as defined by sender"""
+    """Duration of the audio in seconds as defined by sender."""
 
     performer: Option[str] = Nothing
-    """Optional. Performer of the audio as defined by sender or by audio tags"""
+    """Optional. Performer of the audio as defined by sender or by audio tags."""
 
     title: Option[str] = Nothing
-    """Optional. Title of the audio as defined by sender or by audio tags"""
+    """Optional. Title of the audio as defined by sender or by audio tags."""
 
     file_name: Option[str] = Nothing
-    """Optional. Original filename as defined by sender"""
+    """Optional. Original filename as defined by sender."""
 
     mime_type: Option[str] = Nothing
-    """Optional. MIME type of the file as defined by sender"""
+    """Optional. MIME type of the file as defined by sender."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
     languages may have difficulty/silent defects in interpreting it. But 
     it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this value."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Thumbnail of the album cover to which the music file belongs"""
+    """Optional. Thumbnail of the album cover to which the music file belongs."""
 
 
 class Document(Model):
-    """Object `Document`, see the [documentation](https://core.telegram.org/bots/api#document)
+    """Object `Document`, see the [documentation](https://core.telegram.org/bots/api#document).
 
     This object represents a general file (as opposed to photos, voice messages and audio files).
     """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Document thumbnail as defined by sender"""
+    """Optional. Document thumbnail as defined by sender."""
 
     file_name: Option[str] = Nothing
-    """Optional. Original filename as defined by sender"""
+    """Optional. Original filename as defined by sender."""
 
     mime_type: Option[str] = Nothing
-    """Optional. MIME type of the file as defined by sender"""
+    """Optional. MIME type of the file as defined by sender."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
     languages may have difficulty/silent defects in interpreting it. But 
     it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this value."""
 
 
 class Story(Model):
-    """Object `Story`, see the [documentation](https://core.telegram.org/bots/api#story)
+    """Object `Story`, see the [documentation](https://core.telegram.org/bots/api#story).
 
-    This object represents a message about a forwarded story in the chat. Currently holds no information.
+    This object represents a story.
     """
 
-    pass
+    chat: "Chat"
+    """Chat that posted the story."""
+
+    id: int
+    """Unique identifier for the story in the chat."""
 
 
 class Video(Model):
-    """Object `Video`, see the [documentation](https://core.telegram.org/bots/api#video)
+    """Object `Video`, see the [documentation](https://core.telegram.org/bots/api#video).
 
-    This object represents a video file."""
+    This object represents a video file.
+    """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     width: int
-    """Video width as defined by sender"""
+    """Video width as defined by sender."""
 
     height: int
-    """Video height as defined by sender"""
+    """Video height as defined by sender."""
 
     duration: int
-    """Duration of the video in seconds as defined by sender"""
+    """Duration of the video in seconds as defined by sender."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Video thumbnail"""
+    """Optional. Video thumbnail."""
 
     file_name: Option[str] = Nothing
-    """Optional. Original filename as defined by sender"""
+    """Optional. Original filename as defined by sender."""
 
     mime_type: Option[str] = Nothing
-    """Optional. MIME type of the file as defined by sender"""
+    """Optional. MIME type of the file as defined by sender."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
     languages may have difficulty/silent defects in interpreting it. But 
     it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this value."""
 
 
 class VideoNote(Model):
-    """Object `VideoNote`, see the [documentation](https://core.telegram.org/bots/api#videonote)
+    """Object `VideoNote`, see the [documentation](https://core.telegram.org/bots/api#videonote).
 
-    This object represents a video message (available in Telegram apps as of v.4.0)."""
+    This object represents a video message (available in Telegram apps as of v.4.0).
+    """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     length: int
-    """Video width and height (diameter of the video message) as defined by sender"""
+    """Video width and height (diameter of the video message) as defined by sender."""
 
     duration: int
-    """Duration of the video in seconds as defined by sender"""
+    """Duration of the video in seconds as defined by sender."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Video thumbnail"""
+    """Optional. Video thumbnail."""
 
     file_size: Option[int] = Nothing
-    """Optional. File size in bytes"""
+    """Optional. File size in bytes."""
 
 
 class Voice(Model):
-    """Object `Voice`, see the [documentation](https://core.telegram.org/bots/api#voice)
+    """Object `Voice`, see the [documentation](https://core.telegram.org/bots/api#voice).
 
-    This object represents a voice note."""
+    This object represents a voice note.
+    """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     duration: int
-    """Duration of the audio in seconds as defined by sender"""
+    """Duration of the audio in seconds as defined by sender."""
 
     mime_type: Option[str] = Nothing
-    """Optional. MIME type of the file as defined by sender"""
+    """Optional. MIME type of the file as defined by sender."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
     languages may have difficulty/silent defects in interpreting it. But 
     it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this value."""
 
 
 class Contact(Model):
-    """Object `Contact`, see the [documentation](https://core.telegram.org/bots/api#contact)
+    """Object `Contact`, see the [documentation](https://core.telegram.org/bots/api#contact).
 
-    This object represents a phone contact."""
+    This object represents a phone contact.
+    """
 
     phone_number: str
-    """Contact's phone number"""
+    """Contact's phone number."""
 
     first_name: str
-    """Contact's first name"""
+    """Contact's first name."""
 
     last_name: Option[str] = Nothing
-    """Optional. Contact's last name"""
+    """Optional. Contact's last name."""
 
     user_id: Option[int] = Nothing
     """Optional. Contact's user identifier in Telegram. This number may have 
     more than 32 significant bits and some programming languages may have difficulty/silent 
     defects in interpreting it. But it has at most 52 significant bits, so a 64-bit 
     integer or double-precision float type are safe for storing this identifier."""
 
     vcard: Option[str] = Nothing
-    """Optional. Additional data about the contact in the form of a vCard"""
+    """Optional. Additional data about the contact in the form of a vCard."""
 
 
 class Dice(Model):
-    """Object `Dice`, see the [documentation](https://core.telegram.org/bots/api#dice)
+    """Object `Dice`, see the [documentation](https://core.telegram.org/bots/api#dice).
 
-    This object represents an animated emoji that displays a random value."""
+    This object represents an animated emoji that displays a random value.
+    """
 
     emoji: DiceEmoji
-    """Emoji on which the dice throw animation is based"""
+    """Emoji on which the dice throw animation is based."""
 
     value: int
     """Value of the dice, 1-6 for `🎲`, `🎯` and `🎳` base emoji, 1-5 for `🏀` and `⚽` base 
-    emoji, 1-64 for `🎰` base emoji"""
+    emoji, 1-64 for `🎰` base emoji."""
 
 
 class PollOption(Model):
-    """Object `PollOption`, see the [documentation](https://core.telegram.org/bots/api#polloption)
+    """Object `PollOption`, see the [documentation](https://core.telegram.org/bots/api#polloption).
 
-    This object contains information about one answer option in a poll."""
+    This object contains information about one answer option in a poll.
+    """
 
     text: str
-    """Option text, 1-100 characters"""
+    """Option text, 1-100 characters."""
 
     voter_count: int
-    """Number of users that voted for this option"""
+    """Number of users that voted for this option."""
 
 
 class PollAnswer(Model):
-    """Object `PollAnswer`, see the [documentation](https://core.telegram.org/bots/api#pollanswer)
+    """Object `PollAnswer`, see the [documentation](https://core.telegram.org/bots/api#pollanswer).
 
-    This object represents an answer of a user in a non-anonymous poll."""
+    This object represents an answer of a user in a non-anonymous poll.
+    """
 
     poll_id: str
-    """Unique poll identifier"""
+    """Unique poll identifier."""
 
     option_ids: list[int]
     """0-based identifiers of chosen answer options. May be empty if the vote was 
     retracted."""
 
     voter_chat: Option["Chat"] = Nothing
-    """Optional. The chat that changed the answer to the poll, if the voter is anonymous"""
+    """Optional. The chat that changed the answer to the poll, if the voter is anonymous."""
 
     user: Option["User"] = Nothing
     """Optional. The user that changed the answer to the poll, if the voter isn't 
-    anonymous"""
+    anonymous."""
 
 
 class Poll(Model):
-    """Object `Poll`, see the [documentation](https://core.telegram.org/bots/api#poll)
+    """Object `Poll`, see the [documentation](https://core.telegram.org/bots/api#poll).
 
-    This object contains information about a poll."""
+    This object contains information about a poll.
+    """
 
     id: str
-    """Unique poll identifier"""
+    """Unique poll identifier."""
 
     question: str
-    """Poll question, 1-300 characters"""
+    """Poll question, 1-300 characters."""
 
     options: list["PollOption"]
-    """List of poll options"""
+    """List of poll options."""
 
     total_voter_count: int
-    """Total number of users that voted in the poll"""
+    """Total number of users that voted in the poll."""
 
     is_closed: bool
-    """True, if the poll is closed"""
+    """True, if the poll is closed."""
 
     is_anonymous: bool
-    """True, if the poll is anonymous"""
+    """True, if the poll is anonymous."""
 
-    type: str
-    """Poll type, currently can be `regular` or `quiz`"""
+    type: typing.Literal["regular", "quiz"]
+    """Poll type, currently can be `regular` or `quiz`."""
 
     allows_multiple_answers: bool
-    """True, if the poll allows multiple answers"""
+    """True, if the poll allows multiple answers."""
 
     correct_option_id: Option[int] = Nothing
     """Optional. 0-based identifier of the correct answer option. Available 
     only for polls in the quiz mode, which are closed, or was sent (not forwarded) 
     by the bot or to the private chat with the bot."""
 
     explanation: Option[str] = Nothing
     """Optional. Text that is shown when a user chooses an incorrect answer or taps 
-    on the lamp icon in a quiz-style poll, 0-200 characters"""
+    on the lamp icon in a quiz-style poll, 0-200 characters."""
 
     explanation_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. Special entities like usernames, URLs, bot commands, etc. that 
-    appear in the explanation"""
+    appear in the explanation."""
 
     open_period: Option[int] = Nothing
-    """Optional. Amount of time in seconds the poll will be active after creation"""
+    """Optional. Amount of time in seconds the poll will be active after creation."""
 
-    close_date: Option[int] = Nothing
+    close_date: Option[datetime] = Nothing
     """Optional. Point in time (Unix timestamp) when the poll will be automatically 
-    closed"""
+    closed."""
 
 
 class Location(Model):
-    """Object `Location`, see the [documentation](https://core.telegram.org/bots/api#location)
-
-    This object represents a point on the map."""
+    """Object `Location`, see the [documentation](https://core.telegram.org/bots/api#location).
 
-    longitude: float
-    """Longitude as defined by sender"""
+    This object represents a point on the map.
+    """
 
     latitude: float
-    """Latitude as defined by sender"""
+    """Latitude as defined by sender."""
+
+    longitude: float
+    """Longitude as defined by sender."""
 
     horizontal_accuracy: Option[float] = Nothing
     """Optional. The radius of uncertainty for the location, measured in meters; 
-    0-1500"""
+    0-1500."""
 
     live_period: Option[int] = Nothing
     """Optional. Time relative to the message sending date, during which the location 
     can be updated; in seconds. For active live locations only."""
 
     heading: Option[int] = Nothing
     """Optional. The direction in which user is moving, in degrees; 1-360. For 
@@ -1444,390 +1579,429 @@
 
     proximity_alert_radius: Option[int] = Nothing
     """Optional. The maximum distance for proximity alerts about approaching 
     another chat member, in meters. For sent live locations only."""
 
 
 class Venue(Model):
-    """Object `Venue`, see the [documentation](https://core.telegram.org/bots/api#venue)
+    """Object `Venue`, see the [documentation](https://core.telegram.org/bots/api#venue).
 
-    This object represents a venue."""
+    This object represents a venue.
+    """
 
     location: "Location"
-    """Venue location. Can't be a live location"""
+    """Venue location. Can't be a live location."""
 
     title: str
-    """Name of the venue"""
+    """Name of the venue."""
 
     address: str
-    """Address of the venue"""
+    """Address of the venue."""
 
     foursquare_id: Option[str] = Nothing
-    """Optional. Foursquare identifier of the venue"""
+    """Optional. Foursquare identifier of the venue."""
 
     foursquare_type: Option[str] = Nothing
     """Optional. Foursquare type of the venue. (For example, `arts_entertainment/default`, 
-    `arts_entertainment/aquarium` or `food/icecream`.)"""
+    `arts_entertainment/aquarium` or `food/icecream`.)."""
 
     google_place_id: Option[str] = Nothing
-    """Optional. Google Places identifier of the venue"""
+    """Optional. Google Places identifier of the venue."""
 
     google_place_type: Option[str] = Nothing
-    """Optional. Google Places type of the venue. (See supported types.)"""
+    """Optional. Google Places type of the venue. (See supported types.)."""
 
 
 class WebAppData(Model):
-    """Object `WebAppData`, see the [documentation](https://core.telegram.org/bots/api#webappdata)
+    """Object `WebAppData`, see the [documentation](https://core.telegram.org/bots/api#webappdata).
 
-    Describes data sent from a Web App to the bot."""
+    Describes data sent from a Web App to the bot.
+    """
 
     data: str
     """The data. Be aware that a bad client can send arbitrary data in this field."""
 
     button_text: str
     """Text of the web_app keyboard button from which the Web App was opened. Be 
     aware that a bad client can send arbitrary data in this field."""
 
 
 class ProximityAlertTriggered(Model):
-    """Object `ProximityAlertTriggered`, see the [documentation](https://core.telegram.org/bots/api#proximityalerttriggered)
+    """Object `ProximityAlertTriggered`, see the [documentation](https://core.telegram.org/bots/api#proximityalerttriggered).
 
     This object represents the content of a service message, sent whenever a user in the chat triggers a proximity alert set by another user.
     """
 
     traveler: "User"
-    """User that triggered the alert"""
+    """User that triggered the alert."""
 
     watcher: "User"
-    """User that set the alert"""
+    """User that set the alert."""
 
     distance: int
-    """The distance between the users"""
+    """The distance between the users."""
 
 
 class MessageAutoDeleteTimerChanged(Model):
-    """Object `MessageAutoDeleteTimerChanged`, see the [documentation](https://core.telegram.org/bots/api#messageautodeletetimerchanged)
+    """Object `MessageAutoDeleteTimerChanged`, see the [documentation](https://core.telegram.org/bots/api#messageautodeletetimerchanged).
 
     This object represents a service message about a change in auto-delete timer settings.
     """
 
     message_auto_delete_time: int
-    """New auto-delete time for messages in the chat; in seconds"""
+    """New auto-delete time for messages in the chat; in seconds."""
+
+
+class ChatBoostAdded(Model):
+    """Object `ChatBoostAdded`, see the [documentation](https://core.telegram.org/bots/api#chatboostadded).
+
+    This object represents a service message about a user boosting a chat.
+    """
+
+    boost_count: int
+    """Number of boosts added by the user."""
 
 
 class ForumTopicCreated(Model):
-    """Object `ForumTopicCreated`, see the [documentation](https://core.telegram.org/bots/api#forumtopiccreated)
+    """Object `ForumTopicCreated`, see the [documentation](https://core.telegram.org/bots/api#forumtopiccreated).
 
     This object represents a service message about a new forum topic created in the chat.
     """
 
     name: str
-    """Name of the topic"""
+    """Name of the topic."""
 
-    icon_color: int
-    """Color of the topic icon in RGB format"""
+    icon_color: TopicIconColor
+    """Color of the topic icon in RGB format."""
 
     icon_custom_emoji_id: Option[str] = Nothing
-    """Optional. Unique identifier of the custom emoji shown as the topic icon"""
+    """Optional. Unique identifier of the custom emoji shown as the topic icon."""
 
 
 class ForumTopicClosed(Model):
-    """Object `ForumTopicClosed`, see the [documentation](https://core.telegram.org/bots/api#forumtopicclosed)
+    """Object `ForumTopicClosed`, see the [documentation](https://core.telegram.org/bots/api#forumtopicclosed).
 
     This object represents a service message about a forum topic closed in the chat. Currently holds no information.
     """
 
-    pass
-
 
 class ForumTopicEdited(Model):
-    """Object `ForumTopicEdited`, see the [documentation](https://core.telegram.org/bots/api#forumtopicedited)
+    """Object `ForumTopicEdited`, see the [documentation](https://core.telegram.org/bots/api#forumtopicedited).
 
-    This object represents a service message about an edited forum topic."""
+    This object represents a service message about an edited forum topic.
+    """
 
     name: Option[str] = Nothing
-    """Optional. New name of the topic, if it was edited"""
+    """Optional. New name of the topic, if it was edited."""
 
     icon_custom_emoji_id: Option[str] = Nothing
     """Optional. New identifier of the custom emoji shown as the topic icon, if 
-    it was edited; an empty string if the icon was removed"""
+    it was edited; an empty string if the icon was removed."""
 
 
 class ForumTopicReopened(Model):
-    """Object `ForumTopicReopened`, see the [documentation](https://core.telegram.org/bots/api#forumtopicreopened)
+    """Object `ForumTopicReopened`, see the [documentation](https://core.telegram.org/bots/api#forumtopicreopened).
 
     This object represents a service message about a forum topic reopened in the chat. Currently holds no information.
     """
 
-    pass
-
 
 class GeneralForumTopicHidden(Model):
-    """Object `GeneralForumTopicHidden`, see the [documentation](https://core.telegram.org/bots/api#generalforumtopichidden)
+    """Object `GeneralForumTopicHidden`, see the [documentation](https://core.telegram.org/bots/api#generalforumtopichidden).
 
     This object represents a service message about General forum topic hidden in the chat. Currently holds no information.
     """
 
-    pass
-
 
 class GeneralForumTopicUnhidden(Model):
-    """Object `GeneralForumTopicUnhidden`, see the [documentation](https://core.telegram.org/bots/api#generalforumtopicunhidden)
+    """Object `GeneralForumTopicUnhidden`, see the [documentation](https://core.telegram.org/bots/api#generalforumtopicunhidden).
 
     This object represents a service message about General forum topic unhidden in the chat. Currently holds no information.
     """
 
-    pass
+
+class SharedUser(Model):
+    """Object `SharedUser`, see the [documentation](https://core.telegram.org/bots/api#shareduser).
+
+    This object contains information about a user that was shared with the bot using a KeyboardButtonRequestUser button.
+    """
+
+    user_id: int
+    """Identifier of the shared user. This number may have more than 32 significant 
+    bits and some programming languages may have difficulty/silent defects 
+    in interpreting it. But it has at most 52 significant bits, so 64-bit integers 
+    or double-precision float types are safe for storing these identifiers. 
+    The bot may not have access to the user and could be unable to use this identifier, 
+    unless the user is already known to the bot by some other means."""
+
+    first_name: Option[str] = Nothing
+    """Optional. First name of the user, if the name was requested by the bot."""
+
+    last_name: Option[str] = Nothing
+    """Optional. Last name of the user, if the name was requested by the bot."""
+
+    username: Option[str] = Nothing
+    """Optional. Username of the user, if the username was requested by the bot."""
+
+    photo: Option[list["PhotoSize"]] = Nothing
+    """Optional. Available sizes of the chat photo, if the photo was requested 
+    by the bot."""
 
 
 class UsersShared(Model):
-    """Object `UsersShared`, see the [documentation](https://core.telegram.org/bots/api#usersshared)
+    """Object `UsersShared`, see the [documentation](https://core.telegram.org/bots/api#usersshared).
 
     This object contains information about the users whose identifiers were shared with the bot using a KeyboardButtonRequestUsers button.
     """
 
     request_id: int
-    """Identifier of the request"""
+    """Identifier of the request."""
 
-    user_ids: list[int]
-    """Identifiers of the shared users. These numbers may have more than 32 significant 
-    bits and some programming languages may have difficulty/silent defects 
-    in interpreting them. But they have at most 52 significant bits, so 64-bit 
-    integers or double-precision float types are safe for storing these identifiers. 
-    The bot may not have access to the users and could be unable to use these identifiers, 
-    unless the users are already known to the bot by some other means."""
+    users: list["SharedUser"]
+    """Information about users shared with the bot."""
 
 
 class ChatShared(Model):
-    """Object `ChatShared`, see the [documentation](https://core.telegram.org/bots/api#chatshared)
+    """Object `ChatShared`, see the [documentation](https://core.telegram.org/bots/api#chatshared).
 
-    This object contains information about the chat whose identifier was shared with the bot using a KeyboardButtonRequestChat button.
+    This object contains information about a chat that was shared with the bot using a KeyboardButtonRequestChat button.
     """
 
     request_id: int
-    """Identifier of the request"""
+    """Identifier of the request."""
 
     chat_id: int
     """Identifier of the shared chat. This number may have more than 32 significant 
     bits and some programming languages may have difficulty/silent defects 
     in interpreting it. But it has at most 52 significant bits, so a 64-bit integer 
     or double-precision float type are safe for storing this identifier. The 
     bot may not have access to the chat and could be unable to use this identifier, 
     unless the chat is already known to the bot by some other means."""
 
+    title: Option[str] = Nothing
+    """Optional. Title of the chat, if the title was requested by the bot."""
+
+    username: Option[str] = Nothing
+    """Optional. Username of the chat, if the username was requested by the bot 
+    and available."""
+
+    photo: Option[list["PhotoSize"]] = Nothing
+    """Optional. Available sizes of the chat photo, if the photo was requested 
+    by the bot."""
+
 
 class WriteAccessAllowed(Model):
-    """Object `WriteAccessAllowed`, see the [documentation](https://core.telegram.org/bots/api#writeaccessallowed)
+    """Object `WriteAccessAllowed`, see the [documentation](https://core.telegram.org/bots/api#writeaccessallowed).
 
     This object represents a service message about a user allowing a bot to write messages after adding it to the attachment menu, launching a Web App from a link, or accepting an explicit request from a Web App sent by the method requestWriteAccess.
     """
 
     from_request: Option[bool] = Nothing
     """Optional. True, if the access was granted after the user accepted an explicit 
-    request from a Web App sent by the method requestWriteAccess"""
+    request from a Web App sent by the method requestWriteAccess."""
 
     web_app_name: Option[str] = Nothing
     """Optional. Name of the Web App, if the access was granted when the Web App was 
-    launched from a link"""
+    launched from a link."""
 
     from_attachment_menu: Option[bool] = Nothing
     """Optional. True, if the access was granted when the bot was added to the attachment 
-    or side menu"""
+    or side menu."""
 
 
 class VideoChatScheduled(Model):
-    """Object `VideoChatScheduled`, see the [documentation](https://core.telegram.org/bots/api#videochatscheduled)
+    """Object `VideoChatScheduled`, see the [documentation](https://core.telegram.org/bots/api#videochatscheduled).
 
     This object represents a service message about a video chat scheduled in the chat.
     """
 
-    start_date: int
+    start_date: datetime
     """Point in time (Unix timestamp) when the video chat is supposed to be started 
-    by a chat administrator"""
+    by a chat administrator."""
 
 
 class VideoChatStarted(Model):
-    """Object `VideoChatStarted`, see the [documentation](https://core.telegram.org/bots/api#videochatstarted)
+    """Object `VideoChatStarted`, see the [documentation](https://core.telegram.org/bots/api#videochatstarted).
 
     This object represents a service message about a video chat started in the chat. Currently holds no information.
     """
 
-    pass
-
 
 class VideoChatEnded(Model):
-    """Object `VideoChatEnded`, see the [documentation](https://core.telegram.org/bots/api#videochatended)
+    """Object `VideoChatEnded`, see the [documentation](https://core.telegram.org/bots/api#videochatended).
 
-    This object represents a service message about a video chat ended in the chat."""
+    This object represents a service message about a video chat ended in the chat.
+    """
 
     duration: int
-    """Video chat duration in seconds"""
+    """Video chat duration in seconds."""
 
 
 class VideoChatParticipantsInvited(Model):
-    """Object `VideoChatParticipantsInvited`, see the [documentation](https://core.telegram.org/bots/api#videochatparticipantsinvited)
+    """Object `VideoChatParticipantsInvited`, see the [documentation](https://core.telegram.org/bots/api#videochatparticipantsinvited).
 
     This object represents a service message about new members invited to a video chat.
     """
 
     users: list["User"]
-    """New members that were invited to the video chat"""
+    """New members that were invited to the video chat."""
 
 
 class GiveawayCreated(Model):
-    """Object `GiveawayCreated`, see the [documentation](https://core.telegram.org/bots/api#giveawaycreated)
+    """Object `GiveawayCreated`, see the [documentation](https://core.telegram.org/bots/api#giveawaycreated).
 
     This object represents a service message about the creation of a scheduled giveaway. Currently holds no information.
     """
 
-    pass
-
 
 class Giveaway(Model):
-    """Object `Giveaway`, see the [documentation](https://core.telegram.org/bots/api#giveaway)
+    """Object `Giveaway`, see the [documentation](https://core.telegram.org/bots/api#giveaway).
 
-    This object represents a message about a scheduled giveaway."""
+    This object represents a message about a scheduled giveaway.
+    """
 
     chats: list["Chat"]
-    """The list of chats which the user must join to participate in the giveaway"""
+    """The list of chats which the user must join to participate in the giveaway."""
 
-    winners_selection_date: int
-    """Point in time (Unix timestamp) when winners of the giveaway will be selected"""
+    winners_selection_date: datetime
+    """Point in time (Unix timestamp) when winners of the giveaway will be selected."""
 
     winner_count: int
-    """The number of users which are supposed to be selected as winners of the giveaway"""
+    """The number of users which are supposed to be selected as winners of the giveaway."""
 
     only_new_members: Option[bool] = Nothing
     """Optional. True, if only users who join the chats after the giveaway started 
-    should be eligible to win"""
+    should be eligible to win."""
 
     has_public_winners: Option[bool] = Nothing
-    """Optional. True, if the list of giveaway winners will be visible to everyone"""
+    """Optional. True, if the list of giveaway winners will be visible to everyone."""
 
     prize_description: Option[str] = Nothing
-    """Optional. Description of additional giveaway prize"""
+    """Optional. Description of additional giveaway prize."""
 
     country_codes: Option[list[str]] = Nothing
     """Optional. A list of two-letter ISO 3166-1 alpha-2 country codes indicating 
     the countries from which eligible users for the giveaway must come. If empty, 
     then all users can participate in the giveaway. Users with a phone number 
     that was bought on Fragment can always participate in giveaways."""
 
     premium_subscription_month_count: Option[int] = Nothing
     """Optional. The number of months the Telegram Premium subscription won from 
-    the giveaway will be active for"""
+    the giveaway will be active for."""
 
 
 class GiveawayWinners(Model):
-    """Object `GiveawayWinners`, see the [documentation](https://core.telegram.org/bots/api#giveawaywinners)
+    """Object `GiveawayWinners`, see the [documentation](https://core.telegram.org/bots/api#giveawaywinners).
 
     This object represents a message about the completion of a giveaway with public winners.
     """
 
     chat: "Chat"
-    """The chat that created the giveaway"""
+    """The chat that created the giveaway."""
 
     giveaway_message_id: int
-    """Identifier of the messsage with the giveaway in the chat"""
+    """Identifier of the message with the giveaway in the chat."""
 
-    winners_selection_date: int
-    """Point in time (Unix timestamp) when winners of the giveaway were selected"""
+    winners_selection_date: datetime
+    """Point in time (Unix timestamp) when winners of the giveaway were selected."""
 
     winner_count: int
-    """Total number of winners in the giveaway"""
+    """Total number of winners in the giveaway."""
 
     winners: list["User"]
-    """List of up to 100 winners of the giveaway"""
+    """List of up to 100 winners of the giveaway."""
 
     additional_chat_count: Option[int] = Nothing
     """Optional. The number of other chats the user had to join in order to be eligible 
-    for the giveaway"""
+    for the giveaway."""
 
     premium_subscription_month_count: Option[int] = Nothing
     """Optional. The number of months the Telegram Premium subscription won from 
-    the giveaway will be active for"""
+    the giveaway will be active for."""
 
     unclaimed_prize_count: Option[int] = Nothing
-    """Optional. Number of undistributed prizes"""
+    """Optional. Number of undistributed prizes."""
 
     only_new_members: Option[bool] = Nothing
     """Optional. True, if only users who had joined the chats after the giveaway 
-    started were eligible to win"""
+    started were eligible to win."""
 
     was_refunded: Option[bool] = Nothing
     """Optional. True, if the giveaway was canceled because the payment for it 
-    was refunded"""
+    was refunded."""
 
     prize_description: Option[str] = Nothing
-    """Optional. Description of additional giveaway prize"""
+    """Optional. Description of additional giveaway prize."""
 
 
 class GiveawayCompleted(Model):
-    """Object `GiveawayCompleted`, see the [documentation](https://core.telegram.org/bots/api#giveawaycompleted)
+    """Object `GiveawayCompleted`, see the [documentation](https://core.telegram.org/bots/api#giveawaycompleted).
 
     This object represents a service message about the completion of a giveaway without public winners.
     """
 
     winner_count: int
-    """Number of winners in the giveaway"""
+    """Number of winners in the giveaway."""
 
     unclaimed_prize_count: Option[int] = Nothing
-    """Optional. Number of undistributed prizes"""
+    """Optional. Number of undistributed prizes."""
 
     giveaway_message: Option["Message"] = Nothing
-    """Optional. Message with the giveaway that was completed, if it wasn't deleted"""
+    """Optional. Message with the giveaway that was completed, if it wasn't deleted."""
 
 
 class LinkPreviewOptions(Model):
-    """Object `LinkPreviewOptions`, see the [documentation](https://core.telegram.org/bots/api#linkpreviewoptions)
+    """Object `LinkPreviewOptions`, see the [documentation](https://core.telegram.org/bots/api#linkpreviewoptions).
 
-    Describes the options used for link preview generation."""
+    Describes the options used for link preview generation.
+    """
 
     is_disabled: Option[bool] = Nothing
-    """Optional. True, if the link preview is disabled"""
+    """Optional. True, if the link preview is disabled."""
 
     url: Option[str] = Nothing
     """Optional. URL to use for the link preview. If empty, then the first URL found 
-    in the message text will be used"""
+    in the message text will be used."""
 
     prefer_small_media: Option[bool] = Nothing
-    """Optional. True, if the media in the link preview is suppposed to be shrunk; 
+    """Optional. True, if the media in the link preview is supposed to be shrunk; 
     ignored if the URL isn't explicitly specified or media size change isn't 
-    supported for the preview"""
+    supported for the preview."""
 
     prefer_large_media: Option[bool] = Nothing
-    """Optional. True, if the media in the link preview is suppposed to be enlarged; 
+    """Optional. True, if the media in the link preview is supposed to be enlarged; 
     ignored if the URL isn't explicitly specified or media size change isn't 
-    supported for the preview"""
+    supported for the preview."""
 
     show_above_text: Option[bool] = Nothing
     """Optional. True, if the link preview must be shown above the message text; 
-    otherwise, the link preview will be shown below the message text"""
+    otherwise, the link preview will be shown below the message text."""
 
 
 class UserProfilePhotos(Model):
-    """Object `UserProfilePhotos`, see the [documentation](https://core.telegram.org/bots/api#userprofilephotos)
+    """Object `UserProfilePhotos`, see the [documentation](https://core.telegram.org/bots/api#userprofilephotos).
 
-    This object represent a user's profile pictures."""
+    This object represent a user's profile pictures.
+    """
 
     total_count: int
-    """Total number of profile pictures the target user has"""
+    """Total number of profile pictures the target user has."""
 
     photos: list[list["PhotoSize"]]
-    """Requested profile pictures (in up to 4 sizes each)"""
+    """Requested profile pictures (in up to 4 sizes each)."""
 
 
 class File(Model):
-    """Object `File`, see the [documentation](https://core.telegram.org/bots/api#file)
+    """Object `File`, see the [documentation](https://core.telegram.org/bots/api#file).
 
     This object represents a file ready to be downloaded. The file can be downloaded via the link https://api.telegram.org/file/bot<token>/<file_path>. It is guaranteed that the link will be valid for at least 1 hour. When the link expires, a new one can be requested by calling getFile.
     """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     file_size: Option[int] = Nothing
     """Optional. File size in bytes. It can be bigger than 2^31 and some programming 
@@ -1837,31 +2011,32 @@
 
     file_path: Option[str] = Nothing
     """Optional. File path. Use https://api.telegram.org/file/bot<token>/<file_path> 
     to get the file."""
 
 
 class WebAppInfo(Model):
-    """Object `WebAppInfo`, see the [documentation](https://core.telegram.org/bots/api#webappinfo)
+    """Object `WebAppInfo`, see the [documentation](https://core.telegram.org/bots/api#webappinfo).
 
-    Describes a Web App."""
+    Describes a Web App.
+    """
 
     url: str
     """An HTTPS URL of a Web App to be opened with additional data as specified in 
-    Initializing Web Apps"""
+    Initializing Web Apps."""
 
 
 class ReplyKeyboardMarkup(Model):
-    """Object `ReplyKeyboardMarkup`, see the [documentation](https://core.telegram.org/bots/api#replykeyboardmarkup)
+    """Object `ReplyKeyboardMarkup`, see the [documentation](https://core.telegram.org/bots/api#replykeyboardmarkup).
 
     This object represents a custom keyboard with reply options (see Introduction to bots for details and examples).
     """
 
     keyboard: list[list["KeyboardButton"]]
-    """Array of button rows, each represented by an Array of KeyboardButton objects"""
+    """Array of button rows, each represented by an Array of KeyboardButton objects."""
 
     is_persistent: Option[bool] = Nothing
     """Optional. Requests clients to always show the keyboard when the regular 
     keyboard is hidden. Defaults to false, in which case the custom keyboard 
     can be hidden and opened with a keyboard icon."""
 
     resize_keyboard: Option[bool] = Nothing
@@ -1874,35 +2049,41 @@
     """Optional. Requests clients to hide the keyboard as soon as it's been used. 
     The keyboard will still be available, but clients will automatically display 
     the usual letter-keyboard in the chat - the user can press a special button 
     in the input field to see the custom keyboard again. Defaults to false."""
 
     input_field_placeholder: Option[str] = Nothing
     """Optional. The placeholder to be shown in the input field when the keyboard 
-    is active; 1-64 characters"""
+    is active; 1-64 characters."""
 
     selective: Option[bool] = Nothing
     """Optional. Use this parameter if you want to show the keyboard to specific 
     users only. Targets: 1) users that are @mentioned in the text of the Message 
     object; 2) if the bot's message is a reply to a message in the same chat and 
     forum topic, sender of the original message. Example: A user requests to 
     change the bot's language, bot replies to the request with a keyboard to 
     select the new language. Other users in the group don't see the keyboard."""
 
+    @property
+    def empty_markup(self) -> "ReplyKeyboardRemove":
+        """Empty keyboard to remove the custom keyboard."""
+
+        return ReplyKeyboardRemove(remove_keyboard=True, selective=self.selective)
+
 
 class KeyboardButton(Model):
-    """Object `KeyboardButton`, see the [documentation](https://core.telegram.org/bots/api#keyboardbutton)
+    """Object `KeyboardButton`, see the [documentation](https://core.telegram.org/bots/api#keyboardbutton).
 
     This object represents one button of the reply keyboard. For simple text buttons, String can be used instead of this object to specify the button text. The optional fields web_app, request_users, request_chat, request_contact, request_location, and request_poll are mutually exclusive.
     Note: request_users and request_chat options will only work in Telegram versions released after 3 February, 2023. Older clients will display unsupported message.
     """
 
     text: str
     """Text of the button. If none of the optional fields are used, it will be sent 
-    as a message when the button is pressed"""
+    as a message when the button is pressed."""
 
     request_users: Option["KeyboardButtonRequestUsers"] = Nothing
     """Optional. If specified, pressing the button will open a list of suitable 
     users. Identifiers of selected users will be sent to the bot in a `users_shared` 
     service message. Available in private chats only."""
 
     request_chat: Option["KeyboardButtonRequestChat"] = Nothing
@@ -1925,45 +2106,54 @@
     web_app: Option["WebAppInfo"] = Nothing
     """Optional. If specified, the described Web App will be launched when the 
     button is pressed. The Web App will be able to send a `web_app_data` service 
     message. Available in private chats only."""
 
 
 class KeyboardButtonRequestUsers(Model):
-    """Object `KeyboardButtonRequestUsers`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonrequestusers)
+    """Object `KeyboardButtonRequestUsers`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonrequestusers).
 
-    This object defines the criteria used to request suitable users. The identifiers of the selected users will be shared with the bot when the corresponding button is pressed. More about requesting users: https://core.telegram.org/bots/features#chat-and-user-selection
+    This object defines the criteria used to request suitable users. Information about the selected users will be shared with the bot when the corresponding button is pressed. More about requesting users: https://core.telegram.org/bots/features#chat-and-user-selection
     """
 
     request_id: int
     """Signed 32-bit identifier of the request that will be received back in the 
-    UsersShared object. Must be unique within the message"""
+    UsersShared object. Must be unique within the message."""
 
     user_is_bot: Option[bool] = Nothing
     """Optional. Pass True to request bots, pass False to request regular users. 
     If not specified, no additional restrictions are applied."""
 
     user_is_premium: Option[bool] = Nothing
     """Optional. Pass True to request premium users, pass False to request non-premium 
     users. If not specified, no additional restrictions are applied."""
 
     max_quantity: Option[int] = Nothing
     """Optional. The maximum number of users to be selected; 1-10. Defaults to 
     1."""
 
+    request_name: Option[bool] = Nothing
+    """Optional. Pass True to request the users' first and last name."""
+
+    request_username: Option[bool] = Nothing
+    """Optional. Pass True to request the users' username."""
+
+    request_photo: Option[bool] = Nothing
+    """Optional. Pass True to request the users' photo."""
+
 
 class KeyboardButtonRequestChat(Model):
-    """Object `KeyboardButtonRequestChat`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonrequestchat)
+    """Object `KeyboardButtonRequestChat`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonrequestchat).
 
-    This object defines the criteria used to request a suitable chat. The identifier of the selected chat will be shared with the bot when the corresponding button is pressed. More about requesting chats: https://core.telegram.org/bots/features#chat-and-user-selection
+    This object defines the criteria used to request a suitable chat. Information about the selected chat will be shared with the bot when the corresponding button is pressed. The bot will be granted requested rights in the сhat if appropriate More about requesting chats: https://core.telegram.org/bots/features#chat-and-user-selection
     """
 
     request_id: int
     """Signed 32-bit identifier of the request, which will be received back in 
-    the ChatShared object. Must be unique within the message"""
+    the ChatShared object. Must be unique within the message."""
 
     chat_is_channel: bool
     """Pass True to request a channel chat, pass False to request a group or a supergroup 
     chat."""
 
     chat_is_forum: Option[bool] = Nothing
     """Optional. Pass True to request a forum supergroup, pass False to request 
@@ -1988,76 +2178,85 @@
     rights of the bot in the chat. The rights must be a subset of user_administrator_rights. 
     If not specified, no additional restrictions are applied."""
 
     bot_is_member: Option[bool] = Nothing
     """Optional. Pass True to request a chat with the bot as a member. Otherwise, 
     no additional restrictions are applied."""
 
+    request_title: Option[bool] = Nothing
+    """Optional. Pass True to request the chat's title."""
+
+    request_username: Option[bool] = Nothing
+    """Optional. Pass True to request the chat's username."""
+
+    request_photo: Option[bool] = Nothing
+    """Optional. Pass True to request the chat's photo."""
+
 
 class KeyboardButtonPollType(Model):
-    """Object `KeyboardButtonPollType`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonpolltype)
+    """Object `KeyboardButtonPollType`, see the [documentation](https://core.telegram.org/bots/api#keyboardbuttonpolltype).
 
     This object represents type of a poll, which is allowed to be created and sent when the corresponding button is pressed.
     """
 
-    type: Option[str] = Nothing
+    type: Option[typing.Literal["quiz", "regular"]] = Nothing
     """Optional. If quiz is passed, the user will be allowed to create only polls 
     in the quiz mode. If regular is passed, only regular polls will be allowed. 
     Otherwise, the user will be allowed to create a poll of any type."""
 
 
 class ReplyKeyboardRemove(Model):
-    """Object `ReplyKeyboardRemove`, see the [documentation](https://core.telegram.org/bots/api#replykeyboardremove)
+    """Object `ReplyKeyboardRemove`, see the [documentation](https://core.telegram.org/bots/api#replykeyboardremove).
 
     Upon receiving a message with this object, Telegram clients will remove the current custom keyboard and display the default letter-keyboard. By default, custom keyboards are displayed until a new keyboard is sent by a bot. An exception is made for one-time keyboards that are hidden immediately after the user presses a button (see ReplyKeyboardMarkup).
     """
 
     remove_keyboard: bool
     """Requests clients to remove the custom keyboard (user will not be able to 
     summon this keyboard; if you want to hide the keyboard from sight but keep 
-    it accessible, use one_time_keyboard in ReplyKeyboardMarkup)"""
+    it accessible, use one_time_keyboard in ReplyKeyboardMarkup)."""
 
     selective: Option[bool] = Nothing
     """Optional. Use this parameter if you want to remove the keyboard for specific 
     users only. Targets: 1) users that are @mentioned in the text of the Message 
     object; 2) if the bot's message is a reply to a message in the same chat and 
     forum topic, sender of the original message. Example: A user votes in a poll, 
     bot returns confirmation message in reply to the vote and removes the keyboard 
     for that user, while still showing the keyboard with poll options to users 
     who haven't voted yet."""
 
 
 class InlineKeyboardMarkup(Model):
-    """Object `InlineKeyboardMarkup`, see the [documentation](https://core.telegram.org/bots/api#inlinekeyboardmarkup)
+    """Object `InlineKeyboardMarkup`, see the [documentation](https://core.telegram.org/bots/api#inlinekeyboardmarkup).
 
     This object represents an inline keyboard that appears right next to the message it belongs to.
     """
 
     inline_keyboard: list[list["InlineKeyboardButton"]]
     """Array of button rows, each represented by an Array of InlineKeyboardButton 
-    objects"""
+    objects."""
 
 
 class InlineKeyboardButton(Model):
-    """Object `InlineKeyboardButton`, see the [documentation](https://core.telegram.org/bots/api#inlinekeyboardbutton)
+    """Object `InlineKeyboardButton`, see the [documentation](https://core.telegram.org/bots/api#inlinekeyboardbutton).
 
     This object represents one button of an inline keyboard. You must use exactly one of the optional fields.
     """
 
     text: str
-    """Label text on the button"""
+    """Label text on the button."""
 
     url: Option[str] = Nothing
     """Optional. HTTP or tg:// URL to be opened when the button is pressed. Links 
     tg://user?id=<user_id> can be used to mention a user by their identifier 
     without using a username, if this is allowed by their privacy settings."""
 
     callback_data: Option[str] = Nothing
     """Optional. Data to be sent in a callback query to the bot when button is pressed, 
-    1-64 bytes"""
+    1-64 bytes."""
 
     web_app: Option["WebAppInfo"] = Nothing
     """Optional. Description of the Web App that will be launched when the user 
     presses the button. The Web App will be able to send an arbitrary message 
     on behalf of the user using the method answerWebAppQuery. Available only 
     in private chats between a user and the bot."""
 
@@ -2077,32 +2276,33 @@
     in which case only the bot's username will be inserted. This offers a quick 
     way for the user to open your bot in inline mode in the same chat - good for selecting 
     something from multiple options."""
 
     switch_inline_query_chosen_chat: Option["SwitchInlineQueryChosenChat"] = Nothing
     """Optional. If set, pressing the button will prompt the user to select one 
     of their chats of the specified type, open that chat and insert the bot's 
-    username and the specified inline query in the input field"""
+    username and the specified inline query in the input field."""
 
     callback_game: Option["CallbackGame"] = Nothing
     """Optional. Description of the game that will be launched when the user presses 
     the button. NOTE: This type of button must always be the first button in the 
     first row."""
 
     pay: Option[bool] = Nothing
     """Optional. Specify True, to send a Pay button. NOTE: This type of button must 
     always be the first button in the first row and can only be used in invoice 
     messages."""
 
 
 class LoginUrl(Model):
-    """Object `LoginUrl`, see the [documentation](https://core.telegram.org/bots/api#loginurl)
+    """Object `LoginUrl`, see the [documentation](https://core.telegram.org/bots/api#loginurl).
 
     This object represents a parameter of the inline keyboard button used to automatically authorize a user. Serves as a great replacement for the Telegram Login Widget when the user is coming from Telegram. All the user needs to do is tap/click a button and confirm that they want to log in:
-    Telegram apps support these buttons as of version 5.7."""
+    Telegram apps support these buttons as of version 5.7.
+    """
 
     url: str
     """An HTTPS URL to be opened with user authorization data added to the query 
     string when the button is pressed. If the user refuses to provide authorization 
     data, the original URL without information about the user will be opened. 
     The data added is the same as described in Receiving authorization data. 
     NOTE: You must always check the hash of the received data to verify the authentication 
@@ -2119,94 +2319,95 @@
 
     request_write_access: Option[bool] = Nothing
     """Optional. Pass True to request the permission for your bot to send messages 
     to the user."""
 
 
 class SwitchInlineQueryChosenChat(Model):
-    """Object `SwitchInlineQueryChosenChat`, see the [documentation](https://core.telegram.org/bots/api#switchinlinequerychosenchat)
+    """Object `SwitchInlineQueryChosenChat`, see the [documentation](https://core.telegram.org/bots/api#switchinlinequerychosenchat).
 
     This object represents an inline button that switches the current user to inline mode in a chosen chat, with an optional default inline query.
     """
 
     query: Option[str] = Nothing
     """Optional. The default inline query to be inserted in the input field. If 
-    left empty, only the bot's username will be inserted"""
+    left empty, only the bot's username will be inserted."""
 
     allow_user_chats: Option[bool] = Nothing
-    """Optional. True, if private chats with users can be chosen"""
+    """Optional. True, if private chats with users can be chosen."""
 
     allow_bot_chats: Option[bool] = Nothing
-    """Optional. True, if private chats with bots can be chosen"""
+    """Optional. True, if private chats with bots can be chosen."""
 
     allow_group_chats: Option[bool] = Nothing
-    """Optional. True, if group and supergroup chats can be chosen"""
+    """Optional. True, if group and supergroup chats can be chosen."""
 
     allow_channel_chats: Option[bool] = Nothing
-    """Optional. True, if channel chats can be chosen"""
+    """Optional. True, if channel chats can be chosen."""
 
 
 class CallbackQuery(Model):
-    """Object `CallbackQuery`, see the [documentation](https://core.telegram.org/bots/api#callbackquery)
+    """Object `CallbackQuery`, see the [documentation](https://core.telegram.org/bots/api#callbackquery).
 
     This object represents an incoming callback query from a callback button in an inline keyboard. If the button that originated the query was attached to a message sent by the bot, the field message will be present. If the button was attached to a message sent via the bot (in inline mode), the field inline_message_id will be present. Exactly one of the fields data or game_short_name will be present.
     """
 
     id: str
-    """Unique identifier for this query"""
+    """Unique identifier for this query."""
 
     from_: "User"
-    """Sender"""
+    """Sender."""
 
     chat_instance: str
     """Global identifier, uniquely corresponding to the chat to which the message 
     with the callback button was sent. Useful for high scores in games."""
 
-    message: Option[Union["Message", "InaccessibleMessage"]] = Nothing
+    message: Option[Variative["Message", "InaccessibleMessage"]] = Nothing
     """Optional. Message sent by the bot with the callback button that originated 
-    the query"""
+    the query."""
 
     inline_message_id: Option[str] = Nothing
     """Optional. Identifier of the message sent via the bot in inline mode, that 
     originated the query."""
 
     data: Option[str] = Nothing
     """Optional. Data associated with the callback button. Be aware that the message 
     originated the query can contain no callback buttons with this data."""
 
     game_short_name: Option[str] = Nothing
     """Optional. Short name of a Game to be returned, serves as the unique identifier 
-    for the game"""
+    for the game."""
 
 
 class ForceReply(Model):
-    """Object `ForceReply`, see the [documentation](https://core.telegram.org/bots/api#forcereply)
+    """Object `ForceReply`, see the [documentation](https://core.telegram.org/bots/api#forcereply).
 
     Upon receiving a message with this object, Telegram clients will display a reply interface to the user (act as if the user has selected the bot's message and tapped 'Reply'). This can be extremely useful if you want to create user-friendly step-by-step interfaces without having to sacrifice privacy mode.
     """
 
     force_reply: bool
     """Shows reply interface to the user, as if they manually selected the bot's 
-    message and tapped 'Reply'"""
+    message and tapped 'Reply'."""
 
     input_field_placeholder: Option[str] = Nothing
     """Optional. The placeholder to be shown in the input field when the reply is 
-    active; 1-64 characters"""
+    active; 1-64 characters."""
 
     selective: Option[bool] = Nothing
     """Optional. Use this parameter if you want to force reply from specific users 
     only. Targets: 1) users that are @mentioned in the text of the Message object; 
     2) if the bot's message is a reply to a message in the same chat and forum topic, 
     sender of the original message."""
 
 
 class ChatPhoto(Model):
-    """Object `ChatPhoto`, see the [documentation](https://core.telegram.org/bots/api#chatphoto)
+    """Object `ChatPhoto`, see the [documentation](https://core.telegram.org/bots/api#chatphoto).
 
-    This object represents a chat photo."""
+    This object represents a chat photo.
+    """
 
     small_file_id: str
     """File identifier of small (160x160) chat photo. This file_id can be used 
     only for photo download and only for as long as the photo is not changed."""
 
     small_file_unique_id: str
     """Unique file identifier of small (160x160) chat photo, which is supposed 
@@ -2220,1153 +2421,1312 @@
     big_file_unique_id: str
     """Unique file identifier of big (640x640) chat photo, which is supposed to 
     be the same over time and for different bots. Can't be used to download or 
     reuse the file."""
 
 
 class ChatInviteLink(Model):
-    """Object `ChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#chatinvitelink)
+    """Object `ChatInviteLink`, see the [documentation](https://core.telegram.org/bots/api#chatinvitelink).
 
-    Represents an invite link for a chat."""
+    Represents an invite link for a chat.
+    """
 
     invite_link: str
     """The invite link. If the link was created by another chat administrator, 
     then the second part of the link will be replaced with `...`."""
 
     creator: "User"
-    """Creator of the link"""
+    """Creator of the link."""
 
     creates_join_request: bool
-    """True, if users joining the chat via the link need to be approved by chat administrators"""
+    """True, if users joining the chat via the link need to be approved by chat administrators."""
 
     is_primary: bool
-    """True, if the link is primary"""
+    """True, if the link is primary."""
 
     is_revoked: bool
-    """True, if the link is revoked"""
+    """True, if the link is revoked."""
 
     name: Option[str] = Nothing
-    """Optional. Invite link name"""
+    """Optional. Invite link name."""
 
-    expire_date: Option[int] = Nothing
+    expire_date: Option[datetime] = Nothing
     """Optional. Point in time (Unix timestamp) when the link will expire or has 
-    been expired"""
+    been expired."""
 
     member_limit: Option[int] = Nothing
     """Optional. The maximum number of users that can be members of the chat simultaneously 
-    after joining the chat via this invite link; 1-99999"""
+    after joining the chat via this invite link; 1-99999."""
 
     pending_join_request_count: Option[int] = Nothing
-    """Optional. Number of pending join requests created using this link"""
+    """Optional. Number of pending join requests created using this link."""
 
 
 class ChatAdministratorRights(Model):
-    """Object `ChatAdministratorRights`, see the [documentation](https://core.telegram.org/bots/api#chatadministratorrights)
+    """Object `ChatAdministratorRights`, see the [documentation](https://core.telegram.org/bots/api#chatadministratorrights).
 
-    Represents the rights of an administrator in a chat."""
+    Represents the rights of an administrator in a chat.
+    """
 
     is_anonymous: bool
-    """True, if the user's presence in the chat is hidden"""
+    """True, if the user's presence in the chat is hidden."""
 
     can_manage_chat: bool
-    """True, if the administrator can access the chat event log, boost list in channels, 
-    see channel members, report spam messages, see anonymous administrators 
-    in supergroups and ignore slow mode. Implied by any other administrator 
-    privilege"""
+    """True, if the administrator can access the chat event log, get boost list, 
+    see hidden supergroup and channel members, report spam messages and ignore 
+    slow mode. Implied by any other administrator privilege."""
 
     can_delete_messages: bool
-    """True, if the administrator can delete messages of other users"""
+    """True, if the administrator can delete messages of other users."""
 
     can_manage_video_chats: bool
-    """True, if the administrator can manage video chats"""
+    """True, if the administrator can manage video chats."""
 
     can_restrict_members: bool
     """True, if the administrator can restrict, ban or unban chat members, or access 
-    supergroup statistics"""
+    supergroup statistics."""
 
     can_promote_members: bool
     """True, if the administrator can add new administrators with a subset of their 
     own privileges or demote administrators that they have promoted, directly 
-    or indirectly (promoted by administrators that were appointed by the user)"""
+    or indirectly (promoted by administrators that were appointed by the user)."""
 
     can_change_info: bool
-    """True, if the user is allowed to change the chat title, photo and other settings"""
+    """True, if the user is allowed to change the chat title, photo and other settings."""
 
     can_invite_users: bool
-    """True, if the user is allowed to invite new users to the chat"""
+    """True, if the user is allowed to invite new users to the chat."""
+
+    can_post_stories: bool
+    """True, if the administrator can post stories to the chat."""
+
+    can_edit_stories: bool
+    """True, if the administrator can edit stories posted by other users."""
+
+    can_delete_stories: bool
+    """True, if the administrator can delete stories posted by other users."""
 
     can_post_messages: Option[bool] = Nothing
     """Optional. True, if the administrator can post messages in the channel, 
-    or access channel statistics; channels only"""
+    or access channel statistics; for channels only."""
 
     can_edit_messages: Option[bool] = Nothing
     """Optional. True, if the administrator can edit messages of other users and 
-    can pin messages; channels only"""
+    can pin messages; for channels only."""
 
     can_pin_messages: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to pin messages; groups and supergroups 
-    only"""
-
-    can_post_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can post stories in the channel; channels 
-    only"""
-
-    can_edit_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can edit stories posted by other users; 
-    channels only"""
-
-    can_delete_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can delete stories posted by other 
-    users; channels only"""
+    """Optional. True, if the user is allowed to pin messages; for groups and supergroups 
+    only."""
 
     can_manage_topics: Option[bool] = Nothing
     """Optional. True, if the user is allowed to create, rename, close, and reopen 
-    forum topics; supergroups only"""
+    forum topics; for supergroups only."""
 
 
 class ChatMemberUpdated(Model):
-    """Object `ChatMemberUpdated`, see the [documentation](https://core.telegram.org/bots/api#chatmemberupdated)
+    """Object `ChatMemberUpdated`, see the [documentation](https://core.telegram.org/bots/api#chatmemberupdated).
 
-    This object represents changes in the status of a chat member."""
+    This object represents changes in the status of a chat member.
+    """
 
     chat: "Chat"
-    """Chat the user belongs to"""
+    """Chat the user belongs to."""
 
     from_: "User"
-    """Performer of the action, which resulted in the change"""
+    """Performer of the action, which resulted in the change."""
 
-    date: int
-    """Date the change was done in Unix time"""
+    date: datetime
+    """Date the change was done in Unix time."""
 
-    old_chat_member: Union[
+    old_chat_member: Variative[
         "ChatMemberOwner",
         "ChatMemberAdministrator",
         "ChatMemberMember",
         "ChatMemberRestricted",
         "ChatMemberLeft",
         "ChatMemberBanned",
     ]
-    """Previous information about the chat member"""
+    """Previous information about the chat member."""
 
-    new_chat_member: Union[
+    new_chat_member: Variative[
         "ChatMemberOwner",
         "ChatMemberAdministrator",
         "ChatMemberMember",
         "ChatMemberRestricted",
         "ChatMemberLeft",
         "ChatMemberBanned",
     ]
-    """New information about the chat member"""
+    """New information about the chat member."""
 
     invite_link: Option["ChatInviteLink"] = Nothing
     """Optional. Chat invite link, which was used by the user to join the chat; for 
     joining by invite link events only."""
 
     via_chat_folder_invite_link: Option[bool] = Nothing
-    """Optional. True, if the user joined the chat via a chat folder invite link"""
+    """Optional. True, if the user joined the chat via a chat folder invite link."""
 
 
 class ChatMemberOwner(ChatMember):
-    """Object `ChatMemberOwner`, see the [documentation](https://core.telegram.org/bots/api#chatmemberowner)
+    """Object `ChatMemberOwner`, see the [documentation](https://core.telegram.org/bots/api#chatmemberowner).
 
-    Represents a chat member that owns the chat and has all administrator privileges."""
+    Represents a chat member that owns the chat and has all administrator privileges.
+    """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `creator`"""
+    status: typing.Literal["creator"]
+    """The member's status in the chat, always `creator`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
     is_anonymous: bool
-    """True, if the user's presence in the chat is hidden"""
+    """True, if the user's presence in the chat is hidden."""
 
     custom_title: Option[str] = Nothing
-    """Optional. Custom title for this user"""
+    """Optional. Custom title for this user."""
 
 
 class ChatMemberAdministrator(ChatMember):
-    """Object `ChatMemberAdministrator`, see the [documentation](https://core.telegram.org/bots/api#chatmemberadministrator)
+    """Object `ChatMemberAdministrator`, see the [documentation](https://core.telegram.org/bots/api#chatmemberadministrator).
 
-    Represents a chat member that has some additional privileges."""
+    Represents a chat member that has some additional privileges.
+    """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `administrator`"""
+    status: typing.Literal["administrator"]
+    """The member's status in the chat, always `administrator`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
     can_be_edited: bool
-    """True, if the bot is allowed to edit administrator privileges of that user"""
+    """True, if the bot is allowed to edit administrator privileges of that user."""
 
     is_anonymous: bool
-    """True, if the user's presence in the chat is hidden"""
+    """True, if the user's presence in the chat is hidden."""
 
     can_manage_chat: bool
-    """True, if the administrator can access the chat event log, boost list in channels, 
-    see channel members, report spam messages, see anonymous administrators 
-    in supergroups and ignore slow mode. Implied by any other administrator 
-    privilege"""
+    """True, if the administrator can access the chat event log, get boost list, 
+    see hidden supergroup and channel members, report spam messages and ignore 
+    slow mode. Implied by any other administrator privilege."""
 
     can_delete_messages: bool
-    """True, if the administrator can delete messages of other users"""
+    """True, if the administrator can delete messages of other users."""
 
     can_manage_video_chats: bool
-    """True, if the administrator can manage video chats"""
+    """True, if the administrator can manage video chats."""
 
     can_restrict_members: bool
     """True, if the administrator can restrict, ban or unban chat members, or access 
-    supergroup statistics"""
+    supergroup statistics."""
 
     can_promote_members: bool
     """True, if the administrator can add new administrators with a subset of their 
     own privileges or demote administrators that they have promoted, directly 
-    or indirectly (promoted by administrators that were appointed by the user)"""
+    or indirectly (promoted by administrators that were appointed by the user)."""
 
     can_change_info: bool
-    """True, if the user is allowed to change the chat title, photo and other settings"""
+    """True, if the user is allowed to change the chat title, photo and other settings."""
 
     can_invite_users: bool
-    """True, if the user is allowed to invite new users to the chat"""
+    """True, if the user is allowed to invite new users to the chat."""
+
+    can_post_stories: bool
+    """True, if the administrator can post stories to the chat."""
+
+    can_edit_stories: bool
+    """True, if the administrator can edit stories posted by other users."""
+
+    can_delete_stories: bool
+    """True, if the administrator can delete stories posted by other users."""
 
     can_post_messages: Option[bool] = Nothing
     """Optional. True, if the administrator can post messages in the channel, 
-    or access channel statistics; channels only"""
+    or access channel statistics; for channels only."""
 
     can_edit_messages: Option[bool] = Nothing
     """Optional. True, if the administrator can edit messages of other users and 
-    can pin messages; channels only"""
+    can pin messages; for channels only."""
 
     can_pin_messages: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to pin messages; groups and supergroups 
-    only"""
-
-    can_post_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can post stories in the channel; channels 
-    only"""
-
-    can_edit_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can edit stories posted by other users; 
-    channels only"""
-
-    can_delete_stories: Option[bool] = Nothing
-    """Optional. True, if the administrator can delete stories posted by other 
-    users; channels only"""
+    """Optional. True, if the user is allowed to pin messages; for groups and supergroups 
+    only."""
 
     can_manage_topics: Option[bool] = Nothing
     """Optional. True, if the user is allowed to create, rename, close, and reopen 
-    forum topics; supergroups only"""
+    forum topics; for supergroups only."""
 
     custom_title: Option[str] = Nothing
-    """Optional. Custom title for this user"""
+    """Optional. Custom title for this user."""
 
 
 class ChatMemberMember(ChatMember):
-    """Object `ChatMemberMember`, see the [documentation](https://core.telegram.org/bots/api#chatmembermember)
+    """Object `ChatMemberMember`, see the [documentation](https://core.telegram.org/bots/api#chatmembermember).
 
-    Represents a chat member that has no additional privileges or restrictions."""
+    Represents a chat member that has no additional privileges or restrictions.
+    """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `member`"""
+    status: typing.Literal["member"]
+    """The member's status in the chat, always `member`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
 
 class ChatMemberRestricted(ChatMember):
-    """Object `ChatMemberRestricted`, see the [documentation](https://core.telegram.org/bots/api#chatmemberrestricted)
+    """Object `ChatMemberRestricted`, see the [documentation](https://core.telegram.org/bots/api#chatmemberrestricted).
 
     Represents a chat member that is under certain restrictions in the chat. Supergroups only.
     """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `restricted`"""
+    status: typing.Literal["restricted"]
+    """The member's status in the chat, always `restricted`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
     is_member: bool
-    """True, if the user is a member of the chat at the moment of the request"""
+    """True, if the user is a member of the chat at the moment of the request."""
 
     can_send_messages: bool
     """True, if the user is allowed to send text messages, contacts, giveaways, 
-    giveaway winners, invoices, locations and venues"""
+    giveaway winners, invoices, locations and venues."""
 
     can_send_audios: bool
-    """True, if the user is allowed to send audios"""
+    """True, if the user is allowed to send audios."""
 
     can_send_documents: bool
-    """True, if the user is allowed to send documents"""
+    """True, if the user is allowed to send documents."""
 
     can_send_photos: bool
-    """True, if the user is allowed to send photos"""
+    """True, if the user is allowed to send photos."""
 
     can_send_videos: bool
-    """True, if the user is allowed to send videos"""
+    """True, if the user is allowed to send videos."""
 
     can_send_video_notes: bool
-    """True, if the user is allowed to send video notes"""
+    """True, if the user is allowed to send video notes."""
 
     can_send_voice_notes: bool
-    """True, if the user is allowed to send voice notes"""
+    """True, if the user is allowed to send voice notes."""
 
     can_send_polls: bool
-    """True, if the user is allowed to send polls"""
+    """True, if the user is allowed to send polls."""
 
     can_send_other_messages: bool
     """True, if the user is allowed to send animations, games, stickers and use 
-    inline bots"""
+    inline bots."""
 
     can_add_web_page_previews: bool
-    """True, if the user is allowed to add web page previews to their messages"""
+    """True, if the user is allowed to add web page previews to their messages."""
 
     can_change_info: bool
-    """True, if the user is allowed to change the chat title, photo and other settings"""
+    """True, if the user is allowed to change the chat title, photo and other settings."""
 
     can_invite_users: bool
-    """True, if the user is allowed to invite new users to the chat"""
+    """True, if the user is allowed to invite new users to the chat."""
 
     can_pin_messages: bool
-    """True, if the user is allowed to pin messages"""
+    """True, if the user is allowed to pin messages."""
 
     can_manage_topics: bool
-    """True, if the user is allowed to create forum topics"""
+    """True, if the user is allowed to create forum topics."""
 
-    until_date: int
+    until_date: datetime
     """Date when restrictions will be lifted for this user; Unix time. If 0, then 
-    the user is restricted forever"""
+    the user is restricted forever."""
 
 
 class ChatMemberLeft(ChatMember):
-    """Object `ChatMemberLeft`, see the [documentation](https://core.telegram.org/bots/api#chatmemberleft)
+    """Object `ChatMemberLeft`, see the [documentation](https://core.telegram.org/bots/api#chatmemberleft).
 
     Represents a chat member that isn't currently a member of the chat, but may join it themselves.
     """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `left`"""
+    status: typing.Literal["left"]
+    """The member's status in the chat, always `left`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
 
 class ChatMemberBanned(ChatMember):
-    """Object `ChatMemberBanned`, see the [documentation](https://core.telegram.org/bots/api#chatmemberbanned)
+    """Object `ChatMemberBanned`, see the [documentation](https://core.telegram.org/bots/api#chatmemberbanned).
 
     Represents a chat member that was banned in the chat and can't return to the chat or view chat messages.
     """
 
-    status: ChatMemberStatus
-    """The member's status in the chat, always `kicked`"""
+    status: typing.Literal["kicked"]
+    """The member's status in the chat, always `kicked`."""
 
     user: "User"
-    """Information about the user"""
+    """Information about the user."""
 
-    until_date: int
+    until_date: datetime
     """Date when restrictions will be lifted for this user; Unix time. If 0, then 
-    the user is banned forever"""
+    the user is banned forever."""
 
 
 class ChatJoinRequest(Model):
-    """Object `ChatJoinRequest`, see the [documentation](https://core.telegram.org/bots/api#chatjoinrequest)
+    """Object `ChatJoinRequest`, see the [documentation](https://core.telegram.org/bots/api#chatjoinrequest).
 
-    Represents a join request sent to a chat."""
+    Represents a join request sent to a chat.
+    """
 
     chat: "Chat"
-    """Chat to which the request was sent"""
+    """Chat to which the request was sent."""
 
     from_: "User"
-    """User that sent the join request"""
+    """User that sent the join request."""
 
     user_chat_id: int
     """Identifier of a private chat with the user who sent the join request. This 
     number may have more than 32 significant bits and some programming languages 
     may have difficulty/silent defects in interpreting it. But it has at most 
     52 significant bits, so a 64-bit integer or double-precision float type 
     are safe for storing this identifier. The bot can use this identifier for 
     5 minutes to send messages until the join request is processed, assuming 
     no other administrator contacted the user."""
 
-    date: int
-    """Date the request was sent in Unix time"""
+    date: datetime
+    """Date the request was sent in Unix time."""
 
     bio: Option[str] = Nothing
     """Optional. Bio of the user."""
 
     invite_link: Option["ChatInviteLink"] = Nothing
-    """Optional. Chat invite link that was used by the user to send the join request"""
+    """Optional. Chat invite link that was used by the user to send the join request."""
 
 
 class ChatPermissions(Model):
-    """Object `ChatPermissions`, see the [documentation](https://core.telegram.org/bots/api#chatpermissions)
+    """Object `ChatPermissions`, see the [documentation](https://core.telegram.org/bots/api#chatpermissions).
 
-    Describes actions that a non-administrator user is allowed to take in a chat."""
+    Describes actions that a non-administrator user is allowed to take in a chat.
+    """
 
     can_send_messages: Option[bool] = Nothing
     """Optional. True, if the user is allowed to send text messages, contacts, 
-    giveaways, giveaway winners, invoices, locations and venues"""
+    giveaways, giveaway winners, invoices, locations and venues."""
 
     can_send_audios: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send audios"""
+    """Optional. True, if the user is allowed to send audios."""
 
     can_send_documents: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send documents"""
+    """Optional. True, if the user is allowed to send documents."""
 
     can_send_photos: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send photos"""
+    """Optional. True, if the user is allowed to send photos."""
 
     can_send_videos: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send videos"""
+    """Optional. True, if the user is allowed to send videos."""
 
     can_send_video_notes: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send video notes"""
+    """Optional. True, if the user is allowed to send video notes."""
 
     can_send_voice_notes: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send voice notes"""
+    """Optional. True, if the user is allowed to send voice notes."""
 
     can_send_polls: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to send polls"""
+    """Optional. True, if the user is allowed to send polls."""
 
     can_send_other_messages: Option[bool] = Nothing
     """Optional. True, if the user is allowed to send animations, games, stickers 
-    and use inline bots"""
+    and use inline bots."""
 
     can_add_web_page_previews: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to add web page previews to their messages"""
+    """Optional. True, if the user is allowed to add web page previews to their messages."""
 
     can_change_info: Option[bool] = Nothing
     """Optional. True, if the user is allowed to change the chat title, photo and 
-    other settings. Ignored in public supergroups"""
+    other settings. Ignored in public supergroups."""
 
     can_invite_users: Option[bool] = Nothing
-    """Optional. True, if the user is allowed to invite new users to the chat"""
+    """Optional. True, if the user is allowed to invite new users to the chat."""
 
     can_pin_messages: Option[bool] = Nothing
     """Optional. True, if the user is allowed to pin messages. Ignored in public 
-    supergroups"""
+    supergroups."""
 
     can_manage_topics: Option[bool] = Nothing
     """Optional. True, if the user is allowed to create forum topics. If omitted 
-    defaults to the value of can_pin_messages"""
+    defaults to the value of can_pin_messages."""
+
+
+class Birthdate(Model):
+    """Object `Birthdate`, see the [documentation](https://core.telegram.org/bots/api#birthdate).
+
+    No description yet.
+    """
+
+    day: int
+    """Day of the user's birth; 1-31."""
+
+    month: int
+    """Month of the user's birth; 1-12."""
+
+    year: Option[int] = Nothing
+    """Optional. Year of the user's birth."""
+
+    @property
+    def is_birthday(self) -> bool:
+        """True, if today is a user's birthday."""
+
+        now = datetime.now()
+        return now.month == self.month and now.day == self.day
+
+    @property
+    def age(self) -> Option[int]:
+        """Optional. Contains the user's age, if the user has a birth year specified."""
+
+        return self.year.map(
+            lambda year: (
+                (datetime.now() - datetime(year, self.month, self.day)) // 365
+            ).days
+        )
+
+
+class BusinessIntro(Model):
+    """Object `BusinessIntro`, see the [documentation](https://core.telegram.org/bots/api#businessintro).
+
+    No description yet.
+    """
+
+    title: Option[str] = Nothing
+    """Optional. Title text of the business intro."""
+
+    message: Option[str] = Nothing
+    """Optional. Message text of the business intro."""
+
+    sticker: Option["Sticker"] = Nothing
+    """Optional. Sticker of the business intro."""
+
+
+class BusinessLocation(Model):
+    """Object `BusinessLocation`, see the [documentation](https://core.telegram.org/bots/api#businesslocation).
+
+    No description yet.
+    """
+
+    address: str
+    """Address of the business."""
+
+    location: Option["Location"] = Nothing
+    """Optional. Location of the business."""
+
+
+class BusinessOpeningHoursInterval(Model):
+    """Object `BusinessOpeningHoursInterval`, see the [documentation](https://core.telegram.org/bots/api#businessopeninghoursinterval).
+
+    No description yet.
+    """
+
+    opening_minute: int
+    """The minute's sequence number in a week, starting on Monday, marking the 
+    start of the time interval during which the business is open; 0 - 7 * 24 * 60."""
+
+    closing_minute: int
+    """The minute's sequence number in a week, starting on Monday, marking the 
+    end of the time interval during which the business is open; 0 - 8 * 24 * 60."""
+
+
+class BusinessOpeningHours(Model):
+    """Object `BusinessOpeningHours`, see the [documentation](https://core.telegram.org/bots/api#businessopeninghours).
+
+    No description yet.
+    """
+
+    time_zone_name: str
+    """Unique name of the time zone for which the opening hours are defined."""
+
+    opening_hours: list["BusinessOpeningHoursInterval"]
+    """List of time intervals describing business opening hours."""
 
 
 class ChatLocation(Model):
-    """Object `ChatLocation`, see the [documentation](https://core.telegram.org/bots/api#chatlocation)
+    """Object `ChatLocation`, see the [documentation](https://core.telegram.org/bots/api#chatlocation).
 
-    Represents a location to which a chat is connected."""
+    Represents a location to which a chat is connected.
+    """
 
     location: "Location"
     """The location to which the supergroup is connected. Can't be a live location."""
 
     address: str
-    """Location address; 1-64 characters, as defined by the chat owner"""
+    """Location address; 1-64 characters, as defined by the chat owner."""
 
 
 class ReactionTypeEmoji(ReactionType):
-    """Object `ReactionTypeEmoji`, see the [documentation](https://core.telegram.org/bots/api#reactiontypeemoji)
+    """Object `ReactionTypeEmoji`, see the [documentation](https://core.telegram.org/bots/api#reactiontypeemoji).
 
-    The reaction is based on an emoji."""
+    The reaction is based on an emoji.
+    """
 
-    type: ReactionTypeType
-    """Type of the reaction, always `emoji`"""
+    type: typing.Literal["emoji"]
+    """Type of the reaction, always `emoji`."""
 
-    emoji: str
+    emoji: ReactionEmoji
     """Reaction emoji. Currently, it can be one of `👍`, `👎`, `❤`, `🔥`, `🥰`, `👏`, 
     `😁`, `🤔`, `🤯`, `😱`, `🤬`, `😢`, `🎉`, `🤩`, `🤮`, `💩`, `🙏`, `👌`, `🕊`, `🤡`, `🥱`, 
     `🥴`, `😍`, `🐳`, `❤‍🔥`, `🌚`, `🌭`, `💯`, `🤣`, `⚡`, `🍌`, `🏆`, `💔`, `🤨`, `😐`, `🍓`, 
     `🍾`, `💋`, `🖕`, `😈`, `😴`, `😭`, `🤓`, `👻`, `👨‍💻`, `👀`, `🎃`, `🙈`, `😇`, `😨`, `🤝`, 
     `✍`, `🤗`, `🫡`, `🎅`, `🎄`, `☃`, `💅`, `🤪`, `🗿`, `🆒`, `💘`, `🙉`, `🦄`, `😘`, `💊`, 
-    `🙊`, `😎`, `👾`, `🤷‍♂`, `🤷`, `🤷‍♀`, `😡`"""
+    `🙊`, `😎`, `👾`, `🤷‍♂`, `🤷`, `🤷‍♀`, `😡`."""
 
 
 class ReactionTypeCustomEmoji(ReactionType):
-    """Object `ReactionTypeCustomEmoji`, see the [documentation](https://core.telegram.org/bots/api#reactiontypecustomemoji)
+    """Object `ReactionTypeCustomEmoji`, see the [documentation](https://core.telegram.org/bots/api#reactiontypecustomemoji).
 
-    The reaction is based on a custom emoji."""
+    The reaction is based on a custom emoji.
+    """
 
-    type: ReactionTypeType
-    """Type of the reaction, always `custom_emoji`"""
+    type: typing.Literal["custom_emoji"]
+    """Type of the reaction, always `custom_emoji`."""
 
     custom_emoji_id: str
-    """Custom emoji identifier"""
+    """Custom emoji identifier."""
 
 
 class ReactionCount(Model):
-    """Object `ReactionCount`, see the [documentation](https://core.telegram.org/bots/api#reactioncount)
+    """Object `ReactionCount`, see the [documentation](https://core.telegram.org/bots/api#reactioncount).
 
     Represents a reaction added to a message along with the number of times it was added.
     """
 
-    type: Union["ReactionTypeEmoji", "ReactionTypeCustomEmoji"]
-    """Type of the reaction"""
+    type: Variative["ReactionTypeEmoji", "ReactionTypeCustomEmoji"]
+    """Type of the reaction."""
 
     total_count: int
-    """Number of times the reaction was added"""
+    """Number of times the reaction was added."""
 
 
 class MessageReactionUpdated(Model):
-    """Object `MessageReactionUpdated`, see the [documentation](https://core.telegram.org/bots/api#messagereactionupdated)
+    """Object `MessageReactionUpdated`, see the [documentation](https://core.telegram.org/bots/api#messagereactionupdated).
 
-    This object represents a change of a reaction on a message performed by a user."""
+    This object represents a change of a reaction on a message performed by a user.
+    """
 
     chat: "Chat"
-    """The chat containing the message the user reacted to"""
+    """The chat containing the message the user reacted to."""
 
     message_id: int
-    """Unique identifier of the message inside the chat"""
+    """Unique identifier of the message inside the chat."""
 
-    date: int
-    """Date of the change in Unix time"""
+    date: datetime
+    """Date of the change in Unix time."""
 
-    old_reaction: list["ReactionType"]
-    """Previous list of reaction types that were set by the user"""
+    old_reaction: list[Variative["ReactionTypeEmoji", "ReactionTypeCustomEmoji"]]
+    """Previous list of reaction types that were set by the user."""
 
-    new_reaction: list["ReactionType"]
-    """New list of reaction types that have been set by the user"""
+    new_reaction: list[Variative["ReactionTypeEmoji", "ReactionTypeCustomEmoji"]]
+    """New list of reaction types that have been set by the user."""
 
     user: Option["User"] = Nothing
-    """Optional. The user that changed the reaction, if the user isn't anonymous"""
+    """Optional. The user that changed the reaction, if the user isn't anonymous."""
 
     actor_chat: Option["Chat"] = Nothing
     """Optional. The chat on behalf of which the reaction was changed, if the user 
-    is anonymous"""
+    is anonymous."""
 
 
 class MessageReactionCountUpdated(Model):
-    """Object `MessageReactionCountUpdated`, see the [documentation](https://core.telegram.org/bots/api#messagereactioncountupdated)
+    """Object `MessageReactionCountUpdated`, see the [documentation](https://core.telegram.org/bots/api#messagereactioncountupdated).
 
-    This object represents reaction changes on a message with anonymous reactions."""
+    This object represents reaction changes on a message with anonymous reactions.
+    """
 
     chat: "Chat"
-    """The chat containing the message"""
+    """The chat containing the message."""
 
     message_id: int
-    """Unique message identifier inside the chat"""
+    """Unique message identifier inside the chat."""
 
-    date: int
-    """Date of the change in Unix time"""
+    date: datetime
+    """Date of the change in Unix time."""
 
     reactions: list["ReactionCount"]
-    """List of reactions that are present on the message"""
+    """List of reactions that are present on the message."""
 
 
 class ForumTopic(Model):
-    """Object `ForumTopic`, see the [documentation](https://core.telegram.org/bots/api#forumtopic)
+    """Object `ForumTopic`, see the [documentation](https://core.telegram.org/bots/api#forumtopic).
 
-    This object represents a forum topic."""
+    This object represents a forum topic.
+    """
 
     message_thread_id: int
-    """Unique identifier of the forum topic"""
+    """Unique identifier of the forum topic."""
 
     name: str
-    """Name of the topic"""
+    """Name of the topic."""
 
-    icon_color: int
-    """Color of the topic icon in RGB format"""
+    icon_color: TopicIconColor
+    """Color of the topic icon in RGB format."""
 
     icon_custom_emoji_id: Option[str] = Nothing
-    """Optional. Unique identifier of the custom emoji shown as the topic icon"""
+    """Optional. Unique identifier of the custom emoji shown as the topic icon."""
 
 
 class BotCommand(Model):
-    """Object `BotCommand`, see the [documentation](https://core.telegram.org/bots/api#botcommand)
+    """Object `BotCommand`, see the [documentation](https://core.telegram.org/bots/api#botcommand).
 
-    This object represents a bot command."""
+    This object represents a bot command.
+    """
 
     command: str
     """Text of the command; 1-32 characters. Can contain only lowercase English 
     letters, digits and underscores."""
 
     description: str
     """Description of the command; 1-256 characters."""
 
 
 class BotCommandScopeDefault(BotCommandScope):
-    """Object `BotCommandScopeDefault`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopedefault)
+    """Object `BotCommandScopeDefault`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopedefault).
 
     Represents the default scope of bot commands. Default commands are used if no commands with a narrower scope are specified for the user.
     """
 
-    type: BotCommandScopeType
-    """Scope type, must be default"""
+    type: typing.Literal["default"]
+    """Scope type, must be default."""
 
 
 class BotCommandScopeAllPrivateChats(BotCommandScope):
-    """Object `BotCommandScopeAllPrivateChats`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallprivatechats)
+    """Object `BotCommandScopeAllPrivateChats`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallprivatechats).
 
-    Represents the scope of bot commands, covering all private chats."""
+    Represents the scope of bot commands, covering all private chats.
+    """
 
-    type: BotCommandScopeType
-    """Scope type, must be all_private_chats"""
+    type: typing.Literal["all_private_chats"]
+    """Scope type, must be all_private_chats."""
 
 
 class BotCommandScopeAllGroupChats(BotCommandScope):
-    """Object `BotCommandScopeAllGroupChats`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallgroupchats)
+    """Object `BotCommandScopeAllGroupChats`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallgroupchats).
 
-    Represents the scope of bot commands, covering all group and supergroup chats."""
+    Represents the scope of bot commands, covering all group and supergroup chats.
+    """
 
-    type: BotCommandScopeType
-    """Scope type, must be all_group_chats"""
+    type: typing.Literal["all_group_chats"]
+    """Scope type, must be all_group_chats."""
 
 
 class BotCommandScopeAllChatAdministrators(BotCommandScope):
-    """Object `BotCommandScopeAllChatAdministrators`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallchatadministrators)
+    """Object `BotCommandScopeAllChatAdministrators`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopeallchatadministrators).
 
     Represents the scope of bot commands, covering all group and supergroup chat administrators.
     """
 
-    type: BotCommandScopeType
-    """Scope type, must be all_chat_administrators"""
+    type: typing.Literal["all_chat_administrators"]
+    """Scope type, must be all_chat_administrators."""
 
 
 class BotCommandScopeChat(BotCommandScope):
-    """Object `BotCommandScopeChat`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechat)
+    """Object `BotCommandScopeChat`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechat).
 
-    Represents the scope of bot commands, covering a specific chat."""
+    Represents the scope of bot commands, covering a specific chat.
+    """
 
-    type: BotCommandScopeType
-    """Scope type, must be chat"""
+    type: typing.Literal["chat"]
+    """Scope type, must be chat."""
 
-    chat_id: int | str
+    chat_id: Variative[int, str]
     """Unique identifier for the target chat or username of the target supergroup 
-    (in the format @supergroupusername)"""
+    (in the format @supergroupusername)."""
 
 
 class BotCommandScopeChatAdministrators(BotCommandScope):
-    """Object `BotCommandScopeChatAdministrators`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechatadministrators)
+    """Object `BotCommandScopeChatAdministrators`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechatadministrators).
 
     Represents the scope of bot commands, covering all administrators of a specific group or supergroup chat.
     """
 
-    type: BotCommandScopeType
-    """Scope type, must be chat_administrators"""
+    type: typing.Literal["chat_administrators"]
+    """Scope type, must be chat_administrators."""
 
-    chat_id: int | str
+    chat_id: Variative[int, str]
     """Unique identifier for the target chat or username of the target supergroup 
-    (in the format @supergroupusername)"""
+    (in the format @supergroupusername)."""
 
 
 class BotCommandScopeChatMember(BotCommandScope):
-    """Object `BotCommandScopeChatMember`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechatmember)
+    """Object `BotCommandScopeChatMember`, see the [documentation](https://core.telegram.org/bots/api#botcommandscopechatmember).
 
     Represents the scope of bot commands, covering a specific member of a group or supergroup chat.
     """
 
-    type: BotCommandScopeType
-    """Scope type, must be chat_member"""
+    type: typing.Literal["chat_member"]
+    """Scope type, must be chat_member."""
 
-    chat_id: int | str
+    chat_id: Variative[int, str]
     """Unique identifier for the target chat or username of the target supergroup 
-    (in the format @supergroupusername)"""
+    (in the format @supergroupusername)."""
 
     user_id: int
-    """Unique identifier of the target user"""
+    """Unique identifier of the target user."""
 
 
 class BotName(Model):
-    """Object `BotName`, see the [documentation](https://core.telegram.org/bots/api#botname)
+    """Object `BotName`, see the [documentation](https://core.telegram.org/bots/api#botname).
 
-    This object represents the bot's name."""
+    This object represents the bot's name.
+    """
 
     name: str
-    """The bot's name"""
+    """The bot's name."""
 
 
 class BotDescription(Model):
-    """Object `BotDescription`, see the [documentation](https://core.telegram.org/bots/api#botdescription)
+    """Object `BotDescription`, see the [documentation](https://core.telegram.org/bots/api#botdescription).
 
-    This object represents the bot's description."""
+    This object represents the bot's description.
+    """
 
     description: str
-    """The bot's description"""
+    """The bot's description."""
 
 
 class BotShortDescription(Model):
-    """Object `BotShortDescription`, see the [documentation](https://core.telegram.org/bots/api#botshortdescription)
+    """Object `BotShortDescription`, see the [documentation](https://core.telegram.org/bots/api#botshortdescription).
 
-    This object represents the bot's short description."""
+    This object represents the bot's short description.
+    """
 
     short_description: str
-    """The bot's short description"""
+    """The bot's short description."""
 
 
 class MenuButtonCommands(MenuButton):
-    """Object `MenuButtonCommands`, see the [documentation](https://core.telegram.org/bots/api#menubuttoncommands)
+    """Object `MenuButtonCommands`, see the [documentation](https://core.telegram.org/bots/api#menubuttoncommands).
 
-    Represents a menu button, which opens the bot's list of commands."""
+    Represents a menu button, which opens the bot's list of commands.
+    """
 
-    type: MenuButtonType
-    """Type of the button, must be commands"""
+    type: typing.Literal["commands"]
+    """Type of the button, must be commands."""
 
 
 class MenuButtonWebApp(MenuButton):
-    """Object `MenuButtonWebApp`, see the [documentation](https://core.telegram.org/bots/api#menubuttonwebapp)
+    """Object `MenuButtonWebApp`, see the [documentation](https://core.telegram.org/bots/api#menubuttonwebapp).
 
-    Represents a menu button, which launches a Web App."""
+    Represents a menu button, which launches a Web App.
+    """
 
-    type: MenuButtonType
-    """Type of the button, must be web_app"""
+    type: typing.Literal["web_app"]
+    """Type of the button, must be web_app."""
 
     text: str
-    """Text on the button"""
+    """Text on the button."""
 
     web_app: "WebAppInfo"
     """Description of the Web App that will be launched when the user presses the 
     button. The Web App will be able to send an arbitrary message on behalf of 
     the user using the method answerWebAppQuery."""
 
 
 class MenuButtonDefault(MenuButton):
-    """Object `MenuButtonDefault`, see the [documentation](https://core.telegram.org/bots/api#menubuttondefault)
+    """Object `MenuButtonDefault`, see the [documentation](https://core.telegram.org/bots/api#menubuttondefault).
 
-    Describes that no specific value for the menu button was set."""
+    Describes that no specific value for the menu button was set.
+    """
 
-    type: MenuButtonType
-    """Type of the button, must be default"""
+    type: typing.Literal["default"]
+    """Type of the button, must be default."""
 
 
 class ChatBoostSourcePremium(ChatBoostSource):
-    """Object `ChatBoostSourcePremium`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcepremium)
+    """Object `ChatBoostSourcePremium`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcepremium).
 
     The boost was obtained by subscribing to Telegram Premium or by gifting a Telegram Premium subscription to another user.
     """
 
-    source: ChatBoostSourceType
-    """Source of the boost, always `premium`"""
+    source: typing.Literal["premium"]
+    """Source of the boost, always `premium`."""
 
     user: "User"
-    """User that boosted the chat"""
+    """User that boosted the chat."""
 
 
 class ChatBoostSourceGiftCode(ChatBoostSource):
-    """Object `ChatBoostSourceGiftCode`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcegiftcode)
+    """Object `ChatBoostSourceGiftCode`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcegiftcode).
 
     The boost was obtained by the creation of Telegram Premium gift codes to boost a chat. Each such code boosts the chat 4 times for the duration of the corresponding Telegram Premium subscription.
     """
 
-    source: ChatBoostSourceType
-    """Source of the boost, always `gift_code`"""
+    source: typing.Literal["gift_code"]
+    """Source of the boost, always `gift_code`."""
 
     user: "User"
-    """User for which the gift code was created"""
+    """User for which the gift code was created."""
 
 
 class ChatBoostSourceGiveaway(ChatBoostSource):
-    """Object `ChatBoostSourceGiveaway`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcegiveaway)
+    """Object `ChatBoostSourceGiveaway`, see the [documentation](https://core.telegram.org/bots/api#chatboostsourcegiveaway).
 
     The boost was obtained by the creation of a Telegram Premium giveaway. This boosts the chat 4 times for the duration of the corresponding Telegram Premium subscription.
     """
 
-    source: ChatBoostSourceType
-    """Source of the boost, always `giveaway`"""
+    source: typing.Literal["giveaway"]
+    """Source of the boost, always `giveaway`."""
 
     giveaway_message_id: int
     """Identifier of a message in the chat with the giveaway; the message could 
     have been deleted already. May be 0 if the message isn't sent yet."""
 
     user: Option["User"] = Nothing
-    """Optional. User that won the prize in the giveaway if any"""
+    """Optional. User that won the prize in the giveaway if any."""
 
     is_unclaimed: Option[bool] = Nothing
     """Optional. True, if the giveaway was completed, but there was no user to win 
-    the prize"""
+    the prize."""
 
 
 class ChatBoost(Model):
-    """Object `ChatBoost`, see the [documentation](https://core.telegram.org/bots/api#chatboost)
+    """Object `ChatBoost`, see the [documentation](https://core.telegram.org/bots/api#chatboost).
 
-    This object contains information about a chat boost."""
+    This object contains information about a chat boost.
+    """
 
     boost_id: str
-    """Unique identifier of the boost"""
+    """Unique identifier of the boost."""
 
-    add_date: int
-    """Point in time (Unix timestamp) when the chat was boosted"""
+    add_date: datetime
+    """Point in time (Unix timestamp) when the chat was boosted."""
 
-    expiration_date: int
+    expiration_date: datetime
     """Point in time (Unix timestamp) when the boost will automatically expire, 
-    unless the booster's Telegram Premium subscription is prolonged"""
+    unless the booster's Telegram Premium subscription is prolonged."""
 
-    source: Union[
+    source: Variative[
         "ChatBoostSourcePremium", "ChatBoostSourceGiftCode", "ChatBoostSourceGiveaway"
     ]
-    """Source of the added boost"""
+    """Source of the added boost."""
 
 
 class ChatBoostUpdated(Model):
-    """Object `ChatBoostUpdated`, see the [documentation](https://core.telegram.org/bots/api#chatboostupdated)
+    """Object `ChatBoostUpdated`, see the [documentation](https://core.telegram.org/bots/api#chatboostupdated).
 
-    This object represents a boost added to a chat or changed."""
+    This object represents a boost added to a chat or changed.
+    """
 
     chat: "Chat"
-    """Chat which was boosted"""
+    """Chat which was boosted."""
 
     boost: "ChatBoost"
-    """Infomation about the chat boost"""
+    """Information about the chat boost."""
 
 
 class ChatBoostRemoved(Model):
-    """Object `ChatBoostRemoved`, see the [documentation](https://core.telegram.org/bots/api#chatboostremoved)
+    """Object `ChatBoostRemoved`, see the [documentation](https://core.telegram.org/bots/api#chatboostremoved).
 
-    This object represents a boost removed from a chat."""
+    This object represents a boost removed from a chat.
+    """
 
     chat: "Chat"
-    """Chat which was boosted"""
+    """Chat which was boosted."""
 
     boost_id: str
-    """Unique identifier of the boost"""
+    """Unique identifier of the boost."""
 
-    remove_date: int
-    """Point in time (Unix timestamp) when the boost was removed"""
+    remove_date: datetime
+    """Point in time (Unix timestamp) when the boost was removed."""
 
-    source: Union[
+    source: Variative[
         "ChatBoostSourcePremium", "ChatBoostSourceGiftCode", "ChatBoostSourceGiveaway"
     ]
-    """Source of the removed boost"""
+    """Source of the removed boost."""
 
 
 class UserChatBoosts(Model):
-    """Object `UserChatBoosts`, see the [documentation](https://core.telegram.org/bots/api#userchatboosts)
+    """Object `UserChatBoosts`, see the [documentation](https://core.telegram.org/bots/api#userchatboosts).
 
-    This object represents a list of boosts added to a chat by a user."""
+    This object represents a list of boosts added to a chat by a user.
+    """
 
     boosts: list["ChatBoost"]
-    """The list of boosts added to the chat by the user"""
+    """The list of boosts added to the chat by the user."""
+
+
+class BusinessConnection(Model):
+    """Object `BusinessConnection`, see the [documentation](https://core.telegram.org/bots/api#businessconnection).
+
+    Describes the connection of the bot with a business account.
+    """
+
+    id: str
+    """Unique identifier of the business connection."""
+
+    user: "User"
+    """Business account user that created the business connection."""
+
+    user_chat_id: int
+    """Identifier of a private chat with the user who created the business connection. 
+    This number may have more than 32 significant bits and some programming 
+    languages may have difficulty/silent defects in interpreting it. But 
+    it has at most 52 significant bits, so a 64-bit integer or double-precision 
+    float type are safe for storing this identifier."""
+
+    date: datetime
+    """Date the connection was established in Unix time."""
+
+    can_reply: bool
+    """True, if the bot can act on behalf of the business account in chats that were 
+    active in the last 24 hours."""
+
+    is_enabled: bool
+    """True, if the connection is active."""
+
+
+class BusinessMessagesDeleted(Model):
+    """Object `BusinessMessagesDeleted`, see the [documentation](https://core.telegram.org/bots/api#businessmessagesdeleted).
+
+    This object is received when messages are deleted from a connected business account.
+    """
+
+    business_connection_id: str
+    """Unique identifier of the business connection."""
+
+    chat: "Chat"
+    """Information about a chat in the business account. The bot may not have access 
+    to the chat or the corresponding user."""
+
+    message_ids: list[int]
+    """A JSON-serialized list of identifiers of deleted messages in the chat of 
+    the business account."""
 
 
 class ResponseParameters(Model):
-    """Object `ResponseParameters`, see the [documentation](https://core.telegram.org/bots/api#responseparameters)
+    """Object `ResponseParameters`, see the [documentation](https://core.telegram.org/bots/api#responseparameters).
 
-    Describes why a request was unsuccessful."""
+    Describes why a request was unsuccessful.
+    """
 
     migrate_to_chat_id: Option[int] = Nothing
     """Optional. The group has been migrated to a supergroup with the specified 
     identifier. This number may have more than 32 significant bits and some 
     programming languages may have difficulty/silent defects in interpreting 
     it. But it has at most 52 significant bits, so a signed 64-bit integer or double-precision 
     float type are safe for storing this identifier."""
 
     retry_after: Option[int] = Nothing
     """Optional. In case of exceeding flood control, the number of seconds left 
-    to wait before the request can be repeated"""
+    to wait before the request can be repeated."""
 
 
 class InputMediaPhoto(InputMedia):
-    """Object `InputMediaPhoto`, see the [documentation](https://core.telegram.org/bots/api#inputmediaphoto)
+    """Object `InputMediaPhoto`, see the [documentation](https://core.telegram.org/bots/api#inputmediaphoto).
 
-    Represents a photo to be sent."""
+    Represents a photo to be sent.
+    """
 
-    type: InputMediaType
-    """Type of the result, must be photo"""
+    type: typing.Literal["photo"]
+    """Type of the result, must be photo."""
 
-    media: str
+    media: Variative["InputFile", str]
     """File to send. Pass a file_id to send a file that exists on the Telegram servers 
     (recommended), pass an HTTP URL for Telegram to get a file from the Internet, 
     or pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
-    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the photo to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the photo caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     has_spoiler: Option[bool] = Nothing
-    """Optional. Pass True if the photo needs to be covered with a spoiler animation"""
+    """Optional. Pass True if the photo needs to be covered with a spoiler animation."""
 
 
 class InputMediaVideo(InputMedia):
-    """Object `InputMediaVideo`, see the [documentation](https://core.telegram.org/bots/api#inputmediavideo)
+    """Object `InputMediaVideo`, see the [documentation](https://core.telegram.org/bots/api#inputmediavideo).
 
-    Represents a video to be sent."""
+    Represents a video to be sent.
+    """
 
-    type: InputMediaType
-    """Type of the result, must be video"""
+    type: typing.Literal["video"]
+    """Type of the result, must be video."""
 
-    media: str
+    media: Variative["InputFile", str]
     """File to send. Pass a file_id to send a file that exists on the Telegram servers 
     (recommended), pass an HTTP URL for Telegram to get a file from the Internet, 
     or pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
-    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
-    thumbnail: Option[Union["InputFile", str]] = Nothing
+    thumbnail: Option[Variative["InputFile", str]] = Nothing
     """Optional. Thumbnail of the file sent; can be ignored if thumbnail generation 
     for the file is supported server-side. The thumbnail should be in JPEG format 
     and less than 200 kB in size. A thumbnail's width and height should not exceed 
     320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails 
     can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` 
     if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. 
-    More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the video to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the video caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     width: Option[int] = Nothing
-    """Optional. Video width"""
+    """Optional. Video width."""
 
     height: Option[int] = Nothing
-    """Optional. Video height"""
+    """Optional. Video height."""
 
     duration: Option[int] = Nothing
-    """Optional. Video duration in seconds"""
+    """Optional. Video duration in seconds."""
 
     supports_streaming: Option[bool] = Nothing
-    """Optional. Pass True if the uploaded video is suitable for streaming"""
+    """Optional. Pass True if the uploaded video is suitable for streaming."""
 
     has_spoiler: Option[bool] = Nothing
-    """Optional. Pass True if the video needs to be covered with a spoiler animation"""
+    """Optional. Pass True if the video needs to be covered with a spoiler animation."""
 
 
 class InputMediaAnimation(InputMedia):
-    """Object `InputMediaAnimation`, see the [documentation](https://core.telegram.org/bots/api#inputmediaanimation)
+    """Object `InputMediaAnimation`, see the [documentation](https://core.telegram.org/bots/api#inputmediaanimation).
 
     Represents an animation file (GIF or H.264/MPEG-4 AVC video without sound) to be sent.
     """
 
-    type: InputMediaType
-    """Type of the result, must be animation"""
+    type: typing.Literal["animation"]
+    """Type of the result, must be animation."""
 
-    media: str
+    media: Variative["InputFile", str]
     """File to send. Pass a file_id to send a file that exists on the Telegram servers 
     (recommended), pass an HTTP URL for Telegram to get a file from the Internet, 
     or pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
-    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
-    thumbnail: Option[Union["InputFile", str]] = Nothing
+    thumbnail: Option[Variative["InputFile", str]] = Nothing
     """Optional. Thumbnail of the file sent; can be ignored if thumbnail generation 
     for the file is supported server-side. The thumbnail should be in JPEG format 
     and less than 200 kB in size. A thumbnail's width and height should not exceed 
     320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails 
     can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` 
     if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. 
-    More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the animation to be sent, 0-1024 characters after 
-    entities parsing"""
+    entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the animation caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     width: Option[int] = Nothing
-    """Optional. Animation width"""
+    """Optional. Animation width."""
 
     height: Option[int] = Nothing
-    """Optional. Animation height"""
+    """Optional. Animation height."""
 
     duration: Option[int] = Nothing
-    """Optional. Animation duration in seconds"""
+    """Optional. Animation duration in seconds."""
 
     has_spoiler: Option[bool] = Nothing
-    """Optional. Pass True if the animation needs to be covered with a spoiler animation"""
+    """Optional. Pass True if the animation needs to be covered with a spoiler animation."""
 
 
 class InputMediaAudio(InputMedia):
-    """Object `InputMediaAudio`, see the [documentation](https://core.telegram.org/bots/api#inputmediaaudio)
+    """Object `InputMediaAudio`, see the [documentation](https://core.telegram.org/bots/api#inputmediaaudio).
 
-    Represents an audio file to be treated as music to be sent."""
+    Represents an audio file to be treated as music to be sent.
+    """
 
-    type: InputMediaType
-    """Type of the result, must be audio"""
+    type: typing.Literal["audio"]
+    """Type of the result, must be audio."""
 
-    media: str
+    media: Variative["InputFile", str]
     """File to send. Pass a file_id to send a file that exists on the Telegram servers 
     (recommended), pass an HTTP URL for Telegram to get a file from the Internet, 
     or pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
-    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
-    thumbnail: Option[Union["InputFile", str]] = Nothing
+    thumbnail: Option[Variative["InputFile", str]] = Nothing
     """Optional. Thumbnail of the file sent; can be ignored if thumbnail generation 
     for the file is supported server-side. The thumbnail should be in JPEG format 
     and less than 200 kB in size. A thumbnail's width and height should not exceed 
     320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails 
     can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` 
     if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. 
-    More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the audio to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the audio caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     duration: Option[int] = Nothing
-    """Optional. Duration of the audio in seconds"""
+    """Optional. Duration of the audio in seconds."""
 
     performer: Option[str] = Nothing
-    """Optional. Performer of the audio"""
+    """Optional. Performer of the audio."""
 
     title: Option[str] = Nothing
-    """Optional. Title of the audio"""
+    """Optional. Title of the audio."""
 
 
 class InputMediaDocument(InputMedia):
-    """Object `InputMediaDocument`, see the [documentation](https://core.telegram.org/bots/api#inputmediadocument)
+    """Object `InputMediaDocument`, see the [documentation](https://core.telegram.org/bots/api#inputmediadocument).
 
-    Represents a general file to be sent."""
+    Represents a general file to be sent.
+    """
 
-    type: InputMediaType
-    """Type of the result, must be document"""
+    type: typing.Literal["document"]
+    """Type of the result, must be document."""
 
-    media: str
+    media: Variative["InputFile", str]
     """File to send. Pass a file_id to send a file that exists on the Telegram servers 
     (recommended), pass an HTTP URL for Telegram to get a file from the Internet, 
     or pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
-    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    under <file_attach_name> name. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
-    thumbnail: Option[Union["InputFile", str]] = Nothing
+    thumbnail: Option[Variative["InputFile", str]] = Nothing
     """Optional. Thumbnail of the file sent; can be ignored if thumbnail generation 
     for the file is supported server-side. The thumbnail should be in JPEG format 
     and less than 200 kB in size. A thumbnail's width and height should not exceed 
     320. Ignored if the file is not uploaded using multipart/form-data. Thumbnails 
     can't be reused and can be only uploaded as a new file, so you can pass `attach://<file_attach_name>` 
     if the thumbnail was uploaded using multipart/form-data under <file_attach_name>. 
-    More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the document to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the document caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     disable_content_type_detection: Option[bool] = Nothing
     """Optional. Disables automatic server-side content type detection for 
     files uploaded using multipart/form-data. Always True, if the document 
     is sent as part of an album."""
 
 
-class InputFile(Model):
-    """Object `InputFile`, see the [documentation](https://core.telegram.org/bots/api#inputfile)
+class InputFile(typing.NamedTuple):
+    """NamedTuple object `InputFile`, see the [documentation](https://core.telegram.org/bots/api#inputfile).
 
     This object represents the contents of a file to be uploaded. Must be posted using multipart/form-data in the usual way that files are uploaded via the browser.
     """
 
     filename: str
-    """Filename."""
+    """File name."""
 
     data: bytes
     """Bytes of file."""
 
 
 class Sticker(Model):
-    """Object `Sticker`, see the [documentation](https://core.telegram.org/bots/api#sticker)
+    """Object `Sticker`, see the [documentation](https://core.telegram.org/bots/api#sticker).
 
-    This object represents a sticker."""
+    This object represents a sticker.
+    """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
-    type: str
+    type: typing.Literal["regular", "mask", "custom_emoji"]
     """Type of the sticker, currently one of `regular`, `mask`, `custom_emoji`. 
     The type of the sticker is independent from its format, which is determined 
     by the fields is_animated and is_video."""
 
     width: int
-    """Sticker width"""
+    """Sticker width."""
 
     height: int
-    """Sticker height"""
+    """Sticker height."""
 
     is_animated: bool
-    """True, if the sticker is animated"""
+    """True, if the sticker is animated."""
 
     is_video: bool
-    """True, if the sticker is a video sticker"""
+    """True, if the sticker is a video sticker."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Sticker thumbnail in the .WEBP or .JPG format"""
+    """Optional. Sticker thumbnail in the .WEBP or .JPG format."""
 
     emoji: Option[str] = Nothing
-    """Optional. Emoji associated with the sticker"""
+    """Optional. Emoji associated with the sticker."""
 
     set_name: Option[str] = Nothing
-    """Optional. Name of the sticker set to which the sticker belongs"""
+    """Optional. Name of the sticker set to which the sticker belongs."""
 
     premium_animation: Option["File"] = Nothing
-    """Optional. For premium regular stickers, premium animation for the sticker"""
+    """Optional. For premium regular stickers, premium animation for the sticker."""
 
     mask_position: Option["MaskPosition"] = Nothing
-    """Optional. For mask stickers, the position where the mask should be placed"""
+    """Optional. For mask stickers, the position where the mask should be placed."""
 
     custom_emoji_id: Option[str] = Nothing
-    """Optional. For custom emoji stickers, unique identifier of the custom emoji"""
+    """Optional. For custom emoji stickers, unique identifier of the custom emoji."""
 
     needs_repainting: Option[bool] = Nothing
     """Optional. True, if the sticker must be repainted to a text color in messages, 
     the color of the Telegram Premium badge in emoji status, white color on chat 
-    photos, or another appropriate color in other places"""
+    photos, or another appropriate color in other places."""
 
     file_size: Option[int] = Nothing
-    """Optional. File size in bytes"""
+    """Optional. File size in bytes."""
 
 
 class StickerSet(Model):
-    """Object `StickerSet`, see the [documentation](https://core.telegram.org/bots/api#stickerset)
+    """Object `StickerSet`, see the [documentation](https://core.telegram.org/bots/api#stickerset).
 
-    This object represents a sticker set."""
+    This object represents a sticker set.
+    """
 
     name: str
-    """Sticker set name"""
+    """Sticker set name."""
 
     title: str
-    """Sticker set title"""
-
-    sticker_type: str
-    """Type of stickers in the set, currently one of `regular`, `mask`, `custom_emoji`"""
+    """Sticker set title."""
 
-    is_animated: bool
-    """True, if the sticker set contains animated stickers"""
-
-    is_video: bool
-    """True, if the sticker set contains video stickers"""
+    sticker_type: typing.Literal["regular", "mask", "custom_emoji"]
+    """Type of stickers in the set, currently one of `regular`, `mask`, `custom_emoji`."""
 
     stickers: list["Sticker"]
-    """List of all set stickers"""
+    """List of all set stickers."""
 
     thumbnail: Option["PhotoSize"] = Nothing
-    """Optional. Sticker set thumbnail in the .WEBP, .TGS, or .WEBM format"""
+    """Optional. Sticker set thumbnail in the .WEBP, .TGS, or .WEBM format."""
 
 
 class MaskPosition(Model):
-    """Object `MaskPosition`, see the [documentation](https://core.telegram.org/bots/api#maskposition)
+    """Object `MaskPosition`, see the [documentation](https://core.telegram.org/bots/api#maskposition).
 
     This object describes the position on faces where a mask should be placed by default.
     """
 
     point: str
     """The part of the face relative to which the mask should be placed. One of `forehead`, 
     `eyes`, `mouth`, or `chin`."""
@@ -3382,75 +3742,80 @@
     mask position."""
 
     scale: float
     """Mask scaling coefficient. For example, 2.0 means double size."""
 
 
 class InputSticker(Model):
-    """Object `InputSticker`, see the [documentation](https://core.telegram.org/bots/api#inputsticker)
+    """Object `InputSticker`, see the [documentation](https://core.telegram.org/bots/api#inputsticker).
 
-    This object describes a sticker to be added to a sticker set."""
+    This object describes a sticker to be added to a sticker set.
+    """
 
-    sticker: Union["InputFile", str]
+    sticker: Variative["InputFile", str]
     """The added sticker. Pass a file_id as a String to send a file that already exists 
     on the Telegram servers, pass an HTTP URL as a String for Telegram to get a 
     file from the Internet, upload a new one using multipart/form-data, or 
     pass `attach://<file_attach_name>` to upload a new one using multipart/form-data 
     under <file_attach_name> name. Animated and video stickers can't be uploaded 
-    via HTTP URL. More information on Sending Files: https://core.telegram.org/bots/api#sending-files"""
+    via HTTP URL. More information on Sending Files: https://core.telegram.org/bots/api#sending-files."""
+
+    format: str
+    """Format of the added sticker, must be one of `static` for a .WEBP or .PNG image, 
+    `animated` for a .TGS animation, `video` for a WEBM video."""
 
     emoji_list: list[str]
-    """List of 1-20 emoji associated with the sticker"""
+    """List of 1-20 emoji associated with the sticker."""
 
     mask_position: Option["MaskPosition"] = Nothing
     """Optional. Position where the mask should be placed on faces. For `mask` 
     stickers only."""
 
     keywords: Option[list[str]] = Nothing
     """Optional. List of 0-20 search keywords for the sticker with total length 
     of up to 64 characters. For `regular` and `custom_emoji` stickers only."""
 
 
 class InlineQuery(Model):
-    """Object `InlineQuery`, see the [documentation](https://core.telegram.org/bots/api#inlinequery)
+    """Object `InlineQuery`, see the [documentation](https://core.telegram.org/bots/api#inlinequery).
 
     This object represents an incoming inline query. When the user sends an empty query, your bot could return some default or trending results.
     """
 
     id: str
-    """Unique identifier for this query"""
+    """Unique identifier for this query."""
 
     from_: "User"
-    """Sender"""
+    """Sender."""
 
     query: str
-    """Text of the query (up to 256 characters)"""
+    """Text of the query (up to 256 characters)."""
 
     offset: str
-    """Offset of the results to be returned, can be controlled by the bot"""
+    """Offset of the results to be returned, can be controlled by the bot."""
 
-    chat_type: Option[str] = Nothing
+    chat_type: Option[ChatType] = Nothing
     """Optional. Type of the chat from which the inline query was sent. Can be either 
     `sender` for a private chat with the inline query sender, `private`, `group`, 
     `supergroup`, or `channel`. The chat type should be always known for requests 
     sent from official clients and most third-party clients, unless the request 
-    was sent from a secret chat"""
+    was sent from a secret chat."""
 
     location: Option["Location"] = Nothing
-    """Optional. Sender location, only for bots that request user location"""
+    """Optional. Sender location, only for bots that request user location."""
 
 
 class InlineQueryResultsButton(Model):
-    """Object `InlineQueryResultsButton`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultsbutton)
+    """Object `InlineQueryResultsButton`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultsbutton).
 
     This object represents a button to be shown above inline query results. You must use exactly one of the optional fields.
     """
 
     text: str
-    """Label text on the button"""
+    """Label text on the button."""
 
     web_app: Option["WebAppInfo"] = Nothing
     """Optional. Description of the Web App that will be launched when the user 
     presses the button. The Web App will be able to switch back to the inline mode 
     using the method switchInlineQuery inside the Web App."""
 
     start_parameter: Option[str] = Nothing
@@ -3463,484 +3828,489 @@
     switches to a private chat with the bot and, in doing so, passes a start parameter 
     that instructs the bot to return an OAuth link. Once done, the bot can offer 
     a switch_inline button so that the user can easily return to the chat where 
     they wanted to use the bot's inline capabilities."""
 
 
 class InlineQueryResultArticle(InlineQueryResult):
-    """Object `InlineQueryResultArticle`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultarticle)
+    """Object `InlineQueryResultArticle`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultarticle).
 
-    Represents a link to an article or web page."""
+    Represents a link to an article or web page.
+    """
 
-    type: InlineQueryResultType
-    """Type of the result, must be article"""
+    type: typing.Literal["article"]
+    """Type of the result, must be article."""
 
     id: str
-    """Unique identifier for this result, 1-64 Bytes"""
+    """Unique identifier for this result, 1-64 Bytes."""
 
     title: str
-    """Title of the result"""
+    """Title of the result."""
 
-    input_message_content: Union[
+    input_message_content: Variative[
         "InputTextMessageContent",
         "InputLocationMessageContent",
         "InputVenueMessageContent",
         "InputContactMessageContent",
         "InputInvoiceMessageContent",
     ]
-    """Content of the message to be sent"""
+    """Content of the message to be sent."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     url: Option[str] = Nothing
-    """Optional. URL of the result"""
+    """Optional. URL of the result."""
 
     hide_url: Option[bool] = Nothing
-    """Optional. Pass True if you don't want the URL to be shown in the message"""
+    """Optional. Pass True if you don't want the URL to be shown in the message."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     thumbnail_url: Option[str] = Nothing
-    """Optional. Url of the thumbnail for the result"""
+    """Optional. Url of the thumbnail for the result."""
 
     thumbnail_width: Option[int] = Nothing
-    """Optional. Thumbnail width"""
+    """Optional. Thumbnail width."""
 
     thumbnail_height: Option[int] = Nothing
-    """Optional. Thumbnail height"""
+    """Optional. Thumbnail height."""
 
 
 class InlineQueryResultPhoto(InlineQueryResult):
-    """Object `InlineQueryResultPhoto`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultphoto)
+    """Object `InlineQueryResultPhoto`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultphoto).
 
     Represents a link to a photo. By default, this photo will be sent by the user with optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the photo.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be photo"""
+    type: typing.Literal["photo"]
+    """Type of the result, must be photo."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     photo_url: str
     """A valid URL of the photo. Photo must be in JPEG format. Photo size must not 
-    exceed 5MB"""
+    exceed 5MB."""
 
     thumbnail_url: str
-    """URL of the thumbnail for the photo"""
+    """URL of the thumbnail for the photo."""
 
     photo_width: Option[int] = Nothing
-    """Optional. Width of the photo"""
+    """Optional. Width of the photo."""
 
     photo_height: Option[int] = Nothing
-    """Optional. Height of the photo"""
+    """Optional. Height of the photo."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the photo to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the photo caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the photo"""
+    """Optional. Content of the message to be sent instead of the photo."""
 
 
 class InlineQueryResultGif(InlineQueryResult):
-    """Object `InlineQueryResultGif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultgif)
+    """Object `InlineQueryResultGif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultgif).
 
     Represents a link to an animated GIF file. By default, this animated GIF file will be sent by the user with optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the animation.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be gif"""
+    type: typing.Literal["gif"]
+    """Type of the result, must be gif."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     gif_url: str
-    """A valid URL for the GIF file. File size must not exceed 1MB"""
+    """A valid URL for the GIF file. File size must not exceed 1MB."""
 
     thumbnail_url: str
-    """URL of the static (JPEG or GIF) or animated (MPEG4) thumbnail for the result"""
+    """URL of the static (JPEG or GIF) or animated (MPEG4) thumbnail for the result."""
 
     gif_width: Option[int] = Nothing
-    """Optional. Width of the GIF"""
+    """Optional. Width of the GIF."""
 
     gif_height: Option[int] = Nothing
-    """Optional. Height of the GIF"""
+    """Optional. Height of the GIF."""
 
     gif_duration: Option[int] = Nothing
-    """Optional. Duration of the GIF in seconds"""
+    """Optional. Duration of the GIF in seconds."""
 
-    thumbnail_mime_type: Option[str] = Nothing
+    thumbnail_mime_type: Option[
+        typing.Literal["image/jpeg", "image/gif", "video/mp4"]
+    ] = Nothing
     """Optional. MIME type of the thumbnail, must be one of `image/jpeg`, `image/gif`, 
-    or `video/mp4`. Defaults to `image/jpeg`"""
+    or `video/mp4`. Defaults to `image/jpeg`."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the GIF file to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the caption. See formatting options 
     for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the GIF animation"""
+    """Optional. Content of the message to be sent instead of the GIF animation."""
 
 
 class InlineQueryResultMpeg4Gif(InlineQueryResult):
-    """Object `InlineQueryResultMpeg4Gif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultmpeg4gif)
+    """Object `InlineQueryResultMpeg4Gif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultmpeg4gif).
 
     Represents a link to a video animation (H.264/MPEG-4 AVC video without sound). By default, this animated MPEG-4 file will be sent by the user with optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the animation.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be mpeg4_gif"""
+    type: typing.Literal["mpeg4_gif"]
+    """Type of the result, must be mpeg4_gif."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     mpeg4_url: str
-    """A valid URL for the MPEG4 file. File size must not exceed 1MB"""
+    """A valid URL for the MPEG4 file. File size must not exceed 1MB."""
 
     thumbnail_url: str
-    """URL of the static (JPEG or GIF) or animated (MPEG4) thumbnail for the result"""
+    """URL of the static (JPEG or GIF) or animated (MPEG4) thumbnail for the result."""
 
     mpeg4_width: Option[int] = Nothing
-    """Optional. Video width"""
+    """Optional. Video width."""
 
     mpeg4_height: Option[int] = Nothing
-    """Optional. Video height"""
+    """Optional. Video height."""
 
     mpeg4_duration: Option[int] = Nothing
-    """Optional. Video duration in seconds"""
+    """Optional. Video duration in seconds."""
 
-    thumbnail_mime_type: Option[str] = Nothing
+    thumbnail_mime_type: Option[
+        typing.Literal["image/jpeg", "image/gif", "video/mp4"]
+    ] = Nothing
     """Optional. MIME type of the thumbnail, must be one of `image/jpeg`, `image/gif`, 
-    or `video/mp4`. Defaults to `image/jpeg`"""
+    or `video/mp4`. Defaults to `image/jpeg`."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the MPEG-4 file to be sent, 0-1024 characters after 
-    entities parsing"""
+    entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the caption. See formatting options 
     for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the video animation"""
+    """Optional. Content of the message to be sent instead of the video animation."""
 
 
 class InlineQueryResultVideo(InlineQueryResult):
-    """Object `InlineQueryResultVideo`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvideo)
+    """Object `InlineQueryResultVideo`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvideo).
 
     Represents a link to a page containing an embedded video player or a video file. By default, this video file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the video.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be video"""
+    type: typing.Literal["video"]
+    """Type of the result, must be video."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     video_url: str
-    """A valid URL for the embedded video player or video file"""
+    """A valid URL for the embedded video player or video file."""
 
     mime_type: str
-    """MIME type of the content of the video URL, `text/html` or `video/mp4`"""
+    """MIME type of the content of the video URL, `text/html` or `video/mp4`."""
 
     thumbnail_url: str
-    """URL of the thumbnail (JPEG only) for the video"""
+    """URL of the thumbnail (JPEG only) for the video."""
 
     title: str
-    """Title for the result"""
+    """Title for the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the video to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the video caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     video_width: Option[int] = Nothing
-    """Optional. Video width"""
+    """Optional. Video width."""
 
     video_height: Option[int] = Nothing
-    """Optional. Video height"""
+    """Optional. Video height."""
 
     video_duration: Option[int] = Nothing
-    """Optional. Video duration in seconds"""
+    """Optional. Video duration in seconds."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
     """Optional. Content of the message to be sent instead of the video. This field 
     is required if InlineQueryResultVideo is used to send an HTML-page as a 
     result (e.g., a YouTube video)."""
 
 
 class InlineQueryResultAudio(InlineQueryResult):
-    """Object `InlineQueryResultAudio`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultaudio)
+    """Object `InlineQueryResultAudio`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultaudio).
 
     Represents a link to an MP3 audio file. By default, this audio file will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the audio.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be audio"""
+    type: typing.Literal["audio"]
+    """Type of the result, must be audio."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     audio_url: str
-    """A valid URL for the audio file"""
+    """A valid URL for the audio file."""
 
     title: str
-    """Title"""
+    """Title."""
 
     caption: Option[str] = Nothing
-    """Optional. Caption, 0-1024 characters after entities parsing"""
+    """Optional. Caption, 0-1024 characters after entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the audio caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     performer: Option[str] = Nothing
-    """Optional. Performer"""
+    """Optional. Performer."""
 
     audio_duration: Option[int] = Nothing
-    """Optional. Audio duration in seconds"""
+    """Optional. Audio duration in seconds."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the audio"""
+    """Optional. Content of the message to be sent instead of the audio."""
 
 
 class InlineQueryResultVoice(InlineQueryResult):
-    """Object `InlineQueryResultVoice`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvoice)
+    """Object `InlineQueryResultVoice`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvoice).
 
     Represents a link to a voice recording in an .OGG container encoded with OPUS. By default, this voice recording will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the the voice message.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be voice"""
+    type: typing.Literal["voice"]
+    """Type of the result, must be voice."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     voice_url: str
-    """A valid URL for the voice recording"""
+    """A valid URL for the voice recording."""
 
     title: str
-    """Recording title"""
+    """Recording title."""
 
     caption: Option[str] = Nothing
-    """Optional. Caption, 0-1024 characters after entities parsing"""
+    """Optional. Caption, 0-1024 characters after entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the voice message caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     voice_duration: Option[int] = Nothing
-    """Optional. Recording duration in seconds"""
+    """Optional. Recording duration in seconds."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the voice recording"""
+    """Optional. Content of the message to be sent instead of the voice recording."""
 
 
 class InlineQueryResultDocument(InlineQueryResult):
-    """Object `InlineQueryResultDocument`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultdocument)
+    """Object `InlineQueryResultDocument`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultdocument).
 
     Represents a link to a file. By default, this file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the file. Currently, only .PDF and .ZIP files can be sent using this method.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be document"""
+    type: typing.Literal["document"]
+    """Type of the result, must be document."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     title: str
-    """Title for the result"""
+    """Title for the result."""
 
     document_url: str
-    """A valid URL for the file"""
+    """A valid URL for the file."""
 
-    mime_type: str
-    """MIME type of the content of the file, either `application/pdf` or `application/zip`"""
+    mime_type: typing.Literal["application/pdf", "application/zip"]
+    """MIME type of the content of the file, either `application/pdf` or `application/zip`."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the document to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the document caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the file"""
+    """Optional. Content of the message to be sent instead of the file."""
 
     thumbnail_url: Option[str] = Nothing
-    """Optional. URL of the thumbnail (JPEG only) for the file"""
+    """Optional. URL of the thumbnail (JPEG only) for the file."""
 
     thumbnail_width: Option[int] = Nothing
-    """Optional. Thumbnail width"""
+    """Optional. Thumbnail width."""
 
     thumbnail_height: Option[int] = Nothing
-    """Optional. Thumbnail height"""
+    """Optional. Thumbnail height."""
 
 
 class InlineQueryResultLocation(InlineQueryResult):
-    """Object `InlineQueryResultLocation`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultlocation)
+    """Object `InlineQueryResultLocation`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultlocation).
 
     Represents a location on a map. By default, the location will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the location.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be location"""
+    type: typing.Literal["location"]
+    """Type of the result, must be location."""
 
     id: str
-    """Unique identifier for this result, 1-64 Bytes"""
+    """Unique identifier for this result, 1-64 Bytes."""
 
     latitude: float
-    """Location latitude in degrees"""
+    """Location latitude in degrees."""
 
     longitude: float
-    """Location longitude in degrees"""
+    """Location longitude in degrees."""
 
     title: str
-    """Location title"""
+    """Location title."""
 
     horizontal_accuracy: Option[float] = Nothing
     """Optional. The radius of uncertainty for the location, measured in meters; 
-    0-1500"""
+    0-1500."""
 
     live_period: Option[int] = Nothing
     """Optional. Period in seconds for which the location can be updated, should 
     be between 60 and 86400."""
 
     heading: Option[int] = Nothing
     """Optional. For live locations, a direction in which the user is moving, in 
@@ -3948,550 +4318,551 @@
 
     proximity_alert_radius: Option[int] = Nothing
     """Optional. For live locations, a maximum distance for proximity alerts 
     about approaching another chat member, in meters. Must be between 1 and 
     100000 if specified."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the location"""
+    """Optional. Content of the message to be sent instead of the location."""
 
     thumbnail_url: Option[str] = Nothing
-    """Optional. Url of the thumbnail for the result"""
+    """Optional. Url of the thumbnail for the result."""
 
     thumbnail_width: Option[int] = Nothing
-    """Optional. Thumbnail width"""
+    """Optional. Thumbnail width."""
 
     thumbnail_height: Option[int] = Nothing
-    """Optional. Thumbnail height"""
+    """Optional. Thumbnail height."""
 
 
 class InlineQueryResultVenue(InlineQueryResult):
-    """Object `InlineQueryResultVenue`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvenue)
+    """Object `InlineQueryResultVenue`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultvenue).
 
     Represents a venue. By default, the venue will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the venue.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be venue"""
+    type: typing.Literal["venue"]
+    """Type of the result, must be venue."""
 
     id: str
-    """Unique identifier for this result, 1-64 Bytes"""
+    """Unique identifier for this result, 1-64 Bytes."""
 
     latitude: float
-    """Latitude of the venue location in degrees"""
+    """Latitude of the venue location in degrees."""
 
     longitude: float
-    """Longitude of the venue location in degrees"""
+    """Longitude of the venue location in degrees."""
 
     title: str
-    """Title of the venue"""
+    """Title of the venue."""
 
     address: str
-    """Address of the venue"""
+    """Address of the venue."""
 
     foursquare_id: Option[str] = Nothing
-    """Optional. Foursquare identifier of the venue if known"""
+    """Optional. Foursquare identifier of the venue if known."""
 
     foursquare_type: Option[str] = Nothing
     """Optional. Foursquare type of the venue, if known. (For example, `arts_entertainment/default`, 
-    `arts_entertainment/aquarium` or `food/icecream`.)"""
+    `arts_entertainment/aquarium` or `food/icecream`.)."""
 
     google_place_id: Option[str] = Nothing
-    """Optional. Google Places identifier of the venue"""
+    """Optional. Google Places identifier of the venue."""
 
     google_place_type: Option[str] = Nothing
-    """Optional. Google Places type of the venue. (See supported types.)"""
+    """Optional. Google Places type of the venue. (See supported types.)."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the venue"""
+    """Optional. Content of the message to be sent instead of the venue."""
 
     thumbnail_url: Option[str] = Nothing
-    """Optional. Url of the thumbnail for the result"""
+    """Optional. Url of the thumbnail for the result."""
 
     thumbnail_width: Option[int] = Nothing
-    """Optional. Thumbnail width"""
+    """Optional. Thumbnail width."""
 
     thumbnail_height: Option[int] = Nothing
-    """Optional. Thumbnail height"""
+    """Optional. Thumbnail height."""
 
 
 class InlineQueryResultContact(InlineQueryResult):
-    """Object `InlineQueryResultContact`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcontact)
+    """Object `InlineQueryResultContact`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcontact).
 
     Represents a contact with a phone number. By default, this contact will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the contact.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be contact"""
+    type: typing.Literal["contact"]
+    """Type of the result, must be contact."""
 
     id: str
-    """Unique identifier for this result, 1-64 Bytes"""
+    """Unique identifier for this result, 1-64 Bytes."""
 
     phone_number: str
-    """Contact's phone number"""
+    """Contact's phone number."""
 
     first_name: str
-    """Contact's first name"""
+    """Contact's first name."""
 
     last_name: Option[str] = Nothing
-    """Optional. Contact's last name"""
+    """Optional. Contact's last name."""
 
     vcard: Option[str] = Nothing
     """Optional. Additional data about the contact in the form of a vCard, 0-2048 
-    bytes"""
+    bytes."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the contact"""
+    """Optional. Content of the message to be sent instead of the contact."""
 
     thumbnail_url: Option[str] = Nothing
-    """Optional. Url of the thumbnail for the result"""
+    """Optional. Url of the thumbnail for the result."""
 
     thumbnail_width: Option[int] = Nothing
-    """Optional. Thumbnail width"""
+    """Optional. Thumbnail width."""
 
     thumbnail_height: Option[int] = Nothing
-    """Optional. Thumbnail height"""
+    """Optional. Thumbnail height."""
 
 
 class InlineQueryResultGame(InlineQueryResult):
-    """Object `InlineQueryResultGame`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultgame)
+    """Object `InlineQueryResultGame`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultgame).
 
-    Represents a Game."""
+    Represents a Game.
+    """
 
-    type: InlineQueryResultType
-    """Type of the result, must be game"""
+    type: typing.Literal["game"]
+    """Type of the result, must be game."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     game_short_name: str
-    """Short name of the game"""
+    """Short name of the game."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
 
 class InlineQueryResultCachedPhoto(InlineQueryResult):
-    """Object `InlineQueryResultCachedPhoto`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedphoto)
+    """Object `InlineQueryResultCachedPhoto`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedphoto).
 
     Represents a link to a photo stored on the Telegram servers. By default, this photo will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the photo.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be photo"""
+    type: typing.Literal["photo"]
+    """Type of the result, must be photo."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     photo_file_id: str
-    """A valid file identifier of the photo"""
+    """A valid file identifier of the photo."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the photo to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the photo caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the photo"""
+    """Optional. Content of the message to be sent instead of the photo."""
 
 
 class InlineQueryResultCachedGif(InlineQueryResult):
-    """Object `InlineQueryResultCachedGif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedgif)
+    """Object `InlineQueryResultCachedGif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedgif).
 
     Represents a link to an animated GIF file stored on the Telegram servers. By default, this animated GIF file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with specified content instead of the animation.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be gif"""
+    type: typing.Literal["gif"]
+    """Type of the result, must be gif."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     gif_file_id: str
-    """A valid file identifier for the GIF file"""
+    """A valid file identifier for the GIF file."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the GIF file to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the caption. See formatting options 
     for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the GIF animation"""
+    """Optional. Content of the message to be sent instead of the GIF animation."""
 
 
 class InlineQueryResultCachedMpeg4Gif(InlineQueryResult):
-    """Object `InlineQueryResultCachedMpeg4Gif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedmpeg4gif)
+    """Object `InlineQueryResultCachedMpeg4Gif`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedmpeg4gif).
 
     Represents a link to a video animation (H.264/MPEG-4 AVC video without sound) stored on the Telegram servers. By default, this animated MPEG-4 file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the animation.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be mpeg4_gif"""
+    type: typing.Literal["mpeg4_gif"]
+    """Type of the result, must be mpeg4_gif."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     mpeg4_file_id: str
-    """A valid file identifier for the MPEG4 file"""
+    """A valid file identifier for the MPEG4 file."""
 
     title: Option[str] = Nothing
-    """Optional. Title for the result"""
+    """Optional. Title for the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the MPEG-4 file to be sent, 0-1024 characters after 
-    entities parsing"""
+    entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the caption. See formatting options 
     for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the video animation"""
+    """Optional. Content of the message to be sent instead of the video animation."""
 
 
 class InlineQueryResultCachedSticker(InlineQueryResult):
-    """Object `InlineQueryResultCachedSticker`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedsticker)
+    """Object `InlineQueryResultCachedSticker`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedsticker).
 
     Represents a link to a sticker stored on the Telegram servers. By default, this sticker will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the sticker.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be sticker"""
+    type: typing.Literal["sticker"]
+    """Type of the result, must be sticker."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     sticker_file_id: str
-    """A valid file identifier of the sticker"""
+    """A valid file identifier of the sticker."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the sticker"""
+    """Optional. Content of the message to be sent instead of the sticker."""
 
 
 class InlineQueryResultCachedDocument(InlineQueryResult):
-    """Object `InlineQueryResultCachedDocument`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcacheddocument)
+    """Object `InlineQueryResultCachedDocument`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcacheddocument).
 
     Represents a link to a file stored on the Telegram servers. By default, this file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the file.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be document"""
+    type: typing.Literal["document"]
+    """Type of the result, must be document."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     title: str
-    """Title for the result"""
+    """Title for the result."""
 
     document_file_id: str
-    """A valid file identifier for the file"""
+    """A valid file identifier for the file."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the document to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the document caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the file"""
+    """Optional. Content of the message to be sent instead of the file."""
 
 
 class InlineQueryResultCachedVideo(InlineQueryResult):
-    """Object `InlineQueryResultCachedVideo`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedvideo)
+    """Object `InlineQueryResultCachedVideo`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedvideo).
 
     Represents a link to a video file stored on the Telegram servers. By default, this video file will be sent by the user with an optional caption. Alternatively, you can use input_message_content to send a message with the specified content instead of the video.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be video"""
+    type: typing.Literal["video"]
+    """Type of the result, must be video."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     video_file_id: str
-    """A valid file identifier for the video file"""
+    """A valid file identifier for the video file."""
 
     title: str
-    """Title for the result"""
+    """Title for the result."""
 
     description: Option[str] = Nothing
-    """Optional. Short description of the result"""
+    """Optional. Short description of the result."""
 
     caption: Option[str] = Nothing
     """Optional. Caption of the video to be sent, 0-1024 characters after entities 
-    parsing"""
+    parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the video caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the video"""
+    """Optional. Content of the message to be sent instead of the video."""
 
 
 class InlineQueryResultCachedVoice(InlineQueryResult):
-    """Object `InlineQueryResultCachedVoice`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedvoice)
+    """Object `InlineQueryResultCachedVoice`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedvoice).
 
     Represents a link to a voice message stored on the Telegram servers. By default, this voice message will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the voice message.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be voice"""
+    type: typing.Literal["voice"]
+    """Type of the result, must be voice."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     voice_file_id: str
-    """A valid file identifier for the voice message"""
+    """A valid file identifier for the voice message."""
 
     title: str
-    """Voice message title"""
+    """Voice message title."""
 
     caption: Option[str] = Nothing
-    """Optional. Caption, 0-1024 characters after entities parsing"""
+    """Optional. Caption, 0-1024 characters after entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the voice message caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the voice message"""
+    """Optional. Content of the message to be sent instead of the voice message."""
 
 
 class InlineQueryResultCachedAudio(InlineQueryResult):
-    """Object `InlineQueryResultCachedAudio`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedaudio)
+    """Object `InlineQueryResultCachedAudio`, see the [documentation](https://core.telegram.org/bots/api#inlinequeryresultcachedaudio).
 
     Represents a link to an MP3 audio file stored on the Telegram servers. By default, this audio file will be sent by the user. Alternatively, you can use input_message_content to send a message with the specified content instead of the audio.
     """
 
-    type: InlineQueryResultType
-    """Type of the result, must be audio"""
+    type: typing.Literal["audio"]
+    """Type of the result, must be audio."""
 
     id: str
-    """Unique identifier for this result, 1-64 bytes"""
+    """Unique identifier for this result, 1-64 bytes."""
 
     audio_file_id: str
-    """A valid file identifier for the audio file"""
+    """A valid file identifier for the audio file."""
 
     caption: Option[str] = Nothing
-    """Optional. Caption, 0-1024 characters after entities parsing"""
+    """Optional. Caption, 0-1024 characters after entities parsing."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the audio caption. See formatting 
     options for more details."""
 
     caption_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in the caption, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     reply_markup: Option["InlineKeyboardMarkup"] = Nothing
-    """Optional. Inline keyboard attached to the message"""
+    """Optional. Inline keyboard attached to the message."""
 
     input_message_content: Option[
-        Union[
+        Variative[
             "InputTextMessageContent",
             "InputLocationMessageContent",
             "InputVenueMessageContent",
             "InputContactMessageContent",
             "InputInvoiceMessageContent",
         ]
     ] = Nothing
-    """Optional. Content of the message to be sent instead of the audio"""
+    """Optional. Content of the message to be sent instead of the audio."""
 
 
 class InputTextMessageContent(InputMessageContent):
-    """Object `InputTextMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputtextmessagecontent)
+    """Object `InputTextMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputtextmessagecontent).
 
     Represents the content of a text message to be sent as the result of an inline query.
     """
 
     message_text: str
-    """Text of the message to be sent, 1-4096 characters"""
+    """Text of the message to be sent, 1-4096 characters."""
 
     parse_mode: Option[str] = Nothing
     """Optional. Mode for parsing entities in the message text. See formatting 
     options for more details."""
 
     entities: Option[list["MessageEntity"]] = Nothing
     """Optional. List of special entities that appear in message text, which can 
-    be specified instead of parse_mode"""
+    be specified instead of parse_mode."""
 
     link_preview_options: Option["LinkPreviewOptions"] = Nothing
-    """Optional. Link preview generation options for the message"""
+    """Optional. Link preview generation options for the message."""
 
 
 class InputLocationMessageContent(InputMessageContent):
-    """Object `InputLocationMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputlocationmessagecontent)
+    """Object `InputLocationMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputlocationmessagecontent).
 
     Represents the content of a location message to be sent as the result of an inline query.
     """
 
     latitude: float
-    """Latitude of the location in degrees"""
+    """Latitude of the location in degrees."""
 
     longitude: float
-    """Longitude of the location in degrees"""
+    """Longitude of the location in degrees."""
 
     horizontal_accuracy: Option[float] = Nothing
     """Optional. The radius of uncertainty for the location, measured in meters; 
-    0-1500"""
+    0-1500."""
 
     live_period: Option[int] = Nothing
     """Optional. Period in seconds for which the location can be updated, should 
     be between 60 and 86400."""
 
     heading: Option[int] = Nothing
     """Optional. For live locations, a direction in which the user is moving, in 
@@ -4500,97 +4871,97 @@
     proximity_alert_radius: Option[int] = Nothing
     """Optional. For live locations, a maximum distance for proximity alerts 
     about approaching another chat member, in meters. Must be between 1 and 
     100000 if specified."""
 
 
 class InputVenueMessageContent(InputMessageContent):
-    """Object `InputVenueMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputvenuemessagecontent)
+    """Object `InputVenueMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputvenuemessagecontent).
 
     Represents the content of a venue message to be sent as the result of an inline query.
     """
 
     latitude: float
-    """Latitude of the venue in degrees"""
+    """Latitude of the venue in degrees."""
 
     longitude: float
-    """Longitude of the venue in degrees"""
+    """Longitude of the venue in degrees."""
 
     title: str
-    """Name of the venue"""
+    """Name of the venue."""
 
     address: str
-    """Address of the venue"""
+    """Address of the venue."""
 
     foursquare_id: Option[str] = Nothing
-    """Optional. Foursquare identifier of the venue, if known"""
+    """Optional. Foursquare identifier of the venue, if known."""
 
     foursquare_type: Option[str] = Nothing
     """Optional. Foursquare type of the venue, if known. (For example, `arts_entertainment/default`, 
-    `arts_entertainment/aquarium` or `food/icecream`.)"""
+    `arts_entertainment/aquarium` or `food/icecream`.)."""
 
     google_place_id: Option[str] = Nothing
-    """Optional. Google Places identifier of the venue"""
+    """Optional. Google Places identifier of the venue."""
 
     google_place_type: Option[str] = Nothing
-    """Optional. Google Places type of the venue. (See supported types.)"""
+    """Optional. Google Places type of the venue. (See supported types.)."""
 
 
 class InputContactMessageContent(InputMessageContent):
-    """Object `InputContactMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputcontactmessagecontent)
+    """Object `InputContactMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputcontactmessagecontent).
 
     Represents the content of a contact message to be sent as the result of an inline query.
     """
 
     phone_number: str
-    """Contact's phone number"""
+    """Contact's phone number."""
 
     first_name: str
-    """Contact's first name"""
+    """Contact's first name."""
 
     last_name: Option[str] = Nothing
-    """Optional. Contact's last name"""
+    """Optional. Contact's last name."""
 
     vcard: Option[str] = Nothing
     """Optional. Additional data about the contact in the form of a vCard, 0-2048 
-    bytes"""
+    bytes."""
 
 
 class InputInvoiceMessageContent(InputMessageContent):
-    """Object `InputInvoiceMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputinvoicemessagecontent)
+    """Object `InputInvoiceMessageContent`, see the [documentation](https://core.telegram.org/bots/api#inputinvoicemessagecontent).
 
     Represents the content of an invoice message to be sent as the result of an inline query.
     """
 
     title: str
-    """Product name, 1-32 characters"""
+    """Product name, 1-32 characters."""
 
     description: str
-    """Product description, 1-255 characters"""
+    """Product description, 1-255 characters."""
 
     payload: str
     """Bot-defined invoice payload, 1-128 bytes. This will not be displayed to 
     the user, use for your internal processes."""
 
     provider_token: str
-    """Payment provider token, obtained via @BotFather"""
+    """Payment provider token, obtained via @BotFather."""
 
     currency: str
-    """Three-letter ISO 4217 currency code, see more on currencies"""
+    """Three-letter ISO 4217 currency code, see more on currencies."""
 
     prices: list["LabeledPrice"]
     """Price breakdown, a JSON-serialized list of components (e.g. product price, 
-    tax, discount, delivery cost, delivery tax, bonus, etc.)"""
+    tax, discount, delivery cost, delivery tax, bonus, etc.)."""
 
     max_tip_amount: Option[int] = Nothing
     """Optional. The maximum accepted amount for tips in the smallest units of 
     the currency (integer, not float/double). For example, for a maximum tip 
     of US$ 1.45 pass max_tip_amount = 145. See the exp parameter in currencies.json, 
     it shows the number of digits past the decimal point for each currency (2 
-    for the majority of currencies). Defaults to 0"""
+    for the majority of currencies). Defaults to 0."""
 
     suggested_tip_amounts: Option[list[int]] = Nothing
     """Optional. A JSON-serialized array of suggested amounts of tip in the smallest 
     units of the currency (integer, not float/double). At most 4 suggested 
     tip amounts can be specified. The suggested tip amounts must be positive, 
     passed in a strictly increased order and must not exceed max_tip_amount."""
 
@@ -4600,567 +4971,625 @@
     fields should be provided by the payment provider."""
 
     photo_url: Option[str] = Nothing
     """Optional. URL of the product photo for the invoice. Can be a photo of the goods 
     or a marketing image for a service."""
 
     photo_size: Option[int] = Nothing
-    """Optional. Photo size in bytes"""
+    """Optional. Photo size in bytes."""
 
     photo_width: Option[int] = Nothing
-    """Optional. Photo width"""
+    """Optional. Photo width."""
 
     photo_height: Option[int] = Nothing
-    """Optional. Photo height"""
+    """Optional. Photo height."""
 
     need_name: Option[bool] = Nothing
-    """Optional. Pass True if you require the user's full name to complete the order"""
+    """Optional. Pass True if you require the user's full name to complete the order."""
 
     need_phone_number: Option[bool] = Nothing
     """Optional. Pass True if you require the user's phone number to complete the 
-    order"""
+    order."""
 
     need_email: Option[bool] = Nothing
     """Optional. Pass True if you require the user's email address to complete 
-    the order"""
+    the order."""
 
     need_shipping_address: Option[bool] = Nothing
     """Optional. Pass True if you require the user's shipping address to complete 
-    the order"""
+    the order."""
 
     send_phone_number_to_provider: Option[bool] = Nothing
-    """Optional. Pass True if the user's phone number should be sent to provider"""
+    """Optional. Pass True if the user's phone number should be sent to provider."""
 
     send_email_to_provider: Option[bool] = Nothing
-    """Optional. Pass True if the user's email address should be sent to provider"""
+    """Optional. Pass True if the user's email address should be sent to provider."""
 
     is_flexible: Option[bool] = Nothing
-    """Optional. Pass True if the final price depends on the shipping method"""
+    """Optional. Pass True if the final price depends on the shipping method."""
 
 
 class ChosenInlineResult(Model):
-    """Object `ChosenInlineResult`, see the [documentation](https://core.telegram.org/bots/api#choseninlineresult)
+    """Object `ChosenInlineResult`, see the [documentation](https://core.telegram.org/bots/api#choseninlineresult).
 
     Represents a result of an inline query that was chosen by the user and sent to their chat partner.
     Note: It is necessary to enable inline feedback via @BotFather in order to receive these objects in updates.
     """
 
     result_id: str
-    """The unique identifier for the result that was chosen"""
+    """The unique identifier for the result that was chosen."""
 
     from_: "User"
-    """The user that chose the result"""
+    """The user that chose the result."""
 
     query: str
-    """The query that was used to obtain the result"""
+    """The query that was used to obtain the result."""
 
     location: Option["Location"] = Nothing
-    """Optional. Sender location, only for bots that require user location"""
+    """Optional. Sender location, only for bots that require user location."""
 
     inline_message_id: Option[str] = Nothing
     """Optional. Identifier of the sent inline message. Available only if there 
     is an inline keyboard attached to the message. Will be also received in callback 
     queries and can be used to edit the message."""
 
 
 class SentWebAppMessage(Model):
-    """Object `SentWebAppMessage`, see the [documentation](https://core.telegram.org/bots/api#sentwebappmessage)
+    """Object `SentWebAppMessage`, see the [documentation](https://core.telegram.org/bots/api#sentwebappmessage).
 
-    Describes an inline message sent by a Web App on behalf of a user."""
+    Describes an inline message sent by a Web App on behalf of a user.
+    """
 
     inline_message_id: Option[str] = Nothing
     """Optional. Identifier of the sent inline message. Available only if there 
     is an inline keyboard attached to the message."""
 
 
 class LabeledPrice(Model):
-    """Object `LabeledPrice`, see the [documentation](https://core.telegram.org/bots/api#labeledprice)
+    """Object `LabeledPrice`, see the [documentation](https://core.telegram.org/bots/api#labeledprice).
 
-    This object represents a portion of the price for goods or services."""
+    This object represents a portion of the price for goods or services.
+    """
 
     label: str
-    """Portion label"""
+    """Portion label."""
 
     amount: int
     """Price of the product in the smallest units of the currency (integer, not 
     float/double). For example, for a price of US$ 1.45 pass amount = 145. See 
     the exp parameter in currencies.json, it shows the number of digits past 
     the decimal point for each currency (2 for the majority of currencies)."""
 
 
 class Invoice(Model):
-    """Object `Invoice`, see the [documentation](https://core.telegram.org/bots/api#invoice)
+    """Object `Invoice`, see the [documentation](https://core.telegram.org/bots/api#invoice).
 
-    This object contains basic information about an invoice."""
+    This object contains basic information about an invoice.
+    """
 
     title: str
-    """Product name"""
+    """Product name."""
 
     description: str
-    """Product description"""
+    """Product description."""
 
     start_parameter: str
-    """Unique bot deep-linking parameter that can be used to generate this invoice"""
+    """Unique bot deep-linking parameter that can be used to generate this invoice."""
 
     currency: str
-    """Three-letter ISO 4217 currency code"""
+    """Three-letter ISO 4217 currency code."""
 
     total_amount: int
     """Total price in the smallest units of the currency (integer, not float/double). 
     For example, for a price of US$ 1.45 pass amount = 145. See the exp parameter 
     in currencies.json, it shows the number of digits past the decimal point 
     for each currency (2 for the majority of currencies)."""
 
 
 class ShippingAddress(Model):
-    """Object `ShippingAddress`, see the [documentation](https://core.telegram.org/bots/api#shippingaddress)
+    """Object `ShippingAddress`, see the [documentation](https://core.telegram.org/bots/api#shippingaddress).
 
-    This object represents a shipping address."""
+    This object represents a shipping address.
+    """
 
     country_code: str
-    """Two-letter ISO 3166-1 alpha-2 country code"""
+    """Two-letter ISO 3166-1 alpha-2 country code."""
 
     state: str
-    """State, if applicable"""
+    """State, if applicable."""
 
     city: str
-    """City"""
+    """City."""
 
     street_line1: str
-    """First line for the address"""
+    """First line for the address."""
 
     street_line2: str
-    """Second line for the address"""
+    """Second line for the address."""
 
     post_code: str
-    """Address post code"""
+    """Address post code."""
 
 
 class OrderInfo(Model):
-    """Object `OrderInfo`, see the [documentation](https://core.telegram.org/bots/api#orderinfo)
+    """Object `OrderInfo`, see the [documentation](https://core.telegram.org/bots/api#orderinfo).
 
-    This object represents information about an order."""
+    This object represents information about an order.
+    """
 
     name: Option[str] = Nothing
-    """Optional. User name"""
+    """Optional. User name."""
 
     phone_number: Option[str] = Nothing
-    """Optional. User's phone number"""
+    """Optional. User's phone number."""
 
     email: Option[str] = Nothing
-    """Optional. User email"""
+    """Optional. User email."""
 
     shipping_address: Option["ShippingAddress"] = Nothing
-    """Optional. User shipping address"""
+    """Optional. User shipping address."""
 
 
 class ShippingOption(Model):
-    """Object `ShippingOption`, see the [documentation](https://core.telegram.org/bots/api#shippingoption)
+    """Object `ShippingOption`, see the [documentation](https://core.telegram.org/bots/api#shippingoption).
 
-    This object represents one shipping option."""
+    This object represents one shipping option.
+    """
 
     id: str
-    """Shipping option identifier"""
+    """Shipping option identifier."""
 
     title: str
-    """Option title"""
+    """Option title."""
 
     prices: list["LabeledPrice"]
-    """List of price portions"""
+    """List of price portions."""
 
 
 class SuccessfulPayment(Model):
-    """Object `SuccessfulPayment`, see the [documentation](https://core.telegram.org/bots/api#successfulpayment)
+    """Object `SuccessfulPayment`, see the [documentation](https://core.telegram.org/bots/api#successfulpayment).
 
-    This object contains basic information about a successful payment."""
+    This object contains basic information about a successful payment.
+    """
 
     currency: str
-    """Three-letter ISO 4217 currency code"""
+    """Three-letter ISO 4217 currency code."""
 
     total_amount: int
     """Total price in the smallest units of the currency (integer, not float/double). 
     For example, for a price of US$ 1.45 pass amount = 145. See the exp parameter 
     in currencies.json, it shows the number of digits past the decimal point 
     for each currency (2 for the majority of currencies)."""
 
     invoice_payload: str
-    """Bot specified invoice payload"""
+    """Bot specified invoice payload."""
 
     telegram_payment_charge_id: str
-    """Telegram payment identifier"""
+    """Telegram payment identifier."""
 
     provider_payment_charge_id: str
-    """Provider payment identifier"""
+    """Provider payment identifier."""
 
     shipping_option_id: Option[str] = Nothing
-    """Optional. Identifier of the shipping option chosen by the user"""
+    """Optional. Identifier of the shipping option chosen by the user."""
 
     order_info: Option["OrderInfo"] = Nothing
-    """Optional. Order information provided by the user"""
+    """Optional. Order information provided by the user."""
 
 
 class ShippingQuery(Model):
-    """Object `ShippingQuery`, see the [documentation](https://core.telegram.org/bots/api#shippingquery)
+    """Object `ShippingQuery`, see the [documentation](https://core.telegram.org/bots/api#shippingquery).
 
-    This object contains information about an incoming shipping query."""
+    This object contains information about an incoming shipping query.
+    """
 
     id: str
-    """Unique query identifier"""
+    """Unique query identifier."""
 
     from_: "User"
-    """User who sent the query"""
+    """User who sent the query."""
 
     invoice_payload: str
-    """Bot specified invoice payload"""
+    """Bot specified invoice payload."""
 
     shipping_address: "ShippingAddress"
-    """User specified shipping address"""
+    """User specified shipping address."""
 
 
 class PreCheckoutQuery(Model):
-    """Object `PreCheckoutQuery`, see the [documentation](https://core.telegram.org/bots/api#precheckoutquery)
+    """Object `PreCheckoutQuery`, see the [documentation](https://core.telegram.org/bots/api#precheckoutquery).
 
-    This object contains information about an incoming pre-checkout query."""
+    This object contains information about an incoming pre-checkout query.
+    """
 
     id: str
-    """Unique query identifier"""
+    """Unique query identifier."""
 
     from_: "User"
-    """User who sent the query"""
+    """User who sent the query."""
 
     currency: str
-    """Three-letter ISO 4217 currency code"""
+    """Three-letter ISO 4217 currency code."""
 
     total_amount: int
     """Total price in the smallest units of the currency (integer, not float/double). 
     For example, for a price of US$ 1.45 pass amount = 145. See the exp parameter 
     in currencies.json, it shows the number of digits past the decimal point 
     for each currency (2 for the majority of currencies)."""
 
     invoice_payload: str
-    """Bot specified invoice payload"""
+    """Bot specified invoice payload."""
 
     shipping_option_id: Option[str] = Nothing
-    """Optional. Identifier of the shipping option chosen by the user"""
+    """Optional. Identifier of the shipping option chosen by the user."""
 
     order_info: Option["OrderInfo"] = Nothing
-    """Optional. Order information provided by the user"""
+    """Optional. Order information provided by the user."""
 
 
 class PassportData(Model):
-    """Object `PassportData`, see the [documentation](https://core.telegram.org/bots/api#passportdata)
+    """Object `PassportData`, see the [documentation](https://core.telegram.org/bots/api#passportdata).
 
-    Describes Telegram Passport data shared with the bot by the user."""
+    Describes Telegram Passport data shared with the bot by the user.
+    """
 
     data: list["EncryptedPassportElement"]
     """Array with information about documents and other Telegram Passport elements 
-    that was shared with the bot"""
+    that was shared with the bot."""
 
     credentials: "EncryptedCredentials"
-    """Encrypted credentials required to decrypt the data"""
+    """Encrypted credentials required to decrypt the data."""
 
 
 class PassportFile(Model):
-    """Object `PassportFile`, see the [documentation](https://core.telegram.org/bots/api#passportfile)
+    """Object `PassportFile`, see the [documentation](https://core.telegram.org/bots/api#passportfile).
 
     This object represents a file uploaded to Telegram Passport. Currently all Telegram Passport files are in JPEG format when decrypted and don't exceed 10MB.
     """
 
     file_id: str
-    """Identifier for this file, which can be used to download or reuse the file"""
+    """Identifier for this file, which can be used to download or reuse the file."""
 
     file_unique_id: str
     """Unique identifier for this file, which is supposed to be the same over time 
     and for different bots. Can't be used to download or reuse the file."""
 
     file_size: int
-    """File size in bytes"""
+    """File size in bytes."""
 
-    file_date: int
-    """Unix time when the file was uploaded"""
+    file_date: datetime
+    """Unix time when the file was uploaded."""
 
 
 class EncryptedPassportElement(Model):
-    """Object `EncryptedPassportElement`, see the [documentation](https://core.telegram.org/bots/api#encryptedpassportelement)
+    """Object `EncryptedPassportElement`, see the [documentation](https://core.telegram.org/bots/api#encryptedpassportelement).
 
     Describes documents or other Telegram Passport elements shared with the bot by the user.
     """
 
-    type: str
+    type: EncryptedPassportElementType
     """Element type. One of `personal_details`, `passport`, `driver_license`, 
     `identity_card`, `internal_passport`, `address`, `utility_bill`, 
     `bank_statement`, `rental_agreement`, `passport_registration`, 
     `temporary_registration`, `phone_number`, `email`."""
 
     hash: str
-    """Base64-encoded element hash for using in PassportElementErrorUnspecified"""
+    """Base64-encoded element hash for using in PassportElementErrorUnspecified."""
 
     data: Option[str] = Nothing
     """Optional. Base64-encoded encrypted Telegram Passport element data provided 
-    by the user, available for `personal_details`, `passport`, `driver_license`, 
+    by the user; available only for `personal_details`, `passport`, `driver_license`, 
     `identity_card`, `internal_passport` and `address` types. Can be decrypted 
     and verified using the accompanying EncryptedCredentials."""
 
     phone_number: Option[str] = Nothing
-    """Optional. User's verified phone number, available only for `phone_number` 
-    type"""
+    """Optional. User's verified phone number; available only for `phone_number` 
+    type."""
 
     email: Option[str] = Nothing
-    """Optional. User's verified email address, available only for `email` type"""
+    """Optional. User's verified email address; available only for `email` type."""
 
     files: Option[list["PassportFile"]] = Nothing
-    """Optional. Array of encrypted files with documents provided by the user, 
-    available for `utility_bill`, `bank_statement`, `rental_agreement`, 
+    """Optional. Array of encrypted files with documents provided by the user; 
+    available only for `utility_bill`, `bank_statement`, `rental_agreement`, 
     `passport_registration` and `temporary_registration` types. Files 
     can be decrypted and verified using the accompanying EncryptedCredentials."""
 
     front_side: Option["PassportFile"] = Nothing
     """Optional. Encrypted file with the front side of the document, provided 
-    by the user. Available for `passport`, `driver_license`, `identity_card` 
+    by the user; available only for `passport`, `driver_license`, `identity_card` 
     and `internal_passport`. The file can be decrypted and verified using 
     the accompanying EncryptedCredentials."""
 
     reverse_side: Option["PassportFile"] = Nothing
     """Optional. Encrypted file with the reverse side of the document, provided 
-    by the user. Available for `driver_license` and `identity_card`. The 
-    file can be decrypted and verified using the accompanying EncryptedCredentials."""
+    by the user; available only for `driver_license` and `identity_card`. 
+    The file can be decrypted and verified using the accompanying EncryptedCredentials."""
 
     selfie: Option["PassportFile"] = Nothing
     """Optional. Encrypted file with the selfie of the user holding a document, 
-    provided by the user; available for `passport`, `driver_license`, `identity_card` 
-    and `internal_passport`. The file can be decrypted and verified using 
-    the accompanying EncryptedCredentials."""
+    provided by the user; available if requested for `passport`, `driver_license`, 
+    `identity_card` and `internal_passport`. The file can be decrypted and 
+    verified using the accompanying EncryptedCredentials."""
 
     translation: Option[list["PassportFile"]] = Nothing
     """Optional. Array of encrypted files with translated versions of documents 
-    provided by the user. Available if requested for `passport`, `driver_license`, 
+    provided by the user; available if requested for `passport`, `driver_license`, 
     `identity_card`, `internal_passport`, `utility_bill`, `bank_statement`, 
     `rental_agreement`, `passport_registration` and `temporary_registration` 
     types. Files can be decrypted and verified using the accompanying EncryptedCredentials."""
 
 
 class EncryptedCredentials(Model):
-    """Object `EncryptedCredentials`, see the [documentation](https://core.telegram.org/bots/api#encryptedcredentials)
+    """Object `EncryptedCredentials`, see the [documentation](https://core.telegram.org/bots/api#encryptedcredentials).
 
     Describes data required for decrypting and authenticating EncryptedPassportElement. See the Telegram Passport Documentation for a complete description of the data decryption and authentication processes.
     """
 
     data: str
     """Base64-encoded encrypted JSON-serialized data with unique user's payload, 
     data hashes and secrets required for EncryptedPassportElement decryption 
-    and authentication"""
+    and authentication."""
 
     hash: str
-    """Base64-encoded data hash for data authentication"""
+    """Base64-encoded data hash for data authentication."""
 
     secret: str
     """Base64-encoded secret, encrypted with the bot's public RSA key, required 
-    for data decryption"""
+    for data decryption."""
 
 
 class PassportElementErrorDataField(PassportElementError):
-    """Object `PassportElementErrorDataField`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrordatafield)
+    """Object `PassportElementErrorDataField`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrordatafield).
 
     Represents an issue in one of the data fields that was provided by the user. The error is considered resolved when the field's value changes.
     """
 
-    source: str
-    """Error source, must be data"""
+    source: typing.Literal["data"]
+    """Error source, must be data."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "passport",
+        "driver_license",
+        "identity_card",
+        "internal_passport",
+        "address",
+    ]
     """The section of the user's Telegram Passport which has the error, one of `personal_details`, 
     `passport`, `driver_license`, `identity_card`, `internal_passport`, 
-    `address`"""
+    `address`."""
 
     field_name: str
-    """Name of the data field which has the error"""
+    """Name of the data field which has the error."""
 
     data_hash: str
-    """Base64-encoded data hash"""
+    """Base64-encoded data hash."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorFrontSide(PassportElementError):
-    """Object `PassportElementErrorFrontSide`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfrontside)
+    """Object `PassportElementErrorFrontSide`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfrontside).
 
     Represents an issue with the front side of a document. The error is considered resolved when the file with the front side of the document changes.
     """
 
-    source: str
-    """Error source, must be front_side"""
+    source: typing.Literal["front_side"]
+    """Error source, must be front_side."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "passport",
+        "driver_license",
+        "identity_card",
+        "internal_passport",
+    ]
     """The section of the user's Telegram Passport which has the issue, one of `passport`, 
-    `driver_license`, `identity_card`, `internal_passport`"""
+    `driver_license`, `identity_card`, `internal_passport`."""
 
     file_hash: str
-    """Base64-encoded hash of the file with the front side of the document"""
+    """Base64-encoded hash of the file with the front side of the document."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorReverseSide(PassportElementError):
-    """Object `PassportElementErrorReverseSide`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorreverseside)
+    """Object `PassportElementErrorReverseSide`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorreverseside).
 
     Represents an issue with the reverse side of a document. The error is considered resolved when the file with reverse side of the document changes.
     """
 
-    source: str
-    """Error source, must be reverse_side"""
+    source: typing.Literal["reverse_side"]
+    """Error source, must be reverse_side."""
 
-    type: PassportElementErrorType
+    type: typing.Literal["driver_license", "identity_card"]
     """The section of the user's Telegram Passport which has the issue, one of `driver_license`, 
-    `identity_card`"""
+    `identity_card`."""
 
     file_hash: str
-    """Base64-encoded hash of the file with the reverse side of the document"""
+    """Base64-encoded hash of the file with the reverse side of the document."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorSelfie(PassportElementError):
-    """Object `PassportElementErrorSelfie`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorselfie)
+    """Object `PassportElementErrorSelfie`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorselfie).
 
     Represents an issue with the selfie with a document. The error is considered resolved when the file with the selfie changes.
     """
 
-    source: str
-    """Error source, must be selfie"""
+    source: typing.Literal["selfie"]
+    """Error source, must be selfie."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "passport",
+        "driver_license",
+        "identity_card",
+        "internal_passport",
+    ]
     """The section of the user's Telegram Passport which has the issue, one of `passport`, 
-    `driver_license`, `identity_card`, `internal_passport`"""
+    `driver_license`, `identity_card`, `internal_passport`."""
 
     file_hash: str
-    """Base64-encoded hash of the file with the selfie"""
+    """Base64-encoded hash of the file with the selfie."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorFile(PassportElementError):
-    """Object `PassportElementErrorFile`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfile)
+    """Object `PassportElementErrorFile`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfile).
 
     Represents an issue with a document scan. The error is considered resolved when the file with the document scan changes.
     """
 
-    source: str
-    """Error source, must be file"""
+    source: typing.Literal["file"]
+    """Error source, must be file."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "utility_bill",
+        "bank_statement",
+        "rental_agreement",
+        "passport_registration",
+        "temporary_registration",
+    ]
     """The section of the user's Telegram Passport which has the issue, one of `utility_bill`, 
     `bank_statement`, `rental_agreement`, `passport_registration`, 
-    `temporary_registration`"""
+    `temporary_registration`."""
 
     file_hash: str
-    """Base64-encoded file hash"""
+    """Base64-encoded file hash."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorFiles(PassportElementError):
-    """Object `PassportElementErrorFiles`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfiles)
+    """Object `PassportElementErrorFiles`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorfiles).
 
     Represents an issue with a list of scans. The error is considered resolved when the list of files containing the scans changes.
     """
 
-    source: str
-    """Error source, must be files"""
+    source: typing.Literal["files"]
+    """Error source, must be files."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "utility_bill",
+        "bank_statement",
+        "rental_agreement",
+        "passport_registration",
+        "temporary_registration",
+    ]
     """The section of the user's Telegram Passport which has the issue, one of `utility_bill`, 
     `bank_statement`, `rental_agreement`, `passport_registration`, 
-    `temporary_registration`"""
+    `temporary_registration`."""
 
     file_hashes: list[str]
-    """List of base64-encoded file hashes"""
+    """List of base64-encoded file hashes."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorTranslationFile(PassportElementError):
-    """Object `PassportElementErrorTranslationFile`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrortranslationfile)
+    """Object `PassportElementErrorTranslationFile`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrortranslationfile).
 
     Represents an issue with one of the files that constitute the translation of a document. The error is considered resolved when the file changes.
     """
 
-    source: str
-    """Error source, must be translation_file"""
+    source: typing.Literal["translation_file"]
+    """Error source, must be translation_file."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "passport",
+        "driver_license",
+        "identity_card",
+        "internal_passport",
+        "utility_bill",
+        "bank_statement",
+        "rental_agreement",
+        "passport_registration",
+        "temporary_registration",
+    ]
     """Type of element of the user's Telegram Passport which has the issue, one 
     of `passport`, `driver_license`, `identity_card`, `internal_passport`, 
     `utility_bill`, `bank_statement`, `rental_agreement`, `passport_registration`, 
-    `temporary_registration`"""
+    `temporary_registration`."""
 
     file_hash: str
-    """Base64-encoded file hash"""
+    """Base64-encoded file hash."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorTranslationFiles(PassportElementError):
-    """Object `PassportElementErrorTranslationFiles`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrortranslationfiles)
+    """Object `PassportElementErrorTranslationFiles`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrortranslationfiles).
 
     Represents an issue with the translated version of a document. The error is considered resolved when a file with the document translation change.
     """
 
-    source: str
-    """Error source, must be translation_files"""
+    source: typing.Literal["translation_files"]
+    """Error source, must be translation_files."""
 
-    type: PassportElementErrorType
+    type: typing.Literal[
+        "passport",
+        "driver_license",
+        "identity_card",
+        "internal_passport",
+        "utility_bill",
+        "bank_statement",
+        "rental_agreement",
+        "passport_registration",
+        "temporary_registration",
+    ]
     """Type of element of the user's Telegram Passport which has the issue, one 
     of `passport`, `driver_license`, `identity_card`, `internal_passport`, 
     `utility_bill`, `bank_statement`, `rental_agreement`, `passport_registration`, 
-    `temporary_registration`"""
+    `temporary_registration`."""
 
     file_hashes: list[str]
-    """List of base64-encoded file hashes"""
+    """List of base64-encoded file hashes."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class PassportElementErrorUnspecified(PassportElementError):
-    """Object `PassportElementErrorUnspecified`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorunspecified)
+    """Object `PassportElementErrorUnspecified`, see the [documentation](https://core.telegram.org/bots/api#passportelementerrorunspecified).
 
     Represents an issue in an unspecified place. The error is considered resolved when new data is added.
     """
 
-    source: str
-    """Error source, must be unspecified"""
+    source: typing.Literal["unspecified"]
+    """Error source, must be unspecified."""
 
-    type: PassportElementErrorType
-    """Type of element of the user's Telegram Passport which has the issue"""
+    type: EncryptedPassportElementType
+    """Type of element of the user's Telegram Passport which has the issue."""
 
     element_hash: str
-    """Base64-encoded element hash"""
+    """Base64-encoded element hash."""
 
     message: str
-    """Error message"""
+    """Error message."""
 
 
 class Game(Model):
-    """Object `Game`, see the [documentation](https://core.telegram.org/bots/api#game)
+    """Object `Game`, see the [documentation](https://core.telegram.org/bots/api#game).
 
     This object represents a game. Use BotFather to create and edit games, their short names will act as unique identifiers.
     """
 
     title: str
-    """Title of the game"""
+    """Title of the game."""
 
     description: str
-    """Description of the game"""
+    """Description of the game."""
 
     photo: list["PhotoSize"]
     """Photo that will be displayed in the game message in chats."""
 
     text: Option[str] = Nothing
     """Optional. Brief description of the game or high scores included in the game 
     message. Can be automatically edited to include current high scores for 
@@ -5169,31 +5598,31 @@
 
     text_entities: Option[list["MessageEntity"]] = Nothing
     """Optional. Special entities that appear in text, such as usernames, URLs, 
     bot commands, etc."""
 
     animation: Option["Animation"] = Nothing
     """Optional. Animation that will be displayed in the game message in chats. 
-    Upload via BotFather"""
+    Upload via BotFather."""
 
 
 class CallbackGame(Model):
-    """Object `CallbackGame`, see the [documentation](https://core.telegram.org/bots/api#callbackgame)
-
-    A placeholder, currently holds no information. Use BotFather to set up your game."""
+    """Object `CallbackGame`, see the [documentation](https://core.telegram.org/bots/api#callbackgame).
 
-    pass
+    A placeholder, currently holds no information. Use BotFather to set up your game.
+    """
 
 
 class GameHighScore(Model):
-    """Object `GameHighScore`, see the [documentation](https://core.telegram.org/bots/api#gamehighscore)
+    """Object `GameHighScore`, see the [documentation](https://core.telegram.org/bots/api#gamehighscore).
 
-    This object represents one row of the high scores table for a game."""
+    This object represents one row of the high scores table for a game.
+    """
 
     position: int
-    """Position in high score table for the game"""
+    """Position in high score table for the game."""
 
     user: "User"
-    """User"""
+    """User."""
 
     score: int
-    """Score"""
+    """Score."""
```

### Comparing `mubble-1.0.0/pyproject.toml` & `mubble-1.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mubble"
-version = "1.0.0"
+version = "1.1.0"
 description = "Async Telegram framework for bot building"
 readme = "README.md"
 authors = ["vladislavkovalskyi <vladislavkovalskyi@icloud.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -14,13 +14,14 @@
 msgspec = "^0.18.4"
 envparse = "^0.2.0"
 PyYAML = "^6.0"
 choicelib = "^0.1.5"
 certifi = "^2022.6.15"
 colorama = "^0.4.0"
 typing-extensions = "^4.8.0"
+fntypes = "^0.1.2.post1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mubble-1.0.0/README.md` & `mubble-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,200 +1,220 @@
-00000000: 2320 4d75 6262 6c65 0d0a 215b 4d75 6262  # Mubble..![Mubb
-00000010: 6c65 206c 6f67 6f5d 2869 6d61 6765 732f  le logo](images/
-00000020: 6d75 6262 6c65 5f6c 6f67 6f2e 706e 6729  mubble_logo.png)
-00000030: 0d0a 5b21 5b44 6f77 6e6c 6f61 6473 5d28  ..[![Downloads](
-00000040: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000050: 6c64 732e 696f 2f70 7970 692f 646d 2f6d  lds.io/pypi/dm/m
-00000060: 7562 626c 652e 7376 673f 7374 796c 653d  ubble.svg?style=
-00000070: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
-00000080: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000090: 6e2e 6f72 672f 7079 7069 2f6d 7562 626c  n.org/pypi/mubbl
-000000a0: 6529 0d0a 5b21 5b44 6f77 6e6c 6f61 6473  e)..[![Downloads
-000000b0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000000c0: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-000000d0: 7665 7273 696f 6e73 2f6d 7562 626c 652e  versions/mubble.
-000000e0: 7376 673f 7374 796c 653d 666c 6174 2d73  svg?style=flat-s
-000000f0: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
-00000100: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-00000110: 7079 7069 2f6d 7562 626c 6529 0d0a 0d0a  pypi/mubble)....
-00000120: 0d0a 2a2a 4d75 6262 6c65 2a2a 2069 7320  ..**Mubble** is 
-00000130: 6120 6e65 7874 2d67 656e 6572 6174 696f  a next-generatio
-00000140: 6e20 6672 616d 6577 6f72 6b20 6b6e 6f77  n framework know
-00000150: 6e20 666f 7220 6974 7320 6772 6561 7420  n for its great 
-00000160: 7370 6565 6420 616e 6420 7369 6d70 6c69  speed and simpli
-00000170: 6369 7479 2e20 4974 2069 7320 7772 6974  city. It is writ
-00000180: 7465 6e20 7573 696e 6720 6169 6f68 7474  ten using aiohtt
-00000190: 702c 2061 7379 6e63 696f 2c20 616e 6420  p, asyncio, and 
-000001a0: 6d73 6773 7065 632e 3c62 723e 0d0a 2a28  msgspec.<br>..*(
-000001b0: 5b41 7574 686f 725d 2868 7474 7073 3a2f  [Author](https:/
-000001c0: 2f67 6974 6875 622e 636f 6d2f 766c 6164  /github.com/vlad
-000001d0: 6973 6c61 766b 6f76 616c 736b 7969 2927  islavkovalskyi)'
-000001e0: 7320 776f 7264 7329 2a0d 0a2a 2a4d 616b  s words)*..**Mak
-000001f0: 6520 7468 6520 6661 7374 6573 7420 626f  e the fastest bo
-00000200: 7420 6576 6572 212a 2a0d 0a0d 0a0d 0a23  t ever!**......#
-00000210: 2047 6574 7469 6e67 2073 7461 7274 6564   Getting started
-00000220: 0d0a 0d0a 0d0a 2323 2320 496e 7374 616c  ......### Instal
-00000230: 6c69 6e67 3a0d 0a55 7369 6e67 202a 2a70  ling:..Using **p
-00000240: 6970 2a2a 0d0a 6060 6062 6173 680d 0a70  ip**..```bash..p
-00000250: 6970 2069 6e73 7461 6c6c 206d 7562 626c  ip install mubbl
-00000260: 650d 0a60 6060 0d0a 5573 696e 6720 2a2a  e..```..Using **
-00000270: 706f 6574 7279 2a2a 0d0a 6060 6062 6173  poetry**..```bas
-00000280: 680d 0a70 6f65 7472 7920 6164 6420 6d75  h..poetry add mu
-00000290: 6262 6c65 0d0a 6060 600d 0a0d 0a23 2323  bble..```....###
-000002a0: 2045 7861 6d70 6c65 733a 0d0a 596f 7520   Examples:..You 
-000002b0: 6361 6e20 7573 6520 7468 6973 2066 696c  can use this fil
-000002c0: 6520 746f 2066 616d 696c 6961 7269 7a65  e to familiarize
-000002d0: 2079 6f75 7273 656c 6620 7769 7468 2074   yourself with t
-000002e0: 6865 2073 796e 7461 7820 6f66 2074 6865  he syntax of the
-000002f0: 2066 7261 6d65 776f 726b 2e0d 0a5b 215b   framework...[![
-00000300: 436c 6963 6b20 6d65 5d28 2e2f 696d 6167  Click me](./imag
-00000310: 6573 2f65 7861 6d70 6c65 735f 6275 7474  es/examples_butt
-00000320: 6f6e 2e70 6e67 295d 282e 2f65 7861 6d70  on.png)](./examp
-00000330: 6c65 732f 7374 6172 742e 6d64 290d 0a0d  les/start.md)...
-00000340: 0a0d 0a23 2323 2053 696d 706c 6520 626f  ...### Simple bo
-00000350: 7420 6578 616d 706c 653a 0d0a 6060 6070  t example:..```p
-00000360: 7974 686f 6e0d 0a69 6d70 6f72 7420 7261  ython..import ra
-00000370: 6e64 6f6d 0d0a 0d0a 6672 6f6d 206d 7562  ndom....from mub
-00000380: 626c 6520 696d 706f 7274 2054 6f6b 656e  ble import Token
-00000390: 2c20 4150 492c 204d 7562 626c 652c 204d  , API, Mubble, M
-000003a0: 6573 7361 6765 2c20 4361 6c6c 6261 636b  essage, Callback
-000003b0: 5175 6572 790d 0a66 726f 6d20 6d75 6262  Query..from mubb
-000003c0: 6c65 2e72 756c 6573 2069 6d70 6f72 7420  le.rules import 
-000003d0: 5374 6172 7443 6f6d 6d61 6e64 2c20 5465  StartCommand, Te
-000003e0: 7874 2c20 4d61 726b 7570 2c20 4361 6c6c  xt, Markup, Call
-000003f0: 6261 636b 4461 7461 0d0a 6672 6f6d 206d  backData..from m
-00000400: 7562 626c 652e 746f 6f6c 732e 6b65 7962  ubble.tools.keyb
-00000410: 6f61 7264 2069 6d70 6f72 7420 496e 6c69  oard import Inli
-00000420: 6e65 4b65 7962 6f61 7264 2c20 496e 6c69  neKeyboard, Inli
-00000430: 6e65 4275 7474 6f6e 0d0a 0d0a 6170 6920  neButton....api 
-00000440: 3d20 4150 4928 546f 6b65 6e28 2259 6f75  = API(Token("You
-00000450: 7220 746f 6b65 6e22 2929 0d0a 626f 7420  r token"))..bot 
-00000460: 3d20 4d75 6262 6c65 2861 7069 290d 0a0d  = Mubble(api)...
-00000470: 0a0d 0a63 6c61 7373 204b 6579 626f 6172  ...class Keyboar
-00000480: 643a 0d0a 2020 2020 6d65 6e75 203d 2028  d:..    menu = (
-00000490: 0d0a 2020 2020 2020 2020 496e 6c69 6e65  ..        Inline
-000004a0: 4b65 7962 6f61 7264 2829 0d0a 2020 2020  Keyboard()..    
-000004b0: 2020 2020 2e61 6464 2849 6e6c 696e 6542      .add(InlineB
-000004c0: 7574 746f 6e28 22e2 9c8d efb8 8f20 5772  utton("...... Wr
-000004d0: 6974 6520 6865 6c6c 6f22 2c20 6361 6c6c  ite hello", call
-000004e0: 6261 636b 5f64 6174 613d 2268 656c 6c6f  back_data="hello
-000004f0: 2229 290d 0a20 2020 2020 2020 202e 726f  "))..        .ro
-00000500: 7728 290d 0a20 2020 2020 2020 202e 6164  w()..        .ad
-00000510: 6428 496e 6c69 6e65 4275 7474 6f6e 2822  d(InlineButton("
-00000520: f09f 8d8c 2043 686f 6963 6520 6261 6e61  .... Choice bana
-00000530: 6e61 222c 2063 616c 6c62 6163 6b5f 6461  na", callback_da
-00000540: 7461 3d22 6261 6e61 6e61 2229 290d 0a20  ta="banana")).. 
-00000550: 2020 2020 2020 202e 6164 6428 496e 6c69         .add(Inli
-00000560: 6e65 4275 7474 6f6e 2822 f09f a59d 2043  neButton(".... C
-00000570: 686f 6963 6520 6b69 7769 222c 2063 616c  hoice kiwi", cal
-00000580: 6c62 6163 6b5f 6461 7461 3d22 6b69 7769  lback_data="kiwi
-00000590: 2229 290d 0a20 2020 2029 2e67 6574 5f6d  "))..    ).get_m
-000005a0: 6172 6b75 7028 290d 0a0d 0a20 2020 2062  arkup()....    b
-000005b0: 6163 6b20 3d20 280d 0a20 2020 2020 2020  ack = (..       
-000005c0: 2049 6e6c 696e 654b 6579 626f 6172 6428   InlineKeyboard(
-000005d0: 292e 6164 6428 496e 6c69 6e65 4275 7474  ).add(InlineButt
-000005e0: 6f6e 2822 e2ac 85ef b88f 2042 6163 6b22  on("...... Back"
-000005f0: 2c20 6361 6c6c 6261 636b 5f64 6174 613d  , callback_data=
-00000600: 226d 656e 7522 2929 0d0a 2020 2020 292e  "menu"))..    ).
-00000610: 6765 745f 6d61 726b 7570 2829 0d0a 0d0a  get_markup()....
-00000620: 0d0a 4062 6f74 2e6f 6e2e 6d65 7373 6167  ..@bot.on.messag
-00000630: 6528 5374 6172 7443 6f6d 6d61 6e64 2829  e(StartCommand()
-00000640: 290d 0a61 7379 6e63 2064 6566 2073 7461  )..async def sta
-00000650: 7274 5f68 616e 646c 6572 286d 6573 7361  rt_handler(messa
-00000660: 6765 3a20 4d65 7373 6167 6529 3a0d 0a20  ge: Message):.. 
-00000670: 2020 2061 7761 6974 206d 6573 7361 6765     await message
-00000680: 2e61 6e73 7765 7228 0d0a 2020 2020 2020  .answer(..      
-00000690: 2020 22f0 9f91 8b20 4865 6c6c 6f2c 2049    ".... Hello, I
-000006a0: 276d 204d 7562 626c 6521 2048 6f77 2063  'm Mubble! How c
-000006b0: 616e 2049 2068 656c 7020 796f 753f 5c6e  an I help you?\n
-000006c0: 5c6e 220d 0a20 2020 2020 2020 2022 4d79  \n"..        "My
-000006d0: 2061 7661 696c 6162 6c65 2063 6f6d 6d61   available comma
-000006e0: 6e64 733a 5c6e 220d 0a20 2020 2020 2020  nds:\n"..       
-000006f0: 2022 2d20 2f73 7461 7274 5c6e 220d 0a20   "- /start\n".. 
-00000700: 2020 2020 2020 2022 2d20 2f6d 656e 755c         "- /menu\
-00000710: 6e22 0d0a 2020 2020 2020 2020 222d 202f  n"..        "- /
-00000720: 7261 6e64 6f6d 205b 6672 6f6d 206e 756d  random [from num
-00000730: 6265 725d 205b 746f 206e 756d 6265 725d  ber] [to number]
-00000740: 220d 0a20 2020 2029 0d0a 0d0a 0d0a 4062  "..    )......@b
-00000750: 6f74 2e6f 6e2e 6d65 7373 6167 6528 5465  ot.on.message(Te
-00000760: 7874 2822 2f6d 656e 7522 2929 0d0a 6173  xt("/menu"))..as
-00000770: 796e 6320 6465 6620 6d65 6e75 5f68 616e  ync def menu_han
-00000780: 646c 6572 286d 6573 7361 6765 3a20 4d65  dler(message: Me
-00000790: 7373 6167 6529 3a0d 0a20 2020 2061 7761  ssage):..    awa
-000007a0: 6974 206d 6573 7361 6765 2e61 6e73 7765  it message.answe
-000007b0: 7228 0d0a 2020 2020 2020 2020 22f0 9f93  r(..        "...
-000007c0: 8320 4865 7265 2773 2079 6f75 7220 6d65  . Here's your me
-000007d0: 6e75 2120 5573 6520 7468 6520 6b65 7962  nu! Use the keyb
-000007e0: 6f61 7264 2e22 2c20 7265 706c 795f 6d61  oard.", reply_ma
-000007f0: 726b 7570 3d4b 6579 626f 6172 642e 6d65  rkup=Keyboard.me
-00000800: 6e75 0d0a 2020 2020 290d 0a0d 0a0d 0a40  nu..    )......@
-00000810: 626f 742e 6f6e 2e6d 6573 7361 6765 284d  bot.on.message(M
-00000820: 6172 6b75 7028 5b22 2f72 616e 646f 6d22  arkup(["/random"
-00000830: 2c20 222f 7261 6e64 6f6d 203c 613a 696e  , "/random <a:in
-00000840: 743e 203c 623a 696e 743e 225d 2929 0d0a  t> <b:int>"]))..
-00000850: 6173 796e 6320 6465 6620 7261 6e64 6f6d  async def random
-00000860: 5f68 616e 646c 6572 286d 6573 7361 6765  _handler(message
-00000870: 3a20 4d65 7373 6167 652c 2061 3a20 696e  : Message, a: in
-00000880: 7420 3d20 4e6f 6e65 2c20 623a 2069 6e74  t = None, b: int
-00000890: 203d 204e 6f6e 6529 3a0d 0a20 2020 2069   = None):..    i
-000008a0: 6620 4e6f 6e65 2069 6e20 2861 2c20 6229  f None in (a, b)
-000008b0: 3a0d 0a20 2020 2020 2020 2061 7761 6974  :..        await
-000008c0: 206d 6573 7361 6765 2e61 6e73 7765 7228   message.answer(
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 22f0  ..            ".
-000008e0: 9fa4 9320 5772 6f6e 6720 7379 6e74 6178  ... Wrong syntax
-000008f0: 2e20 596f 7520 616c 736f 206e 6565 6420  . You also need 
-00000900: 746f 2077 7269 7465 2074 6865 2066 6972  to write the fir
-00000910: 7374 206e 756d 6265 7220 616e 6420 7468  st number and th
-00000920: 6520 7365 636f 6e64 206e 756d 6265 722e  e second number.
-00000930: 220d 0a20 2020 2020 2020 2029 0d0a 2020  "..        )..  
-00000940: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-00000950: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-00000960: 652e 616e 7377 6572 2866 22f0 9f8e b220  e.answer(f".... 
-00000970: 596f 7572 2072 616e 646f 6d20 6e75 6d62  Your random numb
-00000980: 6572 2069 7320 7b72 616e 646f 6d2e 7261  er is {random.ra
-00000990: 6e64 696e 7428 612c 2062 297d 2229 0d0a  ndint(a, b)}")..
-000009a0: 0d0a 0d0a 4062 6f74 2e6f 6e2e 6361 6c6c  ....@bot.on.call
-000009b0: 6261 636b 5f71 7565 7279 2843 616c 6c62  back_query(Callb
-000009c0: 6163 6b44 6174 6128 226d 656e 7522 2929  ackData("menu"))
-000009d0: 0d0a 6173 796e 6320 6465 6620 6d65 6e75  ..async def menu
-000009e0: 5f68 616e 646c 6572 2863 713a 2043 616c  _handler(cq: Cal
-000009f0: 6c62 6163 6b51 7565 7279 293a 0d0a 2020  lbackQuery):..  
-00000a00: 2020 6177 6169 7420 6371 2e65 6469 745f    await cq.edit_
-00000a10: 7465 7874 280d 0a20 2020 2020 2020 2022  text(..        "
-00000a20: f09f 9383 2048 6572 6527 7320 796f 7572  .... Here's your
-00000a30: 206d 656e 7521 2055 7365 2074 6865 206b   menu! Use the k
-00000a40: 6579 626f 6172 642e 222c 2072 6570 6c79  eyboard.", reply
-00000a50: 5f6d 6172 6b75 703d 4b65 7962 6f61 7264  _markup=Keyboard
-00000a60: 2e6d 656e 750d 0a20 2020 2029 0d0a 0d0a  .menu..    )....
-00000a70: 0d0a 4062 6f74 2e6f 6e2e 6361 6c6c 6261  ..@bot.on.callba
-00000a80: 636b 5f71 7565 7279 2843 616c 6c62 6163  ck_query(Callbac
-00000a90: 6b44 6174 6128 2268 656c 6c6f 2229 290d  kData("hello")).
-00000aa0: 0a61 7379 6e63 2064 6566 2068 656c 6c6f  .async def hello
-00000ab0: 5f68 616e 646c 6572 2863 713a 2043 616c  _handler(cq: Cal
-00000ac0: 6c62 6163 6b51 7565 7279 293a 0d0a 2020  lbackQuery):..  
-00000ad0: 2020 6177 6169 7420 6371 2e65 6469 745f    await cq.edit_
-00000ae0: 7465 7874 2822 f09f 918b 2048 656c 6c6f  text(".... Hello
-00000af0: 2c20 4927 6d20 4d75 6262 6c65 2122 2c20  , I'm Mubble!", 
-00000b00: 7265 706c 795f 6d61 726b 7570 3d4b 6579  reply_markup=Key
-00000b10: 626f 6172 642e 6261 636b 290d 0a0d 0a0d  board.back).....
-00000b20: 0a40 626f 742e 6f6e 2e63 616c 6c62 6163  .@bot.on.callbac
-00000b30: 6b5f 7175 6572 7928 4361 6c6c 6261 636b  k_query(Callback
-00000b40: 4461 7461 285b 2262 616e 616e 6122 2c20  Data(["banana", 
-00000b50: 226b 6977 6922 5d29 290d 0a61 7379 6e63  "kiwi"]))..async
-00000b60: 2064 6566 2066 7275 6974 735f 6861 6e64   def fruits_hand
-00000b70: 6c65 7228 6371 3a20 4361 6c6c 6261 636b  ler(cq: Callback
-00000b80: 5175 6572 7929 3a0d 0a20 2020 2066 7275  Query):..    fru
-00000b90: 6974 7320 3d20 7b22 6261 6e61 6e61 223a  its = {"banana":
-00000ba0: 2022 f09f 8d8c 222c 2022 6b69 7769 223a   "....", "kiwi":
-00000bb0: 2022 f09f a59d 227d 0d0a 2020 2020 6966   "...."}..    if
-00000bc0: 2063 712e 6461 7461 2069 6e20 6672 7569   cq.data in frui
-00000bd0: 7473 3a0d 0a20 2020 2020 2020 2061 7761  ts:..        awa
-00000be0: 6974 2063 712e 616e 7377 6572 2866 2259  it cq.answer(f"Y
-00000bf0: 6f75 2063 6c69 636b 6564 206f 6e20 7468  ou clicked on th
-00000c00: 6520 7b66 7275 6974 735b 6371 2e64 6174  e {fruits[cq.dat
-00000c10: 615d 7d21 2229 0d0a 0d0a 0d0a 626f 742e  a]}!")......bot.
-00000c20: 7275 6e5f 666f 7265 7665 7228 290d 0a60  run_forever()..`
-00000c30: 6060 0d0a 0d0a d0a1 d0bb d0b0 d0b2 d0b0  ``..............
-00000c40: 20d0 a3d0 bad1 80d0 b0d1 97d0 bdd1 9621   ..............!
-00000c50: 20f0 9f87 baf0 9f87 a60d 0a0d 0a0d 0a2a   ..............*
-00000c60: 6279 2056 6c61 6479 736c 6176 204b 6f76  by Vladyslav Kov
-00000c70: 616c 736b 7969 2a                        alskyi*
+00000000: 2320 4d75 6262 6c65 0d0a 5b21 5b4d 7562  # Mubble..[![Mub
+00000010: 626c 6520 6c6f 676f 5d28 696d 6167 6573  ble logo](images
+00000020: 2f6d 7562 626c 655f 6c6f 676f 2e70 6e67  /mubble_logo.png
+00000030: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000040: 622e 636f 6d2f 766c 6164 6973 6c61 766b  b.com/vladislavk
+00000050: 6f76 616c 736b 7969 2f6d 7562 626c 652f  ovalskyi/mubble/
+00000060: 626c 6f62 2f6d 6173 7465 722f 696d 6167  blob/master/imag
+00000070: 6573 2f6d 7562 626c 655f 6c6f 676f 2e70  es/mubble_logo.p
+00000080: 6e67 290d 0a0d 0a5b 215b 446f 776e 6c6f  ng)....[![Downlo
+00000090: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
+000000a0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000000b0: 2f64 6d2f 6d75 6262 6c65 2e73 7667 3f73  /dm/mubble.svg?s
+000000c0: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+000000d0: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000000e0: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+000000f0: 6d75 6262 6c65 290d 0a5b 215b 446f 776e  mubble)..[![Down
+00000100: 6c6f 6164 735d 2868 7474 7073 3a2f 2f69  loads](https://i
+00000110: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000120: 7069 2f70 7976 6572 7369 6f6e 732f 6d75  pi/pyversions/mu
+00000130: 6262 6c65 2e73 7667 3f73 7479 6c65 3d66  bble.svg?style=f
+00000140: 6c61 742d 7371 7561 7265 295d 2868 7474  lat-square)](htt
+00000150: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+00000160: 2e6f 7267 2f70 7970 692f 6d75 6262 6c65  .org/pypi/mubble
+00000170: 290d 0a0d 0a3c 6120 6872 6566 3d22 6874  )....<a href="ht
+00000180: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000190: 2f76 6c61 6469 736c 6176 6b6f 7661 6c73  /vladislavkovals
+000001a0: 6b79 692f 6d75 6262 6c65 223e 0d0a 2020  kyi/mubble">..  
+000001b0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000001c0: 2f2f 7570 6c6f 6164 2e77 696b 696d 6564  //upload.wikimed
+000001d0: 6961 2e6f 7267 2f77 696b 6970 6564 6961  ia.org/wikipedia
+000001e0: 2f63 6f6d 6d6f 6e73 2f74 6875 6d62 2f35  /commons/thumb/5
+000001f0: 2f35 342f 4769 7448 7562 5f4c 6f67 6f2e  /54/GitHub_Logo.
+00000200: 706e 672f 3830 3070 782d 4769 7448 7562  png/800px-GitHub
+00000210: 5f4c 6f67 6f2e 706e 6722 2061 6c74 3d22  _Logo.png" alt="
+00000220: 436c 6963 6b20 6d65 2220 7769 6474 683d  Click me" width=
+00000230: 2233 3025 223e 0d0a 3c2f 613e 0d0a 3c62  "30%">..</a>..<b
+00000240: 723e 0d0a 0d0a 5f28 636c 6963 6b61 626c  r>...._(clickabl
+00000250: 6529 5f0d 0a0d 0a3c 6272 3e0d 0a3c 6272  e)_....<br>..<br
+00000260: 3e0d 0a0d 0a2a 2a4d 7562 626c 652a 2a20  >....**Mubble** 
+00000270: 6973 2061 206e 6578 742d 6765 6e65 7261  is a next-genera
+00000280: 7469 6f6e 2066 7261 6d65 776f 726b 206b  tion framework k
+00000290: 6e6f 776e 2066 6f72 2069 7473 2067 7265  nown for its gre
+000002a0: 6174 2073 7065 6564 2061 6e64 2073 696d  at speed and sim
+000002b0: 706c 6963 6974 792e 2049 7420 6973 2077  plicity. It is w
+000002c0: 7269 7474 656e 2075 7369 6e67 2061 696f  ritten using aio
+000002d0: 6874 7470 2c20 6173 796e 6369 6f2c 2061  http, asyncio, a
+000002e0: 6e64 206d 7367 7370 6563 2e3c 6272 3e0d  nd msgspec.<br>.
+000002f0: 0a2a 285b 4175 7468 6f72 5d28 6874 7470  .*([Author](http
+00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
+00000310: 6c61 6469 736c 6176 6b6f 7661 6c73 6b79  ladislavkovalsky
+00000320: 6929 2773 2077 6f72 6473 292a 0d0a 2a2a  i)'s words)*..**
+00000330: 4d61 6b65 2074 6865 2066 6173 7465 7374  Make the fastest
+00000340: 2062 6f74 2065 7665 7221 2a2a 0d0a 0d0a   bot ever!**....
+00000350: 3c21 2d2d 2020 2d2d 3e0d 0a23 2047 6574  <!--  -->..# Get
+00000360: 7469 6e67 2073 7461 7274 6564 0d0a 0d0a  ting started....
+00000370: 0d0a 2323 2320 496e 7374 616c 6c69 6e67  ..### Installing
+00000380: 3a0d 0a55 7369 6e67 202a 2a70 6970 2a2a  :..Using **pip**
+00000390: 0d0a 6060 6062 6173 680d 0a70 6970 2069  ..```bash..pip i
+000003a0: 6e73 7461 6c6c 206d 7562 626c 650d 0a60  nstall mubble..`
+000003b0: 6060 0d0a 5573 696e 6720 2a2a 706f 6574  ``..Using **poet
+000003c0: 7279 2a2a 0d0a 6060 6062 6173 680d 0a70  ry**..```bash..p
+000003d0: 6f65 7472 7920 6164 6420 6d75 6262 6c65  oetry add mubble
+000003e0: 0d0a 6060 600d 0a0d 0a23 2323 2045 7861  ..```....### Exa
+000003f0: 6d70 6c65 733a 0d0a 596f 7520 6361 6e20  mples:..You can 
+00000400: 7573 6520 7468 6973 2066 696c 6520 746f  use this file to
+00000410: 2066 616d 696c 6961 7269 7a65 2079 6f75   familiarize you
+00000420: 7273 656c 6620 7769 7468 2074 6865 2073  rself with the s
+00000430: 796e 7461 7820 6f66 2074 6865 2066 7261  yntax of the fra
+00000440: 6d65 776f 726b 2e0d 0a0d 0a3c 6120 6872  mework.....<a hr
+00000450: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000460: 7562 2e63 6f6d 2f76 6c61 6469 736c 6176  ub.com/vladislav
+00000470: 6b6f 7661 6c73 6b79 692f 6d75 6262 6c65  kovalskyi/mubble
+00000480: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00000490: 6d70 6c65 732f 7374 6172 742e 6d64 223e  mples/start.md">
+000004a0: 0d0a 2020 3c69 6d67 2073 7263 3d22 6874  ..  <img src="ht
+000004b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004c0: 2f76 6c61 6469 736c 6176 6b6f 7661 6c73  /vladislavkovals
+000004d0: 6b79 692f 6d75 6262 6c65 2f62 6c6f 622f  kyi/mubble/blob/
+000004e0: 6d61 7374 6572 2f69 6d61 6765 732f 6578  master/images/ex
+000004f0: 616d 706c 6573 5f62 7574 746f 6e2e 706e  amples_button.pn
+00000500: 673f 7261 773d 7472 7565 2220 616c 743d  g?raw=true" alt=
+00000510: 2243 6c69 636b 206d 6522 2077 6964 7468  "Click me" width
+00000520: 3d22 3130 3025 223e 0d0a 3c2f 613e 0d0a  ="100%">..</a>..
+00000530: 0d0a 2323 2320 5369 6d70 6c65 2062 6f74  ..### Simple bot
+00000540: 2065 7861 6d70 6c65 3a0d 0a60 6060 7079   example:..```py
+00000550: 7468 6f6e 0d0a 696d 706f 7274 2072 616e  thon..import ran
+00000560: 646f 6d0d 0a0d 0a66 726f 6d20 6d75 6262  dom....from mubb
+00000570: 6c65 2069 6d70 6f72 7420 546f 6b65 6e2c  le import Token,
+00000580: 2041 5049 2c20 4d75 6262 6c65 2c20 4d65   API, Mubble, Me
+00000590: 7373 6167 652c 2043 616c 6c62 6163 6b51  ssage, CallbackQ
+000005a0: 7565 7279 0d0a 6672 6f6d 206d 7562 626c  uery..from mubbl
+000005b0: 652e 7275 6c65 7320 696d 706f 7274 2053  e.rules import S
+000005c0: 7461 7274 436f 6d6d 616e 642c 2054 6578  tartCommand, Tex
+000005d0: 742c 204d 6172 6b75 702c 2043 616c 6c62  t, Markup, Callb
+000005e0: 6163 6b44 6174 610d 0a66 726f 6d20 6d75  ackData..from mu
+000005f0: 6262 6c65 2e74 6f6f 6c73 2e6b 6579 626f  bble.tools.keybo
+00000600: 6172 6420 696d 706f 7274 2049 6e6c 696e  ard import Inlin
+00000610: 654b 6579 626f 6172 642c 2049 6e6c 696e  eKeyboard, Inlin
+00000620: 6542 7574 746f 6e0d 0a0d 0a61 7069 203d  eButton....api =
+00000630: 2041 5049 2854 6f6b 656e 2822 596f 7572   API(Token("Your
+00000640: 2074 6f6b 656e 2229 290d 0a62 6f74 203d   token"))..bot =
+00000650: 204d 7562 626c 6528 6170 6929 0d0a 0d0a   Mubble(api)....
+00000660: 0d0a 636c 6173 7320 4b65 7962 6f61 7264  ..class Keyboard
+00000670: 3a0d 0a20 2020 206d 656e 7520 3d20 280d  :..    menu = (.
+00000680: 0a20 2020 2020 2020 2049 6e6c 696e 654b  .        InlineK
+00000690: 6579 626f 6172 6428 290d 0a20 2020 2020  eyboard()..     
+000006a0: 2020 202e 6164 6428 496e 6c69 6e65 4275     .add(InlineBu
+000006b0: 7474 6f6e 2822 e29c 8def b88f 2057 7269  tton("...... Wri
+000006c0: 7465 2068 656c 6c6f 222c 2063 616c 6c62  te hello", callb
+000006d0: 6163 6b5f 6461 7461 3d22 6865 6c6c 6f22  ack_data="hello"
+000006e0: 2929 0d0a 2020 2020 2020 2020 2e72 6f77  ))..        .row
+000006f0: 2829 0d0a 2020 2020 2020 2020 2e61 6464  ()..        .add
+00000700: 2849 6e6c 696e 6542 7574 746f 6e28 22f0  (InlineButton(".
+00000710: 9f8d 8c20 4368 6f69 6365 2062 616e 616e  ... Choice banan
+00000720: 6122 2c20 6361 6c6c 6261 636b 5f64 6174  a", callback_dat
+00000730: 613d 2262 616e 616e 6122 2929 0d0a 2020  a="banana"))..  
+00000740: 2020 292e 6765 745f 6d61 726b 7570 2829    ).get_markup()
+00000750: 0d0a 0d0a 2020 2020 6261 636b 203d 2028  ....    back = (
+00000760: 0d0a 2020 2020 2020 2020 496e 6c69 6e65  ..        Inline
+00000770: 4b65 7962 6f61 7264 2829 2e61 6464 2849  Keyboard().add(I
+00000780: 6e6c 696e 6542 7574 746f 6e28 22e2 ac85  nlineButton("...
+00000790: efb8 8f20 4261 636b 222c 2063 616c 6c62  ... Back", callb
+000007a0: 6163 6b5f 6461 7461 3d22 6d65 6e75 2229  ack_data="menu")
+000007b0: 290d 0a20 2020 2029 2e67 6574 5f6d 6172  )..    ).get_mar
+000007c0: 6b75 7028 290d 0a0d 0a0d 0a40 626f 742e  kup()......@bot.
+000007d0: 6f6e 2e6d 6573 7361 6765 2853 7461 7274  on.message(Start
+000007e0: 436f 6d6d 616e 6428 2929 0d0a 6173 796e  Command())..asyn
+000007f0: 6320 6465 6620 7374 6172 745f 6861 6e64  c def start_hand
+00000800: 6c65 7228 6d65 7373 6167 653a 204d 6573  ler(message: Mes
+00000810: 7361 6765 293a 0d0a 2020 2020 6177 6169  sage):..    awai
+00000820: 7420 6d65 7373 6167 652e 616e 7377 6572  t message.answer
+00000830: 280d 0a20 2020 2020 2020 2022 f09f 918b  (..        "....
+00000840: 2048 656c 6c6f 2c20 4927 6d20 4d75 6262   Hello, I'm Mubb
+00000850: 6c65 2120 486f 7720 6361 6e20 4920 6865  le! How can I he
+00000860: 6c70 2079 6f75 3f5c 6e5c 6e22 0d0a 2020  lp you?\n\n"..  
+00000870: 2020 2020 2020 224d 7920 6176 6169 6c61        "My availa
+00000880: 626c 6520 636f 6d6d 616e 6473 3a5c 6e22  ble commands:\n"
+00000890: 0d0a 2020 2020 2020 2020 222d 202f 7374  ..        "- /st
+000008a0: 6172 745c 6e22 0d0a 2020 2020 2020 2020  art\n"..        
+000008b0: 222d 202f 6d65 6e75 5c6e 220d 0a20 2020  "- /menu\n"..   
+000008c0: 2020 2020 2022 2d20 2f72 616e 646f 6d20       "- /random 
+000008d0: 5b66 726f 6d20 6e75 6d62 6572 5d20 5b74  [from number] [t
+000008e0: 6f20 6e75 6d62 6572 5d22 0d0a 2020 2020  o number]"..    
+000008f0: 290d 0a0d 0a0d 0a40 626f 742e 6f6e 2e6d  )......@bot.on.m
+00000900: 6573 7361 6765 2854 6578 7428 222f 6d65  essage(Text("/me
+00000910: 6e75 2229 290d 0a61 7379 6e63 2064 6566  nu"))..async def
+00000920: 206d 656e 755f 6861 6e64 6c65 7228 6d65   menu_handler(me
+00000930: 7373 6167 653a 204d 6573 7361 6765 293a  ssage: Message):
+00000940: 0d0a 2020 2020 6177 6169 7420 6d65 7373  ..    await mess
+00000950: 6167 652e 616e 7377 6572 280d 0a20 2020  age.answer(..   
+00000960: 2020 2020 2022 f09f 9383 2048 6572 6527       ".... Here'
+00000970: 7320 796f 7572 206d 656e 7521 2055 7365  s your menu! Use
+00000980: 2074 6865 206b 6579 626f 6172 642e 222c   the keyboard.",
+00000990: 2072 6570 6c79 5f6d 6172 6b75 703d 4b65   reply_markup=Ke
+000009a0: 7962 6f61 7264 2e6d 656e 750d 0a20 2020  yboard.menu..   
+000009b0: 2029 0d0a 0d0a 0d0a 4062 6f74 2e6f 6e2e   )......@bot.on.
+000009c0: 6d65 7373 6167 6528 4d61 726b 7570 285b  message(Markup([
+000009d0: 222f 7261 6e64 6f6d 222c 2022 2f72 616e  "/random", "/ran
+000009e0: 646f 6d20 3c61 3a69 6e74 3e20 3c62 3a69  dom <a:int> <b:i
+000009f0: 6e74 3e22 5d29 290d 0a61 7379 6e63 2064  nt>"]))..async d
+00000a00: 6566 2072 616e 646f 6d5f 6861 6e64 6c65  ef random_handle
+00000a10: 7228 6d65 7373 6167 653a 204d 6573 7361  r(message: Messa
+00000a20: 6765 2c20 613a 2069 6e74 203d 204e 6f6e  ge, a: int = Non
+00000a30: 652c 2062 3a20 696e 7420 3d20 4e6f 6e65  e, b: int = None
+00000a40: 293a 0d0a 2020 2020 6966 204e 6f6e 6520  ):..    if None 
+00000a50: 696e 2028 612c 2062 293a 0d0a 2020 2020  in (a, b):..    
+00000a60: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
+00000a70: 652e 616e 7377 6572 280d 0a20 2020 2020  e.answer(..     
+00000a80: 2020 2020 2020 2022 f09f a493 2057 726f         ".... Wro
+00000a90: 6e67 2073 796e 7461 782e 2059 6f75 2061  ng syntax. You a
+00000aa0: 6c73 6f20 6e65 6564 2074 6f20 7772 6974  lso need to writ
+00000ab0: 6520 7468 6520 6669 7273 7420 6e75 6d62  e the first numb
+00000ac0: 6572 2061 6e64 2074 6865 2073 6563 6f6e  er and the secon
+00000ad0: 6420 6e75 6d62 6572 2e22 0d0a 2020 2020  d number."..    
+00000ae0: 2020 2020 290d 0a20 2020 2020 2020 2072      )..        r
+00000af0: 6574 7572 6e0d 0a0d 0a20 2020 2061 7761  eturn....    awa
+00000b00: 6974 206d 6573 7361 6765 2e61 6e73 7765  it message.answe
+00000b10: 7228 6622 f09f 8eb2 2059 6f75 7220 7261  r(f".... Your ra
+00000b20: 6e64 6f6d 206e 756d 6265 7220 6973 207b  ndom number is {
+00000b30: 7261 6e64 6f6d 2e72 616e 6469 6e74 2861  random.randint(a
+00000b40: 2c20 6229 7d22 290d 0a0d 0a0d 0a40 626f  , b)}")......@bo
+00000b50: 742e 6f6e 2e63 616c 6c62 6163 6b5f 7175  t.on.callback_qu
+00000b60: 6572 7928 4361 6c6c 6261 636b 4461 7461  ery(CallbackData
+00000b70: 2822 6d65 6e75 2229 290d 0a61 7379 6e63  ("menu"))..async
+00000b80: 2064 6566 206d 656e 755f 6861 6e64 6c65   def menu_handle
+00000b90: 7228 6371 3a20 4361 6c6c 6261 636b 5175  r(cq: CallbackQu
+00000ba0: 6572 7929 3a0d 0a20 2020 2061 7761 6974  ery):..    await
+00000bb0: 2063 712e 6564 6974 5f74 6578 7428 0d0a   cq.edit_text(..
+00000bc0: 2020 2020 2020 2020 22f0 9f93 8320 4865          ".... He
+00000bd0: 7265 2773 2079 6f75 7220 6d65 6e75 2120  re's your menu! 
+00000be0: 5573 6520 7468 6520 6b65 7962 6f61 7264  Use the keyboard
+00000bf0: 2e22 2c20 7265 706c 795f 6d61 726b 7570  .", reply_markup
+00000c00: 3d4b 6579 626f 6172 642e 6d65 6e75 0d0a  =Keyboard.menu..
+00000c10: 2020 2020 290d 0a0d 0a0d 0a40 626f 742e      )......@bot.
+00000c20: 6f6e 2e63 616c 6c62 6163 6b5f 7175 6572  on.callback_quer
+00000c30: 7928 4361 6c6c 6261 636b 4461 7461 2822  y(CallbackData("
+00000c40: 6865 6c6c 6f22 2929 0d0a 6173 796e 6320  hello"))..async 
+00000c50: 6465 6620 6865 6c6c 6f5f 6861 6e64 6c65  def hello_handle
+00000c60: 7228 6371 3a20 4361 6c6c 6261 636b 5175  r(cq: CallbackQu
+00000c70: 6572 7929 3a0d 0a20 2020 2061 7761 6974  ery):..    await
+00000c80: 2063 712e 6564 6974 5f74 6578 7428 22f0   cq.edit_text(".
+00000c90: 9f91 8b20 4865 6c6c 6f2c 2049 276d 204d  ... Hello, I'm M
+00000ca0: 7562 626c 6521 222c 2072 6570 6c79 5f6d  ubble!", reply_m
+00000cb0: 6172 6b75 703d 4b65 7962 6f61 7264 2e62  arkup=Keyboard.b
+00000cc0: 6163 6b29 0d0a 0d0a 0d0a 4062 6f74 2e6f  ack)......@bot.o
+00000cd0: 6e2e 6361 6c6c 6261 636b 5f71 7565 7279  n.callback_query
+00000ce0: 2843 616c 6c62 6163 6b44 6174 6128 2262  (CallbackData("b
+00000cf0: 616e 616e 6122 2929 0d0a 6173 796e 6320  anana"))..async 
+00000d00: 6465 6620 6672 7569 7473 5f68 616e 646c  def fruits_handl
+00000d10: 6572 2863 713a 2043 616c 6c62 6163 6b51  er(cq: CallbackQ
+00000d20: 7565 7279 293a 0d0a 2020 2020 6177 6169  uery):..    awai
+00000d30: 7420 6371 2e61 6e73 7765 7228 2259 6f75  t cq.answer("You
+00000d40: 2063 6c69 636b 6564 206f 6e20 7468 6520   clicked on the 
+00000d50: f09f 8d8c 2122 290d 0a0d 0a0d 0a62 6f74  ....!")......bot
+00000d60: 2e72 756e 5f66 6f72 6576 6572 2829 0d0a  .run_forever()..
+00000d70: 6060 600d 0a0d 0ad0 a1d0 bbd0 b0d0 b2d0  ```.............
+00000d80: b020 d0a3 d0ba d180 d0b0 d197 d0bd d196  . ..............
+00000d90: 2120 f09f 87ba f09f 87a6 0d0a 0d0a 0d0a  ! ..............
+00000da0: 2a62 7920 566c 6164 7973 6c61 7620 4b6f  *by Vladyslav Ko
+00000db0: 7661 6c73 6b79 692a 0d0a                 valskyi*..
```

### Comparing `mubble-1.0.0/PKG-INFO` & `mubble-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mubble
-Version: 1.0.0
+Version: 1.1.0
 Summary: Async Telegram framework for bot building
 License: MIT
 Author: vladislavkovalskyi
 Author-email: vladislavkovalskyi@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,31 +12,42 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
 Requires-Dist: choicelib (>=0.1.5,<0.2.0)
 Requires-Dist: colorama (>=0.4.0,<0.5.0)
 Requires-Dist: envparse (>=0.2.0,<0.3.0)
+Requires-Dist: fntypes (>=0.1.2.post1,<0.2.0)
 Requires-Dist: msgspec (>=0.18.4,<0.19.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Requires-Dist: vbml (>=1.1.post1,<2.0)
 Description-Content-Type: text/markdown
 
 # Mubble
-![Mubble logo](images/mubble_logo.png)
+[![Mubble logo](images/mubble_logo.png)](https://github.com/vladislavkovalskyi/mubble/blob/master/images/mubble_logo.png)
+
 [![Downloads](https://img.shields.io/pypi/dm/mubble.svg?style=flat-square)](https://pypi.python.org/pypi/mubble)
 [![Downloads](https://img.shields.io/pypi/pyversions/mubble.svg?style=flat-square)](https://pypi.python.org/pypi/mubble)
 
+<a href="https://github.com/vladislavkovalskyi/mubble">
+  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/GitHub_Logo.png/800px-GitHub_Logo.png" alt="Click me" width="30%">
+</a>
+<br>
+
+_(clickable)_
+
+<br>
+<br>
 
 **Mubble** is a next-generation framework known for its great speed and simplicity. It is written using aiohttp, asyncio, and msgspec.<br>
 *([Author](https://github.com/vladislavkovalskyi)'s words)*
 **Make the fastest bot ever!**
 
-
+<!--  -->
 # Getting started
 
 
 ### Installing:
 Using **pip**
 ```bash
 pip install mubble
@@ -44,16 +55,18 @@
 Using **poetry**
 ```bash
 poetry add mubble
 ```
 
 ### Examples:
 You can use this file to familiarize yourself with the syntax of the framework.
-[![Click me](./images/examples_button.png)](./examples/start.md)
 
+<a href="https://github.com/vladislavkovalskyi/mubble/blob/master/examples/start.md">
+  <img src="https://github.com/vladislavkovalskyi/mubble/blob/master/images/examples_button.png?raw=true" alt="Click me" width="100%">
+</a>
 
 ### Simple bot example:
 ```python
 import random
 
 from mubble import Token, API, Mubble, Message, CallbackQuery
 from mubble.rules import StartCommand, Text, Markup, CallbackData
@@ -65,15 +78,14 @@
 
 class Keyboard:
     menu = (
         InlineKeyboard()
         .add(InlineButton("✍️ Write hello", callback_data="hello"))
         .row()
         .add(InlineButton("🍌 Choice banana", callback_data="banana"))
-        .add(InlineButton("🥝 Choice kiwi", callback_data="kiwi"))
     ).get_markup()
 
     back = (
         InlineKeyboard().add(InlineButton("⬅️ Back", callback_data="menu"))
     ).get_markup()
 
 
@@ -114,21 +126,20 @@
 
 
 @bot.on.callback_query(CallbackData("hello"))
 async def hello_handler(cq: CallbackQuery):
     await cq.edit_text("👋 Hello, I'm Mubble!", reply_markup=Keyboard.back)
 
 
-@bot.on.callback_query(CallbackData(["banana", "kiwi"]))
+@bot.on.callback_query(CallbackData("banana"))
 async def fruits_handler(cq: CallbackQuery):
-    fruits = {"banana": "🍌", "kiwi": "🥝"}
-    if cq.data in fruits:
-        await cq.answer(f"You clicked on the {fruits[cq.data]}!")
+    await cq.answer("You clicked on the 🍌!")
 
 
 bot.run_forever()
 ```
 
 Слава Україні! 🇺🇦
 
 
 *by Vladyslav Kovalskyi*
+
```

