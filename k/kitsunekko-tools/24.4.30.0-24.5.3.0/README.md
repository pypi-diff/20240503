# Comparing `tmp/kitsunekko_tools-24.4.30.0.tar.gz` & `tmp/kitsunekko_tools-24.5.3.0.tar.gz`

## Comparing `kitsunekko_tools-24.4.30.0.tar` & `kitsunekko_tools-24.5.3.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/format.sh
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.github/workflows/black.yml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/__init__.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/__main__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/__version__.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/common.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/config.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/consts.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/ignore.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/kitsu_download.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/kitsu_parse.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/kitsu_types.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/kitsunekko_tools/mega_upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/tests/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/tests/test_parser.py
--rw-r--r--   0        0        0   663796 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/tests/data/main_dir_page.html
--rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/tests/data/subs_page.html
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/LICENSE
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/pyproject.toml
--rw-r--r--   0        0        0    42071 2020-02-02 00:00:00.000000 kitsunekko_tools-24.4.30.0/PKG-INFO
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/format.sh
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__main__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/__version__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/common.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/config.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/consts.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/file_downloader.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/ignore.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/mega_upload.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/__init__.py
+-rw-r--r--   0        0        0     8859 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/download.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/file_entry.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/rate_limit.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/api_access/root_directory.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/__init__.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/download.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/parse.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/types.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/test_directory.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/test_parser.py
+-rw-r--r--   0        0        0  1070007 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/entries_search_anime_response.json
+-rw-r--r--   0        0        0   444457 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/entries_search_dramas_response.json
+-rw-r--r--   0        0        0   663796 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/main_dir_page.html
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/tests/data/subs_page.html
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/LICENSE
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/pyproject.toml
+-rw-r--r--   0        0        0    42329 2020-02-02 00:00:00.000000 kitsunekko_tools-24.5.3.0/PKG-INFO
```

### Comparing `kitsunekko_tools-24.4.30.0/.github/ISSUE_TEMPLATE/config.yml` & `kitsunekko_tools-24.5.3.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.4.30.0/.github/workflows/ci-cd.yml` & `kitsunekko_tools-24.5.3.0/.github/workflows/ci-cd.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 name: Publish Python distribution to PyPI
 
-on: push
+on:
+  push:
+    tags:
+      - "v*"
 
 jobs:
   # step 1
   build:
     name: Build distribution
     runs-on: ubuntu-latest
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/__main__.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
 import sys
 
 import fire
 
 from kitsunekko_tools.__version__ import __version__
+from kitsunekko_tools.api_access.download import ApiSyncClient
 from kitsunekko_tools.common import KitsuException
-from kitsunekko_tools.config import ConfigFileNotFoundError, Config
+from kitsunekko_tools.config import ConfigFileNotFoundError, Config, KitsuConfig
 from kitsunekko_tools.consts import PROG_NAME
-from kitsunekko_tools.ignore import IgnoreList, IgnoreListException
-from kitsunekko_tools.kitsu_download import Sync
+from kitsunekko_tools.ignore import IgnoreList
 from kitsunekko_tools.mega_upload import mega_upload
+from kitsunekko_tools.scrapper.download import KitsuScrapper
 
 
 class ConfigCli:
     """
     Manage config.
     """
 
@@ -59,99 +60,94 @@
 
 
 class IgnoreCli:
     """
     Manage the list of ignore patterns.
     """
 
-    def __init__(self, ignore_list: IgnoreList):
-        self._ignore_list = ignore_list
+    _config: Config
+
+    def __init__(self, config: Config):
+        self._config = config
+
+    def _get_list(self) -> IgnoreList:
+        return IgnoreList(self._config.data())
 
     def locate(self) -> None:
         """
         Print path to the ignore file.
         """
-        print(self._ignore_list.ignore_filepath)
+        print(self._get_list().ignore_filepath)
 
     def show(self) -> None:
         """
         Print the list of ignore rules as Unix shell-style wildcards.
         """
-        print("\n".join(self._ignore_list.patterns()))
+        print("\n".join(self._get_list().patterns()))
 
     def add(self, pattern: str) -> None:
         """
         Add a new ignore rule.
         """
         if pattern:
-            self._ignore_list.add(str(pattern))
-            self._ignore_list.commit()
-            print(f"File written: {self._ignore_list.path()}")
+            ignore_list = self._get_list()
+            ignore_list.add(str(pattern))
+            ignore_list.commit()
+            print(f"File written: {ignore_list.path()}")
         else:
             print("Nothing to add.")
 
 
+def get_client(api: bool, config: KitsuConfig, full_sync: bool) -> ApiSyncClient | KitsuScrapper:
+    return (ApiSyncClient if api else KitsuScrapper)(config=config, full_sync=full_sync)
+
+
 class Application:
     """
     A set of scripts for creating a local kitsunekko mirror.
 
     :param version: Print version and exit.
     :param config_path: Alternative path to the config file.
     """
 
     def __init__(self, version: bool = False, config_path: str | None = None):
         self._config = Config(config_path)
+        self.config = ConfigCli(self._config)
+        self.ignore = IgnoreCli(self._config)
         if version:
             # handle ktools --version
             sys.exit(self.version())
 
     @staticmethod
     def version() -> None:
         """
         Print version and exit.
         """
         print(f"{PROG_NAME} version: {__version__}")
 
-    def config(self) -> ConfigCli:
-        """
-        Manage config.
-        """
-        try:
-            return ConfigCli(self._config)
-        except IgnoreListException as ex:
-            print(ex.what)
-
     def destination(self) -> None:
         """
         Print path to destination directory.
         """
         try:
             data = self._config.data()
         except ConfigFileNotFoundError as ex:
             print(ex.what)
         else:
             print(data.destination)
 
-    def ignore(self) -> IgnoreCli:
-        """
-        Manage the list of ignore patterns.
-        """
-        try:
-            return IgnoreCli(IgnoreList(self._config.data()))
-        except IgnoreListException as ex:
-            print(ex.what)
-
-    async def sync(self, full: bool = False) -> None:
+    async def sync(self, full: bool = False, api: bool = False) -> None:
         """
         Download everything from Kitsunekko to a local folder.
 
         :param full: Do a full sync. Ignore the 'skip_older' setting.
+        :param api: Use the API to access the contents.
         """
         try:
-            s = Sync(config=self._config.data(), full_sync=full)
+            s = get_client(api=api, config=self._config.data(), full_sync=full)
         except KitsuException as ex:
             print(ex.what)
         else:
             await s.sync_all()
 
     def upload(self):
         """
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/config.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import functools
 import io
 import os.path
 import pathlib
 import tomllib
 import typing
-
+import os
 from kitsunekko_tools.common import KitsuException
 from kitsunekko_tools.consts import *
 
 DEFAULT_HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:108.0) Gecko/20100101 Firefox/108.0",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
     "Accept-Charset": "ISO-8859-1,utf-8;q=0.7,*;q=0.3",
@@ -41,33 +41,37 @@
     with io.StringIO() as si:
         si.write("Couldn't find config file. ")
         si.write("Create the file in one of the following locations:\n")
         si.write("\n".join(f"・ {location}" for location in config_locations()))
         return si.getvalue()
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ConfigFileNotFoundError(KitsuException, FileNotFoundError):
     what: str = default_config_not_found_description()
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class DestDirNotFoundError(KitsuException):
     what: str
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class ConfigFileInvalidError(KitsuException, ValueError):
     what: str
 
 
 def as_toml_str(d: dict[str, str | int | dict]) -> str:
     with io.StringIO() as si:
         for key, value in d.items():
             match value:
+                case None:
+                    si.write(f'{key} = ""\n')
+                case frozenset():
+                    si.write(f"{key} = {list(value)}\n")
                 case str() | pathlib.Path():
                     si.write(f'{key} = "{value}"\n')
                 case int():
                     si.write(f"{key} = {value}\n")
                 case datetime.timedelta():
                     value = str(value).split(",")[0]
                     si.write(f'{key} = "{value}"\n')
@@ -75,53 +79,79 @@
                     si.write(f"[{key}]\n")
                     si.write(as_toml_str(value))
                 case _:
                     raise RuntimeError(f"Unknown value type {type(value)}")
         return si.getvalue()
 
 
-@dataclasses.dataclass
+class ApiHeaders(typing.TypedDict):
+    Authorization: str
+
+
+def convert_time_delta(skip_older: str | datetime.timedelta) -> datetime.timedelta:
+    if isinstance(skip_older, datetime.timedelta):
+        return skip_older
+    assert isinstance(skip_older, str), "Parameter 'skip_older' is expected to be a string."
+    period, time_unit = skip_older.split()
+    return datetime.timedelta(**{time_unit: int(period)})
+
+
+@dataclasses.dataclass(frozen=True)
 class KitsuConfig:
-    destination: str = "/mnt/archive/japanese/kitsunekko-mirror"
-    proxy: str = "socks5://127.0.0.1:9050"
+    destination: pathlib.Path = pathlib.Path.home() / "kitsunekko"
+    proxy: str | None = "socks5://127.0.0.1:9050"
     download_root: str = "https://kitsunekko.net/dirlist.php?dir=subtitles/japanese/"
     timeout: int = 120
-    skip_older: str = "30 days"
+    skip_older: datetime.timedelta = datetime.timedelta(days=30)  # 30 days
+    api_url: str = ""  # URL of a subtitle server's API. Normally looks like 'https://example.com/api'.
+    api_key: str = ""  # API key of the subtitle server
+    allowed_file_types: frozenset[str] = dataclasses.field(
+        default_factory=lambda: frozenset(["ssa", "ass", "srt", "zip", "rar", "7z"])
+    )
     headers: dict[str, str] = dataclasses.field(default_factory=lambda: DEFAULT_HEADERS.copy())
 
-    def __post_init__(self) -> None:
-        if "dirlist.php?dir=" not in self.download_root:
+    @classmethod
+    def from_file(cls, file: typing.BinaryIO) -> typing.Self:
+        instance = cls(**tomllib.load(file))
+        if "dirlist.php?dir=" not in instance.download_root:
             raise ConfigFileInvalidError("Download root doesn't appear to be a valid kitsunekko URL.")
-        self.destination: pathlib.Path = pathlib.Path(self.destination).expanduser()
-        self.skip_older: datetime.timedelta = self._convert_time_delta()
-        self.proxy: str | None = self.proxy or None  # coerce proxy to null if it's empty
-
-    def _convert_time_delta(self) -> datetime.timedelta:
-        assert isinstance(self.skip_older, str), "Parameter 'skip_older' is expected to be a string."
-        period, time_unit = self.skip_older.split()
-        return datetime.timedelta(**{time_unit: int(period)})
+        return dataclasses.replace(
+            instance,
+            destination=pathlib.Path(instance.destination).expanduser(),
+            skip_older=convert_time_delta(instance.skip_older),
+            proxy=instance.proxy or None,  # coerce proxy to null if it's empty
+            allowed_file_types=frozenset(instance.allowed_file_types),
+            api_key=os.getenv("KITSU_API_KEY", instance.api_key),
+            api_url=os.getenv("KITSU_API_URL", instance.api_url),
+        )
 
     def raise_for_destination(self) -> None:
         if not self.destination.is_dir():
             raise DestDirNotFoundError(f"Destination directory does not exist: {self.destination}")
 
     def as_toml_str(self) -> str:
         return as_toml_str(dataclasses.asdict(self))
 
+    def api_headers(self) -> ApiHeaders:
+        return {"Authorization": self.api_key}
+
+    def is_allowed_file_type(self, file_path: pathlib.Path) -> bool:
+        return any(file_path.name.endswith(f".{ext}") for ext in self.allowed_file_types)
+
 
 class ReadConfigResult(typing.NamedTuple):
     data: KitsuConfig
     file_path: pathlib.Path
 
 
 @functools.cache
 def read_config_file(config_file_path: pathlib.Path) -> ReadConfigResult:
     try:
         with open(config_file_path, "rb") as f:
-            return ReadConfigResult(KitsuConfig(**tomllib.load(f)), pathlib.Path(config_file_path))
+            return ReadConfigResult(KitsuConfig.from_file(f), pathlib.Path(config_file_path))
     except FileNotFoundError as ex:
         raise ConfigFileNotFoundError() from ex
 
 
 @functools.cache
 def get_config(config_file_path: pathlib.Path | str | None = None) -> ReadConfigResult:
     if config_file_path:
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/ignore.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/ignore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
 
 import dataclasses
-import fnmatch
 import pathlib
 import typing
 
 from kitsunekko_tools.common import KitsuException
-from kitsunekko_tools.config import KitsuConfig, get_config
-from kitsunekko_tools.consts import *
+from kitsunekko_tools.config import KitsuConfig
+from kitsunekko_tools.consts import IGNORE_FILENAME
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class IgnoreListException(KitsuException):
     what: str
 
 
 class IgnoreList:
     """
     Holds a list of files that should not be downloaded even if they're not present in expected locations.
@@ -44,19 +43,15 @@
     def ignore_filepath(self) -> pathlib.Path:
         return self._ignore_filepath
 
     def _pattern_from_path(self, file_path: pathlib.Path) -> str:
         return str(file_path.relative_to(self._config.destination))
 
     def is_matching(self, file_path: pathlib.Path) -> bool:
-        path_dest_stripped = self._pattern_from_path(file_path)
-        if path_dest_stripped in self._patterns:
-            # try without wildcards first.
-            return True
-        return any(fnmatch.fnmatch(path_dest_stripped, pattern) for pattern in self._patterns)
+        return self._pattern_from_path(file_path) in self._patterns
 
     def patterns(self) -> typing.Iterable[str]:
         """
         Return all known ignore patterns.
         """
         return self._patterns.keys()
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/kitsu_parse.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 import pathlib
 import re
 import typing
 import urllib.parse
 
 from kitsunekko_tools.consts import KITSUNEKKO_DOMAIN_URL
-from kitsunekko_tools.kitsu_types import AnimeDir, SubtitleFile
+from kitsunekko_tools.scrapper.types import AnimeDir, SubtitleFile
 
 MOD_TIMESTAMP_FORMAT = "%b %d %Y %I:%M:%S %p"  # timestamp format used on kitsunekko
 
 
 def datetime_from_str(mod_timestamp: str) -> datetime.datetime:
     return datetime.datetime.strptime(mod_timestamp, MOD_TIMESTAMP_FORMAT)
 
@@ -26,15 +26,15 @@
     r'<a href="/?(?P<abs_path>dirlist.php\?dir=[^"\']+)"[^<>]*>\s*<strong>\s*(?P<show_name>.+?)\s*</strong>\s*</a>.*<td class="tdright" title="(?P<mod_timestamp>[^<>"]+)"\s*>',
     flags=RE_FLAGS,
 )
 
 # <tr><td><a href="subtitles/japanese/Henjin no Salad Bowl/Henjin no Salad Bowl - 01 「麒麟がくる(異世界から)」 (TBS 1920x1080 x264 AAC).srt" class=""><strong>Henjin no Salad Bowl - 01 「麒麟がくる(異世界から)」 (TBS 1920x1080 x264 AAC).srt</strong> </a></td> <td class="tdleft"  title="29823"  > 29&nbsp;KB </td> <td class="tdright" title="Apr 05 2024 05:45:25 AM" > 3&nbsp;weeks </td></tr>
 # <tr><td><a href="subtitles/japanese/Henjin no Salad Bowl/Henjin no Salad Bowl - 02 「ホームレス女騎士／はじめてのおしごと他」 (TBS 1920x1080 x264 AAC).srt" class=""><strong>Henjin no Salad Bowl - 02 「ホームレス女騎士／はじめてのおしごと他」 (TBS 1920x1080 x264 AAC).srt</strong> </a></td> <td class="tdleft"  title="31494"  > 31&nbsp;KB </td> <td class="tdright" title="Apr 12 2024 01:28:54 PM" > 2&nbsp;weeks </td></tr>
 RE_SUBTITLE_FILE = re.compile(
-    r'<a href="/?(?P<abs_path>subtitles/[^"\']+\.(?:zip|rar|7z|ass|srt))"[^<>]*>.*<td class="tdright" title="(?P<mod_timestamp>[^<>"]+)"\s*>',
+    r'<a href="/?(?P<abs_path>subtitles/[^"\']+\.(?:zip|rar|7z|ass|srt|ssa))"[^<>]*>.*<td class="tdright" title="(?P<mod_timestamp>[^<>"]+)"\s*>',
     flags=RE_FLAGS,
 )
 
 
 def sanitize_title(title: str) -> str:
     return urllib.parse.unquote(title).strip()
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/kitsu_types.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/scrapper/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # Copyright: Ajatt-Tools and contributors; https://github.com/Ajatt-Tools
 # License: GNU AGPL, version 3 or later; http://www.gnu.org/licenses/agpl.html
-
 import datetime
 import typing
 
 
+class CompareError(ValueError):
+    def __init__(self, obj1, obj2):
+        super().__init__(f"Can't compare type {type(obj1).__name__} to type {type(obj2).__name__}")
+
+
 class AnimeDir(typing.NamedTuple):
     url: str  # full URL to the directory with subtitle files
     show_name: str  # name of the anime
     mod_timestamp: datetime.datetime  # last modified
 
-    def __eq__(self, other: typing.Self) -> bool:
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, AnimeDir):
+            raise CompareError(self, other)
         return self.show_name == other.show_name
 
-    def __ne__(self, other: typing.Self) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return hash(self.show_name)
 
 
 class SubtitleFile(typing.NamedTuple):
     url: str  # full URL to the subtitle file
     show_name: str  # anime title
     file_name: str  # name of the subtitle file
     mod_timestamp: datetime.datetime  # last modified
 
-    def __eq__(self, other: typing.Self) -> bool:
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, SubtitleFile):
+            raise CompareError(self, other)
         return self.show_name == other.show_name and self.file_name == other.file_name
 
-    def __ne__(self, other: typing.Self) -> bool:
+    def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return hash(f"{self.show_name}/{self.file_name}")
```

### Comparing `kitsunekko_tools-24.4.30.0/kitsunekko_tools/mega_upload.py` & `kitsunekko_tools-24.5.3.0/kitsunekko_tools/mega_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 
 from kitsunekko_tools.common import KitsuException
 from kitsunekko_tools.config import KitsuConfig
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class MegaError(KitsuException, RuntimeError):
     what: str
 
 
 def raise_for_status(out: subprocess.CompletedProcess):
     if out.returncode != 0:
         raise MegaError(f"Command failed with code {out.returncode}")
```

### Comparing `kitsunekko_tools-24.4.30.0/tests/test_parser.py` & `kitsunekko_tools-24.5.3.0/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import pathlib
 from collections.abc import Sequence
 
 import pytest
 
 from kitsunekko_tools.consts import KITSUNEKKO_DOMAIN_URL
-from kitsunekko_tools.kitsu_parse import AnimeDir, SubtitleFile, find_all_subtitle_dirs, find_all_subtitle_files
+from kitsunekko_tools.scrapper.parse import AnimeDir, SubtitleFile, find_all_subtitle_dirs, find_all_subtitle_files
 
 DATA_DIR = pathlib.Path(__file__).parent.joinpath("data")
 EXPECTED_DIRS = [
     AnimeDir(
         f"{KITSUNEKKO_DOMAIN_URL}/dirlist.php?dir=subtitles%2Fjapanese%2FYuru+Camp+S3%2F",
         "Yuru Camp S3",
         datetime.datetime(2024, 4, 25, 19, 38, 39),
```

### Comparing `kitsunekko_tools-24.4.30.0/tests/data/main_dir_page.html` & `kitsunekko_tools-24.5.3.0/tests/data/main_dir_page.html`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.4.30.0/tests/data/subs_page.html` & `kitsunekko_tools-24.5.3.0/tests/data/subs_page.html`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.4.30.0/LICENSE` & `kitsunekko_tools-24.5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.4.30.0/README.md` & `kitsunekko_tools-24.5.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -31,14 +31,18 @@
    Set to `""` (empty string) if you don't use proxies.
    By default, it is set to the default Tor address.
 
 Everything else usually doesn't need to be changed.
 
 ## Usage
 
+> [!TIP]
+> Clone [kitsunekko-mirror](https://github.com/Ajatt-Tools/kitsunekko-mirror)
+> before downloading from kitsunekko directly.
+
 The first time, run full sync.
 It will download everything.
 
 ``` bash
 ktools sync --full
 ```
 
@@ -58,17 +62,22 @@
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
 
 ## Ignoring certain files
 
 To prevent some files from being downloaded (because they are too big, broken, etc.),
 Create a file named `.kitsuignore` in the root of `destination`
-and fill it with Unix shell-style wildcards, one per line.
+and fill it with paths relative to `destination`.
 
 ## Help
 
 Run `ktools --help` to print a help page. 
 
+## Environment variables
+
+* `KITSU_API_KEY` - overwrite api_key in the config.
+* `KITSU_API_URL` - overwrite api_url in the config.
+
 ## Kitsunekko mirror
 
 [kitsunekko-mirror](https://github.com/Ajatt-Tools/kitsunekko-mirror)
 is a git repository with Japanese anime subtitles.
```

### Comparing `kitsunekko_tools-24.4.30.0/pyproject.toml` & `kitsunekko_tools-24.5.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kitsunekko_tools-24.4.30.0/PKG-INFO` & `kitsunekko_tools-24.5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kitsunekko-tools
-Version: 24.4.30.0
+Version: 24.5.3.0
 Summary: A set of scripts for creating a local kitsunekko mirror.
 Author-email: Ren Tatsumoto <tatsu@autistici.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,18 @@
    Set to `""` (empty string) if you don't use proxies.
    By default, it is set to the default Tor address.
 
 Everything else usually doesn't need to be changed.
 
 ## Usage
 
+> [!TIP]
+> Clone [kitsunekko-mirror](https://github.com/Ajatt-Tools/kitsunekko-mirror)
+> before downloading from kitsunekko directly.
+
 The first time, run full sync.
 It will download everything.
 
 ``` bash
 ktools sync --full
 ```
 
@@ -730,17 +734,22 @@
 2) Create `~/.megarc` and [specify](https://megatools.megous.com/man/megarc.html) your credentials.
 3) Run `ktools upload`.
 
 ## Ignoring certain files
 
 To prevent some files from being downloaded (because they are too big, broken, etc.),
 Create a file named `.kitsuignore` in the root of `destination`
-and fill it with Unix shell-style wildcards, one per line.
+and fill it with paths relative to `destination`.
 
 ## Help
 
 Run `ktools --help` to print a help page. 
 
+## Environment variables
+
+* `KITSU_API_KEY` - overwrite api_key in the config.
+* `KITSU_API_URL` - overwrite api_url in the config.
+
 ## Kitsunekko mirror
 
 [kitsunekko-mirror](https://github.com/Ajatt-Tools/kitsunekko-mirror)
 is a git repository with Japanese anime subtitles.
```

