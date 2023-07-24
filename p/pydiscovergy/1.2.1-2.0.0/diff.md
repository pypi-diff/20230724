# Comparing `tmp/pydiscovergy-1.2.1.tar.gz` & `tmp/pydiscovergy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiscovergy-1.2.1.tar", last modified: Mon Sep 19 12:35:59 2022, max compression
+gzip compressed data, was "pydiscovergy-2.0.0.tar", max compression
```

## Comparing `pydiscovergy-1.2.1.tar` & `pydiscovergy-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/pydiscovergy/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/pydiscovergy/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/authentication/basicauth.py
--rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/authentication/token.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     6088 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/discovergy.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/pydiscovergy/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/pydiscovergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-19 12:35:59.000000 pydiscovergy-1.2.1/pydiscovergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-19 12:35:59.000000 pydiscovergy-1.2.1/pydiscovergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 12:35:59.000000 pydiscovergy-1.2.1/pydiscovergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-19 12:35:59.000000 pydiscovergy-1.2.1/pydiscovergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-19 12:35:59.000000 pydiscovergy-1.2.1/pydiscovergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 12:35:59.744468 pydiscovergy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-19 12:35:50.000000 pydiscovergy-1.2.1/setup.py
+-rw-r--r--   0        0        0     1081 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/LICENSE
+-rw-r--r--   0        0        0      575 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/README.md
+-rw-r--r--   0        0        0      102 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/__init__.py
+-rw-r--r--   0        0        0      444 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/base.py
+-rw-r--r--   0        0        0      658 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/basicauth.py
+-rw-r--r--   0        0        0     7022 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/authentication/token.py
+-rw-r--r--   0        0        0      646 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/const.py
+-rw-r--r--   0        0        0     6278 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/discovergy.py
+-rw-r--r--   0        0        0      547 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/error.py
+-rw-r--r--   0        0        0     1041 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/marshmallow.py
+-rw-r--r--   0        0        0     1318 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pydiscovergy/models.py
+-rw-r--r--   0        0        0     1068 2023-07-24 20:17:59.912585 pydiscovergy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 pydiscovergy-2.0.0/PKG-INFO
```

### Comparing `pydiscovergy-1.2.1/LICENSE` & `pydiscovergy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiscovergy-1.2.1/README.md` & `pydiscovergy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pydiscovergy-1.2.1/pydiscovergy/authentication/token.py` & `pydiscovergy-2.0.0/pydiscovergy/authentication/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,83 @@
+"""Authentication module for token auth."""
 from __future__ import annotations
 
 import json
-from typing import Union
+from dataclasses import dataclass
+from urllib.parse import parse_qs
 
-import httpx
 from authlib.integrations.httpx_client import AsyncOAuth1Client
-from httpx import AsyncClient
+from httpx import AsyncClient, HTTPStatusError, RequestError
 
-from pydiscovergy.authentication import BaseAuthentication
-from pydiscovergy.const import API_CONSUMER_TOKEN, API_REQUEST_TOKEN, API_AUTHORIZATION, API_ACCESS_TOKEN, API_BASE
-from pydiscovergy.error import DiscovergyClientError, HTTPError, DiscovergyError, InvalidLogin, AccessTokenExpired, \
-    MissingToken
-from pydiscovergy.models import ConsumerToken, RequestToken, AccessToken
-from urllib.parse import parse_qs
+from ..const import (
+    API_ACCESS_TOKEN,
+    API_AUTHORIZATION,
+    API_CONSUMER_TOKEN,
+    API_REQUEST_TOKEN,
+    DEFAULT_APP_NAME,
+)
+from ..error import (
+    DiscovergyClientError,
+    DiscovergyError,
+    HTTPError,
+    InvalidLogin,
+    MissingToken,
+)
+from .base import BaseAuthentication
+
+
+@dataclass
+class ConsumerToken:
+    """Represents a consumer token pair."""
+
+    key: str
+    secret: str
+
+
+@dataclass
+class RequestToken:
+    """Represents a request token pair."""
+
+    token: str
+    token_secret: str
+
+
+@dataclass
+class AccessToken(RequestToken):
+    """Represents an access token pair."""
 
 
+@dataclass
 class TokenAuth(BaseAuthentication):
+    """Authentication class for token auth."""
 
-    def __init__(self,
-                 consumer_token: ConsumerToken = None,
-                 access_token: AccessToken = None):
-        """"""
-        self.consumer_token = consumer_token
-        self.access_token = access_token
+    consumer_token: ConsumerToken
+    access_token: AccessToken
+    app_name: str = DEFAULT_APP_NAME
+
+    async def get_client(
+        self, email: str, password: str, timeout: int, httpx_client: AsyncClient = None
+    ) -> AsyncOAuth1Client:
+        """Returns a AsyncOAuth1Client."""
 
-    async def get_client(self, email: str, password: str, httpx_client: AsyncClient = None) -> AsyncOAuth1Client:
         await self._do_exchange(email, password)
-        return AsyncOAuth1Client(**self._get_oauth_client_params())
+        return AsyncOAuth1Client(**self._get_oauth_client_params(), timeout=timeout)
 
     async def _do_exchange(
-            self, email: str, password: str
-    ) -> Union[tuple[AccessToken, ConsumerToken], tuple[AccessToken, None]]:
-        """Do the auth workflow"""
+        self, email: str, password: str
+    ) -> tuple[AccessToken, ConsumerToken] | tuple[AccessToken, None]:
+        """Do the auth workflow."""
 
-        # class already initialised with consumer and access token so we don't need to request one
+        # class already initialised with consumer and access token,
+        # so we don't need to request one
         if self.consumer_token is not None and self.access_token is not None:
             return self.access_token, self.consumer_token
 
-        # no access token and consumer token were supplied so we need to do the auth workflow
+        # no access token and consumer token were supplied,
+        # so we need to do the auth workflow
         # first fetch a consumer token
         await self._fetch_consumer_token()
 
         # then fetch a temporary request token
         temp_request_token = await self._fetch_request_token()
 
         # authorize the temporary request token with email and password
@@ -54,104 +90,105 @@
             request_token=temp_request_token.token,
             request_token_secret=temp_request_token.token_secret,
             verifier=verifier,
         )
         return self.access_token, self.consumer_token
 
     def _get_oauth_client_params(self) -> dict:
-        """Return parameters for the OAuth1Client"""
+        """Return parameters for the OAuth1Client."""
         if self.consumer_token is None:
             raise MissingToken("Consumer token is missing")
         if self.access_token is None:
             raise MissingToken("Access token is missing")
 
         return {
             "client_id": self.consumer_token.key,
             "client_secret": self.consumer_token.secret,
             "token": self.access_token.token,
             "token_secret": self.access_token.token_secret,
         }
 
     async def _fetch_consumer_token(self) -> ConsumerToken:
-        """Fetches consumer token for app name"""
-        async with httpx.AsyncClient() as client:
+        """Fetches consumer token for app name."""
+        async with AsyncClient() as client:
             try:
                 consumer_response = await client.post(
                     url=API_CONSUMER_TOKEN,
                     data={"client": self.app_name},
                 )
                 consumer_response.raise_for_status()
 
                 consumer_tokens = json.loads(consumer_response.content.decode("utf-8"))
                 self.consumer_token = ConsumerToken(
                     consumer_tokens["key"], consumer_tokens["secret"]
                 )
                 return self.consumer_token
-            except httpx.RequestError as exc:
+            except RequestError as exc:
                 raise DiscovergyClientError from exc
-            except httpx.HTTPStatusError as exc:
+            except HTTPStatusError as exc:
                 raise HTTPError(
                     f"Status {exc.response.status_code}: {exc.response.content}"
                 ) from exc
             except json.JSONDecodeError as exc:
                 raise DiscovergyError(f"Failed to decode json: {exc}") from exc
 
     async def _fetch_request_token(self) -> RequestToken:
-        """Fetch request token"""
+        """Fetch request token."""
         async with AsyncOAuth1Client(
-                client_id=self.consumer_token.key, client_secret=self.consumer_token.secret
+            client_id=self.consumer_token.key, client_secret=self.consumer_token.secret
         ) as client:
             try:
                 oauth_token_response = await client.fetch_request_token(
                     API_REQUEST_TOKEN
                 )
                 return RequestToken(
                     oauth_token_response.get("oauth_token"),
                     oauth_token_response.get("oauth_token_secret"),
                 )
             except Exception as exc:
                 raise HTTPError(f"Request failed: {exc}") from exc
 
     async def _authorize_request_token(
-            self, email: str, password: str, request_token: str
-    ) -> str:  # pylint: disable=no-self-use
-        """Authorize request token for account"""
-        async with httpx.AsyncClient() as client:
+        self, email: str, password: str, request_token: str
+    ) -> str:
+        """Authorize request token for account."""
+        async with AsyncClient() as client:
             try:
                 params = {
                     "oauth_token": request_token,
                     "email": email,
                     "password": password,
                 }
                 response = await client.get(API_AUTHORIZATION, params=params)
                 response.raise_for_status()
 
                 parsed_response = parse_qs(response.content.decode("utf-8"))
 
                 verifier = parsed_response["oauth_verifier"][0]
                 return verifier
-            except httpx.RequestError as exc:
+            except RequestError as exc:
                 raise DiscovergyClientError from exc
-            except httpx.HTTPStatusError as exc:
+            except HTTPStatusError as exc:
                 if exc.response.status_code == 403:
                     # the credentials are invaild so raise the correct error
                     raise InvalidLogin from exc
                 raise HTTPError(
-                    f"Request failed with {exc.response.status_code}: {exc.response.content}"
+                    f"Request failed with {exc.response.status_code}: "
+                    f"{exc.response.content}"
                 ) from exc
 
     async def _fetch_access_token(
-            self, request_token, request_token_secret, verifier
+        self, request_token, request_token_secret, verifier
     ) -> AccessToken:
-        """Fetch access token"""
+        """Fetch access token."""
         async with AsyncOAuth1Client(
-                client_id=self.consumer_token.key,
-                client_secret=self.consumer_token.secret,
-                token=request_token,
-                token_secret=request_token_secret,
+            client_id=self.consumer_token.key,
+            client_secret=self.consumer_token.secret,
+            token=request_token,
+            token_secret=request_token_secret,
         ) as client:
             try:
                 access_token_response = await client.fetch_access_token(
                     API_ACCESS_TOKEN, verifier
                 )
                 return AccessToken(
                     access_token_response.get("oauth_token"),
```

### Comparing `pydiscovergy-1.2.1/pydiscovergy/discovergy.py` & `pydiscovergy-2.0.0/pydiscovergy/discovergy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,167 +1,166 @@
 """Discovergy API."""
 from __future__ import annotations
 
 import json
+from dataclasses import dataclass
+from datetime import datetime
+from typing import Any
 
 import httpx
-from httpx import AsyncClient
 
-from pydiscovergy.authentication import BaseAuthentication, TokenAuth, BasicAuth
-from pydiscovergy.const import (
-    API_BASE,
-)
-from pydiscovergy.error import (
+from .authentication import BaseAuthentication, BasicAuth, TokenAuth
+from .const import API_BASE, DEFAULT_TIMEOUT, Resolution
+from .error import (
     AccessTokenExpired,
+    DiscovergyClientError,
     DiscovergyError,
     HTTPError,
-    DiscovergyClientError, InvalidLogin,
+    InvalidLogin,
 )
-from pydiscovergy.models import Meter, Reading
+from .marshmallow import DeviceList, FieldNameList, Statistics
+from .models import Meter, Reading, Statistic
 
 
+@dataclass
 class Discovergy:
-    """Discovergy API."""
+    """Async client for Discovergy API."""
 
-    def __init__(
-            self,
-            email: str,
-            password: str,
-            authentication: BaseAuthentication,
-            app_name: str = "pydicovergy",
-            httpx_client: AsyncClient = None,
-    ) -> None:
-        """Initialize the Python Discovergy class."""
-        self.authentication = authentication
-        self.authentication.app_name = app_name
-
-        self.email = email
-        self.password = password
-        self.app_name = app_name
-        self.httpx_client = httpx_client
+    email: str
+    password: str
+    timeout: int = DEFAULT_TIMEOUT
+    httpx_client: httpx.AsyncClient = None
+    authentication: BaseAuthentication = BasicAuth()
 
-    async def _get(self, path: str, params: dict = None) -> dict | list:
+    async def _get(self, path: str, params: dict[str, Any] = None) -> Any:
         """Execute a GET request against the API."""
 
-        async with await self.authentication.get_client(self.email, self.password, self.httpx_client) as client:
-            try:
-                response = await client.get(API_BASE + path, params=params)
+        # remove keys with empty values
+        if params is not None:
+            params = {key: value for (key, value) in params.items() if value != ""}
+
+        # get ready to use client from authentication module
+        client = await self.authentication.get_client(
+            email=self.email,
+            password=self.password,
+            timeout=self.timeout,
+            httpx_client=self.httpx_client,
+        )
+
+        try:
+            async with client:
+                response = await client.get(url=API_BASE + path, params=params)
                 response.raise_for_status()
 
                 return json.loads(response.content.decode("utf-8"))
-            except httpx.RequestError as exc:
-                raise DiscovergyClientError from exc
-            except httpx.HTTPStatusError as exc:
-                if exc.response.status_code == 401 and isinstance(self.authentication, TokenAuth):
-                    raise AccessTokenExpired from exc
-                elif isinstance(self.authentication, BasicAuth):
-                    raise InvalidLogin from exc
-                raise HTTPError(
-                    f"Request failed with status {exc.response.status_code}: {exc.response.content}"
-                ) from exc
-            except json.JSONDecodeError as exc:
-                raise DiscovergyError("Decoding failed: {exc}") from exc
+        except httpx.TimeoutException as exception:
+            raise DiscovergyClientError(
+                "Timeout occurred while connecting to Discovergy."
+            ) from exception
+        except httpx.RequestError as exception:
+            raise DiscovergyClientError(
+                "Unexpected error occurred while executing request"
+            ) from exception
+        except httpx.HTTPStatusError as exception:
+            if exception.response.status_code == 401 and isinstance(
+                self.authentication, TokenAuth
+            ):
+                raise AccessTokenExpired from exception
+
+            if exception.response.status_code == 401 and isinstance(
+                self.authentication, BasicAuth
+            ):
+                raise InvalidLogin from exception
+
+            raise HTTPError(
+                f"Request failed with HTTP status {exception.response.status_code}: "
+                f"{exception.response.content}"
+            ) from exception
+        except json.JSONDecodeError as exception:
+            raise DiscovergyError(f"JSON decoding failed: {exception}") from exception
 
-    async def get_meters(self) -> list[Meter]:
-        """Get smart meters"""
+    async def meters(self) -> list[Meter]:
+        """Get list of smart meters."""
         response = await self._get("/meters")
+        return Meter.schema().load(response, many=True)  # pylint: disable=no-member
 
-        result = []
-        for json_meter in response:
-            result.append(Meter(**json_meter))
-        return result
-
-    async def get_last_reading(self, meter_id: str) -> Reading:
+    async def meter_last_reading(self, meter_id: str) -> Reading:
         """Get last reading for meter"""
         response = await self._get("/last_reading", params={"meterId": meter_id})
-        return Reading(**response)
+        return Reading.schema().load(response)  # pylint: disable=no-member
 
-    # pylint: disable=too-many-arguments
-    async def get_readings(
-            self,
-            meter_id: str,
-            start_time: int,
-            end_time: int = 0,
-            resolution: str = "",
-            fields: list = None,
-            disaggregation: bool = False,
-            each: bool = False,
+    async def meter_readings(
+        self,
+        meter_id: str,
+        start_time: datetime,
+        end_time: datetime | None = None,
+        resolution: Resolution | None = None,
+        field_names: list[str] | None = None,
+        disaggregation: bool = False,
+        each: bool = False,
     ) -> list[Reading]:
         """Return the measurements for the specified meter in the specified time interval
 
-        each: Return data from the virtual meter itself (false) or all its sub-meters (true).
-        Only applies if meterId refers to a virtual meter
+        start_time: as datetime
 
-        disaggregation:  Include load disaggregation as pseudo-measurement fields, if available.
-        Only applies if raw resolution is selected
+        end_time: as datetime
 
-        resolution: Time distance between returned readings. Possible values:
-        raw:                1 day
-        three_minutes:      10 days
-        fifteen_minutes:    31 days
-        one_hour:           93 days
-        one_day:            10 years
-        one_week:	        20 years
-        one_month:	        50 years
-        one_year:	        100 years
+        resolution: Time distance between returned readings.
 
-        start_time: as unix time stamp in miliseconds
+        field_names: list of fields (get field names with Discovergy.meter_field_names() function)
 
-        end_time: as unix time stamp in miliseconds
+        disaggregation:  Include load disaggregation as pseudo-measurement fields, if available.
+        Only applies if raw resolution is selected
 
-        fields: comma separated list of fields (get field names with get_field_names function)
-        or put field_names to get all available values
+        each: Return data from the virtual meter itself (false) or all its sub-meters (true).
+        Only applies if meterId refers to a virtual meter
         """
-        response = await self._get(
-            "/readings?meterId="
-            + meter_id
-            + ("&field_names" if fields is None else "&fields=" + ",".join(fields))
-            + "&from="
-            + str(start_time)
-            + ("" if end_time == 0 else "&to=" + str(int(end_time)))
-            + ("" if resolution == "" else "&resolution=" + str(resolution))
-            + "&disaggregation="
-            + str(disaggregation).lower()
-            + "&each="
-            + str(each).lower()
-        )
 
-        result = []
-        for json_reading in response:
-            result.append(Reading(**json_reading))
-        return result
+        params = {
+            "meterId": meter_id,
+            "from": str(int(start_time.timestamp() * 1000)),
+            "to": ("" if end_time is None else str(int(end_time.timestamp() * 1000))),
+            "fields": ("" if field_names is None else ",".join(field_names)),
+            "resolution": ("" if resolution is None else str(resolution)),
+            "disaggregation": str(disaggregation).lower(),
+            "each": str(each).lower(),
+        }
 
-    async def get_field_names(self, meter_id: str) -> list:
+        response = await self._get("/readings", params)
+        return Reading.schema().load(response, many=True)  # pylint: disable=no-member
+
+    async def meter_field_names(self, meter_id: str) -> list[str]:
         """Return all available measurement field names for the specified meter."""
-        return await self._get("/field_names", params={"meterId": meter_id})
+        field_names = await self._get("/field_names", params={"meterId": meter_id})
+        return FieldNameList.schema().load({"field_names": field_names}).field_names
 
-    async def get_devices_for_meter(self, meter_id: str) -> list:
-        """Get devices by meter id."""
-        return await self._get("/devices", params={"meterId": meter_id})
-
-    async def get_statistics(
-            self,
-            meter_id: str,
-            start_time: int,
-            end_time: int = 0,
-            fields: list = None,
-    ) -> dict | list:
+    async def meter_devices(self, meter_id: str) -> list[str]:
+        """Return all recognized devices by meter id."""
+        devices = await self._get("/devices", params={"meterId": meter_id})
+        return DeviceList.schema().load({"devices": devices}).devices
+
+    async def meter_statistics(
+        self,
+        meter_id: str,
+        start_time: datetime,
+        end_time: datetime | None = None,
+        field_names: list[str] | None = None,
+    ) -> dict[str, Statistic]:
         """Return various statistics calculated over all measurements for the specified meter
          in the specified time interval
 
-        field_names: default value which gives out stats for all available fields
-        carry out get_field_names function to get all available field options for the specific meter
-        enter start- and end_time as time in miliseconds"""
-
-        request = (
-                "/statistics?meterId="
-                + str(meter_id)
-                + ("&field_names" if fields is None else "&fields=" + ",".join(fields))
-                + "&from="
-                + str(start_time)
-                + ("" if end_time == 0 else "&to=" + str(end_time))
-        )
+        start_time: as datetime
 
-        try:
-            return await self._get(request)
-        except json.JSONDecodeError as exc:
-            raise DiscovergyError("Decoding failed: {exc}") from exc
+        end_time: as datetime
+
+        field_names: list of fields (get field names with Discovergy.meter_field_names() function)
+        """
+
+        params = {
+            "meterId": meter_id,
+            "from": str(int(start_time.timestamp() * 1000)),
+            "to": ("" if end_time is None else str(int(end_time.timestamp() * 1000))),
+            "fields": ("" if field_names is None else ",".join(field_names)),
+        }
+
+        statistics = await self._get("/statistics", params)
+        return Statistics.schema().load({"statistics": statistics}).statistics
```

### Comparing `pydiscovergy-1.2.1/pydiscovergy/error.py` & `pydiscovergy-2.0.0/pydiscovergy/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Discovergy errors."""
+"""Exceptions for Discovergy API."""
 
 
 class DiscovergyError(Exception):
     """Generic error occurred in Discovergy package."""
 
 
 class DiscovergyClientError(DiscovergyError):
```

