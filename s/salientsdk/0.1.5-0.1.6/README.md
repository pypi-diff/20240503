# Comparing `tmp/salientsdk-0.1.5.tar.gz` & `tmp/salientsdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salientsdk-0.1.5.tar", max compression
+gzip compressed data, was "salientsdk-0.1.6.tar", max compression
```

## Comparing `salientsdk-0.1.5.tar` & `salientsdk-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     3463 2024-04-22 11:58:45.166017 salientsdk-0.1.5/docs/index.md
--rw-r--r--   0        0        0     2689 2024-04-22 11:58:54.829954 salientsdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/.gitignore
--rw-r--r--   0        0        0     1858 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/__init__.py
--rw-r--r--   0        0        0    10159 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/__main__.py
--rw-r--r--   0        0        0     3297 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/constants.py
--rw-r--r--   0        0        0     6654 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/data_timeseries_api.py
--rw-r--r--   0        0        0     3642 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/downscale_api.py
--rw-r--r--   0        0        0     6925 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/forecast_timeseries_api.py
--rw-r--r--   0        0        0    12562 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/hindcast_summary_api.py
--rw-r--r--   0        0        0     5987 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/location.py
--rw-r--r--   0        0        0    11838 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/login_api.py
--rw-r--r--   0        0        0     4542 2024-04-22 11:58:45.170017 salientsdk-0.1.5/salientsdk/upload_file_api.py
--rw-r--r--   0        0        0     4523 1970-01-01 00:00:00.000000 salientsdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3611 2024-05-03 12:49:01.789628 salientsdk-0.1.6/docs/index.md
+-rw-r--r--   0        0        0     7707 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/downscale.ipynb
+-rw-r--r--   0        0        0     7990 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/hindcast_summary.ipynb
+-rw-r--r--   0        0        0    32274 2024-05-03 12:49:01.793628 salientsdk-0.1.6/examples/ski.ipynb
+-rw-r--r--   0        0        0     3006 2024-05-03 12:49:23.045599 salientsdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/.gitignore
+-rw-r--r--   0        0        0     2022 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/__init__.py
+-rw-r--r--   0        0        0    11106 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/__main__.py
+-rw-r--r--   0        0        0      335 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/cli.py
+-rw-r--r--   0        0        0     7531 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/constants.py
+-rw-r--r--   0        0        0     7493 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/data_timeseries_api.py
+-rw-r--r--   0        0        0     4619 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/downscale_api.py
+-rw-r--r--   0        0        0     6431 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/forecast_timeseries_api.py
+-rw-r--r--   0        0        0    12001 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/hindcast_summary_api.py
+-rw-r--r--   0        0        0     6548 2024-05-03 12:49:01.793628 salientsdk-0.1.6/salientsdk/location.py
+-rw-r--r--   0        0        0    11778 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/login_api.py
+-rw-r--r--   0        0        0    13515 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/snow.py
+-rw-r--r--   0        0        0     6214 2024-05-03 12:49:01.797628 salientsdk-0.1.6/salientsdk/upload_file_api.py
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 salientsdk-0.1.6/PKG-INFO
```

### Comparing `salientsdk-0.1.5/docs/index.md` & `salientsdk-0.1.6/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,25 @@
 print(xr.open_file(history))
 ```
 
 Note that this example uses the limited credentials `testusr` and `testpwd`.  To access the full capabilities of your license, use your Salient-provided credentials.
 
 See all available functions in the [API Reference](api.md).
 
+# Examples
+
+
 The [examples](https://github.com/Salient-Predictions/salientsdk/tree/main/examples) directory contains `ipynb` notebooks to help you get started with common operations. 
 
+These examples are also included within the package. You can list their file locations with:
+
+```
+python3 -m salientsdk examples
+```
+
+
 # License
 
 This SDK is licensed for use by Salient customers [details](https://salient-predictions.github.io/salientsdk/LICENSE/).
 
 
 Copyright 2024 [Salient Predictions](https://www.salientpredictions.com/)
```

### Comparing `salientsdk-0.1.5/pyproject.toml` & `salientsdk-0.1.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [tool.poetry]
 name = "salientsdk"
-version = "0.1.5"
+version = "0.1.6"
 description = "Salient Predictions Software Development Kit"
 authors = ["Salient Predictions <help@salientpredictions.com>"]
 license = "LicenseRef-Custom"
 readme = "docs/index.md"
 keywords = ["weather","climate","forecasting","sdk","salient","s2s"]
 homepage = "https://salientpredictions.com"
 # Native doc at https://salient-predictions.github.io/salientsdk/
 # Redirect to sdk via CNAME at https://domains.google.com/registrar/salientpredictions.com/dns
 # Configure custom domain at https://github.com/Salient-Predictions/salientsdk/settings/pages
 documentation = "https://sdk.salientpredictions.com"
 repository = "https://github.com/Salient-Predictions/salientsdk"
+include = ["examples/*.ipynb"]
 
 [tool.poetry.urls]
 "License" = "https://sdk.salientpredictions.com/LICENSE/"
 
+
 [tool.poetry.dependencies]
 # use "poetry add <packagename>" to edit this list
 h5netcdf = "^1.3.0"
 netCDF4 = "^1.6.5"
 pandas = "^2.2.1"
 python = "^3.11"
 requests = "^2.31.0"
 toml = "^0.10.2"
 xarray = "^2024.2.0"
 numpy = "^1.26.4"
+dask = "^2024.4.2"
 
 [tool.poetry.group.dev.dependencies]
 # use "poetry add --dev <packagename>" to edit this list
 google = "^3.0.0"
 google-cloud-secret-manager = "^2.19.0"
 markdown-include = "^0.8.1"
 mkdocs = "^1.5.3"
@@ -40,14 +43,23 @@
 mkdocstrings-python = "^1.9.0"
 nbmake = "^1.5.3"
 pydoc-markdown = "^4.8.2"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.3.4"
 
+[tool.poetry.group.examples.dependencies]
+# These dependencies are used by the examples ipynotebooks
+# poetry add <packagename> --group examples
+matplotlib = "^3.8.4"
+
+[tool.poetry.scripts]
+# This creates the 'salientsdk' command
+salientsdk = "salientsdk.cli:main"
+
 [build-system]
 # poetry build
 # -- to publish to test pypi --
 # poetry config repositories.testpypi https://test.pypi.org/legacy/
 # poetry config pypi-token.testpypi <your-test-pypi-token>
 # poetry publish -r testpypi
 # pip install --index-url https://test.pypi.org/simple/ salientsdk
```

### Comparing `salientsdk-0.1.5/salientsdk/__init__.py` & `salientsdk-0.1.6/salientsdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 
 import os
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
 import toml
 
-from .constants import get_model_version, set_model_version
+from .constants import (
+    get_file_destination,
+    get_model_version,
+    set_file_destination,
+    set_model_version,
+)
 from .data_timeseries_api import data_timeseries, load_multihistory
 from .downscale_api import downscale
 from .forecast_timeseries_api import forecast_timeseries
 from .hindcast_summary_api import hindcast_summary, transpose_hindcast_summary
 from .location import Location
 from .login_api import (
     get_current_session,
     get_verify_ssl,
     login,
     set_current_session,
     set_verify_ssl,
 )
+from .snow import calc_swe
 from .upload_file_api import upload_bounding_box, upload_file, upload_location_file
 
 
 def _get_version(pkgname):
     pyproject_path = Path(__file__).resolve().parent.parent / "pyproject.toml"
     if pyproject_path.exists():
         pyproject_content = toml.load(pyproject_path)
@@ -39,27 +45,30 @@
             return "unknown"  # Development fallback
 
 
 __version__ = _get_version("salientsdk")
 __author__ = "Salient Predictions"
 __all__ = [
     "login",
+    "calc_swe",
     "data_timeseries",
     "downscale",
     "forecast_timeseries",
     "get_current_session",
+    "set_file_destination",
     "get_model_version",
     "get_verify_ssl",
     "hindcast_summary",
     "transpose_hindcast_summary",
     "load_multihistory",
     "Location",
+    "set_current_session",
+    "get_file_destination",
     "set_model_version",
     "set_verify_ssl",
-    "set_current_session",
     "upload_file",
     "upload_bounding_box",
     "upload_location_file",
 ]
 
 if __name__ == "__main__":
     print(f"ver: {__version__} by: {__author__}")
```

### Comparing `salientsdk-0.1.5/salientsdk/__main__.py` & `salientsdk-0.1.6/salientsdk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #!/usr/bin/env python
 # Copyright Salient Predictions 2024
 
 """Command line interface for the Salient SDK."""
 
 import argparse
+import glob
+import importlib.resources as pkg_resources
 import os
+from importlib.util import find_spec
 
 import pandas as pd
 import xarray as xr
 
 from .__init__ import __version__
-from .constants import get_model_version
 from .data_timeseries_api import data_timeseries
 from .downscale_api import downscale
 from .forecast_timeseries_api import forecast_timeseries
 from .hindcast_summary_api import hindcast_summary
 from .location import Location
-from .login_api import get_api_key, get_verify_ssl, login
+from .login_api import get_verify_ssl, login
 
 
 def main() -> None:
     """Command line interface for the Salient SDK."""
     parser = _get_parser()
 
     # Convert arguments into action -------
@@ -41,21 +43,29 @@
     elif cmd == "hindcast_summary":
         file_name = hindcast_summary(**args_dict)
     elif cmd == "version":
         file_name = __version__
         args.verbose = False
     elif cmd == "login":
         file_name = args_dict["session"]
+    elif cmd == "examples":
+        file_name = "\n".join(_list_examples())
     else:
-        file_name = None
+        # print(f"Command '{cmd}' not recognized")
         parser.print_help()
+        file_name = None
 
     if file_name is None:
         pass
-    elif args.verbose and isinstance(file_name, str) and os.path.exists(file_name):
+    elif (
+        "verbose" in args
+        and args.verbose
+        and isinstance(file_name, str)
+        and os.path.exists(file_name)
+    ):
         ext = os.path.splitext(file_name)[1]
         if ext == ".nc":
             print(xr.open_dataset(file_name))
         elif ext == ".csv":
             print(pd.read_csv(file_name).head())
         else:
             print(file_name)
@@ -81,31 +91,33 @@
 
 
 def _login_from_arg(arg: dict) -> dict:
     if all(key in arg for key in ["username", "password", "apikey"]):
         arg["session"] = login(
             username=arg.pop("username"),
             password=arg.pop("password"),
-            apikey=arg.pop("apikey"),
-            verify=arg.pop("verify"),
+            apikey=arg["apikey"],  # don't pop, we need this later
+            verify=arg.pop("verify"),  # will reset momentarily
             verbose=arg["verbose"],  # don't pop, used elsewhere
         )
-        # login() may change these as a side effect
+        # login() may set this as a side effect:
         arg["verify"] = get_verify_ssl()
-        arg["apikey"] = get_api_key()
     return arg
 
 
 def _get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="salientsdk command line interface")
     subparsers = parser.add_subparsers(dest="command")
 
     # version command ---------
     version_parser = subparsers.add_parser("version", help="Print the Salient SDK version")
 
+    # examples command ---------
+    examples_parser = subparsers.add_parser("examples", help="List example notebooks")
+
     # login command ----------
     login_parser = _add_common_args(
         subparsers.add_parser("login", help="Login to the Salient API"),
         [],
         location_args=False,
         login_args=True,
         force=False,
@@ -262,24 +274,40 @@
             "--debias",
             action="store_true",
             help="Debias to observation stations (default is no debiasing)",
         )
 
     if "version" in args:
         argparser.add_argument(
-            "-ver", "--version", type=str, default=get_model_version(), help="Model version to use"
+            "-ver", "--version", type=str, default="-default", help="Model version to use"
         )
 
     if "date" in args:
         argparser.add_argument("--date", type=str, default="-today")
 
     if "region" in args:
         argparser.add_argument("--region", type=str, default=None)
 
     if "variable" in args:
         argparser.add_argument("-var", "--variable", type=str, default="temp")
 
     return argparser
 
 
+def _list_examples() -> list[str]:
+    """List example notebooks."""
+    if find_spec("salientsdk.examples") is not None:
+        # If the package is installed, use importlib.resources
+        with pkg_resources.path("salientsdk.examples", "") as examples_path:
+            notebook_dir = str(examples_path)
+    else:
+        # Fallback to a development path relative to this file
+        notebook_dir = os.path.join(os.path.dirname(__file__), "..", "examples")
+
+    notebook_dir = os.path.abspath(notebook_dir)
+
+    files = glob.glob(os.path.join(notebook_dir, "*.ipynb"))
+    return files
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `salientsdk-0.1.5/salientsdk/data_timeseries_api.py` & `salientsdk-0.1.6/salientsdk/data_timeseries_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,83 +7,98 @@
 observed data.  It also includes utility functions for operating on the returned data.
 
 Command line usage example:
 
 ```
 cd ~/salientsdk
 # this will get a single variable in a single file:
-python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 --force
+python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all --start 2020-01-01 --end 2020-12-31 --force  -u username -p password
 # this will get multiple variables in separate files:
-python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all -var temp,precip
+python -m salientsdk data_timeseries -lat 42 -lon -73 -fld all -var temp,precip -u username -p password
+# test with an apikey
+python -m salientsdk data_timeseries -lat 42 -lon -73 -fld anom --start 2020-01-01 --end 2020-12-31 --force --apikey testkey
 ```
 
 """
 
 import os
 
+import numpy as np
+import pandas as pd
 import requests
 import xarray as xr
 
-from .constants import _build_url
+from .constants import _build_urls, _expand_comma
 from .location import Location
-from .login_api import download_query, get_api_key, get_current_session, get_verify_ssl
+from .login_api import download_queries
 
 
 def data_timeseries(
+    # API inputs -------
     loc: Location,
-    variable: str = "temp",
+    variable: str | list[str] = "temp",
     field: str = "anom",
     debias: bool = False,
     start: str = "1950-01-01",
     end: str = "-today",
     format: str = "nc",
     frequency: str = "daily",
+    # non-API arguments ---
+    destination: str = "-default",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    apikey: str | None = get_api_key(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    apikey: str | None = None,
+    verify: bool | None = None,
     verbose: bool = False,
     **kwargs,
-) -> str | dict[str, str]:
+) -> str | pd.DataFrame:
     """Get a historical time series of ERA5 data.
 
     This function is a convenience wrapper to the Salient
     [API](https://api.salientpredictions.com/v2/documentation/api/#/Historical/get_data_timeseries).
 
     Args:
-        loc (Location): The location to query
-        variable (str): The variable to query, defaults to `temp`
+        loc (Location): The location to query.
+            If using a `shapefile` or `location_file`, may input a vector of file names which
+            will trigger multiple calls to `data_timeseries`.
+        variable (str | list[str]): The variable to query, defaults to `temp`
             To request multiple variables, separate them with a comma `temp,precip`
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         field (str): The field to query, defaults to "anom"
-        debias (bool): If True, debias the data to local observations.  Disabled for `shapefile` locations.  [detail](https://salientpredictions.notion.site/Debiasing-2888d5759eef4fe89a5ba3e40cd72c8f)
+        debias (bool): If True, debias the data to local observations.
+            Disabled for `shapefile` locations.
+            [detail](https://salientpredictions.notion.site/Debiasing-2888d5759eef4fe89a5ba3e40cd72c8f)
         start (str): The start date of the time series
         end (str): The end date of the time series
         format (str): The format of the response
         frequency (str): The frequency of the time series
+        destination (str): The directory to download the data to
         force (bool): If False (default), don't download the data if it already exists
-        session (requests.Session): The session object to use for the request
+        session (requests.Session): The session object to use for the request.
+            If `None` (default) uses `get_current_session()`.
         apikey (str | None): The API key to use for the request.
-            In most cases, this is not needed if a `session` is provided
-            and `get_api_key()` returns `None`.
+            In most cases, this is not needed if a `session` is provided.
         verify (bool): If True (default), verify the SSL certificate
         verbose (bool): If True (default False) print status messages
         **kwargs: Additional arguments to pass to the API
 
     Keyword Arguments:
         units (str): `SI` or `US`
 
     Returns:
-        str | dict: the file name of the downloaded data.  File names are a hash of the query parameters.
+        str | pd.DataFrame:
+            the file name of the downloaded data.  File names are a hash of the query parameters.
             When `force=False` and the file already exists, the function will return the file name
             almost instantaneously without querying the API.
-            If multiple variables are requested, returns a `dict` of `{variable:file_name}`
+            If multiple variables are requested, returns a `pd.DataFrame` with columns `file_name`
+            and additional columns documenting the vectorized input arguments such as `location_file`
+            or `variable`
     """
     assert field in [
         "anom",
         "anom_d",
         "anom_ds",
         "anom_qnt",
         "anom_s",
@@ -97,96 +112,91 @@
     assert frequency in [
         "daily",
         "weekly",
         "monthly",
         "3-monthly",
     ], f"Invalid frequency {frequency}"
 
-    # if there is a comma in variable, vectorize:
-    if isinstance(variable, str) and "," in variable:
-        variable = variable.split(",")
-
-    if isinstance(variable, list):
-        file_names = {
-            var: data_timeseries(
-                loc=loc,
-                variable=var,
-                field=field,
-                debias=debias,
-                start=start,
-                end=end,
-                format=format,
-                frequency=frequency,
-                force=force,
-                session=session,
-                verify=verify,
-                verbose=verbose,
-                apikey=apikey,
-                **kwargs,
-            )
-            for var in variable
-        }
-        if verbose:
-            print(file_names)
-        return file_names
+    variable = _expand_comma(variable)
 
     endpoint = "data_timeseries"
     args = loc.asdict(
         start=start,
         end=end,
         debias=debias,
         field=field,
         format=format,
         frequency=frequency,
         variable=variable,
         apikey=apikey,
         **kwargs,
     )
 
-    (query, file_name) = _build_url(endpoint, args)
+    queries = _build_urls(endpoint, args, destination)
 
-    download_query(
-        query=query,
-        file_name=file_name,
+    download_queries(
+        query=queries["query"].values,
+        file_name=queries["file_name"].values,
         force=force,
         session=session,
         verify=verify,
         verbose=verbose,
         format=format,
     )
 
-    return file_name
+    if len(queries) == 1:
+        return queries["file_name"].values[0]
+    else:
+        # Now that we've executed the queries, we don't need it anymore:
+        queries = queries.drop(columns="query")
+
+        # we vectorized on something other than variable, but we still need it
+        # in load_multihistory to rename the fields since we don't have short_name
+        if not "variable" in queries:
+            queries["variable"] = variable
+
+        return queries
+
+
+def _load_history_row(row: pd.DataFrame, fields: list[str] = ["vals"]) -> xr.Dataset:
+    """Load a single history file and prepare for merging with others."""
+    variable = row["variable"] if "variable" in row else "variable"
+
+    hst = xr.load_dataset(row["file_name"])
+    hst = hst[fields]
+    fields_new = [variable if field == "vals" else variable + "_" + field for field in fields]
+    hst = hst.rename({field: field_new for field, field_new in zip(fields, fields_new)})
+    for fld in fields_new:
+        hst[fld].attrs = hst.attrs
+    hst.attrs = {}
+
+    if "location_file" in row:
+        # Preserve the provenance of the source location_file
+        location_files = np.repeat(row["location_file"], len(hst.location))
+        hst = hst.assign_coords(location_file=("location", location_files))
 
+    hst.close()
 
-def load_multihistory(files: dict, fields: list[str] = ["vals"]) -> xr.Dataset:
-    """Load multiple history files and merge them into a single dataset.
+    return hst
+
+
+def load_multihistory(files: pd.DataFrame, fields: list[str] = ["vals"]) -> xr.Dataset:
+    """Load multiple .nc history files and merge them into a single dataset.
 
     Args:
-        files (dict): Dictionary of `{variable:file_name}` of the type returned by
-                      `data_timeseries` when multiple `variable`s are requested
-                      e.g. `data_timeseries(..., variable = "temp,precip")`
-        fields (list[str]): List of fields to extract from the history files
+        files (pd.DataFramme): Table of the type returned by
+            `data_timeseries` when multiple `variable`s, `location_file`s
+            or `shapefile`s are requested
+            e.g. `data_timeseries(..., variable = "temp,precip")`
+
+        fields (list[str]): List of fields to extract from the history files.
+            Useful if when calling `data_timeseries(..., field = "all")`
 
     Returns:
         xr.Dataset: The merged dataset, where each field and variable is renamed
-        to `<variable>_<field>` or simply `variable` if field = "vals".
+            to `<variable>_<field>` or simply `variable` if field = "vals".
+            This will cause the format of a multi-variable file to match the data
+            variable names of `downscale`, which natively supports multi-variable queries.
     """
-
-    def __extract_history_fields(file: str, variable: str, fields: str) -> xr.Dataset:
-        hst = xr.load_dataset(file)
-        hst = hst[fields]
-        fields_new = [variable if field == "vals" else variable + "_" + field for field in fields]
-        hst = hst.rename({field: field_new for field, field_new in zip(fields, fields_new)})
-        for fld in fields_new:
-            hst[fld].attrs = hst.attrs
-        hst.attrs = {}
-        hst.close()
-
-        return hst
-
-    # Would prefer to use xr.open_mfdataset, but we need to pass in the variable name
-    # Can convert when history files have a short_name attribute
-    # https://salientpredictions.atlassian.net/browse/RD-1184
-    hst = xr.merge(
-        [__extract_history_fields(files[variable], variable, fields) for variable in files.keys()]
-    )
+    hst = [_load_history_row(row, fields) for _, row in files.iterrows()]
+    hst = xr.merge(hst)
     return hst
```

### Comparing `salientsdk-0.1.5/salientsdk/downscale_api.py` & `salientsdk-0.1.6/salientsdk/downscale_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,75 +13,86 @@
 
 import os
 from datetime import datetime
 
 import requests
 import xarray as xr
 
-from .constants import _build_url, get_model_version
+from .constants import _build_urls
 from .location import Location
-from .login_api import download_query, get_api_key, get_current_session, get_verify_ssl
+from .login_api import download_queries
 
 REFERENCE_CLIMS = ["30_yr", "10_yr", "5_yr"]
 
 
 def downscale(
+    # API arguments -----
     loc: Location,
     variables: str = "temp,precip",
     debias: bool = False,
     date: str = "-today",
     reference_clim: str = "30_yr",
     members: int = 50,
-    version: str = get_model_version(),
+    version: str | list[str] = "-default",
+    # Non-API arguments --------
+    destination: str = "-default",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    apikey: str | None = get_api_key(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    apikey: str | None = None,
+    verify: bool | None = None,
     verbose: bool = False,
     **kwargs,
 ) -> str | list[str]:
     """Temporal downscale of forecasts.
 
     Convert temporally coarse probabilistic forecasts into granular daily ensembles.
     For more detail, see the
     [api doc](https://api.salientpredictions.com/v2/documentation/api/#/Forecasts/downscale).
 
     Args:
-        loc (Location): The location to query
+        loc (Location): The location to query.
+            If using a `shapefile` or `location_file`, may input a vector of file names which
+            will trigger multiple calls to `downscale`.  This is useful because `downscale` requires
+            that all points in a file be from the same continent.
         variables (str): The variables to query, separated by commas
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available variables.
+            Note that `downscale` natively supports a list of variables, so passing a list of
+            variables here will not necessarily trigger downloading multiple files.
         date (str): The start date of the time series.
+            If `date` is `-today`, use the current date.
         reference_clim (str): Reference period to calculate anomalies.
         members (int): The number of ensemble members to download
         debias (bool): If True, debias the data
         version (str): The model version of the Salient `blend` forecast.
+        destination (str): The destination directory for downloaded files.
         force (bool): If False (default), don't download the data if it already exists
         session (requests.Session): The session object to use for the request
         apikey (str | None): The API key to use for the request.
-            In most cases, this is not needed if a `session` is provided
-            and `get_api_key()` returns `None`.
+            In most cases, this is not needed if a `session` is provided.
         verify (bool): If True (default), verify the SSL certificate
         verbose (bool): If True (default False) print status messages
         **kwargs: Additional arguments to pass to the API
 
     Keyword Arguments:
         gdd_base (int): The base temperature for growing degree days
         units (str): US or SI
 
     Returns:
-        str: the name of the downloaded (or cached) downscale data file
+        str | pd.DataFrame : If only one file was downloaded, return the name of the file.
+            If multiple files were downloaded, return a table with column `file_name` and
+            additional columns documenting the vectorized input arguments such as
+            `location_file`.
     """
     format = "nc"
     frequency = "daily"
     model = "blend"
 
     assert members > 0, "members must be a positive integer"
-    assert isinstance(session, requests.Session), "Must login to the Salient API first"
 
     if date == "-today":
         date = datetime.today().strftime("%Y-%m-%d")
 
     assert reference_clim in REFERENCE_CLIMS, f"reference_clim must be one of {REFERENCE_CLIMS}"
 
     endpoint = "downscale"
@@ -95,20 +106,26 @@
         model=model,
         version=version,
         frequency=frequency,
         apikey=apikey,
         **kwargs,
     )
 
-    (query, file_name) = _build_url(endpoint, args)
+    queries = _build_urls(endpoint, args, destination)
 
-    download_query(
-        query=query,
-        file_name=file_name,
+    download_queries(
+        query=queries["query"].values,
+        file_name=queries["file_name"].values,
         force=force,
         session=session,
         verify=verify,
         verbose=verbose,
         format=format,
+        max_workers=5,  # downscale @limiter.limit("5 per second")
     )
 
-    return file_name
+    if len(queries) == 1:
+        return queries["file_name"].values[0]
+    else:
+        # Now that we've executed the queries, we don't need it anymore:
+        queries = queries.drop(columns="query")
+        return queries
```

### Comparing `salientsdk-0.1.5/salientsdk/forecast_timeseries_api.py` & `salientsdk-0.1.6/salientsdk/forecast_timeseries_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,52 +17,57 @@
 ```
 
 """
 
 import os
 from datetime import datetime
 
+import pandas as pd
 import requests
 import xarray as xr
 
 from . import login_api
-from .constants import _build_url, get_model_version
+from .constants import _build_urls, _expand_comma
 from .location import Location
-from .login_api import get_api_key, get_current_session, get_verify_ssl
+from .login_api import download_queries
+
+FORECAST_VARIABLES = ["temp", "precip", "wspd", "tsi", "cdd", "hdd"]
 
 
 def forecast_timeseries(
+    # API inputs -------
     loc: Location,
     date: str = "-today",
     debias: bool = False,
     field: str = "anom",
     format: str = "nc",
     model: str = "blend",
     reference_clim: str = "30_yr",
     timescale="all",
     variable: str = "temp",
-    version: str = get_model_version(),
+    version: str | list[str] = "-default",
+    # non-API arguments ---
+    destination: str = "-default",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    apikey: str | None = get_api_key(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    apikey: str | None = None,
+    verify: bool | None = None,
     verbose: bool = False,
     **kwargs,
-) -> str | dict[str, str]:
+) -> str | pd.DataFrame:
     """Get time series of S2S meteorological forecasts.
 
     This function is a convenience wrapper to the Salient
     [API](https://api.salientpredictions.com/v2/documentation/api/#/Forecasts/forecast_timeseries).
 
     Args:
         loc (Location): The location to query
         date (str): The date the forecast was generated.  Defaults to `-today`, which will find the
             most recent forecast.  Can also be a specific date in the format `YYYY-MM-DD`.
         debias (bool): If True, debias the data to local observations.
-            Disabled for `shapefile` locations.
             [detail](https://salientpredictions.notion.site/Debiasing-2888d5759eef4fe89a5ba3e40cd72c8f)
         field (str): The field to query, defaults to `anom` which is an anomaly value from climatology.
             Also available: `vals`, which will return absolute values without regard to climatology.
         format (str): The file format of the response.
             Defaults to `nc` which returns a multivariate NetCDF file.
             Also available: `csv` which returns a CSV file.
         model (str): The model to query.  Defaults to `blend`, which is the Salient blended forecast.
@@ -74,78 +79,55 @@
                 a data variable `anom_weekly` or `vals_weekly`.
             - `seasonal` is 1-3 months.  Will return a coordinate `forecast_date_monthly` and a
                 data variable `anom_monthly` or `vals_monthly`.
             - `long-range` is 1-4 quarters.  Will return a coordinate `forecast_date_quarterly` and a
                 data variable `anom_quarterly` or `vals_quarterly`.
             - `all` (default) will include `sub-seasonal`, `seasonal`, and `long-range` timescales
         variable (str): The variable to query, defaults to `temp`
-            To request multiple variables, separate them with a comma `temp,precip`
+            To request multiple variables, separate them with a comma `temp,precip` or use a `list`.
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         version (str): The model version of the Salient `blend` forecast.
+        destination (str): The destination directory for downloaded files.
         force (bool): If False (default), don't download the data if it already exists
         session (requests.Session): The session object to use for the request
         apikey (str | None): The API key to use for the request.
-            In most cases, this is not needed if a `session` is provided
-            and `get_api_key()` returns `None`.
-        verify (bool): If True (default), verify the SSL certificate
+            In most cases, this is not needed if a `session` is provided.
+        verify (bool): If True (default), verify the SSL certificate.
+            Defaults to use the value returned by `get_verify_ssl()`
         verbose (bool): If True (default False) print status messages
         **kwargs: Additional arguments to pass to the API
 
     Keyword Arguments:
         units (str): `SI` or `US`
 
     Returns:
-        str | dict: the file name of the downloaded data.
+        str | pd.DataFrame: the file name(s) of the downloaded data.
             File names are a hash of the query parameters.
             When `force=False` and the file already exists, the function will return the file name
             almost instantaneously without querying the API.
-            If multiple variables are requested, returns a `dict` of `{variable:file_name}`
+            If multiple variables are requested, returns a `DataFrame` with column `file_name`
+            and an additional column for `variable`.
     """
     assert field in [
         "anom",
         "vals",
         "vals_ens",
     ], f"Invalid field {field}"
     assert format in ["nc", "csv"], f"Invalid format {format}"
 
+    # https://salientpredictions.atlassian.net/browse/RD-1437
+    assert loc.shapefile is None, "Shapefile not supported for forecast_timeseries"
+
     if date == "-today":
         date = datetime.today().strftime("%Y-%m-%d")
 
-    # if there is a comma in variable, vectorize:
-    if isinstance(variable, str) and "," in variable:
-        variable = variable.split(",")
-
-    if isinstance(variable, list):
-        file_names = {
-            var: forecast_timeseries(
-                loc=loc,
-                date=date,
-                debias=debias,
-                field=field,
-                format=format,
-                model=model,
-                reference_clim=reference_clim,
-                timescale=timescale,
-                variable=var,
-                version=version,
-                force=force,
-                session=session,
-                verify=verify,
-                verbose=verbose,
-                apikey=apikey,
-                **kwargs,
-            )
-            for var in variable
-        }
-        if verbose:
-            print(file_names)
-        return file_names
+    variable = _expand_comma(variable, FORECAST_VARIABLES, "variable")
 
     endpoint = "forecast_timeseries"
     args = loc.asdict(
         date=date,
         debias=debias,
         field=field,
         format=format,
@@ -153,24 +135,24 @@
         reference_clim=reference_clim,
         timescale=timescale,
         variable=variable,
         version=version,
         apikey=apikey,
         **kwargs,
     )
+    queries = _build_urls(endpoint, args, destination)
 
-    (query, file_name) = _build_url(endpoint, args)
-
-    if force or not os.path.exists(file_name):
-        if verbose:
-            print(f"Downloading {query} to {file_name}")
-        with open(file_name, "wb" if format == "nc" else "w") as f:
-            result = session.get(query, verify=verify)
-            result.raise_for_status()
-            if format == "nc":
-                f.write(result.content)
-            else:
-                f.write(result.text)
-    elif verbose:
-        print(f"File {file_name} already exists")
+    download_queries(
+        query=queries["query"].values,
+        file_name=queries["file_name"].values,
+        force=force,
+        session=session,
+        verify=verify,
+        verbose=verbose,
+        format=format,
+    )
 
-    return file_name
+    if len(queries) == 1:
+        return queries["file_name"].values[0]
+    else:
+        queries = queries.drop(columns="query")  # not needed anymore
+        return queries
```

### Comparing `salientsdk-0.1.5/salientsdk/hindcast_summary_api.py` & `salientsdk-0.1.6/salientsdk/hindcast_summary_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,44 +27,42 @@
 
 import numpy as np
 import pandas as pd
 import requests
 import xarray as xr
 
 from . import login_api
-from .constants import _build_urls, get_model_version
+from .constants import _build_url, _build_urls, _expand_comma
 from .location import Location
-from .login_api import (
-    download_queries,
-    get_api_key,
-    get_current_session,
-    get_verify_ssl,
-)
+from .login_api import download_queries
 
 REFERENCE_VALUES = ["-auto", "ai", "clim", "gfs", "ecmwf", "blend", "norm_5yr", "norm_10yr"]
 METRIC_VALUES = ["rps", "mae", "crps", "rps_skill_score", "mae_skill_score", "crps_skill_score"]
 SEASON_VALUES = ["all", "DJF", "MAM", "JJA", "SON"]
 
 COL_FILE = "file_name"
 ENDPOINT = "hindcast_summary"
 
 
 def hindcast_summary(
+    # API inputs -------
     loc: Location,
     metric: str = "crps",
     reference: str = "-auto",
     season: str | list[str] = "all",
     split_set: str = "all",
     timescale="all",
     variable: str | list[str] = "temp",
-    version: str | list[str] = get_model_version(),
+    version: str | list[str] = "-default",
+    # non-API arguments ---
+    destination: str = "-default",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    apikey: str | None = get_api_key(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    apikey: str | None = None,
+    verify: bool | None = None,
     verbose: bool = False,
     **kwargs,
 ) -> str:
     """Get summary of accuracy metrics.
 
     This function is a convenience wrapper to the Salient
     [API](https://api.salientpredictions.com/v2/documentation/api/#/Validation/hindcast_summary).
@@ -90,20 +88,20 @@
             To request multiple variables, separate them with a comma `temp,precip` or use a list.
             This will download one file per variable
             See the
             [Data Fields](https://salientpredictions.notion.site/Variables-d88463032846402e80c9c0972412fe60)
             documentation for a full list of available historical variables.
         version (str | list[str]): The model version of the Salient `blend` forecast.
             To compare multiple versions, provide a list or comma-separated string.
+        destination (str): The destination directory for downloaded files.
         force (bool): If False (default), don't download the data if it already exists
         session (requests.Session): The `Session` object to use for the request.
             Defaults to use get_current_session(), typically set during `login()`.
         apikey (str | None): The API key to use for the request.
-            In most cases, this is not needed if a `session` is provided
-            and `get_api_key()` returns `None`.
+            In most cases, this is not needed if a `session` is provided.
         verify (bool): Verify the SSL certificate.
             Defaults to use get_verify_ssl(), typically set during `login()`.
         verbose (bool): If True (default False) print status messages.
         **kwargs: Additional arguments to pass to the API
 
     Keyword Arguments:
         units (str): `SI` or `US`
@@ -140,35 +138,37 @@
         version=version,
         format=format,
         model=model,
         apikey=apikey,
         **kwargs,
     )
 
-    queries = _build_urls(ENDPOINT, args)
+    queries = _build_urls(ENDPOINT, args, destination)
 
     download_queries(
         query=queries["query"].values,
         file_name=queries[COL_FILE].values,
         force=force,
         session=session,
         verify=verify,
         verbose=verbose,
         format=format,
     )
 
-    file_name = _concatenate_hindcast_summary(queries, format)
+    file_name = _concatenate_hindcast_summary(queries, format, destination)
 
     if verbose:
         print(f"Saving combined table to {file_name}")
 
     return file_name
 
 
-def _concatenate_hindcast_summary(queries: pd.DataFrame, format: str) -> str:
+def _concatenate_hindcast_summary(
+    queries: pd.DataFrame, format: str = "csv", destination: str = "-default"
+) -> str:
     file_names = queries[COL_FILE].values
     if len(file_names) == 1:
         # Most of the time, we'll only have downloaded a single file.
         # No need to concatenate.
         return file_names[0]
 
     scores = pd.concat(
@@ -176,70 +176,47 @@
             pd.read_csv(row[COL_FILE]).assign(
                 **{col: row[col] for col in queries.columns if col not in ["query", COL_FILE]}
             )
             for index, row in queries.iterrows()
         ],
         ignore_index=True,
     )
-
-    # Now let's generate a filename for the combined table
-    hash = hashlib.md5(str(file_names).encode()).hexdigest()
-    file_name = f"{ENDPOINT}_{hash}.{format}"
+    # We don't care abut the url here - just calling it to get a consistent filename
+    [url, file_name] = _build_url(
+        endpoint=ENDPOINT,
+        args={"concatenate_file_names": str(file_names), "format": format},
+        destination=destination,
+    )
 
     scores.to_csv(file_name, index=False)
 
     return file_name
 
 
-def _expand_comma(
-    val: str | list[str], valid: list[str] | None = None, name="value"
-) -> list[str] | str:
-    """Expand a comma-separated string into a list of strings.
-
-    Args:
-        val (str | list[str]): A single string that may contain commas.
-            If a list of strings, convert to a single string if length == 1
-        valid (list[str] | None): A list of valid values for the string.
-            If None (default) no validation is performed.
-            If provided, asserts
-        name (str): The name of the value to use in error messages.
-
-    Returns:
-        list[str] | str: A list of strings if commas are present,
-            otherwise the original string or list of strings.
-    """
-    if isinstance(val, str) and "," in val:
-        val = val.split(",")
-
-    # Check to see if val is a list of strings
-    if isinstance(val, list):
-        if len(val) == 1:
-            val = val[0]
-
-    if valid:
-        if isinstance(val, list):
-            for v in val:
-                assert v in valid, f"{name} {v} not in {valid}"
-        else:
-            assert val in valid, f"{name} {val} not in {valid}"
-
-    return val
-
-
-def transpose_hindcast_summary(scores: str | pd.DataFrame, min_score: float = 0.0) -> pd.DataFrame:
+def transpose_hindcast_summary(
+    scores: str | pd.DataFrame,
+    min_score: float = 0.0,
+    weight_weeks=1.0,
+    weight_months=0.5,
+    weight_quarters=0.25,
+) -> pd.DataFrame:
     """Transpose hindcast_summary long to wide, preserving groups.
 
     Transposes the hindcast summary data from a long format to a wide format
-    where each 'Lead' row becomes a column.
+    where each 'Lead' row becomes a column.  Adds a column `mean` with a
+    weighted average of the scores.
 
     Parameters:
         scores (str | pd.DataFrame): The hindcast scores data.
             This can be either a file path as a string or a pre-loaded DataFrame
             of the type returned by `hindcast_summary()`
         min_score (float): Render any scores below this threshold as NA
+        weight_weeks (float): Weight for weeks 3-5, defaults to 1.0
+        weight_months (float): Weight for months 2-3, defaults to 0.5
+        weight_quarters (float): Weight for quarters 2-4, defaults to 0.25
 
     Returns:
         pd.DataFrame: The transposed DataFrame with 'Lead' categories as columns.
     """
     if isinstance(scores, str):
         scores = pd.read_csv(scores)
 
@@ -255,15 +232,15 @@
     if isinstance(extract_col, int):
         extract_col = scores.columns[extract_col]
 
     scores.set_index(index_cols, inplace=True)
     scores = scores[[extract_col]]
 
     # Adds new rows with Lead="mean"
-    scores = _add_mean(scores)
+    scores = _add_mean(scores, weight_weeks, weight_months, weight_quarters)
 
     if len(index_cols) == 1:
         # If there is no vector expansion we don't need an unstack.
         # A simple transpose will do.
         scores = scores.T
     else:
         # Preserve the order of the original table rows
```

### Comparing `salientsdk-0.1.5/salientsdk/location.py` & `salientsdk-0.1.6/salientsdk/location.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,39 +23,56 @@
     defined in a shapefile.
     """
 
     def __init__(
         self,
         lat: float | None = None,
         lon: float | None = None,
-        location_file: str | None = None,
-        shapefile: str | None = None,
-        region: str | None = None,
+        location_file: str | list[str] | None = None,
+        shapefile: str | list[str] | None = None,
+        region: str | list[str] | None = None,
     ):
         """Initialize a Location object.
 
         Only one of the following 4 options should be used at a time: lat/lon,
         location_file, shapefile, or region.
 
         Args:
             lat (float): Latitude in degrees, -90 to 90.
             lon (float): Longitude in degrees, -180 to 180.
-            location_file (str): Path to a CSV file with latitude and longitude columns.
-            shapefile (str): Path to a shapefile with a polygon defining the location.
-            region (str): Accepts continents, countries, or U.S. states (e.g. "usa")
+            location_file (str | list[str]): Path(s) to CSV file(s) with latitude and longitude columns.
+            shapefile (str | list[str]): Path(s) to a shapefile(s) with a polygon defining the location.
+            region (str | list[str]): Accepts continents, countries, or U.S. states (e.g. "usa")
                 Only available for `hindcast_summary()`
         """
         self.lat = lat
         self.lon = lon
-        self.location_file = location_file
-        self.shapefile = shapefile
+        self.location_file = self._expand_user_files(location_file)
+        self.shapefile = self._expand_user_files(shapefile)
         self.region = region
 
         self.__validate()
 
+    @staticmethod
+    def _expand_user_files(files: str | list[str] | None) -> str | list[str] | None:
+        files = constants._expand_comma(files)
+
+        # When referencing user files, the user may specify them with
+        # a directory name because that's how functions like upload_*
+        # create them.  But the API doesn't have a directory structure and
+        # only uses the file name.  So we need to strip off the directory.
+        if files is None:
+            pass
+        elif isinstance(files, str):
+            files = os.path.basename(files)
+        elif isinstance(files, list):
+            files = [os.path.basename(f) for f in files]
+
+        return files
+
     def asdict(self, **kwargs) -> dict:
         """Render as a dictionary.
 
         Generates a dictionary representation that can be encoded into a URL.
         Will contain one and only one location_file, shapefile, or lat/lon pair.
 
         Args:
@@ -68,28 +85,30 @@
             dct = {"shapefile": self.shapefile, **kwargs}
         elif self.region:
             dct = {"region": self.region, **kwargs}
         else:
             dct = {"lat": self.lat, "lon": self.lon, **kwargs}
 
         if "apikey" in dct and dct["apikey"] is not None:
-            assert isinstance(dct["apikey"], str), f"API key {dct['apikey']} must be a string"
-            assert len(dct["apikey"]) > 0, f"API key must not be empty"
+            dct["apikey"] = login_api._get_api_key(dct["apikey"])
 
         if "start" in dct:
             dct["start"] = constants._validate_date(dct["start"])
         if "end" in dct:
             dct["end"] = constants._validate_date(dct["end"])
         if "forecast_date" in dct:
             dct["forecast_date"] = constants._validate_date(dct["forecast_date"])
 
         if "version" in dct:
-            assert (
-                dct["version"] in constants.MODEL_VERSIONS
-            ), f"Version {dct['version']} not in {constants.MODEL_VERSIONS}"
+            dct["version"] = constants._expand_comma(
+                val=dct["version"],
+                valid=constants.MODEL_VERSIONS,
+                name="version",
+                default=constants.get_model_version(),
+            )
 
         if "shapefile" in dct and "debias" in dct and dct["debias"]:
             raise ValueError("Cannot debias with shapefile locations")
 
         return dct
 
     def asargs(self, **kwargs) -> str:
@@ -98,23 +117,19 @@
         Encodes a dictionary of the type returned by `asdict` into a
         single string appropriate for an API request.
         """
         return urllib.parse.urlencode(self.asdict(**kwargs), safe=",")
 
     def __validate(self):
         if self.location_file:
-            assert os.path.exists(
-                self.location_file
-            ), f"Location file {self.location_file} does not exist"
             assert not self.lat, "Cannot specify both lat and location_file"
             assert not self.lon, "Cannot specify both lon and location_file"
             assert not self.region, "Cannot specify both region and location_file"
             assert not self.shapefile, "Cannot specify both shape_file and location_file"
         elif self.shapefile:
-            assert os.path.exists(self.shapefile), f"Shape file {self.shapefile} does not exist"
             assert not self.region, "Cannot specify both region and shapefile"
             assert not self.lat, "Cannot specify both lat and shape_file"
             assert not self.lon, "Cannot specify both lon and shape_file"
         elif self.region:
             assert not self.lat, "Cannot specify both lat and region"
             assert not self.lon, "Cannot specify both lon and region"
             assert not self.location_file, "Cannot specify both location_file and region"
```

### Comparing `salientsdk-0.1.5/salientsdk/login_api.py` & `salientsdk-0.1.6/salientsdk/login_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,81 +26,56 @@
     from google.cloud import secretmanager
 except ImportError as ie:
     # secretmanager is a convenience for internal Salient users.
     # Not needed for customer use.
     pass
 
 
-VERFY_SSL = True
+VERIFY_SSL = True
 
 CURRENT_SESSION = None
 
-API_KEY = None
 
+def _get_api_key(apikey: str | None = None) -> str | None:
+    """Regularize API key values."""
+    if apikey is None:
+        return apikey
 
-def get_api_key() -> str | None:
-    """Get the current API key.
+    apikey = str(apikey)
+    assert len(apikey) > 0, f"API key must not be empty"
 
-    All calls to the Salient API have an `api_key` argument
-    that defaults to call this function. In most cases, users
-    will never need to call it explicitly.
-
-    Returns:
-        str: The current API key, or `None` if one is not set.
-
-    """
-    return API_KEY
-
-
-def set_api_key(apikey: str | None) -> str | None:
-    """Set the current API key.
-
-    Sets the default value to be used when calling
-    `apikey = get_api_key()`.
-
-    Args:
-        apikey (str | None): The API key that will be returned by `get_api_key()`.
-            Special value `testkey` will use a universal key with limited permissions.
-            Value `None` will clear the stored API key.
-
-    Returns:
-        str | None: The API key that was set
-    """
     if apikey == "apikey":
         apikey_path = "projects/forecast-161702/secrets/API_TEST_USER_KEY/versions/1"
         try:
             apikey = (
                 secretmanager.SecretManagerServiceClient()
                 .access_secret_version(request={"name": apikey_path})
                 .payload.data.decode("UTF-8")
             )
         except Exception as e:
             raise ValueError("Supply your Salient api key")
-
     elif apikey == "testkey":
         # https://api.salientpredictions.com/accounts/testing
         apikey = "950d43ac7571d8a8"
 
-    global API_KEY
-    API_KEY = apikey
-
     return apikey
 
 
-def get_current_session() -> None | requests.Session:
+def get_current_session() -> requests.Session:
     """Get the current session.
 
     All calls to the Salient API have a `session` argument
-    that defaults to call this function. In most cases, users
-    will never need to call it explicitly since it will be
-    set during `login()`.
+    that defaults to `None`.  If session is not passed to the
+    function, the api call will use the output of this function.
+
 
     Returns:
-        requests.Session: The current session, or a temporary
-            one for use with `apikey`.
+        requests.Session: The current session if one was set via
+            `login()` or `set_current_session()`, or a temporary
+            session for use with `apikey`.
     """
     return requests.Session() if CURRENT_SESSION is None else CURRENT_SESSION
 
 
 def set_current_session(session: requests.Session | None) -> None:
     """Set the current session.
 
@@ -116,46 +91,63 @@
     """
     assert session is None or isinstance(session, requests.Session)
 
     global CURRENT_SESSION
     CURRENT_SESSION = session
 
 
-def get_verify_ssl() -> bool:
+def get_verify_ssl(verify: bool | None = None) -> bool:
     """Get the current SSL verification setting.
 
     All functions that call the Salient API have a
     `verify` argument that controls whether or not to use
     SSL verification when making the call.  That argument
     will default to use this function, so in most cases
     users will never need to call it.
 
+    Args:
+        verify (bool | None): If `None` (default), returns the
+            SSL verification setting that was set
+            by `set_verify_ssl()` as a side effect of `login()`.
+            If `True` or `False`, passes through without checking
+            the default value.
+
     Returns:
         bool: The current SSL verification setting
 
     """
-    return VERFY_SSL
+    if verify is None:
+        verify = VERIFY_SSL
+        if verify is None:
+            verify = True
 
+    verify = bool(verify)
 
-def set_verify_ssl(verify: bool) -> None:
+    return verify
+
+
+def set_verify_ssl(verify: bool = True) -> bool:
     """Set the SSL verification setting.
 
     Sets the default value to be used when calling
-    `verify = get_verify_ssl()` in most API calls.
+    `get_verify_ssl(None)`.
     This is usually set automatically as a side
     effect of `login(..., verify=None)` so in most
     cases users will never need to call it.
 
     Args:
         verify (bool): The SSL verification setting
            that will be returned by `get_verify_ssl()`.
 
+    Returns:
+        bool: The SSL verification setting that was set
     """
-    global VERFY_SSL
-    VERFY_SSL = verify
+    global VERIFY_SSL
+    VERIFY_SSL = bool(verify)
+    return VERIFY_SSL
 
 
 def login(
     username: str = "username",
     password: str = "password",
     apikey: str | None = None,
     verify: bool | None = None,
@@ -169,31 +161,28 @@
     can use to execute API calls.
 
     Args:
         username (str): The username to login with
         password (str): The password to login with
         apikey (str | None): The API key to use instead of a login.
             If `None` (default) uses `username` and `password` to create a `Session`.
-            If specified, sets the default key to use with `set_api_key()`, ignores
-            `username` and `password`, does not create a `Session`.
+            If specified bypasses `login` and ignores `username` / `password`
         verify (bool): Whether to verify the SSL certificate.
             If `None` (default) will try `True` and then `False`, remembering the
             last successful setting and preserving it for future calls in `get_verify_ssl()`.
         verbose (bool): Whether to print the response status
 
     Returns:
         Session | None: Session object to pass to other API calls.
             As a side effect, will also set the default session for
             use with `get_current_session()`
-            Returns `None` if called with `apikey`
     """
     if apikey is not None:
-        set_api_key(apikey)
         set_current_session(None)  # clear out existing session, if there is one
-        session = get_current_session()  # temporary
+        session = get_current_session()  # temporary session
         if verbose:
             print(f"Using API key {apikey} with a temporary Session {session}.")
         return session
 
     if username == "username" and password == "password":
         password_path = "projects/forecast-161702/secrets/API_TEST_USER_PWD/versions/1"
         try:
@@ -227,28 +216,27 @@
     login_ok = session.get(url, auth=auth, verify=verify)
     login_ok.raise_for_status()
 
     if verbose:
         print(login_ok.text)
 
     set_current_session(session)
-    # Now that we have successfully created a session, make sure we don't preempt it:
-    set_api_key(None)
 
     return session
 
 
 def download_queries(
     query: list[str],
     file_name: list[str],
     format: str = "-auto",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    verify: bool | None = None,
     verbose: bool = False,
+    max_workers: int | None = None,
 ) -> None:
     """Downloads multiple queries saves them to a file.
 
     This function handles the downloading of data based on the provided query URLs.
     It saves the data to the specified file names.
     If the file already exists and `force` is not set to True, the download is skipped.
     Download will happen in parallel.
@@ -257,35 +245,39 @@
         query (list[str]): The URLs from which to download the data.
         file_name (list[str]): The paths where the data will be saved.
         format (str, optional): The format of the file.
             Defaults to '-auto', which will infer the format from the file extension.
         force (bool, optional): If True, the file will be downloaded even if it already exists.
             Defaults to False.
         session (requests.Session, optional): The session to use for the download.
-            Defaults to the current session via `get_current_session()`.
+            If `None` (default) uses `get_current_session()`.
         verify (bool, optional): Whether to verify the server's TLS certificate.
             Defaults to the current verification setting via `get_verify_ssl()`.
         verbose (bool, optional): If True, prints additional output about the download process.
             Defaults to False.
+        max_workers (int, optional): The maximum number of threads to use for downloading.
 
 
     Raises:
         requests.HTTPError: If the server returns an error status code.
     """
     assert len(query) == len(file_name)
 
     if len(query) == 0:
         return None
     elif len(query) == 1:
         # Much of the time we won't have vectorized queries.  Keep it simple.
         download_query(query[0], file_name[0], format, force, session, verify, verbose)
         return None
 
-    # max_workers defaults to os.cpu_count() * 5
-    with ThreadPoolExecutor() as executor:
+    if max_workers is None:
+        # This is the default value for ThreadPoolExecutor
+        max_workers = os.cpu_count() * 5
+
+    with ThreadPoolExecutor(max_workers=max_workers) as executor:
         futures = [
             executor.submit(download_query, qry, fil, format, force, session, verify, verbose)
             for qry, fil in zip(query, file_name)
         ]
         for future in futures:
             future.result()  # raises exceptions
 
@@ -293,49 +285,53 @@
 
 
 def download_query(
     query: str,
     file_name: str,
     format: str = "-auto",
     force: bool = False,
-    session: requests.Session = get_current_session(),
-    verify: bool = get_verify_ssl(),
+    session: requests.Session | None = None,
+    verify: bool = None,
     verbose: bool = False,
 ) -> [requests.Response | None]:
     """Downloads the query result and saves it to a file.
 
     This function handles the downloading of data based on the provided query URL.
     It saves the data to the specified file name.
     If the file already exists and `force` is not set to True, the download is skipped.
 
     Parameters:
         query (str): The URL from which to download the data.
         file_name (str): The path where the data will be saved.
         format (str, optional): The format of the file.
             Defaults to '-auto', which will infer the format from the file extension.
-        force (bool, optional): If True, the file will be downloaded even if it already exists.
-            Defaults to False.
+        force (bool, optional): If False (default) skips downloading `file_name` if it already exists.
         session (requests.Session, optional): The session to use for the download.
-            Defaults to the current session via `get_current_session()`.
+            If `None` (default) uses `get_current_session()`.
         verify (bool, optional): Whether to verify the server's TLS certificate.
-            Defaults to the current verification setting via `get_verify_ssl()`.
+            If `None` (default) uses the current verification setting via `get_verify_ssl()`.
         verbose (bool, optional): If True, prints additional output about the download process.
             Defaults to False.
 
     Returns:
         requests.Response | None: The response object from the server after attempting the download,
             or None if the file was already cached and not re-downloaded.
 
     Raises:
         requests.HTTPError: If the server returns an error status code.
     """
     if format == "-auto":
         # extract the file extension from the file name
         format = file_name.split(".")[-1]
 
+    if session is None:
+        session = get_current_session()
+
+    verify = get_verify_ssl(verify)
+
     result = None
     if force or not os.path.exists(file_name):
         if verbose:
             print(f"Downloading\n  {query}\n to {file_name}\n with {session}")
         result = session.get(query, verify=verify)
         result.raise_for_status()
         with open(file_name, "wb" if format == "nc" else "w") as f:
```

### Comparing `salientsdk-0.1.5/PKG-INFO` & `salientsdk-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: salientsdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Salient Predictions Software Development Kit
 Home-page: https://salientpredictions.com
 License: LicenseRef-Custom
 Keywords: weather,climate,forecasting,sdk,salient,s2s
 Author: Salient Predictions
 Author-email: help@salientpredictions.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dask (>=2024.4.2,<2025.0.0)
 Requires-Dist: h5netcdf (>=1.3.0,<2.0.0)
 Requires-Dist: netCDF4 (>=1.6.5,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: xarray (>=2024.2.0,<2025.0.0)
@@ -120,16 +121,26 @@
 print(xr.open_file(history))
 ```
 
 Note that this example uses the limited credentials `testusr` and `testpwd`.  To access the full capabilities of your license, use your Salient-provided credentials.
 
 See all available functions in the [API Reference](api.md).
 
+# Examples
+
+
 The [examples](https://github.com/Salient-Predictions/salientsdk/tree/main/examples) directory contains `ipynb` notebooks to help you get started with common operations. 
 
+These examples are also included within the package. You can list their file locations with:
+
+```
+python3 -m salientsdk examples
+```
+
+
 # License
 
 This SDK is licensed for use by Salient customers [details](https://salient-predictions.github.io/salientsdk/LICENSE/).
 
 
 Copyright 2024 [Salient Predictions](https://www.salientpredictions.com/)
```

