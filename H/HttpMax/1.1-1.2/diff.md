# Comparing `tmp/HttpMax-1.1.tar.gz` & `tmp/HttpMax-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HttpMax-1.1.tar", last modified: Fri Feb 10 16:21:52 2023, max compression
+gzip compressed data, was "HttpMax-1.2.tar", last modified: Sun Jul 23 22:06:34 2023, max compression
```

## Comparing `HttpMax-1.1.tar` & `HttpMax-1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 16:21:52.006010 HttpMax-1.1/
-drwxrwxrwx   0        0        0        0 2023-02-10 16:21:51.990397 HttpMax-1.1/HttpMax/
--rw-rw-rw-   0        0        0     4866 2023-02-10 16:05:30.000000 HttpMax-1.1/HttpMax/__init__.py
--rw-rw-rw-   0        0        0      325 2023-02-10 16:21:30.000000 HttpMax-1.1/HttpMax/__version__.py
--rw-rw-rw-   0        0        0     1395 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/_internal_utils.py
--rw-rw-rw-   0        0        0    21266 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/adapters.py
--rw-rw-rw-   0        0        0     6575 2023-02-10 15:00:54.000000 HttpMax-1.1/HttpMax/api.py
--rw-rw-rw-   0        0        0    10181 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/auth.py
--rw-rw-rw-   0        0        0      427 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/certs.py
--rw-rw-rw-   0        0        0     1450 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/compat.py
--rw-rw-rw-   0        0        0    18543 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/cookies.py
--rw-rw-rw-   0        0        0     3799 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/exceptions.py
--rw-rw-rw-   0        0        0     3872 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/help.py
--rw-rw-rw-   0        0        0      731 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/hooks.py
--rw-rw-rw-   0        0        0    35212 2023-02-10 15:22:09.000000 HttpMax-1.1/HttpMax/models.py
--rw-rw-rw-   0        0        0      954 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/packages.py
--rw-rw-rw-   0        0        0    30260 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/sessions.py
--rw-rw-rw-   0        0        0     4230 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/status_codes.py
--rw-rw-rw-   0        0        0     2910 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/structures.py
--rw-rw-rw-   0        0        0    33217 2023-02-10 15:10:34.000000 HttpMax-1.1/HttpMax/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:21:52.006010 HttpMax-1.1/HttpMax.egg-info/
--rw-rw-rw-   0        0        0     2219 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      163 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-10 16:21:51.000000 HttpMax-1.1/HttpMax.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10142 2023-01-12 16:16:59.000000 HttpMax-1.1/LICENSE
--rw-rw-rw-   0        0        0     2219 2023-02-10 16:21:52.006010 HttpMax-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-02-10 15:27:14.000000 HttpMax-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-10 16:21:52.006010 HttpMax-1.1/setup.cfg
--rw-rw-rw-   0        0        0     2844 2023-02-10 15:42:09.000000 HttpMax-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:06:34.422737 HttpMax-1.2/
+drwxrwxrwx   0        0        0        0 2023-07-23 22:06:34.391456 HttpMax-1.2/HttpMax/
+-rw-rw-rw-   0        0        0     3216 2023-07-21 20:55:36.000000 HttpMax-1.2/HttpMax/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-07-23 22:05:40.000000 HttpMax-1.2/HttpMax/__version__.py
+-rw-rw-rw-   0        0        0    13033 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_api.py
+-rw-rw-rw-   0        0        0    11773 2020-02-02 00:00:00.000000 HttpMax-1.2/HttpMax/_auth.py
+-rw-rw-rw-   0        0        0    68189 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_client.py
+-rw-rw-rw-   0        0        0     1602 2020-02-02 00:00:00.000000 HttpMax-1.2/HttpMax/_compat.py
+-rw-rw-rw-   0        0        0    12395 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_config.py
+-rw-rw-rw-   0        0        0     8094 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_content.py
+-rw-rw-rw-   0        0        0     9743 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_decoders.py
+-rw-rw-rw-   0        0        0     7884 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_exceptions.py
+-rw-rw-rw-   0        0        0    15788 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_main.py
+-rw-rw-rw-   0        0        0    42696 2020-02-02 00:00:00.000000 HttpMax-1.2/HttpMax/_models.py
+-rw-rw-rw-   0        0        0     8974 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_multipart.py
+-rw-rw-rw-   0        0        0     5584 2020-02-02 00:00:00.000000 HttpMax-1.2/HttpMax/_status_codes.py
+-rw-rw-rw-   0        0        0     3333 2020-02-02 00:00:00.000000 HttpMax-1.2/HttpMax/_types.py
+-rw-rw-rw-   0        0        0    16671 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_urlparse.py
+-rw-rw-rw-   0        0        0    21926 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_urls.py
+-rw-rw-rw-   0        0        0    15419 2023-07-21 20:55:34.000000 HttpMax-1.2/HttpMax/_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-23 22:06:34.422737 HttpMax-1.2/HttpMax.egg-info/
+-rw-rw-rw-   0        0        0     2225 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      267 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-23 22:06:34.000000 HttpMax-1.2/HttpMax.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10142 2023-01-12 16:16:59.000000 HttpMax-1.2/LICENSE
+-rw-rw-rw-   0        0        0     2225 2023-07-23 22:06:34.422737 HttpMax-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-02-10 15:27:14.000000 HttpMax-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-23 22:06:34.422737 HttpMax-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2941 2023-07-23 22:06:04.000000 HttpMax-1.2/setup.py
```

### Comparing `HttpMax-1.1/HttpMax/auth.py` & `HttpMax-1.2/HttpMax/_auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,315 +1,347 @@
-"""
-HttpMax.auth
-~~~~~~~~~~~~~
-
-This module contains the authentication handlers for HttpMax.
-"""
-
 import hashlib
+import netrc
 import os
 import re
-import threading
 import time
-import warnings
+import typing
 from base64 import b64encode
+from urllib.request import parse_http_list
 
-from ._internal_utils import to_native_string
-from .compat import basestring, str, urlparse
-from .cookies import extract_cookies_to_jar
-from .utils import parse_dict_header
-
-CONTENT_TYPE_FORM_URLENCODED = "application/x-www-form-urlencoded"
-CONTENT_TYPE_MULTI_PART = "multipart/form-data"
-
-
-def _basic_auth_str(username, password):
-    """Returns a Basic Auth string."""
-
-    # "I want us to put a big-ol' comment on top of it that
-    # says that this behaviour is dumb but we need to preserve
-    # it because people are relying on it."
-    #    - Lukasa
-    #
-    # These are here solely to maintain backwards compatibility
-    # for things like ints. This will be removed in 3.0.0.
-    if not isinstance(username, basestring):
-        warnings.warn(
-            "Non-string usernames will no longer be supported in HttpMax "
-            "3.0.0. Please convert the object you've passed in ({!r}) to "
-            "a string or bytes object in the near future to avoid "
-            "problems.".format(username),
-            category=DeprecationWarning,
-        )
-        username = str(username)
-
-    if not isinstance(password, basestring):
-        warnings.warn(
-            "Non-string passwords will no longer be supported in HttpMax "
-            "3.0.0. Please convert the object you've passed in ({!r}) to "
-            "a string or bytes object in the near future to avoid "
-            "problems.".format(type(password)),
-            category=DeprecationWarning,
-        )
-        password = str(password)
-    # -- End Removal --
-
-    if isinstance(username, str):
-        username = username.encode("latin1")
+from ._exceptions import ProtocolError
+from ._models import Request, Response
+from ._utils import to_bytes, to_str, unquote
 
-    if isinstance(password, str):
-        password = password.encode("latin1")
+if typing.TYPE_CHECKING:  # pragma: no cover
+    from hashlib import _Hash
 
-    authstr = "Basic " + to_native_string(
-        b64encode(b":".join((username, password))).strip()
-    )
 
-    return authstr
+class Auth:
+    """
+    Base class for all authentication schemes.
 
+    To implement a custom authentication scheme, subclass `Auth` and override
+    the `.auth_flow()` method.
 
-class AuthBase:
-    """Base class that all auth implementations derive from"""
+    If the authentication scheme does I/O such as disk access or network calls, or uses
+    synchronization primitives such as locks, you should override `.sync_auth_flow()`
+    and/or `.async_auth_flow()` instead of `.auth_flow()` to provide specialized
+    implementations that will be used by `Client` and `AsyncClient` respectively.
+    """
 
-    def __call__(self, r):
-        raise NotImplementedError("Auth hooks must be callable.")
+    requires_request_body = False
+    requires_response_body = False
 
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        """
+        Execute the authentication flow.
 
-class HTTPBasicAuth(AuthBase):
-    """Attaches HTTP Basic Authentication to the given Request object."""
+        To dispatch a request, `yield` it:
 
-    def __init__(self, username, password):
-        self.username = username
-        self.password = password
+        ```
+        yield request
+        ```
 
-    def __eq__(self, other):
-        return all(
-            [
-                self.username == getattr(other, "username", None),
-                self.password == getattr(other, "password", None),
-            ]
-        )
+        The client will `.send()` the response back into the flow generator. You can
+        access it like so:
 
-    def __ne__(self, other):
-        return not self == other
+        ```
+        response = yield request
+        ```
 
-    def __call__(self, r):
-        r.headers["Authorization"] = _basic_auth_str(self.username, self.password)
-        return r
-
-
-class HTTPProxyAuth(HTTPBasicAuth):
-    """Attaches HTTP Proxy Authentication to a given Request object."""
-
-    def __call__(self, r):
-        r.headers["Proxy-Authorization"] = _basic_auth_str(self.username, self.password)
-        return r
-
-
-class HTTPDigestAuth(AuthBase):
-    """Attaches HTTP Digest Authentication to the given Request object."""
-
-    def __init__(self, username, password):
-        self.username = username
-        self.password = password
-        # Keep state in per-thread local storage
-        self._thread_local = threading.local()
-
-    def init_per_thread_state(self):
-        # Ensure state is initialized just once per-thread
-        if not hasattr(self._thread_local, "init"):
-            self._thread_local.init = True
-            self._thread_local.last_nonce = ""
-            self._thread_local.nonce_count = 0
-            self._thread_local.chal = {}
-            self._thread_local.pos = None
-            self._thread_local.num_401_calls = None
+        A `return` (or reaching the end of the generator) will result in the
+        client returning the last response obtained from the server.
 
-    def build_digest_header(self, method, url):
-        """
-        :rtype: str
+        You can dispatch as many requests as is necessary.
         """
+        yield request
 
-        realm = self._thread_local.chal["realm"]
-        nonce = self._thread_local.chal["nonce"]
-        qop = self._thread_local.chal.get("qop")
-        algorithm = self._thread_local.chal.get("algorithm")
-        opaque = self._thread_local.chal.get("opaque")
-        hash_utf8 = None
-
-        if algorithm is None:
-            _algorithm = "MD5"
-        else:
-            _algorithm = algorithm.upper()
-        # lambdas assume digest modules are imported at the top level
-        if _algorithm == "MD5" or _algorithm == "MD5-SESS":
+    def sync_auth_flow(
+        self, request: Request
+    ) -> typing.Generator[Request, Response, None]:
+        """
+        Execute the authentication flow synchronously.
 
-            def md5_utf8(x):
-                if isinstance(x, str):
-                    x = x.encode("utf-8")
-                return hashlib.md5(x).hexdigest()
+        By default, this defers to `.auth_flow()`. You should override this method
+        when the authentication scheme does I/O and/or uses concurrency primitives.
+        """
+        if self.requires_request_body:
+            request.read()
 
-            hash_utf8 = md5_utf8
-        elif _algorithm == "SHA":
+        flow = self.auth_flow(request)
+        request = next(flow)
 
-            def sha_utf8(x):
-                if isinstance(x, str):
-                    x = x.encode("utf-8")
-                return hashlib.sha1(x).hexdigest()
+        while True:
+            response = yield request
+            if self.requires_response_body:
+                response.read()
+
+            try:
+                request = flow.send(response)
+            except StopIteration:
+                break
+
+    async def async_auth_flow(
+        self, request: Request
+    ) -> typing.AsyncGenerator[Request, Response]:
+        """
+        Execute the authentication flow asynchronously.
 
-            hash_utf8 = sha_utf8
-        elif _algorithm == "SHA-256":
+        By default, this defers to `.auth_flow()`. You should override this method
+        when the authentication scheme does I/O and/or uses concurrency primitives.
+        """
+        if self.requires_request_body:
+            await request.aread()
 
-            def sha256_utf8(x):
-                if isinstance(x, str):
-                    x = x.encode("utf-8")
-                return hashlib.sha256(x).hexdigest()
+        flow = self.auth_flow(request)
+        request = next(flow)
 
-            hash_utf8 = sha256_utf8
-        elif _algorithm == "SHA-512":
+        while True:
+            response = yield request
+            if self.requires_response_body:
+                await response.aread()
+
+            try:
+                request = flow.send(response)
+            except StopIteration:
+                break
+
+
+class FunctionAuth(Auth):
+    """
+    Allows the 'auth' argument to be passed as a simple callable function,
+    that takes the request, and returns a new, modified request.
+    """
+
+    def __init__(self, func: typing.Callable[[Request], Request]) -> None:
+        self._func = func
+
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        yield self._func(request)
+
+
+class BasicAuth(Auth):
+    """
+    Allows the 'auth' argument to be passed as a (username, password) pair,
+    and uses HTTP Basic authentication.
+    """
+
+    def __init__(
+        self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
+    ):
+        self._auth_header = self._build_auth_header(username, password)
+
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        request.headers["Authorization"] = self._auth_header
+        yield request
+
+    def _build_auth_header(
+        self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
+    ) -> str:
+        userpass = b":".join((to_bytes(username), to_bytes(password)))
+        token = b64encode(userpass).decode()
+        return f"Basic {token}"
+
+
+class NetRCAuth(Auth):
+    """
+    Use a 'netrc' file to lookup basic auth credentials based on the url host.
+    """
+
+    def __init__(self, file: typing.Optional[str] = None):
+        self._netrc_info = netrc.netrc(file)
+
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        auth_info = self._netrc_info.authenticators(request.url.host)
+        if auth_info is None or not auth_info[2]:
+            # The netrc file did not have authentication credentials for this host.
+            yield request
+        else:
+            # Build a basic auth header with credentials from the netrc file.
+            request.headers["Authorization"] = self._build_auth_header(
+                username=auth_info[0], password=auth_info[2]
+            )
+            yield request
 
-            def sha512_utf8(x):
-                if isinstance(x, str):
-                    x = x.encode("utf-8")
-                return hashlib.sha512(x).hexdigest()
+    def _build_auth_header(
+        self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
+    ) -> str:
+        userpass = b":".join((to_bytes(username), to_bytes(password)))
+        token = b64encode(userpass).decode()
+        return f"Basic {token}"
+
+
+class DigestAuth(Auth):
+    _ALGORITHM_TO_HASH_FUNCTION: typing.Dict[str, typing.Callable[[bytes], "_Hash"]] = {
+        "MD5": hashlib.md5,
+        "MD5-SESS": hashlib.md5,
+        "SHA": hashlib.sha1,
+        "SHA-SESS": hashlib.sha1,
+        "SHA-256": hashlib.sha256,
+        "SHA-256-SESS": hashlib.sha256,
+        "SHA-512": hashlib.sha512,
+        "SHA-512-SESS": hashlib.sha512,
+    }
+
+    def __init__(
+        self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
+    ) -> None:
+        self._username = to_bytes(username)
+        self._password = to_bytes(password)
+        self._last_challenge: typing.Optional[_DigestAuthChallenge] = None
+        self._nonce_count = 1
+
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        if self._last_challenge:
+            request.headers["Authorization"] = self._build_auth_header(
+                request, self._last_challenge
+            )
 
-            hash_utf8 = sha512_utf8
+        response = yield request
 
-        KD = lambda s, d: hash_utf8(f"{s}:{d}")  # noqa:E731
+        if response.status_code != 401 or "www-authenticate" not in response.headers:
+            # If the response is not a 401 then we don't
+            # need to build an authenticated request.
+            return
+
+        for auth_header in response.headers.get_list("www-authenticate"):
+            if auth_header.lower().startswith("digest "):
+                break
+        else:
+            # If the response does not include a 'WWW-Authenticate: Digest ...'
+            # header, then we don't need to build an authenticated request.
+            return
 
-        if hash_utf8 is None:
-            return None
+        self._last_challenge = self._parse_challenge(request, response, auth_header)
+        self._nonce_count = 1
 
-        # XXX not implemented yet
-        entdig = None
-        p_parsed = urlparse(url)
-        #: path is request-uri defined in RFC 2616 which should not be empty
-        path = p_parsed.path or "/"
-        if p_parsed.query:
-            path += f"?{p_parsed.query}"
+        request.headers["Authorization"] = self._build_auth_header(
+            request, self._last_challenge
+        )
+        yield request
 
-        A1 = f"{self.username}:{realm}:{self.password}"
-        A2 = f"{method}:{path}"
+    def _parse_challenge(
+        self, request: Request, response: Response, auth_header: str
+    ) -> "_DigestAuthChallenge":
+        """
+        Returns a challenge from a Digest WWW-Authenticate header.
+        These take the form of:
+        `Digest realm="realm@host.com",qop="auth,auth-int",nonce="abc",opaque="xyz"`
+        """
+        scheme, _, fields = auth_header.partition(" ")
 
-        HA1 = hash_utf8(A1)
-        HA2 = hash_utf8(A2)
+        # This method should only ever have been called with a Digest auth header.
+        assert scheme.lower() == "digest"
 
-        if nonce == self._thread_local.last_nonce:
-            self._thread_local.nonce_count += 1
-        else:
-            self._thread_local.nonce_count = 1
-        ncvalue = f"{self._thread_local.nonce_count:08x}"
-        s = str(self._thread_local.nonce_count).encode("utf-8")
-        s += nonce.encode("utf-8")
-        s += time.ctime().encode("utf-8")
-        s += os.urandom(8)
+        header_dict: typing.Dict[str, str] = {}
+        for field in parse_http_list(fields):
+            key, value = field.strip().split("=", 1)
+            header_dict[key] = unquote(value)
 
-        cnonce = hashlib.sha1(s).hexdigest()[:16]
-        if _algorithm == "MD5-SESS":
-            HA1 = hash_utf8(f"{HA1}:{nonce}:{cnonce}")
-
-        if not qop:
-            respdig = KD(HA1, f"{nonce}:{HA2}")
-        elif qop == "auth" or "auth" in qop.split(","):
-            noncebit = f"{nonce}:{ncvalue}:{cnonce}:auth:{HA2}"
-            respdig = KD(HA1, noncebit)
+        try:
+            realm = header_dict["realm"].encode()
+            nonce = header_dict["nonce"].encode()
+            algorithm = header_dict.get("algorithm", "MD5")
+            opaque = header_dict["opaque"].encode() if "opaque" in header_dict else None
+            qop = header_dict["qop"].encode() if "qop" in header_dict else None
+            return _DigestAuthChallenge(
+                realm=realm, nonce=nonce, algorithm=algorithm, opaque=opaque, qop=qop
+            )
+        except KeyError as exc:
+            message = "Malformed Digest WWW-Authenticate header"
+            raise ProtocolError(message, request=request) from exc
+
+    def _build_auth_header(
+        self, request: Request, challenge: "_DigestAuthChallenge"
+    ) -> str:
+        hash_func = self._ALGORITHM_TO_HASH_FUNCTION[challenge.algorithm.upper()]
+
+        def digest(data: bytes) -> bytes:
+            return hash_func(data).hexdigest().encode()
+
+        A1 = b":".join((self._username, challenge.realm, self._password))
+
+        path = request.url.raw_path
+        A2 = b":".join((request.method.encode(), path))
+        # TODO: implement auth-int
+        HA2 = digest(A2)
+
+        nc_value = b"%08x" % self._nonce_count
+        cnonce = self._get_client_nonce(self._nonce_count, challenge.nonce)
+        self._nonce_count += 1
+
+        HA1 = digest(A1)
+        if challenge.algorithm.lower().endswith("-sess"):
+            HA1 = digest(b":".join((HA1, challenge.nonce, cnonce)))
+
+        qop = self._resolve_qop(challenge.qop, request=request)
+        if qop is None:
+            digest_data = [HA1, challenge.nonce, HA2]
         else:
-            # XXX handle auth-int.
-            return None
-
-        self._thread_local.last_nonce = nonce
+            digest_data = [challenge.nonce, nc_value, cnonce, qop, HA2]
+        key_digest = b":".join(digest_data)
 
-        # XXX should the partial digests be encoded too?
-        base = (
-            f'username="{self.username}", realm="{realm}", nonce="{nonce}", '
-            f'uri="{path}", response="{respdig}"'
-        )
-        if opaque:
-            base += f', opaque="{opaque}"'
-        if algorithm:
-            base += f', algorithm="{algorithm}"'
-        if entdig:
-            base += f', digest="{entdig}"'
+        format_args = {
+            "username": self._username,
+            "realm": challenge.realm,
+            "nonce": challenge.nonce,
+            "uri": path,
+            "response": digest(b":".join((HA1, key_digest))),
+            "algorithm": challenge.algorithm.encode(),
+        }
+        if challenge.opaque:
+            format_args["opaque"] = challenge.opaque
         if qop:
-            base += f', qop="auth", nc={ncvalue}, cnonce="{cnonce}"'
-
-        return f"Digest {base}"
-
-    def handle_redirect(self, r, **kwargs):
-        """Reset num_401_calls counter on redirects."""
-        if r.is_redirect:
-            self._thread_local.num_401_calls = 1
-
-    def handle_401(self, r, **kwargs):
-        """
-        Takes the given response and tries digest-auth, if needed.
-
-        :rtype: HttpMax.Response
-        """
+            format_args["qop"] = b"auth"
+            format_args["nc"] = nc_value
+            format_args["cnonce"] = cnonce
+
+        return "Digest " + self._get_header_value(format_args)
+
+    def _get_client_nonce(self, nonce_count: int, nonce: bytes) -> bytes:
+        s = str(nonce_count).encode()
+        s += nonce
+        s += time.ctime().encode()
+        s += os.urandom(8)
 
-        # If response is not 4xx, do not auth
-        # See https://github.com/psf/HttpMax/issues/3772
-        if not 400 <= r.status_code < 500:
-            self._thread_local.num_401_calls = 1
-            return r
-
-        if self._thread_local.pos is not None:
-            # Rewind the file position indicator of the body to where
-            # it was to resend the request.
-            r.request.body.seek(self._thread_local.pos)
-        s_auth = r.headers.get("www-authenticate", "")
-
-        if "digest" in s_auth.lower() and self._thread_local.num_401_calls < 2:
-
-            self._thread_local.num_401_calls += 1
-            pat = re.compile(r"digest ", flags=re.IGNORECASE)
-            self._thread_local.chal = parse_dict_header(pat.sub("", s_auth, count=1))
-
-            # Consume content and release the original connection
-            # to allow our new request to reuse the same one.
-            r.content
-            r.close()
-            prep = r.request.copy()
-            extract_cookies_to_jar(prep._cookies, r.request, r.raw)
-            prep.prepare_cookies(prep._cookies)
+        return hashlib.sha1(s).hexdigest()[:16].encode()
 
-            prep.headers["Authorization"] = self.build_digest_header(
-                prep.method, prep.url
+    def _get_header_value(self, header_fields: typing.Dict[str, bytes]) -> str:
+        NON_QUOTED_FIELDS = ("algorithm", "qop", "nc")
+        QUOTED_TEMPLATE = '{}="{}"'
+        NON_QUOTED_TEMPLATE = "{}={}"
+
+        header_value = ""
+        for i, (field, value) in enumerate(header_fields.items()):
+            if i > 0:
+                header_value += ", "
+            template = (
+                QUOTED_TEMPLATE
+                if field not in NON_QUOTED_FIELDS
+                else NON_QUOTED_TEMPLATE
             )
-            _r = r.connection.send(prep, **kwargs)
-            _r.history.append(r)
-            _r.request = prep
-
-            return _r
-
-        self._thread_local.num_401_calls = 1
-        return r
-
-    def __call__(self, r):
-        # Initialize per-thread state, if needed
-        self.init_per_thread_state()
-        # If we have a saved nonce, skip the 401
-        if self._thread_local.last_nonce:
-            r.headers["Authorization"] = self.build_digest_header(r.method, r.url)
-        try:
-            self._thread_local.pos = r.body.tell()
-        except AttributeError:
-            # In the case of HTTPDigestAuth being reused and the body of
-            # the previous request was a file-like object, pos has the
-            # file position of the previous body. Ensure it's set to
-            # None.
-            self._thread_local.pos = None
-        r.register_hook("response", self.handle_401)
-        r.register_hook("response", self.handle_redirect)
-        self._thread_local.num_401_calls = 1
-
-        return r
-
-    def __eq__(self, other):
-        return all(
-            [
-                self.username == getattr(other, "username", None),
-                self.password == getattr(other, "password", None),
-            ]
-        )
+            header_value += template.format(field, to_str(value))
 
-    def __ne__(self, other):
-        return not self == other
+        return header_value
+
+    def _resolve_qop(
+        self, qop: typing.Optional[bytes], request: Request
+    ) -> typing.Optional[bytes]:
+        if qop is None:
+            return None
+        qops = re.split(b", ?", qop)
+        if b"auth" in qops:
+            return b"auth"
+
+        if qops == [b"auth-int"]:
+            raise NotImplementedError("Digest auth-int support is not yet implemented")
+
+        message = f'Unexpected qop value "{qop!r}" in digest auth'
+        raise ProtocolError(message, request=request)
+
+
+class _DigestAuthChallenge(typing.NamedTuple):
+    realm: bytes
+    nonce: bytes
+    algorithm: str
+    opaque: typing.Optional[bytes]
+    qop: typing.Optional[bytes]
```

### Comparing `HttpMax-1.1/HttpMax/models.py` & `HttpMax-1.2/HttpMax/_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1034 +1,1209 @@
-"""
-HttpMax.models
-~~~~~~~~~~~~~~~
-
-This module contains the primary objects that power HttpMax.
-"""
-
 import datetime
-
-# Import encoding now, to avoid implicit import later.
-# Implicit import within threads may cause LookupError when standard library is in a ZIP,
-# such as in Embedded Python. See https://github.com/psf/HttpMax/issues/3578.
-import encodings.idna  # noqa: F401
-from io import UnsupportedOperation
-
-from urllib3.exceptions import (
-    DecodeError,
-    LocationParseError,
-    ProtocolError,
-    ReadTimeoutError,
-    SSLError,
+import email.message
+import json as jsonlib
+import typing
+import urllib.request
+from collections.abc import Mapping
+from http.cookiejar import Cookie, CookieJar
+
+from ._content import ByteStream, UnattachedStream, encode_request, encode_response
+from ._decoders import (
+    SUPPORTED_DECODERS,
+    ByteChunker,
+    ContentDecoder,
+    IdentityDecoder,
+    LineDecoder,
+    MultiDecoder,
+    TextChunker,
+    TextDecoder,
 )
-from urllib3.fields import RequestField
-from urllib3.filepost import encode_multipart_formdata
-from urllib3.util import parse_url
-
-from ._internal_utils import to_native_string, unicode_is_ascii
-from .auth import HTTPBasicAuth
-from .compat import (
-    Callable,
-    JSONDecodeError,
-    Mapping,
-    basestring,
-    builtin_str,
-    chardet,
-    cookielib,
+from ._exceptions import (
+    CookieConflict,
+    HTTPStatusError,
+    RequestNotRead,
+    ResponseNotRead,
+    StreamClosed,
+    StreamConsumed,
+    request_context,
 )
-from .compat import json as complexjson
-from .compat import urlencode, urlsplit, urlunparse
-from .cookies import _copy_cookie_jar, cookiejar_from_dict, get_cookie_header
-from .exceptions import (
-    ChunkedEncodingError,
-    ConnectionError,
-    ContentDecodingError,
-    HTTPError,
-    InvalidJSONError,
-    InvalidURL,
+from ._multipart import get_multipart_boundary_from_content_type
+from ._status_codes import codes
+from ._types import (
+    AsyncByteStream,
+    CookieTypes,
+    HeaderTypes,
+    QueryParamTypes,
+    RequestContent,
+    RequestData,
+    RequestExtensions,
+    RequestFiles,
+    ResponseContent,
+    ResponseExtensions,
+    SyncByteStream,
 )
-from .exceptions import JSONDecodeError as HttpMaxJSONDecodeError
-from .exceptions import MissingSchema
-from .exceptions import SSLError as HttpMaxSSLError
-from .exceptions import StreamConsumedError
-from .hooks import default_hooks
-from .status_codes import codes
-from .structures import CaseInsensitiveDict
-from .utils import (
-    check_header_validity,
-    get_auth_from_url,
-    guess_filename,
+from ._urls import URL
+from ._utils import (
     guess_json_utf,
-    iter_slices,
+    is_known_encoding,
+    normalize_header_key,
+    normalize_header_value,
+    obfuscate_sensitive_headers,
+    parse_content_type_charset,
     parse_header_links,
-    requote_uri,
-    stream_decode_response_unicode,
-    super_len,
-    to_key_val_list,
 )
 
-#: The set of HTTP status codes that indicate an automatically
-#: processable redirect.
-REDIRECT_STATI = (
-    codes.moved,  # 301
-    codes.found,  # 302
-    codes.other,  # 303
-    codes.temporary_redirect,  # 307
-    codes.permanent_redirect,  # 308
-)
 
-DEFAULT_REDIRECT_LIMIT = 30
-CONTENT_CHUNK_SIZE = 10 * 1024
-ITER_CHUNK_SIZE = 512
-
-
-class RequestEncodingMixin:
-    @property
-    def path_url(self):
-        """Build the path URL to use."""
-
-        url = []
-
-        p = urlsplit(self.url)
-
-        path = p.path
-        if not path:
-            path = "/"
-
-        url.append(path)
-
-        query = p.query
-        if query:
-            url.append("?")
-            url.append(query)
-
-        return "".join(url)
-
-    @staticmethod
-    def _encode_params(data):
-        """Encode parameters in a piece of data.
-
-        Will successfully encode parameters when passed as a dict or a list of
-        2-tuples. Order is retained if data is a list of 2-tuples but arbitrary
-        if parameters are supplied as a dict.
-        """
-
-        if isinstance(data, (str, bytes)):
-            return data
-        elif hasattr(data, "read"):
-            return data
-        elif hasattr(data, "__iter__"):
-            result = []
-            for k, vs in to_key_val_list(data):
-                if isinstance(vs, basestring) or not hasattr(vs, "__iter__"):
-                    vs = [vs]
-                for v in vs:
-                    if v is not None:
-                        result.append(
-                            (
-                                k.encode("utf-8") if isinstance(k, str) else k,
-                                v.encode("utf-8") if isinstance(v, str) else v,
-                            )
-                        )
-            return urlencode(result, doseq=True)
+class Headers(typing.MutableMapping[str, str]):
+    """
+    HTTP headers, as a case-insensitive multi-dict.
+    """
+
+    def __init__(
+        self,
+        headers: typing.Optional[HeaderTypes] = None,
+        encoding: typing.Optional[str] = None,
+    ) -> None:
+        if headers is None:
+            self._list = []  # type: typing.List[typing.Tuple[bytes, bytes, bytes]]
+        elif isinstance(headers, Headers):
+            self._list = list(headers._list)
+        elif isinstance(headers, Mapping):
+            self._list = [
+                (
+                    normalize_header_key(k, lower=False, encoding=encoding),
+                    normalize_header_key(k, lower=True, encoding=encoding),
+                    normalize_header_value(v, encoding),
+                )
+                for k, v in headers.items()
+            ]
         else:
-            return data
+            self._list = [
+                (
+                    normalize_header_key(k, lower=False, encoding=encoding),
+                    normalize_header_key(k, lower=True, encoding=encoding),
+                    normalize_header_value(v, encoding),
+                )
+                for k, v in headers
+            ]
 
-    @staticmethod
-    def _encode_files(files, data):
-        """Build the body for a multipart/form-data request.
-
-        Will successfully encode files when passed as a dict or a list of
-        tuples. Order is retained if data is a list of tuples but arbitrary
-        if parameters are supplied as a dict.
-        The tuples may be 2-tuples (filename, fileobj), 3-tuples (filename, fileobj, contentype)
-        or 4-tuples (filename, fileobj, contentype, custom_headers).
-        """
-        if not files:
-            raise ValueError("Files must be provided.")
-        elif isinstance(data, basestring):
-            raise ValueError("Data must not be a string.")
-
-        new_fields = []
-        fields = to_key_val_list(data or {})
-        files = to_key_val_list(files or {})
-
-        for field, val in fields:
-            if isinstance(val, basestring) or not hasattr(val, "__iter__"):
-                val = [val]
-            for v in val:
-                if v is not None:
-                    # Don't call str() on bytestrings: in Py3 it all goes wrong.
-                    if not isinstance(v, bytes):
-                        v = str(v)
-
-                    new_fields.append(
-                        (
-                            field.decode("utf-8")
-                            if isinstance(field, bytes)
-                            else field,
-                            v.encode("utf-8") if isinstance(v, str) else v,
-                        )
-                    )
-
-        for (k, v) in files:
-            # support for explicit filename
-            ft = None
-            fh = None
-            if isinstance(v, (tuple, list)):
-                if len(v) == 2:
-                    fn, fp = v
-                elif len(v) == 3:
-                    fn, fp, ft = v
+        self._encoding = encoding
+
+    @property
+    def encoding(self) -> str:
+        """
+        Header encoding is mandated as ascii, but we allow fallbacks to utf-8
+        or iso-8859-1.
+        """
+        if self._encoding is None:
+            for encoding in ["ascii", "utf-8"]:
+                for key, value in self.raw:
+                    try:
+                        key.decode(encoding)
+                        value.decode(encoding)
+                    except UnicodeDecodeError:
+                        break
                 else:
-                    fn, fp, ft, fh = v
+                    # The else block runs if 'break' did not occur, meaning
+                    # all values fitted the encoding.
+                    self._encoding = encoding
+                    break
             else:
-                fn = guess_filename(v) or k
-                fp = v
+                # The ISO-8859-1 encoding covers all 256 code points in a byte,
+                # so will never raise decode errors.
+                self._encoding = "iso-8859-1"
+        return self._encoding
+
+    @encoding.setter
+    def encoding(self, value: str) -> None:
+        self._encoding = value
 
-            if isinstance(fp, (str, bytes, bytearray)):
-                fdata = fp
-            elif hasattr(fp, "read"):
-                fdata = fp.read()
-            elif fp is None:
-                continue
+    @property
+    def raw(self) -> typing.List[typing.Tuple[bytes, bytes]]:
+        """
+        Returns a list of the raw header items, as byte pairs.
+        """
+        return [(raw_key, value) for raw_key, _, value in self._list]
+
+    def keys(self) -> typing.KeysView[str]:
+        return {key.decode(self.encoding): None for _, key, value in self._list}.keys()
+
+    def values(self) -> typing.ValuesView[str]:
+        values_dict: typing.Dict[str, str] = {}
+        for _, key, value in self._list:
+            str_key = key.decode(self.encoding)
+            str_value = value.decode(self.encoding)
+            if str_key in values_dict:
+                values_dict[str_key] += f", {str_value}"
             else:
-                fdata = fp
+                values_dict[str_key] = str_value
+        return values_dict.values()
 
-            rf = RequestField(name=k, data=fdata, filename=fn, headers=fh)
-            rf.make_multipart(content_type=ft)
-            new_fields.append(rf)
+    def items(self) -> typing.ItemsView[str, str]:
+        """
+        Return `(key, value)` items of headers. Concatenate headers
+        into a single comma separated value when a key occurs multiple times.
+        """
+        values_dict: typing.Dict[str, str] = {}
+        for _, key, value in self._list:
+            str_key = key.decode(self.encoding)
+            str_value = value.decode(self.encoding)
+            if str_key in values_dict:
+                values_dict[str_key] += f", {str_value}"
+            else:
+                values_dict[str_key] = str_value
+        return values_dict.items()
 
-        body, content_type = encode_multipart_formdata(new_fields)
+    def multi_items(self) -> typing.List[typing.Tuple[str, str]]:
+        """
+        Return a list of `(key, value)` pairs of headers. Allow multiple
+        occurrences of the same key without concatenating into a single
+        comma separated value.
+        """
+        return [
+            (key.decode(self.encoding), value.decode(self.encoding))
+            for _, key, value in self._list
+        ]
 
-        return body, content_type
+    def get(self, key: str, default: typing.Any = None) -> typing.Any:
+        """
+        Return a header value. If multiple occurrences of the header occur
+        then concatenate them together with commas.
+        """
+        try:
+            return self[key]
+        except KeyError:
+            return default
 
+    def get_list(self, key: str, split_commas: bool = False) -> typing.List[str]:
+        """
+        Return a list of all header values for a given key.
+        If `split_commas=True` is passed, then any comma separated header
+        values are split into multiple return strings.
+        """
+        get_header_key = key.lower().encode(self.encoding)
 
-class RequestHooksMixin:
-    def register_hook(self, event, hook):
-        """Properly register a hook."""
+        values = [
+            item_value.decode(self.encoding)
+            for _, item_key, item_value in self._list
+            if item_key.lower() == get_header_key
+        ]
+
+        if not split_commas:
+            return values
+
+        split_values = []
+        for value in values:
+            split_values.extend([item.strip() for item in value.split(",")])
+        return split_values
+
+    def update(self, headers: typing.Optional[HeaderTypes] = None) -> None:  # type: ignore
+        headers = Headers(headers)
+        for key in headers.keys():
+            if key in self:
+                self.pop(key)
+        self._list.extend(headers._list)
 
-        if event not in self.hooks:
-            raise ValueError(f'Unsupported event specified, with event name "{event}"')
+    def copy(self) -> "Headers":
+        return Headers(self, encoding=self.encoding)
 
-        if isinstance(hook, Callable):
-            self.hooks[event].append(hook)
-        elif hasattr(hook, "__iter__"):
-            self.hooks[event].extend(h for h in hook if isinstance(h, Callable))
+    def __getitem__(self, key: str) -> str:
+        """
+        Return a single header value.
 
-    def deregister_hook(self, event, hook):
-        """Deregister a previously registered hook.
-        Returns True if the hook existed, False if not.
+        If there are multiple headers with the same key, then we concatenate
+        them with commas. See: https://tools.ietf.org/html/rfc7230#section-3.2.2
         """
+        normalized_key = key.lower().encode(self.encoding)
 
-        try:
-            self.hooks[event].remove(hook)
-            return True
-        except ValueError:
-            return False
+        items = [
+            header_value.decode(self.encoding)
+            for _, header_key, header_value in self._list
+            if header_key == normalized_key
+        ]
 
+        if items:
+            return ", ".join(items)
 
-class Request(RequestHooksMixin):
-    """A user-created :class:`Request <Request>` object.
+        raise KeyError(key)
 
-    Used to prepare a :class:`PreparedRequest <PreparedRequest>`, which is sent to the server.
+    def __setitem__(self, key: str, value: str) -> None:
+        """
+        Set the header `key` to `value`, removing any duplicate entries.
+        Retains insertion order.
+        """
+        set_key = key.encode(self._encoding or "utf-8")
+        set_value = value.encode(self._encoding or "utf-8")
+        lookup_key = set_key.lower()
+
+        found_indexes = [
+            idx
+            for idx, (_, item_key, _) in enumerate(self._list)
+            if item_key == lookup_key
+        ]
+
+        for idx in reversed(found_indexes[1:]):
+            del self._list[idx]
+
+        if found_indexes:
+            idx = found_indexes[0]
+            self._list[idx] = (set_key, lookup_key, set_value)
+        else:
+            self._list.append((set_key, lookup_key, set_value))
 
-    :param method: HTTP method to use.
-    :param url: URL to send.
-    :param headers: dictionary of headers to send.
-    :param files: dictionary of {filename: fileobject} files to multipart upload.
-    :param data: the body to attach to the request. If a dictionary or
-        list of tuples ``[(key, value)]`` is provided, form-encoding will
-        take place.
-    :param json: json for the body to attach to the request (if files or data is not specified).
-    :param params: URL parameters to append to the URL. If a dictionary or
-        list of tuples ``[(key, value)]`` is provided, form-encoding will
-        take place.
-    :param auth: Auth handler or (user, pass) tuple.
-    :param cookies: dictionary or CookieJar of cookies to attach to this request.
-    :param hooks: dictionary of callback hooks, for internal usage.
-
-    Usage::
-
-      >>> import HttpMax
-      >>> req = HttpMax.Request('GET', 'https://httpbin.org/get')
-      >>> req.prepare()
-      <PreparedRequest [GET]>
-    """
+    def __delitem__(self, key: str) -> None:
+        """
+        Remove the header `key`.
+        """
+        del_key = key.lower().encode(self.encoding)
 
-    def __init__(
-        self,
-        method=None,
-        url=None,
-        headers=None,
-        files=None,
-        data=None,
-        params=None,
-        auth=None,
-        cookies=None,
-        hooks=None,
-        json=None,
-    ):
+        pop_indexes = [
+            idx
+            for idx, (_, item_key, _) in enumerate(self._list)
+            if item_key.lower() == del_key
+        ]
 
-        # Default empty dicts for dict params.
-        data = [] if data is None else data
-        files = [] if files is None else files
-        headers = {} if headers is None else headers
-        params = {} if params is None else params
-        hooks = {} if hooks is None else hooks
-
-        self.hooks = default_hooks()
-        for (k, v) in list(hooks.items()):
-            self.register_hook(event=k, hook=v)
-
-        self.method = method
-        self.url = url
-        self.headers = headers
-        self.files = files
-        self.data = data
-        self.json = json
-        self.params = params
-        self.auth = auth
-        self.cookies = cookies
-
-    def __repr__(self):
-        return f"<Request [{self.method}]>"
-
-    def prepare(self):
-        """Constructs a :class:`PreparedRequest <PreparedRequest>` for transmission and returns it."""
-        p = PreparedRequest()
-        p.prepare(
-            method=self.method,
-            url=self.url,
-            headers=self.headers,
-            files=self.files,
-            data=self.data,
-            json=self.json,
-            params=self.params,
-            auth=self.auth,
-            cookies=self.cookies,
-            hooks=self.hooks,
-        )
-        return p
+        if not pop_indexes:
+            raise KeyError(key)
 
+        for idx in reversed(pop_indexes):
+            del self._list[idx]
 
-class PreparedRequest(RequestEncodingMixin, RequestHooksMixin):
-    """The fully mutable :class:`PreparedRequest <PreparedRequest>` object,
-    containing the exact bytes that will be sent to the server.
+    def __contains__(self, key: typing.Any) -> bool:
+        header_key = key.lower().encode(self.encoding)
+        return header_key in [key for _, key, _ in self._list]
 
-    Instances are generated from a :class:`Request <Request>` object, and
-    should not be instantiated manually; doing so may produce undesirable
-    effects.
+    def __iter__(self) -> typing.Iterator[typing.Any]:
+        return iter(self.keys())
 
-    Usage::
+    def __len__(self) -> int:
+        return len(self._list)
 
-      >>> import HttpMax
-      >>> req = HttpMax.Request('GET', 'https://httpbin.org/get')
-      >>> r = req.prepare()
-      >>> r
-      <PreparedRequest [GET]>
+    def __eq__(self, other: typing.Any) -> bool:
+        try:
+            other_headers = Headers(other)
+        except ValueError:
+            return False
 
-      >>> s = HttpMax.Session()
-      >>> s.send(r)
-      <Response [200]>
-    """
+        self_list = [(key, value) for _, key, value in self._list]
+        other_list = [(key, value) for _, key, value in other_headers._list]
+        return sorted(self_list) == sorted(other_list)
 
-    def __init__(self):
-        #: HTTP verb to send to the server.
-        self.method = None
-        #: HTTP URL to send the request to.
-        self.url = None
-        #: dictionary of HTTP headers.
-        self.headers = None
-        # The `CookieJar` used to create the Cookie header will be stored here
-        # after prepare_cookies is called
-        self._cookies = None
-        #: request body to send to the server.
-        self.body = None
-        #: dictionary of callback hooks, for internal usage.
-        self.hooks = default_hooks()
-        #: integer denoting starting position of a readable file-like body.
-        self._body_position = None
+    def __repr__(self) -> str:
+        class_name = self.__class__.__name__
 
-    def prepare(
-        self,
-        method=None,
-        url=None,
-        headers=None,
-        files=None,
-        data=None,
-        params=None,
-        auth=None,
-        cookies=None,
-        hooks=None,
-        json=None,
-    ):
-        """Prepares the entire request with the given parameters."""
+        encoding_str = ""
+        if self.encoding != "ascii":
+            encoding_str = f", encoding={self.encoding!r}"
 
-        self.prepare_method(method)
-        self.prepare_url(url, params)
-        self.prepare_headers(headers)
-        self.prepare_cookies(cookies)
-        self.prepare_body(data, files, json)
-        self.prepare_auth(auth, url)
-
-        # Note that prepare_auth must be last to enable authentication schemes
-        # such as OAuth to work on a fully prepared request.
-
-        # This MUST go after prepare_auth. Authenticators could add a hook
-        self.prepare_hooks(hooks)
-
-    def __repr__(self):
-        return f"<PreparedRequest [{self.method}]>"
-
-    def copy(self):
-        p = PreparedRequest()
-        p.method = self.method
-        p.url = self.url
-        p.headers = self.headers.copy() if self.headers is not None else None
-        p._cookies = _copy_cookie_jar(self._cookies)
-        p.body = self.body
-        p.hooks = self.hooks
-        p._body_position = self._body_position
-        return p
-
-    def prepare_method(self, method):
-        """Prepares the given HTTP method."""
-        self.method = method
-        if self.method is not None:
-            self.method = to_native_string(self.method.upper())
-
-    @staticmethod
-    def _get_idna_encoded_host(host):
-        import idna
+        as_list = list(obfuscate_sensitive_headers(self.multi_items()))
+        as_dict = dict(as_list)
 
-        try:
-            host = idna.encode(host, uts46=True).decode("utf-8")
-        except idna.IDNAError:
-            raise UnicodeError
-        return host
-
-    def prepare_url(self, url, params):
-        """Prepares the given HTTP URL."""
-        #: Accept objects that have string representations.
-        #: We're unable to blindly call unicode/str functions
-        #: as this will include the bytestring indicator (b'')
-        #: on python 3.x.
-        #: https://github.com/psf/HttpMax/pull/2238
-        if isinstance(url, bytes):
-            url = url.decode("utf8")
+        no_duplicate_keys = len(as_dict) == len(as_list)
+        if no_duplicate_keys:
+            return f"{class_name}({as_dict!r}{encoding_str})"
+        return f"{class_name}({as_list!r}{encoding_str})"
+
+
+class Request:
+    def __init__(
+        self,
+        method: typing.Union[str, bytes],
+        url: typing.Union["URL", str],
+        *,
+        params: typing.Optional[QueryParamTypes] = None,
+        headers: typing.Optional[HeaderTypes] = None,
+        cookies: typing.Optional[CookieTypes] = None,
+        content: typing.Optional[RequestContent] = None,
+        data: typing.Optional[RequestData] = None,
+        files: typing.Optional[RequestFiles] = None,
+        json: typing.Optional[typing.Any] = None,
+        stream: typing.Union[SyncByteStream, AsyncByteStream, None] = None,
+        extensions: typing.Optional[RequestExtensions] = None,
+    ):
+        self.method = (
+            method.decode("ascii").upper()
+            if isinstance(method, bytes)
+            else method.upper()
+        )
+        self.url = URL(url)
+        if params is not None:
+            self.url = self.url.copy_merge_params(params=params)
+        self.headers = Headers(headers)
+        self.extensions = {} if extensions is None else extensions
+
+        if cookies:
+            Cookies(cookies).set_cookie_header(self)
+
+        if stream is None:
+            content_type: typing.Optional[str] = self.headers.get("content-type")
+            headers, stream = encode_request(
+                content=content,
+                data=data,
+                files=files,
+                json=json,
+                boundary=get_multipart_boundary_from_content_type(
+                    content_type=content_type.encode(self.headers.encoding)
+                    if content_type
+                    else None
+                ),
+            )
+            self._prepare(headers)
+            self.stream = stream
+            # Load the request body, except for streaming content.
+            if isinstance(stream, ByteStream):
+                self.read()
         else:
-            url = str(url)
+            # There's an important distinction between `Request(content=...)`,
+            # and `Request(stream=...)`.
+            #
+            # Using `content=...` implies automatically populated `Host` and content
+            # headers, of either `Content-Length: ...` or `Transfer-Encoding: chunked`.
+            #
+            # Using `stream=...` will not automatically include *any* auto-populated headers.
+            #
+            # As an end-user you don't really need `stream=...`. It's only
+            # useful when:
+            #
+            # * Preserving the request stream when copying requests, eg for redirects.
+            # * Creating request instances on the *server-side* of the transport API.
+            self.stream = stream
+
+    def _prepare(self, default_headers: typing.Dict[str, str]) -> None:
+        for key, value in default_headers.items():
+            # Ignore Transfer-Encoding if the Content-Length has been set explicitly.
+            if key.lower() == "transfer-encoding" and "Content-Length" in self.headers:
+                continue
+            self.headers.setdefault(key, value)
 
-        # Remove leading whitespaces from url
-        url = url.lstrip()
+        auto_headers: typing.List[typing.Tuple[bytes, bytes]] = []
 
-        # Don't do any URL preparation for non-HTTP schemes like `mailto`,
-        # `data` etc to work around exceptions from `url_parse`, which
-        # handles RFC 3986 only.
-        if ":" in url and not url.lower().startswith("http"):
-            self.url = url
-            return
+        has_host = "Host" in self.headers
+        has_content_length = (
+            "Content-Length" in self.headers or "Transfer-Encoding" in self.headers
+        )
 
-        # Support for unicode domain names and paths.
-        try:
-            scheme, auth, host, port, path, query, fragment = parse_url(url)
-        except LocationParseError as e:
-            raise InvalidURL(*e.args)
-
-        if not scheme:
-            raise MissingSchema(
-                f"Invalid URL {url!r}: No scheme supplied. "
-                f"Perhaps you meant https://{url}?"
-            )
+        if not has_host and self.url.host:
+            auto_headers.append((b"Host", self.url.netloc))
+        if not has_content_length and self.method in ("POST", "PUT", "PATCH"):
+            auto_headers.append((b"Content-Length", b"0"))
 
-        if not host:
-            raise InvalidURL(f"Invalid URL {url!r}: No host supplied")
+        self.headers = Headers(auto_headers + self.headers.raw)
 
-        # In general, we want to try IDNA encoding the hostname if the string contains
-        # non-ASCII characters. This allows users to automatically get the correct IDNA
-        # behaviour. For strings containing only ASCII characters, we need to also verify
-        # it doesn't start with a wildcard (*), before allowing the unencoded hostname.
-        if not unicode_is_ascii(host):
-            try:
-                host = self._get_idna_encoded_host(host)
-            except UnicodeError:
-                raise InvalidURL("URL has an invalid label.")
-        elif host.startswith(("*", ".")):
-            raise InvalidURL("URL has an invalid label.")
-
-        # Carefully reconstruct the network location
-        netloc = auth or ""
-        if netloc:
-            netloc += "@"
-        netloc += host
-        if port:
-            netloc += f":{port}"
-
-        # Bare domains aren't valid URLs.
-        if not path:
-            path = "/"
-
-        if isinstance(params, (str, bytes)):
-            params = to_native_string(params)
-
-        enc_params = self._encode_params(params)
-        if enc_params:
-            if query:
-                query = f"{query}&{enc_params}"
-            else:
-                query = enc_params
+    @property
+    def content(self) -> bytes:
+        if not hasattr(self, "_content"):
+            raise RequestNotRead()
+        return self._content
+
+    def read(self) -> bytes:
+        """
+        Read and return the request content.
+        """
+        if not hasattr(self, "_content"):
+            assert isinstance(self.stream, typing.Iterable)
+            self._content = b"".join(self.stream)
+            if not isinstance(self.stream, ByteStream):
+                # If a streaming request has been read entirely into memory, then
+                # we can replace the stream with a raw bytes implementation,
+                # to ensure that any non-replayable streams can still be used.
+                self.stream = ByteStream(self._content)
+        return self._content
 
-        url = requote_uri(urlunparse([scheme, netloc, path, None, query, fragment]))
-        self.url = url
+    async def aread(self) -> bytes:
+        """
+        Read and return the request content.
+        """
+        if not hasattr(self, "_content"):
+            assert isinstance(self.stream, typing.AsyncIterable)
+            self._content = b"".join([part async for part in self.stream])
+            if not isinstance(self.stream, ByteStream):
+                # If a streaming request has been read entirely into memory, then
+                # we can replace the stream with a raw bytes implementation,
+                # to ensure that any non-replayable streams can still be used.
+                self.stream = ByteStream(self._content)
+        return self._content
 
-    def prepare_headers(self, headers):
-        """Prepares the given HTTP headers."""
+    def __repr__(self) -> str:
+        class_name = self.__class__.__name__
+        url = str(self.url)
+        return f"<{class_name}({self.method!r}, {url!r})>"
+
+    def __getstate__(self) -> typing.Dict[str, typing.Any]:
+        return {
+            name: value
+            for name, value in self.__dict__.items()
+            if name not in ["extensions", "stream"]
+        }
 
-        self.headers = CaseInsensitiveDict()
-        if headers:
-            for header in headers.items():
-                # Raise exception on invalid header value.
-                check_header_validity(header)
-                name, value = header
-                self.headers[to_native_string(name)] = value
-
-    def prepare_body(self, data, files, json=None):
-        """Prepares the given HTTP body data."""
-
-        # Check if file, fo, generator, iterator.
-        # If not, run through normal process.
-
-        # Nottin' on you.
-        body = None
-        content_type = None
-
-        if not data and json is not None:
-            # urllib3 requires a bytes-like body. Python 2's json.dumps
-            # provides this natively, but Python 3 gives a Unicode string.
-            content_type = "application/json"
-
-            try:
-                body = complexjson.dumps(json, allow_nan=False)
-            except ValueError as ve:
-                raise InvalidJSONError(ve, request=self)
+    def __setstate__(self, state: typing.Dict[str, typing.Any]) -> None:
+        for name, value in state.items():
+            setattr(self, name, value)
+        self.extensions = {}
+        self.stream = UnattachedStream()
 
-            if not isinstance(body, bytes):
-                body = body.encode("utf-8")
 
-        is_stream = all(
-            [
-                hasattr(data, "__iter__"),
-                not isinstance(data, (basestring, list, tuple, Mapping)),
-            ]
-        )
+class Response:
+    def __init__(
+        self,
+        status_code: int,
+        *,
+        headers: typing.Optional[HeaderTypes] = None,
+        content: typing.Optional[ResponseContent] = None,
+        text: typing.Optional[str] = None,
+        html: typing.Optional[str] = None,
+        json: typing.Any = None,
+        stream: typing.Union[SyncByteStream, AsyncByteStream, None] = None,
+        request: typing.Optional[Request] = None,
+        extensions: typing.Optional[ResponseExtensions] = None,
+        history: typing.Optional[typing.List["Response"]] = None,
+        default_encoding: typing.Union[str, typing.Callable[[bytes], str]] = "utf-8",
+    ):
+        self.status_code = status_code
+        self.headers = Headers(headers)
 
-        if is_stream:
-            try:
-                length = super_len(data)
-            except (TypeError, AttributeError, UnsupportedOperation):
-                length = None
-
-            body = data
-
-            if getattr(body, "tell", None) is not None:
-                # Record the current file position before reading.
-                # This will allow us to rewind a file in the event
-                # of a redirect.
-                try:
-                    self._body_position = body.tell()
-                except OSError:
-                    # This differentiates from None, allowing us to catch
-                    # a failed `tell()` later when trying to rewind the body
-                    self._body_position = object()
-
-            if files:
-                raise NotImplementedError(
-                    "Streamed bodies and files are mutually exclusive."
-                )
+        self._request: typing.Optional[Request] = request
 
-            if length:
-                self.headers["Content-Length"] = builtin_str(length)
-            else:
-                self.headers["Transfer-Encoding"] = "chunked"
+        # When follow_redirects=False and a redirect is received,
+        # the client will set `response.next_request`.
+        self.next_request: typing.Optional[Request] = None
+
+        self.extensions = {} if extensions is None else extensions
+        self.history = [] if history is None else list(history)
+
+        self.is_closed = False
+        self.is_stream_consumed = False
+
+        self.default_encoding = default_encoding
+
+        if stream is None:
+            headers, stream = encode_response(content, text, html, json)
+            self._prepare(headers)
+            self.stream = stream
+            if isinstance(stream, ByteStream):
+                # Load the response body, except for streaming content.
+                self.read()
         else:
-            # Multi-part file uploads.
-            if files:
-                (body, content_type) = self._encode_files(files, data)
-            else:
-                if data:
-                    body = self._encode_params(data)
-                    if isinstance(data, basestring) or hasattr(data, "read"):
-                        content_type = None
-                    else:
-                        content_type = "application/x-www-form-urlencoded"
-
-            self.prepare_content_length(body)
-
-            # Add content-type if it wasn't explicitly provided.
-            if content_type and ("content-type" not in self.headers):
-                self.headers["Content-Type"] = content_type
-
-        self.body = body
-
-    def prepare_content_length(self, body):
-        """Prepare Content-Length header based on request method and body"""
-        if body is not None:
-            length = super_len(body)
-            if length:
-                # If length exists, set it. Otherwise, we fallback
-                # to Transfer-Encoding: chunked.
-                self.headers["Content-Length"] = builtin_str(length)
-        elif (
-            self.method not in ("GET", "HEAD")
-            and self.headers.get("Content-Length") is None
-        ):
-            # Set Content-Length to 0 for methods that can have a body
-            # but don't provide one. (i.e. not GET or HEAD)
-            self.headers["Content-Length"] = "0"
-
-    def prepare_auth(self, auth, url=""):
-        """Prepares the given HTTP auth data."""
-
-        # If no Auth is explicitly provided, extract it from the URL first.
-        if auth is None:
-            url_auth = get_auth_from_url(self.url)
-            auth = url_auth if any(url_auth) else None
-
-        if auth:
-            if isinstance(auth, tuple) and len(auth) == 2:
-                # special-case basic HTTP auth
-                auth = HTTPBasicAuth(*auth)
-
-            # Allow auth to make its changes.
-            r = auth(self)
-
-            # Update self to reflect the auth changes.
-            self.__dict__.update(r.__dict__)
-
-            # Recompute Content-Length
-            self.prepare_content_length(self.body)
-
-    def prepare_cookies(self, cookies):
-        """Prepares the given HTTP cookie data.
-
-        This function eventually generates a ``Cookie`` header from the
-        given cookies using cookielib. Due to cookielib's design, the header
-        will not be regenerated if it already exists, meaning this function
-        can only be called once for the life of the
-        :class:`PreparedRequest <PreparedRequest>` object. Any subsequent calls
-        to ``prepare_cookies`` will have no actual effect, unless the "Cookie"
-        header is removed beforehand.
+            # There's an important distinction between `Response(content=...)`,
+            # and `Response(stream=...)`.
+            #
+            # Using `content=...` implies automatically populated content headers,
+            # of either `Content-Length: ...` or `Transfer-Encoding: chunked`.
+            #
+            # Using `stream=...` will not automatically include any content headers.
+            #
+            # As an end-user you don't really need `stream=...`. It's only
+            # useful when creating response instances having received a stream
+            # from the transport API.
+            self.stream = stream
+
+        self._num_bytes_downloaded = 0
+
+    def _prepare(self, default_headers: typing.Dict[str, str]) -> None:
+        for key, value in default_headers.items():
+            # Ignore Transfer-Encoding if the Content-Length has been set explicitly.
+            if key.lower() == "transfer-encoding" and "content-length" in self.headers:
+                continue
+            self.headers.setdefault(key, value)
+
+    @property
+    def elapsed(self) -> datetime.timedelta:
         """
-        if isinstance(cookies, cookielib.CookieJar):
-            self._cookies = cookies
-        else:
-            self._cookies = cookiejar_from_dict(cookies)
+        Returns the time taken for the complete request/response
+        cycle to complete.
+        """
+        if not hasattr(self, "_elapsed"):
+            raise RuntimeError(
+                "'.elapsed' may only be accessed after the response "
+                "has been read or closed."
+            )
+        return self._elapsed
 
-        cookie_header = get_cookie_header(self._cookies, self)
-        if cookie_header is not None:
-            self.headers["Cookie"] = cookie_header
-
-    def prepare_hooks(self, hooks):
-        """Prepares the given hooks."""
-        # hooks can be passed as None to the prepare method and to this
-        # method. To prevent iterating over None, simply use an empty list
-        # if hooks is False-y
-        hooks = hooks or []
-        for event in hooks:
-            self.register_hook(event, hooks[event])
+    @elapsed.setter
+    def elapsed(self, elapsed: datetime.timedelta) -> None:
+        self._elapsed = elapsed
 
+    @property
+    def request(self) -> Request:
+        """
+        Returns the request instance associated to the current response.
+        """
+        if self._request is None:
+            raise RuntimeError(
+                "The request instance has not been set on this response."
+            )
+        return self._request
 
-class Response:
-    """The :class:`Response <Response>` object, which contains a
-    server's response to an HTTP request.
-    """
+    @request.setter
+    def request(self, value: Request) -> None:
+        self._request = value
 
-    __attrs__ = [
-        "_content",
-        "status_code",
-        "headers",
-        "url",
-        "history",
-        "encoding",
-        "reason",
-        "cookies",
-        "elapsed",
-        "request",
-    ]
-
-    def __init__(self):
-        self._content = False
-        self._content_consumed = False
-        self._next = None
-
-        #: Integer Code of responded HTTP Status, e.g. 404 or 200.
-        self.status_code = None
-
-        #: Case-insensitive Dictionary of Response Headers.
-        #: For example, ``headers['content-encoding']`` will return the
-        #: value of a ``'Content-Encoding'`` response header.
-        self.headers = CaseInsensitiveDict()
-
-        #: File-like object representation of response (for advanced usage).
-        #: Use of ``raw`` requires that ``stream=True`` be set on the request.
-        #: This requirement does not apply for use internally to HttpMax.
-        self.raw = None
-
-        #: Final URL location of Response.
-        self.url = None
-
-        #: Encoding to decode with when accessing r.text.
-        self.encoding = None
-
-        #: A list of :class:`Response <Response>` objects from
-        #: the history of the Request. Any redirect responses will end
-        #: up here. The list is sorted from the oldest to the most recent request.
-        self.history = []
-
-        #: Textual reason of responded HTTP Status, e.g. "Not Found" or "OK".
-        self.reason = None
-
-        #: A CookieJar of Cookies the server sent back.
-        self.cookies = cookiejar_from_dict({})
-
-        #: The amount of time elapsed between sending the request
-        #: and the arrival of the response (as a timedelta).
-        #: This property specifically measures the time taken between sending
-        #: the first byte of the request and finishing parsing the headers. It
-        #: is therefore unaffected by consuming the response content or the
-        #: value of the ``stream`` keyword argument.
-        self.elapsed = datetime.timedelta(0)
-
-        #: The :class:`PreparedRequest <PreparedRequest>` object to which this
-        #: is a response.
-        self.request = None
+    @property
+    def http_version(self) -> str:
+        try:
+            http_version: bytes = self.extensions["http_version"]
+        except KeyError:
+            return "HTTP/1.1"
+        else:
+            return http_version.decode("ascii", errors="ignore")
 
-    def __enter__(self):
-        return self
+    @property
+    def reason_phrase(self) -> str:
+        try:
+            reason_phrase: bytes = self.extensions["reason_phrase"]
+        except KeyError:
+            return codes.get_reason_phrase(self.status_code)
+        else:
+            return reason_phrase.decode("ascii", errors="ignore")
 
-    def __exit__(self, *args):
-        self.close()
+    @property
+    def url(self) -> URL:
+        """
+        Returns the URL for which the request was made.
+        """
+        return self.request.url
 
-    def __getstate__(self):
-        # Consume everything; accessing the content attribute makes
-        # sure the content has been fully read.
-        if not self._content_consumed:
-            self.content
+    @property
+    def content(self) -> bytes:
+        if not hasattr(self, "_content"):
+            raise ResponseNotRead()
+        return self._content
 
-        return {attr: getattr(self, attr, None) for attr in self.__attrs__}
+    @property
+    def text(self) -> str:
+        if not hasattr(self, "_text"):
+            content = self.content
+            if not content:
+                self._text = ""
+            else:
+                decoder = TextDecoder(encoding=self.encoding or "utf-8")
+                self._text = "".join([decoder.decode(self.content), decoder.flush()])
+        return self._text
 
-    def __setstate__(self, state):
-        for name, value in state.items():
-            setattr(self, name, value)
+    @property
+    def encoding(self) -> typing.Optional[str]:
+        """
+        Return an encoding to use for decoding the byte content into text.
+        The priority for determining this is given by...
 
-        # pickled objects do not have .raw
-        setattr(self, "_content_consumed", True)
-        setattr(self, "raw", None)
+        * `.encoding = <>` has been set explicitly.
+        * The encoding as specified by the charset parameter in the Content-Type header.
+        * The encoding as determined by `default_encoding`, which may either be
+          a string like "utf-8" indicating the encoding to use, or may be a callable
+          which enables charset autodetection.
+        """
+        if not hasattr(self, "_encoding"):
+            encoding = self.charset_encoding
+            if encoding is None or not is_known_encoding(encoding):
+                if isinstance(self.default_encoding, str):
+                    encoding = self.default_encoding
+                elif hasattr(self, "_content"):
+                    encoding = self.default_encoding(self._content)
+            self._encoding = encoding or "utf-8"
+        return self._encoding
+
+    @encoding.setter
+    def encoding(self, value: str) -> None:
+        self._encoding = value
 
-    def __repr__(self):
-        return f"<Response [{self.status_code}]>"
+    @property
+    def charset_encoding(self) -> typing.Optional[str]:
+        """
+        Return the encoding, as specified by the Content-Type header.
+        """
+        content_type = self.headers.get("Content-Type")
+        if content_type is None:
+            return None
 
-    def __bool__(self):
-        """Returns True if :attr:`status_code` is less than 400.
+        return parse_content_type_charset(content_type)
 
-        This attribute checks if the status code of the response is between
-        400 and 600 to see if there was a client error or a server error. If
-        the status code, is between 200 and 400, this will return True. This
-        is **not** a check to see if the response code is ``200 OK``.
+    def _get_content_decoder(self) -> ContentDecoder:
+        """
+        Returns a decoder instance which can be used to decode the raw byte
+        content, depending on the Content-Encoding used in the response.
         """
-        return self.ok
+        if not hasattr(self, "_decoder"):
+            decoders: typing.List[ContentDecoder] = []
+            values = self.headers.get_list("content-encoding", split_commas=True)
+            for value in values:
+                value = value.strip().lower()
+                try:
+                    decoder_cls = SUPPORTED_DECODERS[value]
+                    decoders.append(decoder_cls())
+                except KeyError:
+                    continue
+
+            if len(decoders) == 1:
+                self._decoder = decoders[0]
+            elif len(decoders) > 1:
+                self._decoder = MultiDecoder(children=decoders)
+            else:
+                self._decoder = IdentityDecoder()
 
-    def __nonzero__(self):
-        """Returns True if :attr:`status_code` is less than 400.
+        return self._decoder
 
-        This attribute checks if the status code of the response is between
-        400 and 600 to see if there was a client error or a server error. If
-        the status code, is between 200 and 400, this will return True. This
-        is **not** a check to see if the response code is ``200 OK``.
+    @property
+    def is_informational(self) -> bool:
+        """
+        A property which is `True` for 1xx status codes, `False` otherwise.
         """
-        return self.ok
+        return codes.is_informational(self.status_code)
 
-    def __iter__(self):
-        """Allows you to use a response as an iterator."""
-        return self.iter_content(128)
+    @property
+    def is_success(self) -> bool:
+        """
+        A property which is `True` for 2xx status codes, `False` otherwise.
+        """
+        return codes.is_success(self.status_code)
 
     @property
-    def ok(self):
-        """Returns True if :attr:`status_code` is less than 400, False if not.
+    def is_redirect(self) -> bool:
+        """
+        A property which is `True` for 3xx status codes, `False` otherwise.
 
-        This attribute checks if the status code of the response is between
-        400 and 600 to see if there was a client error or a server error. If
-        the status code is between 200 and 400, this will return True. This
-        is **not** a check to see if the response code is ``200 OK``.
+        Note that not all responses with a 3xx status code indicate a URL redirect.
+
+        Use `response.has_redirect_location` to determine responses with a properly
+        formed URL redirection.
         """
-        try:
-            self.raise_for_status()
-        except HTTPError:
-            return False
-        return True
+        return codes.is_redirect(self.status_code)
 
     @property
-    def is_redirect(self):
-        """True if this Response is a well-formed HTTP redirect that could have
-        been processed automatically (by :meth:`Session.resolve_redirects`).
+    def is_client_error(self) -> bool:
+        """
+        A property which is `True` for 4xx status codes, `False` otherwise.
         """
-        return "location" in self.headers and self.status_code in REDIRECT_STATI
+        return codes.is_client_error(self.status_code)
 
     @property
-    def is_permanent_redirect(self):
-        """True if this Response one of the permanent versions of redirect."""
-        return "location" in self.headers and self.status_code in (
-            codes.moved_permanently,
-            codes.permanent_redirect,
-        )
+    def is_server_error(self) -> bool:
+        """
+        A property which is `True` for 5xx status codes, `False` otherwise.
+        """
+        return codes.is_server_error(self.status_code)
 
     @property
-    def next(self):
-        """Returns a PreparedRequest for the next request in a redirect chain, if there is one."""
-        return self._next
-
-    @property
-    def apparent_encoding(self):
-        """The apparent encoding, provided by the charset_normalizer or chardet libraries."""
-        return chardet.detect(self.content)["encoding"]
-
-    def iter_content(self, chunk_size=1, decode_unicode=False):
-        """Iterates over the response data.  When stream=True is set on the
-        request, this avoids reading the content at once into memory for
-        large responses.  The chunk size is the number of bytes it should
-        read into memory.  This is not necessarily the length of each item
-        returned as decoding can take place.
-
-        chunk_size must be of type int or None. A value of None will
-        function differently depending on the value of `stream`.
-        stream=True will read data as it arrives in whatever size the
-        chunks are received. If stream=False, data is returned as
-        a single chunk.
-
-        If decode_unicode is True, content will be decoded using the best
-        available encoding based on the response.
-        """
-
-        def generate():
-            # Special case for urllib3.
-            if hasattr(self.raw, "stream"):
-                try:
-                    yield from self.raw.stream(chunk_size, decode_content=True)
-                except ProtocolError as e:
-                    raise ChunkedEncodingError(e)
-                except DecodeError as e:
-                    raise ContentDecodingError(e)
-                except ReadTimeoutError as e:
-                    raise ConnectionError(e)
-                except SSLError as e:
-                    raise HttpMaxSSLError(e)
-            else:
-                # Standard file-like object.
-                while True:
-                    chunk = self.raw.read(chunk_size)
-                    if not chunk:
-                        break
-                    yield chunk
+    def is_error(self) -> bool:
+        """
+        A property which is `True` for 4xx and 5xx status codes, `False` otherwise.
+        """
+        return codes.is_error(self.status_code)
 
-            self._content_consumed = True
+    @property
+    def has_redirect_location(self) -> bool:
+        """
+        Returns True for 3xx responses with a properly formed URL redirection,
+        `False` otherwise.
+        """
+        return (
+            self.status_code
+            in (
+                # 301 (Cacheable redirect. Method may change to GET.)
+                codes.MOVED_PERMANENTLY,
+                # 302 (Uncacheable redirect. Method may change to GET.)
+                codes.FOUND,
+                # 303 (Client should make a GET or HEAD request.)
+                codes.SEE_OTHER,
+                # 307 (Equiv. 302, but retain method)
+                codes.TEMPORARY_REDIRECT,
+                # 308 (Equiv. 301, but retain method)
+                codes.PERMANENT_REDIRECT,
+            )
+            and "Location" in self.headers
+        )
 
-        if self._content_consumed and isinstance(self._content, bool):
-            raise StreamConsumedError()
-        elif chunk_size is not None and not isinstance(chunk_size, int):
-            raise TypeError(
-                f"chunk_size must be an int, it is instead a {type(chunk_size)}."
+    def raise_for_status(self) -> None:
+        """
+        Raise the `HTTPStatusError` if one occurred.
+        """
+        request = self._request
+        if request is None:
+            raise RuntimeError(
+                "Cannot call `raise_for_status` as the request "
+                "instance has not been set on this response."
             )
-        # simulate reading small chunks of the content
-        reused_chunks = iter_slices(self._content, chunk_size)
 
-        stream_chunks = generate()
+        if self.is_success:
+            return
 
-        chunks = reused_chunks if self._content_consumed else stream_chunks
+        if self.has_redirect_location:
+            message = (
+                "{error_type} '{0.status_code} {0.reason_phrase}' for url '{0.url}'\n"
+                "Redirect location: '{0.headers[location]}'\n"
+                "For more information check: https://httpstatuses.com/{0.status_code}"
+            )
+        else:
+            message = (
+                "{error_type} '{0.status_code} {0.reason_phrase}' for url '{0.url}'\n"
+                "For more information check: https://httpstatuses.com/{0.status_code}"
+            )
 
-        if decode_unicode:
-            chunks = stream_decode_response_unicode(chunks, self)
+        status_class = self.status_code // 100
+        error_types = {
+            1: "Informational response",
+            3: "Redirect response",
+            4: "Client error",
+            5: "Server error",
+        }
+        error_type = error_types.get(status_class, "Invalid status code")
+        message = message.format(self, error_type=error_type)
+        raise HTTPStatusError(message, request=request, response=self)
 
-        return chunks
+    def json(self, **kwargs: typing.Any) -> typing.Any:
+        if self.charset_encoding is None and self.content and len(self.content) > 3:
+            encoding = guess_json_utf(self.content)
+            if encoding is not None:
+                return jsonlib.loads(self.content.decode(encoding), **kwargs)
+        return jsonlib.loads(self.text, **kwargs)
 
-    def iter_lines(
-        self, chunk_size=ITER_CHUNK_SIZE, decode_unicode=False, delimiter=None
-    ):
-        """Iterates over the response data, one line at a time.  When
-        stream=True is set on the request, this avoids reading the
-        content at once into memory for large responses.
+    @property
+    def cookies(self) -> "Cookies":
+        if not hasattr(self, "_cookies"):
+            self._cookies = Cookies()
+            self._cookies.extract_cookies(self)
+        return self._cookies
 
-        .. note:: This method is not reentrant safe.
+    @property
+    def links(self) -> typing.Dict[typing.Optional[str], typing.Dict[str, str]]:
+        """
+        Returns the parsed header links of the response, if any
         """
+        header = self.headers.get("link")
+        ldict = {}
+        if header:
+            links = parse_header_links(header)
+            for link in links:
+                key = link.get("rel") or link.get("url")
+                ldict[key] = link
+        return ldict
+
+    @property
+    def num_bytes_downloaded(self) -> int:
+        return self._num_bytes_downloaded
 
-        pending = None
+    def __repr__(self) -> str:
+        return f"<Response [{self.status_code} {self.reason_phrase}]>"
 
-        for chunk in self.iter_content(
-            chunk_size=chunk_size, decode_unicode=decode_unicode
-        ):
+    def __getstate__(self) -> typing.Dict[str, typing.Any]:
+        return {
+            name: value
+            for name, value in self.__dict__.items()
+            if name not in ["extensions", "stream", "is_closed", "_decoder"]
+        }
 
-            if pending is not None:
-                chunk = pending + chunk
+    def __setstate__(self, state: typing.Dict[str, typing.Any]) -> None:
+        for name, value in state.items():
+            setattr(self, name, value)
+        self.is_closed = True
+        self.extensions = {}
+        self.stream = UnattachedStream()
 
-            if delimiter:
-                lines = chunk.split(delimiter)
-            else:
-                lines = chunk.splitlines()
+    def read(self) -> bytes:
+        """
+        Read and return the response content.
+        """
+        if not hasattr(self, "_content"):
+            self._content = b"".join(self.iter_bytes())
+        return self._content
 
-            if lines and lines[-1] and chunk and lines[-1][-1] == chunk[-1]:
-                pending = lines.pop()
-            else:
-                pending = None
+    def iter_bytes(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.Iterator[bytes]:
+        """
+        A byte-iterator over the decoded response content.
+        This allows us to handle gzip, deflate, and brotli encoded responses.
+        """
+        if hasattr(self, "_content"):
+            chunk_size = len(self._content) if chunk_size is None else chunk_size
+            for i in range(0, len(self._content), max(chunk_size, 1)):
+                yield self._content[i : i + chunk_size]
+        else:
+            decoder = self._get_content_decoder()
+            chunker = ByteChunker(chunk_size=chunk_size)
+            with request_context(request=self._request):
+                for raw_bytes in self.iter_raw():
+                    decoded = decoder.decode(raw_bytes)
+                    for chunk in chunker.decode(decoded):
+                        yield chunk
+                decoded = decoder.flush()
+                for chunk in chunker.decode(decoded):
+                    yield chunk  # pragma: no cover
+                for chunk in chunker.flush():
+                    yield chunk
 
-            yield from lines
+    def iter_text(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.Iterator[str]:
+        """
+        A str-iterator over the decoded response content
+        that handles both gzip, deflate, etc but also detects the content's
+        string encoding.
+        """
+        decoder = TextDecoder(encoding=self.encoding or "utf-8")
+        chunker = TextChunker(chunk_size=chunk_size)
+        with request_context(request=self._request):
+            for byte_content in self.iter_bytes():
+                text_content = decoder.decode(byte_content)
+                for chunk in chunker.decode(text_content):
+                    yield chunk
+            text_content = decoder.flush()
+            for chunk in chunker.decode(text_content):
+                yield chunk
+            for chunk in chunker.flush():
+                yield chunk
+
+    def iter_lines(self) -> typing.Iterator[str]:
+        decoder = LineDecoder()
+        with request_context(request=self._request):
+            for text in self.iter_text():
+                for line in decoder.decode(text):
+                    yield line
+            for line in decoder.flush():
+                yield line
+
+    def iter_raw(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.Iterator[bytes]:
+        """
+        A byte-iterator over the raw response content.
+        """
+        if self.is_stream_consumed:
+            raise StreamConsumed()
+        if self.is_closed:
+            raise StreamClosed()
+        if not isinstance(self.stream, SyncByteStream):
+            raise RuntimeError("Attempted to call a sync iterator on an async stream.")
+
+        self.is_stream_consumed = True
+        self._num_bytes_downloaded = 0
+        chunker = ByteChunker(chunk_size=chunk_size)
+
+        with request_context(request=self._request):
+            for raw_stream_bytes in self.stream:
+                self._num_bytes_downloaded += len(raw_stream_bytes)
+                for chunk in chunker.decode(raw_stream_bytes):
+                    yield chunk
 
-        if pending is not None:
-            yield pending
+        for chunk in chunker.flush():
+            yield chunk
 
-    @property
-    def content(self):
-        """Content of the response, in bytes."""
+        self.close()
 
-        if self._content is False:
-            # Read the contents.
-            if self._content_consumed:
-                raise RuntimeError("The content for this response was already consumed")
+    def close(self) -> None:
+        """
+        Close the response and release the connection.
+        Automatically called if the response body is read to completion.
+        """
+        if not isinstance(self.stream, SyncByteStream):
+            raise RuntimeError("Attempted to call an sync close on an async stream.")
 
-            if self.status_code == 0 or self.raw is None:
-                self._content = None
-            else:
-                self._content = b"".join(self.iter_content(CONTENT_CHUNK_SIZE)) or b""
+        if not self.is_closed:
+            self.is_closed = True
+            with request_context(request=self._request):
+                self.stream.close()
 
-        self._content_consumed = True
-        # don't need to release the connection; that's been handled by urllib3
-        # since we exhausted the data.
+    async def aread(self) -> bytes:
+        """
+        Read and return the response content.
+        """
+        if not hasattr(self, "_content"):
+            self._content = b"".join([part async for part in self.aiter_bytes()])
         return self._content
 
-    @property
-    def text(self):
-        """Content of the response, in unicode.
-
-        If Response.encoding is None, encoding will be guessed using
-        ``charset_normalizer`` or ``chardet``.
+    async def aiter_bytes(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.AsyncIterator[bytes]:
+        """
+        A byte-iterator over the decoded response content.
+        This allows us to handle gzip, deflate, and brotli encoded responses.
+        """
+        if hasattr(self, "_content"):
+            chunk_size = len(self._content) if chunk_size is None else chunk_size
+            for i in range(0, len(self._content), max(chunk_size, 1)):
+                yield self._content[i : i + chunk_size]
+        else:
+            decoder = self._get_content_decoder()
+            chunker = ByteChunker(chunk_size=chunk_size)
+            with request_context(request=self._request):
+                async for raw_bytes in self.aiter_raw():
+                    decoded = decoder.decode(raw_bytes)
+                    for chunk in chunker.decode(decoded):
+                        yield chunk
+                decoded = decoder.flush()
+                for chunk in chunker.decode(decoded):
+                    yield chunk  # pragma: no cover
+                for chunk in chunker.flush():
+                    yield chunk
 
-        The encoding of the response content is determined based solely on HTTP
-        headers, following RFC 2616 to the letter. If you can take advantage of
-        non-HTTP knowledge to make a better guess at the encoding, you should
-        set ``r.encoding`` appropriately before accessing this property.
+    async def aiter_text(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.AsyncIterator[str]:
+        """
+        A str-iterator over the decoded response content
+        that handles both gzip, deflate, etc but also detects the content's
+        string encoding.
         """
+        decoder = TextDecoder(encoding=self.encoding or "utf-8")
+        chunker = TextChunker(chunk_size=chunk_size)
+        with request_context(request=self._request):
+            async for byte_content in self.aiter_bytes():
+                text_content = decoder.decode(byte_content)
+                for chunk in chunker.decode(text_content):
+                    yield chunk
+            text_content = decoder.flush()
+            for chunk in chunker.decode(text_content):
+                yield chunk
+            for chunk in chunker.flush():
+                yield chunk
+
+    async def aiter_lines(self) -> typing.AsyncIterator[str]:
+        decoder = LineDecoder()
+        with request_context(request=self._request):
+            async for text in self.aiter_text():
+                for line in decoder.decode(text):
+                    yield line
+            for line in decoder.flush():
+                yield line
+
+    async def aiter_raw(
+        self, chunk_size: typing.Optional[int] = None
+    ) -> typing.AsyncIterator[bytes]:
+        """
+        A byte-iterator over the raw response content.
+        """
+        if self.is_stream_consumed:
+            raise StreamConsumed()
+        if self.is_closed:
+            raise StreamClosed()
+        if not isinstance(self.stream, AsyncByteStream):
+            raise RuntimeError("Attempted to call an async iterator on an sync stream.")
+
+        self.is_stream_consumed = True
+        self._num_bytes_downloaded = 0
+        chunker = ByteChunker(chunk_size=chunk_size)
+
+        with request_context(request=self._request):
+            async for raw_stream_bytes in self.stream:
+                self._num_bytes_downloaded += len(raw_stream_bytes)
+                for chunk in chunker.decode(raw_stream_bytes):
+                    yield chunk
 
-        # Try charset from content-type
-        content = None
-        encoding = self.encoding
+        for chunk in chunker.flush():
+            yield chunk
 
-        if not self.content:
-            return ""
+        await self.aclose()
 
-        # Fallback to auto-detected encoding.
-        if self.encoding is None:
-            encoding = self.apparent_encoding
+    async def aclose(self) -> None:
+        """
+        Close the response and release the connection.
+        Automatically called if the response body is read to completion.
+        """
+        if not isinstance(self.stream, AsyncByteStream):
+            raise RuntimeError("Attempted to call an async close on an sync stream.")
+
+        if not self.is_closed:
+            self.is_closed = True
+            with request_context(request=self._request):
+                await self.stream.aclose()
 
-        # Decode unicode from given encoding.
-        try:
-            content = str(self.content, encoding, errors="replace")
-        except (LookupError, TypeError):
-            # A LookupError is raised if the encoding was not found which could
-            # indicate a misspelling or similar mistake.
-            #
-            # A TypeError can be raised if encoding is None
-            #
-            # So we try blindly encoding.
-            content = str(self.content, errors="replace")
 
-        return content
+class Cookies(typing.MutableMapping[str, str]):
+    """
+    HTTP Cookies, as a mutable mapping.
+    """
 
-    async def json(self, **kwargs):
-        r"""Returns the json-encoded content of a response, if any.
+    def __init__(self, cookies: typing.Optional[CookieTypes] = None) -> None:
+        if cookies is None or isinstance(cookies, dict):
+            self.jar = CookieJar()
+            if isinstance(cookies, dict):
+                for key, value in cookies.items():
+                    self.set(key, value)
+        elif isinstance(cookies, list):
+            self.jar = CookieJar()
+            for key, value in cookies:
+                self.set(key, value)
+        elif isinstance(cookies, Cookies):
+            self.jar = CookieJar()
+            for cookie in cookies.jar:
+                self.jar.set_cookie(cookie)
+        else:
+            self.jar = cookies
 
-        :param \*\*kwargs: Optional arguments that ``json.loads`` takes.
-        :raises HttpMax.exceptions.JSONDecodeError: If the response body does not
-            contain valid json.
+    def extract_cookies(self, response: Response) -> None:
+        """
+        Loads any cookies based on the response `Set-Cookie` headers.
         """
+        urllib_response = self._CookieCompatResponse(response)
+        urllib_request = self._CookieCompatRequest(response.request)
 
-        if not self.encoding and self.content and len(self.content) > 3:
-            # No encoding set. JSON RFC 4627 section 3 states we should expect
-            # UTF-8, -16 or -32. Detect which one to use; If the detection or
-            # decoding fails, fall back to `self.text` (using charset_normalizer to make
-            # a best guess).
-            encoding = guess_json_utf(self.content)
-            if encoding is not None:
-                try:
-                    return complexjson.loads(self.content.decode(encoding), **kwargs)
-                except UnicodeDecodeError:
-                    # Wrong UTF codec detected; usually because it's not UTF-8
-                    # but some other 8-bit codec.  This is an RFC violation,
-                    # and the server didn't bother to tell us what codec *was*
-                    # used.
-                    pass
-                except JSONDecodeError as e:
-                    raise HttpMaxJSONDecodeError(e.msg, e.doc, e.pos)
+        self.jar.extract_cookies(urllib_response, urllib_request)  # type: ignore
 
-        try:
-            return complexjson.loads(self.text, **kwargs)
-        except JSONDecodeError as e:
-            # Catch JSON-related errors and raise as HttpMax.JSONDecodeError
-            # This aliases json.JSONDecodeError and simplejson.JSONDecodeError
-            raise HttpMaxJSONDecodeError(e.msg, e.doc, e.pos)
+    def set_cookie_header(self, request: Request) -> None:
+        """
+        Sets an appropriate 'Cookie:' HTTP header on the `Request`.
+        """
+        urllib_request = self._CookieCompatRequest(request)
+        self.jar.add_cookie_header(urllib_request)
 
-    @property
-    def links(self):
-        """Returns the parsed header links of the response, if any."""
+    def set(self, name: str, value: str, domain: str = "", path: str = "/") -> None:
+        """
+        Set a cookie value by name. May optionally include domain and path.
+        """
+        kwargs = {
+            "version": 0,
+            "name": name,
+            "value": value,
+            "port": None,
+            "port_specified": False,
+            "domain": domain,
+            "domain_specified": bool(domain),
+            "domain_initial_dot": domain.startswith("."),
+            "path": path,
+            "path_specified": bool(path),
+            "secure": False,
+            "expires": None,
+            "discard": True,
+            "comment": None,
+            "comment_url": None,
+            "rest": {"HttpOnly": None},
+            "rfc2109": False,
+        }
+        cookie = Cookie(**kwargs)  # type: ignore
+        self.jar.set_cookie(cookie)
 
-        header = self.headers.get("link")
+    def get(  # type: ignore
+        self,
+        name: str,
+        default: typing.Optional[str] = None,
+        domain: typing.Optional[str] = None,
+        path: typing.Optional[str] = None,
+    ) -> typing.Optional[str]:
+        """
+        Get a cookie by name. May optionally include domain and path
+        in order to specify exactly which cookie to retrieve.
+        """
+        value = None
+        for cookie in self.jar:
+            if cookie.name == name:
+                if domain is None or cookie.domain == domain:
+                    if path is None or cookie.path == path:
+                        if value is not None:
+                            message = f"Multiple cookies exist with name={name}"
+                            raise CookieConflict(message)
+                        value = cookie.value
+
+        if value is None:
+            return default
+        return value
 
-        resolved_links = {}
+    def delete(
+        self,
+        name: str,
+        domain: typing.Optional[str] = None,
+        path: typing.Optional[str] = None,
+    ) -> None:
+        """
+        Delete a cookie by name. May optionally include domain and path
+        in order to specify exactly which cookie to delete.
+        """
+        if domain is not None and path is not None:
+            return self.jar.clear(domain, path, name)
 
-        if header:
-            links = parse_header_links(header)
+        remove = [
+            cookie
+            for cookie in self.jar
+            if cookie.name == name
+            and (domain is None or cookie.domain == domain)
+            and (path is None or cookie.path == path)
+        ]
+
+        for cookie in remove:
+            self.jar.clear(cookie.domain, cookie.path, cookie.name)
+
+    def clear(
+        self, domain: typing.Optional[str] = None, path: typing.Optional[str] = None
+    ) -> None:
+        """
+        Delete all cookies. Optionally include a domain and path in
+        order to only delete a subset of all the cookies.
+        """
+        args = []
+        if domain is not None:
+            args.append(domain)
+        if path is not None:
+            assert domain is not None
+            args.append(path)
+        self.jar.clear(*args)
+
+    def update(self, cookies: typing.Optional[CookieTypes] = None) -> None:  # type: ignore
+        cookies = Cookies(cookies)
+        for cookie in cookies.jar:
+            self.jar.set_cookie(cookie)
+
+    def __setitem__(self, name: str, value: str) -> None:
+        return self.set(name, value)
+
+    def __getitem__(self, name: str) -> str:
+        value = self.get(name)
+        if value is None:
+            raise KeyError(name)
+        return value
+
+    def __delitem__(self, name: str) -> None:
+        return self.delete(name)
 
-            for link in links:
-                key = link.get("rel") or link.get("url")
-                resolved_links[key] = link
+    def __len__(self) -> int:
+        return len(self.jar)
 
-        return resolved_links
+    def __iter__(self) -> typing.Iterator[str]:
+        return (cookie.name for cookie in self.jar)
 
-    def raise_for_status(self):
-        """Raises :class:`HTTPError`, if one occurred."""
+    def __bool__(self) -> bool:
+        for _ in self.jar:
+            return True
+        return False
 
-        http_error_msg = ""
-        if isinstance(self.reason, bytes):
-            # We attempt to decode utf-8 first because some servers
-            # choose to localize their reason strings. If the string
-            # isn't utf-8, we fall back to iso-8859-1 for all other
-            # encodings. (See PR #3538)
-            try:
-                reason = self.reason.decode("utf-8")
-            except UnicodeDecodeError:
-                reason = self.reason.decode("iso-8859-1")
-        else:
-            reason = self.reason
+    def __repr__(self) -> str:
+        cookies_repr = ", ".join(
+            [
+                f"<Cookie {cookie.name}={cookie.value} for {cookie.domain} />"
+                for cookie in self.jar
+            ]
+        )
 
-        if 400 <= self.status_code < 500:
-            http_error_msg = (
-                f"{self.status_code} Client Error: {reason} for url: {self.url}"
-            )
+        return f"<Cookies[{cookies_repr}]>"
 
-        elif 500 <= self.status_code < 600:
-            http_error_msg = (
-                f"{self.status_code} Server Error: {reason} for url: {self.url}"
-            )
+    class _CookieCompatRequest(urllib.request.Request):
+        """
+        Wraps a `Request` instance up in a compatibility interface suitable
+        for use with `CookieJar` operations.
+        """
 
-        if http_error_msg:
-            raise HTTPError(http_error_msg, response=self)
+        def __init__(self, request: Request) -> None:
+            super().__init__(
+                url=str(request.url),
+                headers=dict(request.headers),
+                method=request.method,
+            )
+            self.request = request
 
-    def close(self):
-        """Releases the connection back to the pool. Once this method has been
-        called the underlying ``raw`` object must not be accessed again.
+        def add_unredirected_header(self, key: str, value: str) -> None:
+            super().add_unredirected_header(key, value)
+            self.request.headers[key] = value
 
-        *Note: Should not normally need to be called explicitly.*
+    class _CookieCompatResponse:
         """
-        if not self._content_consumed:
-            self.raw.close()
+        Wraps a `Request` instance up in a compatibility interface suitable
+        for use with `CookieJar` operations.
+        """
+
+        def __init__(self, response: Response):
+            self.response = response
 
-        release_conn = getattr(self.raw, "release_conn", None)
-        if release_conn is not None:
-            release_conn()
+        def info(self) -> email.message.Message:
+            info = email.message.Message()
+            for key, value in self.response.headers.multi_items():
+                # Note that setting `info[key]` here is an "append" operation,
+                # not a "replace" operation.
+                # https://docs.python.org/3/library/email.compat32-message.html#email.message.Message.__setitem__
+                info[key] = value
+            return info
```

### Comparing `HttpMax-1.1/HttpMax.egg-info/PKG-INFO` & `HttpMax-1.2/HttpMax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HttpMax
-Version: 1.1
+Version: 1.2
 Summary: Python HTTP Client for All.
 Home-page: https://github.com/shayanheidari01/HttpMax
 Author: Shayan Heidari
 Author-email: me@shayanheidari.info
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/shayanheidari01/HttpMax
 Project-URL: Source, https://github.com/shayanheidari01/HttpMax
@@ -24,17 +24,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: security
+Provides-Extra: brotli
+Provides-Extra: cli
+Provides-Extra: http2
 Provides-Extra: socks
-Provides-Extra: use_chardet_on_py3
 License-File: LICENSE
 
 # HttpMax
 
 **HttpMax** is a simple, asynchronous, fast and beautiful HTTP library.
 
 ```python
```

### Comparing `HttpMax-1.1/HttpMax.egg-info/SOURCES.txt` & `HttpMax-1.2/HttpMax.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE
 README.md
 setup.py
 HttpMax/__init__.py
 HttpMax/__version__.py
-HttpMax/_internal_utils.py
-HttpMax/adapters.py
-HttpMax/api.py
-HttpMax/auth.py
-HttpMax/certs.py
-HttpMax/compat.py
-HttpMax/cookies.py
-HttpMax/exceptions.py
-HttpMax/help.py
-HttpMax/hooks.py
-HttpMax/models.py
-HttpMax/packages.py
-HttpMax/sessions.py
-HttpMax/status_codes.py
-HttpMax/structures.py
-HttpMax/utils.py
+HttpMax/_api.py
+HttpMax/_auth.py
+HttpMax/_client.py
+HttpMax/_compat.py
+HttpMax/_config.py
+HttpMax/_content.py
+HttpMax/_decoders.py
+HttpMax/_exceptions.py
+HttpMax/_main.py
+HttpMax/_models.py
+HttpMax/_multipart.py
+HttpMax/_status_codes.py
+HttpMax/_types.py
+HttpMax/_urlparse.py
+HttpMax/_urls.py
+HttpMax/_utils.py
 HttpMax.egg-info/PKG-INFO
 HttpMax.egg-info/SOURCES.txt
 HttpMax.egg-info/dependency_links.txt
 HttpMax.egg-info/not-zip-safe
 HttpMax.egg-info/requires.txt
 HttpMax.egg-info/top_level.txt
```

### Comparing `HttpMax-1.1/LICENSE` & `HttpMax-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HttpMax-1.1/PKG-INFO` & `HttpMax-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HttpMax
-Version: 1.1
+Version: 1.2
 Summary: Python HTTP Client for All.
 Home-page: https://github.com/shayanheidari01/HttpMax
 Author: Shayan Heidari
 Author-email: me@shayanheidari.info
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/shayanheidari01/HttpMax
 Project-URL: Source, https://github.com/shayanheidari01/HttpMax
@@ -24,17 +24,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-Provides-Extra: security
+Provides-Extra: brotli
+Provides-Extra: cli
+Provides-Extra: http2
 Provides-Extra: socks
-Provides-Extra: use_chardet_on_py3
 License-File: LICENSE
 
 # HttpMax
 
 **HttpMax** is a simple, asynchronous, fast and beautiful HTTP library.
 
 ```python
```

### Comparing `HttpMax-1.1/README.md` & `HttpMax-1.2/README.md`

 * *Files identical despite different names*

### Comparing `HttpMax-1.1/setup.py` & `HttpMax-1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,25 @@
         """
 ==========================
 Unsupported Python version
 ==========================
 This version of HttpMax requires at least Python {}.{}, but
 you're trying to install it on Python {}.{}. To resolve this,
 consider upgrading to a supported Python version.
-
-If you can't upgrade your Python version, you'll need to
-pin to an older version of HttpMax (<2.28).
 """.format(
             *(REQUIRED_PYTHON + CURRENT_PYTHON)
         )
     )
     sys.exit(1)
 
 requires = [
-    "charset_normalizer>=2,<4",
-    "idna>=2.5,<4",
-    "urllib3>=1.21.1,<1.27",
-    "certifi>=2017.4.17",
+    'certifi',
+    'httpcore>=0.15.0,<0.18.0',
+    'idna',
+    'sniffio',
 ]
 
 about = {}
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "HttpMax", "__version__.py"), "r", "utf-8") as f:
     exec(f.read(), about)
 
@@ -48,15 +45,15 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     packages=["HttpMax"],
     package_data={"": ["LICENSE", "NOTICE"]},
-    package_dir={"requests": "requests"},
+    package_dir={"HttpMax": "HttpMax"},
     include_package_data=True,
     python_requires=">=3.7, <4",
     install_requires=requires,
     license=about["__license__"],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -75,16 +72,24 @@
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries",
     ],
     extras_require={
-        "security": [],
-        "socks": ["PySocks>=1.5.6, !=1.5.7"],
-        "use_chardet_on_py3": ["chardet>=3.0.2,<6"],
+        'brotli': [
+            'brotli; platform_python_implementation == \'CPython\'',
+            'brotlicffi; platform_python_implementation != \'CPython\'',
+            ],
+        'cli': [
+            'click==8.*',
+            'pygments==2.*',
+            'rich>=10,<14',
+            ],
+        'http2': ['h2>=3,<5'],
+        'socks': ['socksio==1.*']
     },
     project_urls={
         "Documentation": "https://github.com/shayanheidari01/HttpMax",
         "Source": "https://github.com/shayanheidari01/HttpMax",
     },
 )
```

