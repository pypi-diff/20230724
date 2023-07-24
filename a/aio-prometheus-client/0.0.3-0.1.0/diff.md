# Comparing `tmp/aio_prometheus_client-0.0.3-py3-none-any.whl.zip` & `tmp/aio_prometheus_client-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 3664 bytes, number of entries: 8
+Zip file size: 4117 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       77 b- defN 22-Nov-02 09:07 aio_prometheus_client/__init__.py
--rw-rw-r--  2.0 unx     2625 b- defN 22-Nov-18 03:49 aio_prometheus_client/client.py
--rw-rw-r--  2.0 unx      462 b- defN 22-Nov-02 10:36 aio_prometheus_client/errors.py
--rw-rw-r--  2.0 unx     1671 b- defN 22-Nov-18 03:49 aio_prometheus_client/model.py
--rw-rw-r--  2.0 unx      666 b- defN 22-Nov-18 03:50 aio_prometheus_client-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Nov-18 03:50 aio_prometheus_client-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       22 b- defN 22-Nov-18 03:50 aio_prometheus_client-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      703 b- defN 22-Nov-18 03:50 aio_prometheus_client-0.0.3.dist-info/RECORD
-8 files, 6318 bytes uncompressed, 2416 bytes compressed:  61.8%
+-rw-rw-r--  2.0 unx     3215 b- defN 23-Jul-24 02:47 aio_prometheus_client/client.py
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jul-24 02:47 aio_prometheus_client/errors.py
+-rw-rw-r--  2.0 unx     1863 b- defN 23-Jul-24 02:47 aio_prometheus_client/model.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-24 02:47 aio_prometheus_client/py.typed
+-rw-rw-r--  2.0 unx      666 b- defN 23-Jul-24 02:50 aio_prometheus_client-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 02:50 aio_prometheus_client-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       22 b- defN 23-Jul-24 02:50 aio_prometheus_client-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      787 b- defN 23-Jul-24 02:50 aio_prometheus_client-0.1.0.dist-info/RECORD
+9 files, 7212 bytes uncompressed, 2733 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: aio_prometheus_client/errors.py
 Comment: 
 
 Filename: aio_prometheus_client/model.py
 Comment: 
 
-Filename: aio_prometheus_client-0.0.3.dist-info/METADATA
+Filename: aio_prometheus_client/py.typed
 Comment: 
 
-Filename: aio_prometheus_client-0.0.3.dist-info/WHEEL
+Filename: aio_prometheus_client-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: aio_prometheus_client-0.0.3.dist-info/top_level.txt
+Filename: aio_prometheus_client-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: aio_prometheus_client-0.0.3.dist-info/RECORD
+Filename: aio_prometheus_client-0.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: aio_prometheus_client-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aio_prometheus_client/client.py

```diff
@@ -1,25 +1,33 @@
 from time import time as get_current_timestamp
 from urllib.parse import urljoin
+from typing import Optional, Any, Union
 
 import httpx
 
 from . import errors
-from .model import parse_data, InstantVector, Scalar
+from .model import parse_data, InstantVector, Scalar, RangeVector
 
 DEFAULT_USER_AGENT = 'Python Aio Prometheus Client'
 TIMEOUT = 10 * 60
 
 
 class PrometheusClient:
-    def __init__(self, base_url, user_agent=DEFAULT_USER_AGENT):
+    base_url: str
+    user_agent: str
+
+    def __init__(self, base_url: str, user_agent: str = DEFAULT_USER_AGENT):
         self.base_url = base_url
         self.user_agent = user_agent
 
-    async def _request(self, path, params=None):
+    async def _request(
+        self,
+        path: str,
+        params: Optional[dict[str, Union[str, int, float]]] = None
+    ) -> dict[str, Any]:
         async with httpx.AsyncClient() as client:
             try:
                 r = await client.get(
                     urljoin(self.base_url, path),
                     params=params,
                     headers={'User-Agent': self.user_agent},
                     timeout=TIMEOUT,
@@ -35,55 +43,67 @@
             data = r.json()
 
         if data['status'] != 'success':
             raise ValueError('invalid data: %s' % data)
 
         return data['data']
 
-    async def query(self, metric, time=0):
+    async def query(
+        self, metric: str, time: float = 0
+    ) -> Union[Scalar, InstantVector]:
         if not time:
             time = get_current_timestamp()
 
-        data = await self._request(
+        data: dict[str, Any] = await self._request(
             path='api/v1/query',
             params={
                 'query': metric,
                 'time': str(time)
             }
         )
 
         return parse_data(data)
 
-    async def query_value(self, metric):
+    async def query_value(self, metric: str) -> float:
         data = await self.query(metric)
         if isinstance(data, InstantVector):
             series_count = len(data.series)
             if series_count != 1:
                 raise ValueError('series count incorrect: %d' % series_count)
 
             return data.series[0].value.value
         elif isinstance(data, Scalar):
             return data.value
         else:
             raise TypeError('unknown data type: %s' % type(data))
 
-    async def query_range(self, metric, start, end, step=None, step_count=60):
+    async def query_range(
+        self, metric: str, start: float, end: float,
+        step: Optional[float] = None, step_count: int = 60
+    ) -> RangeVector:
         if step is None:
             if start >= end:
                 raise ValueError('end must be greater than start')
 
             step = (end - start) / step_count
             if step < 1:
                 step = 1
             else:
                 step = int(step)
 
-        data = await self._request(
+        data: dict[str, Any] = await self._request(
             path='api/v1/query_range',
             params={
                 'query': metric,
                 'start': start,
                 'end': end,
                 'step': step,
             }
         )
-        return parse_data(data)
+
+        result_type = data['resultType']
+        result = data['result']
+
+        if result_type != 'matrix':
+            raise ValueError('unexpected result type: %s' % result_type)
+
+        return RangeVector.from_data(result)
```

## aio_prometheus_client/errors.py

```diff
@@ -1,19 +1,19 @@
 class PrometheusErrorBase(Exception):
     pass
 
 
 class PrometheusMeticError(PrometheusErrorBase):
-    def __init__(self, http_status, data):
+    def __init__(self, http_status: int, data: dict[str, str]):
         assert data['status'] == 'error'
 
         self.http_status = http_status
         self.data = data
 
-    def __str__(self):
+    def __str__(self) -> str:
         return '%d %s: %s' % (
             self.http_status,
             self.data['errorType'], self.data['error']
         )
 
 
 class PrometheusConnectionError(PrometheusErrorBase):
```

## aio_prometheus_client/model.py

```diff
@@ -1,86 +1,86 @@
 from dataclasses import dataclass
-from typing import List
+from typing import Any, Union
 
 
 @dataclass
 class Scalar:
     timestamp: float
     value: float
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data: tuple[float, float]) -> 'Scalar':
         return cls(
             timestamp=data[0],
             value=float(data[1])
         )
 
 
 @dataclass
 class InstantSeries:
-    metric: dict
+    metric: dict[str, str]
     value: Scalar
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data: dict[str, Any]) -> 'InstantSeries':
         return cls(
             metric=data['metric'],
             value=Scalar.from_data(data['value'])
         )
 
 
 @dataclass
 class InstantVector:
-    series: List[InstantSeries]
+    series: list[InstantSeries]
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data: list[dict[str, Any]]) -> 'InstantVector':
         return cls(
             series=[
                 InstantSeries.from_data(i)
                 for i in data
             ]
         )
 
 
 @dataclass
 class RangeSeries:
-    metric: dict
-    values: List[Scalar]
+    metric: dict[str, str]
+    values: list[Scalar]
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data: dict[str, Any]) -> 'RangeSeries':
         return cls(
             metric=data['metric'],
             values=[
                 Scalar.from_data(i)
                 for i in data['values']
             ]
         )
 
 
 @dataclass
 class RangeVector:
-    series: List[RangeSeries]
+    series: list[RangeSeries]
 
     @classmethod
-    def from_data(cls, data):
+    def from_data(cls, data: list[dict[str, Any]]) -> 'RangeVector':
         return cls(
             series=[
                 RangeSeries.from_data(i)
                 for i in data
             ]
         )
 
 
-def parse_data(data):
+def parse_data(
+    data: dict[str, Any]
+) -> Union[Scalar, InstantVector]:
     result_type = data['resultType']
     result = data['result']
 
     if result_type == 'scalar':
         return Scalar.from_data(result)
     elif result_type == 'vector':
         return InstantVector.from_data(result)
-    elif result_type == 'matrix':
-        return RangeVector.from_data(result)
 
-    raise ValueError('no such type: %s' % result_type)
+    raise ValueError('unexpected result type: %s' % result_type)
```

## Comparing `aio_prometheus_client-0.0.3.dist-info/METADATA` & `aio_prometheus_client-0.1.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-prometheus-client
-Version: 0.0.3
+Version: 0.1.0
 Summary: Prometheus Http Client for Asyncio
 Home-page: https://github.com/lexdene/python-aio-prometheus-client
 License: LGPL
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

