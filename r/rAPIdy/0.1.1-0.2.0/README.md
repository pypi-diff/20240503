# Comparing `tmp/rapidy-0.1.1.tar.gz` & `tmp/rapidy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidy-0.1.1.tar", max compression
+gzip compressed data, was "rapidy-0.2.0.tar", max compression
```

## Comparing `rapidy-0.1.1.tar` & `rapidy-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,35 @@
--rw-r--r--   0        0        0     7762 2024-02-29 16:46:23.292255 rapidy-0.1.1/README.md
--rw-r--r--   0        0        0     5403 2024-02-29 16:46:23.292255 rapidy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/__init__.py
--rw-r--r--   0        0        0     9606 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_annotation_container.py
--rw-r--r--   0        0        0     2676 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_annotation_extractor.py
--rw-r--r--   0        0        0     4385 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_client_errors.py
--rw-r--r--   0        0        0     9294 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_extractors.py
--rw-r--r--   0        0        0      575 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_parsers.py
--rw-r--r--   0        0        0      474 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_request_params_base.py
--rw-r--r--   0        0        0     2594 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/_validators.py
--rw-r--r--   0        0        0      285 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/constants.py
--rw-r--r--   0        0        0     7284 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/fields.py
--rw-r--r--   0        0        0     3496 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/hdrs.py
--rw-r--r--   0        0        0      290 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/media_types.py
--rw-r--r--   0        0        0    10999 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/request_params.py
--rw-r--r--   0        0        0     1943 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/typedefs.py
--rw-r--r--   0        0        0     5421 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web.py
--rw-r--r--   0        0        0     8246 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_app.py
--rw-r--r--   0        0        0     3002 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_exceptions.py
--rw-r--r--   0        0        0      140 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_middlewares.py
--rw-r--r--   0        0        0      130 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_request.py
--rw-r--r--   0        0        0      183 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_response.py
--rw-r--r--   0        0        0      434 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_routedef.py
--rw-r--r--   0        0        0      350 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_runner.py
--rw-r--r--   0        0        0     5083 2024-02-29 16:46:23.292255 rapidy-0.1.1/rapidy/web_urldispatcher.py
--rw-r--r--   0        0        0     9199 1970-01-01 00:00:00.000000 rapidy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-22 08:38:32.528691 rapidy-0.2.0/LICENSE
+-rw-r--r--   0        0        0    19477 2024-05-03 20:23:55.332530 rapidy-0.2.0/README.md
+-rw-r--r--   0        0        0     5921 2024-05-03 20:54:52.580860 rapidy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7822 2024-04-30 11:15:43.280798 rapidy-0.2.0/rapidy/__init__.py
+-rw-r--r--   0        0        0    12717 2024-04-22 03:22:22.724232 rapidy-0.2.0/rapidy/_annotation_container.py
+-rw-r--r--   0        0        0     9154 2024-04-22 03:22:22.724232 rapidy-0.2.0/rapidy/_annotation_extractor.py
+-rw-r--r--   0        0        0     4382 2024-04-22 08:38:32.528691 rapidy-0.2.0/rapidy/_client_errors.py
+-rw-r--r--   0        0        0     9279 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/_extractors.py
+-rw-r--r--   0        0        0     7400 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_fields.py
+-rw-r--r--   0        0        0      627 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/_parsers.py
+-rw-r--r--   0        0        0      474 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_request_params_base.py
+-rw-r--r--   0        0        0     2565 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/_validators.py
+-rw-r--r--   0        0        0      614 2024-04-22 08:38:32.528691 rapidy-0.2.0/rapidy/_version.py
+-rw-r--r--   0        0        0      285 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/constants.py
+-rw-r--r--   0        0        0     3496 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/hdrs.py
+-rw-r--r--   0        0        0      290 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/media_types.py
+-rw-r--r--   0        0        0      169 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/_api_errors.py
+-rw-r--r--   0        0        0     4463 2024-05-01 21:05:46.329849 rapidy-0.2.0/rapidy/mypy/_type_helpers.py
+-rw-r--r--   0        0        0      146 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/_version.py
+-rw-r--r--   0        0        0     5485 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/mypy/plugin.py
+-rw-r--r--   0        0        0        7 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/py.typed
+-rw-r--r--   0        0        0    11108 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/request_params.py
+-rw-r--r--   0        0        0      218 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/streams.py
+-rw-r--r--   0        0        0     2363 2024-05-02 21:51:29.755968 rapidy-0.2.0/rapidy/typedefs.py
+-rw-r--r--   0        0        0     9009 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web.py
+-rw-r--r--   0        0        0     8310 2024-05-02 22:30:37.509688 rapidy-0.2.0/rapidy/web_app.py
+-rw-r--r--   0        0        0    12391 2024-05-02 21:51:29.755968 rapidy-0.2.0/rapidy/web_exceptions.py
+-rw-r--r--   0        0        0      140 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web_middlewares.py
+-rw-r--r--   0        0        0      130 2024-04-22 03:22:22.725232 rapidy-0.2.0/rapidy/web_request.py
+-rw-r--r--   0        0        0     2483 2024-05-02 22:30:37.510688 rapidy-0.2.0/rapidy/web_response.py
+-rw-r--r--   0        0        0     2926 2024-04-22 03:22:22.726232 rapidy-0.2.0/rapidy/web_routedef.py
+-rw-r--r--   0        0        0      350 2024-04-22 03:22:22.726232 rapidy-0.2.0/rapidy/web_runner.py
+-rw-r--r--   0        0        0     5682 2024-04-22 08:38:32.529691 rapidy-0.2.0/rapidy/web_urldispatcher.py
+-rw-r--r--   0        0        0    20927 1970-01-01 00:00:00.000000 rapidy-0.2.0/PKG-INFO
```

### Comparing `rapidy-0.1.1/pyproject.toml` & `rapidy-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "rAPIdy"
-version = "0.1.1"
+version = "0.2.0"
 description = "rAPIdy - write quickly - write beautifully"
-authors = ["Daniil Grois <daniil.grois@gmail.com>"]
+authors = [
+    "Daniil Grois <daniil.grois@gmail.com>",
+    "Lev Zaplatin <lev@zaplatin.dev>",
+]
 keywords = [
     "rAPIdy",
     "aiohttp",
     "pydantic",
     "api",
     "fast",
     "http server",
     "Daniil Grois",
+    "Lev Zaplatin",
 ]
 license = "MIT License"
 readme = "README.md"
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
@@ -34,29 +38,33 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
 ]
+packages = [
+  {include = "rapidy"},
+  {include = "rapidy/py.typed"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-aiohttp = "^3.9.3"
+aiohttp = "^3.8.1"
 pydantic = ">=1.7.4,!=1.8,!=1.8.1,!=1.8.2,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.*"
 pytest-aiohttp = "^1.0.5"
 pytest-cov = "^4.1.0"
 pytest-httpserver = "^1.0.8"
 
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.flake8]
 exclude = [
     "tests/*",
     "benchmarks/*",
@@ -71,14 +79,15 @@
     "D104",    #  Missing docstring in public package
     "D105",    #  Missing docstring in magic method
     "D107",    #  Missing docstring in __init__"
     "P101",    #  format string does contain unindexed parameters
     "S101",    #  Use of assert detected. The enclosed code will be removed when compiling to optimised byte code.
     "WPS110",  #  Found wrong variable name: X
     "WPS111",  #  Found too short name: d < X
+    "WPS113",  #  Found same alias import: X
     "WPS114",  #  Found underscored number name pattern: X_1
     "WPS115",  #  Found upper-case constant in a class: X
     "WPS201",  #  Found module with too many imports: X > 12
     "WPS202",  #  Found too many module members: X > 7
     "WPS203",  #  Found module with too many imported names: X > 50
     "WPS204",  #  Found overused expression: X; used 5 > 4
     "WPS210",  #  Found too many local variables: X > 5
@@ -93,14 +102,15 @@
     "WPS238",  #  Found too many raises in a function: X > 3
     "WPS237",  #  Found a too complex `f` string
     "WPS305",  #  Found `f` string
     "WPS306",  #  Found class without a base class: X
     "WPS318",  #  Found extra indentation
     "WPS326",  #  Found implicit string concatenation
     "WPS337",  #  Found multiline conditions
+    "WPS402",  #  Found `noqa` comments overuse: X
     "WPS410",  #  Found wrong metadata variable: __all__
     "WPS420",  #  Found wrong keyword
     "WPS421",  #  Found wrong function call: vars
     "WPS430",  #  Found nested function: X
     "WPS436",  #  Found protected module import: X
     "WPS437",  #  Found protected attribute usage: _X
     "WPS450",  #  Found protected object import: X
@@ -110,19 +120,24 @@
     "WPS510",  #  Found `in` used with a non-set container
     "WPS529",  #  Found implicit `.get()` dict usage
     "WPS600",  #  Found subclassing a builtin: X
     "WPS604",  #  Found incorrect node inside `class` body
     "W503",    #  line break before binary operator
 ]
 per-file-ignores = [
-    'rapidy/web.py: WPS232',
-    'rapidy/__init__.py: WPS412',
+    'rapidy/__init__.py: N813 WPS412 WPS413 WPS433 WPS442',
+    'rapidy/_version.py: WPS116',
+    'rapidy/web.py: F401 WPS112 WPS232 WPS433',
+    'rapidy/web_exceptions.py: D400 F401 WPS112 WPS433',
     'rapidy/fields.py: C901 WPS113 WPS433',
     'rapidy/typedefs.py: WPS433 WPS113 WPS440',
     'rapidy/_client_errors.py: C901 WPS433 WPS440',
+    'rapidy/mypy/__init__.py: WPS412',
+    'rapidy/mypy/*: WPS433',
+    'rapidy/mypy/_type_helpers.py: WPS221 WPS602',
 ]
 
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 check_untyped_defs = true
@@ -135,15 +150,15 @@
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 allow_untyped_defs = true
 allow_untyped_calls = true
 allow_subclassing_any = true
 allow_untyped_decorators = true
-disable_error_code = "var-annotated, has-type"
+disable_error_code = "var-annotated, has-type, no-redef, empty-body"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 use_parentheses = true
 line_length = 120
 order_by_type = false
```

### Comparing `rapidy-0.1.1/rapidy/_client_errors.py` & `rapidy-0.2.0/rapidy/_client_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import ABC, abstractmethod
-from types import FunctionType
 from typing import Any, Dict, List, Tuple, Type, Union
 
 from pydantic import BaseModel, create_model
 
 from rapidy.constants import PYDANTIC_V1, PYDANTIC_V2
-from rapidy.typedefs import ErrorList, ErrorWrapper
+from rapidy.typedefs import ErrorWrapper, ValidationErrorList
 
 RequestErrorModel: Type[BaseModel] = create_model('Request')
 
 
 class ClientBaseError(ABC, ValueError):
     type: str
     msg_template: str
@@ -92,15 +91,15 @@
             loc_prefix: Tuple[Union[str, int], ...],
     ) -> List[Dict[str, Any]]:
         return [
             {**err, 'loc': loc_prefix + err.get('loc', ())}
             for err in errors
         ]
 
-    def _normalize_errors(errors: List[Any]) -> ErrorList:
+    def _normalize_errors(errors: List[Any]) -> ValidationErrorList:
         for error in errors:  # TODO: FIXME
             error.pop('url', None)
             error.pop('input', None)
         return errors
 
 else:
     raise Exception
@@ -126,16 +125,19 @@
     msg_template = 'Failed to extract body data as Multipart: {multipart_error}'
 
 
 class ExtractMultipartPartError(ExtractMultipartError):
     msg_template = 'Failed to extract body data as Multipart. Failed to read part `{part_num}`: {multipart_error}'
 
 
-def _create_handler_info_msg(handler: FunctionType) -> str:
+def _create_handler_info_msg(handler: Any) -> str:
     return (
-        f'Handler path: `{handler.__code__.co_filename}`.\n'
-        f'Handler name: `{handler.__name__}`.\n'
+        f'\nHandler path: `{handler.__code__.co_filename}`'
+        f'\nHandler name: `{handler.__name__}`\n'
     )
 
 
-def _create_handler_attr_info_msg(handler: FunctionType, attr_name: str) -> str:
-    return f'{_create_handler_info_msg(handler)} Attribute name: `{attr_name}`.\n'
+def _create_handler_attr_info_msg(handler: Any, attr_name: str) -> str:
+    return (
+        f'{_create_handler_info_msg(handler)}'
+        f'Attribute name: `{attr_name}`\n'
+    )
```

### Comparing `rapidy-0.1.1/rapidy/_extractors.py` & `rapidy-0.2.0/rapidy/_extractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,41 @@
 
 from aiohttp import BodyPartReader, MultipartReader
 from aiohttp.abc import Request
 from aiohttp.streams import EmptyStreamReader, StreamReader
 from aiohttp.typedefs import JSONDecoder
 from multidict import MultiDict
 
+from rapidy import hdrs
 from rapidy._client_errors import (
     BodyDataSizeExceedError,
     ExtractJsonError,
     ExtractMultipartError,
     ExtractMultipartPartError,
 )
 from rapidy._parsers import parse_multi_params
 from rapidy.media_types import ApplicationJSON
-from rapidy.typedefs import DictStrAny
+from rapidy.typedefs import DictStrAny, DictStrListAny, DictStrListStr, DictStrStr
 
 
-async def extract_path(request: Request) -> DictStrAny:
+async def extract_path(request: Request) -> DictStrStr:
     return dict(request.match_info)
 
 
-async def extract_headers(request: Request) -> DictStrAny:
-    pairs = request.headers
-    return parse_multi_params(pairs)
+async def extract_headers(request: Request) -> DictStrStr:
+    return parse_multi_params(request.headers)  # type: ignore[return-value]
 
 
-async def extract_cookies(request: Request) -> DictStrAny:
+async def extract_cookies(request: Request) -> DictStrStr:
     cookies = request.cookies
     return dict(cookies)
 
 
-async def extract_query(request: Request) -> DictStrAny:
-    pairs = request.rel_url.query
-    return parse_multi_params(pairs)
+async def extract_query(request: Request) -> DictStrStr:
+    return parse_multi_params(request.rel_url.query)  # type: ignore[return-value]
 
 
 async def extract_body_stream(request: Request, max_size: int) -> StreamReader:
     # TODO: custom StreamReader with body_max_size
     return request.content
 
 
@@ -73,15 +72,15 @@
 
 
 async def extract_body_x_www_form(
         request: Request,
         max_size: int,
         attrs_case_sensitive: bool,
         duplicated_attrs_parse_as_array: bool,
-) -> DictStrAny:
+) -> Union[DictStrStr, DictStrListStr]:
     if not request.body_exists:
         return {}
 
     text_body = await extract_body_text(request=request, max_size=max_size)
     unquotes_text = unquote(text_body)
     key_value_arr = parse_qsl(unquotes_text)
 
@@ -99,23 +98,23 @@
         if duplicated_attrs_parse_as_array:
             # NOTE: Mandatory operation, otherwise all duplicate keys will be overwritten
             data = cast(MultiDict[str], data)
             data.add(key, value)
         else:
             data[key] = value
 
-    return parse_multi_params(data)
+    return parse_multi_params(data, parse_as_array=duplicated_attrs_parse_as_array)
 
 
 async def extract_body_multi_part(
         request: Request,
         max_size: int,
         attrs_case_sensitive: bool,
         duplicated_attrs_parse_as_array: bool,
-) -> DictStrAny:
+) -> Union[DictStrAny, DictStrListAny]:
     if not request.body_exists:
         return {}
 
     multipart_reader = await _get_multipart_reader(request)
 
     data: Union[MultiDict[Union[bytearray, str]], Dict[str, Union[bytearray, str]]]
 
@@ -142,29 +141,29 @@
             part=part,
             available_bytes_to_read=available_bytes_to_read,
             body_max_size=max_size,
         )
 
         available_bytes_to_read = updated_available_bytes_to_read
 
-        payload = _get_part_data_payload(part=part, part_data=part_data, current_part_num=part_num)
+        payload = _get_part_data_payload(part=part, part_data=part_data)
 
         if attrs_case_sensitive is False:
             part_name = part_name.lower()
 
         if duplicated_attrs_parse_as_array:
             # NOTE: Mandatory operation, otherwise all duplicate keys will be overwritten
             data = cast(MultiDict[Union[bytearray, str]], data)
             data.add(part_name, payload)
         else:
             data[part_name] = payload
 
         part_num += 1
 
-    return parse_multi_params(data)
+    return parse_multi_params(data, parse_as_array=duplicated_attrs_parse_as_array)
 
 
 async def _get_multipart_reader(request: Request) -> MultipartReader:
     try:
         reader = await request.multipart()
     except Exception as read_error:
         raise ExtractMultipartError(
@@ -201,14 +200,18 @@
 
 async def _get_next_part(
         multipart_reader: MultipartReader,
         current_part_num: int,
 ) -> Optional[Union[MultipartReader, BodyPartReader]]:
     try:
         part = await multipart_reader.next()
+    except AssertionError as assertion_err:
+        if assertion_err.args[0] == 'Reading after EOF':  # NOTE: this is aiohttp bug
+            return None
+        raise assertion_err
     except Exception as value_error:
         raise ExtractMultipartPartError(
             multipart_error=value_error.args[0],  # TODO: specific error parsing
             part_num=current_part_num,
         )
 
     return part
@@ -224,46 +227,31 @@
             multipart_error='Content-Disposition header doesnt contain `name` attr',
             part_num=current_part_num,
         )
 
     return part_name
 
 
-def _get_part_content_type(
-    part: BodyPartReader,
-    current_part_num: int,
-) -> str:
-    part_content_type = part.headers.get('content-type')
-    if part_content_type is None:
-        raise ExtractMultipartPartError(
-            multipart_error='Part missing Content-Type header',
-            part_num=current_part_num,
-        )
-
-    return part_content_type
-
-
 async def _read_part_chunk(part: BodyPartReader) -> Tuple[bytes, int]:
     if part._at_eof:  # noqa:  WPS437
         return b'', 0
 
     chunk_data = await part.read_chunk(part.chunk_size)
     chunk_len = len(chunk_data)
 
     return chunk_data, chunk_len
 
 
 def _get_part_data_payload(
     part: BodyPartReader,
     part_data: bytearray,
-    current_part_num: int,
 ) -> Union[bytearray, str]:
-    part_content_type = _get_part_content_type(part=part, current_part_num=current_part_num)
+    part_content_type = part.headers.get(hdrs.CONTENT_TYPE)
 
-    if part_content_type.startswith('text/') or part_content_type == ApplicationJSON:
+    if part_content_type and (part_content_type.startswith('text/') or part_content_type == ApplicationJSON):
         part_charset = part.get_charset(default='utf-8')
         part_decoded_data = part.decode(part_data)
         return part_decoded_data.decode(part_charset)
 
     return part_data
```

### Comparing `rapidy-0.1.1/rapidy/_parsers.py` & `rapidy-0.2.0/rapidy/_parsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing import Any, Dict, List, Union
 
 from multidict import MultiMapping
 
 
 def parse_multi_params(
-    data: Union[MultiMapping[Any], Dict[str, Any]],
+        data: Union[MultiMapping[Any], Dict[str, Any]],
+        *,
+        parse_as_array: bool = False,
 ) -> Dict[str, Union[Any, List[Any]]]:
-    parsed_result: Dict[str, Any] = {}
+    if parse_as_array:
+        parsed_result: Dict[str, list[Any]] = {}
 
-    for name, value in data.items():
-        if name in parsed_result:
-            if isinstance(parsed_result[name], list):
+        for name, value in data.items():
+            if name in parsed_result:
                 parsed_result[name].append(value)
             else:
-                parsed_result[name] = [parsed_result[name], value]
-        else:
-            parsed_result[name] = value
+                parsed_result[name] = [value]
 
-    return parsed_result
+        return parsed_result
+
+    if isinstance(data, MultiMapping):
+        return dict(data)
+
+    return data
```

### Comparing `rapidy-0.1.1/rapidy/_validators.py` & `rapidy-0.2.0/rapidy/_validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from copy import deepcopy
 from typing import Any, cast, Dict, List, Optional, Tuple
 
 from rapidy._client_errors import _regenerate_error_with_loc, RequiredFieldIsMissing
-from rapidy.fields import ModelField
+from rapidy._fields import ModelField
 from rapidy.typedefs import DictStrAny, ErrorWrapper
 
 
 def _validate_data_by_field(
         raw_data: Optional[Any],
         loc: Tuple[str, ...],
         model_field: ModelField,
         *,
         values: DictStrAny,
 ) -> Tuple[Optional[Any], List[Any]]:
     if raw_data is None:
         if model_field.required:
             return values, [RequiredFieldIsMissing().get_error_info(loc=loc)]
 
-        return deepcopy(model_field.default), []
+        return model_field.get_default(), []
 
     validated_data, validated_errors = model_field.validate(raw_data, values, loc=loc)
     if isinstance(validated_errors, ErrorWrapper):
         return values, [validated_errors]
 
     if isinstance(validated_errors, list):
         converted_errors = _regenerate_error_with_loc(errors=validated_errors, loc_prefix=())
```

### Comparing `rapidy-0.1.1/rapidy/fields.py` & `rapidy-0.2.0/rapidy/_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,64 +2,52 @@
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, TYPE_CHECKING, Union
 
 from pydantic import ValidationError
 from pydantic.fields import FieldInfo as FieldInfo
 from typing_extensions import Annotated
 
 from rapidy._client_errors import RequestErrorModel
-from rapidy._request_params_base import ValidateType
+from rapidy._request_params_base import ParamType, ValidateType
 from rapidy.constants import PYDANTIC_V1, PYDANTIC_V2
-from rapidy.request_params import ParamType
-from rapidy.typedefs import Required, Undefined, ValidateReturn
+from rapidy.typedefs import NoArgAnyCallable, Required, Undefined, ValidateReturn
 
 
-class Param:
-    def __init__(
-            self,
-            param_type: ParamType,
-            extractor: Any,
-            validate_type: ValidateType,
-            can_default: bool,
-    ) -> None:
-        self.param_type = param_type
-        self.extractor = extractor
-        self.validate_type = validate_type
-        self.can_default = can_default
+class ParamFieldInfo(FieldInfo, ABC):
+    param_type: ParamType
+    extractor: Any
+    validate_type: ValidateType
+    can_default: bool = True
 
-
-class ParamFieldInfo(FieldInfo, Param, ABC):
     def __init__(
             self,
-            param_type: ParamType,
-            extractor: Any,
-            validate_type: ValidateType,
-            can_default: bool = True,
+            default: Any = Undefined,
+            *,
+            default_factory: Optional[NoArgAnyCallable] = None,
             **field_info_kwargs: Any,
     ) -> None:
         FieldInfo.__init__(
             self,
+            default=default,
+            default_factory=default_factory,
             **field_info_kwargs,
         )
+        if PYDANTIC_V1:
+            self._validate()  # check specify both default and default_factory
 
-        Param.__init__(
-            self,
-            param_type=param_type,
-            extractor=extractor,
-            validate_type=validate_type,
-            can_default=can_default,
-        )
+        extractor = getattr(self, 'extractor') or getattr(self.__class__, 'extractor', None)  # noqa: B009
+        if not extractor:
+            raise
 
 
-if PYDANTIC_V1:
-    from pydantic import BaseConfig
-    from pydantic.class_validators import Validator as Validator
-    from pydantic.error_wrappers import ErrorWrapper
-    from pydantic.fields import ModelField as PydanticModelField
-    from pydantic.schema import get_annotation_from_field_info
-    from pydantic.typing import NoArgAnyCallable as NoArgAnyCallable  # noqa: WPS113
+if PYDANTIC_V1:  # noqa: C901
+    from pydantic import BaseConfig  # noqa: WPS433
+    from pydantic.class_validators import Validator as Validator  # noqa: WPS433
+    from pydantic.error_wrappers import ErrorWrapper  # noqa: WPS433
+    from pydantic.fields import ModelField as PydanticModelField  # noqa: WPS433
+    from pydantic.schema import get_annotation_from_field_info  # noqa: WPS433
 
     if TYPE_CHECKING:  # pragma: no cover
         from pydantic.fields import BoolUndefined
 
     class ModelField(PydanticModelField):
         def __init__(
                 self,
@@ -92,22 +80,25 @@
                 self.rapid_param_type = rapid_param_type
 
     def create_field(
             name: str,
             type_: Type[Any],
             field_info: ParamFieldInfo,
     ) -> ModelField:
+        required = field_info.default in (Required, Undefined) and field_info.default_factory is None
+
         kwargs: Dict[str, Any] = {
             'name': name,
             'field_info': field_info,
             'type_': type_,
             'rapid_param_type': field_info.param_type,
-            'required': field_info.default in (Required, Undefined),
+            'required': required,
             'alias': field_info.alias or name,
             'default': field_info.default,
+            'default_factory': field_info.default_factory,
             'class_validators': {},
             'model_config': BaseConfig,
         }
         try:
             return ModelField(**kwargs)
         except Exception:
             raise Exception(
@@ -140,17 +131,17 @@
             elif isinstance(error, list):
                 use_errors.extend(_normalize_errors(error))
             else:
                 use_errors.append(error)
         return use_errors
 
 elif PYDANTIC_V2:
-    from dataclasses import dataclass
+    from dataclasses import dataclass  # noqa: WPS433
 
-    from pydantic import TypeAdapter
+    from pydantic import TypeAdapter  # noqa: WPS433
 
     def get_annotation_from_field_info(annotation: Any, field_info: FieldInfo, field_name: str) -> Any:  # noqa: WPS440
         return annotation
 
     def _regenerate_error_with_loc(  # noqa: WPS440
             *,
             errors: Sequence[Any],
@@ -181,14 +172,17 @@
 
         @property
         def default(self) -> Any:
             if self.field_info.is_required():
                 return Undefined
             return self.field_info.get_default(call_default_factory=True)
 
+        def get_default(self) -> Any:
+            return self.field_info.get_default(call_default_factory=True)
+
         @property
         def type_(self) -> Any:
             return self.field_info.annotation
 
         def __post_init__(self) -> None:
             self._type_adapter: TypeAdapter[Any] = TypeAdapter(Annotated[self.field_info.annotation, self.field_info])
```

### Comparing `rapidy-0.1.1/rapidy/hdrs.py` & `rapidy-0.2.0/rapidy/hdrs.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.1.1/rapidy/request_params.py` & `rapidy-0.2.0/rapidy/request_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     extract_body_text,
     extract_body_x_www_form,
     extract_cookies,
     extract_headers,
     extract_path,
     extract_query,
 )
+from rapidy._fields import create_field, get_annotation_from_field_info, ModelField, ParamFieldInfo
 from rapidy._request_params_base import ParamType, ValidateType
 from rapidy.constants import MAX_BODY_SIZE
-from rapidy.fields import create_field, get_annotation_from_field_info, ModelField, ParamFieldInfo
 from rapidy.media_types import ApplicationBytes, ApplicationJSON, ApplicationXWWWForm, MultipartForm, TextPlain
+from rapidy.typedefs import NoArgAnyCallable, Required, Undefined
 
 __all__ = (
     'BytesBody',
     'Cookie',
     'CookieSchema',
     'CookieRaw',
     'FormDataBody',
@@ -46,331 +47,355 @@
     'Query',
     'QuerySchema',
     'QueryRaw',
     'StreamBody',
     'TextBody',
 )
 
-from rapidy.typedefs import Required
-
 
 class BodyParamAttrDefinitionError(Exception):
     pass
 
 
 class DefaultDefinitionError(Exception):
     pass
 
 
 class PathBase(ParamFieldInfo):
-    def __init__(self, **kwargs: Any):
-        super().__init__(**kwargs, param_type=ParamType.path, extractor=extract_path, can_default=False)
+    param_type = ParamType.path
+    extractor = staticmethod(extract_path)
+    can_default = False
 
 
 class Path(PathBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+    validate_type = ValidateType.param
 
 
 class PathSchema(PathBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class PathRaw(PathBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
 
 
 class HeaderBase(ParamFieldInfo):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, param_type=ParamType.header, extractor=extract_headers)
+    param_type = ParamType.header
+    extractor = staticmethod(extract_headers)
 
 
 class Header(HeaderBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+    validate_type = ValidateType.param
 
 
 class HeaderSchema(HeaderBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class HeaderRaw(HeaderBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class CookieBase(ParamFieldInfo):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, param_type=ParamType.cookie, extractor=extract_cookies)
+    param_type = ParamType.cookie
+    extractor = staticmethod(extract_cookies)
 
 
 class Cookie(CookieBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+    validate_type = ValidateType.param
 
 
 class CookieSchema(CookieBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class CookieRaw(CookieBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class QueryBase(ParamFieldInfo):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, param_type=ParamType.query, extractor=extract_query)
+    param_type = ParamType.query
+    extractor = staticmethod(extract_query)
 
 
 class Query(QueryBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+    validate_type = ValidateType.param
 
 
 class QuerySchema(QueryBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class QueryRaw(QueryBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class BodyBase(ParamFieldInfo, ABC):
+    param_type = ParamType.body
+    media_type: str
+
     def __init__(
             self,
-            media_type: str,
+            default: Any = Undefined,
             *,
-            extractor: Any,
+            default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
-            **kwargs: Any,
+            **field_info_kwargs: Any,
     ) -> None:
         self.body_max_size = body_max_size or MAX_BODY_SIZE
-        self.media_type = media_type
 
-        extractor = partial(extractor, max_size=self.body_max_size)
+        self.extractor = partial(self.extractor, max_size=self.body_max_size)
 
-        super().__init__(
-            **kwargs,
-            extractor=extractor,
-            param_type=ParamType.body,
-        )
+        super().__init__(default=default, default_factory=default_factory, **field_info_kwargs)
 
 
 class StreamBody(BodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(
-            **kwargs,
-            validate_type=ValidateType.no_validate,
-            extractor=extract_body_stream,
-            media_type=ApplicationBytes,
-            can_default=False,
-        )
+    media_type = ApplicationBytes
+    extractor = staticmethod(extract_body_stream)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class BytesBody(BodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(
-            **kwargs,
-            validate_type=ValidateType.no_validate,
-            extractor=extract_body_bytes,
-            media_type=ApplicationBytes,
-        )
+    media_type = ApplicationBytes
+    extractor = staticmethod(extract_body_bytes)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class TextBody(BodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(
-            **kwargs,
-            validate_type=ValidateType.no_validate,
-            extractor=extract_body_text,
-            media_type=TextPlain,
-        )
+    media_type = TextPlain
+    extractor = staticmethod(extract_body_text)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class JsonBodyBase(BodyBase):
+    media_type = ApplicationJSON
+    extractor = staticmethod(extract_body_json)
+
     def __init__(
             self,
+            default: Any = Undefined,
             *,
-            json_decoder: Optional[JSONDecoder] = None,
+            default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
-            **kwargs: Any,
+            json_decoder: Optional[JSONDecoder] = None,
+            **field_info_kwargs: Any,
     ) -> None:
-        extractor = partial(
-            extract_body_json,
+        self.extractor = partial(  # noqa: WPS601
+            self.extractor,
             json_decoder=json_decoder or DEFAULT_JSON_DECODER,
         )
 
         super().__init__(
-            **kwargs,
+            default=default,
+            default_factory=default_factory,
             body_max_size=body_max_size,
-            extractor=extractor,
-            media_type=ApplicationJSON,
+            **field_info_kwargs,
         )
 
 
 class JsonBody(JsonBodyBase):
+    validate_type = ValidateType.param
+
     def __init__(
             self,
+            default: Any = Undefined,
             *,
+            default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
             json_decoder: Optional[JSONDecoder] = None,
-            **kwargs: Any,
+            **field_info_kwargs: Any,
     ) -> None:
         if body_max_size is not None or json_decoder is not None:
             raise BodyParamAttrDefinitionError(
                 'A single JsonBody parameter does not allow to determine `body_max_size` or `json_decoder`. '
                 'Please use JsonSchema or JsonRaw.',
             )
 
         super().__init__(
-            **kwargs,
-            validate_type=ValidateType.param,
+            default=default,
+            default_factory=default_factory,
             body_max_size=body_max_size,
             json_decoder=json_decoder,
+            **field_info_kwargs,
         )
 
 
 class JsonBodySchema(JsonBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class JsonBodyRaw(JsonBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class FormDataBodyBase(BodyBase):
+    media_type = ApplicationXWWWForm
+
     def __init__(
             self,
+            default: Any = Undefined,
             *,
-            attrs_case_sensitive: Optional[bool] = None,
-            duplicated_attrs_parse_as_array: Optional[bool] = None,
-            **kwargs: Any,
+            default_factory: Optional[NoArgAnyCallable] = None,
+            body_max_size: Optional[int] = None,
+            attrs_case_sensitive: bool = False,
+            duplicated_attrs_parse_as_array: bool = False,
+            **field_info_kwargs: Any,
     ) -> None:
-        extractor = partial(
+        self.extractor = partial(
             extract_body_x_www_form,
-            attrs_case_sensitive=attrs_case_sensitive or False,
-            duplicated_attrs_parse_as_array=duplicated_attrs_parse_as_array or False,
+            attrs_case_sensitive=attrs_case_sensitive,
+            duplicated_attrs_parse_as_array=duplicated_attrs_parse_as_array,
         )
 
         super().__init__(
-            **kwargs,
-            extractor=extractor,
-            media_type=ApplicationXWWWForm,
+            default=default,
+            default_factory=default_factory,
+            body_max_size=body_max_size,
+            **field_info_kwargs,
         )
 
 
 class FormDataBody(FormDataBodyBase):
+    validate_type = ValidateType.param
+
     def __init__(
             self,
+            default: Any = Undefined,
             *,
+            default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
-            attrs_case_sensitive: Optional[bool] = None,
-            duplicated_attrs_parse_as_array: Optional[bool] = None,
-            **kwargs: Any,
+            attrs_case_sensitive: bool = False,
+            duplicated_attrs_parse_as_array: bool = False,
+            **field_info_kwargs: Any,
     ) -> None:
         if (
             body_max_size is not None
-            or attrs_case_sensitive is not None
-            or duplicated_attrs_parse_as_array is not None
+            or attrs_case_sensitive
+            or duplicated_attrs_parse_as_array
         ):
             raise BodyParamAttrDefinitionError(
                 'A single FormDataBody parameter does not allow to determine '
                 '`body_max_size` or `attrs_case_sensitive` or `duplicated_attrs_parse_as_array`. '
                 'Please use FormDataSchema or FormDataRaw.',
             )
 
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+        super().__init__(
+            default=default,
+            default_factory=default_factory,
+            body_max_size=body_max_size,
+            attrs_case_sensitive=attrs_case_sensitive,
+            duplicated_attrs_parse_as_array=duplicated_attrs_parse_as_array,
+            **field_info_kwargs,
+        )
 
 
 class FormDataBodySchema(FormDataBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class FormDataBodyRaw(FormDataBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 class MultipartBodyBase(BodyBase):
+    media_type = MultipartForm
+
     def __init__(
             self,
+            default: Any = Undefined,
+            *,
+            default_factory: Optional[NoArgAnyCallable] = None,
+            body_max_size: Optional[int] = None,
             attrs_case_sensitive: bool = False,
             duplicated_attrs_parse_as_array: bool = False,
-            **kwargs: Any,
+            **field_info_kwargs: Any,
     ) -> None:
-        extractor = partial(
+        self.extractor = partial(
             extract_body_multi_part,
             attrs_case_sensitive=attrs_case_sensitive,
             duplicated_attrs_parse_as_array=duplicated_attrs_parse_as_array,
         )
 
         super().__init__(
-            **kwargs,
-            extractor=extractor,
-            media_type=MultipartForm,
+            default=default,
+            default_factory=default_factory,
+            body_max_size=body_max_size,
+            **field_info_kwargs,
         )
 
 
 class MultipartBody(MultipartBodyBase):
+    validate_type = ValidateType.param
+
     def __init__(
             self,
+            default: Any = Undefined,
             *,
+            default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
-            attrs_case_sensitive: Optional[bool] = None,
-            duplicated_attrs_parse_as_array: Optional[bool] = None,
-            **kwargs: Any,
+            attrs_case_sensitive: bool = False,
+            duplicated_attrs_parse_as_array: bool = False,
+            **field_info_kwargs: Any,
     ) -> None:
         if (
             body_max_size is not None
-            or attrs_case_sensitive is not None
-            or duplicated_attrs_parse_as_array is not None
+            or attrs_case_sensitive
+            or duplicated_attrs_parse_as_array
         ):
             raise BodyParamAttrDefinitionError(
                 'A single MultipartBody parameter does not allow to determine '
                 '`body_max_size` or `attrs_case_sensitive` or `duplicated_attrs_parse_as_array`. '
                 'Please use MultipartBodySchema or MultipartBodyRaw.',
             )
 
-        super().__init__(**kwargs, validate_type=ValidateType.param)
+        super().__init__(
+            default=default,
+            default_factory=default_factory,
+            body_max_size=body_max_size,
+            attrs_case_sensitive=attrs_case_sensitive,
+            duplicated_attrs_parse_as_array=duplicated_attrs_parse_as_array,
+            **field_info_kwargs,
+        )
 
 
 class MultipartBodySchema(MultipartBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.schema)
+    validate_type = ValidateType.schema
 
 
 class MultipartBodyRaw(MultipartBodyBase):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__(**kwargs, validate_type=ValidateType.no_validate)
+    validate_type = ValidateType.no_validate
+    can_default = False
 
 
 def create_param_model_field_by_request_param(
         *,
         annotated_type: Any,
         field_info: ParamFieldInfo,
         param_name: str,
         param_default: Any,
+        param_default_factory: Optional[NoArgAnyCallable],
 ) -> ModelField:
     copied_field_info = copy(field_info)
 
     if param_default is not inspect.Signature.empty:
         copied_field_info.default = param_default
     else:
         copied_field_info.default = Required
 
+    if param_default_factory is not None:
+        copied_field_info.default_factory = param_default_factory
+
     inner_attribute_type = get_annotation_from_field_info(
         annotation=annotated_type,
         field_info=field_info,
         field_name=param_name,
     )
 
     return create_field(
```

### Comparing `rapidy-0.1.1/rapidy/typedefs.py` & `rapidy-0.2.0/rapidy/typedefs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, Type, TYPE_CHECKING, Union
 
-from aiohttp.abc import AbstractView
+from aiohttp.abc import AbstractView, Request
 from aiohttp.typedefs import (
     Byteish,
     DEFAULT_JSON_DECODER,
     DEFAULT_JSON_ENCODER,
-    Handler,
     JSONDecoder,
     JSONEncoder,
     LooseCookies,
     LooseCookiesIterables,
     LooseCookiesMappings,
     LooseHeaders,
-    Middleware,
     PathLike,
     RawHeaders,
     StrOrURL,
 )
 from typing_extensions import TypeAlias
 
 from rapidy.constants import PYDANTIC_V1, PYDANTIC_V2
-from rapidy.web_response import StreamResponse
+
+if TYPE_CHECKING:
+    from rapidy.web_response import StreamResponse
 
 __all__ = (
     'Byteish',
     'DEFAULT_JSON_DECODER',
     'DEFAULT_JSON_ENCODER',
     'JSONEncoder',
     'JSONDecoder',
@@ -34,29 +34,41 @@
     'LooseCookiesMappings',
     'LooseCookiesIterables',
     'LooseCookies',
     'Middleware',
     'Handler',
     'PathLike',
     'DictStrAny',
+    'DictStrStr',
+    'DictStrListAny',
+    'DictStrListStr',
     'MethodHandler',
     'HandlerType',
     'HandlerOrMethod',
 )
 
 DictStrAny = Dict[str, Any]
-MethodHandler = Callable[[], Awaitable[StreamResponse]]
-HandlerType = Union[Type[AbstractView], Handler]
+DictStrStr = Dict[str, str]
+DictStrListAny = Dict[str, List[Any]]
+DictStrListStr = Dict[str, List[str]]
+
+Handler = Callable[..., Awaitable['StreamResponse']]
+MethodHandler = Callable[..., Awaitable['StreamResponse']]
+HandlerType = Union[Handler, Type[AbstractView]]
+Middleware = Callable[[Request, Handler], Awaitable['StreamResponse']]
 
 HandlerOrMethod = Union[Handler, MethodHandler]
 
 ResultValidate: TypeAlias = Dict[str, Any]
-ErrorList: TypeAlias = List[Dict[str, Any]]
-ValidateReturn: TypeAlias = Tuple[Optional[ResultValidate], Optional[ErrorList]]
+ValidationErrorList: TypeAlias = List[Dict[str, Any]]
+ValidateReturn: TypeAlias = Tuple[Optional[ResultValidate], Optional[ValidationErrorList]]
+
+RouterDeco = Callable[[HandlerType], HandlerType]
 
+NoArgAnyCallable = Callable[[], Any]
 
 if PYDANTIC_V1:
     from pydantic.error_wrappers import ErrorWrapper as ErrorWrapper
     from pydantic.fields import (
         Required as Required,
         Undefined as Undefined,
         UndefinedType as UndefinedType,
```

### Comparing `rapidy-0.1.1/rapidy/web_app.py` & `rapidy-0.2.0/rapidy/web_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,102 @@
 import asyncio
-import json
 import logging
 import warnings
 from functools import partial, update_wrapper
-from typing import Any, cast, Dict, Iterable, List, Mapping, Optional, Union
+from typing import Any, cast, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple
 
 from aiohttp.abc import AbstractMatchInfo
-from aiohttp.helpers import AppKey
 from aiohttp.log import web_logger
-from aiohttp.web_app import (
-    _AppSignal,
-    _MiddlewaresHandlers,
-    _RespPrepareSignal,
-    _Subapps,
-    Application as AiohttpApplication,
-    CleanupContext,
-    CleanupError,
-)
-from aiohttp.web_exceptions import HTTPUnprocessableEntity
-from aiohttp.web_urldispatcher import MatchInfoError, UrlMappingMatchInfo
-from aiosignal import Signal
-from frozenlist import FrozenList
+from aiohttp.web_app import Application as AiohttpApplication, CleanupError
+from aiohttp.web_middlewares import _fix_request_current_app
+from aiohttp.web_urldispatcher import MatchInfoError
 
 from rapidy import hdrs
-from rapidy._annotation_container import AnnotationContainer, create_annotation_container
+from rapidy._annotation_container import AnnotationContainer, create_annotation_container, HandlerEnumType
 from rapidy._client_errors import _normalize_errors
 from rapidy.constants import CLIENT_MAX_SIZE
-from rapidy.media_types import ApplicationJSON
 from rapidy.typedefs import Handler, Middleware
+from rapidy.web_exceptions import HTTPValidationFailure
 from rapidy.web_request import Request
 from rapidy.web_response import StreamResponse
+from rapidy.web_urldispatcher import UrlDispatcher
 
 __all__ = (
     'Application',
     'CleanupError',
 )
 
-from rapidy.web_urldispatcher import UrlDispatcher
-
 
 class Application(AiohttpApplication):
     def __init__(
             self,
             *,
             logger: logging.Logger = web_logger,
+            router: Optional[UrlDispatcher] = None,
             middlewares: Iterable[Middleware] = (),
             handler_args: Optional[Mapping[str, Any]] = None,
-            # TODO: Add a check that in body extractors the size does not exceed the client size
             client_max_size: int = CLIENT_MAX_SIZE,
             client_errors_response_field_name: str = 'errors',
+            loop: Optional[asyncio.AbstractEventLoop] = None,
+            debug: Any = ...,
+            server_info_in_response: bool = False,
     ) -> None:
-        self._debug = ...
+        # TODO: Add a check that in body extractors the size does not exceed the client size
+
+        super().__init__(
+            logger=logger,
+            router=router,
+            middlewares=middlewares,
+            handler_args=handler_args,
+            client_max_size=client_max_size,
+            loop=loop,
+            debug=debug,
+        )
+
+        # NOTE: override aiohttp router
         self._router = UrlDispatcher()
-        self._loop = None
-        self._handler_args = handler_args
-        self.logger = logger
-
-        self._middlewares: _MiddlewaresHandlers = FrozenList(middlewares)
-        self._middleware_annotation_containers = self._create_annotation_containers_for_middleware(middlewares)
-
-        self._middlewares_handlers: _MiddlewaresHandlers = None  # initialized on freezing
-        self._run_middlewares: Optional[bool] = None  # initialized on freezing
-
-        self._state: Dict[Union[AppKey[Any], str], object] = {}
-        self._frozen = False
-        self._pre_frozen = False
-        self._subapps: _Subapps = []
-
-        self._on_response_prepare: _RespPrepareSignal = Signal(self)
-        self._on_startup: _AppSignal = Signal(self)
-        self._on_shutdown: _AppSignal = Signal(self)
-        self._on_cleanup: _AppSignal = Signal(self)
-        self._cleanup_ctx = CleanupContext()
-        self._on_startup.append(self._cleanup_ctx._on_startup)
-        self._on_cleanup.append(self._cleanup_ctx._on_cleanup)
-        self._client_max_size = client_max_size
+
         self._client_errors_response_field_name = client_errors_response_field_name
 
-    def _create_annotation_containers_for_middleware(
-            self,
-            middlewares: Iterable[Middleware],
-    ) -> Dict[int, AnnotationContainer]:
-        annotation_containers: Dict[int, AnnotationContainer] = {}
-        for middleware in middlewares:
-            if not getattr(middleware, '__middleware_version__', None):
+        self._middleware_annotation_containers: Dict[int, AnnotationContainer] = {}
+
+        # It is hidden by default, as I believe showing server information is a potential vulnerability.
+        self._server_info_in_response = server_info_in_response
+
+    @property
+    def router(self) -> UrlDispatcher:
+        return self._router
+
+    def _add_middleware_annotation_container(self, middleware: Middleware) -> None:
+        self._middleware_annotation_containers[id(middleware)] = create_annotation_container(
+            middleware,
+            handler_type=HandlerEnumType.middleware,
+        )
+
+    def _get_middleware_annotation_container(self, middleware: Middleware) -> Optional[AnnotationContainer]:
+        return self._middleware_annotation_containers.get(id(middleware))
+
+    def _prepare_middleware(self) -> Iterator[Tuple[Middleware, bool]]:  # FIXME: refactor
+        for middleware in reversed(self._middlewares):
+            if getattr(middleware, '__middleware_version__', None) == 1:
+                self._add_middleware_annotation_container(middleware)
+                yield middleware, True
+            else:
                 warnings.warn(
                     'rAPIdy does not support Old-style middleware - please use @middleware decorator.\n'
                     'If you are using middlewares with a nested middlewares wrapped by @middleware -\n'
                     'make sure that in Application(middlewares=[...]) you pass its instance.\n\n'
                     'Example:\n'
                     '>> app = Application(middlewares=[parametrized_middleware(<some_attr>=<some_value>)])',
                     DeprecationWarning,
                     stacklevel=2,
                 )
-                continue
-            annotation_containers[id(middleware)] = create_annotation_container(middleware)
-        return annotation_containers
+                yield middleware, False
 
-    def _get_middleware_annotation_container(self, middleware: Middleware) -> Optional[AnnotationContainer]:
-        return self._middleware_annotation_containers.get(id(middleware))
+        yield _fix_request_current_app(self), True
 
     async def _handle(self, request: Request) -> StreamResponse:  # noqa: C901  # FIXME: refactor
         loop = asyncio.get_event_loop()
         debug = loop.get_debug()
         match_info = await self._router.resolve(request)
         if debug:  # pragma: no cover
             if not isinstance(match_info, AbstractMatchInfo):
@@ -123,17 +117,19 @@
 
         if resp is None:
             handler = match_info.handler
 
             if isinstance(match_info, MatchInfoError):
                 return await handler(request)
 
+            annotation_container = match_info.route.get_method_container(request.method)
+
             if self._run_middlewares:
                 async def w_handler(request: Request) -> StreamResponse:  # noqa: WPS442
-                    return await self._get_handler_response(request, handler, match_info)
+                    return await self._get_handler_response(request, handler, annotation_container)
 
                 for app in match_info.apps[::-1]:
                     for middleware, new_style in app._middlewares_handlers:
                         if new_style:
                             validated_request_data_for_middleware = await self._validate_request_for_middleware(
                                 app=app, request=request, middleware=middleware,
                             )
@@ -143,31 +139,42 @@
                             )
                         else:
                             w_handler = await middleware(app, w_handler)
 
                 resp = await w_handler(request)
 
             else:
-                return await self._get_handler_response(request, handler, match_info)
+                return await self._get_handler_response(request, handler, annotation_container)
 
         return resp
 
     async def _get_handler_response(
             self,
             request: Request,
             handler: Handler,
-            match_info: UrlMappingMatchInfo,
+            annotation_container: AnnotationContainer,
     ) -> StreamResponse:
         validate_request_data_for_handler = await self._validate_request_for_handler(
-            request=request, match_info=match_info,
+            request=request,
+            annotation_container=annotation_container,
         )
-        return await handler(request, **validate_request_data_for_handler)
 
-    async def _validate_request_for_handler(self, request: Request, match_info: UrlMappingMatchInfo) -> Dict[str, Any]:
-        annotation_container = match_info.route.get_method_container(request.method)
+        if annotation_container.is_method_container:
+            return await handler(request, **validate_request_data_for_handler)
+
+        if annotation_container.request_exists:
+            validate_request_data_for_handler[annotation_container.request_param_name] = request
+
+        return await handler(**validate_request_data_for_handler)
+
+    async def _validate_request_for_handler(
+            self,
+            request: Request,
+            annotation_container: AnnotationContainer,
+    ) -> Dict[str, Any]:
         return await self._validate_request(annotation_container=annotation_container, request=request)
 
     async def _validate_request_for_middleware(
             self,
             app: 'Application',
             request: Request,
             middleware: Middleware,
@@ -190,13 +197,13 @@
             param_values, param_errors = await param_container.get_request_data(request)
             if param_errors:
                 errors += param_errors
             else:
                 values.update(cast(Dict[str, Any], param_values))
 
         if errors:
-            response_errors = {self._client_errors_response_field_name: _normalize_errors(errors)}
-            response_errors_body = json.dumps(response_errors)
-
-            raise HTTPUnprocessableEntity(content_type=ApplicationJSON, text=response_errors_body)
+            raise HTTPValidationFailure(
+                validation_failure_field_name=self._client_errors_response_field_name,
+                errors=_normalize_errors(errors),
+            )
 
         return values
```

### Comparing `rapidy-0.1.1/rapidy/web_urldispatcher.py` & `rapidy-0.2.0/rapidy/web_urldispatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from abc import ABC
 from types import FunctionType
 from typing import Any, Awaitable, Callable, cast, Optional, Type, Union
 
 from aiohttp.abc import AbstractView
-from aiohttp.typedefs import Handler
 from aiohttp.web_request import Request
 from aiohttp.web_response import StreamResponse
 from aiohttp.web_urldispatcher import (
-    _ExpectHandler,
     _requote_path,
     AbstractResource,
     AbstractRoute,
     DynamicResource as AioHTTPDynamicResource,
     PlainResource as AioHTTPPlainResource,
     PrefixedSubAppResource,
     Resource as AioHTTPResource,
@@ -20,15 +18,16 @@
     StaticResource,
     UrlDispatcher as AioHTTPUrlDispatcher,
     UrlMappingMatchInfo,
     View as AioHTTPView,
 )
 
 from rapidy import hdrs
-from rapidy._annotation_container import AnnotationContainer, create_annotation_container
+from rapidy._annotation_container import AnnotationContainer, create_annotation_container, HandlerEnumType
+from rapidy.typedefs import Handler, HandlerType, MethodHandler
 
 __all__ = [
     'UrlDispatcher',
     'UrlMappingMatchInfo',
     'AbstractResource',
     'Resource',
     'PlainResource',
@@ -37,56 +36,65 @@
     'AbstractRoute',
     'ResourceRoute',
     'StaticResource',
     'View',
 ]
 
 
+_ExpectHandler = Callable[..., Awaitable[Optional[StreamResponse]]]
+
+
 class ResourceRoute(AioHTTPResourceRoute, ABC):
     def __init__(
             self,
             method: str,
-            handler: Union[Handler, Type[AbstractView]],
+            handler: HandlerType,
             resource: AbstractResource,
             *,
             expect_handler: Optional[_ExpectHandler] = None,
     ) -> None:
         super().__init__(
             method=method,
             handler=handler,
             expect_handler=expect_handler,
             resource=resource,
         )
 
-        self.annotation_container = {}
+        self.annotation_containers = {}
 
         if isinstance(handler, FunctionType):
-            self.annotation_container[method.lower()] = create_annotation_container(handler)
+            self.annotation_containers[method.lower()] = create_annotation_container(
+                handler,
+                handler_type=HandlerEnumType.func,
+            )
 
-        elif issubclass(handler, AbstractView):
+        elif issubclass(handler, AbstractView):  # type: ignore[arg-type]
             for method in (  # noqa: WPS335 WPS352 WPS440
                 handler_attr
                 for handler_attr in dir(handler)
                 if handler_attr.upper() in hdrs.METH_ALL
             ):
-                method_handler: Optional[Callable[[], Awaitable[StreamResponse]]] = getattr(handler, method, None)
+                method_handler: Optional[MethodHandler] = getattr(handler, method, None)
                 if method_handler is None:  # NOTE: Scenario is impossible.  # pragma: no cover
                     raise
 
-                self.annotation_container[method.lower()] = create_annotation_container(method_handler)
+                self.annotation_containers[method.lower()] = create_annotation_container(
+                    method_handler,
+                    handler_type=HandlerEnumType.method,
+                )
 
     def get_method_container(self, method: str) -> AnnotationContainer:
-        return self.annotation_container[method.lower()]
+        return self.annotation_containers[method.lower()]
 
 
 class Resource(AioHTTPResource, ABC):
     def add_route(
         self,
         method: str,
-        handler: Union[Type[AbstractView], Handler],
+        handler: Handler,
         *,
         expect_handler: Optional[_ExpectHandler] = None,
     ) -> 'ResourceRoute':
 
         for route_obj in self._routes:
             if route_obj.method == method or route_obj.method == hdrs.METH_ANY:  # noqa: WPS514
                 raise RuntimeError(  # aiohttp code  # pragma: no cover
@@ -126,27 +134,39 @@
             return resource
 
         resource = DynamicResource(path, name=name)
         self.register_resource(resource)
 
         return resource
 
+    def add_route(
+        self,
+        method: str,
+        path: str,
+        handler: Union[Handler, Type[AbstractView]],
+        *,
+        name: Optional[str] = None,
+        expect_handler: Optional[_ExpectHandler] = None,
+    ) -> AbstractRoute:
+        resource = self.add_resource(path, name=name)
+        return resource.add_route(method, handler, expect_handler=expect_handler)
+
 
 class View(AioHTTPView):
     def __init__(self, request: Request, **request_validated_data: Any) -> None:
         super().__init__(request)
         self._request_validated_data = request_validated_data
 
     async def _iter(self) -> StreamResponse:
         if self.request.method not in hdrs.METH_ALL:  # aiohttp code  # pragma: no cover
             self._raise_allowed_methods()
 
-        method: Optional[Callable[[], Awaitable[StreamResponse]]]
-        method = getattr(self, self.request.method.lower(), None)
-
+        method: Optional[MethodHandler] = getattr(self, self.request.method.lower(), None)
         if method is None:  # aiohttp code  # pragma: no cover
             self._raise_allowed_methods()
 
-        ret = await method(**self._request_validated_data)  # type: ignore[misc]
+        method = cast(MethodHandler, method)
+
+        ret = await method(**self._request_validated_data)
 
         assert isinstance(ret, StreamResponse)
         return ret
```

