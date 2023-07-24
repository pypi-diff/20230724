# Comparing `tmp/WestJR-0.4.tar.gz` & `tmp/westjr-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WestJR-0.4.tar", last modified: Sun Apr  9 08:51:50 2023, max compression
+gzip compressed data, was "westjr-0.4.1.tar", max compression
```

## Comparing `WestJR-0.4.tar` & `westjr-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,15 @@
-drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.084756 WestJR-0.4/
--rw-r--r--   0 y-endo     (501) staff       (20)     1211 2023-04-09 08:51:21.000000 WestJR-0.4/LICENSE
--rw-r--r--   0 y-endo     (501) staff       (20)     3924 2023-04-09 08:51:50.084845 WestJR-0.4/PKG-INFO
--rw-r--r--   0 y-endo     (501) staff       (20)     3282 2023-04-09 08:51:21.000000 WestJR-0.4/README.md
-drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083112 WestJR-0.4/WestJR.egg-info/
--rw-r--r--   0 y-endo     (501) staff       (20)     3924 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/PKG-INFO
--rw-r--r--   0 y-endo     (501) staff       (20)      534 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/SOURCES.txt
--rw-r--r--   0 y-endo     (501) staff       (20)        1 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/dependency_links.txt
--rw-r--r--   0 y-endo     (501) staff       (20)      174 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/requires.txt
--rw-r--r--   0 y-endo     (501) staff       (20)        7 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/top_level.txt
--rw-r--r--   0 y-endo     (501) staff       (20)     1286 2023-04-09 08:51:50.085271 WestJR-0.4/setup.cfg
--rw-r--r--   0 y-endo     (501) staff       (20)       61 2023-04-09 08:51:21.000000 WestJR-0.4/setup.py
-drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083248 WestJR-0.4/tests/
--rw-r--r--   0 y-endo     (501) staff       (20)     2284 2023-04-09 08:51:21.000000 WestJR-0.4/tests/test_example.py
-drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083816 WestJR-0.4/westjr/
--rw-r--r--   0 y-endo     (501) staff       (20)       66 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/__init__.py
--rw-r--r--   0 y-endo     (501) staff       (20)     5905 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/api.py
--rw-r--r--   0 y-endo     (501) staff       (20)    26317 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/const.py
--rw-r--r--   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/py.typed
-drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.084648 WestJR-0.4/westjr/response_types/
--rw-r--r--   0 y-endo     (501) staff       (20)      620 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/__init__.py
--rw-r--r--   0 y-endo     (501) staff       (20)      381 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/area_maintenance.py
--rw-r--r--   0 y-endo     (501) staff       (20)     1003 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/area_master.py
--rw-r--r--   0 y-endo     (501) staff       (20)      895 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/stations.py
--rw-r--r--   0 y-endo     (501) staff       (20)      580 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_info.py
--rw-r--r--   0 y-endo     (501) staff       (20)      364 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_monitor_info.py
--rw-r--r--   0 y-endo     (501) staff       (20)      441 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_pos.py
+-rw-r--r--   0        0        0     1235 2023-02-12 02:27:29.030085 westjr-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2131 2023-07-24 15:14:35.308625 westjr-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3780 2023-07-24 15:08:52.676078 westjr-0.4.1/README.md
+-rw-r--r--   0        0        0       70 2023-07-24 15:00:43.045279 westjr-0.4.1/westjr/__init__.py
+-rw-r--r--   0        0        0     6175 2023-07-24 15:08:52.677077 westjr-0.4.1/westjr/api.py
+-rw-r--r--   0        0        0    27348 2023-07-24 15:08:52.677077 westjr-0.4.1/westjr/const.py
+-rw-r--r--   0        0        0        0 2023-02-12 02:27:29.033077 westjr-0.4.1/westjr/py.typed
+-rw-r--r--   0        0        0      645 2023-07-24 15:00:43.046279 westjr-0.4.1/westjr/response_types/__init__.py
+-rw-r--r--   0        0        0      403 2023-07-24 15:00:43.046279 westjr-0.4.1/westjr/response_types/area_maintenance.py
+-rw-r--r--   0        0        0     1065 2023-07-24 15:08:52.677077 westjr-0.4.1/westjr/response_types/area_master.py
+-rw-r--r--   0        0        0      952 2023-07-24 15:08:52.678581 westjr-0.4.1/westjr/response_types/stations.py
+-rw-r--r--   0        0        0      641 2023-07-24 15:08:52.678581 westjr-0.4.1/westjr/response_types/train_info.py
+-rw-r--r--   0        0        0      386 2023-07-24 15:00:43.046279 westjr-0.4.1/westjr/response_types/train_monitor_info.py
+-rw-r--r--   0        0        0      470 2023-07-24 15:00:43.046279 westjr-0.4.1/westjr/response_types/train_pos.py
+-rw-r--r--   0        0        0     4743 1970-01-01 00:00:00.000000 westjr-0.4.1/PKG-INFO
```

### Comparing `WestJR-0.4/LICENSE` & `westjr-0.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org>
```

### Comparing `WestJR-0.4/PKG-INFO` & `westjr-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
-Name: WestJR
-Version: 0.4
+Name: westjr
+Version: 0.4.1
 Summary: Handling of train operation information of JR West, a railroad company in Japan
 Home-page: https://github.com/unyacat/westjr
-Author: unyacat
-Author-email: admin@unyacat.net
 License: Unlicense
 Keywords: westjr
-Classifier: License :: OSI Approved :: MIT License
+Author: unyacat
+Author-email: admin@unyacat.net
+Requires-Python: >=3.7,<4
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: types-requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
+Project-URL: Repository, https://github.com/unyacat/westjr
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # WestJR
 
 ![Python Versions](https://img.shields.io/pypi/pyversions/WestJR.svg)
 ![PyPI](https://badge.fury.io/py/WestJR.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/unyacat/westjr/master.svg)](https://results.pre-commit.ci/latest/github/unyacat/westjr/master)
 ![GitHubActions](https://github.com/unyacat/westjr/workflows/Test/badge.svg)
@@ -143,7 +151,11 @@
 print(prev)
 # 塚本
 ```
 
 ## Contribution
 
 * develop ブランチにお願いします
+* インストールしていなければ [poetry](https://python-poetry.org/docs/master/) をインストールしてください
+* 初回は `poetry install && poetry run pre-commit install` を実行することで `poetry` と `pre-commit` のセットアップが行えます
+* `poetry shell` を実行すると仮想環境で開発することができます
+
```

### Comparing `WestJR-0.4/README.md` & `westjr-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,130 +1,133 @@
-# WestJR
-
-![Python Versions](https://img.shields.io/pypi/pyversions/WestJR.svg)
-![PyPI](https://badge.fury.io/py/WestJR.svg)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/unyacat/westjr/master.svg)](https://results.pre-commit.ci/latest/github/unyacat/westjr/master)
-![GitHubActions](https://github.com/unyacat/westjr/workflows/Test/badge.svg)
-
-JR西日本列車走行位置 非公式API Pythonライブラリ
-
-* 列車走行位置取得 (`/api/v3/{LINE}.json`)
-* メンテナンス予定取得 (`/api/v3/area_{AREA}_maintenance.json`)
-* 路線名取得 (`/api/v3/area_{AREA}_master.json`)
-* 駅一覧取得 (`/api/v3/{LINE}_st.json`)
-* 運行情報取得 (`/api/v3/area_{AREA}_trafficinfo.json`)
-* 列車環境取得 (`/api/v3/trainmonitorinfo.json`)
-* 列車走行位置駅名，列車停車種別の変換
-
-## Notice
-
-* 動作を完全には確認していません．
-
-## Installation
-
-```bash
-pip install WestJR
-```
-
-## Usage
-
-[Wiki](https://github.com/unyacat/westjr/wiki) に情報があります．
-
-```python
-import westjr
-jr = westjr.WestJR()
-
-# あらかじめ area や line をセットする
-jr = westjr.WestJR(line="kobesanyo", area="kinki")
-```
-
-### Example
-
-#### 列車走行位置取得
-
-```python
-print(jr.get_trains())
-# TrainPos(update='2023-03-21T16:54:54.612Z', trains=[TrainsItem(no='502C', ...
-```
-
-#### メンテナンス予定取得
-
-```python
-print(jr.get_maintenance())
-# 平常時:
-# AreaMaintenance(status=0, notification=Notification(groupId=0, text='', duration=''), ...
-# 異常時:
-# AreaMaintenance(status=1, notification=Notification(groupId=2023012802, text='1月24日から1月31日を, ...
-```
-
-#### 路線一覧取得
-
-```python
-print(jr.get_lines())
-# AreaMaster(lines={'ako': Line(name='赤穂線', range='相生〜播州赤穂', relatelines=None, st='...
-```
-
-#### 駅一覧取得
-
-```python
-print(jr.get_stations())
-# Stations(stations=[StationsItem(info=Info(name='新大阪', code='0415', stopTrains=[1, 2, 5], typeNotice=None, ...
-```
-
-#### 運行情報取得
-
-```Python
-print(jr.get_traffic_info())
-# 平常時:
-# TrainInfo(lines={}, express={})
-# 異常時:
-# TrainInfo(lines={'bantan': Info_LineItem(...)}, express={'bantan': Info_ExpressItem(...)})
-```
-
-#### エリア名一覧表示
-
-```python
-print(jr.areas)
-# ['hokuriku', 'kinki', 'okayama', 'hiroshima', 'sanin']
-```
-
-#### 路線名一覧表示
-
-```python
-print(jr.lines)
-# ['hokuriku', 'kobesanyo', 'hokurikubiwako', 'kyoto', 'ako', 'kosei', 'kusatsu', 'nara', 'sagano', 'sanin1', 'sanin2', 'osakahigashi', 'takarazuka']
-```
-
-#### 列車環境取得
-
-```python
-print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].congestion)
-# 26(%)
-print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].temp)
-# 23(°C)
-```
-
-#### 駅に停車する種別を id から名称に変換する
-
-```python
-station = jr.get_stations(line="kyoto").stations[0]
-
-print(station.info.name)
-# 山科
-
-print(jr.convert_stopTrains(station.info.stopTrains))
-# ['新快速', '快速', '特急']
-```
-
-#### 列車走行位置の場所を前駅と次駅の名前に変換する
-
-```python
-train = jr.get_trains(line="kobesanyo").trains
-tr = train[0]
-prev, next = jr.convert_pos(train=tr)
-print(prev)
-# 塚本
-```
-
-## Contribution
-
-* develop ブランチにお願いします
+# WestJR
+
+![Python Versions](https://img.shields.io/pypi/pyversions/WestJR.svg)
+![PyPI](https://badge.fury.io/py/WestJR.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/unyacat/westjr/master.svg)](https://results.pre-commit.ci/latest/github/unyacat/westjr/master)
+![GitHubActions](https://github.com/unyacat/westjr/workflows/Test/badge.svg)
+
+JR西日本列車走行位置 非公式API Pythonライブラリ
+
+* 列車走行位置取得 (`/api/v3/{LINE}.json`)
+* メンテナンス予定取得 (`/api/v3/area_{AREA}_maintenance.json`)
+* 路線名取得 (`/api/v3/area_{AREA}_master.json`)
+* 駅一覧取得 (`/api/v3/{LINE}_st.json`)
+* 運行情報取得 (`/api/v3/area_{AREA}_trafficinfo.json`)
+* 列車環境取得 (`/api/v3/trainmonitorinfo.json`)
+* 列車走行位置駅名，列車停車種別の変換
+
+## Notice
+
+* 動作を完全には確認していません．
+
+## Installation
+
+```bash
+pip install WestJR
+```
+
+## Usage
+
+[Wiki](https://github.com/unyacat/westjr/wiki) に情報があります．
+
+```python
+import westjr
+jr = westjr.WestJR()
+
+# あらかじめ area や line をセットする
+jr = westjr.WestJR(line="kobesanyo", area="kinki")
+```
+
+### Example
+
+#### 列車走行位置取得
+
+```python
+print(jr.get_trains())
+# TrainPos(update='2023-03-21T16:54:54.612Z', trains=[TrainsItem(no='502C', ...
+```
+
+#### メンテナンス予定取得
+
+```python
+print(jr.get_maintenance())
+# 平常時:
+# AreaMaintenance(status=0, notification=Notification(groupId=0, text='', duration=''), ...
+# 異常時:
+# AreaMaintenance(status=1, notification=Notification(groupId=2023012802, text='1月24日から1月31日を, ...
+```
+
+#### 路線一覧取得
+
+```python
+print(jr.get_lines())
+# AreaMaster(lines={'ako': Line(name='赤穂線', range='相生〜播州赤穂', relatelines=None, st='...
+```
+
+#### 駅一覧取得
+
+```python
+print(jr.get_stations())
+# Stations(stations=[StationsItem(info=Info(name='新大阪', code='0415', stopTrains=[1, 2, 5], typeNotice=None, ...
+```
+
+#### 運行情報取得
+
+```Python
+print(jr.get_traffic_info())
+# 平常時:
+# TrainInfo(lines={}, express={})
+# 異常時:
+# TrainInfo(lines={'bantan': Info_LineItem(...)}, express={'bantan': Info_ExpressItem(...)})
+```
+
+#### エリア名一覧表示
+
+```python
+print(jr.areas)
+# ['hokuriku', 'kinki', 'okayama', 'hiroshima', 'sanin']
+```
+
+#### 路線名一覧表示
+
+```python
+print(jr.lines)
+# ['hokuriku', 'kobesanyo', 'hokurikubiwako', 'kyoto', 'ako', 'kosei', 'kusatsu', 'nara', 'sagano', 'sanin1', 'sanin2', 'osakahigashi', 'takarazuka']
+```
+
+#### 列車環境取得
+
+```python
+print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].congestion)
+# 26(%)
+print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].temp)
+# 23(°C)
+```
+
+#### 駅に停車する種別を id から名称に変換する
+
+```python
+station = jr.get_stations(line="kyoto").stations[0]
+
+print(station.info.name)
+# 山科
+
+print(jr.convert_stopTrains(station.info.stopTrains))
+# ['新快速', '快速', '特急']
+```
+
+#### 列車走行位置の場所を前駅と次駅の名前に変換する
+
+```python
+train = jr.get_trains(line="kobesanyo").trains
+tr = train[0]
+prev, next = jr.convert_pos(train=tr)
+print(prev)
+# 塚本
+```
+
+## Contribution
+
+* develop ブランチにお願いします
+* インストールしていなければ [poetry](https://python-poetry.org/docs/master/) をインストールしてください
+* 初回は `poetry install && poetry run pre-commit install` を実行することで `poetry` と `pre-commit` のセットアップが行えます
+* `poetry shell` を実行すると仮想環境で開発することができます
```

### Comparing `WestJR-0.4/westjr/api.py` & `westjr-0.4.1/westjr/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,174 @@
-from __future__ import annotations
-
-from typing import TypeVar
-
-import requests
-from pydantic import BaseModel
-
-from .const import AREAS, LINES, STATIONS, STOP_TRAINS
-from .response_types import (
-    AreaMaintenance,
-    AreaMaster,
-    Stations,
-    TrainInfo,
-    TrainMonitorInfo,
-    TrainPos,
-    TrainsItem,
-)
-
-_TModel = TypeVar("_TModel", bound=BaseModel)
-
-
-class WestJR:
-    def __init__(self, line: str | None = None, area: str | None = None) -> None:
-        self.uri_suffix = "https://www.train-guide.westjr.co.jp/api/v3/"
-        self.line = line
-        self.area = area
-        self.areas = AREAS
-        self.lines = LINES
-
-    def _request(
-        self,
-        *,
-        endpoint: str,
-        model: type[_TModel],
-        method: str = "GET",
-    ) -> _TModel:
-        uri = f"{self.uri_suffix}{endpoint}.json"
-
-        if method == "GET":
-            res = requests.get(url=uri)
-            try:
-                res.raise_for_status()
-            except requests.RequestException as e:
-                print(e)
-                raise e
-            return model.parse_obj(res.json())
-        else:
-            raise NotImplementedError(method)
-
-    def get_lines(self, area: str | None = None) -> AreaMaster:
-        """
-        広域エリアに属する路線一覧を取得して返す．
-        該当API例: https://www.train-guide.westjr.co.jp/api/v3/area_kinki_master.json
-        :param area: [必須] 広域エリア名(ex. kinki)
-        :return: dict
-        """
-        _area = area if area else self.area
-        if _area is None:
-            raise ValueError("Need to set the area name.")
-        endpoint = f"area_{_area}_master"
-
-        return self._request(endpoint=endpoint, model=AreaMaster)
-
-    def get_stations(self, line: str | None = None) -> Stations:
-        """
-        路線に所属している駅名一覧を取得して返す．
-        :param line: [必須] 路線名(ex. kobesanyo)
-        :return: dict
-        """
-        _line = line if line is not None else self.line
-        if _line is None:
-            raise ValueError("Need to set the line name.")
-        endpoint = f"{_line}_st"
-
-        return self._request(endpoint=endpoint, model=Stations)
-
-    def get_trains(self, line: str | None = None) -> TrainPos:
-        """
-        列車走行位置を取得して返す．
-        :param line: [必須] 路線名(ex. kobesanyo)
-        :return: dict
-        """
-        _line = line if line is not None else self.line
-        if _line is None:
-            raise ValueError("Need to set the line name.")
-
-        return self._request(endpoint=_line, model=TrainPos)
-
-    def get_maintenance(self, area: str | None = None) -> AreaMaintenance:
-        """
-        メンテナンス予定を取得して返す．大雪などで運休が予定されているときのみ情報が載る．
-        :param area: [必須] 広域エリア名(ex. kinki)
-        :return: dict
-        """
-        _area = area if area else self.area
-        if _area is None:
-            raise ValueError("Need to set the area name.")
-        endpoint = f"area_{_area}_maintenance"
-
-        return self._request(endpoint=endpoint, model=AreaMaintenance)
-
-    def get_traffic_info(self, area: str | None = None) -> TrainInfo:
-        """
-        路線の交通情報を取得して返す．問題が発生しているときのみ情報が載る．
-        :param area: [必須] 広域エリア名(ex. kinki)
-        :return: dict
-        """
-        _area = area if area else self.area
-        if _area is None:
-            raise ValueError("Need to set the area name.")
-        endpoint = f"area_{_area}_trafficinfo"
-
-        return self._request(endpoint=endpoint, model=TrainInfo)
-
-    def get_train_monitor_info(self) -> TrainMonitorInfo:
-        """
-        列車の環境を取得して返す．
-        :return: dict
-        """
-        endpoint = "trainmonitorinfo"
-
-        return self._request(endpoint=endpoint, model=TrainMonitorInfo)
-
-    def convert_stopTrains(self, stopTrains: list[int] | None = None) -> list[str]:
-        """
-        駅一覧にある停車種別ID(int, 0~10)の配列を実際の停車種別名の配列に変換する．
-        :param stopTrains: list[int]
-        :return: list[str]
-        """
-        if stopTrains is not None:
-            return [STOP_TRAINS[i] for i in stopTrains]
-        else:
-            return []
-
-    def convert_pos(
-        self, train: TrainsItem, line: str | None = None
-    ) -> tuple[str | None, str | None]:
-        """
-        ID_ID を (前駅名称, 次駅名称) に変換する．
-        停車中の場合 prev_st_name に駅名が入り，next_st_name は None となる．
-        :param train: 列車オブジェクト
-        :param line: 路線ID
-        :return: (前駅名称, 次駅名称)
-        """
-        prev_st_id, next_st_id, *_ = train.pos.split("_")
-
-        prev_st_name, next_st_name = None, None
-
-        _line = line if line is not None else self.line
-        if _line is None:
-            raise ValueError("Need to set the line name.")
-        if _line not in STATIONS:
-            raise ValueError(f"Invalid line name: {_line}")
-
-        _station = STATIONS[_line]
-        _direction = train.direction
-        if _direction == 0:  # 上り
-            if next_st_id == "####":
-                prev_st_name = _station.get(prev_st_id)
-                next_st_name = None
-            else:
-                prev_st_name = _station.get(next_st_id)
-                next_st_name = _station.get(prev_st_id)
-
-        elif _direction == 1:  # 下り
-            prev_st_name = _station.get(prev_st_id)
-            if next_st_id == "####":
-                next_st_name = None
-            else:
-                next_st_name = _station.get(next_st_id)
-        else:
-            raise ValueError(f"invalid direction: {_direction}")
-        return prev_st_name, next_st_name
+from __future__ import annotations
+
+from typing import TypeVar
+
+import requests
+from pydantic import BaseModel
+
+from .const import AREAS, LINES, STATIONS, STOP_TRAINS
+from .response_types import (
+    AreaMaintenance,
+    AreaMaster,
+    Stations,
+    TrainInfo,
+    TrainMonitorInfo,
+    TrainPos,
+    TrainsItem,
+)
+
+_TModel = TypeVar("_TModel", bound=BaseModel)
+
+
+class WestJR:
+    def __init__(self, line: str | None = None, area: str | None = None) -> None:
+        self.uri_suffix = "https://www.train-guide.westjr.co.jp/api/v3/"
+        self.line = line
+        self.area = area
+        self.areas = AREAS
+        self.lines = LINES
+
+    def _request(
+        self,
+        *,
+        endpoint: str,
+        model: type[_TModel],
+        method: str = "GET",
+    ) -> _TModel:
+        uri = f"{self.uri_suffix}{endpoint}.json"
+
+        if method == "GET":
+            res = requests.get(url=uri)  # noqa: S113
+            try:
+                res.raise_for_status()
+            except requests.RequestException as e:
+                print(e)  # noqa: T201
+                raise
+            return model.model_validate(res.json())
+        raise NotImplementedError(method)
+
+    def get_lines(self, area: str | None = None) -> AreaMaster:
+        """
+        広域エリアに属する路線一覧を取得して返す．
+        該当API例: https://www.train-guide.westjr.co.jp/api/v3/area_kinki_master.json
+        :param area: [必須] 広域エリア名(ex. kinki)
+        :return: dict
+        """
+        _area = area if area else self.area
+        if _area is None:
+            msg = "Need to set the area name."
+            raise ValueError(msg)
+        endpoint = f"area_{_area}_master"
+
+        return self._request(endpoint=endpoint, model=AreaMaster)
+
+    def get_stations(self, line: str | None = None) -> Stations:
+        """
+        路線に所属している駅名一覧を取得して返す．
+        :param line: [必須] 路線名(ex. kobesanyo)
+        :return: dict
+        """
+        _line = line if line is not None else self.line
+        if _line is None:
+            msg = "Need to set the line name."
+            raise ValueError(msg)
+        endpoint = f"{_line}_st"
+
+        return self._request(endpoint=endpoint, model=Stations)
+
+    def get_trains(self, line: str | None = None) -> TrainPos:
+        """
+        列車走行位置を取得して返す．
+        :param line: [必須] 路線名(ex. kobesanyo)
+        :return: dict
+        """
+        _line = line if line is not None else self.line
+        if _line is None:
+            msg = "Need to set the line name."
+            raise ValueError(msg)
+
+        return self._request(endpoint=_line, model=TrainPos)
+
+    def get_maintenance(self, area: str | None = None) -> AreaMaintenance:
+        """
+        メンテナンス予定を取得して返す．大雪などで運休が予定されているときのみ情報が載る．
+        :param area: [必須] 広域エリア名(ex. kinki)
+        :return: dict
+        """
+        _area = area if area else self.area
+        if _area is None:
+            msg = "Need to set the area name."
+            raise ValueError(msg)
+        endpoint = f"area_{_area}_maintenance"
+
+        return self._request(endpoint=endpoint, model=AreaMaintenance)
+
+    def get_traffic_info(self, area: str | None = None) -> TrainInfo:
+        """
+        路線の交通情報を取得して返す．問題が発生しているときのみ情報が載る．
+        :param area: [必須] 広域エリア名(ex. kinki)
+        :return: dict
+        """
+        _area = area if area else self.area
+        if _area is None:
+            msg = "Need to set the area name."
+            raise ValueError(msg)
+        endpoint = f"area_{_area}_trafficinfo"
+
+        return self._request(endpoint=endpoint, model=TrainInfo)
+
+    def get_train_monitor_info(self) -> TrainMonitorInfo:
+        """
+        列車の環境を取得して返す．
+        :return: dict
+        """
+        endpoint = "trainmonitorinfo"
+
+        return self._request(endpoint=endpoint, model=TrainMonitorInfo)
+
+    def convert_stopTrains(self, stopTrains: list[int] | None = None) -> list[str]:
+        """
+        駅一覧にある停車種別ID(int, 0~10)の配列を実際の停車種別名の配列に変換する．
+        :param stopTrains: list[int]
+        :return: list[str]
+        """
+        if stopTrains is not None:
+            return [STOP_TRAINS[i] for i in stopTrains]
+        return []
+
+    def convert_pos(self, train: TrainsItem, line: str | None = None) -> tuple[str | None, str | None]:
+        """
+        ID_ID を (前駅名称, 次駅名称) に変換する．
+        停車中の場合 prev_st_name に駅名が入り，next_st_name は None となる．
+        :param train: 列車オブジェクト
+        :param line: 路線ID
+        :return: (前駅名称, 次駅名称)
+        """
+        prev_st_id, next_st_id, *_ = train.pos.split("_")
+
+        prev_st_name, next_st_name = None, None
+
+        _line = line if line is not None else self.line
+        if _line is None:
+            msg = "Need to set the line name."
+            raise ValueError(msg)
+        if _line not in STATIONS:
+            msg = f"Invalid line name: {_line}"
+            raise ValueError(msg)
+
+        _station = STATIONS[_line]
+        _direction = train.direction
+        if _direction == 0:  # 上り
+            if next_st_id == "####":
+                prev_st_name = _station.get(prev_st_id)
+                next_st_name = None
+            else:
+                prev_st_name = _station.get(next_st_id)
+                next_st_name = _station.get(prev_st_id)
+
+        elif _direction == 1:  # 下り
+            prev_st_name = _station.get(prev_st_id)
+            next_st_name = None if next_st_id == "####" else _station.get(next_st_id)
+        else:
+            msg = f"invalid direction: {_direction}"
+            raise ValueError(msg)
+        return prev_st_name, next_st_name
```

### Comparing `WestJR-0.4/westjr/response_types/__init__.py` & `westjr-0.4.1/westjr/response_types/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from __future__ import annotations
-
-from . import area_maintenance, area_master, stations, train_info, train_pos
-from .area_maintenance import AreaMaintenance
-from .area_master import AreaMaster
-from .stations import Stations
-from .train_info import TrainInfo
-from .train_monitor_info import TrainMonitorInfo
-from .train_pos import TrainPos, TrainsItem
-
-__all__ = [
-    "area_maintenance",
-    "area_master",
-    "stations",
-    "train_info",
-    "train_pos",
-    "train_monitor_info",
-    "AreaMaintenance",
-    "AreaMaster",
-    "Stations",
-    "TrainInfo",
-    "TrainPos",
-    "TrainsItem",
-    "TrainMonitorInfo",
-]
+from __future__ import annotations
+
+from . import area_maintenance, area_master, stations, train_info, train_pos
+from .area_maintenance import AreaMaintenance
+from .area_master import AreaMaster
+from .stations import Stations
+from .train_info import TrainInfo
+from .train_monitor_info import TrainMonitorInfo
+from .train_pos import TrainPos, TrainsItem
+
+__all__ = [
+    "area_maintenance",
+    "area_master",
+    "stations",
+    "train_info",
+    "train_pos",
+    "train_monitor_info",
+    "AreaMaintenance",
+    "AreaMaster",
+    "Stations",
+    "TrainInfo",
+    "TrainPos",
+    "TrainsItem",
+    "TrainMonitorInfo",
+]
```

