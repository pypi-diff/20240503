# Comparing `tmp/osmnx-1.9.3.tar.gz` & `tmp/osmnx-2.0.0b0.tar.gz`

## Comparing `osmnx-1.9.3.tar` & `osmnx-2.0.0b0.tar`

### file list

```diff
@@ -1,34 +1,29 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/__init__.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_api.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_downloader.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_errors.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_nominatim.py
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_overpass.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_version.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/bearing.py
--rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/convert.py
--rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/distance.py
--rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/elevation.py
--rw-r--r--   0        0        0    43058 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/features.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/folium.py
--rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/geocoder.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/geometries.py
--rw-r--r--   0        0        0    31809 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/graph.py
--rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/io.py
--rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/osm_xml.py
--rw-r--r--   0        0        0    33374 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/plot.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/projection.py
--rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/routing.py
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/settings.py
--rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/simplification.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/speed.py
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/stats.py
--rw-r--r--   0        0        0     8199 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/truncate.py
--rw-r--r--   0        0        0    11072 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils.py
--rw-r--r--   0        0        0    15817 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils_geo.py
--rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils_graph.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.9.3/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.9.3/LICENSE.txt
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 osmnx-1.9.3/README.md
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 osmnx-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 osmnx-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_errors.py
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_http.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_nominatim.py
+-rw-r--r--   0        0        0    15714 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_osm_xml.py
+-rw-r--r--   0        0        0    17690 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_overpass.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/_version.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/bearing.py
+-rw-r--r--   0        0        0    17525 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/convert.py
+-rw-r--r--   0        0        0    16202 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/distance.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/elevation.py
+-rw-r--r--   0        0        0    27487 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/features.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/geocoder.py
+-rw-r--r--   0        0        0    30258 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/graph.py
+-rw-r--r--   0        0        0    15209 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/io.py
+-rw-r--r--   0        0        0    33597 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/plot.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/projection.py
+-rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/routing.py
+-rw-r--r--   0        0        0     8214 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/settings.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/simplification.py
+-rw-r--r--   0        0        0    13492 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/stats.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/truncate.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/utils.py
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/osmnx/utils_geo.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/LICENSE.txt
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/README.md
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 osmnx-2.0.0b0/PKG-INFO
```

### Comparing `osmnx-1.9.3/osmnx/_downloader.py` & `osmnx-2.0.0b0/osmnx/_http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,239 @@
 """Handle HTTP requests to web APIs."""
 
+from __future__ import annotations
+
 import json
 import logging as lg
 import socket
 from hashlib import sha1
 from pathlib import Path
+from typing import Any
 from urllib.parse import urlparse
-from warnings import warn
 
 import requests
 from requests.exceptions import JSONDecodeError
 
 from . import settings
 from . import utils
 from ._errors import InsufficientResponseError
 from ._errors import ResponseStatusCodeError
 
 # capture getaddrinfo function to use original later after mutating it
 _original_getaddrinfo = socket.getaddrinfo
 
 
-def _save_to_cache(url, response_json, ok):
+def _save_to_cache(
+    url: str,
+    response_json: dict[str, Any] | list[dict[str, Any]],
+    ok: bool,  # noqa: FBT001
+) -> None:
     """
     Save a HTTP response JSON object to a file in the cache folder.
 
-    Function calculates the checksum of url to generate the cache file's name.
-    If the request was sent to server via POST instead of GET, then URL should
-    be a GET-style representation of request. Response is only saved to a
-    cache file if settings.use_cache is True, response_json is not None, and
-    ok is True.
+    This calculates the checksum of `url` to generate the cache file name. If
+    the request was sent to server via POST instead of GET, then `url` should
+    be a GET-style representation of the request. Response is only saved to a
+    cache file if `settings.use_cache` is True, `response_json` is not None,
+    and `ok` is True.
 
     Users should always pass OrderedDicts instead of dicts of parameters into
     request functions, so the parameters remain in the same order each time,
     producing the same URL string, and thus the same hash. Otherwise the cache
     will eventually contain multiple saved responses for the same request
     because the URL's parameters appeared in a different order each time.
 
     Parameters
     ----------
-    url : string
-        the URL of the request
-    response_json : dict
-        the JSON response
-    ok : bool
-        requests response.ok value
+    url
+        The URL of the request.
+    response_json
+        The JSON response from the server.
+    ok
+        A `requests.response.ok` value.
 
     Returns
     -------
     None
     """
     if settings.use_cache:
         if not ok:  # pragma: no cover
-            utils.log("Did not save to cache because response status_code is not OK")
-
-        elif response_json is None:  # pragma: no cover
-            utils.log("Did not save to cache because response_json is None")
-
+            msg = "Did not save to cache because HTTP status code is not OK"
+            utils.log(msg, level=lg.WARNING)
         else:
             # create the folder on the disk if it doesn't already exist
             cache_folder = Path(settings.cache_folder)
             cache_folder.mkdir(parents=True, exist_ok=True)
 
             # hash the url to make the filename succinct but unique
             # sha1 digest is 160 bits = 20 bytes = 40 hexadecimal characters
-            filename = sha1(url.encode("utf-8")).hexdigest() + ".json"
-            cache_filepath = cache_folder / filename
+            checksum = sha1(url.encode("utf-8")).hexdigest()  # noqa: S324
+            cache_filepath = cache_folder / f"{checksum}.json"
 
             # dump to json, and save to file
             cache_filepath.write_text(json.dumps(response_json), encoding="utf-8")
-            utils.log(f"Saved response to cache file {str(cache_filepath)!r}")
+            msg = f"Saved response to cache file {str(cache_filepath)!r}"
+            utils.log(msg, level=lg.INFO)
 
 
-def _url_in_cache(url):
+def _url_in_cache(url: str) -> Path | None:
     """
     Determine if a URL's response exists in the cache.
 
-    Calculates the checksum of url to determine the cache file's name.
+    Calculates the checksum of `url` to determine the cache file's name.
+    Returns None if it cannot be found in the cache.
 
     Parameters
     ----------
-    url : string
-        the URL to look for in the cache
+    url
+        The URL to look for in the cache.
 
     Returns
     -------
-    filepath : pathlib.Path
-        path to cached response for url if it exists, otherwise None
+    cache_filepath
+        Path to cached response for `url` if it exists, otherwise None.
     """
     # hash the url to generate the cache filename
-    filename = sha1(url.encode("utf-8")).hexdigest() + ".json"
-    filepath = Path(settings.cache_folder) / filename
+    checksum = sha1(url.encode("utf-8")).hexdigest()  # noqa: S324
+    cache_filepath = Path(settings.cache_folder) / f"{checksum}.json"
 
     # if this file exists in the cache, return its full path
-    return filepath if filepath.is_file() else None
+    return cache_filepath if cache_filepath.is_file() else None
 
 
-def _retrieve_from_cache(url, check_remark=True):
+def _retrieve_from_cache(url: str) -> dict[str, Any] | list[dict[str, Any]] | None:
     """
-    Retrieve a HTTP response JSON object from the cache, if it exists.
+    Retrieve a HTTP response JSON object from the cache if it exists.
+
+    Returns None if there is a server remark in the cached response.
 
     Parameters
     ----------
-    url : string
-        the URL of the request
-    check_remark : string
-        if True, only return filepath if cached response does not have a
-        remark key indicating a server warning
+    url
+        The URL of the request.
 
     Returns
     -------
-    response_json : dict
-        cached response for url if it exists in the cache, otherwise None
+    response_json
+        Cached response for `url` if it exists in the cache and does not
+        contain a server remark, otherwise None.
     """
     # if the tool is configured to use the cache
     if settings.use_cache:
         # return cached response for this url if exists, otherwise return None
         cache_filepath = _url_in_cache(url)
         if cache_filepath is not None:
-            response_json = json.loads(cache_filepath.read_text(encoding="utf-8"))
-
-            # return None if check_remark is True and there is a server
-            # remark in the cached response
-            if check_remark and "remark" in response_json:  # pragma: no cover
-                utils.log(
+            response_json: dict[str, Any] | list[dict[str, Any]] = json.loads(
+                cache_filepath.read_text(encoding="utf-8"),
+            )
+
+            # return None if there is a server remark in the cached response
+            if isinstance(response_json, dict) and ("remark" in response_json):  # pragma: no cover
+                msg = (
                     f"Ignoring cache file {str(cache_filepath)!r} because "
                     f"it contains a remark: {response_json['remark']!r}"
                 )
+                utils.log(msg, lg.WARNING)
                 return None
 
-            utils.log(f"Retrieved response from cache file {str(cache_filepath)!r}")
+            msg = f"Retrieved response from cache file {str(cache_filepath)!r}"
+            utils.log(msg, lg.INFO)
             return response_json
+
     return None
 
 
-def _get_http_headers(user_agent=None, referer=None, accept_language=None):
+def _get_http_headers(
+    *,
+    user_agent: str | None = None,
+    referer: str | None = None,
+    accept_language: str | None = None,
+) -> dict[str, str]:
     """
-    Update the default requests HTTP headers with OSMnx info.
+    Update the default requests HTTP headers with OSMnx information.
 
     Parameters
     ----------
-    user_agent : string
-        the user agent string, if None will set with OSMnx default
-    referer : string
-        the referer string, if None will set with OSMnx default
-    accept_language : string
-        make accept-language explicit e.g. for consistent nominatim result
-        sorting
+    user_agent
+        The user agent. If None, use `settings.http_user_agent` value.
+    referer
+        The referer. If None, use `settings.http_referer` value.
+    accept_language
+        The accept language. If None, use `settings.http_accept_language`
+        value.
 
     Returns
     -------
-    headers : dict
+    headers
     """
-    if settings.default_accept_language is None:
-        default_accept_language = settings.http_accept_language
-    else:
-        default_accept_language = settings.default_accept_language
-        msg = (
-            "`settings.default_accept_language` is deprecated and will be removed "
-            "in the v2.0.0 release: use `settings.http_accept_language` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if settings.default_referer is None:
-        default_referer = settings.http_referer
-    else:
-        default_referer = settings.default_referer
-        msg = (
-            "`settings.default_referer` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.http_referer` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if settings.default_user_agent is None:
-        default_user_agent = settings.http_user_agent
-    else:
-        default_user_agent = settings.default_user_agent
-        msg = (
-            "`settings.default_user_agent` is deprecated and will be removed in "
-            "the v2.0.0 release: use `settings.http_user_agent` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     if user_agent is None:
-        user_agent = default_user_agent
+        user_agent = settings.http_user_agent
     if referer is None:
-        referer = default_referer
+        referer = settings.http_referer
     if accept_language is None:
-        accept_language = default_accept_language
+        accept_language = settings.http_accept_language
 
-    headers = requests.utils.default_headers()
-    headers.update(
-        {"User-Agent": user_agent, "referer": referer, "Accept-Language": accept_language}
-    )
+    info = {"User-Agent": user_agent, "referer": referer, "Accept-Language": accept_language}
+    headers = dict(requests.utils.default_headers())
+    headers.update(info)
     return headers
 
 
-def _resolve_host_via_doh(hostname):
+def _resolve_host_via_doh(hostname: str) -> str:
     """
     Resolve hostname to IP address via Google's public DNS-over-HTTPS API.
 
     Necessary fallback as socket.gethostbyname will not always work when using
     a proxy. See https://developers.google.com/speed/public-dns/docs/doh/json
     If the user has set `settings.doh_url_template=None` or if resolution
     fails (e.g., due to local network blocking DNS-over-HTTPS) the hostname
     itself will be returned instead. Note that this means that server slot
     management may be violated: see `_config_dns` documentation for details.
 
     Parameters
     ----------
-    hostname : string
-        the hostname to consistently resolve the IP address of
+    hostname
+        The hostname to consistently resolve the IP address of.
 
     Returns
     -------
-    ip_address : string
-        resolved IP address of host, or hostname itself if resolution failed
+    ip_address
+        Resolved IP address of host, or hostname itself if resolution failed.
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
-            "release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     if settings.doh_url_template is None:
         # if user has set the url template to None, return hostname itself
-        utils.log("User set `doh_url_template=None`, requesting host by name", level=lg.WARNING)
+        msg = "User set `doh_url_template=None`, requesting host by name"
+        utils.log(msg, level=lg.WARNING)
         return hostname
 
     err_msg = f"Failed to resolve {hostname!r} IP via DoH, requesting host by name"
     try:
         url = settings.doh_url_template.format(hostname=hostname)
-        response = requests.get(url, timeout=timeout)
+        response = requests.get(url, timeout=settings.requests_timeout)
         data = response.json()
 
     # if we cannot reach DoH server or resolve host, return hostname itself
     except requests.exceptions.RequestException:  # pragma: no cover
         utils.log(err_msg, level=lg.ERROR)
         return hostname
 
-    # if there were no exceptions, return
+    # if there were no request exceptions, return
     else:
         if response.ok and data["Status"] == 0:
             # status 0 means NOERROR, so return the IP address
-            return data["Answer"][0]["data"]
+            ip_address: str = data["Answer"][0]["data"]
+            return ip_address
 
         # otherwise, if we cannot reach DoH server or cannot resolve host
         # just return the hostname itself
         utils.log(err_msg, level=lg.ERROR)
         return hostname
 
 
-def _config_dns(url):
+def _config_dns(url: str) -> None:
     """
     Force socket.getaddrinfo to use IP address instead of hostname.
 
     Resolves the URL's domain to an IP address so that we use the same server
     for both 1) checking the necessary pause duration and 2) sending the query
     itself even if there is round-robin redirecting among multiple server
     machines on the server-side. Mutates the getaddrinfo function so it uses
@@ -273,87 +244,95 @@
     if we check the status endpoint of overpass-api.de, we may see results for
     server gall, but when we submit the query itself it gets redirected to
     server lambert. This could result in violating server lambert's slot
     management timing.
 
     Parameters
     ----------
-    url : string
-        the URL to consistently resolve the IP address of
+    url
+        The URL to consistently resolve the IP address of.
 
     Returns
     -------
     None
     """
     hostname = _hostname_from_url(url)
     try:
         ip = socket.gethostbyname(hostname)
     except socket.gaierror:  # pragma: no cover
         # may occur when using a proxy, so instead resolve IP address via DoH
-        utils.log(
-            f"Encountered gaierror while trying to resolve {hostname!r}, trying again via DoH...",
-            level=lg.ERROR,
-        )
+        msg = f"Encountered gaierror while trying to resolve {hostname!r}, trying again via DoH..."
+        utils.log(msg, level=lg.ERROR)
         ip = _resolve_host_via_doh(hostname)
 
     # mutate socket.getaddrinfo to map hostname -> IP address
-    def _getaddrinfo(*args, **kwargs):
+    def _getaddrinfo(*args: Any, **kwargs: Any) -> Any:  # noqa: ANN401
         if args[0] == hostname:
-            utils.log(f"Resolved {hostname!r} to {ip!r}")
+            msg = f"Resolved {hostname!r} to {ip!r}"
+            utils.log(msg, level=lg.INFO)
             return _original_getaddrinfo(ip, *args[1:], **kwargs)
 
         # otherwise
         return _original_getaddrinfo(*args, **kwargs)
 
     socket.getaddrinfo = _getaddrinfo
 
 
-def _hostname_from_url(url):
+def _hostname_from_url(url: str) -> str:
     """
     Extract the hostname (domain) from a URL.
 
     Parameters
     ----------
-    url : string
-        the url from which to extract the hostname
+    url
+        The url from which to extract the hostname.
 
     Returns
     -------
-    hostname : string
-        the extracted hostname (domain)
+    hostname
+        The extracted hostname (domain).
     """
     return urlparse(url).netloc.split(":")[0]
 
 
-def _parse_response(response):
+def _parse_response(response: requests.Response) -> dict[str, Any] | list[dict[str, Any]]:
     """
     Parse JSON from a requests response and log the details.
 
     Parameters
     ----------
-    response : requests.response
-        the response object
+    response
+        The response object.
 
     Returns
     -------
-    response_json : dict
+    response_json
+        Value will be a dict if the response is from the Google or Overpass
+        APIs, and a list if the response is from the Nominatim API.
     """
     # log the response size and domain
     domain = _hostname_from_url(response.url)
     size_kb = len(response.content) / 1000
-    utils.log(f"Downloaded {size_kb:,.1f}kB from {domain!r} with status {response.status_code}")
+    msg = f"Downloaded {size_kb:,.1f}kB from {domain!r} with status {response.status_code}"
+    utils.log(msg, level=lg.INFO)
 
     # parse the response to JSON and log/raise exceptions
     try:
-        response_json = response.json()
+        response_json: dict[str, Any] | list[dict[str, Any]] = response.json()
     except JSONDecodeError as e:  # pragma: no cover
         msg = f"{domain!r} responded: {response.status_code} {response.reason} {response.text}"
         utils.log(msg, level=lg.ERROR)
         if response.ok:
             raise InsufficientResponseError(msg) from e
         raise ResponseStatusCodeError(msg) from e
 
     # log any remarks if they exist
-    if "remark" in response_json:  # pragma: no cover
-        utils.log(f'{domain!r} remarked: {response_json["remark"]!r}', level=lg.WARNING)
+    if isinstance(response_json, dict) and "remark" in response_json:  # pragma: no cover
+        msg = f"{domain!r} remarked: {response_json['remark']!r}"
+        utils.log(msg, level=lg.WARNING)
+
+    # log if the response status_code is not OK
+    if not response.ok:
+        msg = f"{domain!r} returned HTTP status code {response.status_code}"
+        utils.log(msg, level=lg.WARNING)
 
     return response_json
```

### Comparing `osmnx-1.9.3/osmnx/_nominatim.py` & `osmnx-2.0.0b0/osmnx/_nominatim.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 """Tools to work with the Nominatim API."""
 
+from __future__ import annotations
+
 import logging as lg
 import time
 from collections import OrderedDict
-from warnings import warn
+from typing import Any
 
 import requests
 
-from . import _downloader
+from . import _http
 from . import settings
 from . import utils
+from ._errors import InsufficientResponseError
 
 
-def _download_nominatim_element(query, by_osmid=False, limit=1, polygon_geojson=1):
+def _download_nominatim_element(
+    query: str | dict[str, str],
+    *,
+    by_osmid: bool = False,
+    limit: int = 1,
+    polygon_geojson: bool = True,
+) -> list[dict[str, Any]]:
     """
     Retrieve an OSM element from the Nominatim API.
 
     Parameters
     ----------
-    query : string or dict
-        query string or structured query dict
-    by_osmid : bool
-        if True, treat query as an OSM ID lookup rather than text search
-    limit : int
-        max number of results to return
-    polygon_geojson : int
-        retrieve the place's geometry from the API, 0=no, 1=yes
+    query
+        Query string or structured query dict.
+    by_osmid
+        If True, treat `query` as an OSM ID lookup rather than text search.
+    limit
+        Max number of results to return.
+    polygon_geojson
+        Whether to retrieve the place's geometry from the API.
 
     Returns
     -------
-    response_json : dict
-        JSON response from the Nominatim server
+    response_json
     """
     # define the parameters
-    params = OrderedDict()
+    params: OrderedDict[str, int | str] = OrderedDict()
     params["format"] = "json"
-    params["polygon_geojson"] = polygon_geojson
+    params["polygon_geojson"] = int(polygon_geojson)  # bool -> int
 
     if by_osmid:
         # if querying by OSM ID, use the lookup endpoint
+        if not isinstance(query, str):
+            msg = "`query` must be a string if `by_osmid` is True."
+            raise TypeError(msg)
         request_type = "lookup"
         params["osm_ids"] = query
 
     else:
         # if not querying by OSM ID, use the search endpoint
         request_type = "search"
 
@@ -54,96 +65,94 @@
             params["q"] = query
         elif isinstance(query, dict):
             # add query keys in alphabetical order so URL is the same string
             # each time, for caching purposes
             for key in sorted(query):
                 params[key] = query[key]
         else:  # pragma: no cover
-            msg = "query must be a dict or a string"
+            msg = "Each query must be a dict or a string."  # type: ignore[unreachable]
             raise TypeError(msg)
 
     # request the URL, return the JSON
     return _nominatim_request(params=params, request_type=request_type)
 
 
-def _nominatim_request(params, request_type="search", pause=1, error_pause=60):
+def _nominatim_request(
+    params: OrderedDict[str, int | str],
+    *,
+    request_type: str = "search",
+    pause: float = 1,
+    error_pause: float = 60,
+) -> list[dict[str, Any]]:
     """
     Send a HTTP GET request to the Nominatim API and return response.
 
     Parameters
     ----------
-    params : OrderedDict
-        key-value pairs of parameters
-    request_type : string {"search", "reverse", "lookup"}
-        which Nominatim API endpoint to query
-    pause : float
-        how long to pause before request, in seconds. per the nominatim usage
-        policy: "an absolute maximum of 1 request per second" is allowed
-    error_pause : float
-        how long to pause in seconds before re-trying request if error
+    params
+        Key-value pairs of parameters.
+    request_type
+        {"search", "reverse", "lookup"}
+        Which Nominatim API endpoint to query.
+    pause
+        How long to pause before request, in seconds. Per the Nominatim usage
+        policy: "an absolute maximum of 1 request per second" is allowed.
+    error_pause
+        How long to pause in seconds before re-trying request if error.
 
     Returns
     -------
-    response_json : dict
+    response_json
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
-            "release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if settings.nominatim_endpoint is None:
-        nominatim_endpoint = settings.nominatim_url
-    else:
-        nominatim_endpoint = settings.nominatim_endpoint
-        msg = (
-            "`settings.nominatim_endpoint` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.nominatim_url` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     if request_type not in {"search", "reverse", "lookup"}:  # pragma: no cover
-        msg = 'Nominatim request_type must be "search", "reverse", or "lookup"'
+        msg = "Nominatim `request_type` must be 'search', 'reverse', or 'lookup'."
         raise ValueError(msg)
 
+    # add nominatim API key to params if one has been provided in settings
+    if settings.nominatim_key is not None:
+        params["key"] = settings.nominatim_key
+
     # prepare Nominatim API URL and see if request already exists in cache
-    url = nominatim_endpoint.rstrip("/") + "/" + request_type
-    params["key"] = settings.nominatim_key
-    prepared_url = requests.Request("GET", url, params=params).prepare().url
-    cached_response_json = _downloader._retrieve_from_cache(prepared_url)
-    if cached_response_json is not None:
+    url = settings.nominatim_url.rstrip("/") + "/" + request_type
+    prepared_url = str(requests.Request("GET", url, params=params).prepare().url)
+    cached_response_json = _http._retrieve_from_cache(prepared_url)
+    if isinstance(cached_response_json, list):
         return cached_response_json
 
     # pause then request this URL
-    domain = _downloader._hostname_from_url(url)
-    utils.log(f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}")
+    domain = _http._hostname_from_url(url)
+    msg = f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}"
+    utils.log(msg, level=lg.INFO)
     time.sleep(pause)
 
     # transmit the HTTP GET request
-    utils.log(f"Get {prepared_url} with timeout={timeout}")
+    msg = f"Get {prepared_url} with timeout={settings.requests_timeout}"
+    utils.log(msg, level=lg.INFO)
     response = requests.get(
         url,
         params=params,
-        timeout=timeout,
-        headers=_downloader._get_http_headers(),
+        timeout=settings.requests_timeout,
+        headers=_http._get_http_headers(),
         **settings.requests_kwargs,
     )
 
     # handle 429 and 504 errors by pausing then recursively re-trying request
     if response.status_code in {429, 504}:  # pragma: no cover
         msg = (
             f"{domain!r} responded {response.status_code} {response.reason}: "
             f"we'll retry in {error_pause} secs"
         )
         utils.log(msg, level=lg.WARNING)
         time.sleep(error_pause)
-        return _nominatim_request(params, request_type, pause, error_pause)
+        return _nominatim_request(
+            params,
+            request_type=request_type,
+            pause=pause,
+            error_pause=error_pause,
+        )
 
-    response_json = _downloader._parse_response(response)
-    _downloader._save_to_cache(prepared_url, response_json, response.status_code)
+    response_json = _http._parse_response(response)
+    if not isinstance(response_json, list):
+        msg = "Nominatim API did not return a list of results."
+        raise InsufficientResponseError(msg)
+    _http._save_to_cache(prepared_url, response_json, response.ok)
     return response_json
```

### Comparing `osmnx-1.9.3/osmnx/_overpass.py` & `osmnx-2.0.0b0/osmnx/_overpass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,81 @@
 """Tools to work with the Overpass API."""
 
+from __future__ import annotations
+
 import datetime as dt
 import logging as lg
 import time
-from warnings import warn
+from collections import OrderedDict
+from typing import TYPE_CHECKING
+from typing import Any
 
 import numpy as np
 import requests
 from requests.exceptions import ConnectionError
 
-from . import _downloader
+from . import _http
 from . import projection
 from . import settings
 from . import utils
 from . import utils_geo
+from ._errors import InsufficientResponseError
+
+if TYPE_CHECKING:
+    from collections.abc import Iterator
 
+    from shapely import MultiPolygon
+    from shapely import Polygon
 
-def _get_osm_filter(network_type):
+
+def _get_network_filter(network_type: str) -> str:
     """
-    Create a filter to query OSM for the specified network type.
+    Create a filter to query Overpass for the specified network type.
+
+    The filter queries Overpass for every OSM way with a "highway" tag but
+    excludes ways that are incompatible with the requested network type. You
+    can choose from the following types:
+
+    "all" retrieves all public and private-access ways currently in use.
+
+    "all_public" retrieves all public ways currently in use.
+
+    "bike" retrieves public bikeable ways and excludes foot ways, motor ways,
+    and anything tagged biking=no.
+
+    "drive" retrieves public drivable streets and excludes service roads,
+    anything tagged motor=no, and certain non-service roads tagged as
+    providing certain services (such as alleys or driveways).
+
+    "drive_service" retrieves public drivable streets including service roads
+    but excludes certain services (such as parking or emergency access).
+
+    "walk" retrieves public walkable ways and excludes cycle ways, motor ways,
+    and anything tagged foot=no. It includes service roads like parking lot
+    aisles and alleys that you can walk on even if they are unpleasant walks.
 
     Parameters
     ----------
-    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve.
 
     Returns
     -------
-    string
+    way_filter
+        The Overpass query filter.
     """
-    if network_type == "all_private":
-        network_type = "all"
-        msg = (
-            "The 'all_private' network type has been renamed 'all'. The old "
-            "'all_private' naming is deprecated and will be removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     # define built-in queries to send to the API. specifying way["highway"]
     # means that all ways returned must have a highway tag. the filters then
     # remove ways by tag/value.
     filters = {}
 
     # driving: filter out un-drivable roads, service roads, private ways, and
-    # anything specifying motor=no. also filter out any non-service roads that
-    # are tagged as providing certain services
+    # anything tagged motor=no. also filter out any non-service roads that are
+    # tagged as providing certain services
     filters["drive"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bridleway|bus_guideway|construction|corridor|cycleway|elevator|'
         f"escalator|footway|no|path|pedestrian|planned|platform|proposed|raceway|razed|service|"
         f'steps|track"]'
         f'["motor_vehicle"!~"no"]["motorcar"!~"no"]'
         f'["service"!~"alley|driveway|emergency_access|parking|parking_aisle|private"]'
@@ -62,238 +88,219 @@
         f"escalator|footway|no|path|pedestrian|planned|platform|proposed|raceway|razed|steps|"
         f'track"]'
         f'["motor_vehicle"!~"no"]["motorcar"!~"no"]'
         f'["service"!~"emergency_access|parking|parking_aisle|private"]'
     )
 
     # walking: filter out cycle ways, motor ways, private ways, and anything
-    # specifying foot=no. allow service roads, permitting things like parking
-    # lot lanes, alleys, etc that you *can* walk on even if they're not
-    # exactly pleasant walks. some cycleways may allow pedestrians, but this
-    # filter ignores such cycleways.
+    # tagged foot=no. allow service roads, permitting things like parking lot
+    # aisles, alleys, etc that you *can* walk on even if they're not exactly
+    # pleasant walks. some cycleways may allow pedestrians, but this filter
+    # ignores such cycleways.
     filters["walk"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bus_guideway|construction|cycleway|motor|no|planned|platform|'
         f'proposed|raceway|razed"]'
         f'["foot"!~"no"]["service"!~"private"]'
     )
 
     # biking: filter out foot ways, motor ways, private ways, and anything
-    # specifying biking=no
+    # tagged biking=no
     filters["bike"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|bus_guideway|construction|corridor|elevator|escalator|footway|'
         f'motor|no|planned|platform|proposed|raceway|razed|steps"]'
         f'["bicycle"!~"no"]["service"!~"private"]'
     )
 
-    # to download all ways, just filter out everything not currently in use or
-    # that is private-access only
+    # to download all public ways, just filter out everything not currently in
+    # use or that is private-access only
     filters["all_public"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|construction|no|planned|platform|proposed|raceway|razed"]'
         f'["service"!~"private"]'
     )
 
     # to download all ways, including private-access ones, just filter out
     # everything not currently in use
     filters["all"] = (
         '["highway"]["area"!~"yes"]["highway"!~"abandoned|construction|no|planned|platform|'
         'proposed|raceway|razed"]'
     )
 
     if network_type in filters:
-        osm_filter = filters[network_type]
+        way_filter = filters[network_type]
     else:  # pragma: no cover
-        msg = f"Unrecognized network_type {network_type!r}"
+        msg = f"Unrecognized network_type {network_type!r}."
         raise ValueError(msg)
 
-    return osm_filter
+    return way_filter
 
 
-def _get_overpass_pause(base_endpoint, recursive_delay=5, default_duration=60):
+def _get_overpass_pause(
+    base_endpoint: str,
+    *,
+    recursive_delay: float = 5,
+    default_duration: float = 60,
+) -> float:
     """
     Retrieve a pause duration from the Overpass API status endpoint.
 
     Check the Overpass API status endpoint to determine how long to wait until
     the next slot is available. You can disable this via the `settings`
     module's `overpass_rate_limit` setting.
 
     Parameters
     ----------
-    base_endpoint : string
-        base Overpass API url (without "/status" at the end)
-    recursive_delay : int
-        how long to wait between recursive calls if the server is currently
-        running a query
-    default_duration : int
-        if fatal error, fall back on returning this value
+    base_endpoint
+        Base Overpass API URL (without "/status" at the end).
+    recursive_delay
+        How long to wait between recursive calls if the server is currently
+        running a query.
+    default_duration
+        If a fatal error occurs, fall back on returning this value.
 
     Returns
     -------
-    pause : int
+    pause
+        The current pause duration specified by the Overpass status endpoint.
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     if not settings.overpass_rate_limit:
         # if overpass rate limiting is False, then there is zero pause
         return 0
 
     try:
         url = base_endpoint.rstrip("/") + "/status"
         response = requests.get(
             url,
-            headers=_downloader._get_http_headers(),
-            timeout=timeout,
+            headers=_http._get_http_headers(),
+            timeout=settings.requests_timeout,
             **settings.requests_kwargs,
         )
         status = response.text.split("\n")[4]
-        status_first_token = status.split(" ")[0]
-    except ConnectionError:  # pragma: no cover
+        status_first_part = status.split(" ")[0]
+    except ConnectionError as e:  # pragma: no cover
         # cannot reach status endpoint, log error and return default duration
-        utils.log(f"Unable to query {url}, got status {response.status_code}", level=lg.ERROR)
+        msg = f"Unable to query {url}, {e}"
+        utils.log(msg, level=lg.ERROR)
         return default_duration
     except (AttributeError, IndexError, ValueError):  # pragma: no cover
         # cannot parse output, log error and return default duration
-        utils.log(f"Unable to parse {url} response: {response.text}", level=lg.ERROR)
+        msg = f"Unable to parse {url} response: {response.text}"
+        utils.log(msg, level=lg.ERROR)
         return default_duration
 
     try:
         # if first token is numeric, it's how many slots you have available,
         # no wait required
-        _ = int(status_first_token)  # number of available slots
-        pause = 0
+        _ = int(status_first_part)  # number of available slots
+        pause: float = 0
 
     except ValueError:  # pragma: no cover
         # if first token is 'Slot', it tells you when your slot will be free
-        if status_first_token == "Slot":
+        if status_first_part == "Slot":
             utc_time_str = status.split(" ")[3]
             pattern = "%Y-%m-%dT%H:%M:%SZ,"
             utc_time = dt.datetime.strptime(utc_time_str, pattern).astimezone(dt.timezone.utc)
             utc_now = dt.datetime.now(tz=dt.timezone.utc)
             seconds = int(np.ceil((utc_time - utc_now).total_seconds()))
             pause = max(seconds, 1)
 
         # if first token is 'Currently', it is currently running a query so
         # check back in recursive_delay seconds
-        elif status_first_token == "Currently":
+        elif status_first_part == "Currently":
             time.sleep(recursive_delay)
             pause = _get_overpass_pause(base_endpoint)
 
         # any other status is unrecognized: log error, return default duration
         else:
-            utils.log(f"Unrecognized server status: {status!r}", level=lg.ERROR)
+            msg = f"Unrecognized server status: {status!r}"
+            utils.log(msg, level=lg.ERROR)
             return default_duration
 
     return pause
 
 
-def _make_overpass_settings():
+def _make_overpass_settings() -> str:
     """
     Make settings string to send in Overpass query.
 
     Returns
     -------
-    string
+    overpass_settings
+        The `settings.overpass_settings` string formatted with "timeout" and
+        "maxsize" values.
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if settings.memory is None:
-        memory = settings.overpass_memory
-    else:
-        memory = settings.memory
-        msg = (
-            "`settings.memory` is deprecated and will be removed in the "
-            " v2.0.0 release: use `settings.overpass_memory` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
+    maxsize = "" if settings.overpass_memory is None else f"[maxsize:{settings.overpass_memory}]"
+    return settings.overpass_settings.format(timeout=settings.requests_timeout, maxsize=maxsize)
 
-    maxsize = "" if memory is None else f"[maxsize:{memory}]"
-    return settings.overpass_settings.format(timeout=timeout, maxsize=maxsize)
 
-
-def _make_overpass_polygon_coord_strs(polygon):
+def _make_overpass_polygon_coord_strs(polygon: Polygon | MultiPolygon) -> list[str]:
     """
     Subdivide query polygon and return list of coordinate strings.
 
-    Project to utm, divide polygon up into sub-polygons if area exceeds a
+    Project to UTM, divide `polygon` up into sub-polygons if area exceeds a
     max size (in meters), project back to lat-lon, then get a list of
     polygon(s) exterior coordinates. Ignore interior ("holes") coordinates.
 
     Parameters
     ----------
-    polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        polygon to convert to exterior coordinate strings
+    polygon
+        The (Multi)Polygon to convert to exterior coordinate strings.
 
     Returns
     -------
-    coord_strs : list
-        list of strings of exterior coordinates of polygon(s)
+    coord_strs
+        Exterior coordinates of polygon(s).
     """
     # first subdivide the polygon if its area exceeds max size
     # this results in a multipolygon of 1+ constituent polygons
     poly_proj, crs_proj = projection.project_geometry(polygon)
     multi_poly_proj = utils_geo._consolidate_subdivide_geometry(poly_proj)
     multi_poly, _ = projection.project_geometry(multi_poly_proj, crs=crs_proj, to_latlong=True)
 
     # then extract each's exterior coords to the string format Overpass
-    # expects, rounding lats and lons to 6 decimals (ie, ~100 mm) so we
-    # can hash and cache URL strings consistently
+    # expects, rounding lats and lons to 6 decimals (approx 5 to 10 cm
+    # resolution) so we can hash and cache URL strings consistently
     coord_strs = []
     for geom in multi_poly.geoms:
         x, y = geom.exterior.xy
-        coord_list = [f'{xy[1]:.6f}{" "}{xy[0]:.6f}' for xy in zip(x, y)]
+        coord_list = [f"{xy[1]:.6f}{' '}{xy[0]:.6f}" for xy in zip(x, y)]
         coord_strs.append(" ".join(coord_list))
 
     return coord_strs
 
 
-def _create_overpass_query(polygon_coord_str, tags):
+def _create_overpass_features_query(  # noqa: PLR0912
+    polygon_coord_str: str,
+    tags: dict[str, bool | str | list[str]],
+) -> str:
     """
-    Create an Overpass features query string based on passed tags.
+    Create an Overpass features query string based on tags.
 
     Parameters
     ----------
-    polygon_coord_str : list
-        list of lat lon coordinates
-    tags : dict
-        dict of tags used for finding elements in the search area
+    polygon_coord_str
+        The lat lon coordinates.
+    tags
+        Tags used for finding elements in the search area.
 
     Returns
     -------
-    query : string
+    query
     """
     # create overpass settings string
     overpass_settings = _make_overpass_settings()
 
     # make sure every value in dict is bool, str, or list of str
-    err_msg = "tags must be a dict with values of bool, str, or list of str"
+    err_msg = "`tags` must be a dict with values of bool, str, or list of str."
     if not isinstance(tags, dict):  # pragma: no cover
         raise TypeError(err_msg)
 
-    tags_dict = {}
+    tags_dict: dict[str, bool | str | list[str]] = {}
     for key, value in tags.items():
         if isinstance(value, bool):
             tags_dict[key] = value
 
         elif isinstance(value, str):
             tags_dict[key] = [value]
 
@@ -302,15 +309,15 @@
                 raise TypeError(err_msg)
             tags_dict[key] = value
 
         else:  # pragma: no cover
             raise TypeError(err_msg)
 
     # convert the tags dict into a list of {tag:value} dicts
-    tags_list = []
+    tags_list: list[dict[str, bool | str | list[str]]] = []
     for key, value in tags_dict.items():
         if isinstance(value, bool):
             tags_list.append({key: value})
         else:
             for value_item in value:
                 tags_list.append({key: value_item})  # noqa: PERF401
 
@@ -325,155 +332,152 @@
                 # otherwise, pass "key"="value"
                 tag_str = f"[{key!r}={value!r}](poly:{polygon_coord_str!r});(._;>;);"
 
             for kind in ("node", "way", "relation"):
                 components.append(f"({kind}{tag_str});")  # noqa: PERF401
 
     # finalize query and return
-    components = "".join(components)
-    return f"{overpass_settings};({components});out;"
+    components_str = "".join(components)
+    return f"{overpass_settings};({components_str});out;"
 
 
-def _download_overpass_network(polygon, network_type, custom_filter):
+def _download_overpass_network(
+    polygon: Polygon | MultiPolygon,
+    network_type: str,
+    custom_filter: str | None,
+) -> Iterator[dict[str, Any]]:
     """
     Retrieve networked ways and nodes within boundary from the Overpass API.
 
     Parameters
     ----------
-    polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        boundary to fetch the network ways/nodes within
-    network_type : string
-        what type of street network to get if custom_filter is None
-    custom_filter : string
-        a custom "ways" filter to be used instead of the network_type presets
+    polygon
+        The boundary to fetch the network ways/nodes within.
+    network_type
+        What type of street network to get if `custom_filter` is None.
+    custom_filter
+        A custom "ways" filter to be used instead of `network_type` presets.
 
     Yields
     ------
-    response_json : dict
-        a generator of JSON responses from the Overpass server
+    response_json
+        JSON response from the Overpass server.
     """
     # create a filter to exclude certain kinds of ways based on the requested
     # network_type, if provided, otherwise use custom_filter
-    osm_filter = custom_filter if custom_filter is not None else _get_osm_filter(network_type)
+    way_filter = custom_filter if custom_filter is not None else _get_network_filter(network_type)
 
     # create overpass settings string
     overpass_settings = _make_overpass_settings()
 
     # subdivide query polygon to get list of sub-divided polygon coord strings
     polygon_coord_strs = _make_overpass_polygon_coord_strs(polygon)
-    utils.log(f"Requesting data from API in {len(polygon_coord_strs)} request(s)")
+    msg = f"Requesting data from API in {len(polygon_coord_strs)} request(s)"
+    utils.log(msg, level=lg.INFO)
 
     # pass exterior coordinates of each polygon in list to API, one at a time
     # the '>' makes it recurse so we get ways and the ways' nodes.
     for polygon_coord_str in polygon_coord_strs:
-        query_str = f"{overpass_settings};(way{osm_filter}(poly:{polygon_coord_str!r});>;);out;"
-        yield _overpass_request(data={"data": query_str})
+        query_str = f"{overpass_settings};(way{way_filter}(poly:{polygon_coord_str!r});>;);out;"
+        yield _overpass_request(OrderedDict(data=query_str))
 
 
-def _download_overpass_features(polygon, tags):
+def _download_overpass_features(
+    polygon: Polygon,
+    tags: dict[str, bool | str | list[str]],
+) -> Iterator[dict[str, Any]]:
     """
-    Retrieve OSM features within boundary from the Overpass API.
+    Retrieve OSM features within some boundary polygon from the Overpass API.
 
     Parameters
     ----------
-    polygon : shapely.geometry.Polygon
-        boundaries to fetch elements within
-    tags : dict
-        dict of tags used for finding elements in the selected area
+    polygon
+        Boundary to retrieve elements within.
+    tags
+        Tags used for finding elements in the selected area.
 
     Yields
     ------
-    response_json : dict
-        a generator of JSON responses from the Overpass server
+    response_json
+        JSON response from the Overpass server.
     """
     # subdivide query polygon to get list of sub-divided polygon coord strings
     polygon_coord_strs = _make_overpass_polygon_coord_strs(polygon)
-    utils.log(f"Requesting data from API in {len(polygon_coord_strs)} request(s)")
+    msg = f"Requesting data from API in {len(polygon_coord_strs)} request(s)"
+    utils.log(msg, level=lg.INFO)
 
     # pass exterior coordinates of each polygon in list to API, one at a time
     for polygon_coord_str in polygon_coord_strs:
-        query_str = _create_overpass_query(polygon_coord_str, tags)
-        yield _overpass_request(data={"data": query_str})
+        query_str = _create_overpass_features_query(polygon_coord_str, tags)
+        yield _overpass_request(OrderedDict(data=query_str))
 
 
-def _overpass_request(data, pause=None, error_pause=60):
+def _overpass_request(
+    data: OrderedDict[str, Any],
+    *,
+    pause: float | None = None,
+    error_pause: float = 60,
+) -> dict[str, Any]:
     """
     Send a HTTP POST request to the Overpass API and return response.
 
     Parameters
     ----------
-    data : OrderedDict
-        key-value pairs of parameters
-    pause : float
-        how long to pause in seconds before request, if None, will query API
-        status endpoint to find when next slot is available
-    error_pause : float
-        how long to pause in seconds (in addition to `pause`) before re-trying
-        request if error
+    data
+        Key-value pairs of parameters.
+    pause
+        How long to pause in seconds before request. If None, will query API
+        status endpoint to find when next slot is available.
+    error_pause
+        How long to pause in seconds (in addition to `pause`) before re-trying
+        request if error.
 
     Returns
     -------
-    response_json : dict
+    response_json
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if settings.overpass_endpoint is None:
-        overpass_endpoint = settings.overpass_url
-    else:
-        overpass_endpoint = settings.overpass_endpoint
-        msg = (
-            "`settings.overpass_endpoint` is deprecated and will be removed in the "
-            "v2.0.0 release: use `settings.overpass_url` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     # resolve url to same IP even if there is server round-robin redirecting
-    _downloader._config_dns(overpass_endpoint)
+    _http._config_dns(settings.overpass_url)
 
     # prepare the Overpass API URL and see if request already exists in cache
-    url = overpass_endpoint.rstrip("/") + "/interpreter"
-    prepared_url = requests.Request("GET", url, params=data).prepare().url
-    cached_response_json = _downloader._retrieve_from_cache(prepared_url)
-    if cached_response_json is not None:
+    url = settings.overpass_url.rstrip("/") + "/interpreter"
+    prepared_url = str(requests.Request("GET", url, params=data).prepare().url)
+    cached_response_json = _http._retrieve_from_cache(prepared_url)
+    if isinstance(cached_response_json, dict):
         return cached_response_json
 
     # pause then request this URL
     if pause is None:
-        this_pause = _get_overpass_pause(overpass_endpoint)
-    domain = _downloader._hostname_from_url(url)
-    utils.log(f"Pausing {this_pause} second(s) before making HTTP POST request to {domain!r}")
+        this_pause = _get_overpass_pause(settings.overpass_url)
+    domain = _http._hostname_from_url(url)
+    msg = f"Pausing {this_pause} second(s) before making HTTP POST request to {domain!r}"
+    utils.log(msg, level=lg.INFO)
     time.sleep(this_pause)
 
     # transmit the HTTP POST request
-    utils.log(f"Post {prepared_url} with timeout={timeout}")
+    msg = f"Post {prepared_url} with timeout={settings.requests_timeout}"
+    utils.log(msg, level=lg.INFO)
     response = requests.post(
         url,
         data=data,
-        timeout=timeout,
-        headers=_downloader._get_http_headers(),
+        timeout=settings.requests_timeout,
+        headers=_http._get_http_headers(),
         **settings.requests_kwargs,
     )
 
     # handle 429 and 504 errors by pausing then recursively re-trying request
     if response.status_code in {429, 504}:  # pragma: no cover
-        this_pause = error_pause + _get_overpass_pause(overpass_endpoint)
+        this_pause = error_pause + _get_overpass_pause(settings.overpass_url)
         msg = (
             f"{domain!r} responded {response.status_code} {response.reason}: "
             f"we'll retry in {this_pause} secs"
         )
         utils.log(msg, level=lg.WARNING)
         time.sleep(this_pause)
-        return _overpass_request(data, pause, error_pause)
+        return _overpass_request(data, pause=pause, error_pause=error_pause)
 
-    response_json = _downloader._parse_response(response)
-    _downloader._save_to_cache(prepared_url, response_json, response.status_code)
+    response_json = _http._parse_response(response)
+    if not isinstance(response_json, dict):  # pragma: no cover
+        msg = "Overpass API did not return a dict of results."
+        raise InsufficientResponseError(msg)
+    _http._save_to_cache(prepared_url, response_json, response.ok)
     return response_json
```

### Comparing `osmnx-1.9.3/osmnx/bearing.py` & `osmnx-2.0.0b0/osmnx/bearing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,325 +1,296 @@
-"""Calculate graph edge bearings."""
+"""Calculate graph edge bearings and orientation entropy."""
 
+from __future__ import annotations
+
+from typing import overload
 from warnings import warn
 
 import networkx as nx
 import numpy as np
+import numpy.typing as npt
 
-from . import plot
 from . import projection
 
 # scipy is an optional dependency for entropy calculation
 try:
     import scipy
 except ImportError:  # pragma: no cover
     scipy = None
 
 
-def calculate_bearing(lat1, lon1, lat2, lon2):
+# if coords are all floats, return float
+@overload
+def calculate_bearing(
+    lat1: float,
+    lon1: float,
+    lat2: float,
+    lon2: float,
+) -> float: ...
+
+
+# if coords are all arrays, return array
+@overload
+def calculate_bearing(
+    lat1: npt.NDArray[np.float64],
+    lon1: npt.NDArray[np.float64],
+    lat2: npt.NDArray[np.float64],
+    lon2: npt.NDArray[np.float64],
+) -> npt.NDArray[np.float64]: ...
+
+
+def calculate_bearing(
+    lat1: float | npt.NDArray[np.float64],
+    lon1: float | npt.NDArray[np.float64],
+    lat2: float | npt.NDArray[np.float64],
+    lon2: float | npt.NDArray[np.float64],
+) -> float | npt.NDArray[np.float64]:
     """
     Calculate the compass bearing(s) between pairs of lat-lon points.
 
     Vectorized function to calculate initial bearings between two points'
     coordinates or between arrays of points' coordinates. Expects coordinates
-    in decimal degrees. Bearing represents the clockwise angle in degrees
-    between north and the geodesic line from (lat1, lon1) to (lat2, lon2).
+    in decimal degrees. The bearing represents the clockwise angle in degrees
+    between north and the geodesic line from `(lat1, lon1)` to `(lat2, lon2)`.
 
     Parameters
     ----------
-    lat1 : float or numpy.array of float
-        first point's latitude coordinate
-    lon1 : float or numpy.array of float
-        first point's longitude coordinate
-    lat2 : float or numpy.array of float
-        second point's latitude coordinate
-    lon2 : float or numpy.array of float
-        second point's longitude coordinate
+    lat1
+        First point's latitude coordinate(s).
+    lon1
+        First point's longitude coordinate(s).
+    lat2
+        Second point's latitude coordinate(s).
+    lon2
+        Second point's longitude coordinate(s).
 
     Returns
     -------
-    bearing : float or numpy.array of float
-        the bearing(s) in decimal degrees
+    bearing
+        The bearing(s) in decimal degrees.
     """
     # get the latitudes and the difference in longitudes, all in radians
     lat1 = np.radians(lat1)
     lat2 = np.radians(lat2)
     delta_lon = np.radians(lon2 - lon1)
 
     # calculate initial bearing from -180 degrees to +180 degrees
     y = np.sin(delta_lon) * np.cos(lat2)
     x = np.cos(lat1) * np.sin(lat2) - np.sin(lat1) * np.cos(lat2) * np.cos(delta_lon)
     initial_bearing = np.degrees(np.arctan2(y, x))
 
     # normalize to 0-360 degrees to get compass bearing
-    return initial_bearing % 360
+    bearing: float | npt.NDArray[np.float64] = initial_bearing % 360
+    return bearing
 
 
-def add_edge_bearings(G, precision=None):
+def add_edge_bearings(G: nx.MultiDiGraph) -> nx.MultiDiGraph:
     """
-    Add compass `bearing` attributes to all graph edges.
+    Calculate and add compass `bearing` attributes to all graph edges.
 
     Vectorized function to calculate (initial) bearing from origin node to
     destination node for each edge in a directed, unprojected graph then add
-    these bearings as new edge attributes. Bearing represents angle in degrees
-    (clockwise) between north and the geodesic line from the origin node to
-    the destination node. Ignores self-loop edges as their bearings are
-    undefined.
+    these bearings as new `bearing` edge attributes. Bearing represents angle
+    in degrees (clockwise) between north and the geodesic line from the origin
+    node to the destination node. Ignores self-loop edges as their bearings
+    are undefined.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        unprojected graph
-    precision : int
-        deprecated, do not use
+    G
+        Unprojected graph.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with edge bearing attributes
+    G
+        Graph with `bearing` attributes on the edges.
     """
-    if precision is None:
-        precision = 1
-    else:
-        warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
     if projection.is_projected(G.graph["crs"]):  # pragma: no cover
-        msg = "graph must be unprojected to add edge bearings"
+        msg = "Graph must be unprojected to add edge bearings."
         raise ValueError(msg)
 
     # extract edge IDs and corresponding coordinates from their nodes
     uvk = [(u, v, k) for u, v, k in G.edges if u != v]
     x = G.nodes(data="x")
     y = G.nodes(data="y")
     coords = np.array([(y[u], x[u], y[v], x[v]) for u, v, k in uvk])
 
     # calculate bearings then set as edge attributes
     bearings = calculate_bearing(coords[:, 0], coords[:, 1], coords[:, 2], coords[:, 3])
-    values = zip(uvk, bearings.round(precision))
+    values = zip(uvk, bearings)
     nx.set_edge_attributes(G, dict(values), name="bearing")
 
     return G
 
 
-def orientation_entropy(Gu, num_bins=36, min_length=0, weight=None):
+def orientation_entropy(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    num_bins: int = 36,
+    min_length: float = 0,
+    weight: str | None = None,
+) -> float:
     """
-    Calculate undirected graph's orientation entropy.
+    Calculate graph's orientation entropy.
 
-    Orientation entropy is the entropy of its edges' bidirectional bearings
+    Orientation entropy is the Shannon entropy of the graphs' edges' bearings
     across evenly spaced bins. Ignores self-loop edges as their bearings are
-    undefined.
+    undefined. If `G` is a MultiGraph, all edge bearings will be bidirectional
+    (ie, two reciprocal bearings per undirected edge). If `G` is a
+    MultiDiGraph, all edge bearings will be directional (ie, one bearing per
+    directed edge).
 
     For more info see: Boeing, G. 2019. "Urban Spatial Order: Street Network
     Orientation, Configuration, and Entropy." Applied Network Science, 4 (1),
     67. https://doi.org/10.1007/s41109-019-0189-1
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected, unprojected graph with `bearing` attributes on each edge
-    num_bins : int
-        number of bins; for example, if `num_bins=36` is provided, then each
-        bin will represent 10 degrees around the compass
-    min_length : float
-        ignore edges with `length` attributes less than `min_length`; useful
-        to ignore the noise of many very short edges
-    weight : string
-        if not None, weight edges' bearings by this (non-null) edge attribute.
-        for example, if "length" is provided, this will return 1 bearing
-        observation per meter per street, which could result in a very large
-        `bearings` array.
+    G
+        Unprojected graph with `bearing` attributes on each edge.
+    num_bins
+        Number of bins. For example, if `num_bins=36` is provided, then each
+        bin will represent 10 degrees around the compass.
+    min_length
+        Ignore edges with "length" attributes less than `min_length`. Useful
+        to ignore the noise of many very short edges.
+    weight
+        If None, apply equal weight for each bearing. Otherwise, weight edges'
+        bearings by this (non-null) edge attribute. For example, if "length"
+        is provided, each edge's bearing observation will be weighted by its
+        "length" attribute value.
 
     Returns
     -------
-    entropy : float
-        the graph's orientation entropy
+    entropy
+        The orientation entropy of `G`.
     """
     # check if we were able to import scipy
     if scipy is None:  # pragma: no cover
-        msg = "scipy must be installed to calculate entropy"
+        msg = "scipy must be installed as an optional dependency to calculate entropy."
         raise ImportError(msg)
-    bin_counts, _ = _bearings_distribution(Gu, num_bins, min_length, weight)
-    return scipy.stats.entropy(bin_counts)
-
-
-def _extract_edge_bearings(Gu, min_length=0, weight=None):
-    """
-    Extract undirected graph's bidirectional edge bearings.
-
-    For example, if an edge has a bearing of 90 degrees then we will record
+    bin_counts, _ = _bearings_distribution(G, num_bins, min_length, weight)
+    entropy: float = scipy.stats.entropy(bin_counts)
+    return entropy
+
+
+def _extract_edge_bearings(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    min_length: float,
+    weight: str | None,
+) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
+    """
+    Extract graph's edge bearings.
+
+    Ignores self-loop edges as their bearings are undefined. If `G` is a
+    MultiGraph, all edge bearings will be bidirectional (ie, two reciprocal
+    bearings per undirected edge). If `G` is a MultiDiGraph, all edge bearings
+    will be directional (ie, one bearing per directed edge). For example, if
+    an undirected edge has a bearing of 90 degrees then we will record
     bearings of both 90 degrees and 270 degrees for this edge.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected, unprojected graph with `bearing` attributes on each edge
-    min_length : float
-        ignore edges with `length` attributes less than `min_length`; useful
-        to ignore the noise of many very short edges
-    weight : string
-        if not None, weight edges' bearings by this (non-null) edge attribute.
-        for example, if "length" is provided, this will return 1 bearing
-        observation per meter per street, which could result in a very large
-        `bearings` array.
+    G
+        Unprojected graph with `bearing` attributes on each edge.
+    min_length
+        Ignore edges with `length` attributes less than `min_length`. Useful
+        to ignore the noise of many very short edges.
+    weight
+        If None, apply equal weight for each bearing. Otherwise, weight edges'
+        bearings by this (non-null) edge attribute. For example, if "length"
+        is provided, each edge's bearing observation will be weighted by its
+        "length" attribute value.
 
     Returns
     -------
-    bearings : numpy.array
-        the graph's bidirectional edge bearings
+    bearings, weights
+        The edge bearings of `G` and their corresponding weights.
     """
-    if nx.is_directed(Gu) or projection.is_projected(Gu.graph["crs"]):  # pragma: no cover
-        msg = "graph must be undirected and unprojected to analyze edge bearings"
+    if projection.is_projected(G.graph["crs"]):  # pragma: no cover
+        msg = "Graph must be unprojected to analyze edge bearings."
         raise ValueError(msg)
     bearings = []
-    for u, v, data in Gu.edges(data=True):
+    weights = []
+    for u, v, data in G.edges(data=True):
         # ignore self-loops and any edges below min_length
         if u != v and data["length"] >= min_length:
-            if weight:
-                # weight edges' bearings by some edge attribute value
-                bearings.extend([data["bearing"]] * int(data[weight]))
-            else:
-                # don't weight bearings, just take one value per edge
-                bearings.append(data["bearing"])
-
-    # drop any nulls, calculate reverse bearings, concatenate and return
-    bearings = np.array(bearings)
-    bearings = bearings[~np.isnan(bearings)]
-    bearings_r = (bearings - 180) % 360
-    return np.concatenate([bearings, bearings_r])
+            bearings.append(data["bearing"])
+            weights.append(data[weight] if weight is not None else 1.0)
+
+    # drop any nulls
+    bearings_array = np.array(bearings)
+    weights_array = np.array(weights)
+    keep_idx = ~np.isnan(bearings_array)
+    bearings_array = bearings_array[keep_idx]
+    weights_array = weights_array[keep_idx]
+    if nx.is_directed(G):
+        msg = (
+            "`G` is a MultiDiGraph, so edge bearings will be directional (one per "
+            "edge). If you want bidirectional edge bearings (two reciprocal bearings "
+            "per edge), pass a MultiGraph instead. Use `convert.to_undirected`."
+        )
+        warn(msg, category=UserWarning, stacklevel=2)
+        return bearings_array, weights_array
+    # for undirected graphs, add reverse bearings
+    bearings_array = np.concatenate([bearings_array, (bearings_array - 180) % 360])
+    weights_array = np.concatenate([weights_array, weights_array])
+    return bearings_array, weights_array
 
 
-def _bearings_distribution(Gu, num_bins, min_length=0, weight=None):
+def _bearings_distribution(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    num_bins: int,
+    min_length: float,
+    weight: str | None,
+) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     """
     Compute distribution of bearings across evenly spaced bins.
 
     Prevents bin-edge effects around common values like 0 degrees and 90
     degrees by initially creating twice as many bins as desired, then merging
     them in pairs. For example, if `num_bins=36` is provided, then each bin
     will represent 10 degrees around the compass, with the first bin
     representing 355 degrees to 5 degrees.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected, unprojected graph with `bearing` attributes on each edge
-    num_bins : int
-        number of bins for the bearings histogram
-    min_length : float
-        ignore edges with `length` attributes less than `min_length`; useful
-        to ignore the noise of many very short edges
-    weight : string
-        if not None, weight edges' bearings by this (non-null) edge attribute.
-        for example, if "length" is provided, this will return 1 bearing
-        observation per meter per street, which could result in a very large
-        `bearings` array.
-
-    Returns
-    -------
-    bin_counts, bin_edges : tuple of numpy.array
-        counts of bearings per bin and the bins edges
-    """
-    n = num_bins * 2
-    bins = np.arange(n + 1) * 360 / n
-
-    bearings = _extract_edge_bearings(Gu, min_length, weight)
-    count, bin_edges = np.histogram(bearings, bins=bins)
-
-    # move last bin to front, so eg 0.01 degrees and 359.99 degrees will be
-    # binned together
-    count = np.roll(count, 1)
-    bin_counts = count[::2] + count[1::2]
-
-    # because we merged the bins, their edges are now only every other one
-    bin_edges = bin_edges[range(0, len(bin_edges), 2)]
-    return bin_counts, bin_edges
-
-
-def plot_orientation(
-    Gu,
-    num_bins=36,
-    min_length=0,
-    weight=None,
-    ax=None,
-    figsize=(5, 5),
-    area=True,
-    color="#003366",
-    edgecolor="k",
-    linewidth=0.5,
-    alpha=0.7,
-    title=None,
-    title_y=1.05,
-    title_font=None,
-    xtick_font=None,
-):
-    """
-    Do not use: deprecated.
-
-    The plot_orientation function moved to the plot module. Calling it via the
-    bearing module will raise an error starting in the v2.0.0 release.
-
-    Parameters
-    ----------
-    Gu : networkx.MultiGraph
-        deprecated, do not use
-    num_bins : int
-        deprecated, do not use
-    min_length : float
-        deprecated, do not use
-    weight : string
-        deprecated, do not use
-    ax : matplotlib.axes.PolarAxesSubplot
-        deprecated, do not use
-    figsize : tuple
-        deprecated, do not use
-    area : bool
-        deprecated, do not use
-    color : string
-        deprecated, do not use
-    edgecolor : string
-        deprecated, do not use
-    linewidth : float
-        deprecated, do not use
-    alpha : float
-        deprecated, do not use
-    title : string
-        deprecated, do not use
-    title_y : float
-        deprecated, do not use
-    title_font : dict
-        deprecated, do not use
-    xtick_font : dict
-        deprecated, do not use
+    G
+        Unprojected graph with `bearing` attributes on each edge.
+    num_bins
+        Number of bins for the bearing histogram.
+    min_length
+        Ignore edges with `length` attributes less than `min_length`. Useful
+        to ignore the noise of many very short edges.
+    weight
+        If None, apply equal weight for each bearing. Otherwise, weight edges'
+        bearings by this (non-null) edge attribute. For example, if "length"
+        is provided, each edge's bearing observation will be weighted by its
+        "length" attribute value.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
-    """
-    warn(
-        "The `plot_orientation` function moved to the `plot` module. Calling it "
-        "via the `bearing` module will raise an exception starting with the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return plot.plot_orientation(
-        Gu,
-        num_bins=num_bins,
-        min_length=min_length,
-        weight=weight,
-        ax=ax,
-        figsize=figsize,
-        area=area,
-        color=color,
-        edgecolor=edgecolor,
-        linewidth=linewidth,
-        alpha=alpha,
-        title=title,
-        title_y=title_y,
-        title_font=title_font,
-        xtick_font=xtick_font,
+    bin_counts, bin_centers
+        Counts of bearings per bin and the bins' centers in degrees. Both
+        arrays are of length `num_bins`.
+    """
+    # Split bins in half to prevent bin-edge effects around common values.
+    # Bins will be merged in pairs after the histogram is computed. The last
+    # bin edge is the same as the first (i.e., 0 degrees = 360 degrees).
+    num_split_bins = num_bins * 2
+    split_bin_edges = np.arange(num_split_bins + 1) * 360 / num_split_bins
+
+    bearings, weights = _extract_edge_bearings(G, min_length, weight)
+    split_bin_counts, split_bin_edges = np.histogram(
+        bearings,
+        bins=split_bin_edges,
+        weights=weights,
     )
+
+    # Move last bin to front, so eg 0.01 degrees and 359.99 degrees will be
+    # binned together. Then combine counts from pairs of split bins.
+    split_bin_counts = np.roll(split_bin_counts, 1)
+    bin_counts = split_bin_counts[::2] + split_bin_counts[1::2]
+
+    # Every other edge of the split bins is the center of a merged bin.
+    bin_centers = split_bin_edges[range(0, num_split_bins - 1, 2)]
+    return bin_counts, bin_centers
```

### Comparing `osmnx-1.9.3/osmnx/convert.py` & `osmnx-2.0.0b0/osmnx/convert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,192 @@
 """Convert spatial graphs to/from different data types."""
 
+from __future__ import annotations
+
 import itertools
+import logging as lg
+from typing import Any
+from typing import Literal
+from typing import overload
 from warnings import warn
 
 import geopandas as gpd
 import networkx as nx
 import pandas as pd
-from shapely.geometry import LineString
-from shapely.geometry import Point
+from shapely import LineString
+from shapely import Point
 
 from . import utils
 
 
-def graph_to_gdfs(G, nodes=True, edges=True, node_geometry=True, fill_edge_geometry=True):
+# nodes and edges are both missing (therefore both default true)
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]: ...
+
+
+# both present/True
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: Literal[True],
+    edges: Literal[True],
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]: ...
+
+
+# both present, nodes true, edges false
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: Literal[True],
+    edges: Literal[False],
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> gpd.GeoDataFrame: ...
+
+
+# both present, nodes false, edges true
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: Literal[False],
+    edges: Literal[True],
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> gpd.GeoDataFrame: ...
+
+
+# nodes missing (therefore default true), edges present/true
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    edges: Literal[True],
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]: ...
+
+
+# nodes missing (therefore default true), edges present/false
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    edges: Literal[False],
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> gpd.GeoDataFrame: ...
+
+
+# nodes present/true, edges missing (therefore default true)
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: Literal[True],
+    edges: bool = True,
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]: ...
+
+
+# nodes present/false, edges missing (therefore default true)
+@overload
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: Literal[False],
+    edges: bool = True,
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> gpd.GeoDataFrame: ...
+
+
+def graph_to_gdfs(
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    nodes: bool = True,
+    edges: bool = True,
+    node_geometry: bool = True,
+    fill_edge_geometry: bool = True,
+) -> gpd.GeoDataFrame | tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
     """
-    Convert a MultiDiGraph to node and/or edge GeoDataFrames.
+    Convert a MultiGraph or MultiDiGraph to node and/or edge GeoDataFrames.
 
     This function is the inverse of `graph_from_gdfs`.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    nodes : bool
-        if True, convert graph nodes to a GeoDataFrame and return it
-    edges : bool
-        if True, convert graph edges to a GeoDataFrame and return it
-    node_geometry : bool
-        if True, create a geometry column from node x and y attributes
-    fill_edge_geometry : bool
-        if True, fill in missing edge geometry fields using nodes u and v
+    G
+        Input graph.
+    nodes
+        If True, convert graph nodes to a GeoDataFrame and return it.
+    edges
+        If True, convert graph edges to a GeoDataFrame and return it.
+    node_geometry
+        If True, create a geometry column from node "x" and "y" attributes.
+    fill_edge_geometry
+        If True, fill missing edge geometry fields using endpoint nodes'
+        coordinates to create a LineString.
 
     Returns
     -------
-    geopandas.GeoDataFrame or tuple
-        gdf_nodes or gdf_edges or tuple of (gdf_nodes, gdf_edges). gdf_nodes
-        is indexed by osmid and gdf_edges is multi-indexed by u, v, key
-        following normal MultiDiGraph structure.
+    gdf_nodes or gdf_edges or (gdf_nodes, gdf_edges)
+        `gdf_nodes` is indexed by `osmid` and `gdf_edges` is multi-indexed by
+        `(u, v, key)` following normal MultiGraph/MultiDiGraph structure.
     """
     crs = G.graph["crs"]
 
     if nodes:
-        if not G.nodes:  # pragma: no cover
-            msg = "graph contains no nodes"
+        if len(G.nodes) == 0:  # pragma: no cover
+            msg = "Graph contains no nodes."
             raise ValueError(msg)
 
         uvk, data = zip(*G.nodes(data=True))
 
         if node_geometry:
             # convert node x/y attributes to Points for geometry column
             node_geoms = (Point(d["x"], d["y"]) for d in data)
             gdf_nodes = gpd.GeoDataFrame(data, index=uvk, crs=crs, geometry=list(node_geoms))
         else:
             gdf_nodes = gpd.GeoDataFrame(data, index=uvk)
 
         gdf_nodes.index = gdf_nodes.index.rename("osmid")
-        utils.log("Created nodes GeoDataFrame from graph")
+        msg = "Created nodes GeoDataFrame from graph"
+        utils.log(msg, level=lg.INFO)
 
     if edges:
-        if not G.edges:  # pragma: no cover
-            msg = "Graph contains no edges"
+        if len(G.edges) == 0:  # pragma: no cover
+            msg = "Graph contains no edges."
             raise ValueError(msg)
 
         u, v, k, data = zip(*G.edges(keys=True, data=True))
 
         if fill_edge_geometry:
             # subroutine to get geometry for every edge: if edge already has
             # geometry return it, otherwise create it using the incident nodes
             x_lookup = nx.get_node_attributes(G, "x")
             y_lookup = nx.get_node_attributes(G, "y")
 
-            def _make_edge_geometry(u, v, data, x=x_lookup, y=y_lookup):
+            def _make_edge_geometry(
+                u: int,
+                v: int,
+                data: dict[str, Any],
+                x: dict[int, float] = x_lookup,
+                y: dict[int, float] = y_lookup,
+            ) -> LineString:
                 if "geometry" in data:
                     return data["geometry"]
 
                 # otherwise
                 return LineString((Point((x[u], y[u])), Point((x[v], y[v]))))
 
             edge_geoms = map(_make_edge_geometry, u, v, data)
@@ -89,82 +201,92 @@
 
         # add u, v, key attributes as index
         gdf_edges["u"] = u
         gdf_edges["v"] = v
         gdf_edges["key"] = k
         gdf_edges = gdf_edges.set_index(["u", "v", "key"])
 
-        utils.log("Created edges GeoDataFrame from graph")
+        msg = "Created edges GeoDataFrame from graph"
+        utils.log(msg, level=lg.INFO)
 
     if nodes and edges:
         return gdf_nodes, gdf_edges
 
     if nodes:
         return gdf_nodes
 
     if edges:
         return gdf_edges
 
     # otherwise
-    msg = "you must request nodes or edges or both"
+    msg = "You must request nodes or edges or both."
     raise ValueError(msg)
 
 
-def graph_from_gdfs(gdf_nodes, gdf_edges, graph_attrs=None):
+def graph_from_gdfs(
+    gdf_nodes: gpd.GeoDataFrame,
+    gdf_edges: gpd.GeoDataFrame,
+    *,
+    graph_attrs: dict[str, Any] | None = None,
+) -> nx.MultiDiGraph:
     """
     Convert node and edge GeoDataFrames to a MultiDiGraph.
 
     This function is the inverse of `graph_to_gdfs` and is designed to work in
-    conjunction with it.
+    conjunction with it. However, you can convert arbitrary node and edge
+    GeoDataFrames as long as 1) `gdf_nodes` is uniquely indexed by `osmid`, 2)
+    `gdf_nodes` contains `x` and `y` coordinate columns representing node
+    geometries, 3) `gdf_edges` is uniquely multi-indexed by `(u, v, key)`
+    (following normal MultiDiGraph structure). This allows you to load any
+    node/edge Shapefiles or GeoPackage layers as GeoDataFrames then convert
+    them to a MultiDiGraph for network analysis.
 
-    However, you can convert arbitrary node and edge GeoDataFrames as long as
-    1) `gdf_nodes` is uniquely indexed by `osmid`, 2) `gdf_nodes` contains `x`
-    and `y` coordinate columns representing node geometries, 3) `gdf_edges` is
-    uniquely multi-indexed by `u`, `v`, `key` (following normal MultiDiGraph
-    structure). This allows you to load any node/edge shapefiles or GeoPackage
-    layers as GeoDataFrames then convert them to a MultiDiGraph for graph
-    analysis. Note that any `geometry` attribute on `gdf_nodes` is discarded
-    since `x` and `y` provide the necessary node geometry information instead.
+    Note that any `geometry` attribute on `gdf_nodes` is discarded, since `x`
+    and `y` provide the necessary node geometry information instead.
 
     Parameters
     ----------
-    gdf_nodes : geopandas.GeoDataFrame
-        GeoDataFrame of graph nodes uniquely indexed by osmid
-    gdf_edges : geopandas.GeoDataFrame
-        GeoDataFrame of graph edges uniquely multi-indexed by u, v, key
-    graph_attrs : dict
-        the new G.graph attribute dict. if None, use crs from gdf_edges as the
-        only graph-level attribute (gdf_edges must have crs attribute set)
+    gdf_nodes
+        GeoDataFrame of graph nodes uniquely indexed by `osmid`.
+    gdf_edges
+        GeoDataFrame of graph edges uniquely multi-indexed by `(u, v, key)`.
+    graph_attrs
+        The new `G.graph` attribute dictionary. If None, use `gdf_edges`'s CRS
+        as the only graph-level attribute (`gdf_edges` must have its `crs`
+        attribute set).
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     if not ("x" in gdf_nodes.columns and "y" in gdf_nodes.columns):  # pragma: no cover
-        msg = "gdf_nodes must contain x and y columns"
+        msg = "`gdf_nodes` must contain 'x' and 'y' columns."
+        raise ValueError(msg)
+
+    if not hasattr(gdf_nodes, "geometry"):
+        msg = "`gdf_nodes` must have a 'geometry' attribute."
         raise ValueError(msg)
 
-    # if gdf_nodes has a geometry attribute set, drop that column (as we use x
-    # and y for geometry information) and warn the user if the geometry values
-    # differ from the coordinates in the x and y columns
-    if hasattr(gdf_nodes, "geometry"):
-        try:
-            all_x_match = (gdf_nodes.geometry.x == gdf_nodes["x"]).all()
-            all_y_match = (gdf_nodes.geometry.y == gdf_nodes["y"]).all()
-            assert all_x_match
-            assert all_y_match
-        except (AssertionError, ValueError):  # pragma: no cover
-            # AssertionError if x/y coords don't match geometry column
-            # ValueError if geometry column contains non-point geometry types
-            warn(
-                "discarding the gdf_nodes geometry column, though its "
-                "values differ from the coordinates in the x and y columns",
-                stacklevel=2,
-            )
-        gdf_nodes = gdf_nodes.drop(columns=gdf_nodes.geometry.name)
+    # drop geometry column from gdf_nodes (as we use x and y for geometry
+    # information), but warn the user if the geometry values differ from the
+    # coordinates in the x and y columns. this results in a df instead of gdf.
+    msg = (
+        "Discarding the `gdf_nodes` 'geometry' column, though its values "
+        "differ from the coordinates in the 'x' and 'y' columns."
+    )
+    try:
+        all_x_match = (gdf_nodes.geometry.x == gdf_nodes["x"]).all()
+        all_y_match = (gdf_nodes.geometry.y == gdf_nodes["y"]).all()
+        if not (all_x_match and all_y_match):
+            # warn if x/y coords don't match geometry column
+            warn(msg, category=UserWarning, stacklevel=2)
+    except ValueError:  # pragma: no cover
+        # warn if geometry column contains non-point geometry types
+        warn(msg, category=UserWarning, stacklevel=2)
+    df_nodes = gdf_nodes.drop(columns=gdf_nodes.geometry.name)
 
     # create graph and add graph-level attribute dict
     if graph_attrs is None:
         graph_attrs = {"crs": gdf_edges.crs}
     G = nx.MultiDiGraph(**graph_attrs)
 
     # add edges and their attributes to graph, but filter out null attribute
@@ -172,76 +294,78 @@
     attr_names = gdf_edges.columns.to_list()
     for (u, v, k), attr_vals in zip(gdf_edges.index, gdf_edges.to_numpy()):
         data_all = zip(attr_names, attr_vals)
         data = {name: val for name, val in data_all if isinstance(val, list) or pd.notna(val)}
         G.add_edge(u, v, key=k, **data)
 
     # add any nodes with no incident edges, since they wouldn't be added above
-    G.add_nodes_from(set(gdf_nodes.index) - set(G.nodes))
+    G.add_nodes_from(set(df_nodes.index) - set(G.nodes))
 
     # now all nodes are added, so set nodes' attributes
-    for col in gdf_nodes.columns:
-        nx.set_node_attributes(G, name=col, values=gdf_nodes[col].dropna())
+    for col in df_nodes.columns:
+        nx.set_node_attributes(G, name=col, values=df_nodes[col].dropna())
 
-    utils.log("Created graph from node/edge GeoDataFrames")
+    msg = "Created graph from node/edge GeoDataFrames"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
-def to_digraph(G, weight="length"):
+def to_digraph(G: nx.MultiDiGraph, *, weight: str = "length") -> nx.DiGraph:
     """
     Convert MultiDiGraph to DiGraph.
 
-    Chooses between parallel edges by minimizing `weight` attribute value.
-    Note: see also `to_undirected` to convert MultiDiGraph to MultiGraph.
+    Chooses between parallel edges by minimizing `weight` attribute value. See
+    also `to_undirected` to convert MultiDiGraph to MultiGraph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    weight : string
-        attribute value to minimize when choosing between parallel edges
+    G
+        Input graph.
+    weight
+        Attribute value to minimize when choosing between parallel edges.
 
     Returns
     -------
-    networkx.DiGraph
+    G
     """
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
-    to_remove = []
+    to_remove: list[tuple[int, int, int]] = []
 
     # identify all the parallel edges in the MultiDiGraph
-    parallels = ((u, v) for u, v in G.edges(keys=False) if len(G.get_edge_data(u, v)) > 1)
+    parallels = ((u, v) for u, v in G.edges(keys=False) if G.number_of_edges(u, v) > 1)
 
     # among all sets of parallel edges, remove all except the one with the
     # minimum "weight" attribute value
     for u, v in set(parallels):
         k_min, _ = min(G.get_edge_data(u, v).items(), key=lambda x: x[1][weight])
         to_remove.extend((u, v, k) for k in G[u][v] if k != k_min)
 
     G.remove_edges_from(to_remove)
-    utils.log("Converted MultiDiGraph to DiGraph")
+    msg = "Converted MultiDiGraph to DiGraph"
+    utils.log(msg, level=lg.INFO)
 
     return nx.DiGraph(G)
 
 
-def to_undirected(G):
+def to_undirected(G: nx.MultiDiGraph) -> nx.MultiGraph:
     """
     Convert MultiDiGraph to undirected MultiGraph.
 
-    Maintains parallel edges only if their geometries differ. Note: see also
+    Maintains parallel edges only if their geometries differ. See also
     `to_digraph` to convert MultiDiGraph to DiGraph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    networkx.MultiGraph
+    Gu
     """
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
 
     # set from/to nodes before making graph undirected
     for u, v, d in G.edges(data=True):
         d["from"] = u
@@ -255,55 +379,56 @@
 
     # increment parallel edges' keys so we don't retain only one edge of sets
     # of true parallel edges when we convert from MultiDiGraph to MultiGraph
     G = _update_edge_keys(G)
 
     # convert MultiDiGraph to MultiGraph, retaining edges in both directions
     # of parallel edges and self-loops for now
-    H = nx.MultiGraph(**G.graph)
-    H.add_nodes_from(G.nodes(data=True))
-    H.add_edges_from(G.edges(keys=True, data=True))
+    Gu = nx.MultiGraph(**G.graph)
+    Gu.add_nodes_from(G.nodes(data=True))
+    Gu.add_edges_from(G.edges(keys=True, data=True))
 
     # the previous operation added all directed edges from G as undirected
-    # edges in H. we now have duplicate edges for every bidirectional parallel
+    # edges in Gu. we now have duplicate edges for each bidirectional parallel
     # edge or self-loop. so, look through the edges and remove any duplicates.
     duplicate_edges = set()
-    for u1, v1, key1, data1 in H.edges(keys=True, data=True):
+    for u1, v1, key1, data1 in Gu.edges(keys=True, data=True):
         # if we haven't already flagged this edge as a duplicate
         if (u1, v1, key1) not in duplicate_edges:
             # look at every other edge between u and v, one at a time
-            for key2 in H[u1][v1]:
+            for key2 in Gu[u1][v1]:
                 # don't compare this edge to itself
                 if key1 != key2:
                     # compare the first edge's data to the second's
                     # if they match up, flag the duplicate for removal
-                    data2 = H.edges[u1, v1, key2]
+                    data2 = Gu.edges[u1, v1, key2]
                     if _is_duplicate_edge(data1, data2):
                         duplicate_edges.add((u1, v1, key2))
 
-    H.remove_edges_from(duplicate_edges)
-    utils.log("Converted MultiDiGraph to undirected MultiGraph")
+    Gu.remove_edges_from(duplicate_edges)
+    msg = "Converted MultiDiGraph to undirected MultiGraph"
+    utils.log(msg, level=lg.INFO)
 
-    return H
+    return Gu
 
 
-def _is_duplicate_edge(data1, data2):
+def _is_duplicate_edge(data1: dict[str, Any], data2: dict[str, Any]) -> bool:
     """
-    Check if two graph edge data dicts have the same osmid and geometry.
+    Check if two graph edge data dicts have the same `osmid` and `geometry`.
 
     Parameters
     ----------
-    data1: dict
-        the first edge's data
-    data2 : dict
-        the second edge's data
+    data1
+        The first edge's attribute data.
+    data2
+        The second edge's attribute data.
 
     Returns
     -------
-    is_dupe : bool
+    is_dupe
     """
     is_dupe = False
 
     # if either edge's osmid contains multiple values (due to simplification)
     # compare them as sets to see if they contain the same values
     osmid1 = set(data1["osmid"]) if isinstance(data1["osmid"], list) else data1["osmid"]
     osmid2 = set(data2["osmid"]) if isinstance(data2["osmid"], list) else data2["osmid"]
@@ -322,65 +447,65 @@
         # if one edge has geometry attribute but the other doesn't: not dupes
         else:
             pass
 
     return is_dupe
 
 
-def _is_same_geometry(ls1, ls2):
+def _is_same_geometry(ls1: LineString, ls2: LineString) -> bool:
     """
     Determine if two LineString geometries are the same (in either direction).
 
     Check both the normal and reversed orders of their constituent points.
 
     Parameters
     ----------
-    ls1 : shapely.geometry.LineString
-        the first LineString geometry
-    ls2 : shapely.geometry.LineString
-        the second LineString geometry
+    ls1
+        The first LineString geometry.
+    ls2
+        The second LineString geometry.
 
     Returns
     -------
-    bool
+    is_same
     """
     # extract coordinates from each LineString geometry
     geom1 = [tuple(coords) for coords in ls1.xy]
     geom2 = [tuple(coords) for coords in ls2.xy]
 
     # reverse the first LineString's coordinates' direction
     geom1_r = [tuple(reversed(coords)) for coords in ls1.xy]
 
     # if second geometry matches first in either direction, return True
-    return geom2 in (geom1, geom1_r)  # noqa: PLR6201
+    return geom2 in (geom1, geom1_r)
 
 
-def _update_edge_keys(G):
+def _update_edge_keys(G: nx.MultiDiGraph) -> nx.MultiDiGraph:
     """
     Increment key of one edge of parallel edges that differ in geometry.
 
-    For example, two streets from u to v that bow away from each other as
+    For example, two streets from `u` to `v` that bow away from each other as
     separate streets, rather than opposite direction edges of a single street.
-    Increment one of these edge's keys so that they do not match across u, v,
-    k or v, u, k so we can add both to an undirected MultiGraph.
+    Increment one of these edge's keys so that they do not match across
+    `(u, v, k)` or `(v, u, k)` so we can add both to an undirected MultiGraph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     # identify all the edges that are duplicates based on a sorted combination
     # of their origin, destination, and key. that is, edge uv will match edge vu
     # as a duplicate, but only if they have the same key
     edges = graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
-    edges["uvk"] = ["_".join(sorted([str(u), str(v)]) + [str(k)]) for u, v, k in edges.index]
+    edges["uvk"] = ["_".join([*sorted([str(u), str(v)]), str(k)]) for u, v, k in edges.index]
     mask = edges["uvk"].duplicated(keep=False)
     dupes = edges[mask].dropna(subset=["geometry"])
 
     different_streets = []
     groups = dupes[["geometry", "uvk"]].groupby("uvk")
 
     # for each group of duplicate edges
```

### Comparing `osmnx-1.9.3/osmnx/distance.py` & `osmnx-2.0.0b0/osmnx/distance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,499 +1,534 @@
-"""Calculate distances and find nearest node/edge(s) to point(s)."""
+"""Calculate distances and find nearest graph node/edge(s) to point(s)."""
 
-from warnings import warn
+from __future__ import annotations
+
+import logging as lg
+from collections.abc import Iterable
+from typing import Literal
+from typing import overload
 
 import networkx as nx
 import numpy as np
-import pandas as pd
-from shapely.geometry import Point
+import numpy.typing as npt
+from shapely import Point
 from shapely.strtree import STRtree
 
 from . import convert
 from . import projection
-from . import routing
 from . import utils
-from . import utils_geo
 
 # scipy is optional dependency for projected nearest-neighbor search
 try:
     from scipy.spatial import cKDTree
 except ImportError:  # pragma: no cover
-    cKDTree = None
+    cKDTree = None  # noqa: N816
 
 # scikit-learn is optional dependency for unprojected nearest-neighbor search
 try:
     from sklearn.neighbors import BallTree
 except ImportError:  # pragma: no cover
     BallTree = None
 
 EARTH_RADIUS_M = 6_371_009
 
 
-def great_circle(lat1, lon1, lat2, lon2, earth_radius=EARTH_RADIUS_M):
+# if coords are all floats, return float
+@overload
+def great_circle(lat1: float, lon1: float, lat2: float, lon2: float) -> float: ...
+
+
+# if coords are all floats (and optional arg is provided), return float
+@overload
+def great_circle(
+    lat1: float,
+    lon1: float,
+    lat2: float,
+    lon2: float,
+    earth_radius: float,
+) -> float: ...
+
+
+# if coords are all arrays, return array
+@overload
+def great_circle(
+    lat1: npt.NDArray[np.float64],
+    lon1: npt.NDArray[np.float64],
+    lat2: npt.NDArray[np.float64],
+    lon2: npt.NDArray[np.float64],
+) -> npt.NDArray[np.float64]: ...
+
+
+# if coords are all arrays (and optional arg is provided), return array
+@overload
+def great_circle(
+    lat1: npt.NDArray[np.float64],
+    lon1: npt.NDArray[np.float64],
+    lat2: npt.NDArray[np.float64],
+    lon2: npt.NDArray[np.float64],
+    earth_radius: float,
+) -> npt.NDArray[np.float64]: ...
+
+
+def great_circle(
+    lat1: float | npt.NDArray[np.float64],
+    lon1: float | npt.NDArray[np.float64],
+    lat2: float | npt.NDArray[np.float64],
+    lon2: float | npt.NDArray[np.float64],
+    earth_radius: float = EARTH_RADIUS_M,
+) -> float | npt.NDArray[np.float64]:
     """
     Calculate great-circle distances between pairs of points.
 
     Vectorized function to calculate the great-circle distance between two
     points' coordinates or between arrays of points' coordinates using the
     haversine formula. Expects coordinates in decimal degrees.
 
     Parameters
     ----------
-    lat1 : float or numpy.array of float
-        first point's latitude coordinate
-    lon1 : float or numpy.array of float
-        first point's longitude coordinate
-    lat2 : float or numpy.array of float
-        second point's latitude coordinate
-    lon2 : float or numpy.array of float
-        second point's longitude coordinate
-    earth_radius : float
-        earth's radius in units in which distance will be returned (default is
-        meters)
+    lat1
+        First point's latitude coordinate(s).
+    lon1
+        First point's longitude coordinate(s).
+    lat2
+        Second point's latitude coordinate(s).
+    lon2
+        Second point's longitude coordinate(s).
+    earth_radius
+        Earth's radius in units in which distance will be returned (default
+        represents meters).
 
     Returns
     -------
-    dist : float or numpy.array of float
-        distance from each (lat1, lon1) to each (lat2, lon2) in units of
-        earth_radius
+    dist
+        Distance from each `(lat1, lon1)` point to each `(lat2, lon2)` point
+        in units of `earth_radius`.
     """
     y1 = np.deg2rad(lat1)
     y2 = np.deg2rad(lat2)
     delta_y = y2 - y1
 
     x1 = np.deg2rad(lon1)
     x2 = np.deg2rad(lon2)
     delta_x = x2 - x1
 
     h = np.sin(delta_y / 2) ** 2 + np.cos(y1) * np.cos(y2) * np.sin(delta_x / 2) ** 2
     h = np.minimum(1, h)  # protect against floating point errors
     arc = 2 * np.arcsin(np.sqrt(h))
 
     # return distance in units of earth_radius
-    return arc * earth_radius
+    dist: float | npt.NDArray[np.float64] = arc * earth_radius
+    return dist
 
 
-def euclidean(y1, x1, y2, x2):
+# if coords are all floats, return float
+@overload
+def euclidean(y1: float, x1: float, y2: float, x2: float) -> float: ...
+
+
+# if coords are all arrays, return array
+@overload
+def euclidean(
+    y1: npt.NDArray[np.float64],
+    x1: npt.NDArray[np.float64],
+    y2: npt.NDArray[np.float64],
+    x2: npt.NDArray[np.float64],
+) -> npt.NDArray[np.float64]: ...
+
+
+def euclidean(
+    y1: float | npt.NDArray[np.float64],
+    x1: float | npt.NDArray[np.float64],
+    y2: float | npt.NDArray[np.float64],
+    x2: float | npt.NDArray[np.float64],
+) -> float | npt.NDArray[np.float64]:
     """
     Calculate Euclidean distances between pairs of points.
 
     Vectorized function to calculate the Euclidean distance between two
     points' coordinates or between arrays of points' coordinates. For accurate
     results, use projected coordinates rather than decimal degrees.
 
     Parameters
     ----------
-    y1 : float or numpy.array of float
-        first point's y coordinate
-    x1 : float or numpy.array of float
-        first point's x coordinate
-    y2 : float or numpy.array of float
-        second point's y coordinate
-    x2 : float or numpy.array of float
-        second point's x coordinate
+    y1
+        First point's y coordinate(s).
+    x1
+        First point's x coordinate(s).
+    y2
+        Second point's y coordinate(s).
+    x2
+        Second point's x coordinate(s).
 
     Returns
     -------
-    dist : float or numpy.array of float
-        distance from each (x1, y1) to each (x2, y2) in coordinates' units
+    dist
+        Distance from each `(x1, y1)` point to each `(x2, y2)` point in same
+        units as the points' coordinates.
     """
     # pythagorean theorem
-    return ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5
-
-
-def great_circle_vec(lat1, lng1, lat2, lng2, earth_radius=EARTH_RADIUS_M):
-    """
-    Do not use, deprecated.
-
-    The `great_circle_vec` function has been renamed `great_circle`. Calling
-    `great_circle_vec` will raise an error in the v2.0.0 release.
-
-    Parameters
-    ----------
-    lat1 : float or numpy.array of float
-        first point's latitude coordinate
-    lng1 : float or numpy.array of float
-        first point's longitude coordinate
-    lat2 : float or numpy.array of float
-        second point's latitude coordinate
-    lng2 : float or numpy.array of float
-        second point's longitude coordinate
-    earth_radius : float
-        earth's radius in units in which distance will be returned (default is
-        meters)
-
-    Returns
-    -------
-    dist : float or numpy.array of float
-        distance from each (lat1, lng1) to each (lat2, lng2) in units of
-        earth_radius
-    """
-    warn(
-        "The `great_circle_vec` function has been renamed `great_circle`. Calling "
-        "`great_circle_vec` will raise an error starting in the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return great_circle(lat1, lng1, lat2, lng2, earth_radius)
-
-
-def euclidean_dist_vec(y1, x1, y2, x2):
-    """
-    Do not use, deprecated.
-
-    The `euclidean_dist_vec` function has been renamed `euclidean`. Calling
-    `euclidean_dist_vec` will raise an error in the v2.0.0 release.
-
-    Parameters
-    ----------
-    y1 : float or numpy.array of float
-        first point's y coordinate
-    x1 : float or numpy.array of float
-        first point's x coordinate
-    y2 : float or numpy.array of float
-        second point's y coordinate
-    x2 : float or numpy.array of float
-        second point's x coordinate
-
-    Returns
-    -------
-    dist : float or numpy.array of float
-        distance from each (x1, y1) to each (x2, y2) in coordinates' units
-    """
-    warn(
-        "The `euclidean_dist_vec` function has been renamed `euclidean`. Calling "
-        "`euclidean_dist_vec` will raise an error starting in the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return euclidean(y1, x1, y2, x2)
+    dist: float | npt.NDArray[np.float64] = ((x1 - x2) ** 2 + (y1 - y2) ** 2) ** 0.5
+    return dist
 
 
-def add_edge_lengths(G, precision=None, edges=None):
+def add_edge_lengths(
+    G: nx.MultiDiGraph,
+    *,
+    edges: Iterable[tuple[int, int, int]] | None = None,
+) -> nx.MultiDiGraph:
     """
-    Add `length` attribute (in meters) to each edge.
+    Calculate and add `length` attribute (in meters) to each edge.
 
     Vectorized function to calculate great-circle distance between each edge's
-    incident nodes. Ensure graph is in unprojected coordinates, and
-    unsimplified to get accurate distances.
+    incident nodes. Ensure graph is unprojected and unsimplified to calculate
+    accurate distances.
 
     Note: this function is run by all the `graph.graph_from_x` functions
     automatically to add `length` attributes to all edges. It calculates edge
     lengths as the great-circle distance from node `u` to node `v`. When
     OSMnx automatically runs this function upon graph creation, it does it
     before simplifying the graph: thus it calculates the straight-line lengths
     of edge segments that are themselves all straight. Only after
-    simplification do edges take on a (potentially) curvilinear geometry. If
-    you wish to calculate edge lengths later, you are calculating
+    simplification do edges take on (potentially) curvilinear geometry. If you
+    wish to calculate edge lengths later, note that you will be calculating
     straight-line distances which necessarily ignore the curvilinear geometry.
-    You only want to run this function on a graph with all straight edges
+    Thus you only want to run this function on a graph with all straight edges
     (such as is the case with an unsimplified graph).
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        unprojected, unsimplified input graph
-    precision : int
-        deprecated, do not use
-    edges : tuple
-        tuple of (u, v, k) tuples representing subset of edges to add length
-        attributes to. if None, add lengths to all edges.
+    G
+        Unprojected and unsimplified input graph.
+    edges
+        The subset of edges to add `length` attributes to, as `(u, v, k)`
+        tuples. If None, add lengths to all edges.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with edge length attributes
+    G
+        Graph with `length` attributes on the edges.
     """
-    if precision is None:
-        precision = 3
-    else:
-        warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    uvk = tuple(G.edges) if edges is None else edges
+    uvk = G.edges if edges is None else edges
 
     # extract edge IDs and corresponding coordinates from their nodes
     x = G.nodes(data="x")
     y = G.nodes(data="y")
+    msg = "Some edges missing nodes, possibly due to input data clipping issue."
     try:
         # two-dimensional array of coordinates: y0, x0, y1, x1
         c = np.array([(y[u], x[u], y[v], x[v]) for u, v, k in uvk])
-        # ensure all coordinates can be converted to float and are non-null
-        assert not np.isnan(c.astype(float)).any()
-    except (AssertionError, KeyError) as e:  # pragma: no cover
-        msg = "some edges missing nodes, possibly due to input data clipping issue"
+    except KeyError as e:  # pragma: no cover
         raise ValueError(msg) from e
+    else:
+        # ensure all coordinates can be converted to float and are non-null
+        if np.isnan(c.astype(float)).any():
+            raise ValueError(msg)
 
     # calculate great circle distances, round, and fill nulls with zeros
-    dists = great_circle(c[:, 0], c[:, 1], c[:, 2], c[:, 3]).round(precision)
+    dists = great_circle(c[:, 0], c[:, 1], c[:, 2], c[:, 3])
     dists[np.isnan(dists)] = 0
     nx.set_edge_attributes(G, values=dict(zip(uvk, dists)), name="length")
 
-    utils.log("Added length attributes to graph edges")
+    msg = "Added length attributes to graph edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
-def nearest_nodes(G, X, Y, return_dist=False):
+# if X and Y are floats and return_dist is not provided (defaults False)
+@overload
+def nearest_nodes(G: nx.MultiDiGraph, X: float, Y: float) -> int: ...
+
+
+# if X and Y are floats and return_dist is provided/False
+@overload
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: float,
+    Y: float,
+    *,
+    return_dist: Literal[False],
+) -> int: ...
+
+
+# if X and Y are floats and return_dist is provided/True
+@overload
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: float,
+    Y: float,
+    *,
+    return_dist: Literal[True],
+) -> tuple[npt.NDArray[np.int64], npt.NDArray[np.float64]]: ...
+
+
+# if X and Y are iterable and return_dist is not provided (defaults False)
+@overload
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+) -> npt.NDArray[np.int64]: ...
+
+
+# if X and Y are iterable and return_dist is provided/False
+@overload
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+    *,
+    return_dist: Literal[False],
+) -> npt.NDArray[np.int64]: ...
+
+
+# if X and Y are iterable and return_dist is provided/True
+@overload
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+    *,
+    return_dist: Literal[True],
+) -> tuple[npt.NDArray[np.int64], npt.NDArray[np.float64]]: ...
+
+
+def nearest_nodes(
+    G: nx.MultiDiGraph,
+    X: float | Iterable[float],
+    Y: float | Iterable[float],
+    *,
+    return_dist: bool = False,
+) -> (
+    int
+    | npt.NDArray[np.int64]
+    | tuple[int, float]
+    | tuple[npt.NDArray[np.int64], npt.NDArray[np.float64]]
+):
     """
     Find the nearest node to a point or to each of several points.
 
     If `X` and `Y` are single coordinate values, this will return the nearest
-    node to that point. If `X` and `Y` are lists of coordinate values, this
-    will return the nearest node to each point.
+    node to that point. If `X` and `Y` are iterables of coordinate values,
+    this will return the nearest node to each point.
 
-    If the graph is projected, this uses a k-d tree for euclidean nearest
+    If the graph is projected, this uses a k-d tree for Euclidean nearest
     neighbor search, which requires that scipy is installed as an optional
     dependency. If it is unprojected, this uses a ball tree for haversine
     nearest neighbor search, which requires that scikit-learn is installed as
     an optional dependency.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        graph in which to find nearest nodes
-    X : float or list
-        points' x (longitude) coordinates, in same CRS/units as graph and
-        containing no nulls
-    Y : float or list
-        points' y (latitude) coordinates, in same CRS/units as graph and
-        containing no nulls
-    return_dist : bool
-        optionally also return distance between points and nearest nodes
+    G
+        Graph in which to find nearest nodes.
+    X
+        The points' x (longitude) coordinates, in same CRS/units as graph and
+        containing no nulls.
+    Y
+        The points' y (latitude) coordinates, in same CRS/units as graph and
+        containing no nulls.
+    return_dist
+        If True, optionally also return the distance(s) between point(s) and
+        nearest node(s).
 
     Returns
     -------
-    nn or (nn, dist) : int/list or tuple
-        nearest node IDs or optionally a tuple where `dist` contains distances
-        between the points and their nearest nodes
+    nn or (nn, dist)
+        Nearest node ID(s) or optionally a tuple of ID(s) and distance(s)
+        between each point and its nearest node.
     """
-    is_scalar = False
-    if not (hasattr(X, "__iter__") and hasattr(Y, "__iter__")):
-        # make coordinates arrays if user passed non-iterable values
+    # make coordinates arrays whether user passed iterable values or not
+    if not (isinstance(X, Iterable) and isinstance(Y, Iterable)):
         is_scalar = True
-        X = np.array([X])
-        Y = np.array([Y])
+        X_arr = np.array([X])
+        Y_arr = np.array([Y])
+    else:
+        is_scalar = False
+        X_arr = np.array(X)
+        Y_arr = np.array(Y)
 
-    if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
-        msg = "`X` and `Y` cannot contain nulls"
+    if np.isnan(X_arr).any() or np.isnan(Y_arr).any():  # pragma: no cover
+        msg = "`X` and `Y` cannot contain nulls."
         raise ValueError(msg)
+
     nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
+    nn_array: npt.NDArray[np.int64]
+    dist_array: npt.NDArray[np.float64]
 
     if projection.is_projected(G.graph["crs"]):
         # if projected, use k-d tree for euclidean nearest-neighbor search
         if cKDTree is None:  # pragma: no cover
-            msg = "scipy must be installed to search a projected graph"
+            msg = "scipy must be installed as an optional dependency to search a projected graph."
             raise ImportError(msg)
-        dist, pos = cKDTree(nodes).query(np.array([X, Y]).T, k=1)
-        nn = nodes.index[pos]
+        dist_array, pos = cKDTree(nodes).query(np.array([X_arr, Y_arr]).T, k=1)
+        nn_array = nodes.index[pos].to_numpy()
 
     else:
         # if unprojected, use ball tree for haversine nearest-neighbor search
         if BallTree is None:  # pragma: no cover
-            msg = "scikit-learn must be installed to search an unprojected graph"
+            msg = "scikit-learn must be installed as an optional dependency to search an unprojected graph."
             raise ImportError(msg)
         # haversine requires lat, lon coords in radians
         nodes_rad = np.deg2rad(nodes[["y", "x"]])
-        points_rad = np.deg2rad(np.array([Y, X]).T)
-        dist, pos = BallTree(nodes_rad, metric="haversine").query(points_rad, k=1)
-        dist = dist[:, 0] * EARTH_RADIUS_M  # convert radians -> meters
-        nn = nodes.index[pos[:, 0]]
+        points_rad = np.deg2rad(np.array([Y_arr, X_arr]).T)
+        dist_array, pos = BallTree(nodes_rad, metric="haversine").query(points_rad, k=1)
+        dist_array = dist_array[:, 0] * EARTH_RADIUS_M  # convert radians -> meters
+        nn_array = nodes.index[pos[:, 0]].to_numpy()
 
     # convert results to correct types for return
-    nn = nn.tolist()
-    dist = dist.tolist()
     if is_scalar:
-        nn = nn[0]
-        dist = dist[0]
+        nn = int(nn_array[0])
+        dist = float(dist_array[0])
+        if return_dist:
+            return nn, dist
+        # otherwise
+        return nn
 
+    # otherwise
     if return_dist:
-        return nn, dist
-
+        return nn_array, dist_array
     # otherwise
-    return nn
+    return nn_array
 
 
-def nearest_edges(G, X, Y, interpolate=None, return_dist=False):
+# if X and Y are floats and return_dist is not provided (defaults False)
+@overload
+def nearest_edges(G: nx.MultiDiGraph, X: float, Y: float) -> tuple[int, int, int]: ...
+
+
+# if X and Y are floats and return_dist is provided/False
+@overload
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: float,
+    Y: float,
+    *,
+    return_dist: Literal[False],
+) -> tuple[int, int, int]: ...
+
+
+# if X and Y are floats and return_dist is provided/True
+@overload
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: float,
+    Y: float,
+    *,
+    return_dist: Literal[True],
+) -> tuple[tuple[int, int, int], float]: ...
+
+
+# if X and Y are iterable and return_dist is not provided (defaults False)
+@overload
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+) -> npt.NDArray[np.object_]: ...
+
+
+# if X and Y are iterable and return_dist is provided/False
+@overload
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+    *,
+    return_dist: Literal[False],
+) -> npt.NDArray[np.object_]: ...
+
+
+# if X and Y are iterable and return_dist is provided/True
+@overload
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: Iterable[float],
+    Y: Iterable[float],
+    *,
+    return_dist: Literal[True],
+) -> tuple[npt.NDArray[np.object_], npt.NDArray[np.float64]]: ...
+
+
+def nearest_edges(
+    G: nx.MultiDiGraph,
+    X: float | Iterable[float],
+    Y: float | Iterable[float],
+    *,
+    return_dist: bool = False,
+) -> (
+    tuple[int, int, int]
+    | npt.NDArray[np.object_]
+    | tuple[tuple[int, int, int], float]
+    | tuple[npt.NDArray[np.object_], npt.NDArray[np.float64]]
+):
     """
     Find the nearest edge to a point or to each of several points.
 
     If `X` and `Y` are single coordinate values, this will return the nearest
-    edge to that point. If `X` and `Y` are lists of coordinate values, this
-    will return the nearest edge to each point. This function uses an R-tree
-    spatial index and minimizes the euclidean distance from each point to the
+    edge to that point. If `X` and `Y` are iterables of coordinate values,
+    this will return the nearest edge to each point. This uses an R-tree
+    spatial index and minimizes the Euclidean distance from each point to the
     possible matches. For accurate results, use a projected graph and points.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        graph in which to find nearest edges
-    X : float or list
-        points' x (longitude) coordinates, in same CRS/units as graph and
-        containing no nulls
-    Y : float or list
-        points' y (latitude) coordinates, in same CRS/units as graph and
-        containing no nulls
-    interpolate : float
-        deprecated, do not use
-    return_dist : bool
-        optionally also return distance between points and nearest edges
+    G
+        Graph in which to find nearest edges.
+    X
+        The points' x (longitude) coordinates, in same CRS/units as graph and
+        containing no nulls.
+    Y
+        The points' y (latitude) coordinates, in same CRS/units as graph and
+        containing no nulls.
+    return_dist
+        If True, optionally also return the distance(s) between point(s) and
+        nearest edge(s).
 
     Returns
     -------
-    ne or (ne, dist) : tuple or list
-        nearest edges as (u, v, key) or optionally a tuple where `dist`
-        contains distances between the points and their nearest edges
+    ne or (ne, dist)
+        Nearest edge ID(s) as `(u, v, k)` tuples, or optionally a tuple of
+        ID(s) and distance(s) between each point and its nearest edge.
     """
-    is_scalar = False
-    if not (hasattr(X, "__iter__") and hasattr(Y, "__iter__")):
-        # make coordinates arrays if user passed non-iterable values
+    # make coordinates arrays whether user passed iterable values or not
+    if not (isinstance(X, Iterable) and isinstance(Y, Iterable)):
         is_scalar = True
-        X = np.array([X])
-        Y = np.array([Y])
+        X_arr = np.array([X])
+        Y_arr = np.array([Y])
+    else:
+        is_scalar = False
+        X_arr = np.array(X)
+        Y_arr = np.array(Y)
 
-    if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
-        msg = "`X` and `Y` cannot contain nulls"
+    if np.isnan(X_arr).any() or np.isnan(Y_arr).any():  # pragma: no cover
+        msg = "`X` and `Y` cannot contain nulls."
         raise ValueError(msg)
     geoms = convert.graph_to_gdfs(G, nodes=False)["geometry"]
+    ne_array: npt.NDArray[np.object_]  # array of tuple[int, int, int]
+    dist_array: npt.NDArray[np.float64]
 
-    # if no interpolation distance was provided
-    if interpolate is None:
-        # build an r-tree spatial index by position for subsequent iloc
-        rtree = STRtree(geoms)
-
-        # use the r-tree to find each point's nearest neighbor and distance
-        points = [Point(xy) for xy in zip(X, Y)]
-        pos, dist = rtree.query_nearest(points, all_matches=False, return_distance=True)
-
-        # if user passed X/Y lists, the 2nd subarray contains geom indices
-        if len(pos.shape) > 1:
-            pos = pos[1]
-        ne = geoms.iloc[pos].index
+    # build an r-tree spatial index by position for subsequent iloc
+    rtree = STRtree(geoms)
 
-    # otherwise, if interpolation distance was provided
-    else:
-        warn(
-            "The `interpolate` parameter has been deprecated and will be "
-            "removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-        # interpolate points along edges to index with k-d tree or ball tree
-        uvk_xy = []
-        for uvk, geom in zip(geoms.index, geoms.to_numpy()):
-            uvk_xy.extend((uvk, xy) for xy in utils_geo.interpolate_points(geom, interpolate))
-        labels, xy = zip(*uvk_xy)
-        vertices = pd.DataFrame(xy, index=labels, columns=["x", "y"])
-
-        if projection.is_projected(G.graph["crs"]):
-            # if projected, use k-d tree for euclidean nearest-neighbor search
-            if cKDTree is None:  # pragma: no cover
-                msg = "scipy must be installed to search a projected graph"
-                raise ImportError(msg)
-            dist, pos = cKDTree(vertices).query(np.array([X, Y]).T, k=1)
-            ne = vertices.index[pos]
-
-        else:
-            # if unprojected, use ball tree for haversine nearest-neighbor search
-            if BallTree is None:  # pragma: no cover
-                msg = "scikit-learn must be installed to search an unprojected graph"
-                raise ImportError(msg)
-            # haversine requires lat, lon coords in radians
-            vertices_rad = np.deg2rad(vertices[["y", "x"]])
-            points_rad = np.deg2rad(np.array([Y, X]).T)
-            dist, pos = BallTree(vertices_rad, metric="haversine").query(points_rad, k=1)
-            dist = dist[:, 0] * EARTH_RADIUS_M  # convert radians -> meters
-            ne = vertices.index[pos[:, 0]]
+    # use the r-tree to find each point's nearest neighbor and distance
+    points = [Point(xy) for xy in zip(X_arr, Y_arr)]
+    pos, dist_array = rtree.query_nearest(points, all_matches=False, return_distance=True)
+
+    # if user passed X/Y lists, the 2nd subarray contains geom indices
+    if len(pos.shape) > 1:
+        pos = pos[1]
+    ne_array = geoms.iloc[pos].index.to_numpy()
 
     # convert results to correct types for return
-    ne = list(ne)
-    dist = list(dist)
     if is_scalar:
-        ne = ne[0]
-        dist = dist[0]
+        ne: tuple[int, int, int] = ne_array[0]
+        dist = float(dist_array[0])
+        if return_dist:
+            return ne, dist
+        # otherwise
+        return ne
 
+    # otherwise
     if return_dist:
-        return ne, dist
-
+        return ne_array, dist_array
     # otherwise
-    return ne
-
-
-def shortest_path(G, orig, dest, weight="length", cpus=1):
-    """
-    Do not use, deprecated.
-
-    The `shortest_path` function has moved to the `routing` module. Calling
-    it via the `distance` module will raise an error in the v2.0.0 release.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        input graph
-    orig : int or list
-        origin node ID, or a list of origin node IDs
-    dest : int or list
-        destination node ID, or a list of destination node IDs
-    weight : string
-        edge attribute to minimize when solving shortest path
-    cpus : int
-        how many CPU cores to use; if None, use all available
-
-    Returns
-    -------
-    path : list
-        list of node IDs constituting the shortest path, or, if orig and dest
-        are lists, then a list of path lists
-    """
-    warn(
-        "The `shortest_path` function has moved to the `routing` module. Calling it "
-        "via the `distance` module will raise an error starting in the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return routing.shortest_path(G, orig, dest, weight, cpus)
-
-
-def k_shortest_paths(G, orig, dest, k, weight="length"):
-    """
-    Do not use, deprecated.
-
-    The `k_shortest_paths` function has moved to the `routing` module. Calling
-    it via the `distance` module will raise an error in the v2.0.0 release.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        input graph
-    orig : int
-        origin node ID
-    dest : int
-        destination node ID
-    k : int
-        number of shortest paths to solve
-    weight : string
-        edge attribute to minimize when solving shortest paths. default is
-        edge length in meters.
-
-    Yields
-    ------
-    path : list
-        a generator of `k` shortest paths ordered by total weight. each path
-        is a list of node IDs.
-    """
-    warn(
-        "The `k_shortest_paths` function has moved to the `routing` module. "
-        "Calling it via the `distance` module will raise an error in the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return routing.k_shortest_paths(G, orig, dest, k, weight)
+    return ne_array
```

### Comparing `osmnx-1.9.3/osmnx/elevation.py` & `osmnx-2.0.0b0/osmnx/elevation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,332 +1,296 @@
 """Add node elevations from raster files or web APIs, and calculate edge grades."""
 
+from __future__ import annotations
+
+import logging as lg
 import multiprocessing as mp
 import time
 from hashlib import sha1
 from pathlib import Path
-from warnings import warn
+from typing import TYPE_CHECKING
+from typing import Any
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import requests
 
-from . import _downloader
+from . import _http
 from . import convert
 from . import settings
 from . import utils
 from ._errors import InsufficientResponseError
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
 # rasterio and gdal are optional dependencies for raster querying
 try:
     import rasterio
     from osgeo import gdal
 except ImportError:  # pragma: no cover
-    rasterio = gdal = None
+    rasterio = None
+    gdal = None
 
 
-def add_edge_grades(G, add_absolute=True, precision=None):
+def add_edge_grades(G: nx.MultiDiGraph, *, add_absolute: bool = True) -> nx.MultiDiGraph:
     """
-    Add `grade` attribute to each graph edge.
+    Calculate and add `grade` attributes to all graph edges.
 
-    Vectorized function to calculate the directed grade (ie, rise over run)
+    Vectorized function to calculate the directed grade (i.e., rise over run)
     for each edge in the graph and add it to the edge as an attribute. Nodes
-    must already have `elevation` attributes to use this function.
+    must already have `elevation` and `length` attributes before using this
+    function.
 
     See also the `add_node_elevations_raster` and `add_node_elevations_google`
     functions.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph with `elevation` node attribute
-    add_absolute : bool
-        if True, also add absolute value of grade as `grade_abs` attribute
-    precision : int
-        deprecated, do not use
+    G
+        Graph with `elevation` node attributes.
+    add_absolute
+        If True, also add absolute value of grade as `grade_abs` attribute.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with edge `grade` (and optionally `grade_abs`) attributes
+    G
+        Graph with `grade` (and optionally `grade_abs`) attributes on the
+        edges.
     """
-    if precision is None:
-        precision = 3
-    else:
-        warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
     elev_lookup = G.nodes(data="elevation")
     u, v, k, lengths = zip(*G.edges(keys=True, data="length"))
     uvk = tuple(zip(u, v, k))
 
     # calculate edges' elevation changes from u to v then divide by lengths
     elevs = np.array([(elev_lookup[u], elev_lookup[v]) for u, v, k in uvk])
-    grades = ((elevs[:, 1] - elevs[:, 0]) / np.array(lengths)).round(precision)
+    grades = (elevs[:, 1] - elevs[:, 0]) / np.array(lengths)
     nx.set_edge_attributes(G, dict(zip(uvk, grades)), name="grade")
 
     # optionally add grade absolute value to the edge attributes
     if add_absolute:
         nx.set_edge_attributes(G, dict(zip(uvk, np.abs(grades))), name="grade_abs")
 
-    utils.log("Added grade attributes to all edges.")
+    msg = "Added grade attributes to all edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
-def _query_raster(nodes, filepath, band):
+def _query_raster(
+    nodes: pd.DataFrame,
+    filepath: str | Path,
+    band: int,
+) -> Iterable[tuple[int, Any]]:
     """
-    Query a raster for values at coordinates in a DataFrame's x/y columns.
+    Query a raster file for values at coordinates in DataFrame x/y columns.
 
     Parameters
     ----------
-    nodes : pandas.DataFrame
-        DataFrame indexed by node ID and with two columns: x and y
-    filepath : string or pathlib.Path
-        path to the raster file or VRT to query
-    band : int
-        which raster band to query
+    nodes
+        DataFrame indexed by node ID and with two columns representing x and y
+        coordinates.
+    filepath
+        Path to the raster file or VRT to query.
+    band
+        Which raster band to query.
 
     Returns
     -------
-    nodes_values : zip
-        zipped node IDs and corresponding raster values
+    nodes_values
+        Zip of node IDs and corresponding raster values.
     """
     # must open raster file here: cannot pickle it to pass in multiprocessing
     with rasterio.open(filepath) as raster:
         values = np.array(tuple(raster.sample(nodes.to_numpy(), band)), dtype=float).squeeze()
         values[values == raster.nodata] = np.nan
         return zip(nodes.index, values)
 
 
-def add_node_elevations_raster(G, filepath, band=1, cpus=None):
+def add_node_elevations_raster(
+    G: nx.MultiDiGraph,
+    filepath: str | Path | Iterable[str | Path],
+    *,
+    band: int = 1,
+    cpus: int | None = None,
+) -> nx.MultiDiGraph:
     """
-    Add `elevation` attribute to each node from local raster file(s).
+    Add `elevation` attributes to all nodes from local raster file(s).
 
-    If `filepath` is a list of paths, this will generate a virtual raster
+    If `filepath` is an iterable of paths, this will generate a virtual raster
     composed of the files at those paths as an intermediate step.
 
     See also the `add_edge_grades` function.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph, in same CRS as raster
-    filepath : string or pathlib.Path or list of strings/Paths
-        path (or list of paths) to the raster file(s) to query
-    band : int
-        which raster band to query
-    cpus : int
-        how many CPU cores to use; if None, use all available
+    G
+        Graph in same CRS as raster.
+    filepath
+        The path(s) to the raster file(s) to query.
+    band
+        Which raster band to query.
+    cpus
+        How many CPU cores to use. If None, use all available.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with node elevation attributes
+    G
+        Graph with `elevation` attributes on the nodes.
     """
     if rasterio is None or gdal is None:  # pragma: no cover
-        msg = "gdal and rasterio must be installed to query raster files"
+        msg = "gdal and rasterio must be installed as optional dependencies to query raster files."
         raise ImportError(msg)
 
     if cpus is None:
         cpus = mp.cpu_count()
     cpus = min(cpus, mp.cpu_count())
-    utils.log(f"Attaching elevations with {cpus} CPUs...")
+    msg = f"Attaching elevations with {cpus} CPUs..."
+    utils.log(msg, level=lg.INFO)
 
-    # if a list of filepaths is passed, compose them all as a virtual raster
-    # use the sha1 hash of the filepaths list as the vrt filename
+    # if multiple filepaths are passed in, compose them as a virtual raster
+    # use the sha1 hash of the filepaths object as the vrt filename
     if not isinstance(filepath, (str, Path)):
         filepaths = [str(p) for p in filepath]
-        sha = sha1(str(filepaths).encode("utf-8")).hexdigest()
-        filepath = f"./.osmnx_{sha}.vrt"
+        checksum = sha1(str(filepaths).encode("utf-8")).hexdigest()  # noqa: S324
+        filepath = f"./.osmnx_{checksum}.vrt"
         gdal.UseExceptions()
         gdal.BuildVRT(filepath, filepaths).FlushCache()
 
     nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
     if cpus == 1:
         elevs = dict(_query_raster(nodes, filepath, band))
     else:
         # divide nodes into equal-sized chunks for multiprocessing
         size = int(np.ceil(len(nodes) / cpus))
         args = ((nodes.iloc[i : i + size], filepath, band) for i in range(0, len(nodes), size))
         with mp.get_context("spawn").Pool(cpus) as pool:
             results = pool.starmap_async(_query_raster, args).get()
         elevs = {k: v for kv in results for k, v in kv}
 
-    assert len(G) == len(elevs)
     nx.set_node_attributes(G, elevs, name="elevation")
-    utils.log("Added elevation data from raster to all nodes.")
+    msg = "Added elevation data from raster to all nodes"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def add_node_elevations_google(
-    G,
-    api_key=None,
-    batch_size=350,
-    pause=0,
-    max_locations_per_batch=None,
-    precision=None,
-    url_template=None,
-):
+    G: nx.MultiDiGraph,
+    *,
+    api_key: str | None = None,
+    batch_size: int = 512,
+    pause: float = 0,
+) -> nx.MultiDiGraph:
     """
-    Add an `elevation` (meters) attribute to each node using a web service.
+    Add `elevation` (meters) attributes to all nodes using a web service.
 
     By default, this uses the Google Maps Elevation API but you can optionally
     use an equivalent API with the same interface and response format, such as
     Open Topo Data, via the `settings` module's `elevation_url_template`. The
     Google Maps Elevation API requires an API key but other providers may not.
+    You can find more information about the Google Maps Elevation API at:
+    https://developers.google.com/maps/documentation/elevation
 
     For a free local alternative see the `add_node_elevations_raster`
     function. See also the `add_edge_grades` function.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    api_key : string
-        a valid API key, can be None if the API does not require a key
-    batch_size : int
-        max number of coordinate pairs to submit in each API call (if this is
-        too high, the server will reject the request because its character
-        limit exceeds the max allowed)
-    pause : float
-        time to pause between API calls, which can be increased if you get
-        rate limited
-    max_locations_per_batch : int
-        deprecated, do not use
-    precision : int
-        deprecated, do not use
-    url_template : string
-        deprecated, do not use
+    G
+        Graph to add elevation data to.
+    api_key
+        A valid API key. Can be None if the API does not require a key.
+    batch_size
+        Max number of coordinate pairs to submit in each request (depends on
+        provider's limits). Google's limit is 512.
+    pause
+        How long to pause in seconds between API calls, which can be increased
+        if you get rate limited.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with node elevation attributes
+    G
+        Graph with `elevation` attributes on the nodes.
     """
-    if max_locations_per_batch is None:
-        max_locations_per_batch = batch_size
-    else:
-        warn(
-            "The `max_locations_per_batch` parameter is deprecated and will be "
-            "removed the v2.0.0 release, use the `batch_size` parameter instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
+    # make a pandas series of all the nodes' coordinates as "lat,lon" and
+    # round coordinates to 6 decimal places (approx 5 to 10 cm resolution)
+    node_points = pd.Series({n: f"{d['y']:.6f},{d['x']:.6f}" for n, d in G.nodes(data=True)})
+    n_calls = int(np.ceil(len(node_points) / batch_size))
+    domain = _http._hostname_from_url(settings.elevation_url_template)
 
-    if precision is None:
-        precision = 3
-    else:
-        warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
+    msg = f"Requesting node elevations from {domain!r} in {n_calls} request(s)"
+    utils.log(msg, level=lg.INFO)
 
-    if url_template is None:
-        url_template = settings.elevation_url_template
-    else:
-        warn(
-            "The `url_template` parameter is deprecated and will be removed "
-            "in the v2.0.0 release. Configure the `settings` module's "
-            "`elevation_url_template` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    # make a pandas series of all the nodes' coordinates as 'lat,lon'
-    # round coordinates to 5 decimal places (approx 1 meter) to be able to fit
-    # in more locations per API call
-    node_points = pd.Series(
-        {node: f'{data["y"]:.5f},{data["x"]:.5f}' for node, data in G.nodes(data=True)}
-    )
-    n_calls = int(np.ceil(len(node_points) / max_locations_per_batch))
-    domain = _downloader._hostname_from_url(url_template)
-    utils.log(f"Requesting node elevations from {domain!r} in {n_calls} request(s)")
-
-    # break the series of coordinates into chunks of max_locations_per_batch
+    # break the series of coordinates into chunks of batch_size
     # API format is locations=lat,lon|lat,lon|lat,lon|lat,lon...
     results = []
-    for i in range(0, len(node_points), max_locations_per_batch):
-        chunk = node_points.iloc[i : i + max_locations_per_batch]
+    for i in range(0, len(node_points), batch_size):
+        chunk = node_points.iloc[i : i + batch_size]
         locations = "|".join(chunk)
-        url = url_template.format(locations=locations, key=api_key)
+        url = settings.elevation_url_template.format(locations=locations, key=api_key)
 
         # download and append these elevation results to list of all results
         response_json = _elevation_request(url, pause)
         if "results" in response_json and len(response_json["results"]) > 0:
             results.extend(response_json["results"])
         else:
             raise InsufficientResponseError(str(response_json))
 
     # sanity check that all our vectors have the same number of elements
     msg = f"Graph has {len(G):,} nodes and we received {len(results):,} results from {domain!r}"
-    utils.log(msg)
+    utils.log(msg, level=lg.INFO)
     if not (len(results) == len(G) == len(node_points)):  # pragma: no cover
         err_msg = f"{msg}\n{response_json}"
         raise InsufficientResponseError(err_msg)
 
     # add elevation as an attribute to the nodes
     df_elev = pd.DataFrame(node_points, columns=["node_points"])
     df_elev["elevation"] = [result["elevation"] for result in results]
-    df_elev["elevation"] = df_elev["elevation"].round(precision)
     nx.set_node_attributes(G, name="elevation", values=df_elev["elevation"].to_dict())
-    utils.log(f"Added elevation data from {domain!r} to all nodes.")
+    msg = f"Added elevation data from {domain!r} to all nodes."
+    utils.log(msg, level=lg.INFO)
 
     return G
 
 
-def _elevation_request(url, pause):
+def _elevation_request(url: str, pause: float) -> dict[str, Any]:
     """
-    Send a HTTP GET request to Google Maps-style Elevation API.
+    Send a HTTP GET request to a Google Maps-style Elevation API.
 
     Parameters
     ----------
-    url : string
-        URL for API endpoint populated with request data
-    pause : float
-        how long to pause in seconds before request
+    url
+        URL of API endpoint, populated with request data.
+    pause
+        How long to pause in seconds before request.
 
     Returns
     -------
-    response_json : dict
+    response_json
     """
-    if settings.timeout is None:
-        timeout = settings.requests_timeout
-    else:
-        timeout = settings.timeout
-        msg = (
-            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
-            "release: use `settings.requests_timeout` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
     # check if request already exists in cache
-    cached_response_json = _downloader._retrieve_from_cache(url)
-    if cached_response_json is not None:
+    cached_response_json = _http._retrieve_from_cache(url)
+    if isinstance(cached_response_json, dict):
         return cached_response_json
 
     # pause then request this URL
-    domain = _downloader._hostname_from_url(url)
-    utils.log(f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}")
+    domain = _http._hostname_from_url(url)
+    msg = f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}"
+    utils.log(msg, level=lg.INFO)
     time.sleep(pause)
 
     # transmit the HTTP GET request
-    utils.log(f"Get {url} with timeout={timeout}")
+    msg = f"Get {url} with timeout={settings.requests_timeout}"
+    utils.log(msg, level=lg.INFO)
     response = requests.get(
         url,
-        timeout=timeout,
-        headers=_downloader._get_http_headers(),
+        timeout=settings.requests_timeout,
+        headers=_http._get_http_headers(),
         **settings.requests_kwargs,
     )
 
-    response_json = _downloader._parse_response(response)
-    _downloader._save_to_cache(url, response_json, response.status_code)
+    response_json = _http._parse_response(response)
+    if not isinstance(response_json, dict):  # pragma: no cover
+        msg = "Elevation API did not return a dict of results."
+        raise InsufficientResponseError(msg)
+    _http._save_to_cache(url, response_json, response.ok)
     return response_json
```

### Comparing `osmnx-1.9.3/osmnx/geocoder.py` & `osmnx-2.0.0b0/osmnx/geocoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,66 +2,74 @@
 Geocode place names or addresses or retrieve OSM elements by place name or ID.
 
 This module uses the Nominatim API's "search" and "lookup" endpoints. For more
 details see https://wiki.openstreetmap.org/wiki/Elements and
 https://nominatim.org/.
 """
 
+from __future__ import annotations
+
 import logging as lg
 from collections import OrderedDict
-from warnings import warn
+from typing import Any
 
 import geopandas as gpd
 import pandas as pd
 
 from . import _nominatim
-from . import projection
 from . import settings
 from . import utils
 from ._errors import InsufficientResponseError
 
 
-def geocode(query):
+def geocode(query: str) -> tuple[float, float]:
     """
-    Geocode place names or addresses to (lat, lon) with the Nominatim API.
+    Geocode place names or addresses to `(lat, lon)` with the Nominatim API.
 
     This geocodes the query via the Nominatim "search" endpoint.
 
     Parameters
     ----------
-    query : string
-        the query string to geocode
+    query
+        The query string to geocode.
 
     Returns
     -------
-    point : tuple
-        the (lat, lon) coordinates returned by the geocoder
+    point
+        The `(lat, lon)` coordinates returned by the geocoder.
     """
     # define the parameters
-    params = OrderedDict()
+    params: OrderedDict[str, int | str] = OrderedDict()
     params["format"] = "json"
     params["limit"] = 1
     params["dedupe"] = 0  # prevent deduping to get precise number of results
     params["q"] = query
     response_json = _nominatim._nominatim_request(params=params)
 
     # if results were returned, parse lat and lon out of the result
     if response_json and "lat" in response_json[0] and "lon" in response_json[0]:
         lat = float(response_json[0]["lat"])
         lon = float(response_json[0]["lon"])
         point = (lat, lon)
-        utils.log(f"Geocoded {query!r} to {point}")
+
+        msg = f"Geocoded {query!r} to {point}"
+        utils.log(msg, level=lg.INFO)
         return point
 
     # otherwise we got no results back
-    msg = f"Nominatim could not geocode query {query!r}"
+    msg = f"Nominatim could not geocode query {query!r}."
     raise InsufficientResponseError(msg)
 
 
-def geocode_to_gdf(query, which_result=None, by_osmid=False, buffer_dist=None):
+def geocode_to_gdf(
+    query: str | dict[str, str] | list[str | dict[str, str]],
+    *,
+    which_result: int | None | list[int | None] = None,
+    by_osmid: bool = False,
+) -> gpd.GeoDataFrame:
     """
     Retrieve OSM elements by place name or OSM ID with the Nominatim API.
 
     If searching by place name, the `query` argument can be a string or
     structured dict, or a list of such strings/dicts to send to the geocoder.
     This uses the Nominatim "search" endpoint to geocode the place name to the
     best-matching OSM element, then returns that element and its attribute
@@ -70,140 +78,114 @@
     You can instead query by OSM ID by passing `by_osmid=True`. This uses the
     Nominatim "lookup" endpoint to retrieve the OSM element with that ID. In
     this case, the function treats the `query` argument as an OSM ID (or list
     of OSM IDs), which must be prepended with their types: node (N), way (W),
     or relation (R) in accordance with the Nominatim API format. For example,
     `query=["R2192363", "N240109189", "W427818536"]`.
 
-    If `query` is a list, then `which_result` must be either a single value or
-    a list with the same length as `query`. The queries you provide must be
+    If `query` is a list, then `which_result` must be either an int or a list
+    with the same length as `query`. The queries you provide must be
     resolvable to elements in the Nominatim database. The resulting
     GeoDataFrame's geometry column contains place boundaries if they exist.
 
     Parameters
     ----------
-    query : string or dict or list of strings/dicts
-        query string(s) or structured dict(s) to geocode
-    which_result : int
-        which search result to return. if None, auto-select the first
-        (Multi)Polygon or raise an error if OSM doesn't return one. to get
-        the top match regardless of geometry type, set which_result=1.
-        ignored if by_osmid=True.
-    by_osmid : bool
-        if True, treat query as an OSM ID lookup rather than text search
-    buffer_dist : float
-        deprecated, do not use
+    query
+        The query string(s) or structured dict(s) to geocode.
+    which_result
+        Which search result to return. If None, auto-select the first
+        (Multi)Polygon or raise an error if OSM doesn't return one. To get
+        the top match regardless of geometry type, set `which_result=1`.
+        Ignored if `by_osmid=True`.
+    by_osmid
+        If True, treat query as an OSM ID lookup rather than text search.
 
     Returns
     -------
-    gdf : geopandas.GeoDataFrame
-        a GeoDataFrame with one row for each query
+    gdf
+        GeoDataFrame with one row for each query result.
     """
-    if buffer_dist is not None:
-        warn(
-            "The buffer_dist argument has been deprecated and will be removed "
-            "in the v2.0.0 release. Buffer your results directly, if desired. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    if not isinstance(query, (str, dict, list)):  # pragma: no cover
-        msg = "query must be a string or dict or list"
-        raise TypeError(msg)
-
-    # if caller passed a list of queries but a scalar which_result value, then
-    # turn which_result into a list with same length as query list
-    if isinstance(query, list) and (isinstance(which_result, int) or which_result is None):
-        which_result = [which_result] * len(query)
-
-    # turn query and which_result into lists if they're not already
-    if not isinstance(query, list):
-        query = [query]
-    if not isinstance(which_result, list):
-        which_result = [which_result]
+    if isinstance(query, list):
+        # if query is a list of queries but which_result is int/None, then
+        # turn which_result into a list with same length as query list
+        q_list = query
+        wr_list = which_result if isinstance(which_result, list) else [which_result] * len(query)
+    else:
+        # if query is not already a list, turn it into one
+        # if which_result was a list, take 0th element, otherwise make it list
+        q_list = [query]
+        wr_list = [which_result[0]] if isinstance(which_result, list) else [which_result]
 
     # ensure same length
-    if len(query) != len(which_result):  # pragma: no cover
-        msg = "which_result length must equal query length"
+    if len(q_list) != len(wr_list):  # pragma: no cover
+        msg = "`which_result` length must equal `query` length."
         raise ValueError(msg)
 
-    # ensure query type of each item
-    for q in query:
-        if not isinstance(q, (str, dict)):  # pragma: no cover
-            msg = "each query must be a dict or a string"
-            raise TypeError(msg)
-
-    # geocode each query and add to GeoDataFrame as a new row
-    gdf = gpd.GeoDataFrame()
-    for q, wr in zip(query, which_result):
-        gdf = pd.concat([gdf, _geocode_query_to_gdf(q, wr, by_osmid)])
-
-    # reset GeoDataFrame index and set its CRS
-    gdf = gdf.reset_index(drop=True)
-    gdf = gdf.set_crs(settings.default_crs)
-
-    # if buffer_dist was passed in, project the geometry to UTM, buffer it in
-    # meters, then project it back to lat-lon
-    if buffer_dist is not None and len(gdf) > 0:
-        gdf_utm = projection.project_gdf(gdf)
-        gdf_utm["geometry"] = gdf_utm["geometry"].buffer(buffer_dist)
-        gdf = projection.project_gdf(gdf_utm, to_latlong=True)
-        utils.log(f"Buffered GeoDataFrame to {buffer_dist} meters")
+    # geocode each query, concat as GeoDataFrame rows, then set the CRS
+    results = (_geocode_query_to_gdf(q, wr, by_osmid) for q, wr in zip(q_list, wr_list))
+    gdf = pd.concat(results, ignore_index=True).set_crs(settings.default_crs)
 
-    utils.log(f"Created GeoDataFrame with {len(gdf)} rows from {len(query)} queries")
+    msg = f"Created GeoDataFrame with {len(gdf)} rows from {len(q_list)} queries"
+    utils.log(msg, level=lg.INFO)
     return gdf
 
 
-def _geocode_query_to_gdf(query, which_result, by_osmid):
+def _geocode_query_to_gdf(
+    query: str | dict[str, str],
+    which_result: int | None,
+    by_osmid: bool,  # noqa: FBT001
+) -> gpd.GeoDataFrame:
     """
     Geocode a single place query to a GeoDataFrame.
 
     Parameters
     ----------
-    query : string or dict
-        query string or structured dict to geocode
-    which_result : int
-        which geocoding result to use. if None, auto-select the first
-        (Multi)Polygon or raise an error if OSM doesn't return one. to get
-        the top match regardless of geometry type, set which_result=1.
-        ignored if by_osmid=True.
-    by_osmid : bool
-        if True, handle query as an OSM ID for lookup rather than text search
+    query
+        Query string or structured dict to geocode.
+    which_result
+        Which search result to return. If None, auto-select the first
+        (Multi)Polygon or raise an error if OSM doesn't return one. To get
+        the top match regardless of geometry type, set `which_result=1`.
+        Ignored if `by_osmid=True`.
+    by_osmid
+        If True, treat query as an OSM ID lookup rather than text search.
 
     Returns
     -------
-    gdf : geopandas.GeoDataFrame
-        a GeoDataFrame with one row containing the result of geocoding
+    gdf
+        GeoDataFrame with one row containing the geocoding result.
     """
     limit = 50 if which_result is None else which_result
-
     results = _nominatim._download_nominatim_element(query, by_osmid=by_osmid, limit=limit)
 
     # choose the right result from the JSON response
-    if not results:
+    if len(results) == 0:
         # if no results were returned, raise error
-        msg = f"Nominatim geocoder returned 0 results for query {query!r}"
+        msg = f"Nominatim geocoder returned 0 results for query {query!r}."
         raise InsufficientResponseError(msg)
 
     if by_osmid:
         # if searching by OSM ID, always take the first (ie, only) result
         result = results[0]
 
     elif which_result is None:
         # else, if which_result=None, auto-select the first (Multi)Polygon
-        result = _get_first_polygon(results, query)
+        try:
+            result = _get_first_polygon(results)
+        except TypeError as e:
+            msg = f"Nominatim did not geocode query {query!r} to a geometry of type (Multi)Polygon."
+            raise TypeError(msg) from e
 
     elif len(results) >= which_result:
         # else, if we got at least which_result results, choose that one
         result = results[which_result - 1]
 
     else:  # pragma: no cover
         # else, we got fewer results than which_result, raise error
-        msg = f"Nominatim returned {len(results)} result(s) but which_result={which_result}"
+        msg = f"Nominatim returned {len(results)} result(s) but `which_result={which_result}`."
         raise InsufficientResponseError(msg)
 
     # if we got a non (Multi)Polygon geometry type (like a point), log warning
     geom_type = result["geojson"]["type"]
     if geom_type not in {"Polygon", "MultiPolygon"}:
         msg = f"Nominatim geocoder returned a {geom_type} as the geometry for query {query!r}"
         utils.log(msg, level=lg.WARNING)
@@ -229,31 +211,29 @@
     # create and return the GeoDataFrame
     gdf = gpd.GeoDataFrame.from_features([feature])
     cols = ["lat", "lon", "bbox_north", "bbox_south", "bbox_east", "bbox_west"]
     gdf[cols] = gdf[cols].astype(float)
     return gdf
 
 
-def _get_first_polygon(results, query):
+def _get_first_polygon(results: list[dict[str, Any]]) -> dict[str, Any]:
     """
     Choose first result of geometry type (Multi)Polygon from list of results.
 
     Parameters
     ----------
-    results : list
-        list of results from _downloader._osm_place_download
-    query : str
-        the query string or structured dict that was geocoded
+    results
+        Results from the Nominatim API.
 
     Returns
     -------
-    result : dict
-        the chosen result
+    result
+        The chosen result.
     """
     polygon_types = {"Polygon", "MultiPolygon"}
+
     for result in results:
         if "geojson" in result and result["geojson"]["type"] in polygon_types:
             return result
 
-    # if we never found a polygon, throw an error
-    msg = f"Nominatim could not geocode query {query!r} to a geometry of type (Multi)Polygon"
-    raise TypeError(msg)
+    # if we never found a polygon, raise an error
+    raise TypeError
```

### Comparing `osmnx-1.9.3/osmnx/graph.py` & `osmnx-2.0.0b0/osmnx/graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,648 +1,609 @@
 """
 Download and create graphs from OpenStreetMap data.
 
-This module uses filters to query the Overpass API: you can either specify a
-built-in network type or provide your own custom filter with Overpass QL.
-
 Refer to the Getting Started guide for usage limitations.
 """
 
-import itertools
-from warnings import warn
+from __future__ import annotations
+
+import logging as lg
+from collections.abc import Iterable
+from itertools import groupby
+from pathlib import Path
+from typing import TYPE_CHECKING
+from typing import Any
 
 import networkx as nx
-from shapely.geometry import MultiPolygon
-from shapely.geometry import Polygon
+from shapely import MultiPolygon
+from shapely import Polygon
 
+from . import _osm_xml
 from . import _overpass
 from . import distance
 from . import geocoder
-from . import osm_xml
 from . import projection
 from . import settings
 from . import simplification
 from . import stats
 from . import truncate
 from . import utils
 from . import utils_geo
 from ._errors import CacheOnlyInterruptError
 from ._errors import InsufficientResponseError
 from ._version import __version__
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from pathlib import Path
+
 
 def graph_from_bbox(
-    north=None,
-    south=None,
-    east=None,
-    west=None,
-    bbox=None,
-    network_type="all",
-    simplify=True,
-    retain_all=False,
-    truncate_by_edge=False,
-    clean_periphery=None,
-    custom_filter=None,
-):
-    """
-    Download and create a graph within some bounding box.
-
-    You can use the `settings` module to retrieve a snapshot of historical OSM
-    data as of a certain date, or to configure the Overpass server timeout,
-    memory allocation, and other custom settings.
+    bbox: tuple[float, float, float, float],
+    *,
+    network_type: str = "all",
+    simplify: bool = True,
+    retain_all: bool = False,
+    truncate_by_edge: bool = False,
+    custom_filter: str | None = None,
+) -> nx.MultiDiGraph:
+    """
+    Download and create a graph within a lat-lon bounding box.
+
+    This function uses filters to query the Overpass API: you can either
+    specify a pre-defined `network_type` or provide your own `custom_filter`
+    with Overpass QL.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes. You can also use the `settings` module to retrieve a snapshot
+    of historical OSM data as of a certain date, or to configure the Overpass
+    server timeout, memory allocation, and other custom settings.
 
     Parameters
     ----------
-    north : float
-        deprecated, do not use
-    south : float
-        deprecated, do not use
-    east : float
-        deprecated, do not use
-    west : float
-        deprecated, do not use
-    bbox : tuple of floats
-        bounding box as (north, south, east, west)
-    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get if custom_filter is None
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    truncate_by_edge : bool
-        if True, retain nodes outside bounding box if at least one of node's
-        neighbors is within the bounding box
-    clean_periphery : bool
-        deprecated, do not use
-    custom_filter : string
-        a custom ways filter to be used instead of the network_type presets
-        e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
-        in a network_type that is in settings.bidirectional_network_types if
-        you want graph to be fully bi-directional.
+    bbox
+        Bounding box as `(north, south, east, west)`. Coordinates should be in
+        unprojected latitude-longitude degrees (EPSG:4326).
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve if `custom_filter` is None.
+    simplify
+        If True, simplify graph topology via the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    truncate_by_edge
+        If True, retain nodes outside bounding box if at least one of node's
+        neighbors is within the bounding box.
+    custom_filter
+        A custom ways filter to be used instead of the `network_type` presets,
+        e.g. `'["power"~"line"]' or '["highway"~"motorway|trunk"]'`. Also pass
+        in a `network_type` that is in `settings.bidirectional_network_types`
+        if you want the graph to be fully bidirectional.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
-    if not (north is None and south is None and east is None and west is None):
-        msg = (
-            "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-        bbox = (north, south, east, west)
-
     # convert bounding box to a polygon
-    polygon = utils_geo.bbox_to_poly(bbox=bbox)
+    polygon = utils_geo.bbox_to_poly(bbox)
 
     # create graph using this polygon geometry
     G = graph_from_polygon(
         polygon,
         network_type=network_type,
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
-        clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
 
-    utils.log(f"graph_from_bbox returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    msg = f"graph_from_bbox returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def graph_from_point(
-    center_point,
-    dist=1000,
-    dist_type="bbox",
-    network_type="all",
-    simplify=True,
-    retain_all=False,
-    truncate_by_edge=False,
-    clean_periphery=None,
-    custom_filter=None,
-):
-    """
-    Download and create a graph within some distance of a (lat, lon) point.
-
-    You can use the `settings` module to retrieve a snapshot of historical OSM
-    data as of a certain date, or to configure the Overpass server timeout,
-    memory allocation, and other custom settings.
+    center_point: tuple[float, float],
+    dist: float,
+    *,
+    dist_type: str = "bbox",
+    network_type: str = "all",
+    simplify: bool = True,
+    retain_all: bool = False,
+    truncate_by_edge: bool = False,
+    custom_filter: str | None = None,
+) -> nx.MultiDiGraph:
+    """
+    Download and create a graph within some distance of a lat-lon point.
+
+    This function uses filters to query the Overpass API: you can either
+    specify a pre-defined `network_type` or provide your own `custom_filter`
+    with Overpass QL.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes. You can also use the `settings` module to retrieve a snapshot
+    of historical OSM data as of a certain date, or to configure the Overpass
+    server timeout, memory allocation, and other custom settings.
 
     Parameters
     ----------
-    center_point : tuple
-        the (lat, lon) center point around which to construct the graph
-    dist : int
-        retain only those nodes within this many meters of the center of the
-        graph, with distance determined according to dist_type argument
-    dist_type : string {"network", "bbox"}
-        if "bbox", retain only those nodes within a bounding box of the
-        distance parameter. if "network", retain only those nodes within some
-        network distance from the center-most node.
-    network_type : string, {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get if custom_filter is None
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    truncate_by_edge : bool
-        if True, retain nodes outside bounding box if at least one of node's
-        neighbors is within the bounding box
-    clean_periphery : bool,
-        deprecated, do not use
-    custom_filter : string
-        a custom ways filter to be used instead of the network_type presets
-        e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
-        in a network_type that is in settings.bidirectional_network_types if
-        you want graph to be fully bi-directional.
+    center_point
+        The `(lat, lon)` center point around which to construct the graph.
+        Coordinates should be in unprojected latitude-longitude degrees
+        (EPSG:4326).
+    dist
+        Retain only those nodes within this many meters of `center_point`,
+        measuring distance according to `dist_type`.
+    dist_type
+        {"bbox", "network"}
+        If "bbox", retain only those nodes within a bounding box of `dist`
+        length/width. If "network", retain only those nodes within `dist`
+        network distance of the nearest node to `center_point`.
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve if `custom_filter` is None.
+    simplify
+        If True, simplify graph topology with the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    truncate_by_edge
+        If True, retain nodes outside bounding box if at least one of node's
+        neighbors is within the bounding box.
+    custom_filter
+        A custom ways filter to be used instead of the `network_type` presets,
+        e.g. `'["power"~"line"]' or '["highway"~"motorway|trunk"]'`. Also pass
+        in a `network_type` that is in `settings.bidirectional_network_types`
+        if you want the graph to be fully bidirectional.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
     if dist_type not in {"bbox", "network"}:  # pragma: no cover
-        msg = 'dist_type must be "bbox" or "network"'
+        msg = "`dist_type` must be 'bbox' or 'network'."
         raise ValueError(msg)
 
     # create bounding box from center point and distance in each direction
     bbox = utils_geo.bbox_from_point(center_point, dist)
 
     # create a graph from the bounding box
     G = graph_from_bbox(
-        bbox=bbox,
+        bbox,
         network_type=network_type,
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
-        clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
 
     if dist_type == "network":
-        # if dist_type is network, find node in graph nearest to center point
-        # then truncate graph by network dist from it
-        node = distance.nearest_nodes(G, X=[center_point[1]], Y=[center_point[0]])[0]
-        G = truncate.truncate_graph_dist(G, node, max_dist=dist)
+        # find node nearest to center then truncate graph by dist from it
+        node = distance.nearest_nodes(G, X=center_point[1], Y=center_point[0])
+        G = truncate.truncate_graph_dist(G, node, dist)
 
-    utils.log(f"graph_from_point returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    msg = f"graph_from_point returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def graph_from_address(
-    address,
-    dist=1000,
-    dist_type="bbox",
-    network_type="all",
-    simplify=True,
-    retain_all=False,
-    truncate_by_edge=False,
-    return_coords=None,
-    clean_periphery=None,
-    custom_filter=None,
-):
+    address: str,
+    dist: float,
+    *,
+    dist_type: str = "bbox",
+    network_type: str = "all",
+    simplify: bool = True,
+    retain_all: bool = False,
+    truncate_by_edge: bool = False,
+    custom_filter: str | None = None,
+) -> nx.MultiDiGraph | tuple[nx.MultiDiGraph, tuple[float, float]]:
     """
     Download and create a graph within some distance of an address.
 
-    You can use the `settings` module to retrieve a snapshot of historical OSM
-    data as of a certain date, or to configure the Overpass server timeout,
-    memory allocation, and other custom settings.
+    This function uses filters to query the Overpass API: you can either
+    specify a pre-defined `network_type` or provide your own `custom_filter`
+    with Overpass QL.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes. You can also use the `settings` module to retrieve a snapshot
+    of historical OSM data as of a certain date, or to configure the Overpass
+    server timeout, memory allocation, and other custom settings.
 
     Parameters
     ----------
-    address : string
-        the address to geocode and use as the central point around which to
-        construct the graph
-    dist : int
-        retain only those nodes within this many meters of the center of the
-        graph
-    dist_type : string {"network", "bbox"}
-        if "bbox", retain only those nodes within a bounding box of the
-        distance parameter. if "network", retain only those nodes within some
-        network distance from the center-most node.
-    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get if custom_filter is None
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    truncate_by_edge : bool
-        if True, retain nodes outside bounding box if at least one of node's
-        neighbors is within the bounding box
-    return_coords : bool
-        deprecated, do not use
-    clean_periphery : bool
-        deprecated, do not use
-    custom_filter : string
-        a custom ways filter to be used instead of the network_type presets
-        e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
-        in a network_type that is in settings.bidirectional_network_types if
-        you want graph to be fully bi-directional.
+    address
+        The address to geocode and use as the central point around which to
+        construct the graph.
+    dist
+        Retain only those nodes within this many meters of `center_point`,
+        measuring distance according to `dist_type`.
+    dist_type
+        {"network", "bbox"}
+        If "bbox", retain only those nodes within a bounding box of `dist`. If
+        "network", retain only those nodes within `dist` network distance from
+        the centermost node.
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve if `custom_filter` is None.
+    simplify
+        If True, simplify graph topology with the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    truncate_by_edge
+        If True, retain nodes outside bounding box if at least one of node's
+        neighbors is within the bounding box.
+    custom_filter
+        A custom ways filter to be used instead of the `network_type` presets,
+        e.g. `'["power"~"line"]' or '["highway"~"motorway|trunk"]'`. Also pass
+        in a `network_type` that is in `settings.bidirectional_network_types`
+        if you want the graph to be fully bidirectional.
 
     Returns
     -------
-    networkx.MultiDiGraph or optionally (networkx.MultiDiGraph, (lat, lon))
+    G or (G, (lat, lon))
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
-    if return_coords is None:
-        return_coords = False
-    else:
-        warn(
-            "The `return_coords` argument has been deprecated and will be removed in "
-            "the v2.0.0 release. Future behavior will be as though `return_coords=False`. "
-            "If you want the address's geocoded coordinates, use the `geocode` function. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
     # geocode the address string to a (lat, lon) point
-    point = geocoder.geocode(query=address)
+    point = geocoder.geocode(address)
 
     # then create a graph from this point
     G = graph_from_point(
         point,
         dist,
-        dist_type,
+        dist_type=dist_type,
         network_type=network_type,
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
-        clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
-    utils.log(f"graph_from_address returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
 
-    if return_coords:
-        return G, point
-
-    # otherwise
+    msg = f"graph_from_address returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def graph_from_place(
-    query,
-    network_type="all",
-    simplify=True,
-    retain_all=False,
-    truncate_by_edge=False,
-    which_result=None,
-    buffer_dist=None,
-    clean_periphery=None,
-    custom_filter=None,
-):
+    query: str | dict[str, str] | list[str | dict[str, str]],
+    *,
+    network_type: str = "all",
+    simplify: bool = True,
+    retain_all: bool = False,
+    truncate_by_edge: bool = False,
+    which_result: int | None | list[int | None] = None,
+    custom_filter: str | None = None,
+) -> nx.MultiDiGraph:
     """
     Download and create a graph within the boundaries of some place(s).
 
     The query must be geocodable and OSM must have polygon boundaries for the
     geocode result. If OSM does not have a polygon for this place, you can
-    instead get its street network using the graph_from_address function,
+    instead get its street network using the `graph_from_address` function,
     which geocodes the place name to a point and gets the network within some
     distance of that point.
 
     If OSM does have polygon boundaries for this place but you're not finding
     it, try to vary the query string, pass in a structured query dict, or vary
-    the which_result argument to use a different geocode result. If you know
+    the `which_result` argument to use a different geocode result. If you know
     the OSM ID of the place, you can retrieve its boundary polygon using the
-    geocode_to_gdf function, then pass it to the graph_from_polygon function.
+    `geocode_to_gdf` function, then pass it to the `features_from_polygon`
+    function.
 
-    You can use the `settings` module to retrieve a snapshot of historical OSM
-    data as of a certain date, or to configure the Overpass server timeout,
-    memory allocation, and other custom settings.
+    This function uses filters to query the Overpass API: you can either
+    specify a pre-defined `network_type` or provide your own `custom_filter`
+    with Overpass QL.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes. You can also use the `settings` module to retrieve a snapshot
+    of historical OSM data as of a certain date, or to configure the Overpass
+    server timeout, memory allocation, and other custom settings.
 
     Parameters
     ----------
-    query : string or dict or list
-        the query or queries to geocode to get place boundary polygon(s)
-    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get if custom_filter is None
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    truncate_by_edge : bool
-        if True, retain nodes outside boundary polygon if at least one of
-        node's neighbors is within the polygon
-    which_result : int
+    query
+        The query or queries to geocode to retrieve place boundary polygon(s).
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve if `custom_filter` is None.
+    simplify
+        If True, simplify graph topology with the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    truncate_by_edge
+        If True, retain nodes outside bounding box if at least one of node's
+        neighbors is within the bounding box.
+    which_result
         which geocoding result to use. if None, auto-select the first
         (Multi)Polygon or raise an error if OSM doesn't return one.
-    buffer_dist : float
-        deprecated, do not use
-    clean_periphery : bool
-        deprecated, do not use
-    custom_filter : string
-        a custom ways filter to be used instead of the network_type presets
-        e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
-        in a network_type that is in settings.bidirectional_network_types if
-        you want graph to be fully bi-directional.
+    custom_filter
+        A custom ways filter to be used instead of the `network_type` presets,
+        e.g. `'["power"~"line"]' or '["highway"~"motorway|trunk"]'`. Also pass
+        in a `network_type` that is in `settings.bidirectional_network_types`
+        if you want the graph to be fully bidirectional.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
-    if buffer_dist is not None:
-        warn(
-            "The buffer_dist argument has been deprecated and will be removed "
-            "in the v2.0.0 release. Buffer your query area directly, if desired. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    # create a GeoDataFrame with the spatial boundaries of the place(s)
-    if isinstance(query, (str, dict)):
-        # if it is a string (place name) or dict (structured place query),
-        # then it is a single place
-        gdf_place = geocoder.geocode_to_gdf(
-            query, which_result=which_result, buffer_dist=buffer_dist
-        )
-    elif isinstance(query, list):
-        # if it is a list, it contains multiple places to get
-        gdf_place = geocoder.geocode_to_gdf(query, buffer_dist=buffer_dist)
-    else:  # pragma: no cover
-        msg = "query must be dict, string, or list of strings"
-        raise TypeError(msg)
-
-    # extract the geometry from the GeoDataFrame to use in API query
+    # extract the geometry from the GeoDataFrame to use in query
+    gdf_place = geocoder.geocode_to_gdf(query, which_result=which_result)
     polygon = gdf_place["geometry"].unary_union
-    utils.log("Constructed place geometry polygon(s) to query API")
+
+    msg = "Constructed place geometry polygon(s) to query Overpass"
+    utils.log(msg, level=lg.INFO)
 
     # create graph using this polygon(s) geometry
     G = graph_from_polygon(
         polygon,
         network_type=network_type,
         simplify=simplify,
         retain_all=retain_all,
         truncate_by_edge=truncate_by_edge,
-        clean_periphery=clean_periphery,
         custom_filter=custom_filter,
     )
 
-    utils.log(f"graph_from_place returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    msg = f"graph_from_place returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def graph_from_polygon(
-    polygon,
-    network_type="all",
-    simplify=True,
-    retain_all=False,
-    truncate_by_edge=False,
-    clean_periphery=None,
-    custom_filter=None,
-):
-    """
-    Download and create a graph within the boundaries of a (multi)polygon.
-
-    You can use the `settings` module to retrieve a snapshot of historical OSM
-    data as of a certain date, or to configure the Overpass server timeout,
-    memory allocation, and other custom settings.
+    polygon: Polygon | MultiPolygon,
+    *,
+    network_type: str = "all",
+    simplify: bool = True,
+    retain_all: bool = False,
+    truncate_by_edge: bool = False,
+    custom_filter: str | None = None,
+) -> nx.MultiDiGraph:
+    """
+    Download and create a graph within the boundaries of a (Multi)Polygon.
+
+    This function uses filters to query the Overpass API: you can either
+    specify a pre-defined `network_type` or provide your own `custom_filter`
+    with Overpass QL.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes. You can also use the `settings` module to retrieve a snapshot
+    of historical OSM data as of a certain date, or to configure the Overpass
+    server timeout, memory allocation, and other custom settings.
 
     Parameters
     ----------
-    polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        the shape to get network data within. coordinates should be in
-        unprojected latitude-longitude degrees (EPSG:4326).
-    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
-        what type of street network to get if custom_filter is None
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    truncate_by_edge : bool
-        if True, retain nodes outside boundary polygon if at least one of
-        node's neighbors is within the polygon
-    clean_periphery : bool
-        deprecated, do not use
-    custom_filter : string
-        a custom ways filter to be used instead of the network_type presets
-        e.g., '["power"~"line"]' or '["highway"~"motorway|trunk"]'. Also pass
-        in a network_type that is in settings.bidirectional_network_types if
-        you want graph to be fully bi-directional.
+    polygon
+        The geometry within which to construct the graph. Coordinates should
+        be in unprojected latitude-longitude degrees (EPSG:4326).
+    network_type
+        {"all", "all_public", "bike", "drive", "drive_service", "walk"}
+        What type of street network to retrieve if `custom_filter` is None.
+    simplify
+        If True, simplify graph topology with the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    truncate_by_edge
+        If True, retain nodes outside bounding box if at least one of node's
+        neighbors is within the bounding box.
+    custom_filter
+        A custom ways filter to be used instead of the `network_type` presets,
+        e.g. `'["power"~"line"]' or '["highway"~"motorway|trunk"]'`. Also pass
+        in a `network_type` that is in `settings.bidirectional_network_types`
+        if you want the graph to be fully bidirectional.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
 
     Notes
     -----
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
-    if clean_periphery is None:
-        clean_periphery = True
-    else:
-        warn(
-            "The clean_periphery argument has been deprecated and will be removed in "
-            "the v2.0.0 release. Future behavior will be as though clean_periphery=True. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
     # verify that the geometry is valid and is a shapely Polygon/MultiPolygon
     # before proceeding
     if not polygon.is_valid:  # pragma: no cover
-        msg = "The geometry to query within is invalid"
+        msg = "The geometry of `polygon` is invalid."
         raise ValueError(msg)
     if not isinstance(polygon, (Polygon, MultiPolygon)):  # pragma: no cover
         msg = (
             "Geometry must be a shapely Polygon or MultiPolygon. If you "
             "requested graph from place name, make sure your query resolves "
             "to a Polygon or MultiPolygon, and not some other geometry, like "
             "a Point. See OSMnx documentation for details."
         )
         raise TypeError(msg)
 
-    if clean_periphery:
-        # create a new buffered polygon 0.5km around the desired one
-        buffer_dist = 500
-        poly_proj, crs_utm = projection.project_geometry(polygon)
-        poly_proj_buff = poly_proj.buffer(buffer_dist)
-        poly_buff, _ = projection.project_geometry(poly_proj_buff, crs=crs_utm, to_latlong=True)
-
-        # download the network data from OSM within buffered polygon
-        response_jsons = _overpass._download_overpass_network(
-            poly_buff, network_type, custom_filter
-        )
+    # create a new buffered polygon 0.5km around the desired one
+    poly_proj, crs_utm = projection.project_geometry(polygon)
+    poly_proj_buff = poly_proj.buffer(500)
+    poly_buff, _ = projection.project_geometry(poly_proj_buff, crs=crs_utm, to_latlong=True)
+
+    # download the network data from OSM within buffered polygon
+    response_jsons = _overpass._download_overpass_network(poly_buff, network_type, custom_filter)
+
+    # create buffered graph from the downloaded data
+    bidirectional = network_type in settings.bidirectional_network_types
+    G_buff = _create_graph(response_jsons, bidirectional)
+
+    # truncate buffered graph to the buffered polygon and retain_all for
+    # now. needed because overpass returns entire ways that also include
+    # nodes outside the poly if the way (that is, a way with a single OSM
+    # ID) has a node inside the poly at some point.
+    G_buff = truncate.truncate_graph_polygon(G_buff, poly_buff, truncate_by_edge=truncate_by_edge)
 
-        # create buffered graph from the downloaded data
-        bidirectional = network_type in settings.bidirectional_network_types
-        G_buff = _create_graph(response_jsons, retain_all=True, bidirectional=bidirectional)
-
-        # truncate buffered graph to the buffered polygon and retain_all for
-        # now. needed because overpass returns entire ways that also include
-        # nodes outside the poly if the way (that is, a way with a single OSM
-        # ID) has a node inside the poly at some point.
-        G_buff = truncate.truncate_graph_polygon(G_buff, poly_buff, True, truncate_by_edge)
-
-        # simplify the graph topology
-        if simplify:
-            G_buff = simplification.simplify_graph(G_buff)
-
-        # truncate graph by original polygon to return graph within polygon
-        # caller wants. don't simplify again: this allows us to retain
-        # intersections along the street that may now only connect 2 street
-        # segments in the network, but in reality also connect to an
-        # intersection just outside the polygon
-        G = truncate.truncate_graph_polygon(G_buff, polygon, retain_all, truncate_by_edge)
-
-        # count how many physical streets in buffered graph connect to each
-        # intersection in un-buffered graph, to retain true counts for each
-        # intersection, even if some of its neighbors are outside the polygon
-        spn = stats.count_streets_per_node(G_buff, nodes=G.nodes)
-        nx.set_node_attributes(G, values=spn, name="street_count")
-
-    # if clean_periphery=False, just use the polygon as provided
-    else:
-        # download the network data from OSM
-        response_jsons = _overpass._download_overpass_network(polygon, network_type, custom_filter)
-
-        # create graph from the downloaded data
-        bidirectional = network_type in settings.bidirectional_network_types
-        G = _create_graph(response_jsons, retain_all=True, bidirectional=bidirectional)
-
-        # truncate the graph to the extent of the polygon
-        G = truncate.truncate_graph_polygon(G, polygon, retain_all, truncate_by_edge)
-
-        # simplify the graph topology after truncation. don't truncate after
-        # simplifying or you may have simplified out to an endpoint beyond the
-        # truncation distance, which would strip out the entire edge
-        if simplify:
-            G = simplification.simplify_graph(G)
-
-        # count how many physical streets connect to each intersection/deadend
-        # note this will be somewhat inaccurate due to periphery effects, so
-        # it's best to parameterize function with clean_periphery=True
-        spn = stats.count_streets_per_node(G)
-        nx.set_node_attributes(G, values=spn, name="street_count")
-        warn(
-            "the graph-level street_count attribute will likely be inaccurate "
-            "when you set clean_periphery=False",
-            stacklevel=2,
-        )
+    # keep only the largest weakly connected component if retain_all is False
+    if not retain_all:
+        G_buff = truncate.largest_component(G_buff, strongly=False)
+
+    # simplify the graph topology
+    if simplify:
+        G_buff = simplification.simplify_graph(G_buff)
+
+    # truncate graph by original polygon to return graph within polygon
+    # caller wants. don't simplify again: this allows us to retain
+    # intersections along the street that may now only connect 2 street
+    # segments in the network, but in reality also connect to an
+    # intersection just outside the polygon
+    G = truncate.truncate_graph_polygon(G_buff, polygon, truncate_by_edge=truncate_by_edge)
+
+    # keep only the largest weakly connected component if retain_all is False
+    # we're doing this again in case the last truncate disconnected anything
+    # on the periphery
+    if not retain_all:
+        G = truncate.largest_component(G, strongly=False)
 
-    utils.log(f"graph_from_polygon returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    # count how many physical streets in buffered graph connect to each
+    # intersection in un-buffered graph, to retain true counts for each
+    # intersection, even if some of its neighbors are outside the polygon
+    spn = stats.count_streets_per_node(G_buff, nodes=G.nodes)
+    nx.set_node_attributes(G, values=spn, name="street_count")
+
+    msg = f"graph_from_polygon returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def graph_from_xml(
-    filepath, bidirectional=False, simplify=True, retain_all=False, encoding="utf-8"
-):
-    """
-    Create a graph from data in a .osm formatted XML file.
-
-    Do not load an XML file generated by OSMnx: this use case is not supported
-    and may not behave as expected. To save/load graphs to/from disk for later
-    use in OSMnx, use the `io.save_graphml` and `io.load_graphml` functions
-    instead.
+    filepath: str | Path,
+    *,
+    bidirectional: bool = False,
+    simplify: bool = True,
+    retain_all: bool = False,
+    encoding: str = "utf-8",
+) -> nx.MultiDiGraph:
+    """
+    Create a graph from data in an OSM XML file.
+
+    Do not load an XML file previously generated by OSMnx: this use case is
+    not supported and may not behave as expected. To save/load graphs to/from
+    disk for later use in OSMnx, use the `io.save_graphml` and
+    `io.load_graphml` functions instead.
+
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which OSM node/way tags are added as graph node/edge
+    attributes.
 
     Parameters
     ----------
-    filepath : string or pathlib.Path
-        path to file containing OSM XML data
-    bidirectional : bool
-        if True, create bi-directional edges for one-way streets
-    simplify : bool
-        if True, simplify graph topology with the `simplify_graph` function
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    encoding : string
-        the XML file's character encoding
+    filepath
+        Path to file containing OSM XML data.
+    bidirectional
+        If True, create bidirectional edges for one-way streets.
+    simplify
+        If True, simplify graph topology with the `simplify_graph` function.
+    retain_all
+        If True, return the entire graph even if it is not connected. If
+        False, retain only the largest weakly connected component.
+    encoding
+        The OSM XML file's character encoding.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     # transmogrify file of OSM XML data into JSON
-    response_jsons = [osm_xml._overpass_json_from_file(filepath, encoding)]
+    response_jsons = [_osm_xml._overpass_json_from_xml(filepath, encoding)]
 
     # create graph using this response JSON
-    G = _create_graph(response_jsons, bidirectional=bidirectional, retain_all=retain_all)
+    G = _create_graph(response_jsons, bidirectional)
+
+    # keep only the largest weakly connected component if retain_all is False
+    if not retain_all:
+        G = truncate.largest_component(G, strongly=False)
 
     # simplify the graph topology as the last step
     if simplify:
         G = simplification.simplify_graph(G)
 
-    utils.log(f"graph_from_xml returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    msg = f"graph_from_xml returned graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
-def _create_graph(response_jsons, retain_all=False, bidirectional=False):
+def _create_graph(
+    response_jsons: Iterable[dict[str, Any]],
+    bidirectional: bool,  # noqa: FBT001
+) -> nx.MultiDiGraph:
     """
-    Create a networkx MultiDiGraph from Overpass API responses.
+    Create a NetworkX MultiDiGraph from Overpass API responses.
 
     Adds length attributes in meters (great-circle distance between endpoints)
     to all of the graph's (pre-simplified, straight-line) edges via the
     `distance.add_edge_lengths` function.
 
     Parameters
     ----------
-    response_jsons : iterable
-        iterable of dicts of JSON responses from from the Overpass API
-    retain_all : bool
-        if True, return the entire graph even if it is not connected.
-        otherwise, retain only the largest weakly connected component.
-    bidirectional : bool
-        if True, create bi-directional edges for one-way streets
+    response_jsons
+        Iterable of JSON responses from the Overpass API.
+    retain_all
+        If True, return the entire graph even if it is not connected.
+        Otherwise, retain only the largest weakly connected component.
+    bidirectional
+        If True, create bidirectional edges for one-way streets.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
-    response_count = 0
-    nodes = {}
-    paths = {}
+    # each dict's keys are OSM IDs and values are dicts of attributes
+    nodes: dict[int, dict[str, Any]] = {}
+    paths: dict[int, dict[str, Any]] = {}
 
     # consume response_jsons generator to download data from server
+    response_count = 0
     for response_json in response_jsons:
         response_count += 1
 
         # if cache_only_mode, consume response_jsons then continue next loop
         if settings.cache_only_mode:  # pragma: no cover
             continue
 
         # otherwise, extract nodes and paths from the downloaded OSM data
         nodes_temp, paths_temp = _parse_nodes_paths(response_json)
         nodes.update(nodes_temp)
         paths.update(paths_temp)
 
-    utils.log(f"Retrieved all data from API in {response_count} request(s)")
+    msg = f"Retrieved all data from API in {response_count} request(s)"
+    utils.log(msg, level=lg.INFO)
     if settings.cache_only_mode:  # pragma: no cover
         # after consuming all response_jsons in loop, raise exception to catch
-        msg = "Interrupted because `settings.cache_only_mode=True`"
+        msg = "Interrupted because `settings.cache_only_mode=True`."
         raise CacheOnlyInterruptError(msg)
 
     # ensure we got some node/way data back from the server request(s)
     if (len(nodes) == 0) and (len(paths) == 0):  # pragma: no cover
         msg = "No data elements in server response. Check query location/filters and log."
         raise InsufficientResponseError(msg)
 
@@ -651,180 +612,184 @@
         "created_date": utils.ts(),
         "created_with": f"OSMnx {__version__}",
         "crs": settings.default_crs,
     }
     G = nx.MultiDiGraph(**metadata)
 
     # add each OSM node and way (a path of edges) to the graph
-    utils.log(f"Creating graph from {len(nodes):,} OSM nodes and {len(paths):,} OSM ways...")
+    msg = f"Creating graph from {len(nodes):,} OSM nodes and {len(paths):,} OSM ways..."
+    utils.log(msg, level=lg.INFO)
     G.add_nodes_from(nodes.items())
     _add_paths(G, paths.values(), bidirectional)
 
-    # retain only the largest connected component if retain_all=False
-    if not retain_all:
-        G = truncate.largest_component(G)
-
-    utils.log(f"Created graph with {len(G):,} nodes and {len(G.edges):,} edges")
+    msg = f"Created graph with {len(G):,} nodes and {len(G.edges):,} edges"
+    utils.log(msg, level=lg.INFO)
 
     # add length (great-circle distance between nodes) attribute to each edge
     if len(G.edges) > 0:
         G = distance.add_edge_lengths(G)
 
     return G
 
 
-def _convert_node(element):
+def _convert_node(element: dict[str, Any]) -> dict[str, Any]:
     """
-    Convert an OSM node element into the format for a networkx node.
+    Convert an OSM node element into the format for a NetworkX node.
 
     Parameters
     ----------
-    element : dict
-        an OSM node element
+    element
+        OSM element of type "node".
 
     Returns
     -------
-    node : dict
+    node
     """
     node = {"y": element["lat"], "x": element["lon"]}
     if "tags" in element:
         for useful_tag in settings.useful_tags_node:
             if useful_tag in element["tags"]:
                 node[useful_tag] = element["tags"][useful_tag]
     return node
 
 
-def _convert_path(element):
+def _convert_path(element: dict[str, Any]) -> dict[str, Any]:
     """
-    Convert an OSM way element into the format for a networkx path.
+    Convert an OSM way element into the format for a NetworkX path.
 
     Parameters
     ----------
-    element : dict
-        an OSM way element
+    element
+        OSM element of type "way".
 
     Returns
     -------
-    path : dict
+    path
     """
     path = {"osmid": element["id"]}
 
     # remove any consecutive duplicate elements in the list of nodes
-    path["nodes"] = [group[0] for group in itertools.groupby(element["nodes"])]
+    path["nodes"] = [group[0] for group in groupby(element["nodes"])]
 
     if "tags" in element:
         for useful_tag in settings.useful_tags_way:
             if useful_tag in element["tags"]:
                 path[useful_tag] = element["tags"][useful_tag]
     return path
 
 
-def _parse_nodes_paths(response_json):
+def _parse_nodes_paths(
+    response_json: dict[str, Any],
+) -> tuple[dict[int, dict[str, Any]], dict[int, dict[str, Any]]]:
     """
     Construct dicts of nodes and paths from an Overpass response.
 
     Parameters
     ----------
-    response_json : dict
-        JSON response from the Overpass API
+    response_json
+        JSON response from the Overpass API.
 
     Returns
     -------
-    nodes, paths : tuple of dicts
-        dicts' keys = osmid and values = dict of attributes
+    nodes, paths
+        Each dict's keys are OSM IDs and values are dicts of attributes.
     """
     nodes = {}
     paths = {}
     for element in response_json["elements"]:
         if element["type"] == "node":
             nodes[element["id"]] = _convert_node(element)
         elif element["type"] == "way":
             paths[element["id"]] = _convert_path(element)
 
     return nodes, paths
 
 
-def _is_path_one_way(path, bidirectional, oneway_values):
+def _is_path_one_way(attrs: dict[str, Any], bidirectional: bool, oneway_values: set[str]) -> bool:  # noqa: FBT001
     """
     Determine if a path of nodes allows travel in only one direction.
 
     Parameters
     ----------
-    path : dict
-        a path's `tag:value` attribute data
-    bidirectional : bool
-        whether this is a bi-directional network type
-    oneway_values : set
-        the values OSM uses in its 'oneway' tag to denote True
+    attrs
+        A path's `tag:value` attribute data.
+    bidirectional
+        Whether this is a bidirectional network type.
+    oneway_values
+        The values OSM uses in its "oneway" tag to denote True.
 
     Returns
     -------
-    bool
+    is_one_way
     """
     # rule 1
     if settings.all_oneway:
         # if globally configured to set every edge one-way, then it's one-way
         return True
 
     # rule 2
     if bidirectional:
-        # if this is a bi-directional network type, then nothing in it is
+        # if this is a bidirectional network type, then nothing in it is
         # considered one-way. eg, if this is a walking network, this may very
         # well be a one-way street (as cars/bikes go), but in a walking-only
-        # network it is a bi-directional edge (you can walk both directions on
+        # network it is a bidirectional edge (you can walk both directions on
         # a one-way street). so we will add this path (in both directions) to
         # the graph and set its oneway attribute to False.
         return False
 
     # rule 3
-    if "oneway" in path and path["oneway"] in oneway_values:
-        # if this path is tagged as one-way and if it is not a bi-directional
+    if "oneway" in attrs and attrs["oneway"] in oneway_values:
+        # if this path is tagged as one-way and if it is not a bidirectional
         # network type then we'll add the path in one direction only
         return True
 
     # rule 4
-    if "junction" in path and path["junction"] == "roundabout":
+    if "junction" in attrs and attrs["junction"] == "roundabout":
         # roundabouts are also one-way but are not explicitly tagged as such
         return True
 
     # otherwise, if no rule passed then this path is not tagged as a one-way
     return False
 
 
-def _is_path_reversed(path, reversed_values):
+def _is_path_reversed(attrs: dict[str, Any], reversed_values: set[str]) -> bool:
     """
     Determine if the order of nodes in a path should be reversed.
 
     Parameters
     ----------
-    path : dict
-        a path's `tag:value` attribute data
-    reversed_values : set
-        the values OSM uses in its 'oneway' tag to denote travel can only
-        occur in the opposite direction of the node order
+    attrs
+        A path's `tag:value` attribute data.
+    reversed_values
+        The values OSM uses in its 'oneway' tag to denote travel can only
+        occur in the opposite direction of the node order.
 
     Returns
     -------
-    bool
+    is_reversed
     """
-    return "oneway" in path and path["oneway"] in reversed_values
+    return "oneway" in attrs and attrs["oneway"] in reversed_values
 
 
-def _add_paths(G, paths, bidirectional=False):
+def _add_paths(
+    G: nx.MultiDiGraph,
+    paths: Iterable[dict[str, Any]],
+    bidirectional: bool,  # noqa: FBT001
+) -> None:
     """
-    Add a list of paths to the graph as edges.
+    Add OSM paths to the graph as edges.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        graph to add paths to
-    paths : list
-        list of paths' `tag:value` attribute data dicts
-    bidirectional : bool
-        if True, create bi-directional edges for one-way streets
+    G
+        The graph to add paths to.
+    paths
+        Iterable of paths' `tag:value` attribute data dicts.
+    bidirectional
+        If True, create bidirectional edges for one-way streets.
 
     Returns
     -------
     None
     """
     # the values OSM uses in its 'oneway' tag to denote True, and to denote
     # travel can only occur in the opposite direction of the node order. see:
```

### Comparing `osmnx-1.9.3/osmnx/io.py` & `osmnx-2.0.0b0/osmnx/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,54 @@
-"""Serialize graphs to/from files on disk."""
+"""File I/O functions to save/load graphs to/from files on disk."""
+
+from __future__ import annotations
 
 import ast
 import contextlib
+import logging as lg
 from pathlib import Path
-from warnings import warn
+from typing import TYPE_CHECKING
+from typing import Any
 
 import networkx as nx
 import pandas as pd
 from shapely import wkt
 
+from . import _osm_xml
 from . import convert
-from . import osm_xml
 from . import settings
 from . import utils
 
+if TYPE_CHECKING:
+    import geopandas as gpd
+
 
-def save_graph_geopackage(G, filepath=None, encoding="utf-8", directed=False):
+def save_graph_geopackage(
+    G: nx.MultiDiGraph,
+    filepath: str | Path | None = None,
+    *,
+    directed: bool = False,
+    encoding: str = "utf-8",
+) -> None:
     """
     Save graph nodes and edges to disk as layers in a GeoPackage file.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    filepath : string or pathlib.Path
-        path to the GeoPackage file including extension. if None, use default
-        data folder + graph.gpkg
-    encoding : string
-        the character encoding for the saved file
-    directed : bool
-        if False, save one edge for each undirected edge in the graph but
-        retain original oneway and to/from information as edge attributes; if
-        True, save one edge for each directed edge in the graph
+    G
+        The graph to save.
+    filepath
+        Path to the GeoPackage file including extension. If None, use default
+        `settings.data_folder/graph.gpkg`.
+    directed
+        If False, save one edge for each undirected edge in the graph but
+        retain original oneway and to/from information as edge attributes. If
+        True, save one edge for each directed edge in the graph.
+    encoding
+        The character encoding of the saved GeoPackage file.
 
     Returns
     -------
     None
     """
     # default filepath if none was provided
     filepath = Path(settings.data_folder) / "graph.gpkg" if filepath is None else Path(filepath)
@@ -50,93 +63,41 @@
         gdf_nodes, gdf_edges = convert.graph_to_gdfs(convert.to_undirected(G))
     gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
     gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
 
     # save the nodes and edges as GeoPackage layers
     gdf_nodes.to_file(filepath, layer="nodes", driver="GPKG", index=True, encoding=encoding)
     gdf_edges.to_file(filepath, layer="edges", driver="GPKG", index=True, encoding=encoding)
-    utils.log(f"Saved graph as GeoPackage at {filepath!r}")
-
-
-def save_graph_shapefile(G, filepath=None, encoding="utf-8", directed=False):
-    """
-    Do not use: deprecated. Use the save_graph_geopackage function instead.
 
-    The Shapefile format is proprietary and outdated. Instead, use the
-    superior GeoPackage file format via the save_graph_geopackage function.
-    See http://switchfromshapefile.org/ for more information.
+    msg = f"Saved graph as GeoPackage at {filepath!r}"
+    utils.log(msg, level=lg.INFO)
 
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        input graph
-    filepath : string or pathlib.Path
-        path to the shapefiles folder (no file extension). if None, use
-        default data folder + graph_shapefile
-    encoding : string
-        the character encoding for the saved files
-    directed : bool
-        if False, save one edge for each undirected edge in the graph but
-        retain original oneway and to/from information as edge attributes; if
-        True, save one edge for each directed edge in the graph
 
-    Returns
-    -------
-    None
-    """
-    warn(
-        "The `save_graph_shapefile` function is deprecated and will be removed "
-        "in the v2.0.0 release. Instead, use the `save_graph_geopackage` function "
-        "to save graphs as GeoPackage files for subsequent GIS analysis. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-
-    # default filepath if none was provided
-    filepath = (
-        Path(settings.data_folder) / "graph_shapefile" if filepath is None else Path(filepath)
-    )
-
-    # if save folder does not already exist, create it (shapefiles
-    # get saved as set of files)
-    filepath.mkdir(parents=True, exist_ok=True)
-    filepath_nodes = filepath / "nodes.shp"
-    filepath_edges = filepath / "edges.shp"
-
-    # convert graph to gdfs and stringify non-numeric columns
-    if directed:
-        gdf_nodes, gdf_edges = convert.graph_to_gdfs(G)
-    else:
-        gdf_nodes, gdf_edges = convert.graph_to_gdfs(convert.to_undirected(G))
-    gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
-    gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
-
-    # save the nodes and edges as separate ESRI shapefiles
-    gdf_nodes.to_file(filepath_nodes, driver="ESRI Shapefile", index=True, encoding=encoding)
-    gdf_edges.to_file(filepath_edges, driver="ESRI Shapefile", index=True, encoding=encoding)
-    utils.log(f"Saved graph as shapefiles at {filepath!r}")
-
-
-def save_graphml(G, filepath=None, gephi=False, encoding="utf-8"):
+def save_graphml(
+    G: nx.MultiDiGraph,
+    filepath: str | Path | None = None,
+    *,
+    gephi: bool = False,
+    encoding: str = "utf-8",
+) -> None:
     """
     Save graph to disk as GraphML file.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    filepath : string or pathlib.Path
-        path to the GraphML file including extension. if None, use default
-        data folder + graph.graphml
-    gephi : bool
-        if True, give each edge a unique key/id to work around Gephi's
-        interpretation of the GraphML specification
-    encoding : string
-        the character encoding for the saved file
+    G
+        The graph to save as.
+    filepath
+        Path to the GraphML file including extension. If None, use default
+        `settings.data_folder/graph.graphml`.
+    gephi
+        If True, give each edge a unique key/id for compatibility with Gephi's
+        interpretation of the GraphML specification.
+    encoding
+        The character encoding of the saved GraphML file.
 
     Returns
     -------
     None
     """
     # default filepath if none was provided
     filepath = Path(settings.data_folder) / "graph.graphml" if filepath is None else Path(filepath)
@@ -164,20 +125,26 @@
 
     # stringify all the edge attribute values
     for _, _, data in G.edges(keys=False, data=True):
         for attr, value in data.items():
             data[attr] = str(value)
 
     nx.write_graphml(G, path=filepath, encoding=encoding)
-    utils.log(f"Saved graph as GraphML file at {filepath!r}")
+    msg = f"Saved graph as GraphML file at {filepath!r}"
+    utils.log(msg, level=lg.INFO)
 
 
 def load_graphml(
-    filepath=None, graphml_str=None, node_dtypes=None, edge_dtypes=None, graph_dtypes=None
-):
+    filepath: str | Path | None = None,
+    *,
+    graphml_str: str | None = None,
+    node_dtypes: dict[str, Any] | None = None,
+    edge_dtypes: dict[str, Any] | None = None,
+    graph_dtypes: dict[str, Any] | None = None,
+) -> nx.MultiDiGraph:
     """
     Load an OSMnx-saved GraphML file from disk or GraphML string.
 
     This function converts node, edge, and graph-level attributes (serialized
     as strings) to their appropriate data types. These can be customized as
     needed by passing in dtypes arguments providing types or custom converter
     functions. For example, if you want to convert some attribute's values to
@@ -190,46 +157,43 @@
 
     Note that you must pass one and only one of `filepath` or `graphml_str`.
     If passing `graphml_str`, you may need to decode the bytes read from your
     file before converting to string to pass to this function.
 
     Parameters
     ----------
-    filepath : string or pathlib.Path
-        path to the GraphML file
-    graphml_str : string
-        a valid and decoded string representation of a GraphML file's contents
-    node_dtypes : dict
-        dict of node attribute names:types to convert values' data types. the
-        type can be a python type or a custom string converter function.
-    edge_dtypes : dict
-        dict of edge attribute names:types to convert values' data types. the
-        type can be a python type or a custom string converter function.
-    graph_dtypes : dict
-        dict of graph-level attribute names:types to convert values' data
-        types. the type can be a python type or a custom string converter
-        function.
+    filepath
+        Path to the GraphML file.
+    graphml_str
+        Valid and decoded string representation of a GraphML file's contents.
+    node_dtypes
+        Dict of node attribute names:types to convert values' data types. The
+        type can be a type or a custom string converter function.
+    edge_dtypes
+        Dict of edge attribute names:types to convert values' data types. The
+        type can be a type or a custom string converter function.
+    graph_dtypes
+        Dict of graph-level attribute names:types to convert values' data
+        types. The type can be a type or a custom string converter function.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     if (filepath is None and graphml_str is None) or (
         filepath is not None and graphml_str is not None
     ):  # pragma: no cover
         msg = "You must pass one and only one of `filepath` or `graphml_str`."
         raise ValueError(msg)
 
     # specify default graph/node/edge attribute values' data types
     default_graph_dtypes = {"simplified": _convert_bool_string}
     default_node_dtypes = {
         "elevation": float,
         "elevation_res": float,
-        "lat": float,
-        "lon": float,
         "osmid": int,
         "street_count": int,
         "x": float,
         "y": float,
     }
     default_edge_dtypes = {
         "bearing": float,
@@ -251,149 +215,129 @@
     if edge_dtypes is not None:
         default_edge_dtypes.update(edge_dtypes)
 
     if filepath is not None:
         # read the graphml file from disk
         source = filepath
         G = nx.read_graphml(
-            Path(filepath), node_type=default_node_dtypes["osmid"], force_multigraph=True
+            Path(filepath),
+            node_type=default_node_dtypes["osmid"],
+            force_multigraph=True,
         )
     else:
         # parse the graphml string
         source = "string"
         G = nx.parse_graphml(
-            graphml_str, node_type=default_node_dtypes["osmid"], force_multigraph=True
+            graphml_str,
+            node_type=default_node_dtypes["osmid"],
+            force_multigraph=True,
         )
 
     # convert graph/node/edge attribute data types
-    utils.log("Converting node, edge, and graph-level attribute data types")
+    msg = "Converting node, edge, and graph-level attribute data types"
+    utils.log(msg, level=lg.INFO)
     G = _convert_graph_attr_types(G, default_graph_dtypes)
     G = _convert_node_attr_types(G, default_node_dtypes)
     G = _convert_edge_attr_types(G, default_edge_dtypes)
 
-    utils.log(f"Loaded graph with {len(G)} nodes and {len(G.edges)} edges from {source!r}")
+    msg = f"Loaded graph with {len(G)} nodes and {len(G.edges)} edges from {source!r}"
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def save_graph_xml(
-    data,
-    filepath=None,
-    node_tags=None,
-    node_attrs=None,
-    edge_tags=None,
-    edge_attrs=None,
-    oneway=None,
-    merge_edges=None,
-    edge_tag_aggs=None,
-    api_version=None,
-    precision=None,
-    way_tag_aggs=None,
-):
+    G: nx.MultiDiGraph,
+    filepath: str | Path | None = None,
+    *,
+    way_tag_aggs: dict[str, Any] | None = None,
+    encoding: str = "utf-8",
+) -> None:
     """
-    Save graph to disk as an OSM-formatted XML .osm file.
+    Save graph to disk as an OSM XML file.
 
-    This function exists only to allow serialization to the .osm file format
+    This function exists only to allow serialization to the OSM XML format
     for applications that require it, and has constraints to conform to that.
-    As such, this function has a limited use case which does not include
-    saving/loading graphs for subsequent OSMnx analysis. To save/load graphs
-    to/from disk for later use in OSMnx, use the `io.save_graphml` and
-    `io.load_graphml` functions instead. To load a graph from a .osm file that
-    you have downloaded or generated elsewhere, use the `graph.graph_from_xml`
+    As such, it has a limited use case which does not include saving/loading
+    graphs for subsequent OSMnx analysis. To save/load graphs to/from disk for
+    later use in OSMnx, use the `io.save_graphml` and `io.load_graphml`
+    functions instead. To load a graph from an OSM XML file that you have
+    downloaded or generated elsewhere, use the `graph.graph_from_xml`
     function.
 
+    Use the `settings` module's `useful_tags_node` and `useful_tags_way`
+    settings to configure which tags your graph is created and saved with.
+    This function merges graph edges such that each OSM way has one entry in
+    the XML output, with the way's nodes topologically sorted. `G` must be
+    unsimplified to save as OSM XML: otherwise, one edge could comprise
+    multiple OSM ways, making it impossible to group and sort edges in way.
+    `G` should also have been created with `ox.settings.all_oneway=True` for
+    this function to behave properly.
+
     Parameters
     ----------
-    data : networkx.MultiDiGraph
-        the input graph
-    filepath : string or pathlib.Path
-        do not use, deprecated
-    node_tags : list
-        do not use, deprecated
-    node_attrs: list
-        do not use, deprecated
-    edge_tags : list
-        do not use, deprecated
-    edge_attrs : list
-        do not use, deprecated
-    oneway : bool
-        do not use, deprecated
-    merge_edges : bool
-        do not use, deprecated
-    edge_tag_aggs : tuple
-        do not use, deprecated
-    api_version : float
-        do not use, deprecated
-    precision : int
-        do not use, deprecated
-    way_tag_aggs : dict
+    G
+        Unsimplified, unprojected graph to save as an OSM XML file.
+    filepath
+        Path to the saved file including extension. If None, use default
+        `settings.data_folder/graph.osm`.
+    way_tag_aggs
         Keys are OSM way tag keys and values are aggregation functions
         (anything accepted as an argument by pandas.agg). Allows user to
         aggregate graph edge attribute values into single OSM way values. If
         None, or if some tag's key does not exist in the dict, the way
         attribute will be assigned the value of the first edge of the way.
+    encoding
+        The character encoding of the saved OSM XML file.
 
     Returns
     -------
     None
     """
-    osm_xml._save_graph_xml(
-        data,
-        filepath,
-        node_tags,
-        node_attrs,
-        edge_tags,
-        edge_attrs,
-        oneway,
-        merge_edges,
-        edge_tag_aggs,
-        api_version,
-        precision,
-        way_tag_aggs,
-    )
+    _osm_xml._save_graph_xml(G, filepath, way_tag_aggs, encoding)
 
 
-def _convert_graph_attr_types(G, dtypes=None):
+def _convert_graph_attr_types(G: nx.MultiDiGraph, dtypes: dict[str, Any]) -> nx.MultiDiGraph:
     """
     Convert graph-level attributes using a dict of data types.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    dtypes : dict
-        dict of graph-level attribute names:types
+    G
+        Graph to convert the graph-level attributes of.
+    dtypes
+        Dict of graph-level attribute names:types.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     # remove node_default and edge_default metadata keys if they exist
     G.graph.pop("node_default", None)
     G.graph.pop("edge_default", None)
 
     for attr in G.graph.keys() & dtypes.keys():
         G.graph[attr] = dtypes[attr](G.graph[attr])
 
     return G
 
 
-def _convert_node_attr_types(G, dtypes=None):
+def _convert_node_attr_types(G: nx.MultiDiGraph, dtypes: dict[str, Any]) -> nx.MultiDiGraph:
     """
     Convert graph nodes' attributes using a dict of data types.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    dtypes : dict
-        dict of node attribute names:types
+    G
+        Graph to convert the node attributes of.
+    dtypes
+        Dict of node attribute names:types.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     for _, data in G.nodes(data=True):
         # first, eval stringified lists, dicts, or sets to convert them to objects
         # lists, dicts, or sets would be custom attribute types added by a user
         for attr, value in data.items():
             if (value.startswith("[") and value.endswith("]")) or (
                 value.startswith("{") and value.endswith("}")
@@ -402,28 +346,28 @@
                     data[attr] = ast.literal_eval(value)
 
         for attr in data.keys() & dtypes.keys():
             data[attr] = dtypes[attr](data[attr])
     return G
 
 
-def _convert_edge_attr_types(G, dtypes=None):
+def _convert_edge_attr_types(G: nx.MultiDiGraph, dtypes: dict[str, Any]) -> nx.MultiDiGraph:
     """
     Convert graph edges' attributes using a dict of data types.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    dtypes : dict
-        dict of edge attribute names:types
+    G
+        Graph to convert the edge attributes of.
+    dtypes
+        Dict of edge attribute names:types.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
+    G
     """
     # for each edge in the graph, eval attribute value lists and convert types
     for _, _, data in G.edges(data=True, keys=False):
         # remove extraneous "id" attribute added by graphml saving
         data.pop("id", None)
 
         # first, eval stringified lists, dicts, or sets to convert them to objects
@@ -448,61 +392,61 @@
         # if "geometry" attr exists, convert its well-known text to LineString
         if "geometry" in data:
             data["geometry"] = wkt.loads(data["geometry"])
 
     return G
 
 
-def _convert_bool_string(value):
+def _convert_bool_string(value: bool | str) -> bool:
     """
     Convert a "True" or "False" string literal to corresponding boolean type.
 
     This is necessary because Python will otherwise parse the string "False"
     to the boolean value True, that is, `bool("False") == True`. This function
     raises a ValueError if a value other than "True" or "False" is passed.
 
     If the value is already a boolean, this function just returns it, to
     accommodate usage when the value was originally inside a stringified list.
 
     Parameters
     ----------
-    value : string {"True", "False"}
-        the value to convert
+    value
+        The string value to convert to bool.
 
     Returns
     -------
-    bool
+    bool_value
     """
-    if value in {"True", "False"}:
-        return value == "True"
-
     if isinstance(value, bool):
         return value
 
+    if value in {"True", "False"}:
+        return value == "True"
+
     # otherwise the value is not a valid boolean
-    msg = f"invalid literal for boolean: {value!r}"
+    msg = f"Invalid literal for boolean: {value!r}."
     raise ValueError(msg)
 
 
-def _stringify_nonnumeric_cols(gdf):
+def _stringify_nonnumeric_cols(gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     """
     Make every non-numeric GeoDataFrame column (besides geometry) a string.
 
     This allows proper serializing via Fiona of GeoDataFrames with mixed types
     such as strings and ints in the same column.
 
     Parameters
     ----------
-    gdf : geopandas.GeoDataFrame
-        gdf to stringify non-numeric columns of
+    gdf
+        GeoDataFrame to stringify non-numeric columns of.
 
     Returns
     -------
-    gdf : geopandas.GeoDataFrame
-        gdf with non-numeric columns stringified
+    gdf
+        GeoDataFrame with non-numeric columns stringified.
     """
     # stringify every non-numeric column other than geometry column
     for col in (c for c in gdf.columns if c != "geometry"):
         if not pd.api.types.is_numeric_dtype(gdf[col]):
             gdf[col] = gdf[col].fillna("").astype(str)
 
     return gdf
```

### Comparing `osmnx-1.9.3/osmnx/plot.py` & `osmnx-2.0.0b0/osmnx/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,334 +1,355 @@
 """Visualize street networks, routes, orientations, and geospatial features."""
 
+from __future__ import annotations
+
+import logging as lg
+from collections.abc import Iterable
+from collections.abc import Sequence
 from pathlib import Path
-from warnings import warn
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import Literal
+from typing import overload
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from . import bearing
 from . import convert
-from . import graph
 from . import projection
 from . import settings
-from . import simplification
 from . import utils
 from . import utils_geo
 
+if TYPE_CHECKING:
+    import geopandas as gpd
+
 # matplotlib is an optional dependency needed for visualization
 try:
     import matplotlib.pyplot as plt
     from matplotlib import cm
     from matplotlib import colormaps
     from matplotlib import colors
+    from matplotlib.axes._axes import Axes  # noqa: TCH002
+    from matplotlib.figure import Figure  # noqa: TCH002
+    from matplotlib.projections.polar import PolarAxes  # noqa: TCH002
+
+    mpl_available = True
+
 except ImportError:  # pragma: no cover
-    cm = colors = plt = colormaps = None  # type: ignore[assignment]
+    mpl_available = False
 
 
-def get_colors(n, cmap="viridis", start=0.0, stop=1.0, alpha=1.0, return_hex=None):
+def get_colors(
+    n: int,
+    *,
+    cmap: str = "viridis",
+    start: float = 0,
+    stop: float = 1,
+    alpha: float | None = None,
+) -> list[str]:
     """
-    Get `n` evenly-spaced colors from a matplotlib colormap.
+    Return `n` evenly-spaced colors from a matplotlib colormap.
 
     Parameters
     ----------
-    n : int
-        number of colors
-    cmap : string
-        name of a matplotlib colormap
-    start : float
-        where to start in the colorspace
-    stop : float
-        where to end in the colorspace
-    alpha : float
+    n
+        How many colors to generate.
+    cmap
+        Name of the matplotlib colormap from which to choose the colors.
+    start
+        Where to start in the colorspace (from 0 to 1).
+    stop
+        Where to end in the colorspace (from 0 to 1).
+    alpha
         If `None`, return colors as HTML-like hex triplet "#rrggbb" RGB
         strings. If `float`, return as "#rrggbbaa" RGBa strings.
-    return_hex : bool
-        deprecated, do not use
 
     Returns
     -------
-    color_list : list
+    color_list
     """
-    if return_hex is None:
-        return_hex = False
-    else:
-        warn(
-            "The `return_hex` parameter has been deprecated and will be removed "
-            "in the v2.0.0 release. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-            FutureWarning,
-            stacklevel=2,
-        )
-
     _verify_mpl()
-
-    color_list = [colormaps[cmap](x) for x in np.linspace(start, stop, n)]
+    color_gen = (colormaps[cmap](x) for x in np.linspace(start, stop, n))
     keep_alpha = alpha is not None
     if keep_alpha:
-        color_list = [(r, g, b, alpha) for r, g, b, _ in color_list]
-    else:
-        color_list = [(r, g, b) for r, g, b, _ in color_list]
-
-    if return_hex:
-        return [colors.to_hex(c, keep_alpha=keep_alpha) for c in color_list]
-
-    return color_list
+        color_gen = ((r, g, b, alpha) for r, g, b, _ in color_gen)
+    return [colors.to_hex(c, keep_alpha=keep_alpha) for c in color_gen]
 
 
 def get_node_colors_by_attr(
-    G, attr, num_bins=None, cmap="viridis", start=0, stop=1, na_color="none", equal_size=False
-):
+    G: nx.MultiDiGraph,
+    attr: str,
+    *,
+    num_bins: int | None = None,
+    cmap: str = "viridis",
+    start: float = 0,
+    stop: float = 1,
+    na_color: str = "none",
+    equal_size: bool = False,
+) -> pd.Series:  # type: ignore[type-arg]
     """
-    Get colors based on node attribute values.
+    Return colors based on nodes' numerical attribute values.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    attr : string
-        name of a numerical node attribute
-    num_bins : int
-        if None, linearly map a color to each value. otherwise, assign values
+    G
+        Input graph.
+    attr
+        Name of a node attribute with numerical values.
+    num_bins
+        If None, linearly map a color to each value. Otherwise, assign values
         to this many bins then assign a color to each bin.
-    cmap : string
-        name of a matplotlib colormap
-    start : float
-        where to start in the colorspace
-    stop : float
-        where to end in the colorspace
-    na_color : string
-        what color to assign nodes with missing attr values
-    equal_size : bool
-        ignored if num_bins is None. if True, bin into equal-sized quantiles
-        (requires unique bin edges). if False, bin into equal-spaced bins.
+    cmap
+        Name of the matplotlib colormap from which to choose the colors.
+    start
+        Where to start in the colorspace (from 0 to 1).
+    stop
+        Where to end in the colorspace (from 0 to 1).
+    na_color
+        The color to assign to nodes with missing `attr` values.
+    equal_size
+        Ignored if `num_bins` is None. If True, bin into equal-sized quantiles
+        (requires unique bin edges). If False, bin into equal-spaced bins.
 
     Returns
     -------
-    node_colors : pandas.Series
-        series labels are node IDs and values are colors
+    node_colors
+        Labels are node IDs, values are colors as hex strings.
     """
-    _verify_mpl()
     vals = pd.Series(nx.get_node_attributes(G, attr))
     return _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size)
 
 
 def get_edge_colors_by_attr(
-    G, attr, num_bins=None, cmap="viridis", start=0, stop=1, na_color="none", equal_size=False
-):
+    G: nx.MultiDiGraph,
+    attr: str,
+    *,
+    num_bins: int | None = None,
+    cmap: str = "viridis",
+    start: float = 0,
+    stop: float = 1,
+    na_color: str = "none",
+    equal_size: bool = False,
+) -> pd.Series:  # type: ignore[type-arg]
     """
-    Get colors based on edge attribute values.
+    Return colors based on edges' numerical attribute values.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    attr : string
-        name of a numerical edge attribute
-    num_bins : int
-        if None, linearly map a color to each value. otherwise, assign values
+    G
+        Input graph.
+    attr
+        Name of a node attribute with numerical values.
+    num_bins
+        If None, linearly map a color to each value. Otherwise, assign values
         to this many bins then assign a color to each bin.
-    cmap : string
-        name of a matplotlib colormap
-    start : float
-        where to start in the colorspace
-    stop : float
-        where to end in the colorspace
-    na_color : string
-        what color to assign edges with missing attr values
-    equal_size : bool
-        ignored if num_bins is None. if True, bin into equal-sized quantiles
-        (requires unique bin edges). if False, bin into equal-spaced bins.
+    cmap
+        Name of the matplotlib colormap from which to choose the colors.
+    start
+        Where to start in the colorspace (from 0 to 1).
+    stop
+        Where to end in the colorspace (from 0 to 1).
+    na_color
+        The color to assign to nodes with missing `attr` values.
+    equal_size
+        Ignored if `num_bins` is None. If True, bin into equal-sized quantiles
+        (requires unique bin edges). If False, bin into equal-spaced bins.
 
     Returns
     -------
-    edge_colors : pandas.Series
-        series labels are edge IDs (u, v, key) and values are colors
+    edge_colors
+        Labels are `(u, v, k)` edge IDs, values are colors as hex strings.
     """
-    _verify_mpl()
     vals = pd.Series(nx.get_edge_attributes(G, attr))
     return _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size)
 
 
-def plot_graph(
-    G,
-    ax=None,
-    figsize=(8, 8),
-    bgcolor="#111111",
-    node_color="w",
-    node_size=15,
-    node_alpha=None,
-    node_edgecolor="none",
-    node_zorder=1,
-    edge_color="#999999",
-    edge_linewidth=1,
-    edge_alpha=None,
-    show=True,
-    close=False,
-    save=False,
-    filepath=None,
-    dpi=300,
-    bbox=None,
-):
+def plot_graph(  # noqa: PLR0913
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    ax: Axes | None = None,
+    figsize: tuple[float, float] = (8, 8),
+    bgcolor: str = "#111111",
+    node_color: str | Sequence[str] = "w",
+    node_size: float | Sequence[float] = 15,
+    node_alpha: float | None = None,
+    node_edgecolor: str | Iterable[str] = "none",
+    node_zorder: int = 1,
+    edge_color: str | Iterable[str] = "#999999",
+    edge_linewidth: float | Sequence[float] = 1,
+    edge_alpha: float | None = None,
+    bbox: tuple[float, float, float, float] | None = None,
+    show: bool = True,
+    close: bool = False,
+    save: bool = False,
+    filepath: str | Path | None = None,
+    dpi: int = 300,
+) -> tuple[Figure, Axes]:
     """
     Visualize a graph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    ax : matplotlib axis
-        if not None, plot on this preexisting axis
-    figsize : tuple
-        if ax is None, create new figure with size (width, height)
-    bgcolor : string
-        background color of plot
-    node_color : string or list
-        color(s) of the nodes
-    node_size : int
-        size of the nodes: if 0, then skip plotting the nodes
-    node_alpha : float
-        opacity of the nodes, note: if you passed RGBA values to node_color,
-        set node_alpha=None to use the alpha channel in node_color
-    node_edgecolor : string
-        color of the nodes' markers' borders
-    node_zorder : int
-        zorder to plot nodes: edges are always 1, so set node_zorder=0 to plot
-        nodes below edges
-    edge_color : string or list
-        color(s) of the edges' lines
-    edge_linewidth : float
-        width of the edges' lines: if 0, then skip plotting the edges
-    edge_alpha : float
-        opacity of the edges, note: if you passed RGBA values to edge_color,
-        set edge_alpha=None to use the alpha channel in edge_color
-    show : bool
-        if True, call pyplot.show() to show the figure
-    close : bool
-        if True, call pyplot.close() to close the figure
-    save : bool
-        if True, save the figure to disk at filepath
-    filepath : string
-        if save is True, the path to the file. file format determined from
-        extension. if None, use settings.imgs_folder/image.png
-    dpi : int
-        if save is True, the resolution of saved file
-    bbox : tuple
-        bounding box as (north, south, east, west). if None, will calculate
+    G
+        Input graph.
+    ax
+        If not None, plot on this pre-existing axes instance.
+    figsize
+        If `ax` is None, create new figure with size `(width, height)`.
+    bgcolor
+        Background color of the figure.
+    node_color
+        Color(s) of the nodes.
+    node_size
+        Size(s) of the nodes. If 0, then skip plotting the nodes.
+    node_alpha
+        Opacity of the nodes. If you passed RGBa values to `node_color`, set
+        `node_alpha=None` to use the alpha channel in `node_color`.
+    node_edgecolor
+        Color(s) of the nodes' markers' borders.
+    node_zorder
+        The zorder to plot nodes. Edges are always 1, so set `node_zorder=0`
+        to plot nodes beneath edges.
+    edge_color
+        Color(s) of the edges' lines.
+    edge_linewidth
+        Width(s) of the edges' lines. If 0, then skip plotting the edges.
+    edge_alpha
+        Opacity of the edges. If you passed RGBa values to `edge_color`, set
+        `edge_alpha=None` to use the alpha channel in `edge_color`.
+    bbox
+        Bounding box as `(north, south, east, west)`. If None, calculate it
         from spatial extents of plotted geometries.
+    show
+        If True, call `pyplot.show()` to show the figure.
+    close
+        If True, call `pyplot.close()` to close the figure.
+    save
+        If True, save the figure to disk at `filepath`.
+    filepath
+        The path to the file if `save` is True. File format is determined from
+        the extension. If None, save at `settings.imgs_folder/image.png`.
+    dpi
+        The resolution of saved file if `save` is True.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     _verify_mpl()
-    max_node_size = max(node_size) if hasattr(node_size, "__iter__") else node_size
-    max_edge_lw = max(edge_linewidth) if hasattr(edge_linewidth, "__iter__") else edge_linewidth
+    max_node_size = max(node_size) if isinstance(node_size, Sequence) else node_size
+    max_edge_lw = max(edge_linewidth) if isinstance(edge_linewidth, Sequence) else edge_linewidth
     if max_node_size <= 0 and max_edge_lw <= 0:  # pragma: no cover
-        msg = "Either node_size or edge_linewidth must be > 0 to plot something."
+        msg = "Either `node_size` or `edge_linewidth` must be > 0 to plot something."
         raise ValueError(msg)
 
     # create fig, ax as needed
-    utils.log("Begin plotting the graph...")
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
-        ax.set_facecolor(bgcolor)
-    else:
-        fig = ax.figure
+    msg = "Begin plotting the graph..."
+    utils.log(msg, level=lg.INFO)
+    fig, ax = _get_fig_ax(ax=ax, figsize=figsize, bgcolor=bgcolor, polar=False)
 
     if max_edge_lw > 0:
         # plot the edges' geometries
         gdf_edges = convert.graph_to_gdfs(G, nodes=False)["geometry"]
         ax = gdf_edges.plot(ax=ax, color=edge_color, lw=edge_linewidth, alpha=edge_alpha, zorder=1)
 
     if max_node_size > 0:
         # scatter plot the nodes' x/y coordinates
         gdf_nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
-        ax.scatter(
+        ax.scatter(  # type: ignore[union-attr]
             x=gdf_nodes["x"],
             y=gdf_nodes["y"],
             s=node_size,
             c=node_color,
             alpha=node_alpha,
             edgecolor=node_edgecolor,
             zorder=node_zorder,
         )
 
     # get spatial extents from bbox parameter or the edges' geometries
-    padding = 0
+    padding = 0.0
     if bbox is None:
         try:
             west, south, east, north = gdf_edges.total_bounds
         except NameError:
             west, south = gdf_nodes.min()
             east, north = gdf_nodes.max()
         bbox = north, south, east, west
         padding = 0.02  # pad 2% to not cut off peripheral nodes' circles
 
-    # configure axis appearance, save/show figure as specified, and return
-    ax = _config_ax(ax, G.graph["crs"], bbox, padding)
-    fig, ax = _save_and_show(fig, ax, save, show, close, filepath, dpi)
-    utils.log("Finished plotting the graph")
+    # configure axes appearance, save/show figure as specified, and return
+    ax = _config_ax(ax, G.graph["crs"], bbox, padding)  # type: ignore[arg-type]
+    fig, ax = _save_and_show(
+        fig=fig,
+        ax=ax,
+        show=show,
+        close=close,
+        save=save,
+        filepath=filepath,
+        dpi=dpi,
+    )
+    msg = "Finished plotting the graph"
+    utils.log(msg, level=lg.INFO)
     return fig, ax
 
 
 def plot_graph_route(
-    G,
-    route,
-    route_color="r",
-    route_linewidth=4,
-    route_alpha=0.5,
-    orig_dest_size=100,
-    ax=None,
-    **pg_kwargs,
-):
-    """
-    Visualize a route along a graph.
+    G: nx.MultiDiGraph,
+    route: list[int],
+    *,
+    route_color: str = "r",
+    route_linewidth: float = 4,
+    route_alpha: float = 0.5,
+    orig_dest_size: float = 100,
+    ax: Axes | None = None,
+    **pg_kwargs: Any,  # noqa: ANN401
+) -> tuple[Figure, Axes]:
+    """
+    Visualize a path along a graph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    route : list
-        route as a list of node IDs
-    route_color : string
-        color of the route
-    route_linewidth : int
-        width of the route line
-    route_alpha : float
-        opacity of the route line
-    orig_dest_size : int
-        size of the origin and destination nodes
-    ax : matplotlib axis
-        if not None, plot route on this preexisting axis instead of creating a
-        new fig, ax and drawing the underlying graph
+    G
+        Input graph.
+    route
+        A path of node IDs.
+    route_color
+        The color of the route.
+    route_linewidth
+        Width of the route's line.
+    route_alpha
+        Opacity of the route's line.
+    orig_dest_size
+        Size of the origin and destination nodes.
+    ax
+        If not None, plot on this pre-existing axes instance.
     pg_kwargs
-        keyword arguments to pass to plot_graph
+        Keyword arguments to pass to `plot_graph`.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     _verify_mpl()
     if ax is None:
         # plot the graph but not the route, and override any user show/close
         # args for now: we'll do that later
         overrides = {"show", "save", "close"}
         kwargs = {k: v for k, v in pg_kwargs.items() if k not in overrides}
         fig, ax = plot_graph(G, show=False, save=False, close=False, **kwargs)
     else:
-        fig = ax.figure
+        fig = ax.figure  # type: ignore[assignment]
 
     # scatterplot origin and destination points (first/last nodes in route)
-    x = (G.nodes[route[0]]["x"], G.nodes[route[-1]]["x"])
-    y = (G.nodes[route[0]]["y"], G.nodes[route[-1]]["y"])
-    ax.scatter(x, y, s=orig_dest_size, c=route_color, alpha=route_alpha, edgecolor="none")
+    od_x = (G.nodes[route[0]]["x"], G.nodes[route[-1]]["x"])
+    od_y = (G.nodes[route[0]]["y"], G.nodes[route[-1]]["y"])
+    ax.scatter(od_x, od_y, s=orig_dest_size, c=route_color, alpha=route_alpha, edgecolor="none")
 
     # assemble the route edge geometries' x and y coords then plot the line
     x = []
     y = []
     for u, v in zip(route[:-1], route[1:]):
         # if there are parallel edges, select the shortest in length
         data = min(G.get_edge_data(u, v).values(), key=lambda d: d["length"])
@@ -340,60 +361,70 @@
         else:
             # otherwise, the edge is a straight line from node to node
             x.extend((G.nodes[u]["x"], G.nodes[v]["x"]))
             y.extend((G.nodes[u]["y"], G.nodes[v]["y"]))
     ax.plot(x, y, c=route_color, lw=route_linewidth, alpha=route_alpha)
 
     # save and show the figure as specified, passing relevant kwargs
-    sas_kwargs = {"save", "show", "close", "filepath", "file_format", "dpi"}
+    sas_kwargs = {"show", "close", "save", "filepath", "dpi"}
     kwargs = {k: v for k, v in pg_kwargs.items() if k in sas_kwargs}
-    fig, ax = _save_and_show(fig, ax, **kwargs)
+    fig, ax = _save_and_show(fig=fig, ax=ax, **kwargs)
     return fig, ax
 
 
-def plot_graph_routes(G, routes, route_colors="r", route_linewidths=4, **pgr_kwargs):
+def plot_graph_routes(
+    G: nx.MultiDiGraph,
+    routes: Iterable[list[int]],
+    *,
+    route_colors: str | Iterable[str] = "r",
+    route_linewidths: float | Iterable[float] = 4,
+    **pgr_kwargs: Any,  # noqa: ANN401
+) -> tuple[Figure, Axes]:
     """
-    Visualize several routes along a graph.
+    Visualize multiple paths along a graph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    routes : list
-        routes as a list of lists of node IDs
-    route_colors : string or list
-        if string, 1 color for all routes. if list, the colors for each route.
-    route_linewidths : int or list
-        if int, 1 linewidth for all routes. if list, the linewidth for each route.
+    G
+        Input graph.
+    routes
+        Paths of node IDs.
+    route_colors
+        If string, the one color for all routes. Otherwise, the color for each
+        route.
+    route_linewidths
+        If float, the one linewidth for all routes. Otherwise, the linewidth
+        for each route.
     pgr_kwargs
-        keyword arguments to pass to plot_graph_route
+        Keyword arguments to pass to `plot_graph_route`.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
-    _verify_mpl()
+    # make iterables lists (so we're guaranteed to be able to get their sizes)
+    routes = list(routes)
+    route_colors = (
+        [route_colors] * len(routes) if isinstance(route_colors, str) else list(route_colors)
+    )
+    route_linewidths = (
+        [route_linewidths] * len(routes)
+        if not isinstance(route_linewidths, Iterable)
+        else list(route_linewidths)
+    )
 
     # check for valid arguments
     if not all(isinstance(r, list) for r in routes):  # pragma: no cover
-        msg = "routes must be a list of route lists"
-        raise ValueError(msg)
-    if len(routes) <= 1:  # pragma: no cover
-        msg = "You must pass more than 1 route"
+        msg = "`routes` must be an iterable of route lists."
+        raise TypeError(msg)
+    if len(routes) == 0:  # pragma: no cover
+        msg = "You must pass at least 1 route."
         raise ValueError(msg)
-    if isinstance(route_colors, str):
-        route_colors = [route_colors] * len(routes)
-    if len(routes) != len(route_colors):  # pragma: no cover
-        msg = "route_colors list must have same length as routes"
-        raise ValueError(msg)
-    if isinstance(route_linewidths, int):
-        route_linewidths = [route_linewidths] * len(routes)
-    if len(routes) != len(route_linewidths):  # pragma: no cover
-        msg = "route_linewidths list must have same length as routes"
+    if not (len(routes) == len(route_colors) == len(route_linewidths)):  # pragma: no cover
+        msg = "`route_colors` and `route_linewidths` must have same lengths as `routes`."
         raise ValueError(msg)
 
     # plot the graph and the first route
     overrides = {"route", "route_color", "route_linewidth", "show", "save", "close"}
     kwargs = {k: v for k, v in pgr_kwargs.items() if k not in overrides}
     fig, ax = plot_graph_route(
         G,
@@ -420,390 +451,328 @@
             save=False,
             close=False,
             ax=ax,
             **kwargs,
         )
 
     # save and show the figure as specified, passing relevant kwargs
-    sas_kwargs = {"save", "show", "close", "filepath", "file_format", "dpi"}
+    sas_kwargs = {"show", "close", "save", "filepath", "dpi"}
     kwargs = {k: v for k, v in pgr_kwargs.items() if k in sas_kwargs}
-    fig, ax = _save_and_show(fig, ax, **kwargs)
+    fig, ax = _save_and_show(fig=fig, ax=ax, **kwargs)
     return fig, ax
 
 
 def plot_figure_ground(
-    G=None,
-    address=None,
-    point=None,
-    dist=805,
-    network_type="drive_service",
-    street_widths=None,
-    default_width=4,
-    color="w",
-    edge_color=None,
-    smooth_joints=None,
-    **pg_kwargs,
-):
+    G: nx.MultiDiGraph,
+    *,
+    dist: float = 805,
+    street_widths: dict[str, float] | None = None,
+    default_width: float = 4,
+    color: str = "w",
+    **pg_kwargs: Any,  # noqa: ANN401
+) -> tuple[Figure, Axes]:
     """
     Plot a figure-ground diagram of a street network.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph, must be unprojected
-    address : string
-        deprecated, do not use
-    point : tuple
-        deprecated, do not use
-    dist : numeric
-        how many meters to extend north, south, east, west from center point
-    network_type : string
-        deprecated, do not use
-    street_widths : dict
-        dict keys are street types and values are widths to plot in pixels
-    default_width : numeric
-        fallback width in pixels for any street type not in street_widths
-    color : string
-        color of the streets
-    edge_color : string
-        deprecated, do not use
-    smooth_joints : bool
-        deprecated, do not use
+    G
+        An unprojected graph.
+    dist
+        How many meters to extend plot's bounding box north, south, east, and
+        west from the graph's center point. Default corresponds to a square
+        mile bounding box.
+    street_widths
+        Dict keys are street types (ie, OSM "highway" tags) and values are the
+        widths to plot them, in pixels.
+    default_width
+        Fallback width, in pixels, for any street type not in `street_widths`.
+    color
+        The color of the streets.
     pg_kwargs
-        keyword arguments to pass to plot_graph
+        Keyword arguments to pass to `plot_graph`.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     _verify_mpl()
 
-    if edge_color is None:
-        edge_color = color
-    else:
-        msg = (
-            "The `edge_color` parameter is deprecated and will be removed in the "
-            "v2.0.0 release. Use `color` instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    if smooth_joints is None:
-        smooth_joints = True
-    else:
-        msg = (
-            "The `smooth_joints` parameter is deprecated and will be removed in the "
-            "v2.0.0 release. In the future this function will behave as though True. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-
-    # if user did not pass in custom street widths, create a dict of defaults
+    # if user did not pass in custom street widths, define default values
     if street_widths is None:
         street_widths = {
             "footway": 1.5,
             "steps": 1.5,
             "pedestrian": 1.5,
             "service": 1.5,
             "path": 1.5,
             "track": 1.5,
             "motorway": 6,
         }
 
-    multiplier = 1.2
-    dep_msg = (
-        "The `address`, `point`, and `network_type` parameters are deprecated "
-        "and will be removed in the v2.0.0 release. Pass `G` instead. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-    )
-
-    # if G was passed in, plot it centered on its node centroid
-    if G is not None:
-        gdf_nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=True)
-        lonlat_point = gdf_nodes.unary_union.centroid.coords[0]
-        point = tuple(reversed(lonlat_point))
-
-    # otherwise get network by address or point (whichever was passed) using a
-    # dist multiplier to ensure we get more than enough network. simplify in
-    # non-strict mode to not combine multiple street types into single edge
-    elif address is not None:
-        warn(dep_msg, FutureWarning, stacklevel=2)
-        G, point = graph.graph_from_address(
-            address,
-            dist=dist * multiplier,
-            dist_type="bbox",
-            network_type=network_type,
-            simplify=False,
-            truncate_by_edge=True,
-            return_coords=True,
-        )
-        G = simplification.simplify_graph(G, edge_attrs_differ=["osmid"])
-    elif point is not None:
-        warn(dep_msg, FutureWarning, stacklevel=2)
-        G = graph.graph_from_point(
-            point,
-            dist=dist * multiplier,
-            dist_type="bbox",
-            network_type=network_type,
-            simplify=False,
-            truncate_by_edge=True,
-        )
-        G = simplification.simplify_graph(G, edge_attrs_differ=["osmid"])
-    else:  # pragma: no cover
-        msg = "You must pass an address or lat-lon point or graph."
-        raise ValueError(msg)
-
     # we need an undirected graph to find every edge incident on a node
     Gu = convert.to_undirected(G)
 
     # for each edge, get a linewidth according to street type
     edge_linewidths = []
     for _, _, d in Gu.edges(keys=False, data=True):
         street_type = d["highway"][0] if isinstance(d["highway"], list) else d["highway"]
         if street_type in street_widths:
             edge_linewidths.append(street_widths[street_type])
         else:
             edge_linewidths.append(default_width)
 
-    if smooth_joints:
-        # for each node, get a nodesize according to the narrowest incident edge
-        node_widths = {}
-        for node in Gu.nodes:
-            # first, identify all the highway types of this node's incident edges
-            ie_data = [Gu.get_edge_data(node, nbr) for nbr in Gu.neighbors(node)]
-            edge_types = [d[min(d)]["highway"] for d in ie_data]
-            if not edge_types:
-                # if node has no incident edges, make size zero
-                node_widths[node] = 0
-            else:
-                # flatten the list of edge types
-                et_flat = []
-                for et in edge_types:
-                    if isinstance(et, list):
-                        et_flat.extend(et)
-                    else:
-                        et_flat.append(et)
-
-                # lookup corresponding width for each edge type in flat list
-                edge_widths = [street_widths.get(et, default_width) for et in et_flat]
-
-                # node diameter should equal largest edge width to make joints
-                # perfectly smooth. alternatively use min(?) to prevent
-                # anything larger from extending past smallest street's line.
-                # circle marker sizes are in area, so use diameter squared.
-                circle_diameter = max(edge_widths)
-                circle_area = circle_diameter**2
-                node_widths[node] = circle_area
+    # smooth the street segment joints
+    # for each node, get a node size according to the narrowest incident edge
+    node_widths: dict[int, float] = {}
+    for node in Gu.nodes:
+        # first, identify all the highway types of this node's incident edges
+        ie_data = (Gu.get_edge_data(node, nbr) for nbr in Gu.neighbors(node))
+        edge_types = [d[min(d)]["highway"] for d in ie_data]
+        if len(edge_types) == 0:
+            # if node has no incident edges, make size zero
+            node_widths[node] = 0
+        else:
+            # flatten the list of edge types
+            et_flat = []
+            for et in edge_types:
+                if isinstance(et, list):
+                    et_flat.extend(et)
+                else:
+                    et_flat.append(et)
+
+            # look up corresponding width for each edge type in flat list
+            edge_widths = [street_widths.get(et, default_width) for et in et_flat]
+
+            # node diameter should = largest edge width to make joints smooth
+            # mpl circle marker sizes are in area, so use diameter squared
+            circle_diameter = max(edge_widths)
+            circle_area = circle_diameter**2
+            node_widths[node] = circle_area
 
-        # assign the node size to each node in the graph
-        node_sizes = [node_widths[node] for node in Gu.nodes]
-    else:
-        node_sizes = 0
+    # assign the node size to each node in the graph
+    node_sizes: list[float] | float = [node_widths[node] for node in Gu.nodes]
 
     # define the view extents of the plotting figure
-    bbox = utils_geo.bbox_from_point(point, dist, project_utm=False)
+    node_geoms = convert.graph_to_gdfs(Gu, edges=False, node_geometry=True).unary_union
+    lonlat_point = node_geoms.centroid.coords[0]
+    latlon_point = tuple(reversed(lonlat_point))
+    bbox = utils_geo.bbox_from_point(latlon_point, dist=dist, project_utm=False)
 
     # plot the figure
     overrides = {"bbox", "node_size", "node_color", "edge_linewidth"}
     kwargs = {k: v for k, v in pg_kwargs.items() if k not in overrides}
     fig, ax = plot_graph(
         G=Gu,
         bbox=bbox,
         node_size=node_sizes,
-        node_color=edge_color,
-        edge_color=edge_color,
+        node_color=color,
+        edge_color=color,
         edge_linewidth=edge_linewidths,
         **kwargs,
     )
     return fig, ax
 
 
-def plot_footprints(
-    gdf,
-    ax=None,
-    figsize=(8, 8),
-    color="orange",
-    edge_color="none",
-    edge_linewidth=0,
-    alpha=None,
-    bgcolor="#111111",
-    bbox=None,
-    save=False,
-    show=True,
-    close=False,
-    filepath=None,
-    dpi=600,
-):
+def plot_footprints(  # noqa: PLR0913
+    gdf: gpd.GeoDataFrame,
+    *,
+    ax: Axes | None = None,
+    figsize: tuple[float, float] = (8, 8),
+    color: str = "orange",
+    edge_color: str = "none",
+    edge_linewidth: float = 0,
+    alpha: float | None = None,
+    bgcolor: str = "#111111",
+    bbox: tuple[float, float, float, float] | None = None,
+    show: bool = True,
+    close: bool = False,
+    save: bool = False,
+    filepath: str | Path | None = None,
+    dpi: int = 600,
+) -> tuple[Figure, Axes]:
     """
     Visualize a GeoDataFrame of geospatial features' footprints.
 
     Parameters
     ----------
-    gdf : geopandas.GeoDataFrame
-        GeoDataFrame of footprints (shapely Polygons and MultiPolygons)
-    ax : axis
-        if not None, plot on this preexisting axis
-    figsize : tuple
-        if ax is None, create new figure with size (width, height)
-    color : string
-        color of the footprints
-    edge_color : string
-        color of the edge of the footprints
-    edge_linewidth : float
-        width of the edge of the footprints
-    alpha : float
-        opacity of the footprints
-    bgcolor : string
-        background color of the plot
-    bbox : tuple
-        bounding box as (north, south, east, west). if None, will calculate
-        from the spatial extents of the geometries in gdf
-    save : bool
-        if True, save the figure to disk at filepath
-    show : bool
-        if True, call pyplot.show() to show the figure
-    close : bool
-        if True, call pyplot.close() to close the figure
-    filepath : string
-        if save is True, the path to the file. file format determined from
-        extension. if None, use settings.imgs_folder/image.png
-    dpi : int
-        if save is True, the resolution of saved file
+    gdf
+        GeoDataFrame of footprints (i.e., Polygons and/or MultiPolygons).
+    ax
+        If not None, plot on this pre-existing axes instance.
+    figsize
+        If `ax` is None, create new figure with size `(width, height)`.
+    color
+        Color of the footprints.
+    edge_color
+        Color of the footprints' edges.
+    edge_linewidth
+        Width of the footprints' edges.
+    alpha
+        Opacity of the footprints' edges.
+    bgcolor
+        Background color of the figure.
+    bbox
+        Bounding box as `(north, south, east, west)`. If None, calculate it
+        from the spatial extents of the geometries in `gdf`.
+    show
+        If True, call `pyplot.show()` to show the figure.
+    close
+        If True, call `pyplot.close()` to close the figure.
+    save
+        If True, save the figure to disk at `filepath`.
+    filepath
+        The path to the file if `save` is True. File format is determined from
+        the extension. If None, save at `settings.imgs_folder/image.png`.
+    dpi
+        The resolution of saved file if `save` is True.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     _verify_mpl()
-
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
-        ax.set_facecolor(bgcolor)
-    else:
-        fig = ax.figure
+    fig, ax = _get_fig_ax(ax=ax, figsize=figsize, bgcolor=bgcolor, polar=False)
 
     # retain only Polygons and MultiPolygons, then plot
     gdf = gdf[gdf["geometry"].type.isin({"Polygon", "MultiPolygon"})]
     ax = gdf.plot(
-        ax=ax, facecolor=color, edgecolor=edge_color, linewidth=edge_linewidth, alpha=alpha
+        ax=ax,
+        facecolor=color,
+        edgecolor=edge_color,
+        linewidth=edge_linewidth,
+        alpha=alpha,
     )
 
     # determine figure extents
     if bbox is None:
         west, south, east, north = gdf.total_bounds
     else:
         north, south, east, west = bbox
 
-    # configure axis appearance, save/show figure as specified, and return
-    ax = _config_ax(ax, gdf.crs, (north, south, east, west), 0)
-    fig, ax = _save_and_show(fig, ax, save, show, close, filepath, dpi)
+    # configure axes appearance, save/show figure as specified, and return
+    ax = _config_ax(ax, gdf.crs, (north, south, east, west), 0)  # type: ignore[arg-type]
+    fig, ax = _save_and_show(
+        fig=fig,
+        ax=ax,
+        show=show,
+        close=close,
+        save=save,
+        filepath=filepath,
+        dpi=dpi,
+    )
     return fig, ax
 
 
-def plot_orientation(
-    Gu,
-    num_bins=36,
-    min_length=0,
-    weight=None,
-    ax=None,
-    figsize=(5, 5),
-    area=True,
-    color="#003366",
-    edgecolor="k",
-    linewidth=0.5,
-    alpha=0.7,
-    title=None,
-    title_y=1.05,
-    title_font=None,
-    xtick_font=None,
-):
-    """
-    Plot a polar histogram of a spatial network's bidirectional edge bearings.
-
-    Ignores self-loop edges as their bearings are undefined.
+def plot_orientation(  # noqa: PLR0913
+    G: nx.MultiGraph | nx.MultiDiGraph,
+    *,
+    num_bins: int = 36,
+    min_length: float = 0,
+    weight: str | None = None,
+    ax: PolarAxes | None = None,
+    figsize: tuple[float, float] = (5, 5),
+    area: bool = True,
+    color: str = "#003366",
+    edgecolor: str = "k",
+    linewidth: float = 0.5,
+    alpha: float = 0.7,
+    title: str | None = None,
+    title_y: float = 1.05,
+    title_font: dict[str, Any] | None = None,
+    xtick_font: dict[str, Any] | None = None,
+) -> tuple[Figure, PolarAxes]:
+    """
+    Plot a polar histogram of a spatial network's edge bearings.
+
+    Ignores self-loop edges as their bearings are undefined. If `G` is a
+    MultiGraph, all edge bearings will be bidirectional (ie, two reciprocal
+    bearings per undirected edge). If `G` is a MultiDiGraph, all edge bearings
+    will be directional (ie, one bearing per directed edge). See also the
+    `bearings` module.
 
     For more info see: Boeing, G. 2019. "Urban Spatial Order: Street Network
     Orientation, Configuration, and Entropy." Applied Network Science, 4 (1),
     67. https://doi.org/10.1007/s41109-019-0189-1
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected, unprojected graph with `bearing` attributes on each edge
-    num_bins : int
-        number of bins; for example, if `num_bins=36` is provided, then each
-        bin will represent 10 degrees around the compass
-    min_length : float
-        ignore edges with `length` attributes less than `min_length`
-    weight : string
-        if not None, weight edges' bearings by this (non-null) edge attribute
-    ax : matplotlib.axes.PolarAxesSubplot
-        if not None, plot on this preexisting axis; must have projection=polar
-    figsize : tuple
-        if ax is None, create new figure with size (width, height)
-    area : bool
-        if True, set bar length so area is proportional to frequency,
-        otherwise set bar length so height is proportional to frequency
-    color : string
-        color of histogram bars
-    edgecolor : string
-        color of histogram bar edges
-    linewidth : float
-        width of histogram bar edges
-    alpha : float
-        opacity of histogram bars
-    title : string
-        title for plot
-    title_y : float
-        y position to place title
-    title_font : dict
-        the title's fontdict to pass to matplotlib
-    xtick_font : dict
-        the xtick labels' fontdict to pass to matplotlib
+    G
+        Unprojected graph with `bearing` attributes on each edge.
+    num_bins
+        Number of bins. For example, if `num_bins=36` is provided, then each
+        bin will represent 10 degrees around the compass.
+    min_length
+        Ignore edges with "length" attribute values less than `min_length`.
+    weight
+        If not None, weight the edges' bearings by this (non-null) edge
+        attribute.
+    ax
+        If not None, plot on this pre-existing axes instance (must have
+        projection=polar).
+    figsize
+        If `ax` is None, create new figure with size `(width, height)`.
+    area
+        If True, set bar length so area is proportional to frequency.
+        Otherwise, set bar length so height is proportional to frequency.
+    color
+        Color of the histogram bars.
+    edgecolor
+        Color of the histogram bar edges.
+    linewidth
+        Width of the histogram bar edges.
+    alpha
+        Opacity of the histogram bars.
+    title
+        The figure's title.
+    title_y
+        The y position to place `title`.
+    title_font
+        The title's `fontdict` to pass to matplotlib.
+    xtick_font
+        The xtick labels' `fontdict` to pass to matplotlib.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     _verify_mpl()
 
     if title_font is None:
         title_font = {"family": "DejaVu Sans", "size": 24, "weight": "bold"}
     if xtick_font is None:
         xtick_font = {
             "family": "DejaVu Sans",
             "size": 10,
             "weight": "bold",
             "alpha": 1.0,
             "zorder": 3,
         }
 
-    # get the bearings' distribution's bin counts and edges
-    bin_counts, bin_edges = bearing._bearings_distribution(Gu, num_bins, min_length, weight)
+    # get the bearing distribution's bin counts and center values in degrees
+    bin_counts, bin_centers = bearing._bearings_distribution(
+        G,
+        num_bins,
+        min_length=min_length,
+        weight=weight,
+    )
 
-    # positions: where to center each bar. ignore the last bin edge, because
-    # it's the same as the first (i.e., 0 degrees = 360 degrees)
-    positions = np.radians(bin_edges[:-1])
+    # positions: where to center each bar
+    positions = np.radians(bin_centers)
 
     # width: make bars fill the circumference without gaps or overlaps
     width = 2 * np.pi / num_bins
 
     # radius: how long to make each bar. set bar length so either the bar area
     # (ie, via sqrt) or the bar height is proportional to the bin's frequency
     bin_frequency = bin_counts / bin_counts.sum()
     radius = np.sqrt(bin_frequency) if area else bin_frequency
 
-    # create ax (if necessary) then set N at top and go clockwise
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize, subplot_kw={"projection": "polar"})
-    else:
-        fig = ax.figure
+    # create PolarAxes (if not passed-in) then set N at top and go clockwise
+    fig, ax = _get_fig_ax(ax=ax, figsize=figsize, bgcolor=None, polar=True)
     ax.set_theta_zero_location("N")
     ax.set_theta_direction("clockwise")
     ax.set_ylim(top=radius.max())
 
     # configure the y-ticks and remove their labels
     ax.set_yticks(np.linspace(0, radius.max(), 5))
     ax.set_yticklabels(labels="")
@@ -830,42 +799,52 @@
 
     if title:
         ax.set_title(title, y=title_y, fontdict=title_font)
     fig.tight_layout()
     return fig, ax
 
 
-def _get_colors_by_value(vals, num_bins, cmap, start, stop, na_color, equal_size):
+def _get_colors_by_value(
+    vals: pd.Series,  # type: ignore[type-arg]
+    num_bins: int | None,
+    cmap: str,
+    start: float,
+    stop: float,
+    na_color: str,
+    equal_size: bool,  # noqa: FBT001
+) -> pd.Series:  # type: ignore[type-arg]
     """
-    Map colors to the values in a series.
+    Map colors to the values in a Series of node/edge attribute values.
 
     Parameters
     ----------
-    vals : pandas.Series
-        series labels are node/edge IDs and values are attribute values
-    num_bins : int
-        if None, linearly map a color to each value. otherwise, assign values
+    vals
+        Series labels are node/edge IDs and values are attribute values.
+    num_bins
+        If None, linearly map a color to each value. Otherwise, assign values
         to this many bins then assign a color to each bin.
-    cmap : string
-        name of a matplotlib colormap
-    start : float
-        where to start in the colorspace
-    stop : float
-        where to end in the colorspace
-    na_color : string
-        what color to assign to missing values
-    equal_size : bool
-        ignored if num_bins is None. if True, bin into equal-sized quantiles
-        (requires unique bin edges). if False, bin into equal-spaced bins.
+    cmap
+        Name of the matplotlib colormap from which to choose the colors.
+    start
+        Where to start in the colorspace (from 0 to 1).
+    stop
+        Where to end in the colorspace (from 0 to 1).
+    na_color
+        The color to assign to nodes with missing `attr` values.
+    equal_size
+        Ignored if `num_bins` is None. If True, bin into equal-sized quantiles
+        (requires unique bin edges). If False, bin into equal-spaced bins.
 
     Returns
     -------
-    color_series : pandas.Series
-        series labels are node/edge IDs and values are colors
+    color_series
+        Labels are node/edge IDs, values are colors as hex strings.
     """
+    _verify_mpl()
+
     if len(vals) == 0:
         msg = "There are no attribute values."
         raise ValueError(msg)
 
     if num_bins is None:
         # calculate min/max values based on start/stop and data range
         vals_min = vals.dropna().min()
@@ -873,129 +852,138 @@
         full_range = (vals_max - vals_min) / (stop - start)
         full_min = vals_min - full_range * start
         full_max = full_min + full_range
 
         # linearly map a color to each attribute value
         normalizer = colors.Normalize(full_min, full_max)
         scalar_mapper = cm.ScalarMappable(normalizer, colormaps[cmap])
-        color_series = vals.map(scalar_mapper.to_rgba)
+        color_series = vals.map(scalar_mapper.to_rgba).map(colors.to_hex)
         color_series.loc[pd.isna(vals)] = na_color
 
     else:
         # otherwise, bin values then assign colors to bins
-        cut_func = pd.qcut if equal_size else pd.cut
-        bins = cut_func(vals, num_bins, labels=range(num_bins))
-        bin_colors = get_colors(num_bins, cmap, start, stop)
+        if equal_size:
+            bins = pd.qcut(vals, num_bins, labels=range(num_bins))
+        else:
+            bins = pd.cut(vals, num_bins, labels=range(num_bins))
+        bin_colors = get_colors(num_bins, cmap=cmap, start=start, stop=stop)
         color_list = [bin_colors[b] if pd.notna(b) else na_color for b in bins]
         color_series = pd.Series(color_list, index=bins.index)
 
     return color_series
 
 
-def _save_and_show(fig, ax, save=False, show=True, close=True, filepath=None, dpi=300):
+def _save_and_show(
+    fig: Figure,
+    ax: Axes,
+    *,
+    show: bool = True,
+    close: bool = True,
+    save: bool = False,
+    filepath: str | Path | None = None,
+    dpi: int = 300,
+) -> tuple[Figure, Axes]:
     """
-    Save a figure to disk and/or show it, as specified by args.
+    Save a figure to disk and/or show it, as specified by arguments.
 
     Parameters
     ----------
-    fig : figure
-        matplotlib figure
-    ax : axis
-        matplotlib axis
-    save : bool
-        if True, save the figure to disk at filepath
-    show : bool
-        if True, call pyplot.show() to show the figure
-    close : bool
-        if True, call pyplot.close() to close the figure
-    filepath : string
-        if save is True, the path to the file. file format determined from
-        extension. if None, use settings.imgs_folder/image.png
-    dpi : int
-        if save is True, the resolution of saved file
+    fig
+        The figure.
+    ax
+        The axes instance.
+    show
+        If True, call `pyplot.show()` to show the figure.
+    close
+        If True, call `pyplot.close()` to close the figure.
+    save
+        If True, save the figure to disk at `filepath`.
+    filepath
+        The path to the file if `save` is True. File format is determined from
+        the extension. If None, save at `settings.imgs_folder/image.png`.
+    dpi
+        The resolution of saved file if `save` is True.
 
     Returns
     -------
-    fig, ax : tuple
-        matplotlib figure, axis
+    fig, ax
     """
     fig.canvas.draw()
     fig.canvas.flush_events()
 
     if save:
         # default filepath, if none provided
-        filepath = Path(settings.imgs_folder) / "image.png" if filepath is None else Path(filepath)
+        fp = Path(settings.imgs_folder) / "image.png" if filepath is None else Path(filepath)
 
         # if save folder does not already exist, create it
-        filepath.parent.mkdir(parents=True, exist_ok=True)
+        fp.parent.mkdir(parents=True, exist_ok=True)
 
         # get the file extension and figure facecolor
-        ext = filepath.suffix.strip(".")
+        ext = fp.suffix.strip(".")
         fc = fig.get_facecolor()
 
         if ext == "svg":
             # if the file format is svg, prep the fig/ax for saving
             ax.axis("off")
-            ax.set_position([0, 0, 1, 1])
-            ax.patch.set_alpha(0.0)
-            fig.patch.set_alpha(0.0)
-            fig.savefig(filepath, bbox_inches=0, format=ext, facecolor=fc, transparent=True)
+            ax.set_position((0, 0, 1, 1))
+            ax.patch.set_alpha(0)
+            fig.patch.set_alpha(0)
+            fig.savefig(fp, bbox_inches=0, format=ext, facecolor=fc, transparent=True)
         else:
-            # constrain saved figure's extent to interior of the axis
+            # constrain saved figure's extent to interior of the axes
             extent = ax.bbox.transformed(fig.dpi_scale_trans.inverted())
 
             # temporarily turn figure frame on to save with facecolor
             fig.set_frameon(True)
-            fig.savefig(
-                filepath, dpi=dpi, bbox_inches=extent, format=ext, facecolor=fc, transparent=True
-            )
+            fig.savefig(fp, dpi=dpi, bbox_inches=extent, format=ext, facecolor=fc, transparent=True)
             fig.set_frameon(False)  # and turn it back off again
-        utils.log(f"Saved figure to disk at {filepath}")
+
+        msg = f"Saved figure to disk at {fp!r}"
+        utils.log(msg, level=lg.INFO)
 
     if show:
         plt.show()
 
     if close:
         plt.close()
 
     return fig, ax
 
 
-def _config_ax(ax, crs, bbox, padding):
+def _config_ax(ax: Axes, crs: Any, bbox: tuple[float, float, float, float], padding: float) -> Axes:  # noqa: ANN401
     """
-    Configure axis for display.
+    Configure a matplotlib axes instance for display.
 
     Parameters
     ----------
-    ax : matplotlib axis
-        the axis containing the plot
-    crs : dict or string or pyproj.CRS
-        the CRS of the plotted geometries
-    bbox : tuple
-        bounding box as (north, south, east, west)
-    padding : float
-        relative padding to add around the plot's bbox
+    ax
+        The axes instance.
+    crs
+        The coordinate reference system of the plotted geometries.
+    bbox
+        Bounding box as `(north, south, east, west)`.
+    padding
+        Relative padding to add around `bbox`.
 
     Returns
     -------
-    ax : matplotlib axis
-        the configured/styled axis
+    ax
     """
-    # set the axis view limits to bbox + relative padding
+    # set the axes view limits to bbox + relative padding
     north, south, east, west = bbox
     padding_ns = (north - south) * padding
     padding_ew = (east - west) * padding
     ax.set_ylim((south - padding_ns, north + padding_ns))
     ax.set_xlim((west - padding_ew, east + padding_ew))
 
     # set margins to zero, point ticks inward, turn off ax border and x/y axis
     # so there is no space around the plot
     ax.margins(0)
     ax.tick_params(which="both", direction="in")
-    _ = [s.set_visible(False) for s in ax.spines.values()]
+    _ = [s.set_visible(False) for s in ax.spines.values()]  # type: ignore[func-returns-value]
     ax.get_xaxis().set_visible(False)
     ax.get_yaxis().set_visible(False)
 
     # set aspect ratio
     if projection.is_projected(crs):
         # if projected, make equal aspect ratio
         ax.set_aspect("equal")
@@ -1003,18 +991,76 @@
         # if not projected, conform aspect ratio to not stretch plot
         cos_lat = np.cos((south + north) / 2 / 180 * np.pi)
         ax.set_aspect(1 / cos_lat)
 
     return ax
 
 
-def _verify_mpl():
+# if polar = False, return Axes
+@overload
+def _get_fig_ax(
+    ax: Axes | None,
+    figsize: tuple[float, float],
+    bgcolor: str | None,
+    polar: Literal[False],
+) -> tuple[Figure, Axes]: ...
+
+
+# if polar = True, return PolarAxes
+@overload
+def _get_fig_ax(
+    ax: Axes | None,
+    figsize: tuple[float, float],
+    bgcolor: str | None,
+    polar: Literal[True],
+) -> tuple[Figure, PolarAxes]: ...
+
+
+def _get_fig_ax(
+    ax: Axes | None,
+    figsize: tuple[float, float],
+    bgcolor: str | None,
+    polar: bool,  # noqa: FBT001
+) -> tuple[Figure, Axes | PolarAxes]:
+    """
+    Generate a matplotlib Figure and (Polar)Axes or return existing ones.
+
+    Parameters
+    ----------
+    ax
+        If not None, plot on this pre-existing axes instance.
+    figsize
+        If `ax` is None, create new figure with size `(width, height)`.
+    bgcolor
+        Background color of figure.
+    polar
+        If True, generate a `PolarAxes` instead of an `Axes` instance.
+
+    Returns
+    -------
+    fig, ax
+    """
+    if ax is None:
+        if polar:
+            # make PolarAxes
+            fig, ax = plt.subplots(figsize=figsize, subplot_kw={"projection": "polar"})
+        else:
+            # make regular Axes
+            fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
+            ax.set_facecolor(bgcolor)
+    else:
+        fig = ax.figure  # type: ignore[assignment]
+
+    return fig, ax
+
+
+def _verify_mpl() -> None:
     """
-    Verify that matplotlib is installed and successfully imported.
+    Verify that matplotlib is installed and imported.
 
     Returns
     -------
     None
     """
-    if cm is None or colors is None or plt is None or colormaps is None:  # pragma: no cover
-        msg = "matplotlib must be installed as an optional dependency for visualization"
+    if not mpl_available:  # pragma: no cover
+        msg = "matplotlib must be installed as an optional dependency for visualization."
         raise ImportError(msg)
```

### Comparing `osmnx-1.9.3/osmnx/projection.py` & `osmnx-2.0.0b0/osmnx/projection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,190 @@
 """Project a graph, GeoDataFrame, or geometry to a different CRS."""
 
+from __future__ import annotations
+
+import logging as lg
+from typing import TYPE_CHECKING
+from typing import Any
+
 import geopandas as gpd
 
 from . import convert
 from . import settings
 from . import utils
 
+if TYPE_CHECKING:
+    import networkx as nx
+    from shapely import Geometry
+
 
-def is_projected(crs):
+def is_projected(crs: Any) -> bool:  # noqa: ANN401
     """
     Determine if a coordinate reference system is projected or not.
 
     Parameters
     ----------
-    crs : string or pyproj.CRS
-        the identifier of the coordinate reference system, which can be
-        anything accepted by `pyproj.CRS.from_user_input()` such as an
-        authority string or a WKT string
+    crs
+        The identifier of the coordinate reference system. This can be
+        anything accepted by `pyproj.CRS.from_user_input()`, such as an
+        authority string or a WKT string.
 
     Returns
     -------
-    projected : bool
-        True if crs is projected, otherwise False
+    projected
+        True if `crs` is projected, otherwise False
     """
-    return gpd.GeoSeries(crs=crs).crs.is_projected
+    return bool(gpd.GeoSeries(crs=crs).crs.is_projected)
 
 
-def project_geometry(geometry, crs=None, to_crs=None, to_latlong=False):
+def project_geometry(
+    geometry: Geometry,
+    *,
+    crs: Any | None = None,  # noqa: ANN401
+    to_crs: Any | None = None,  # noqa: ANN401
+    to_latlong: bool = False,
+) -> tuple[Geometry, Any]:
     """
     Project a Shapely geometry from its current CRS to another.
 
-    If `to_latlong` is `True`, this projects the GeoDataFrame to the CRS
-    defined by `settings.default_crs`, otherwise it projects it to the CRS
-    defined by `to_crs`. If `to_crs` is `None`, it projects it to the CRS of
-    an appropriate UTM zone given `geometry`'s bounds.
+    If `to_latlong` is True, this projects the geometry to the coordinate
+    reference system defined by `settings.default_crs`. Otherwise it projects
+    it to the CRS defined by `to_crs`. If `to_crs` is `None`, it projects it
+    to the CRS of an appropriate UTM zone given `geometry`'s bounds.
 
     Parameters
     ----------
-    geometry : shapely geometry
-        the geometry to be projected
-    crs : string or pyproj.CRS
-        the initial CRS of `geometry`. if None, it will be set to
-        `settings.default_crs`
-    to_crs : string or pyproj.CRS
-        if None, project to an appropriate UTM zone, otherwise project to
-        this CRS
-    to_latlong : bool
-        if True, project to `settings.default_crs` and ignore `to_crs`
+    geometry
+        The geometry to be projected.
+    crs
+        The initial CRS of `geometry`. If None, it will be set to
+        `settings.default_crs`.
+    to_crs
+        If None, project to an appropriate UTM zone. Otherwise project to this
+        CRS.
+    to_latlong
+        If True, project to `settings.default_crs` and ignore `to_crs`.
 
     Returns
     -------
-    geometry_proj, crs : tuple
-        the projected geometry and its new CRS
+    geometry_proj, crs
+        The projected geometry and its new CRS.
     """
     if crs is None:
         crs = settings.default_crs
 
     gdf = gpd.GeoDataFrame(geometry=[geometry], crs=crs)
     gdf_proj = project_gdf(gdf, to_crs=to_crs, to_latlong=to_latlong)
     geometry_proj = gdf_proj["geometry"].iloc[0]
     return geometry_proj, gdf_proj.crs
 
 
-def project_gdf(gdf, to_crs=None, to_latlong=False):
+def project_gdf(
+    gdf: gpd.GeoDataFrame,
+    *,
+    to_crs: Any | None = None,  # noqa: ANN401
+    to_latlong: bool = False,
+) -> gpd.GeoDataFrame:
     """
     Project a GeoDataFrame from its current CRS to another.
 
-    If `to_latlong` is `True`, this projects the GeoDataFrame to the CRS
-    defined by `settings.default_crs`, otherwise it projects it to the CRS
-    defined by `to_crs`. If `to_crs` is `None`, it projects it to the CRS of
-    an appropriate UTM zone given `gdf`'s bounds.
+    If `to_latlong` is True, this projects the GeoDataFrame to the coordinate
+    reference system defined by `settings.default_crs`. Otherwise it projects
+    it to the CRS defined by `to_crs`. If `to_crs` is `None`, it projects it
+    to the CRS of an appropriate UTM zone given `geometry`'s bounds.
 
     Parameters
     ----------
-    gdf : geopandas.GeoDataFrame
-        the GeoDataFrame to be projected
-    to_crs : string or pyproj.CRS
-        if None, project to an appropriate UTM zone, otherwise project to
-        this CRS
-    to_latlong : bool
-        if True, project to `settings.default_crs` and ignore `to_crs`
+    gdf
+        The GeoDataFrame to be projected.
+    to_crs
+        If None, project to an appropriate UTM zone. Otherwise project to
+        this CRS.
+    to_latlong
+        If True, project to `settings.default_crs` and ignore `to_crs`.
 
     Returns
     -------
-    gdf_proj : geopandas.GeoDataFrame
-        the projected GeoDataFrame
+    gdf_proj
+        The projected GeoDataFrame.
     """
-    if gdf.crs is None or len(gdf) < 1:  # pragma: no cover
-        msg = "GeoDataFrame must have a valid CRS and cannot be empty"
+    if gdf.crs is None or len(gdf) == 0:  # pragma: no cover
+        msg = "`gdf` must have a valid CRS and cannot be empty."
         raise ValueError(msg)
 
     # if to_latlong is True, project the gdf to the default_crs
     if to_latlong:
         to_crs = settings.default_crs
 
     # else if to_crs is None, project gdf to an appropriate UTM zone
     elif to_crs is None:
         to_crs = gdf.estimate_utm_crs()
 
     # project the gdf
     gdf_proj = gdf.to_crs(to_crs)
     crs_desc = f"{gdf_proj.crs.to_string()} / {gdf_proj.crs.name}"
-    utils.log(f"Projected GeoDataFrame to {crs_desc!r}")
+
+    msg = f"Projected GeoDataFrame to {crs_desc!r}"
+    utils.log(msg, level=lg.INFO)
     return gdf_proj
 
 
-def project_graph(G, to_crs=None, to_latlong=False):
+def project_graph(
+    G: nx.MultiDiGraph,
+    *,
+    to_crs: Any | None = None,  # noqa: ANN401
+    to_latlong: bool = False,
+) -> nx.MultiDiGraph:
     """
     Project a graph from its current CRS to another.
 
-    If `to_latlong` is `True`, this projects the GeoDataFrame to the CRS
-    defined by `settings.default_crs`, otherwise it projects it to the CRS
-    defined by `to_crs`. If `to_crs` is `None`, it projects it to the CRS of
-    an appropriate UTM zone given `G`'s bounds.
+    If `to_latlong` is True, this projects the graph to the coordinate
+    reference system defined by `settings.default_crs`. Otherwise it projects
+    it to the CRS defined by `to_crs`. If `to_crs` is `None`, it projects it
+    to the CRS of an appropriate UTM zone given `geometry`'s bounds.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        the graph to be projected
-    to_crs : string or pyproj.CRS
-        if None, project to an appropriate UTM zone, otherwise project to
-        this CRS
-    to_latlong : bool
-        if True, project to `settings.default_crs` and ignore `to_crs`
+    G
+        The graph to be projected.
+    to_crs
+        If None, project to an appropriate UTM zone. Otherwise project to
+        this CRS.
+    to_latlong
+        If True, project to `settings.default_crs` and ignore `to_crs`.
 
     Returns
     -------
-    G_proj : networkx.MultiDiGraph
-        the projected graph
+    G_proj
+        The projected graph.
     """
     if to_latlong:
         to_crs = settings.default_crs
 
     # STEP 1: PROJECT THE NODES
     gdf_nodes = convert.graph_to_gdfs(G, edges=False)
 
-    # create new lat/lon columns to preserve lat/lon for later reference if
-    # cols do not already exist (ie, don't overwrite in later re-projections)
-    if "lon" not in gdf_nodes.columns or "lat" not in gdf_nodes.columns:
-        gdf_nodes["lon"] = gdf_nodes["x"]
-        gdf_nodes["lat"] = gdf_nodes["y"]
-
     # project the nodes GeoDataFrame and extract the projected x/y values
     gdf_nodes_proj = project_gdf(gdf_nodes, to_crs=to_crs)
     gdf_nodes_proj["x"] = gdf_nodes_proj["geometry"].x
     gdf_nodes_proj["y"] = gdf_nodes_proj["geometry"].y
     to_crs = gdf_nodes_proj.crs
-    gdf_nodes_proj = gdf_nodes_proj.drop(columns=["geometry"])
 
     # STEP 2: PROJECT THE EDGES
-    if "simplified" in G.graph and G.graph["simplified"]:
+    if G.graph.get("simplified"):
         # if graph has previously been simplified, project the edge geometries
         gdf_edges = convert.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
         gdf_edges_proj = project_gdf(gdf_edges, to_crs=to_crs)
     else:
         # if not, you don't have to project these edges because the nodes
         # contain all the spatial data in the graph (unsimplified edges have
         # no geometry attributes)
-        gdf_edges_proj = convert.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False).drop(
-            columns=["geometry"]
-        )
+        gdf_edges_proj = convert.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
 
     # STEP 3: REBUILD GRAPH
     # turn projected node/edge gdfs into a graph and update its CRS attribute
-    G_proj = convert.graph_from_gdfs(gdf_nodes_proj, gdf_edges_proj, G.graph)
+    G_proj = convert.graph_from_gdfs(gdf_nodes_proj, gdf_edges_proj, graph_attrs=G.graph)
     G_proj.graph["crs"] = to_crs
 
-    utils.log(f"Projected graph with {len(G)} nodes and {len(G.edges)} edges")
+    msg = f"Projected graph with {len(G)} nodes and {len(G.edges)} edges"
+    utils.log(msg, level=lg.INFO)
     return G_proj
```

### Comparing `osmnx-1.9.3/osmnx/simplification.py` & `osmnx-2.0.0b0/osmnx/simplification.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,79 @@
-"""Simplify, correct, and consolidate network topology."""
+"""Simplify, correct, and consolidate spatial graph nodes and edges."""
+
+from __future__ import annotations
 
 import logging as lg
-from warnings import warn
+from typing import TYPE_CHECKING
+from typing import Any
 
 import geopandas as gpd
 import networkx as nx
-from shapely.geometry import LineString
-from shapely.geometry import MultiPolygon
-from shapely.geometry import Point
-from shapely.geometry import Polygon
+import numpy as np
+import pandas as pd
+from shapely import LineString
+from shapely import Point
 
 from . import convert
 from . import stats
 from . import utils
 from ._errors import GraphSimplificationError
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+    from collections.abc import Iterator
+
 
-def _is_endpoint(G, node, endpoint_attrs):
+def _is_endpoint(
+    G: nx.MultiDiGraph,
+    node: int,
+    node_attrs_include: Iterable[str] | None,
+    edge_attrs_differ: Iterable[str] | None,
+) -> bool:
     """
     Determine if a node is a true endpoint of an edge.
 
     Return True if the node is a "true" endpoint of an edge in the network,
     otherwise False. OpenStreetMap data includes many nodes that exist only as
-    geometric vertices to allow ways to curve. A true edge endpoint is a node
-    that satisfies at least 1 of the following 4 rules:
+    geometric vertices to allow ways to curve. `node` is a true edge endpoint
+    if it satisfies at least 1 of the following 5 rules:
 
     1) It is its own neighbor (ie, it self-loops).
 
     2) Or, it has no incoming edges or no outgoing edges (ie, all its incident
     edges are inbound or all its incident edges are outbound).
 
     3) Or, it does not have exactly two neighbors and degree of 2 or 4.
 
-    4) Or, if `endpoint_attrs` is not None, and its incident edges have
+    4) Or, if `node_attrs_include` is not None and it has one or more of the
+    attributes in `node_attrs_include`.
+
+    5) Or, if `edge_attrs_differ` is not None and its incident edges have
     different values than each other for any of the edge attributes in
-    `endpoint_attrs`.
+    `edge_attrs_differ`.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    node : int
-        the node to examine
-    endpoint_attrs : iterable
-        An iterable of edge attribute names for relaxing the strictness of
-        endpoint determination. If not None, a node is an endpoint if its
-        incident edges have different values then each other for any of the
-        edge attributes in `endpoint_attrs`.
+    G
+        Input graph.
+    node
+        The ID of the node.
+    node_attrs_include
+        Node attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if it possesses one or
+        more of the attributes in `node_attrs_include`.
+    edge_attrs_differ
+        Edge attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if its incident edges have
+        different values than each other for any attribute in
+        `edge_attrs_differ`.
 
     Returns
     -------
-    bool
+    endpoint
     """
     neighbors = set(list(G.predecessors(node)) + list(G.successors(node)))
     n = len(neighbors)
     d = G.degree(node)
 
     # RULE 1
     # if the node appears in its list of neighbors, it self-loops: this is
@@ -73,51 +92,61 @@
     # a dead-end or an intersection of multiple streets or it has 2 neighbors
     # but 3 degree (indicating a change from oneway to twoway) or more than 4
     # degree (indicating a parallel edge) and thus is an endpoint
     if not ((n == 2) and (d in {2, 4})):  # noqa: PLR2004
         return True
 
     # RULE 4
+    # non-strict mode: does it contain an attr denoting that it is an endpoint
+    if node_attrs_include is not None and len(set(node_attrs_include) & G.nodes[node].keys()) > 0:
+        return True
+
+    # RULE 5
     # non-strict mode: do its incident edges have different attr values? for
     # each attribute to check, collect the attribute's values in all inbound
-    # and outbound edges. if there is more than 1 unique value then then this
-    # node is an endpoint
-    if endpoint_attrs is not None:
-        for attr in endpoint_attrs:
+    # and outbound edges. if there is more than 1 unique value then this node
+    # is an endpoint
+    if edge_attrs_differ is not None:
+        for attr in edge_attrs_differ:
             in_values = {v for _, _, v in G.in_edges(node, data=attr, keys=False)}
             out_values = {v for _, _, v in G.out_edges(node, data=attr, keys=False)}
             if len(in_values | out_values) > 1:
                 return True
 
     # if none of the preceding rules passed, then it is not an endpoint
     return False
 
 
-def _build_path(G, endpoint, endpoint_successor, endpoints):
+def _build_path(
+    G: nx.MultiDiGraph,
+    endpoint: int,
+    endpoint_successor: int,
+    endpoints: set[int],
+) -> list[int]:
     """
     Build a path of nodes from one endpoint node to next endpoint node.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    endpoint : int
-        the endpoint node from which to start the path
-    endpoint_successor : int
-        the successor of endpoint through which the path to the next endpoint
-        will be built
-    endpoints : set
-        the set of all nodes in the graph that are endpoints
+    G
+        Input graph.
+    endpoint
+        Ehe endpoint node from which to start the path.
+    endpoint_successor
+        The successor of endpoint through which the path to the next endpoint
+        will be built.
+    endpoints
+        The set of all nodes in the graph that are endpoints.
 
     Returns
     -------
-    path : list
-        the first and last items in the resulting path list are endpoint
+    path
+        The first and last items in the resulting path list are endpoint
         nodes, and all other items are interstitial nodes that can be removed
-        subsequently
+        subsequently.
     """
     # start building path from endpoint node through its successor
     path = [endpoint, endpoint_successor]
 
     # for each successor of the endpoint's successor
     for this_successor in G.successors(endpoint_successor):
         successor = this_successor
@@ -135,452 +164,503 @@
                     path.append(successor)
 
                 # handle relatively rare cases or OSM digitization quirks
                 elif len(successors) == 0:
                     if endpoint in G.successors(successor):
                         # we have come to the end of a self-looping edge, so
                         # add first node to end of path to close it and return
-                        return path + [endpoint]
+                        return [*path, endpoint]
 
                     # otherwise, this can happen due to OSM digitization error
                     # where a one-way street turns into a two-way here, but
                     # duplicate incoming one-way edges are present
                     msg = f"Unexpected simplify pattern handled near {successor}"
                     utils.log(msg, level=lg.WARNING)
                     return path
                 else:  # pragma: no cover
                     # if successor has >1 successors, then successor must have
                     # been an endpoint because you can go in 2 new directions.
                     # this should never occur in practice
-                    msg = f"Impossible simplify pattern failed near {successor}"
+                    msg = f"Impossible simplify pattern failed near {successor}."
                     raise GraphSimplificationError(msg)
 
             # if this successor is an endpoint, we've completed the path
             return path
 
     # if endpoint_successor has no successors not already in the path, return
     # the current path: this is usually due to a digitization quirk on OSM
     return path
 
 
-def _get_paths_to_simplify(G, endpoint_attrs):
+def _get_paths_to_simplify(
+    G: nx.MultiDiGraph,
+    node_attrs_include: Iterable[str] | None,
+    edge_attrs_differ: Iterable[str] | None,
+) -> Iterator[list[int]]:
     """
     Generate all the paths to be simplified between endpoint nodes.
 
     The path is ordered from the first endpoint, through the interstitial nodes,
     to the second endpoint.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    endpoint_attrs : iterable
-        An iterable of edge attribute names for relaxing the strictness of
-        endpoint determination. If not None, a node is an endpoint if its
-        incident edges have different values then each other for any of the
-        edge attributes in `endpoint_attrs`.
+    G
+        Input graph.
+    node_attrs_include
+        Node attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if it possesses one or
+        more of the attributes in `node_attrs_include`.
+    edge_attrs_differ
+        Edge attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if its incident edges have
+        different values than each other for any attribute in
+        `edge_attrs_differ`.
 
     Yields
     ------
-    path_to_simplify : list
-        a generator of paths to simplify
+    path_to_simplify
     """
     # first identify all the nodes that are endpoints
-    endpoints = {n for n in G.nodes if _is_endpoint(G, n, endpoint_attrs)}
-    utils.log(f"Identified {len(endpoints):,} edge endpoints")
+    endpoints = {n for n in G.nodes if _is_endpoint(G, n, node_attrs_include, edge_attrs_differ)}
+    msg = f"Identified {len(endpoints):,} edge endpoints"
+    utils.log(msg, level=lg.INFO)
 
     # for each endpoint node, look at each of its successor nodes
     for endpoint in endpoints:
         for successor in G.successors(endpoint):
             if successor not in endpoints:
                 # if endpoint node's successor is not an endpoint, build path
                 # from the endpoint node, through the successor, and on to the
                 # next endpoint node
                 yield _build_path(G, endpoint, successor, endpoints)
 
 
-def _remove_rings(G, endpoint_attrs):
+def _remove_rings(
+    G: nx.MultiDiGraph,
+    node_attrs_include: Iterable[str] | None,
+    edge_attrs_differ: Iterable[str] | None,
+) -> nx.MultiDiGraph:
     """
-    Remove all self-contained rings from a graph.
+    Remove all graph components that consist only of a single chordless cycle.
 
-    This identifies any connected components that form a self-contained ring
-    without any endpoints, and removes them from the graph.
+    This identifies all connected components in the graph that consist only of
+    a single isolated self-contained ring, and removes them from the graph.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    endpoint_attrs : iterable
-        An iterable of edge attribute names for relaxing the strictness of
-        endpoint determination. If not None, a node is an endpoint if its
-        incident edges have different values then each other for any of the
-        edge attributes in `endpoint_attrs`.
+    G
+        Input graph.
+    node_attrs_include
+        Node attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if it possesses one or
+        more of the attributes in `node_attrs_include`.
+    edge_attrs_differ
+        Edge attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if its incident edges have
+        different values than each other for any attribute in
+        `edge_attrs_differ`.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        graph with self-contained rings removed
+    G
+        Graph with all chordless cycle components removed.
     """
-    nodes_in_rings = set()
+    to_remove = set()
     for wcc in nx.weakly_connected_components(G):
-        if not any(_is_endpoint(G, n, endpoint_attrs) for n in wcc):
-            nodes_in_rings.update(wcc)
-    G.remove_nodes_from(nodes_in_rings)
+        if not any(_is_endpoint(G, n, node_attrs_include, edge_attrs_differ) for n in wcc):
+            to_remove.update(wcc)
+    G.remove_nodes_from(to_remove)
     return G
 
 
-def simplify_graph(  # noqa: C901
-    G,
-    strict=None,
-    edge_attrs_differ=None,
-    endpoint_attrs=None,
-    remove_rings=True,
-    track_merged=False,
-):
+def simplify_graph(  # noqa: C901, PLR0912
+    G: nx.MultiDiGraph,
+    *,
+    node_attrs_include: Iterable[str] | None = None,
+    edge_attrs_differ: Iterable[str] | None = None,
+    remove_rings: bool = True,
+    track_merged: bool = False,
+    edge_attr_aggs: dict[str, Any] | None = None,
+) -> nx.MultiDiGraph:
     """
     Simplify a graph's topology by removing interstitial nodes.
 
-    This simplifies graph topology by removing all nodes that are not
+    This simplifies the graph's topology by removing all nodes that are not
     intersections or dead-ends, by creating an edge directly between the end
     points that encapsulate them while retaining the full geometry of the
     original edges, saved as a new `geometry` attribute on the new edge.
 
     Note that only simplified edges receive a `geometry` attribute. Some of
     the resulting consolidated edges may comprise multiple OSM ways, and if
-    so, their multiple attribute values are stored as a list. Optionally, the
+    so, their unique attribute values are stored as a list. Optionally, the
     simplified edges can receive a `merged_edges` attribute that contains a
-    list of all the (u, v) node pairs that were merged together.
+    list of all the `(u, v)` node pairs that were merged together.
 
-    Use the `edge_attrs_differ` parameter to relax simplification strictness. For
-    example, `edge_attrs_differ=['osmid']` will retain every node whose incident
-    edges have different OSM IDs. This lets you keep nodes at elbow two-way
-    intersections (but be aware that sometimes individual blocks have multiple
-    OSM IDs within them too). You could also use this parameter to retain
-    nodes where sidewalks or bike lanes begin/end in the middle of a block.
+    Use the `node_attrs_include` or `edge_attrs_differ` parameters to relax
+    simplification strictness. For example, `edge_attrs_differ=["osmid"]` will
+    retain every node whose incident edges have different OSM IDs. This lets
+    you keep nodes at elbow two-way intersections (but be aware that sometimes
+    individual blocks have multiple OSM IDs within them too). You could also
+    use this parameter to retain nodes where sidewalks or bike lanes begin/end
+    in the middle of a block. Or for example, `node_attrs_include=["highway"]`
+    will retain every node with a "highway" attribute (regardless of its
+    value), even if it does not represent a street junction.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    strict : bool
-        deprecated, do not use
-    edge_attrs_differ : iterable
-        An iterable of edge attribute names for relaxing the strictness of
-        endpoint determination. If not None, a node is an endpoint if its
-        incident edges have different values then each other for any of the
-        edge attributes in `edge_attrs_differ`.
-    endpoint_attrs : iterable
-        deprecated, do not use
-    remove_rings : bool
-        if True, remove isolated self-contained rings that have no endpoints
-    track_merged : bool
-        if True, add `merged_edges` attribute on simplified edges, containing
-        a list of all the (u, v) node pairs that were merged together
+    G
+        Input graph.
+    node_attrs_include
+        Node attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if it possesses one or
+        more of the attributes in `node_attrs_include`.
+    edge_attrs_differ
+        Edge attribute names for relaxing the strictness of endpoint
+        determination. A node is always an endpoint if its incident edges have
+        different values than each other for any attribute in
+        `edge_attrs_differ`.
+    remove_rings
+        If True, remove any graph components that consist only of a single
+        chordless cycle (i.e., an isolated self-contained ring).
+    track_merged
+        If True, add `merged_edges` attribute on simplified edges, containing
+        a list of all the `(u, v)` node pairs that were merged together.
+    edge_attr_aggs
+        Allows user to aggregate edge segment attributes when simplifying an
+        edge. Keys are edge attribute names and values are aggregation
+        functions to apply to these attributes when they exist for a set of
+        edges being merged. Edge attributes not in `edge_attr_aggs` will
+        contain the unique values across the merged edge segments. If None,
+        defaults to `{"length": sum, "travel_time": sum}`.
 
     Returns
     -------
-    G : networkx.MultiDiGraph
-        topologically simplified graph, with a new `geometry` attribute on
-        each simplified edge
-    """
-    if endpoint_attrs is not None:
-        msg = (
-            "The `endpoint_attrs` parameter has been deprecated and will be removed "
-            "in the v2.0.0 release. Use the `edge_attrs_differ` parameter instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-        edge_attrs_differ = endpoint_attrs
-
-    if strict is not None:
-        msg = (
-            "The `strict` parameter has been deprecated and will be removed in "
-            "the v2.0.0 release. Use the `edge_attrs_differ` parameter instead to "
-            "relax simplification strictness. For example, `edge_attrs_differ=None` "
-            "reproduces the old `strict=True` behvavior and `edge_attrs_differ=['osmid']` "
-            "reproduces the old `strict=False` behavior. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-        # maintain old behavior if strict is passed during deprecation
-        edge_attrs_differ = None if strict else ["osmid"]
-
-    if "simplified" in G.graph and G.graph["simplified"]:  # pragma: no cover
+    G
+        Topologically simplified graph, with a new `geometry` attribute on
+        each simplified edge.
+    """
+    if G.graph.get("simplified"):  # pragma: no cover
         msg = "This graph has already been simplified, cannot simplify it again."
         raise GraphSimplificationError(msg)
 
-    utils.log("Begin topologically simplifying the graph...")
+    msg = "Begin topologically simplifying the graph..."
+    utils.log(msg, level=lg.INFO)
 
-    # define edge segment attributes to sum upon edge simplification
-    attrs_to_sum = {"length", "travel_time"}
+    # default edge segment attributes to aggregate upon simplification
+    if edge_attr_aggs is None:
+        edge_attr_aggs = {"length": sum, "travel_time": sum}
 
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
     initial_node_count = len(G)
     initial_edge_count = len(G.edges)
     all_nodes_to_remove = []
     all_edges_to_add = []
 
     # generate each path that needs to be simplified
-    for path in _get_paths_to_simplify(G, edge_attrs_differ):
+    for path in _get_paths_to_simplify(G, node_attrs_include, edge_attrs_differ):
         # add the interstitial edges we're removing to a list so we can retain
         # their spatial geometry
         merged_edges = []
-        path_attributes = {}
+        path_attributes: dict[str, Any] = {}
         for u, v in zip(path[:-1], path[1:]):
             if track_merged:
                 # keep track of the edges that were merged
                 merged_edges.append((u, v))
 
             # there should rarely be multiple edges between interstitial nodes
             # usually happens if OSM has duplicate ways digitized for just one
             # street... we will keep only one of the edges (see below)
             edge_count = G.number_of_edges(u, v)
             if edge_count != 1:
-                utils.log(f"Found {edge_count} edges between {u} and {v} when simplifying")
+                msg = f"Found {edge_count} edges between {u} and {v} when simplifying"
+                utils.log(msg, level=lg.WARNING)
 
             # get edge between these nodes: if multiple edges exist between
             # them (see above), we retain only one in the simplified graph
             # We can't assume that there exists an edge from u to v
             # with key=0, so we get a list of all edges from u to v
             # and just take the first one.
-            edge_data = list(G.get_edge_data(u, v).values())[0]
+            edge_data = next(iter(G.get_edge_data(u, v).values()))
             for attr in edge_data:
                 if attr in path_attributes:
                     # if this key already exists in the dict, append it to the
                     # value list
                     path_attributes[attr].append(edge_data[attr])
                 else:
                     # if this key doesn't already exist, set the value to a list
                     # containing the one value
                     path_attributes[attr] = [edge_data[attr]]
 
         # consolidate the path's edge segments' attribute values
         for attr in path_attributes:
-            if attr in attrs_to_sum:
-                # if this attribute must be summed, sum it now
-                path_attributes[attr] = sum(path_attributes[attr])
+            if attr in edge_attr_aggs:
+                # if this attribute's values must be aggregated, do so now
+                agg_func = edge_attr_aggs[attr]
+                path_attributes[attr] = agg_func(path_attributes[attr])
             elif len(set(path_attributes[attr])) == 1:
-                # if there's only 1 unique value in this attribute list,
-                # consolidate it to the single value (the zero-th):
+                # if there's only 1 unique value, keep that single value
                 path_attributes[attr] = path_attributes[attr][0]
             else:
-                # otherwise, if there are multiple values, keep one of each
+                # otherwise, if there are multiple uniques, keep one of each
                 path_attributes[attr] = list(set(path_attributes[attr]))
 
         # construct the new consolidated edge's geometry for this path
         path_attributes["geometry"] = LineString(
-            [Point((G.nodes[node]["x"], G.nodes[node]["y"])) for node in path]
+            [Point((G.nodes[node]["x"], G.nodes[node]["y"])) for node in path],
         )
 
         if track_merged:
             # add the merged edges as a new attribute of the simplified edge
             path_attributes["merged_edges"] = merged_edges
 
         # add the nodes and edge to their lists for processing at the end
         all_nodes_to_remove.extend(path[1:-1])
         all_edges_to_add.append(
-            {"origin": path[0], "destination": path[-1], "attr_dict": path_attributes}
+            {"origin": path[0], "destination": path[-1], "attr_dict": path_attributes},
         )
 
     # for each edge to add in the list we assembled, create a new edge between
     # the origin and destination
     for edge in all_edges_to_add:
         G.add_edge(edge["origin"], edge["destination"], **edge["attr_dict"])
 
     # finally remove all the interstitial nodes between the new edges
     G.remove_nodes_from(set(all_nodes_to_remove))
 
     if remove_rings:
-        G = _remove_rings(G, edge_attrs_differ)
+        G = _remove_rings(G, node_attrs_include, edge_attrs_differ)
 
     # mark the graph as having been simplified
     G.graph["simplified"] = True
 
     msg = (
         f"Simplified graph: {initial_node_count:,} to {len(G):,} nodes, "
         f"{initial_edge_count:,} to {len(G.edges):,} edges"
     )
-    utils.log(msg)
+    utils.log(msg, level=lg.INFO)
     return G
 
 
 def consolidate_intersections(
-    G, tolerance=10, rebuild_graph=True, dead_ends=False, reconnect_edges=True
-):
+    G: nx.MultiDiGraph,
+    *,
+    tolerance: float | dict[int, float] = 10,
+    rebuild_graph: bool = True,
+    dead_ends: bool = False,
+    reconnect_edges: bool = True,
+    node_attr_aggs: dict[str, Any] | None = None,
+) -> nx.MultiDiGraph | gpd.GeoSeries:
     """
     Consolidate intersections comprising clusters of nearby nodes.
 
     Merges nearby nodes and returns either their centroids or a rebuilt graph
     with consolidated intersections and reconnected edge geometries. The
-    tolerance argument should be adjusted to approximately match street design
-    standards in the specific street network, and you should always use a
-    projected graph to work in meaningful and consistent units like meters.
-    Note the tolerance represents a per-node buffering radius: for example, to
-    consolidate nodes within 10 meters of each other, use tolerance=5.
+    `tolerance` argument can be a single value applied to all nodes or
+    individual per-node values. It should be adjusted to approximately match
+    street design standards in the specific street network, and you should use
+    a projected graph to work in meaningful and consistent units like meters.
+    Note: `tolerance` represents a per-node buffering radius. For example, to
+    consolidate nodes within 10 meters of each other, use `tolerance=5`.
 
-    When rebuild_graph=False, it uses a purely geometrical (and relatively
+    When `rebuild_graph` is False, it uses a purely geometric (and relatively
     fast) algorithm to identify "geometrically close" nodes, merge them, and
-    return just the merged intersections' centroids. When rebuild_graph=True,
+    return the merged intersections' centroids. When `rebuild_graph` is True,
     it uses a topological (and slower but more accurate) algorithm to identify
     "topologically close" nodes, merge them, then rebuild/return the graph.
-    Returned graph's node IDs represent clusters rather than osmids. Refer to
-    nodes' osmid_original attributes for original osmids. If multiple nodes
-    were merged together, the osmid_original attribute is a list of merged
-    nodes' osmids.
+    Returned graph's node IDs represent clusters rather than "osmid" values.
+    Refer to nodes' "osmid_original" attributes for original "osmid" values.
+    If multiple nodes were merged together, the "osmid_original" attribute is
+    a list of merged nodes' "osmid" values.
 
     Divided roads are often represented by separate centerline edges. The
     intersection of two divided roads thus creates 4 nodes, representing where
     each edge intersects a perpendicular edge. These 4 nodes represent a
     single intersection in the real world. A similar situation occurs with
     roundabouts and traffic circles. This function consolidates nearby nodes
     by buffering them to an arbitrary distance, merging overlapping buffers,
     and taking their centroid.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        a projected graph
-    tolerance : float
-        nodes are buffered to this distance (in graph's geometry's units) and
-        subsequent overlaps are dissolved into a single node
-    rebuild_graph : bool
-        if True, consolidate the nodes topologically, rebuild the graph, and
-        return as networkx.MultiDiGraph. if False, consolidate the nodes
-        geometrically and return the consolidated node points as
-        geopandas.GeoSeries
-    dead_ends : bool
-        if False, discard dead-end nodes to return only street-intersection
-        points
-    reconnect_edges : bool
-        ignored if rebuild_graph is not True. if True, reconnect edges and
-        their geometries in rebuilt graph to the consolidated nodes and update
-        edge length attributes; if False, returned graph has no edges (which
-        is faster if you just need topologically consolidated intersection
-        counts).
+    G
+        A projected graph.
+    tolerance
+        Nodes are buffered to this distance (in graph's geometry's units) and
+        subsequent overlaps are dissolved into a single node. If scalar, then
+        that single value will be used for all nodes. If dict (mapping node
+        IDs to individual values), then those values will be used per node and
+        any missing node IDs will not be buffered.
+    rebuild_graph
+        If True, consolidate the nodes topologically, rebuild the graph, and
+        return as MultiDiGraph. Otherwise, consolidate the nodes geometrically
+        and return the consolidated node points as GeoSeries.
+    dead_ends
+        If False, discard dead-end nodes to return only street-intersection
+        points.
+    reconnect_edges
+        If True, reconnect edges (and their geometries) to the consolidated
+        nodes in rebuilt graph, and update the edge length attributes. If
+        False, the returned graph has no edges (which is faster if you just
+        need topologically consolidated intersection counts). Ignored if
+        `rebuild_graph` is not True.
+    node_attr_aggs
+        Allows user to aggregate node attributes values when merging nodes.
+        Keys are node attribute names and values are aggregation functions
+        (anything accepted as an argument by `pandas.agg`). Node attributes
+        not in `node_attr_aggs` will contain the unique values across the
+        merged nodes. If None, defaults to `{"elevation": numpy.mean}`.
 
     Returns
     -------
-    networkx.MultiDiGraph or geopandas.GeoSeries
-        if rebuild_graph=True, returns MultiDiGraph with consolidated
-        intersections and reconnected edge geometries. if rebuild_graph=False,
-        returns GeoSeries of shapely Points representing the centroids of
-        street intersections
+    G or gs
+        If `rebuild_graph=True`, returns MultiDiGraph with consolidated
+        intersections and (optionally) reconnected edge geometries. If
+        `rebuild_graph=False`, returns GeoSeries of Points representing the
+        centroids of street intersections.
     """
     # if dead_ends is False, discard dead-ends to retain only intersections
     if not dead_ends:
         spn = stats.streets_per_node(G)
         dead_end_nodes = [node for node, count in spn.items() if count <= 1]
 
         # make a copy to not mutate original graph object caller passed in
         G = G.copy()
         G.remove_nodes_from(dead_end_nodes)
 
     if rebuild_graph:
-        if not G or not G.edges:
+        if len(G.nodes) == 0 or len(G.edges) == 0:
             # cannot rebuild a graph with no nodes or no edges, just return it
             return G
 
         # otherwise
-        return _consolidate_intersections_rebuild_graph(G, tolerance, reconnect_edges)
+        return _consolidate_intersections_rebuild_graph(
+            G,
+            tolerance,
+            reconnect_edges,
+            node_attr_aggs,
+        )
 
     # otherwise, if we're not rebuilding the graph
-    if not G:
+    if len(G) == 0:
         # if graph has no nodes, just return empty GeoSeries
         return gpd.GeoSeries(crs=G.graph["crs"])
 
     # otherwise, return the centroids of the merged intersection polygons
     return _merge_nodes_geometric(G, tolerance).centroid
 
 
-def _merge_nodes_geometric(G, tolerance):
+def _merge_nodes_geometric(
+    G: nx.MultiDiGraph,
+    tolerance: float | dict[int, float],
+) -> gpd.GeoSeries:
     """
     Geometrically merge nodes within some distance of each other.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        a projected graph
-    tolerance : float
-        buffer nodes to this distance (in graph's geometry's units) then merge
-        overlapping polygons into a single polygon via a unary union operation
+    G
+        A projected graph.
+    tolerance
+        Nodes are buffered to this distance (in graph's geometry's units) and
+        subsequent overlaps are dissolved into a single node. If scalar, then
+        that single value will be used for all nodes. If dict (mapping node
+        IDs to individual values), then those values will be used per node and
+        any missing node IDs will not be buffered.
 
     Returns
     -------
-    merged : GeoSeries
-        the merged overlapping polygons of the buffered nodes
+    merged
+        The merged overlapping polygons of the buffered nodes.
     """
-    # buffer nodes GeoSeries then get unary union to merge overlaps
-    merged = convert.graph_to_gdfs(G, edges=False)["geometry"].buffer(tolerance).unary_union
-
-    # if only a single node results, make it iterable to convert to GeoSeries
-    merged = MultiPolygon([merged]) if isinstance(merged, Polygon) else merged
-    return gpd.GeoSeries(merged.geoms, crs=G.graph["crs"])
+    gdf_nodes = convert.graph_to_gdfs(G, edges=False)
 
-
-def _consolidate_intersections_rebuild_graph(G, tolerance=10, reconnect_edges=True):
+    if isinstance(tolerance, dict):
+        # create series of tolerances reindexed like nodes, then buffer, then
+        # fill nulls (resulting from missing tolerances) with original points,
+        # then merge overlapping geometries
+        tols = pd.Series(tolerance).reindex(gdf_nodes.index)
+        merged = gdf_nodes.buffer(tols).fillna(gdf_nodes["geometry"]).unary_union
+    else:
+        # buffer nodes then merge overlapping geometries
+        merged = gdf_nodes.buffer(tolerance).unary_union
+
+    # extract the member geometries if it's a multi-geometry
+    merged = merged.geoms if hasattr(merged, "geoms") else merged
+    return gpd.GeoSeries(merged, crs=G.graph["crs"])
+
+
+def _consolidate_intersections_rebuild_graph(  # noqa: C901,PLR0912,PLR0915
+    G: nx.MultiDiGraph,
+    tolerance: float | dict[int, float],
+    reconnect_edges: bool,  # noqa: FBT001
+    node_attr_aggs: dict[str, Any] | None,
+) -> nx.MultiDiGraph:
     """
     Consolidate intersections comprising clusters of nearby nodes.
 
     Merge nodes and return a rebuilt graph with consolidated intersections and
     reconnected edge geometries.
 
-    The tolerance argument should be adjusted to approximately match street
-    design standards in the specific street network, and you should always use
-    a projected graph to work in meaningful and consistent units like meters.
-
-    Returned graph's node IDs represent clusters rather than osmids. Refer to
-    nodes' osmid_original attributes for original osmids. If multiple nodes
-    were merged together, the osmid_original attribute is a list of merged
-    nodes' osmids.
-
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        a projected graph
-    tolerance : float
-        nodes are buffered to this distance (in graph's geometry's units) and
-        subsequent overlaps are dissolved into a single node
-    reconnect_edges : bool
-        ignored if rebuild_graph is not True. if True, reconnect edges and
-        their geometries in rebuilt graph to the consolidated nodes and update
-        edge length attributes; if False, returned graph has no edges (which
-        is faster if you just need topologically consolidated intersection
-        counts).
+    G
+        A projected graph.
+    tolerance
+        Nodes are buffered to this distance (in graph's geometry's units) and
+        subsequent overlaps are dissolved into a single node. If scalar, then
+        that single value will be used for all nodes. If dict (mapping node
+        IDs to individual values), then those values will be used per node and
+        any missing node IDs will not be buffered.
+    reconnect_edges
+        If True, reconnect edges (and their geometries) to the consolidated
+        nodes in rebuilt graph, and update the edge length attributes. If
+        False, the returned graph has no edges (which is faster if you just
+        need topologically consolidated intersection counts).
+    node_attr_aggs
+        Allows user to aggregate node attributes values when merging nodes.
+        Keys are node attribute names and values are aggregation functions
+        (anything accepted as an argument by `pandas.agg`). Node attributes
+        not in `node_attr_aggs` will contain the unique values across the
+        merged nodes. If None, defaults to `{"elevation": numpy.mean}`.
 
     Returns
     -------
-    H : networkx.MultiDiGraph
-        a rebuilt graph with consolidated intersections and reconnected
-        edge geometries
-    """
+    Gc
+        A rebuilt graph with consolidated intersections and (optionally)
+        reconnected edge geometries.
+    """
+    # default node attributes to aggregate upon consolidation
+    if node_attr_aggs is None:
+        node_attr_aggs = {"elevation": np.mean}
+
     # STEP 1
     # buffer nodes to passed-in distance and merge overlaps. turn merged nodes
     # into gdf and get centroids of each cluster as x, y
     node_clusters = gpd.GeoDataFrame(geometry=_merge_nodes_geometric(G, tolerance))
     centroids = node_clusters.centroid
     node_clusters["x"] = centroids.x
     node_clusters["y"] = centroids.y
 
     # STEP 2
     # attach each node to its cluster of merged nodes. first get the original
     # graph's node points then spatial join to give each node the label of
     # cluster it's within. make cluster labels type string.
-    node_points = convert.graph_to_gdfs(G, edges=False)[["geometry"]]
+    node_points = convert.graph_to_gdfs(G, edges=False).drop(columns=["x", "y"])
     gdf = gpd.sjoin(node_points, node_clusters, how="left", predicate="within")
     gdf = gdf.drop(columns="geometry").rename(columns={"index_right": "cluster"})
     gdf["cluster"] = gdf["cluster"].astype(str)
 
     # STEP 3
     # if a cluster contains multiple components (i.e., it's not connected)
     # move each component to its own cluster (otherwise you will connect
     # nodes together that are not truly connected, e.g., nearby deadends or
     # surface streets with bridge).
-    groups = gdf.groupby("cluster")
-    for cluster_label, nodes_subset in groups:
+    for cluster_label, nodes_subset in gdf.groupby("cluster"):
         if len(nodes_subset) > 1:
             # identify all the (weakly connected) component in cluster
             wccs = list(nx.weakly_connected_components(G.subgraph(nodes_subset.index)))
             if len(wccs) > 1:
                 # if there are multiple components in this cluster
                 for suffix, wcc in enumerate(wccs):
                     # set subcluster xy to the centroid of just these nodes
@@ -592,46 +672,57 @@
                     gdf.loc[idx, "cluster"] = f"{cluster_label}-{suffix}"
 
     # give nodes unique integer IDs (subclusters with suffixes are strings)
     gdf["cluster"] = gdf["cluster"].factorize()[0]
 
     # STEP 4
     # create new empty graph and copy over misc graph data
-    H = nx.MultiDiGraph()
-    H.graph = G.graph
+    Gc = nx.MultiDiGraph()
+    Gc.graph = G.graph
 
     # STEP 5
     # create a new node for each cluster of merged nodes
     # regroup now that we potentially have new cluster labels from step 3
     groups = gdf.groupby("cluster")
     for cluster_label, nodes_subset in groups:
         osmids = nodes_subset.index.to_list()
         if len(osmids) == 1:
             # if cluster is a single node, add that node to new graph
             osmid = osmids[0]
-            H.add_node(cluster_label, osmid_original=osmid, **G.nodes[osmid])
+            Gc.add_node(cluster_label, osmid_original=osmid, **G.nodes[osmid])
         else:
-            # if cluster is multiple merged nodes, create one new node to
-            # represent them
-            H.add_node(
-                cluster_label,
-                osmid_original=str(osmids),
-                x=nodes_subset["x"].iloc[0],
-                y=nodes_subset["y"].iloc[0],
-            )
-
-    # calculate street_count attribute for all nodes lacking it
-    null_nodes = [n for n, sc in H.nodes(data="street_count") if sc is None]
-    street_count = stats.count_streets_per_node(H, nodes=null_nodes)
-    nx.set_node_attributes(H, street_count, name="street_count")
+            # if cluster is multiple merged nodes, create one new node with
+            # attributes to represent the merged nodes' non-null values
+            node_attrs = {
+                "osmid_original": osmids,
+                "x": nodes_subset["x"].iloc[0],
+                "y": nodes_subset["y"].iloc[0],
+            }
+            for col in set(nodes_subset.columns):
+                # get the unique non-null values (we won't add null attrs)
+                unique_vals = list(set(nodes_subset[col].dropna()))
+                if len(unique_vals) > 0 and col in node_attr_aggs:
+                    # if this attribute's values must be aggregated, do so now
+                    node_attrs[col] = nodes_subset[col].agg(node_attr_aggs[col])
+                elif col == "street_count":
+                    # if user doesn't specifically handle street_count with an
+                    # agg function, just skip it here then calculate it later
+                    continue
+                elif len(unique_vals) == 1:
+                    # if there's 1 unique value for this attribute, keep it
+                    node_attrs[col] = unique_vals[0]
+                elif len(unique_vals) > 1:
+                    # if there are multiple unique values, keep one of each
+                    node_attrs[col] = unique_vals
+            Gc.add_node(cluster_label, **node_attrs)
 
-    if not G.edges or not reconnect_edges:
+    if len(G.edges) == 0 or not reconnect_edges:
         # if reconnect_edges is False or there are no edges in original graph
         # (after dead-end removed), then skip edges and return new graph as-is
-        return H
+        return Gc
 
     # STEP 6
     # create new edge from cluster to cluster for each edge in original graph
     gdf_edges = convert.graph_to_gdfs(G, nodes=False)
     for u, v, k, data in G.edges(keys=True, data=True):
         u2 = gdf.loc[u, "cluster"]
         v2 = gdf.loc[v, "cluster"]
@@ -639,36 +730,41 @@
         # only create the edge if we're not connecting the cluster
         # to itself, but always add original self-loops
         if (u2 != v2) or (u == v):
             data["u_original"] = u
             data["v_original"] = v
             if "geometry" not in data:
                 data["geometry"] = gdf_edges.loc[(u, v, k), "geometry"]
-            H.add_edge(u2, v2, **data)
+            Gc.add_edge(u2, v2, **data)
 
     # STEP 7
     # for every group of merged nodes with more than 1 node in it, extend the
     # edge geometries to reach the new node point
     for cluster_label, nodes_subset in groups:
         # but only if there were multiple nodes merged together,
         # otherwise it's the same old edge as in original graph
         if len(nodes_subset) > 1:
             # get coords of merged nodes point centroid to prepend or
             # append to the old edge geom's coords
-            x = H.nodes[cluster_label]["x"]
-            y = H.nodes[cluster_label]["y"]
+            x = Gc.nodes[cluster_label]["x"]
+            y = Gc.nodes[cluster_label]["y"]
             xy = [(x, y)]
 
             # for each edge incident on this new merged node, update its
             # geometry to extend to/from the new node's point coords
-            in_edges = set(H.in_edges(cluster_label, keys=True))
-            out_edges = set(H.out_edges(cluster_label, keys=True))
+            in_edges = set(Gc.in_edges(cluster_label, keys=True))
+            out_edges = set(Gc.out_edges(cluster_label, keys=True))
             for u, v, k in in_edges | out_edges:
-                old_coords = list(H.edges[u, v, k]["geometry"].coords)
+                old_coords = list(Gc.edges[u, v, k]["geometry"].coords)
                 new_coords = xy + old_coords if cluster_label == u else old_coords + xy
                 new_geom = LineString(new_coords)
-                H.edges[u, v, k]["geometry"] = new_geom
+                Gc.edges[u, v, k]["geometry"] = new_geom
 
                 # update the edge length attribute, given the new geometry
-                H.edges[u, v, k]["length"] = new_geom.length
+                Gc.edges[u, v, k]["length"] = new_geom.length
+
+    # calculate street_count attribute for all nodes lacking it
+    null_nodes = [n for n, sc in Gc.nodes(data="street_count") if sc is None]
+    street_counts = stats.count_streets_per_node(Gc, nodes=null_nodes)
+    nx.set_node_attributes(Gc, street_counts, name="street_count")
 
-    return H
+    return Gc
```

### Comparing `osmnx-1.9.3/osmnx/stats.py` & `osmnx-2.0.0b0/osmnx/stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,257 @@
 """
 Calculate geometric and topological network measures.
 
 This module defines streets as the edges in an undirected representation of
 the graph. Using undirected graph edges prevents double-counting bidirectional
 edges of a two-way street, but may double-count a divided road's separate
-centerlines with different end point nodes. If `clean_periphery=True` when the
-graph was created (which is the default parameterization), then you will get
-accurate node degrees (and in turn streets-per-node counts) even at the
-periphery of the graph.
+centerlines with different end point nodes. Due to OSMnx's periphery cleaning
+when the graph was created, you will get accurate node degrees (and in turn
+streets-per-node counts) even at the periphery of the graph.
 
 You can use NetworkX directly for additional topological network measures.
 """
 
-import itertools
+from __future__ import annotations
+
 import logging as lg
 from collections import Counter
+from itertools import chain
+from typing import TYPE_CHECKING
+from typing import Any
 
 import networkx as nx
 import numpy as np
 
 from . import convert
 from . import distance
 from . import projection
 from . import simplification
 from . import utils
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
 
-def streets_per_node(G):
+def streets_per_node(G: nx.MultiDiGraph) -> dict[int, int]:
     """
-    Count streets (undirected edges) incident on each node.
+    Retrieve nodes' `street_count` attribute values.
+
+    See also the `count_streets_per_node` function for the calculation.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    spn : dict
-        dictionary with node ID keys and street count values
+    spn
+        Dictionary with node ID keys and street count values.
     """
-    spn = dict(nx.get_node_attributes(G, "street_count"))
+    # ensure each count value has type int (otherwise could be type np.int64)
+    # if user has projected the graph bc GeoDataFrames use np.int64 for ints
+    spn = {k: int(v) for k, v in nx.get_node_attributes(G, "street_count").items()}
     if set(spn) != set(G.nodes):
-        utils.log("Graph nodes changed since `street_count`s were calculated", level=lg.WARNING)
+        msg = "Graph nodes changed since `street_count`s were calculated"
+        utils.log(msg, level=lg.WARNING)
     return spn
 
 
-def streets_per_node_avg(G):
+def streets_per_node_avg(G: nx.MultiDiGraph) -> float:
     """
     Calculate graph's average count of streets per node.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    spna : float
-        average count of streets per node
+    spna
+        Average count of streets per node.
     """
     spn_vals = streets_per_node(G).values()
-    return sum(spn_vals) / len(G.nodes)
+    return float(sum(spn_vals) / len(G.nodes))
 
 
-def streets_per_node_counts(G):
+def streets_per_node_counts(G: nx.MultiDiGraph) -> dict[int, int]:
     """
     Calculate streets-per-node counts.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    spnc : dict
-        dictionary keyed by count of streets incident on each node, and with
-        values of how many nodes in the graph have this count
+    spnc
+        Dictionary keyed by count of streets incident on each node, and with
+        values of how many nodes in the graph have this count.
     """
     spn_vals = list(streets_per_node(G).values())
     return {i: spn_vals.count(i) for i in range(int(max(spn_vals)) + 1)}
 
 
-def streets_per_node_proportions(G):
+def streets_per_node_proportions(G: nx.MultiDiGraph) -> dict[int, float]:
     """
     Calculate streets-per-node proportions.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    spnp : dict
-        dictionary keyed by count of streets incident on each node, and with
-        values of what proportion of nodes in the graph have this count
+    spnp
+        Dictionary keyed by count of streets incident on each node, and with
+        values of what proportion of nodes in the graph have this count.
     """
     n = len(G.nodes)
     spnc = streets_per_node_counts(G)
     return {i: count / n for i, count in spnc.items()}
 
 
-def intersection_count(G=None, min_streets=2):
+def intersection_count(G: nx.MultiDiGraph, *, min_streets: int = 2) -> int:
     """
     Count the intersections in a graph.
 
     Intersections are defined as nodes with at least `min_streets` number of
     streets incident on them.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    min_streets : int
-        a node must have at least `min_streets` incident on them to count as
-        an intersection
+    G
+        Input graph.
+    min_streets
+        A node must have at least `min_streets` incident on them to count as
+        an intersection.
 
     Returns
     -------
-    count : int
-        count of intersections in graph
+    count
+        Count of intersections in graph.
     """
     spn = streets_per_node(G)
     node_ids = set(G.nodes)
-    return sum(count >= min_streets and node in node_ids for node, count in spn.items())
+    count = sum(c >= min_streets and n in node_ids for n, c in spn.items())
+
+    # ensure count value has type int (otherwise could be type np.int64) if
+    # user has projected the graph bc GeoDataFrames use np.int64 for ints
+    return int(count)
 
 
-def street_segment_count(Gu):
+def street_segment_count(Gu: nx.MultiGraph) -> int:
     """
     Count the street segments in a graph.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected input graph
+    Gu
+        Undirected input graph.
 
     Returns
     -------
-    count : int
-        count of street segments in graph
+    count
+        Count of street segments in graph.
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        msg = "`Gu` must be undirected"
+        msg = "`Gu` must be undirected."
         raise ValueError(msg)
     return len(Gu.edges)
 
 
-def street_length_total(Gu):
+def street_length_total(Gu: nx.MultiGraph) -> float:
     """
     Calculate graph's total street segment length.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected input graph
+    Gu
+        Undirected input graph.
 
     Returns
     -------
-    length : float
-        total length (meters) of streets in graph
+    length
+        Total length (meters) of streets in graph.
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        msg = "`Gu` must be undirected"
+        msg = "`Gu` must be undirected."
         raise ValueError(msg)
-    return sum(d["length"] for u, v, d in Gu.edges(data=True))
+    return float(sum(d["length"] for u, v, d in Gu.edges(data=True)))
 
 
-def edge_length_total(G):
+def edge_length_total(G: nx.MultiGraph) -> float:
     """
     Calculate graph's total edge length.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
+    G
+        Input graph.
 
     Returns
     -------
-    length : float
-        total length (meters) of edges in graph
+    length
+        Total length (meters) of edges in graph.
     """
-    return sum(d["length"] for u, v, d in G.edges(data=True))
+    return float(sum(d["length"] for u, v, d in G.edges(data=True)))
 
 
-def self_loop_proportion(Gu):
+def self_loop_proportion(Gu: nx.MultiGraph) -> float:
     """
     Calculate percent of edges that are self-loops in a graph.
 
     A self-loop is defined as an edge from node `u` to node `v` where `u==v`.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected input graph
+    Gu
+        Undirected input graph.
 
     Returns
     -------
-    proportion : float
-        proportion of graph edges that are self-loops
+    proportion
+        Proportion of graph edges that are self-loops.
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        msg = "`Gu` must be undirected"
+        msg = "`Gu` must be undirected."
         raise ValueError(msg)
-    return sum(u == v for u, v, k in Gu.edges) / len(Gu.edges)
+    return float(sum(u == v for u, v, k in Gu.edges) / len(Gu.edges))
 
 
-def circuity_avg(Gu):
+def circuity_avg(Gu: nx.MultiGraph) -> float | None:
     """
     Calculate average street circuity using edges of undirected graph.
 
     Circuity is the sum of edge lengths divided by the sum of straight-line
     distances between edge endpoints. Calculates straight-line distance as
     euclidean distance if projected or great-circle distance if unprojected.
+    Returns None if the edge lengths sum to zero.
 
     Parameters
     ----------
-    Gu : networkx.MultiGraph
-        undirected input graph
+    Gu
+        Undirected input graph.
 
     Returns
     -------
-    circuity_avg : float
-        the graph's average undirected edge circuity
+    circuity_avg
+        The graph's average undirected edge circuity.
     """
     if nx.is_directed(Gu):  # pragma: no cover
-        msg = "`Gu` must be undirected"
+        msg = "`Gu` must be undirected."
         raise ValueError(msg)
 
     # extract the edges' endpoint nodes' coordinates
-    coords = np.array(
-        [
-            (Gu.nodes[u]["y"], Gu.nodes[u]["x"], Gu.nodes[v]["y"], Gu.nodes[v]["x"])
-            for u, v, _ in Gu.edges
-        ]
-    )
+    n = Gu.nodes
+    coords = np.array([(n[u]["y"], n[u]["x"], n[v]["y"], n[v]["x"]) for u, v, _ in Gu.edges])
     y1 = coords[:, 0]
     x1 = coords[:, 1]
     y2 = coords[:, 2]
     x2 = coords[:, 3]
 
     # calculate straight-line distances as euclidean distances if projected or
     # great-circle distances if unprojected
@@ -247,94 +259,104 @@
         sl_dists = distance.euclidean(y1=y1, x1=x1, y2=y2, x2=x2)
     else:
         sl_dists = distance.great_circle(lat1=y1, lon1=x1, lat2=y2, lon2=x2)
 
     # return the ratio, handling possible division by zero
     sl_dists_total = sl_dists[~np.isnan(sl_dists)].sum()
     try:
-        return edge_length_total(Gu) / sl_dists_total
+        return float(edge_length_total(Gu) / sl_dists_total)
     except ZeroDivisionError:
         return None
 
 
-def count_streets_per_node(G, nodes=None):
+def count_streets_per_node(
+    G: nx.MultiDiGraph,
+    *,
+    nodes: Iterable[int] | None = None,
+) -> dict[int, int]:
     """
     Count how many physical street segments connect to each node in a graph.
 
     This function uses an undirected representation of the graph and special
     handling of self-loops to accurately count physical streets rather than
     directed edges. Note: this function is automatically run by all the
     `graph.graph_from_x` functions prior to truncating the graph to the
     requested boundaries, to add accurate `street_count` attributes to each
     node even if some of its neighbors are outside the requested graph
     boundaries.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    nodes : list
-        which node IDs to get counts for. if None, use all graph nodes,
-        otherwise calculate counts only for these node IDs
+    G
+        Input graph.
+    nodes
+        Which node IDs to get counts for. If None, use all graph nodes.
+        Otherwise calculate counts only for these node IDs.
 
     Returns
     -------
-    streets_per_node : dict
-        counts of how many physical streets connect to each node, with keys =
-        node ids and values = counts
+    streets_per_node
+        Counts of how many physical streets connect to each node, with keys =
+        node ids and values = counts.
     """
     if nodes is None:
         nodes = G.nodes
 
     # get one copy of each self-loop edge, because bi-directional self-loops
     # appear twice in the undirected graph (u,v,0 and u,v,1 where u=v), but
     # one-way self-loops will appear only once
     Gu = G.to_undirected(reciprocal=False, as_view=True)
-    self_loop_edges = set(nx.selfloop_edges(Gu))
+    self_loop_edges = set(nx.selfloop_edges(Gu, keys=False))
 
     # get all non-self-loop undirected edges, including parallel edges
     non_self_loop_edges = [e for e in Gu.edges(keys=False) if e not in self_loop_edges]
 
     # make list of all unique edges including each parallel edge unless the
     # parallel edge is a self-loop, in which case we don't double-count it
     all_unique_edges = non_self_loop_edges + list(self_loop_edges)
 
     # flatten list of (u, v) edge tuples to count how often each node appears
-    edges_flat = itertools.chain.from_iterable(all_unique_edges)
+    edges_flat = chain.from_iterable(all_unique_edges)
     counts = Counter(edges_flat)
     streets_per_node = {node: counts[node] for node in nodes}
 
-    utils.log("Counted undirected street segments incident on each node")
+    msg = "Counted undirected street segments incident on each node"
+    utils.log(msg, level=lg.INFO)
     return streets_per_node
 
 
-def basic_stats(G, area=None, clean_int_tol=None):
+def basic_stats(
+    G: nx.MultiDiGraph,
+    *,
+    area: float | None = None,
+    clean_int_tol: float | None = None,
+) -> dict[str, Any]:
     """
     Calculate basic descriptive geometric and topological measures of a graph.
 
     Density measures are only calculated if `area` is provided and clean
     intersection measures are only calculated if `clean_int_tol` is provided.
 
     Parameters
     ----------
-    G : networkx.MultiDiGraph
-        input graph
-    area : float
-        if not None, calculate density measures and use this value (in square
-        meters) as the denominator
-    clean_int_tol : float
-        if not None, calculate consolidated intersections count (and density,
-        if `area` is also provided) and use this tolerance value; refer to the
+    G
+        Input graph.
+    area
+        If not None, calculate density measures and use `area` (in square
+        meters) as the denominator.
+    clean_int_tol
+        If not None, calculate consolidated intersections count (and density,
+        if `area` is also provided) and use this tolerance value. Refer to the
         `simplification.consolidate_intersections` function documentation for
-        details
+        details.
 
     Returns
     -------
-    stats : dict
-        dictionary containing the following keys
+    stats
+        Dictionary containing the following keys:
           - `circuity_avg` - see `circuity_avg` function documentation
           - `clean_intersection_count` - see `clean_intersection_count` function documentation
           - `clean_intersection_density_km` - `clean_intersection_count` per sq km
           - `edge_density_km` - `edge_length_total` per sq km
           - `edge_length_avg` - `edge_length_total / m`
           - `edge_length_total` - see `edge_length_total` function documentation
           - `intersection_count` - see `intersection_count` function documentation
@@ -349,15 +371,15 @@
           - `street_length_total` - see `street_length_total` function documentation
           - `street_segment_count` - see `street_segment_count` function documentation
           - `streets_per_node_avg` - see `streets_per_node_avg` function documentation
           - `streets_per_node_counts` - see `streets_per_node_counts` function documentation
           - `streets_per_node_proportions` - see `streets_per_node_proportions` function documentation
     """
     Gu = convert.to_undirected(G)
-    stats = {}
+    stats: dict[str, Any] = {}
 
     stats["n"] = len(G.nodes)
     stats["m"] = len(G.edges)
     stats["k_avg"] = 2 * stats["m"] / stats["n"]
     stats["edge_length_total"] = edge_length_total(G)
     stats["edge_length_avg"] = stats["edge_length_total"] / stats["m"]
     stats["streets_per_node_avg"] = streets_per_node_avg(G)
@@ -370,16 +392,19 @@
     stats["circuity_avg"] = circuity_avg(Gu)
     stats["self_loop_proportion"] = self_loop_proportion(Gu)
 
     # calculate clean intersection counts if requested
     if clean_int_tol:
         stats["clean_intersection_count"] = len(
             simplification.consolidate_intersections(
-                G, tolerance=clean_int_tol, rebuild_graph=False, dead_ends=False
-            )
+                G,
+                tolerance=clean_int_tol,
+                rebuild_graph=False,
+                dead_ends=False,
+            ),
         )
 
     # can only calculate density measures if area was provided
     if area is not None:
         area_km = area / 1_000_000  # convert m^2 to km^2
         stats["node_density_km"] = stats["n"] / area_km
         stats["intersection_density_km"] = stats["intersection_count"] / area_km
```

### Comparing `osmnx-1.9.3/osmnx/utils_geo.py` & `osmnx-2.0.0b0/osmnx/utils_geo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,276 +1,127 @@
 """Geospatial utility functions."""
 
+from __future__ import annotations
+
+import logging as lg
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import Literal
+from typing import overload
 from warnings import warn
 
 import networkx as nx
 import numpy as np
-from shapely.geometry import LineString
-from shapely.geometry import MultiLineString
-from shapely.geometry import MultiPoint
-from shapely.geometry import MultiPolygon
-from shapely.geometry import Point
-from shapely.geometry import Polygon
+from shapely import LineString
+from shapely import MultiPolygon
+from shapely import Polygon
 from shapely.ops import split
 
 from . import convert
 from . import projection
 from . import settings
 from . import utils
 
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+
+    import geopandas as gpd
+
 
-def sample_points(G, n):
+def sample_points(G: nx.MultiGraph, n: int) -> gpd.GeoSeries:
     """
     Randomly sample points constrained to a spatial graph.
 
     This generates a graph-constrained uniform random sample of points. Unlike
     typical spatially uniform random sampling, this method accounts for the
     graph's geometry. And unlike equal-length edge segmenting, this method
     guarantees uniform randomness.
 
     Parameters
     ----------
-    G : networkx.MultiGraph
-        graph from which to sample points. should be undirected (to avoid
+    G
+        Graph from which to sample points. Should be undirected (to avoid
         oversampling bidirectional edges) and projected (for accurate point
-        interpolation)
-    n : int
-        how many points to sample
+        interpolation).
+    n
+        How many points to sample.
 
     Returns
     -------
-    points : geopandas.GeoSeries
-        the sampled points, multi-indexed by (u, v, key) of the edge from
-        which each point was drawn
+    point
+        The sampled points, multi-indexed by `(u, v, key)` of the edge from
+        which each point was sampled.
     """
     if nx.is_directed(G):  # pragma: no cover
-        warn("graph should be undirected to avoid oversampling bidirectional edges", stacklevel=2)
+        msg = "`G` should be undirected to avoid oversampling bidirectional edges."
+        warn(msg, category=UserWarning, stacklevel=2)
     gdf_edges = convert.graph_to_gdfs(G, nodes=False)[["geometry", "length"]]
     weights = gdf_edges["length"] / gdf_edges["length"].sum()
     idx = np.random.default_rng().choice(gdf_edges.index, size=n, p=weights)
     lines = gdf_edges.loc[idx, "geometry"]
     return lines.interpolate(np.random.default_rng().random(n), normalized=True)
 
 
-def interpolate_points(geom, dist):
+def interpolate_points(geom: LineString, dist: float) -> Iterator[tuple[float, float]]:
     """
     Interpolate evenly spaced points along a LineString.
 
     The spacing is approximate because the LineString's length may not be
     evenly divisible by it.
 
     Parameters
     ----------
-    geom : shapely.geometry.LineString
-        a LineString geometry
-    dist : float
-        spacing distance between interpolated points, in same units as `geom`.
-        smaller values accordingly generate more points.
+    geom
+        A LineString geometry.
+    dist
+        Spacing distance between interpolated points, in same units as `geom`.
+        Smaller values accordingly generate more points.
 
     Yields
     ------
-    points : generator
-        tuples of (x, y) floats of the interpolated points' coordinates
+    point
+        Interpolated point's `(x, y)` coordinates.
     """
     if isinstance(geom, LineString):
         num_vert = max(round(geom.length / dist), 1)
         for n in range(num_vert + 1):
             point = geom.interpolate(n / num_vert, normalized=True)
             yield point.x, point.y
     else:  # pragma: no cover
-        msg = f"unhandled geometry type {geom.geom_type}"
+        msg = "`geom` must be a LineString."
         raise TypeError(msg)
 
 
-def _round_polygon_coords(p, precision):
-    """
-    Round the coordinates of a shapely Polygon to some decimal precision.
-
-    Parameters
-    ----------
-    p : shapely.geometry.Polygon
-        the polygon to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.Polygon
-    """
-    # round coords of Polygon exterior
-    shell = [[round(x, precision) for x in c] for c in p.exterior.coords]
-
-    # round coords of (possibly multiple, possibly none) Polygon interior(s)
-    holes = [[[round(x, precision) for x in c] for c in i.coords] for i in p.interiors]
-
-    # construct new Polygon with rounded coordinates and buffer by zero to
-    # clean self-touching or self-crossing polygons
-    return Polygon(shell=shell, holes=holes).buffer(0)
-
-
-def _round_multipolygon_coords(mp, precision):
-    """
-    Round the coordinates of a shapely MultiPolygon to some decimal precision.
-
-    Parameters
-    ----------
-    mp : shapely.geometry.MultiPolygon
-        the MultiPolygon to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.MultiPolygon
-    """
-    return MultiPolygon([_round_polygon_coords(p, precision) for p in mp.geoms])
-
-
-def _round_point_coords(pt, precision):
-    """
-    Round the coordinates of a shapely Point to some decimal precision.
-
-    Parameters
-    ----------
-    pt : shapely.geometry.Point
-        the Point to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.Point
-    """
-    return Point([round(x, precision) for x in pt.coords[0]])
-
-
-def _round_multipoint_coords(mpt, precision):
-    """
-    Round the coordinates of a shapely MultiPoint to some decimal precision.
-
-    Parameters
-    ----------
-    mpt : shapely.geometry.MultiPoint
-        the MultiPoint to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.MultiPoint
-    """
-    return MultiPoint([_round_point_coords(pt, precision) for pt in mpt.geoms])
-
-
-def _round_linestring_coords(ls, precision):
-    """
-    Round the coordinates of a shapely LineString to some decimal precision.
-
-    Parameters
-    ----------
-    ls : shapely.geometry.LineString
-        the LineString to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.LineString
-    """
-    return LineString([[round(x, precision) for x in c] for c in ls.coords])
-
-
-def _round_multilinestring_coords(mls, precision):
-    """
-    Round the coordinates of a shapely MultiLineString to some decimal precision.
-
-    Parameters
-    ----------
-    mls : shapely.geometry.MultiLineString
-        the MultiLineString to round the coordinates of
-    precision : int
-        decimal precision to round coordinates to
-
-    Returns
-    -------
-    shapely.geometry.MultiLineString
-    """
-    return MultiLineString([_round_linestring_coords(ls, precision) for ls in mls.geoms])
-
-
-def round_geometry_coords(geom, precision):
+def _consolidate_subdivide_geometry(geometry: Polygon | MultiPolygon) -> MultiPolygon:
     """
-    Do not use: deprecated.
-
-    Parameters
-    ----------
-    geom : shapely.geometry.geometry {Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon}
-        deprecated, do not use
-    precision : int
-        deprecated, do not use
-
-    Returns
-    -------
-    shapely.geometry.geometry
-    """
-    warn(
-        "The `round_geometry_coords` function is deprecated and will be "
-        "removed in the v2.0.0 release. "
-        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
-        FutureWarning,
-        stacklevel=2,
-    )
-
-    if isinstance(geom, Point):
-        return _round_point_coords(geom, precision)
-
-    if isinstance(geom, MultiPoint):
-        return _round_multipoint_coords(geom, precision)
-
-    if isinstance(geom, LineString):
-        return _round_linestring_coords(geom, precision)
-
-    if isinstance(geom, MultiLineString):
-        return _round_multilinestring_coords(geom, precision)
-
-    if isinstance(geom, Polygon):
-        return _round_polygon_coords(geom, precision)
-
-    if isinstance(geom, MultiPolygon):
-        return _round_multipolygon_coords(geom, precision)
-
-    # otherwise
-    msg = f"cannot round coordinates of unhandled geometry type: {type(geom)}"
-    raise TypeError(msg)
-
-
-def _consolidate_subdivide_geometry(geometry):
-    """
-    Consolidate and subdivide some geometry.
+    Consolidate and subdivide some (projected) geometry.
 
     Consolidate a geometry into a convex hull, then subdivide it into smaller
     sub-polygons if its area exceeds max size (in geometry's units). Configure
-    the max size via max_query_area_size in the settings module.
+    the max size via the `settings` module's `max_query_area_size`. Geometries
+    with areas much larger than `max_query_area_size` may take a long time to
+    process.
 
     When the geometry has a very large area relative to its vertex count,
     the resulting MultiPolygon's boundary may differ somewhat from the input,
     due to the way long straight lines are projected. You can interpolate
-    additional vertices along your input geometry's exterior to mitigate this.
+    additional vertices along your input geometry's exterior to mitigate this
+    if necessary.
 
     Parameters
     ----------
-    geometry : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        the projected (in meter units) geometry to consolidate and subdivide
+    geometry
+        The projected (in meter units) geometry to consolidate and subdivide.
 
     Returns
     -------
-    geometry : shapely.geometry.MultiPolygon
+    geometry
     """
     if not isinstance(geometry, (Polygon, MultiPolygon)):  # pragma: no cover
-        msg = "Geometry must be a shapely Polygon or MultiPolygon"
+        msg = "Geometry must be a shapely Polygon or MultiPolygon."
         raise TypeError(msg)
 
     # if geometry is either 1) a Polygon whose area exceeds the max size, or
     # 2) a MultiPolygon, then get the convex hull around the geometry
     mqas = settings.max_query_area_size
     if isinstance(geometry, MultiPolygon) or (
         isinstance(geometry, Polygon) and geometry.area > mqas
@@ -282,42 +133,42 @@
     warning_threshold = 10
     if ratio > warning_threshold:
         msg = (
             f"This area is {ratio:,} times your configured Overpass max query "
             "area size. It will automatically be divided up into multiple "
             "sub-queries accordingly. This may take a long time."
         )
-        warn(msg, stacklevel=2)
+        warn(msg, category=UserWarning, stacklevel=2)
 
     # if geometry area exceeds max size, subdivide it into smaller subpolygons
     # that are no greater than settings.max_query_area_size in size
     if geometry.area > mqas:
         geometry = _quadrat_cut_geometry(geometry, quadrat_width=np.sqrt(mqas))
 
     if isinstance(geometry, Polygon):
         geometry = MultiPolygon([geometry])
 
     return geometry
 
 
-def _quadrat_cut_geometry(geometry, quadrat_width):
+def _quadrat_cut_geometry(geometry: Polygon | MultiPolygon, quadrat_width: float) -> MultiPolygon:
     """
     Split a Polygon or MultiPolygon up into sub-polygons of a specified size.
 
     Parameters
     ----------
-    geometry : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        the geometry to split up into smaller sub-polygons
-    quadrat_width : float
-        width (in geometry's units) of quadrat squares with which to split up
-        the geometry
+    geometry
+        The geometry to split up into smaller sub-polygons.
+    quadrat_width
+        Width (in geometry's units) of quadrat squares with which to split up
+        the geometry.
 
     Returns
     -------
-    geometry : shapely.geometry.MultiPolygon
+    geometry
     """
     # min number of dividing lines (3 produces a grid of 4 quadrat squares)
     min_num = 3
 
     # create n evenly spaced points between the min and max x and y bounds
     west, south, east, north = geometry.bounds
     x_num = int(np.ceil((east - west) / quadrat_width) + 1)
@@ -337,83 +188,187 @@
         split_geoms = [split(g, line).geoms if g.intersects(line) else [g] for g in geometries]
         # now flatten the list and process these split geoms on the next line in the list of lines
         geometries = [g for g_list in split_geoms for g in g_list]
 
     return MultiPolygon(geometries)
 
 
-def _intersect_index_quadrats(geometries, polygon):
+def _intersect_index_quadrats(
+    geometries: gpd.GeoSeries,
+    polygon: Polygon | MultiPolygon,
+) -> set[Any]:
     """
     Identify geometries that intersect a (Multi)Polygon.
 
     Uses an r-tree spatial index and cuts polygon up into smaller sub-polygons
     for r-tree acceleration. Ensure that geometries and polygon are in the
     same coordinate reference system.
 
     Parameters
     ----------
-    geometries : geopandas.GeoSeries
-        the geometries to intersect with the polygon
-    polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
-        the polygon to intersect with the geometries
+    geometries
+        The geometries to intersect with the polygon.
+    polygon
+        The polygon to intersect with the geometries.
 
     Returns
     -------
-    geoms_in_poly : set
-        set of the index labels of the geometries that intersected the polygon
+    geoms_in_poly
+        The index labels of the geometries that intersected the polygon.
     """
     # create an r-tree spatial index for the geometries
     rtree = geometries.sindex
-    utils.log(f"Built r-tree spatial index for {len(geometries):,} geometries")
+    msg = f"Built r-tree spatial index for {len(geometries):,} geometries"
+    utils.log(msg, level=lg.INFO)
 
     # cut polygon into chunks for faster spatial index intersecting. specify a
     # sensible quadrat_width to balance performance (eg, 0.1 degrees is approx
     # 8 km at NYC's latitude) with either projected or unprojected coordinates
     quadrat_width = max(0.1, np.sqrt(polygon.area) / 10)
     multipoly = _quadrat_cut_geometry(polygon, quadrat_width)
-    utils.log(f"Accelerating r-tree with {len(multipoly.geoms)} quadrats")
+    msg = f"Accelerating r-tree with {len(multipoly.geoms)} quadrats"
+    utils.log(msg, level=lg.INFO)
 
     # loop through each chunk of the polygon to find intersecting geometries
     # first find approximate matches with spatial index, then precise matches
     # from those approximate ones
     geoms_in_poly = set()
     for poly in multipoly.geoms:
         poly_buff = poly.buffer(0)
         if poly_buff.is_valid and poly_buff.area > 0:
             possible_matches_iloc = rtree.intersection(poly_buff.bounds)
             possible_matches = geometries.iloc[list(possible_matches_iloc)]
             precise_matches = possible_matches[possible_matches.intersects(poly_buff)]
             geoms_in_poly.update(precise_matches.index)
 
-    utils.log(f"Identified {len(geoms_in_poly):,} geometries inside polygon")
+    msg = f"Identified {len(geoms_in_poly):,} geometries inside polygon"
+    utils.log(msg, level=lg.INFO)
     return geoms_in_poly
 
 
-def bbox_from_point(point, dist=1000, project_utm=False, return_crs=False):
+# dist present, project_utm missing/False, return_crs missing/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm missing/False, return_crs present/True
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    return_crs: Literal[True],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm missing/False, return_crs present/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    return_crs: Literal[False],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm present/True, return_crs missing/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[True],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm present/True, return_crs present/True
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[True],
+    return_crs: Literal[True],
+) -> tuple[tuple[float, float, float, float], Any]: ...
+
+
+# dist present, project_utm present/True, return_crs present/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[True],
+    return_crs: Literal[False],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm present/False, return_crs missing/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[False],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm present/False, return_crs present/True
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[False],
+    return_crs: Literal[True],
+) -> tuple[float, float, float, float]: ...
+
+
+# dist present, project_utm present/False, return_crs present/False
+@overload
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: Literal[False],
+    return_crs: Literal[False],
+) -> tuple[float, float, float, float]: ...
+
+
+def bbox_from_point(
+    point: tuple[float, float],
+    dist: float,
+    *,
+    project_utm: bool = False,
+    return_crs: bool = False,
+) -> tuple[float, float, float, float] | tuple[tuple[float, float, float, float], Any]:
     """
     Create a bounding box around a (lat, lon) point.
 
     Create a bounding box some distance (in meters) in each direction (north,
     south, east, and west) from the center point and optionally project it.
 
     Parameters
     ----------
-    point : tuple
-        the (lat, lon) center point to create the bounding box around
-    dist : int
-        bounding box distance in meters from the center point
-    project_utm : bool
-        if True, return bounding box as UTM-projected coordinates
-    return_crs : bool
-        if True, and project_utm=True, return the projected CRS too
+    point
+        The `(lat, lon)` center point to create the bounding box around.
+    dist
+        Bounding box distance in meters from the center point.
+    project_utm
+        If True, return bounding box as UTM-projected coordinates.
+    return_crs
+        If True, and `project_utm` is True, then return the projected CRS too.
 
     Returns
     -------
-    bbox or bbox, crs: tuple or tuple, crs
-        (north, south, east, west) or ((north, south, east, west), crs)
+    bbox or bbox, crs
+        `(north, south, east, west)` or `((north, south, east, west), crs)`.
     """
     EARTH_RADIUS_M = 6_371_009  # meters
     lat, lon = point
 
     delta_lat = (dist / EARTH_RADIUS_M) * (180 / np.pi)
     delta_lon = (dist / EARTH_RADIUS_M) * (180 / np.pi) / np.cos(lat * np.pi / 180)
     north = lat + delta_lat
@@ -422,47 +377,32 @@
     west = lon - delta_lon
 
     if project_utm:
         bbox_poly = bbox_to_poly(bbox=(north, south, east, west))
         bbox_proj, crs_proj = projection.project_geometry(bbox_poly)
         west, south, east, north = bbox_proj.bounds
 
-    utils.log(f"Created bbox {dist} m from {point}: {north},{south},{east},{west}")
+    msg = f"Created bbox {dist} m from {point}: {north},{south},{east},{west}"
+    utils.log(msg, level=lg.INFO)
 
     if project_utm and return_crs:
         return (north, south, east, west), crs_proj
 
     # otherwise
     return north, south, east, west
 
 
-def bbox_to_poly(north=None, south=None, east=None, west=None, bbox=None):
+def bbox_to_poly(bbox: tuple[float, float, float, float]) -> Polygon:
     """
-    Convert bounding box coordinates to shapely Polygon.
+    Convert bounding box coordinates to Shapely Polygon.
 
     Parameters
     ----------
-    north : float
-        deprecated, do not use
-    south : float
-        deprecated, do not use
-    east : float
-        deprecated, do not use
-    west : float
-        deprecated, do not use
-    bbox : tuple of floats
-        bounding box as (north, south, east, west)
+    bbox
+        Bounding box as `(north, south, east, west)`.
 
     Returns
     -------
-    shapely.geometry.Polygon
+    polygon
     """
-    if not (north is None and south is None and east is None and west is None):
-        msg = (
-            "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
-            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
-        )
-        warn(msg, FutureWarning, stacklevel=2)
-    else:
-        north, south, east, west = bbox
+    north, south, east, west = bbox
     return Polygon([(west, south), (east, south), (east, north), (west, north)])
```

### Comparing `osmnx-1.9.3/.gitignore` & `osmnx-2.0.0b0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .temp
 .pytest_cache
-tests/run_tests.bat
 *.vrt
 .DS_Store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `osmnx-1.9.3/LICENSE.txt` & `osmnx-2.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.3/README.md` & `osmnx-2.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.3/PKG-INFO` & `osmnx-2.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: osmnx
-Version: 1.9.3
+Version: 2.0.0b0
 Summary: Download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap
 Project-URL: Documentation, https://osmnx.readthedocs.io
 Project-URL: Code Repository, https://github.com/gboeing/osmnx
 Project-URL: Examples Gallery, https://github.com/gboeing/osmnx-examples
 Author-email: Geoff Boeing <boeing@usc.edu>
 Maintainer: OSMnx contributors
 License: MIT License
@@ -14,28 +14,27 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: geopandas>=0.12
 Requires-Dist: networkx>=2.5
-Requires-Dist: numpy>=1.20
+Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.1
 Requires-Dist: requests>=2.27
 Requires-Dist: shapely>=2.0
 Provides-Extra: entropy
 Requires-Dist: scipy>=1.5; extra == 'entropy'
 Provides-Extra: neighbors
 Requires-Dist: scikit-learn>=0.23; extra == 'neighbors'
```

