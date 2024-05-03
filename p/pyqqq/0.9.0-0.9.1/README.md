# Comparing `tmp/pyqqq-0.9.0.tar.gz` & `tmp/pyqqq-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.9.0.tar", max compression
+gzip compressed data, was "pyqqq-0.9.1.tar", max compression
```

## Comparing `pyqqq-0.9.0.tar` & `pyqqq-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.0/README.md
--rw-r--r--   0        0        0      791 2024-05-02 09:31:16.839861 pyqqq-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.0/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.0/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.0/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    41866 2024-04-26 06:58:08.897413 pyqqq-0.9.0/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.0/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.0/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.0/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.0/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.9.0/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.0/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.0/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.0/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.0/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.0/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.0/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6717 2024-04-30 07:00:37.173273 pyqqq-0.9.0/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     9312 2024-05-02 09:25:25.974592 pyqqq-0.9.0/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.9.0/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.9.0/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.0/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.0/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.0/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.0/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.0/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.0/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.0/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.0/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.0/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.0/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.0/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.0/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.0/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.9.1/README.md
+-rw-r--r--   0        0        0      791 2024-05-03 09:01:00.763367 pyqqq-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1606 2024-04-30 07:51:35.706752 pyqqq-0.9.1/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.9.1/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.9.1/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    41866 2024-04-26 06:58:08.897413 pyqqq-0.9.1/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.9.1/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24448 2024-04-25 01:42:27.858549 pyqqq-0.9.1/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.9.1/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.9.1/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.9.1/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5356 2024-04-23 09:05:13.260008 pyqqq-0.9.1/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.9.1/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.9.1/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.9.1/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.9.1/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.9.1/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6245 2024-05-03 08:53:09.103466 pyqqq-0.9.1/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     9628 2024-05-03 08:51:32.698077 pyqqq-0.9.1/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1521 2024-05-03 08:51:15.982807 pyqqq-0.9.1/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4136 2024-05-03 08:53:53.080239 pyqqq-0.9.1/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.9.1/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.9.1/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.9.1/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.9.1/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-03 08:48:33.699191 pyqqq-0.9.1/pyqqq/utils/api_client.py
+-rw-r--r--   0        0        0      941 2024-04-30 08:35:54.600146 pyqqq-0.9.1/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3229 2024-04-30 08:36:37.055899 pyqqq-0.9.1/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.9.1/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3962 2024-04-23 09:09:34.322415 pyqqq-0.9.1/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     2641 2024-04-30 08:36:57.232261 pyqqq-0.9.1/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     2233 2024-04-30 07:41:29.806969 pyqqq-0.9.1/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.9.1/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.9.1/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     2065 2024-04-30 07:36:13.157361 pyqqq-0.9.1/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 pyqqq-0.9.1/PKG-INFO
```

### Comparing `pyqqq-0.9.0/README.md` & `pyqqq-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyproject.toml` & `pyqqq-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.9.0"
+version = "0.9.1"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.9.0/pyqqq/__init__.py` & `pyqqq-0.9.1/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.9.1/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.9.1/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.9.1/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.9.1/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.9.1/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.9.1/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.9.1/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.9.1/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.9.1/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/data/domestic.py` & `pyqqq-0.9.1/pyqqq/data/domestic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from pyqqq import get_api_key
-from pyqqq.utils.retry import retry
+from pyqqq.utils.api_client import raise_for_status, send_request
 from typing import Optional
 import datetime as dtm
 import pandas as pd
 import pyqqq.config as c
-import requests
 
 
 def get_alert_stocks(alert_type: str, date: dtm.date = None) -> Optional[pd.DataFrame]:
     """
     시장 경보 종목을 조회합니다.
 
     Args:
@@ -40,19 +38,19 @@
         219420  링크제니시스           9100     160         1.79  1720993       9120       9100  83.49
     """
     url = f"{c.PYQQQ_API_URL}/domestic-stock/alert-stocks/{alert_type}"
     params = {}
     if date:
         params["date"] = date
 
-    r = _send_request("GET", url, params=params)
+    r = send_request("GET", url, params=params)
     if r.status_code == 404:
         return None
     else:
-        _raise_for_status(r)
+        raise_for_status(r)
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
@@ -87,19 +85,19 @@
         36328K  티와이홀딩스우           4940     560       -10.18   26011       2024.03.22  감사범위제한으로인한 감사의견한정
     """
     url = f"{c.PYQQQ_API_URL}/domestic-stock/management-stocks"
     params = {}
     if date:
         params["date"] = date
 
-    r = _send_request("GET", url, params=params)
+    r = send_request("GET", url, params=params)
     if r.status_code == 404:
         return None
     else:
-        _raise_for_status(r)
+        raise_for_status(r)
 
         df = pd.DataFrame(r.json())
         if not df.empty:
             df.set_index("code", inplace=True)
         return df
 
 
@@ -155,40 +153,19 @@
 
 def _ticker_request(type: str, value: str):
     url = f"{c.PYQQQ_API_URL}/domestic-stock/tickers"
     params = {
         type: value
     }
 
-    r = _send_request("GET", url, params=params)
+    r = send_request("GET", url, params=params)
     if r.status_code == 404:
         return None
     else:
-        _raise_for_status(r)
+        raise_for_status(r)
 
     ticker_list = [r.json()] if type == 'code' else r.json()
     df = pd.DataFrame(ticker_list)
 
     if not df.empty:
         df.set_index("code", inplace=True)
     return df
-
-
-@retry(requests.HTTPError)
-def _send_request(method: str, url: str, **kwargs):
-    api_key = get_api_key()
-    if not api_key:
-        raise ValueError("API key is not set")
-
-    return requests.request(
-        method=method,
-        url=url,
-        headers={"Authorization": f"Bearer {api_key}"},
-        **kwargs,
-    )
-
-
-def _raise_for_status(r: requests.Response):
-    if r.status_code != 200:
-        print(r.text)
-
-    r.raise_for_status()
```

### Comparing `pyqqq-0.9.0/pyqqq/data/minutes.py` & `pyqqq-0.9.1/pyqqq/data/minutes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,71 @@
+from pyqqq.utils.api_client import send_request
 from pyqqq.utils.logger import get_logger
-import numpy as np
 import datetime as dtm
+import numpy as np
 import pandas as pd
-import pyqqq
 import pyqqq.config as c
 import pytz
-import requests
 
 logger = get_logger("minutes")
 
 
-def get_all_minute_data(
-    time: dtm.datetime, include_empty: bool = False
-) -> pd.DataFrame:
+def get_all_minute_data(time: dtm.datetime) -> pd.DataFrame:
     """
     모든 종목의 분봉 데이터를 반환합니다.
 
     Args:
         time (dtm.datetime): 조회할 시간
-        include_empty (bool): 거래가 없는 종목 데이터도 포함할지 여부 (기본값: False)
 
     Returns:
-        pd.DataFrame: 요청한 시간의 모든 종목의 분봉 데이터를 담은 DataFrame
+        pd.DataFrame: 모든 종목의 분봉 데이터가 포함된 pandas DataFrame.
+
+        DataFrame의 열은 다음과 같습니다:
 
-        - code (str): 종목 코드
-        - time (dtm.datetime): 시간
         - open (int): 시가
         - high (int): 고가
         - low (int): 저가
         - close (int): 종가
         - volume (int): 거래량
+        - sign (str): 대비부호 (1:상한가 2:상승, 3:보합 4:하한가, 5:하락)
+        - change (str): 전일 대비 가격 변화
+        - diff (float): 전일 대비 등락율
+        - chdegree (float): 체결강도
+        - mdvolume (int): 매도체결수량
+        - msvolume (int): 매수체결수량
+        - revolume (int): 순매수체결량
+        - mdchecnt (int): 매도체결건수
+        - mschecnt (int): 매수체결건수
+        - rechecnt (int): 순체결건수
+        - cvolume (int): 체결량
+        - mdchecnttm (int): 시간별매도체결건수
+        - mschecnttm (int): 시간별매수체결건수
+        - totofferrem (int): 매도잔량
+        - totbidrem (int): 매수잔량
+        - mdvolumetm (int): 시간별매도체결량
+        - msvolumetm (int): 시간별매수체결량
 
     Examples:
-        >>> df = get_all_minute_data(dtm.datetime(2024, 4, 2, 13, 0))
+        >>> df = get_all_minute_data(dtm.datetime(2024, 5, 2, 15, 30))
         >>> print(df)
-                                time    open    high     low   close  volume
-        code
-        310210 2024-04-02 13:00:00   33400   33450   33400   33450      11
-        000270 2024-04-02 13:00:00  104300  104500  104300  104500    7386
-        359090 2024-04-02 13:00:00    1449    1456    1447    1451   21871
-        003670 2024-04-02 13:00:00  288000  288000  287500  288000      91
-        028300 2024-04-02 13:00:00  100400  100500  100300  100500    4701
-        ...                    ...     ...     ...     ...     ...     ...
-        002600 2024-04-02 13:00:00  171900  171900  171900  171900       1
-        001725 2024-04-02 13:00:00   63400   63400   63400   63400      83
-        005745 2024-04-02 13:00:00    9770    9770    9770    9770     400
-        032685 2024-04-02 13:00:00   10090   10090   10090   10090      12
-        003075 2024-04-02 13:00:00   13790   13790   13790   13790       1
-        [1981 rows x 6 columns]
+                                    time   open   high    low  ...  totofferrem  totbidrem mdvolumetm  msvolumetm
+        code                                             ...
+        000020 2024-05-02 15:30:00   8700   8700   8700  ...         8404       4015         35           1
+        000040 2024-05-02 15:30:00   1058   1058   1058  ...        13597      24738         20           0
+        000050 2024-05-02 15:30:00   7620   7620   7620  ...         2534       2866          0           0
+        000070 2024-05-02 15:30:00  69400  69400  69400  ...          606        724          0           3
+        000075 2024-05-02 15:30:00  54900  54900  54900  ...          315        308          0           0
 
+        [5 rows x 23 columns]
     """
     tz = pytz.timezone("Asia/Seoul")
 
     url = f"{c.PYQQQ_API_URL}/domestic-stock/ohlcv/minutes/all/{time.date()}/{time.strftime('%H%M')}"
-    if include_empty:
-        url += "?includeEmpty=true"
 
-    r = requests.get(url, headers={"Authorization": f"Bearer {pyqqq.get_api_key()}"})
+    r = send_request("GET", url)
     if r.status_code != 200 and r.status_code != 201:
         logger.error(f"Failed to get minute data: {r.text}")
         return
 
     rows = r.json()
     for data in rows:
         time = data["time"].replace("Z", "+00:00")
@@ -164,17 +169,17 @@
             period.total_seconds() % 30 == 0
         ), "period must be a multiple of 30 seconds"
 
     tz = pytz.timezone("Asia/Seoul")
 
     url = f"{c.PYQQQ_API_URL}/domestic-stock/ohlcv/half-minutes/{date}"
 
-    r = requests.get(
+    r = send_request(
+        "GET",
         url,
-        headers={"Authorization": f"Bearer {pyqqq.get_api_key()}"},
         params={"codes": ",".join(codes) if codes else None},
     )
 
     if r.status_code != 200 and r.status_code != 201:
         logger.error(f"Failed to get day data: {r.text}")
         r.raise_for_status()
```

### Comparing `pyqqq-0.9.0/pyqqq/data/realtime.py` & `pyqqq-0.9.1/pyqqq/data/realtime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,10 @@
+from pyqqq.utils.api_client import raise_for_status, send_request
 from pyqqq.utils.logger import get_logger
-import datetime as dtm
-import pandas as pd
-import pyqqq
 import pyqqq.config as c
-import pytz
-import requests
 
 logger = get_logger("realtime")
 
 
 def get_all_last_trades():
     """
     모든 종목의 최근 체결 정보를 반환합니다.
@@ -39,16 +35,14 @@
             - bidho (int): 매수호가
             - status (str): 장정보
             - jnilvolume (int): 전일거래량
             - shcode (str): 종목코드
 
     """
 
-    r = requests.get(f"{c.PYQQQ_API_URL}/domestic-stock/trades")
-    r.raise_for_status()
+    r = send_request("GET", f"{c.PYQQQ_API_URL}/domestic-stock/trades")
+    raise_for_status(r)
 
     data = r.json()
     result = [data[k] for k in data.keys()]
 
     return result
-
-
```

### Comparing `pyqqq-0.9.0/pyqqq/data/ticks.py` & `pyqqq-0.9.1/pyqqq/data/ticks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from io import BytesIO
-from pyqqq import get_api_key
+from pyqqq.utils.api_client import send_request
 from pyqqq.utils.logger import get_logger
-from typing import Dict, List
 import datetime as dtm
 import pandas as pd
 import pyqqq.config as c
-import requests
 
 logger = get_logger("pyqqq.data.daily")
 
 def get_tick_data(date: dtm.date, asset_code: str) -> pd.DataFrame:
     """
     해당 일 체결 정보를 반환합니다
 
@@ -56,18 +54,17 @@
         2         2     3         1       352   37716    0.28        0        1     0      0    0  37715      +     13       0   69500  08:31:45      NaT     NaT     353    0.0      NaT           0         1     0      10
         3         2     3         2       352   37716    1.99        0        6     0      0    0  37715      +     14       0   69500  08:32:12      NaT     NaT     359    0.0      NaT           0         7     0      10
         4         2     3         3       352   37716   77.84        0      267     0      0    0  37715      +     24       0   69500  08:35:57      NaT     NaT     626    0.0      NaT           0       274     0      10
 
     """
 
     url = f"{c.PYQQQ_API_URL}/domestic-stock/daily/trades/{date}/{asset_code}"
-    r = requests.request(
+    r = send_request(
         "GET",
         url,
-        headers={"Authorization": f"Bearer {get_api_key()}"},
     )
     if r.status_code != 200 and r.status_code != 201:
         logger.error(f"Failed to get tick data: {r.status_code}")
         return None
 
     with BytesIO() as byte_stream:
         byte_stream.write(r.content)
```

### Comparing `pyqqq-0.9.0/pyqqq/datatypes.py` & `pyqqq-0.9.1/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/executors/hook.py` & `pyqqq-0.9.1/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/array.py` & `pyqqq-0.9.1/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/compute.py` & `pyqqq-0.9.1/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/display.py` & `pyqqq-0.9.1/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/kvstore.py` & `pyqqq-0.9.1/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/limiter.py` & `pyqqq-0.9.1/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/logger.py` & `pyqqq-0.9.1/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/market_schedule.py` & `pyqqq-0.9.1/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/mock_api.py` & `pyqqq-0.9.1/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/pyqqq/utils/retry.py` & `pyqqq-0.9.1/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.9.0/PKG-INFO` & `pyqqq-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

