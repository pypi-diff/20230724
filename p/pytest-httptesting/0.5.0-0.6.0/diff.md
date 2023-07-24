# Comparing `tmp/pytest_httptesting-0.5.0.tar.gz` & `tmp/pytest_httptesting-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httptesting-0.5.0.tar", max compression
+gzip compressed data, was "pytest_httptesting-0.6.0.tar", max compression
```

## Comparing `pytest_httptesting-0.5.0.tar` & `pytest_httptesting-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1064 2022-11-13 16:42:42.780000 pytest_httptesting-0.5.0/LICENSE
--rw-r--r--   0        0        0     4049 2023-06-05 21:03:36.750000 pytest_httptesting-0.5.0/README.md
--rw-r--r--   0        0        0      628 2023-06-03 11:58:22.720000 pytest_httptesting-0.5.0/http_testing/__init__.py
--rw-r--r--   0        0        0        0 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/__init__.py
--rw-r--r--   0        0        0      567 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/assert_element_checker_base.py
--rw-r--r--   0        0        0     1354 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/assertion_attribute_base.py
--rw-r--r--   0        0        0     1587 2022-12-08 23:04:34.980000 pytest_httptesting-0.5.0/http_testing/assertion_elements/content_assertion.py
--rw-r--r--   0        0        0     2888 2023-06-03 11:39:49.730000 pytest_httptesting-0.5.0/http_testing/assertion_elements/cookies_assertion.py
--rw-r--r--   0        0        0     1601 2022-12-08 23:04:34.980000 pytest_httptesting-0.5.0/http_testing/assertion_elements/headers_assertion.py
--rw-r--r--   0        0        0      728 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertion_elements/status_code_assertion.py
--rw-r--r--   0        0        0     1316 2022-11-13 15:15:16.890000 pytest_httptesting-0.5.0/http_testing/assertions.py
--rw-r--r--   0        0        0       79 2023-04-19 19:55:13.180000 pytest_httptesting-0.5.0/http_testing/cookie.py
--rw-r--r--   0        0        0      259 2023-04-19 19:55:13.180000 pytest_httptesting-0.5.0/http_testing/http_client_configuration.py
--rw-r--r--   0        0        0     2872 2023-07-09 19:31:42.572186 pytest_httptesting-0.5.0/http_testing/page_checker.py
--rw-r--r--   0        0        0     1217 2023-06-03 11:39:42.590000 pytest_httptesting-0.5.0/http_testing/plugin.py
--rw-r--r--   0        0        0      709 2023-06-03 11:48:20.280000 pytest_httptesting-0.5.0/http_testing/validators.py
--rw-r--r--   0        0        0      705 2023-07-09 19:35:09.342186 pytest_httptesting-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 pytest_httptesting-0.5.0/setup.py
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 pytest_httptesting-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4049 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/README.md
+-rw-r--r--   0        0        0      632 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assert_element_checker_base.py
+-rw-r--r--   0        0        0     1392 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_attribute_base.py
+-rw-r--r--   0        0        0     1820 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_data.py
+-rw-r--r--   0        0        0     1608 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/content_assertion.py
+-rw-r--r--   0        0        0     2368 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/cookies_assertion.py
+-rw-r--r--   0        0        0     1617 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/headers_assertion.py
+-rw-r--r--   0        0        0      843 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/_assertion_elements/status_code_assertion.py
+-rw-r--r--   0        0        0     1557 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/assertions.py
+-rw-r--r--   0        0        0      311 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/cookie.py
+-rw-r--r--   0        0        0     2884 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/page_checker.py
+-rw-r--r--   0        0        0      762 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/plugin.py
+-rw-r--r--   0        0        0      745 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/http_testing/validators.py
+-rw-r--r--   0        0        0      705 2023-07-24 20:13:18.967621 pytest_httptesting-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 pytest_httptesting-0.6.0/PKG-INFO
```

### Comparing `pytest_httptesting-0.5.0/LICENSE` & `pytest_httptesting-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.5.0/README.md` & `pytest_httptesting-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_httptesting-0.5.0/http_testing/__init__.py` & `pytest_httptesting-0.6.0/http_testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .assertion_elements.content_assertion import ContentAssertion
-from .assertion_elements.cookies_assertion import Cookie, CookiesAssertion
-from .assertion_elements.headers_assertion import HeadersAssertion
-from .assertion_elements.status_code_assertion import StatusCodeAssertion
+from ._assertion_elements.content_assertion import ContentAssertion
+from ._assertion_elements.cookies_assertion import Cookie, CookiesAssertion
+from ._assertion_elements.headers_assertion import HeadersAssertion
+from ._assertion_elements.status_code_assertion import StatusCodeAssertion
 from .assertions import Assertions, NegativeAssertions
 from .page_checker import PageChecker
 from .validators import Regex, Text
 
 __all__ = (
     "Assertions",
     "ContentAssertion",
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/assert_element_checker_base.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/assert_element_checker_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from abc import ABC, abstractmethod
 from typing import Generic, Optional, TypeVar
 
-from httpx import Client, Response
+from http_testing._assertion_elements.assertion_data import AssertionData
 
 T = TypeVar("T")
 
 
-class AssertElementCheckerBase(Generic[T]):
+class AssertElementCheckerBase(Generic[T], ABC):
     value: Optional[T]
 
     def __init__(self, value: Optional[T] = None):
         self.value = value
 
-    def check(self, http_client: Client, response: Response, negative: bool = False):
+    @abstractmethod
+    def check(self, assertion_data: AssertionData, negative: bool):
         raise NotImplementedError
 
     @staticmethod
     def _make_message(info: str, check_type: str, url: str, negative: bool) -> str:
         return f"{info}{'' if negative else ' not'} " f"found in {check_type} on page '{url}'"
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/assertion_attribute_base.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/assertion_attribute_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from abc import ABC
 from typing import ClassVar, Type
 from weakref import WeakKeyDictionary
 
-from httpx import Client, Response
-
 from .assert_element_checker_base import AssertElementCheckerBase
+from .assertion_data import AssertionData
 
 
-class AssertionAttributeBase:
+class AssertionAttributeBase(ABC):
     _checker_type: Type[AssertElementCheckerBase]
     # if the owner instance of the descriptor is deleted, we should also remove the its entry from assertion_instances
     # that's why we use WeakKeyDictionary
     # it groups the checkers by owner : {owner_instance: [checker_instance, ...]}
     checkers: ClassVar[WeakKeyDictionary] = WeakKeyDictionary()
 
     def __get__(self, instance, owner):
@@ -25,11 +25,11 @@
         checker = self._checker_type(value)
         if instance not in self.checkers:
             self.checkers.setdefault(instance, [])
         self.checkers[instance].append(checker)
         setattr(instance, self._private_name, checker)
 
 
-def check_all(instance, http_client: Client, response: Response, negative: bool):
+def check_all(instance, assertion_data: AssertionData, negative: bool):
     checker: AssertElementCheckerBase
     for checker in AssertionAttributeBase.checkers[instance]:
-        checker.check(http_client, response, negative)
+        checker.check(assertion_data=assertion_data, negative=negative)
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/content_assertion.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/content_assertion.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import re
 from typing import Sequence, Union
 
-from httpx import Client, Response
+from http_testing.validators import Regex, Text, Validator
 
-from ..validators import Regex, Text, Validator
 from .assert_element_checker_base import AssertElementCheckerBase
 from .assertion_attribute_base import AssertionAttributeBase
+from .assertion_data import AssertionData
 
 
 class _ContentChecker(AssertElementCheckerBase[Sequence[Union[str, Validator]]]):
     """
     Check the response's content.
     If the given expected value is `str`, first convert it to `validators.Text` validator.
     If the given expected value is a `Regex` validator and its flag is 0, override the flag to `re.MULTILINE`
     """
 
-    def check(self, http_client: Client, response: Response, negative: bool = False) -> None:
+    def check(self, assertion_data: AssertionData, negative: bool) -> None:
         if self.value is None:
             return
         for expected in self.value:
             validator: Validator
             if isinstance(expected, str):
                 validator = Text(value=expected)
             elif isinstance(expected, Regex):
                 validator = expected
                 if validator.flags == 0:
                     # prefer multiline mode when search in http content
                     validator.flags = re.MULTILINE
             else:
                 validator = expected
 
-            if (not validator.validate(text=response.text)) ^ negative:
+            if (not validator.validate(text=assertion_data.response_text)) ^ negative:
                 raise AssertionError(
                     self._make_message(
-                        info=f"'{self.value}'", check_type="content", url=str(response.url), negative=negative
+                        info=f"'{self.value}'", check_type="content", url=str(assertion_data.url), negative=negative
                     )
                 )
 
 
 class ContentAssertion(AssertionAttributeBase):
     _checker_type = _ContentChecker
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/cookies_assertion.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/cookies_assertion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,52 @@
-from collections import defaultdict
-from http.cookiejar import Cookie as HttpCookie
-from typing import Mapping, Optional, Sequence, Union
+from typing import Mapping, Sequence
 
-from attrs import define
-from httpx import Client, Response
+from http_testing.cookie import Cookie
+from http_testing.validators import Text, Validator
 
-from ..validators import Text, Validator
 from .assert_element_checker_base import AssertElementCheckerBase
 from .assertion_attribute_base import AssertionAttributeBase
-
-
-@define
-class Cookie:
-    name: str
-    value: Union[str, Validator]
-    domain: Optional[str] = None
-    path: Optional[str] = None
-    secure: Optional[bool] = None
-    expires: Optional[int] = None
+from .assertion_data import AssertionData, HttpClientCookie
 
 
 class _CookiesChecker(AssertElementCheckerBase[Sequence[Cookie]]):
-    def check(self, http_client: Client, response: Response, negative: bool = False) -> None:
+    def check(self, assertion_data: AssertionData, negative: bool) -> None:
         if self.value is None:
             return
         for cookie in self.value:
-            # same cookie name can be on different sites, so use dict to group cookies list by name
-            all_cookies = defaultdict(list)
-            for cookiejar in http_client.cookies.jar:
-                all_cookies[cookiejar.name].append(cookiejar)
-            for cookiejar in response.cookies.jar:
-                all_cookies[cookiejar.name].append(cookiejar)
-
-            is_cookie_exist = self._is_cookie_match(target_cookie=cookie, all_cookies=all_cookies)
+            is_cookie_exist = self._is_cookie_match(target_cookie=cookie, all_cookies=assertion_data.all_cookies)
             if (not is_cookie_exist) ^ negative:
                 raise AssertionError(
                     self._make_message(
                         info=f"'{cookie.name}':'{cookie.value}'",
                         check_type="cookies",
-                        url=str(response.url),
+                        url=str(assertion_data.url),
                         negative=negative,
                     )
                 )
 
     @staticmethod
-    def _is_cookie_match(target_cookie: Cookie, all_cookies: Mapping[str, Sequence[HttpCookie]]):
+    def _is_cookie_match(target_cookie: Cookie, all_cookies: Mapping[str, Sequence[HttpClientCookie]]):
         cookies = all_cookies.get(target_cookie.name)
         if cookies is None:
             return False
         for cookie in cookies:
             if cookie.value is None:
                 continue
-            if target_cookie.domain is not None and cookie.domain_specified and target_cookie.domain != cookie.domain:
+            if target_cookie.domain is not None and cookie.domain is not None and target_cookie.domain != cookie.domain:
                 continue
-            if target_cookie.path is not None and cookie.path_specified and target_cookie.path != cookie.path:
+            if target_cookie.path is not None and cookie.path is not None and target_cookie.path != cookie.path:
                 continue
             if target_cookie.secure is not None and target_cookie.secure != cookie.secure:
                 continue
-            if target_cookie.expires is not None and target_cookie.expires != cookie.expires:
+            if (
+                target_cookie.expires is not None
+                and cookie.expires is not None
+                and target_cookie.expires != cookie.expires
+            ):
                 continue
             validator: Validator
             if isinstance(target_cookie.value, str):
                 validator = Text(value=target_cookie.value)
             else:
                 validator = target_cookie.value
             if validator.validate(cookie.value):
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/headers_assertion.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/headers_assertion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import Mapping, Union
 
-from httpx import Client, Response
+from http_testing.validators import Text, Validator
 
-from ..validators import Text, Validator
 from .assert_element_checker_base import AssertElementCheckerBase
 from .assertion_attribute_base import AssertionAttributeBase
+from .assertion_data import AssertionData
 
 
 class _HeadersChecker(AssertElementCheckerBase[Mapping[str, Union[str, Validator]]]):
-    def check(self, http_client: Client, response: Response, negative: bool = False) -> None:
+    def check(self, assertion_data: AssertionData, negative: bool) -> None:
         """
         Check the response's header.
         If the given expected header value is `str`, first convert it to `validators.Text` validator.
         """
         if self.value is None:
             return
         for header_key, expected_header_value in self.value.items():
+            header_key = header_key.upper()
             validator: Validator
             if isinstance(expected_header_value, str):
                 validator = Text(value=expected_header_value)
             else:
                 validator = expected_header_value
-            # the header names in response are case-insensitive
-            is_header_not_found = header_key not in response.headers or not validator.validate(
-                response.headers[header_key]
+            is_header_not_found = header_key not in assertion_data.response_headers or not validator.validate(
+                assertion_data.response_headers[header_key]
             )
             if is_header_not_found ^ negative:
                 raise AssertionError(
                     self._make_message(
                         info=f"'{header_key}':'{expected_header_value}'",
                         check_type="headers",
-                        url=str(response.url),
+                        url=str(assertion_data.url),
                         negative=negative,
                     )
                 )
 
 
 class HeadersAssertion(AssertionAttributeBase):
     _checker_type = _HeadersChecker
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertion_elements/status_code_assertion.py` & `pytest_httptesting-0.6.0/http_testing/_assertion_elements/status_code_assertion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from httpx import Client, Response
+from http_testing._assertion_elements.assertion_data import AssertionData
 
 from .assert_element_checker_base import AssertElementCheckerBase
 from .assertion_attribute_base import AssertionAttributeBase
 
 
 class _StatusCodeChecker(AssertElementCheckerBase[int]):
-    def check(self, http_client: Client, response: Response, negative: bool = False) -> None:
+    def check(self, assertion_data: AssertionData, negative: bool) -> None:
         if self.value:
-            if (self.value != response.status_code) ^ negative:
+            if (self.value != assertion_data.response_status_code) ^ negative:
                 raise AssertionError(
                     self._make_message(
-                        info=f"'{self.value}'", check_type="status_code", url=str(response.url), negative=negative
+                        info=f"'{self.value}'",
+                        check_type="status_code",
+                        url=str(assertion_data.url),
+                        negative=negative,
                     )
                 )
 
 
 class StatusCodeAssertion(AssertionAttributeBase):
     _checker_type = _StatusCodeChecker
```

### Comparing `pytest_httptesting-0.5.0/http_testing/assertions.py` & `pytest_httptesting-0.6.0/http_testing/assertions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from abc import ABC
 from typing import Mapping, Optional, Sequence
 
 from httpx import Client, Response
 
-from .assertion_elements.assertion_attribute_base import check_all
-from .assertion_elements.content_assertion import ContentAssertion
-from .assertion_elements.cookies_assertion import Cookie, CookiesAssertion
-from .assertion_elements.headers_assertion import HeadersAssertion
-from .assertion_elements.status_code_assertion import StatusCodeAssertion
+from http_testing._assertion_elements.assertion_attribute_base import check_all
+from http_testing._assertion_elements.assertion_data import AssertionData
+from http_testing._assertion_elements.content_assertion import ContentAssertion
+from http_testing._assertion_elements.cookies_assertion import Cookie, CookiesAssertion
+from http_testing._assertion_elements.headers_assertion import HeadersAssertion
+from http_testing._assertion_elements.status_code_assertion import StatusCodeAssertion
 
 
-class _AssertionsBase:
+class _AssertionsBase(ABC):
     _negative: bool = False
     status_code = StatusCodeAssertion()
     content = ContentAssertion()
     headers = HeadersAssertion()
     cookies = CookiesAssertion()
 
     def __init__(
@@ -25,15 +27,16 @@
     ):
         self.status_code = status_code
         self.content = content
         self.headers = headers
         self.cookies = cookies
 
     def check_assertions(self, http_client: Client, response: Response) -> None:
-        check_all(instance=self, http_client=http_client, response=response, negative=self._negative)
+        assertion_data = AssertionData.create(response=response, http_client=http_client)
+        check_all(instance=self, assertion_data=assertion_data, negative=self._negative)
 
 
 class Assertions(_AssertionsBase):
     _negative: bool = False
 
 
 class NegativeAssertions(_AssertionsBase):
```

### Comparing `pytest_httptesting-0.5.0/http_testing/page_checker.py` & `pytest_httptesting-0.6.0/http_testing/page_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from tempfile import NamedTemporaryFile
 from typing import Any, Dict, Optional, Union
 
 from attrs import define
 from httpx import URL, Client, Response
 
-from .assertions import Assertions, NegativeAssertions
+from http_testing.assertions import Assertions, NegativeAssertions
 
 
 @define
 class PageChecker:
     _base_url: Union[URL, str]
     _http_client: Client
     _previous_response: Optional[Response] = None
```

### Comparing `pytest_httptesting-0.5.0/http_testing/validators.py` & `pytest_httptesting-0.6.0/http_testing/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
-from abc import ABC
+from abc import ABC, abstractmethod
 from typing import Union
 
 from attrs import define
 
 
 class Validator(ABC):
+    @abstractmethod
     def validate(self, text: str) -> bool:
         raise NotImplementedError
 
 
 @define
 class Regex(Validator):
     """
```

### Comparing `pytest_httptesting-0.5.0/pyproject.toml` & `pytest_httptesting-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-httptesting"
-version = "0.5.0"
+version = "0.6.0"
 description = "http_testing framework on top of pytest"
 authors = ["HE Qile <mr.qile@gmail.com>"]
 readme = "README.md"
 packages = [{include = "http_testing"}]
 
 homepage = "https://github.com/heqile/http_testing"
 repository = "https://github.com/heqile/http_testing"
```

### Comparing `pytest_httptesting-0.5.0/setup.py` & `pytest_httptesting-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,315 +1,298 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2768 7474 705f 7465 7374 696e   \.['http_testin
-00000050: 6727 2c20 2768 7474 705f 7465 7374 696e  g', 'http_testin
-00000060: 672e 6173 7365 7274 696f 6e5f 656c 656d  g.assertion_elem
-00000070: 656e 7473 275d 0a0a 7061 636b 6167 655f  ents']..package_
-00000080: 6461 7461 203d 205c 0a7b 2727 3a20 5b27  data = \.{'': ['
-00000090: 2a27 5d7d 0a0a 696e 7374 616c 6c5f 7265  *']}..install_re
-000000a0: 7175 6972 6573 203d 205c 0a5b 2761 7474  quires = \.['att
-000000b0: 7273 3e3d 3233 2e31 2e30 2c3c 3234 2e30  rs>=23.1.0,<24.0
-000000c0: 2e30 272c 2027 6874 7470 783e 3d30 2e32  .0', 'httpx>=0.2
-000000d0: 342e 302c 3c30 2e32 352e 3027 2c20 2770  4.0,<0.25.0', 'p
-000000e0: 7974 6573 743e 3d37 2e32 2e30 2c3c 382e  ytest>=7.2.0,<8.
-000000f0: 302e 3027 5d0a 0a65 6e74 7279 5f70 6f69  0.0']..entry_poi
-00000100: 6e74 7320 3d20 5c0a 7b27 7079 7465 7374  nts = \.{'pytest
-00000110: 3131 273a 205b 2768 7474 705f 7061 6765  11': ['http_page
-00000120: 5f63 6865 636b 6572 203d 2068 7474 705f  _checker = http_
-00000130: 7465 7374 696e 672e 706c 7567 696e 275d  testing.plugin']
-00000140: 7d0a 0a73 6574 7570 5f6b 7761 7267 7320  }..setup_kwargs 
-00000150: 3d20 7b0a 2020 2020 276e 616d 6527 3a20  = {.    'name': 
-00000160: 2770 7974 6573 742d 6874 7470 7465 7374  'pytest-httptest
-00000170: 696e 6727 2c0a 2020 2020 2776 6572 7369  ing',.    'versi
-00000180: 6f6e 273a 2027 302e 352e 3027 2c0a 2020  on': '0.5.0',.  
-00000190: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-000001a0: 2027 6874 7470 5f74 6573 7469 6e67 2066   'http_testing f
-000001b0: 7261 6d65 776f 726b 206f 6e20 746f 7020  ramework on top 
-000001c0: 6f66 2070 7974 6573 7427 2c0a 2020 2020  of pytest',.    
-000001d0: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
-000001e0: 6e27 3a20 2723 2048 5454 505f 5445 5354  n': '# HTTP_TEST
-000001f0: 494e 475c 6e5c 6e3c 6120 6872 6566 3d22  ING\n\n<a href="
-00000200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000210: 6f6d 2f68 6571 696c 652f 6874 7470 5f74  om/heqile/http_t
-00000220: 6573 7469 6e67 2f61 6374 696f 6e73 3f71  esting/actions?q
-00000230: 7565 7279 3d62 7261 6e63 6825 3341 6d61  uery=branch%3Ama
-00000240: 696e 2b65 7665 6e74 2533 4170 7573 682b  in+event%3Apush+
-00000250: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00000260: 223e 5c6e 2020 2020 3c69 6d67 2073 7263  ">\n    <img src
-00000270: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000280: 2e63 6f6d 2f68 6571 696c 652f 6874 7470  .com/heqile/http
-00000290: 5f74 6573 7469 6e67 2f77 6f72 6b66 6c6f  _testing/workflo
-000002a0: 7773 2f54 6573 742f 6261 6467 652e 7376  ws/Test/badge.sv
-000002b0: 673f 6576 656e 743d 7075 7368 2662 7261  g?event=push&bra
-000002c0: 6e63 683d 6d61 696e 2220 616c 743d 2254  nch=main" alt="T
-000002d0: 6573 7422 3e5c 6e3c 2f61 3e5c 6e3c 6120  est">\n</a>\n<a 
-000002e0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-000002f0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f70  pi.org/project/p
-00000300: 7974 6573 742d 6874 7470 7465 7374 696e  ytest-httptestin
-00000310: 6722 2074 6172 6765 743d 225f 626c 616e  g" target="_blan
-00000320: 6b22 3e5c 6e20 2020 203c 696d 6720 7372  k">\n    <img sr
-00000330: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000340: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000350: 2f70 7974 6573 742d 6874 7470 7465 7374  /pytest-httptest
-00000360: 696e 673f 636f 6c6f 723d 2532 3333 3444  ing?color=%2334D
-00000370: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
-00000380: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
-00000390: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
-000003a0: 5c6e 3c2f 613e 5c6e 3c61 2068 7265 663d  \n</a>\n<a href=
-000003b0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-000003c0: 672f 7072 6f6a 6563 742f 7079 7465 7374  g/project/pytest
-000003d0: 2d68 7474 7074 6573 7469 6e67 2220 7461  -httptesting" ta
-000003e0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5c6e  rget="_blank">\n
-000003f0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000400: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000410: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000420: 696f 6e73 2f70 7974 6573 742d 6874 7470  ions/pytest-http
-00000430: 7465 7374 696e 672e 7376 673f 636f 6c6f  testing.svg?colo
-00000440: 723d 2532 3333 3444 3035 3822 2061 6c74  r=%2334D058" alt
-00000450: 3d22 5375 7070 6f72 7465 6420 5079 7468  ="Supported Pyth
-00000460: 6f6e 2076 6572 7369 6f6e 7322 3e5c 6e3c  on versions">\n<
-00000470: 2f61 3e5c 6e5c 6e23 2320 4465 7363 7269  /a>\n\n## Descri
-00000480: 7074 696f 6e5c 6e54 6869 7320 7072 6f6a  ption\nThis proj
-00000490: 6563 7420 6169 6d73 2074 6f20 6865 6c70  ect aims to help
-000004a0: 2074 6f20 6372 6561 7465 2065 3265 2074   to create e2e t
-000004b0: 6573 7473 2c20 6279 2063 6861 696e 696e  ests, by chainin
-000004c0: 6720 6874 7470 2063 616c 6c73 2061 6e64  g http calls and
-000004d0: 2076 6572 6966 6963 6174 696f 6e73 206f   verifications o
-000004e0: 6e20 7461 7267 6574 2070 6167 6573 2e5c  n target pages.\
-000004f0: 6e5c 6e23 2320 436f 6e63 6570 745c 6e54  n\n## Concept\nT
-00000500: 6869 7320 7072 6f6a 6563 7420 6973 2062  his project is b
-00000510: 7569 6c74 206f 6e20 7079 7465 7374 2e5c  uilt on pytest.\
-00000520: 6e5c 6e45 6163 6820 2e70 7920 6669 6c65  n\nEach .py file
-00000530: 2069 6e20 7465 7374 2072 6570 7265 7365   in test represe
-00000540: 6e74 7320 7365 7665 7261 6c20 7465 7374  nts several test
-00000550: 7320 7363 656e 6172 696f 206f 6e20 6f6e  s scenario on on
-00000560: 6520 7461 7267 6574 2073 6974 652c 2077  e target site, w
-00000570: 6520 6361 6e20 7072 6f76 6964 6520 7468  e can provide th
-00000580: 6520 7369 7465 5c27 7320 686f 7374 6e61  e site\'s hostna
-00000590: 6d65 5c6e 6173 2061 206c 6f63 616c 2076  me\nas a local v
-000005a0: 6172 6961 626c 652c 2074 6865 2066 7261  ariable, the fra
-000005b0: 6d65 776f 726b 206b 6e6f 7720 686f 7720  mework know how 
-000005c0: 746f 2063 6f6e 7374 7275 6374 2068 7474  to construct htt
-000005d0: 7020 6361 6c6c 2066 726f 6d20 7468 6174  p call from that
-000005e0: 2e5c 6e5c 6e45 6163 6820 7465 7374 2066  .\n\nEach test f
-000005f0: 756e 6374 696f 6e20 696e 2074 6865 202e  unction in the .
-00000600: 7079 2074 6573 7420 6669 6c65 2072 6570  py test file rep
-00000610: 7265 7365 6e74 2061 2073 6365 6e61 7269  resent a scenari
-00000620: 6f20 6f66 2074 6573 7420 7768 6963 6820  o of test which 
-00000630: 6973 2063 6f6e 7369 7374 6564 2062 7920  is consisted by 
-00000640: 7365 7665 7261 6c20 7374 6570 732e 2046  several steps. F
-00000650: 6f72 2065 7861 6d70 6c65 2c5c 6e74 6573  or example,\ntes
-00000660: 7420 7573 6572 5c27 7320 6163 636f 756e  t user\'s accoun
-00000670: 7420 7061 6765 2c20 6669 7273 742c 2077  t page, first, w
-00000680: 6520 6175 7468 656e 7469 6361 7465 2074  e authenticate t
-00000690: 6865 2063 6c69 656e 7420 6279 2070 6f73  he client by pos
-000006a0: 7420 7573 6572 5c27 7320 6e61 6d65 2061  t user\'s name a
-000006b0: 6e64 2070 6173 7377 6f72 642c 5c6e 7468  nd password,\nth
-000006c0: 656e 2061 6363 6573 7320 7468 6520 6163  en access the ac
-000006d0: 636f 756e 7420 7061 6765 2074 6f20 7665  count page to ve
-000006e0: 7269 6679 2073 6f6d 6520 7661 6c75 6573  rify some values
-000006f0: 2e20 4561 6368 2073 7465 7020 6973 2064  . Each step is d
-00000700: 6573 6372 6962 6564 2062 7920 6361 6c6c  escribed by call
-00000710: 696e 6720 7468 6520 7661 7269 6162 6c65  ing the variable
-00000720: 2060 6368 6563 6b60 5c6e 7768 6963 6820   `check`\nwhich 
-00000730: 6973 2061 2070 7974 6573 7420 6669 7874  is a pytest fixt
-00000740: 7572 652e 5c6e 5c6e 2323 2054 7574 6f72  ure.\n\n## Tutor
-00000750: 6961 6c5c 6e23 2323 2049 6e73 7461 6c6c  ial\n### Install
-00000760: 5c6e 6060 6062 6173 685c 6e70 6970 2069  \n```bash\npip i
-00000770: 6e73 7461 6c6c 2070 7974 6573 742d 6874  nstall pytest-ht
-00000780: 7470 7465 7374 696e 675c 6e60 6060 5c6e  tptesting\n```\n
-00000790: 5c6e 2323 2320 4372 6561 7465 2074 6573  \n### Create tes
-000007a0: 7420 7375 6974 655c 6e60 6060 7079 7468  t suite\n```pyth
-000007b0: 6f6e 5c6e 2320 7465 7374 2f74 6573 745f  on\n# test/test_
-000007c0: 6578 616d 706c 652e 7079 5c6e 6672 6f6d  example.py\nfrom
-000007d0: 2068 7474 705f 7465 7374 696e 672e 6173   http_testing.as
-000007e0: 7365 7274 696f 6e73 2069 6d70 6f72 7420  sertions import 
-000007f0: 4173 7365 7274 696f 6e73 2c20 4e65 6761  Assertions, Nega
-00000800: 7469 7665 4173 7365 7274 696f 6e73 5c6e  tiveAssertions\n
-00000810: 6672 6f6d 2068 7474 705f 7465 7374 696e  from http_testin
-00000820: 672e 636f 6f6b 6965 2069 6d70 6f72 7420  g.cookie import 
-00000830: 436f 6f6b 6965 5c6e 6672 6f6d 2068 7474  Cookie\nfrom htt
-00000840: 705f 7465 7374 696e 672e 7061 6765 5f63  p_testing.page_c
-00000850: 6865 636b 6572 2069 6d70 6f72 7420 5061  hecker import Pa
-00000860: 6765 4368 6563 6b65 725c 6e66 726f 6d20  geChecker\nfrom 
-00000870: 6874 7470 5f74 6573 7469 6e67 2e76 616c  http_testing.val
-00000880: 6964 6174 6f72 7320 696d 706f 7274 2052  idators import R
-00000890: 6567 6578 5c6e 5c6e 686f 7374 203d 2022  egex\n\nhost = "
-000008a0: 7777 772e 676f 6f67 6c65 2e63 6f6d 2220  www.google.com" 
-000008b0: 2023 206d 616e 6461 746f 7279 3a20 7573   # mandatory: us
-000008c0: 6564 2069 6e20 7468 6520 6063 6865 636b  ed in the `check
-000008d0: 6020 6669 7874 7572 655c 6e73 6368 656d  ` fixture\nschem
-000008e0: 6520 3d20 2268 7474 7073 2220 2023 2022  e = "https"  # "
-000008f0: 6874 7470 7322 2062 7920 6465 6661 756c  https" by defaul
-00000900: 745c 6e70 6f72 7420 3d20 4e6f 6e65 2020  t\nport = None  
-00000910: 2320 4e6f 6e65 2062 7920 6465 6661 756c  # None by defaul
-00000920: 745c 6e5c 6e5c 6e64 6566 2074 6573 745f  t\n\n\ndef test_
-00000930: 7363 656e 6172 696f 5f6f 6e65 2863 6865  scenario_one(che
-00000940: 636b 3a20 5061 6765 4368 6563 6b65 7229  ck: PageChecker)
-00000950: 3a5c 6e20 2020 2063 6865 636b 285c 6e20  :\n    check(\n 
-00000960: 2020 2020 2020 2074 6974 6c65 3d22 5365         title="Se
-00000970: 6e61 7269 6f20 4f6e 6522 2c5c 6e20 2020  nario One",\n   
-00000980: 2020 2020 2070 6174 683d 222f 222c 5c6e       path="/",\n
-00000990: 2020 2020 2020 2020 7368 6f75 6c64 5f66          should_f
-000009a0: 696e 643d 4173 7365 7274 696f 6e73 285c  ind=Assertions(\
-000009b0: 6e20 2020 2020 2020 2020 2020 2073 7461  n            sta
-000009c0: 7475 735f 636f 6465 3d32 3030 2c5c 6e20  tus_code=200,\n 
-000009d0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-000009e0: 6e74 3d5b 223c 7469 746c 653e 476f 6f67  nt=["<title>Goog
-000009f0: 6c65 3c2f 7469 746c 653e 225d 2c5c 6e20  le</title>"],\n 
-00000a00: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00000a10: 7273 3d7b 2243 6f6e 7465 6e74 2d54 7970  rs={"Content-Typ
-00000a20: 6522 3a20 2274 6578 742f 6874 6d6c 3b20  e": "text/html; 
-00000a30: 6368 6172 7365 743d 4953 4f2d 3838 3539  charset=ISO-8859
-00000a40: 2d31 227d 2c5c 6e20 2020 2020 2020 2020  -1"},\n         
-00000a50: 2020 2063 6f6f 6b69 6573 3d5b 436f 6f6b     cookies=[Cook
-00000a60: 6965 286e 616d 653d 2241 4543 222c 2076  ie(name="AEC", v
-00000a70: 616c 7565 3d52 6567 6578 2872 222e 2a22  alue=Regex(r".*"
-00000a80: 2929 5d2c 5c6e 2020 2020 2020 2020 292c  ))],\n        ),
-00000a90: 5c6e 2020 2020 2020 2020 7368 6f75 6c64  \n        should
-00000aa0: 5f6e 6f74 5f66 696e 643d 4e65 6761 7469  _not_find=Negati
-00000ab0: 7665 4173 7365 7274 696f 6e73 285c 6e20  veAssertions(\n 
-00000ac0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00000ad0: 735f 636f 6465 3d34 3030 2c5c 6e20 2020  s_code=400,\n   
-00000ae0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-00000af0: 3d5b 2267 726f 6f74 225d 2c5c 6e20 2020  =["groot"],\n   
-00000b00: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-00000b10: 3d7b 226e 6f6f 6f6f 6f22 3a20 2222 7d2c  ={"nooooo": ""},
-00000b20: 5c6e 2020 2020 2020 2020 2020 2020 636f  \n            co
-00000b30: 6f6b 6965 733d 5b43 6f6f 6b69 6528 6e61  okies=[Cookie(na
-00000b40: 6d65 3d22 6e6f 7022 2c20 7661 6c75 653d  me="nop", value=
-00000b50: 2261 2229 5d2c 5c6e 2020 2020 2020 2020  "a")],\n        
-00000b60: 292c 5c6e 2020 2020 2020 2020 7469 6d65  ),\n        time
-00000b70: 6f75 743d 3130 2c20 2023 2079 6f75 2063  out=10,  # you c
-00000b80: 616e 2070 6173 7320 6164 6469 7469 6f6e  an pass addition
-00000b90: 616c 206b 7761 7267 7320 746f 2068 7474  al kwargs to htt
-00000ba0: 7078 2072 6571 7565 7374 5c6e 2020 2020  px request\n    
-00000bb0: 295c 6e5c 6e20 2020 2061 7373 6572 7420  )\n\n    assert 
-00000bc0: 6368 6563 6b2e 7072 6576 696f 7573 5f72  check.previous_r
-00000bd0: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
-00000be0: 6f64 6520 3d3d 2032 3030 2020 2320 696e  ode == 200  # in
-00000bf0: 7370 6563 7420 7072 6576 696f 7573 2072  spect previous r
-00000c00: 6573 706f 6e73 655c 6e60 6060 5c6e 5c6e  esponse\n```\n\n
-00000c10: 2323 2320 5275 6e20 7465 7374 5c6e 6060  ### Run test\n``
-00000c20: 6062 6173 685c 6e24 2070 7974 6573 7420  `bash\n$ pytest 
-00000c30: 7465 7374 202d 2d74 623d 6e6f 202d 2d6e  test --tb=no --n
-00000c40: 6f2d 6865 6164 6572 202d 7620 2023 2074  o-header -v  # t
-00000c50: 7261 6365 6261 636b 2069 7320 6469 7361  raceback is disa
-00000c60: 626c 6564 2062 6563 6175 7365 2069 7420  bled because it 
-00000c70: 6973 206e 6f74 2076 6572 7920 7573 6566  is not very usef
-00000c80: 756c 2074 6f20 616e 6179 7365 2074 6865  ul to anayse the
-00000c90: 2066 756e 6374 696f 6e61 6c20 6572 726f   functional erro
-00000ca0: 725c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  r\n=============
-00000cb0: 2074 6573 7420 7365 7373 696f 6e20 7374   test session st
-00000cc0: 6172 7473 203d 3d3d 3d3d 3d3d 3d3d 3d3d  arts ===========
-00000cd0: 3d3d 5c6e 636f 6c6c 6563 7465 6420 3120  ==\ncollected 1 
-00000ce0: 6974 656d 5c6e 5c6e 7465 7374 2f74 6573  item\n\ntest/tes
-00000cf0: 745f 6578 616d 706c 652e 7079 3a3a 7465  t_example.py::te
-00000d00: 7374 5f73 6365 6e61 7269 6f5f 6f6e 6520  st_scenario_one 
-00000d10: 5041 5353 4544 5c6e 5c6e 3d3d 3d3d 3d3d  PASSED\n\n======
-00000d20: 3d3d 3d3d 3d3d 3d20 3120 7061 7373 6564  ======= 1 passed
-00000d30: 2069 6e20 302e 3136 7320 3d3d 3d3d 3d3d   in 0.16s ======
-00000d40: 3d3d 3d3d 3d3d 3d5c 6e5c 6e60 6060 5c6e  =======\n\n```\n
-00000d50: 5c6e 2323 2320 4465 6275 675c 6e49 6e20  \n### Debug\nIn 
-00000d60: 6361 7365 206f 6620 6572 726f 722c 2061  case of error, a
-00000d70: 2074 656d 706f 7261 7279 2066 696c 6520   temporary file 
-00000d80: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
-00000d90: 642c 2061 7320 7368 6f77 6e20 696e 2074  d, as shown in t
-00000da0: 6865 2060 7368 6f72 7420 7465 7374 2073  he `short test s
-00000db0: 756d 6d61 7279 2069 6e66 6f60 2e20 4974  ummary info`. It
-00000dc0: 2069 7320 6120 6a73 6f6e 2066 696c 6520   is a json file 
-00000dd0: 636f 6e63 6c75 6469 6e67 5c6e 7265 7370  concluding\nresp
-00000de0: 6f6e 7365 2063 6f6e 7465 6e74 2c20 7374  onse content, st
-00000df0: 6174 7573 2063 6f64 652c 2068 6561 6465  atus code, heade
-00000e00: 7273 2061 6e64 2063 6f6f 6b69 6573 2e5c  rs and cookies.\
-00000e10: 6e60 6060 6261 7368 5c6e 2420 7079 7465  n```bash\n$ pyte
-00000e20: 7374 2074 6573 7420 2d2d 7462 3d6e 6f20  st test --tb=no 
-00000e30: 2d2d 6e6f 2d68 6561 6465 7220 2d76 5c6e  --no-header -v\n
-00000e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 7465  ============= te
-00000e50: 7374 2073 6573 7369 6f6e 2073 7461 7274  st session start
-00000e60: 7320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d5c  s =============\
-00000e70: 6e63 6f6c 6c65 6374 6564 2031 2069 7465  ncollected 1 ite
-00000e80: 6d5c 6e5c 6e74 6573 742f 7465 7374 5f65  m\n\ntest/test_e
-00000e90: 7861 6d70 6c65 2e70 793a 3a74 6573 745f  xample.py::test_
-00000ea0: 7363 656e 6172 696f 5f6f 6e65 2046 4149  scenario_one FAI
-00000eb0: 4c45 445c 6e5c 6e3d 3d3d 3d3d 3d3d 3d3d  LED\n\n=========
-00000ec0: 3d3d 3d3d 2073 686f 7274 2074 6573 7420  ==== short test 
-00000ed0: 7375 6d6d 6172 7920 696e 666f 203d 3d3d  summary info ===
-00000ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 5c6e 4641 494c  ==========\nFAIL
-00000ef0: 4544 2074 6573 742f 7465 7374 5f65 7861  ED test/test_exa
-00000f00: 6d70 6c65 2e70 793a 3a74 6573 745f 7363  mple.py::test_sc
-00000f10: 656e 6172 696f 5f6f 6e65 202d 2041 7373  enario_one - Ass
-00000f20: 6572 7469 6f6e 4572 726f 723a 2053 656e  ertionError: Sen
-00000f30: 6172 696f 204f 6e65 202d 205c 2743 6f6e  ario One - \'Con
-00000f40: 7465 6e74 2d54 7970 6573 7373 735c 273a  tent-Typessss\':
-00000f50: 5c27 7465 7874 2f68 746d 6c3b 2063 6861  \'text/html; cha
-00000f60: 7273 6574 3d49 534f 2d38 3835 392d 315c  rset=ISO-8859-1\
-00000f70: 2720 6e6f 7420 666f 756e 6420 696e 2068  ' not found in h
-00000f80: 6561 6465 7273 206f 6e20 7061 6765 205c  eaders on page \
-00000f90: 2768 7474 7073 3a2f 2f77 7777 2e67 6f6f  'https://www.goo
-00000fa0: 676c 652e 636f 6d2f 5c27 202d 2070 6c65  gle.com/\' - ple
-00000fb0: 6173 6520 6368 6563 6b20 6669 6c65 205c  ase check file \
-00000fc0: 272f 746d 702f 746d 7074 616f 7764 3275  '/tmp/tmptaowd2u
-00000fd0: 355c 275c 6e3d 3d3d 3d3d 3d3d 3d3d 3d3d  5\'\n===========
-00000fe0: 3d3d 2031 2066 6169 6c65 6420 696e 2031  == 1 failed in 1
-00000ff0: 2e32 3273 203d 3d3d 3d3d 3d3d 3d3d 3d3d  .22s ===========
-00001000: 3d3d 5c6e 5c6e 6060 605c 6e5c 6e23 2323  ==\n\n```\n\n###
-00001010: 2041 6476 616e 6365 645c 6e23 2323 2320   Advanced\n#### 
-00001020: 4375 7374 6f6d 697a 6520 7468 6520 6874  Customize the ht
-00001030: 7470 2063 6c69 656e 7420 636f 6e66 6967  tp client config
-00001040: 7572 6174 696f 6e5c 6e49 7420 6973 2070  uration\nIt is p
-00001050: 6f73 7369 626c 6520 746f 2063 7265 6174  ossible to creat
-00001060: 6520 6120 6669 7874 7572 6520 6068 7474  e a fixture `htt
-00001070: 705f 636c 6965 6e74 6020 746f 2063 7265  p_client` to cre
-00001080: 6174 6520 796f 7572 206f 776e 2068 7474  ate your own htt
-00001090: 7020 636c 6965 6e74 2e5c 6e60 6060 7079  p client.\n```py
-000010a0: 7468 6f6e 5c6e 4070 7974 6573 742e 6669  thon\n@pytest.fi
-000010b0: 7874 7572 655c 6e64 6566 2068 7474 705f  xture\ndef http_
-000010c0: 636c 6965 6e74 2829 3a5c 6e20 2020 2077  client():\n    w
-000010d0: 6974 6820 436c 6965 6e74 2876 6572 6966  ith Client(verif
-000010e0: 793d 4661 6c73 652c 2063 6f6f 6b69 6573  y=False, cookies
-000010f0: 3d7b 2263 6f6f 6b69 655f 3122 3a20 2263  ={"cookie_1": "c
-00001100: 6f6f 6b69 655f 7661 6c75 655f 3122 7d29  ookie_value_1"})
-00001110: 2061 7320 636c 6965 6e74 3a5c 6e20 2020   as client:\n   
-00001120: 2020 2020 2079 6965 6c64 2063 6c69 656e       yield clien
-00001130: 745c 6e60 6060 5c6e 5c6e 2323 2323 2043  t\n```\n\n#### C
-00001140: 7573 746f 6d69 7a65 2074 6865 2062 6173  ustomize the bas
-00001150: 6520 7572 6c5c 6e49 7420 6973 2070 6f73  e url\nIt is pos
-00001160: 7369 626c 6520 746f 2063 7265 6174 6520  sible to create 
-00001170: 6120 6669 7874 7572 6520 6062 6173 655f  a fixture `base_
-00001180: 7572 6c60 2074 6f20 6f76 6572 7269 6465  url` to override
-00001190: 2074 6865 2064 6566 6175 6c74 2063 6f6e   the default con
-000011a0: 7374 7275 6374 696f 6e20 6f66 2062 6173  struction of bas
-000011b0: 6520 7572 6c2e 5c6e 6060 6070 7974 686f  e url.\n```pytho
-000011c0: 6e5c 6e66 726f 6d20 6874 7470 7820 696d  n\nfrom httpx im
-000011d0: 706f 7274 2055 524c 5c6e 4070 7974 6573  port URL\n@pytes
-000011e0: 742e 6669 7874 7572 655c 6e64 6566 2062  t.fixture\ndef b
-000011f0: 6173 655f 7572 6c28 2920 2d3e 2055 524c  ase_url() -> URL
-00001200: 3a5c 6e20 2020 2072 6574 7572 6e20 5552  :\n    return UR
-00001210: 4c28 2268 7474 7073 3a2f 2f77 7777 2e67  L("https://www.g
-00001220: 6f6f 676c 652e 636f 6d22 295c 6e60 6060  oogle.com")\n```
-00001230: 5c6e 272c 0a20 2020 2027 6175 7468 6f72  \n',.    'author
-00001240: 273a 2027 4845 2051 696c 6527 2c0a 2020  ': 'HE Qile',.  
-00001250: 2020 2761 7574 686f 725f 656d 6169 6c27    'author_email'
-00001260: 3a20 276d 722e 7169 6c65 4067 6d61 696c  : 'mr.qile@gmail
-00001270: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-00001280: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-00001290: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-000012a0: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-000012b0: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-000012c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000012d0: 6865 7169 6c65 2f68 7474 705f 7465 7374  heqile/http_test
-000012e0: 696e 6727 2c0a 2020 2020 2770 6163 6b61  ing',.    'packa
-000012f0: 6765 7327 3a20 7061 636b 6167 6573 2c0a  ges': packages,.
-00001300: 2020 2020 2770 6163 6b61 6765 5f64 6174      'package_dat
-00001310: 6127 3a20 7061 636b 6167 655f 6461 7461  a': package_data
-00001320: 2c0a 2020 2020 2769 6e73 7461 6c6c 5f72  ,.    'install_r
-00001330: 6571 7569 7265 7327 3a20 696e 7374 616c  equires': instal
-00001340: 6c5f 7265 7175 6972 6573 2c0a 2020 2020  l_requires,.    
-00001350: 2765 6e74 7279 5f70 6f69 6e74 7327 3a20  'entry_points': 
-00001360: 656e 7472 795f 706f 696e 7473 2c0a 2020  entry_points,.  
-00001370: 2020 2770 7974 686f 6e5f 7265 7175 6972    'python_requir
-00001380: 6573 273a 2027 3e3d 332e 382c 3c34 2e30  es': '>=3.8,<4.0
-00001390: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
-000013a0: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7465  : 2.1.Name: pyte
+00000020: 7374 2d68 7474 7074 6573 7469 6e67 0a56  st-httptesting.V
+00000030: 6572 7369 6f6e 3a20 302e 362e 300a 5375  ersion: 0.6.0.Su
+00000040: 6d6d 6172 793a 2068 7474 705f 7465 7374  mmary: http_test
+00000050: 696e 6720 6672 616d 6577 6f72 6b20 6f6e  ing framework on
+00000060: 2074 6f70 206f 6620 7079 7465 7374 0a48   top of pytest.H
+00000070: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
+00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6571  //github.com/heq
+00000090: 696c 652f 6874 7470 5f74 6573 7469 6e67  ile/http_testing
+000000a0: 0a41 7574 686f 723a 2048 4520 5169 6c65  .Author: HE Qile
+000000b0: 0a41 7574 686f 722d 656d 6169 6c3a 206d  .Author-email: m
+000000c0: 722e 7169 6c65 4067 6d61 696c 2e63 6f6d  r.qile@gmail.com
+000000d0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000000e0: 3a20 3e3d 332e 382c 3c34 2e30 0a43 6c61  : >=3.8,<4.0.Cla
+000000f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000100: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000110: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
+00000120: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000130: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000140: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
+00000150: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000160: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000170: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000180: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001b0: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
+000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001e0: 3a20 332e 3131 0a52 6571 7569 7265 732d  : 3.11.Requires-
+000001f0: 4469 7374 3a20 6174 7472 7320 283e 3d32  Dist: attrs (>=2
+00000200: 332e 312e 302c 3c32 342e 302e 3029 0a52  3.1.0,<24.0.0).R
+00000210: 6571 7569 7265 732d 4469 7374 3a20 6874  equires-Dist: ht
+00000220: 7470 7820 283e 3d30 2e32 342e 302c 3c30  tpx (>=0.24.0,<0
+00000230: 2e32 352e 3029 0a52 6571 7569 7265 732d  .25.0).Requires-
+00000240: 4469 7374 3a20 7079 7465 7374 2028 3e3d  Dist: pytest (>=
+00000250: 372e 322e 302c 3c38 2e30 2e30 290a 5072  7.2.0,<8.0.0).Pr
+00000260: 6f6a 6563 742d 5552 4c3a 2052 6570 6f73  oject-URL: Repos
+00000270: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+00000280: 6974 6875 622e 636f 6d2f 6865 7169 6c65  ithub.com/heqile
+00000290: 2f68 7474 705f 7465 7374 696e 670a 4465  /http_testing.De
+000002a0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000002b0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000002c0: 6b64 6f77 6e0a 0a23 2048 5454 505f 5445  kdown..# HTTP_TE
+000002d0: 5354 494e 470a 0a3c 6120 6872 6566 3d22  STING..<a href="
+000002e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002f0: 6f6d 2f68 6571 696c 652f 6874 7470 5f74  om/heqile/http_t
+00000300: 6573 7469 6e67 2f61 6374 696f 6e73 3f71  esting/actions?q
+00000310: 7565 7279 3d62 7261 6e63 6825 3341 6d61  uery=branch%3Ama
+00000320: 696e 2b65 7665 6e74 2533 4170 7573 682b  in+event%3Apush+
+00000330: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000340: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000350: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000360: 636f 6d2f 6865 7169 6c65 2f68 7474 705f  com/heqile/http_
+00000370: 7465 7374 696e 672f 776f 726b 666c 6f77  testing/workflow
+00000380: 732f 5465 7374 2f62 6164 6765 2e73 7667  s/Test/badge.svg
+00000390: 3f65 7665 6e74 3d70 7573 6826 6272 616e  ?event=push&bran
+000003a0: 6368 3d6d 6169 6e22 2061 6c74 3d22 5465  ch=main" alt="Te
+000003b0: 7374 223e 0a3c 2f61 3e0a 3c61 2068 7265  st">.</a>.<a hre
+000003c0: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+000003d0: 6f72 672f 7072 6f6a 6563 742f 7079 7465  org/project/pyte
+000003e0: 7374 2d68 7474 7074 6573 7469 6e67 2220  st-httptesting" 
+000003f0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000400: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000410: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000420: 6473 2e69 6f2f 7079 7069 2f76 2f70 7974  ds.io/pypi/v/pyt
+00000430: 6573 742d 6874 7470 7465 7374 696e 673f  est-httptesting?
+00000440: 636f 6c6f 723d 2532 3333 3444 3035 3826  color=%2334D058&
+00000450: 6c61 6265 6c3d 7079 7069 2532 3070 6163  label=pypi%20pac
+00000460: 6b61 6765 2220 616c 743d 2250 6163 6b61  kage" alt="Packa
+00000470: 6765 2076 6572 7369 6f6e 223e 0a3c 2f61  ge version">.</a
+00000480: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+00000490: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000004a0: 6563 742f 7079 7465 7374 2d68 7474 7074  ect/pytest-httpt
+000004b0: 6573 7469 6e67 2220 7461 7267 6574 3d22  esting" target="
+000004c0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
+000004d0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+000004e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000004f0: 7069 2f70 7976 6572 7369 6f6e 732f 7079  pi/pyversions/py
+00000500: 7465 7374 2d68 7474 7074 6573 7469 6e67  test-httptesting
+00000510: 2e73 7667 3f63 6f6c 6f72 3d25 3233 3334  .svg?color=%2334
+00000520: 4430 3538 2220 616c 743d 2253 7570 706f  D058" alt="Suppo
+00000530: 7274 6564 2050 7974 686f 6e20 7665 7273  rted Python vers
+00000540: 696f 6e73 223e 0a3c 2f61 3e0a 0a23 2320  ions">.</a>..## 
+00000550: 4465 7363 7269 7074 696f 6e0a 5468 6973  Description.This
+00000560: 2070 726f 6a65 6374 2061 696d 7320 746f   project aims to
+00000570: 2068 656c 7020 746f 2063 7265 6174 6520   help to create 
+00000580: 6532 6520 7465 7374 732c 2062 7920 6368  e2e tests, by ch
+00000590: 6169 6e69 6e67 2068 7474 7020 6361 6c6c  aining http call
+000005a0: 7320 616e 6420 7665 7269 6669 6361 7469  s and verificati
+000005b0: 6f6e 7320 6f6e 2074 6172 6765 7420 7061  ons on target pa
+000005c0: 6765 732e 0a0a 2323 2043 6f6e 6365 7074  ges...## Concept
+000005d0: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+000005e0: 2062 7569 6c74 206f 6e20 7079 7465 7374   built on pytest
+000005f0: 2e0a 0a45 6163 6820 2e70 7920 6669 6c65  ...Each .py file
+00000600: 2069 6e20 7465 7374 2072 6570 7265 7365   in test represe
+00000610: 6e74 7320 7365 7665 7261 6c20 7465 7374  nts several test
+00000620: 7320 7363 656e 6172 696f 206f 6e20 6f6e  s scenario on on
+00000630: 6520 7461 7267 6574 2073 6974 652c 2077  e target site, w
+00000640: 6520 6361 6e20 7072 6f76 6964 6520 7468  e can provide th
+00000650: 6520 7369 7465 2773 2068 6f73 746e 616d  e site's hostnam
+00000660: 650a 6173 2061 206c 6f63 616c 2076 6172  e.as a local var
+00000670: 6961 626c 652c 2074 6865 2066 7261 6d65  iable, the frame
+00000680: 776f 726b 206b 6e6f 7720 686f 7720 746f  work know how to
+00000690: 2063 6f6e 7374 7275 6374 2068 7474 7020   construct http 
+000006a0: 6361 6c6c 2066 726f 6d20 7468 6174 2e0a  call from that..
+000006b0: 0a45 6163 6820 7465 7374 2066 756e 6374  .Each test funct
+000006c0: 696f 6e20 696e 2074 6865 202e 7079 2074  ion in the .py t
+000006d0: 6573 7420 6669 6c65 2072 6570 7265 7365  est file represe
+000006e0: 6e74 2061 2073 6365 6e61 7269 6f20 6f66  nt a scenario of
+000006f0: 2074 6573 7420 7768 6963 6820 6973 2063   test which is c
+00000700: 6f6e 7369 7374 6564 2062 7920 7365 7665  onsisted by seve
+00000710: 7261 6c20 7374 6570 732e 2046 6f72 2065  ral steps. For e
+00000720: 7861 6d70 6c65 2c0a 7465 7374 2075 7365  xample,.test use
+00000730: 7227 7320 6163 636f 756e 7420 7061 6765  r's account page
+00000740: 2c20 6669 7273 742c 2077 6520 6175 7468  , first, we auth
+00000750: 656e 7469 6361 7465 2074 6865 2063 6c69  enticate the cli
+00000760: 656e 7420 6279 2070 6f73 7420 7573 6572  ent by post user
+00000770: 2773 206e 616d 6520 616e 6420 7061 7373  's name and pass
+00000780: 776f 7264 2c0a 7468 656e 2061 6363 6573  word,.then acces
+00000790: 7320 7468 6520 6163 636f 756e 7420 7061  s the account pa
+000007a0: 6765 2074 6f20 7665 7269 6679 2073 6f6d  ge to verify som
+000007b0: 6520 7661 6c75 6573 2e20 4561 6368 2073  e values. Each s
+000007c0: 7465 7020 6973 2064 6573 6372 6962 6564  tep is described
+000007d0: 2062 7920 6361 6c6c 696e 6720 7468 6520   by calling the 
+000007e0: 7661 7269 6162 6c65 2060 6368 6563 6b60  variable `check`
+000007f0: 0a77 6869 6368 2069 7320 6120 7079 7465  .which is a pyte
+00000800: 7374 2066 6978 7475 7265 2e0a 0a23 2320  st fixture...## 
+00000810: 5475 746f 7269 616c 0a23 2323 2049 6e73  Tutorial.### Ins
+00000820: 7461 6c6c 0a60 6060 6261 7368 0a70 6970  tall.```bash.pip
+00000830: 2069 6e73 7461 6c6c 2070 7974 6573 742d   install pytest-
+00000840: 6874 7470 7465 7374 696e 670a 6060 600a  httptesting.```.
+00000850: 0a23 2323 2043 7265 6174 6520 7465 7374  .### Create test
+00000860: 2073 7569 7465 0a60 6060 7079 7468 6f6e   suite.```python
+00000870: 0a23 2074 6573 742f 7465 7374 5f65 7861  .# test/test_exa
+00000880: 6d70 6c65 2e70 790a 6672 6f6d 2068 7474  mple.py.from htt
+00000890: 705f 7465 7374 696e 672e 6173 7365 7274  p_testing.assert
+000008a0: 696f 6e73 2069 6d70 6f72 7420 4173 7365  ions import Asse
+000008b0: 7274 696f 6e73 2c20 4e65 6761 7469 7665  rtions, Negative
+000008c0: 4173 7365 7274 696f 6e73 0a66 726f 6d20  Assertions.from 
+000008d0: 6874 7470 5f74 6573 7469 6e67 2e63 6f6f  http_testing.coo
+000008e0: 6b69 6520 696d 706f 7274 2043 6f6f 6b69  kie import Cooki
+000008f0: 650a 6672 6f6d 2068 7474 705f 7465 7374  e.from http_test
+00000900: 696e 672e 7061 6765 5f63 6865 636b 6572  ing.page_checker
+00000910: 2069 6d70 6f72 7420 5061 6765 4368 6563   import PageChec
+00000920: 6b65 720a 6672 6f6d 2068 7474 705f 7465  ker.from http_te
+00000930: 7374 696e 672e 7661 6c69 6461 746f 7273  sting.validators
+00000940: 2069 6d70 6f72 7420 5265 6765 780a 0a68   import Regex..h
+00000950: 6f73 7420 3d20 2277 7777 2e67 6f6f 676c  ost = "www.googl
+00000960: 652e 636f 6d22 2020 2320 6d61 6e64 6174  e.com"  # mandat
+00000970: 6f72 793a 2075 7365 6420 696e 2074 6865  ory: used in the
+00000980: 2060 6368 6563 6b60 2066 6978 7475 7265   `check` fixture
+00000990: 0a73 6368 656d 6520 3d20 2268 7474 7073  .scheme = "https
+000009a0: 2220 2023 2022 6874 7470 7322 2062 7920  "  # "https" by 
+000009b0: 6465 6661 756c 740a 706f 7274 203d 204e  default.port = N
+000009c0: 6f6e 6520 2023 204e 6f6e 6520 6279 2064  one  # None by d
+000009d0: 6566 6175 6c74 0a0a 0a64 6566 2074 6573  efault...def tes
+000009e0: 745f 7363 656e 6172 696f 5f6f 6e65 2863  t_scenario_one(c
+000009f0: 6865 636b 3a20 5061 6765 4368 6563 6b65  heck: PageChecke
+00000a00: 7229 3a0a 2020 2020 6368 6563 6b28 0a20  r):.    check(. 
+00000a10: 2020 2020 2020 2074 6974 6c65 3d22 5365         title="Se
+00000a20: 6e61 7269 6f20 4f6e 6522 2c0a 2020 2020  nario One",.    
+00000a30: 2020 2020 7061 7468 3d22 2f22 2c0a 2020      path="/",.  
+00000a40: 2020 2020 2020 7368 6f75 6c64 5f66 696e        should_fin
+00000a50: 643d 4173 7365 7274 696f 6e73 280a 2020  d=Assertions(.  
+00000a60: 2020 2020 2020 2020 2020 7374 6174 7573            status
+00000a70: 5f63 6f64 653d 3230 302c 0a20 2020 2020  _code=200,.     
+00000a80: 2020 2020 2020 2063 6f6e 7465 6e74 3d5b         content=[
+00000a90: 223c 7469 746c 653e 476f 6f67 6c65 3c2f  "<title>Google</
+00000aa0: 7469 746c 653e 225d 2c0a 2020 2020 2020  title>"],.      
+00000ab0: 2020 2020 2020 6865 6164 6572 733d 7b22        headers={"
+00000ac0: 436f 6e74 656e 742d 5479 7065 223a 2022  Content-Type": "
+00000ad0: 7465 7874 2f68 746d 6c3b 2063 6861 7273  text/html; chars
+00000ae0: 6574 3d49 534f 2d38 3835 392d 3122 7d2c  et=ISO-8859-1"},
+00000af0: 0a20 2020 2020 2020 2020 2020 2063 6f6f  .            coo
+00000b00: 6b69 6573 3d5b 436f 6f6b 6965 286e 616d  kies=[Cookie(nam
+00000b10: 653d 2241 4543 222c 2076 616c 7565 3d52  e="AEC", value=R
+00000b20: 6567 6578 2872 222e 2a22 2929 5d2c 0a20  egex(r".*"))],. 
+00000b30: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00000b40: 2020 7368 6f75 6c64 5f6e 6f74 5f66 696e    should_not_fin
+00000b50: 643d 4e65 6761 7469 7665 4173 7365 7274  d=NegativeAssert
+00000b60: 696f 6e73 280a 2020 2020 2020 2020 2020  ions(.          
+00000b70: 2020 7374 6174 7573 5f63 6f64 653d 3430    status_code=40
+00000b80: 302c 0a20 2020 2020 2020 2020 2020 2063  0,.            c
+00000b90: 6f6e 7465 6e74 3d5b 2267 726f 6f74 225d  ontent=["groot"]
+00000ba0: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
+00000bb0: 6164 6572 733d 7b22 6e6f 6f6f 6f6f 223a  aders={"nooooo":
+00000bc0: 2022 227d 2c0a 2020 2020 2020 2020 2020   ""},.          
+00000bd0: 2020 636f 6f6b 6965 733d 5b43 6f6f 6b69    cookies=[Cooki
+00000be0: 6528 6e61 6d65 3d22 6e6f 7022 2c20 7661  e(name="nop", va
+00000bf0: 6c75 653d 2261 2229 5d2c 0a20 2020 2020  lue="a")],.     
+00000c00: 2020 2029 2c0a 2020 2020 2020 2020 7469     ),.        ti
+00000c10: 6d65 6f75 743d 3130 2c20 2023 2079 6f75  meout=10,  # you
+00000c20: 2063 616e 2070 6173 7320 6164 6469 7469   can pass additi
+00000c30: 6f6e 616c 206b 7761 7267 7320 746f 2068  onal kwargs to h
+00000c40: 7474 7078 2072 6571 7565 7374 0a20 2020  ttpx request.   
+00000c50: 2029 0a0a 2020 2020 6173 7365 7274 2063   )..    assert c
+00000c60: 6865 636b 2e70 7265 7669 6f75 735f 7265  heck.previous_re
+00000c70: 7370 6f6e 7365 2e73 7461 7475 735f 636f  sponse.status_co
+00000c80: 6465 203d 3d20 3230 3020 2023 2069 6e73  de == 200  # ins
+00000c90: 7065 6374 2070 7265 7669 6f75 7320 7265  pect previous re
+00000ca0: 7370 6f6e 7365 0a60 6060 0a0a 2323 2320  sponse.```..### 
+00000cb0: 5275 6e20 7465 7374 0a60 6060 6261 7368  Run test.```bash
+00000cc0: 0a24 2070 7974 6573 7420 7465 7374 202d  .$ pytest test -
+00000cd0: 2d74 623d 6e6f 202d 2d6e 6f2d 6865 6164  -tb=no --no-head
+00000ce0: 6572 202d 7620 2023 2074 7261 6365 6261  er -v  # traceba
+00000cf0: 636b 2069 7320 6469 7361 626c 6564 2062  ck is disabled b
+00000d00: 6563 6175 7365 2069 7420 6973 206e 6f74  ecause it is not
+00000d10: 2076 6572 7920 7573 6566 756c 2074 6f20   very useful to 
+00000d20: 616e 6179 7365 2074 6865 2066 756e 6374  anayse the funct
+00000d30: 696f 6e61 6c20 6572 726f 720a 3d3d 3d3d  ional error.====
+00000d40: 3d3d 3d3d 3d3d 3d3d 3d20 7465 7374 2073  ========= test s
+00000d50: 6573 7369 6f6e 2073 7461 7274 7320 3d3d  ession starts ==
+00000d60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 636f 6c6c  ===========.coll
+00000d70: 6563 7465 6420 3120 6974 656d 0a0a 7465  ected 1 item..te
+00000d80: 7374 2f74 6573 745f 6578 616d 706c 652e  st/test_example.
+00000d90: 7079 3a3a 7465 7374 5f73 6365 6e61 7269  py::test_scenari
+00000da0: 6f5f 6f6e 6520 5041 5353 4544 0a0a 3d3d  o_one PASSED..==
+00000db0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 3120 7061  =========== 1 pa
+00000dc0: 7373 6564 2069 6e20 302e 3136 7320 3d3d  ssed in 0.16s ==
+00000dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a60 6060  ===========..```
+00000de0: 0a0a 2323 2320 4465 6275 670a 496e 2063  ..### Debug.In c
+00000df0: 6173 6520 6f66 2065 7272 6f72 2c20 6120  ase of error, a 
+00000e00: 7465 6d70 6f72 6172 7920 6669 6c65 2077  temporary file w
+00000e10: 696c 6c20 6265 2067 656e 6572 6174 6564  ill be generated
+00000e20: 2c20 6173 2073 686f 776e 2069 6e20 7468  , as shown in th
+00000e30: 6520 6073 686f 7274 2074 6573 7420 7375  e `short test su
+00000e40: 6d6d 6172 7920 696e 666f 602e 2049 7420  mmary info`. It 
+00000e50: 6973 2061 206a 736f 6e20 6669 6c65 2063  is a json file c
+00000e60: 6f6e 636c 7564 696e 670a 7265 7370 6f6e  oncluding.respon
+00000e70: 7365 2063 6f6e 7465 6e74 2c20 7374 6174  se content, stat
+00000e80: 7573 2063 6f64 652c 2068 6561 6465 7273  us code, headers
+00000e90: 2061 6e64 2063 6f6f 6b69 6573 2e0a 6060   and cookies..``
+00000ea0: 6062 6173 680a 2420 7079 7465 7374 2074  `bash.$ pytest t
+00000eb0: 6573 7420 2d2d 7462 3d6e 6f20 2d2d 6e6f  est --tb=no --no
+00000ec0: 2d68 6561 6465 7220 2d76 0a3d 3d3d 3d3d  -header -v.=====
+00000ed0: 3d3d 3d3d 3d3d 3d3d 2074 6573 7420 7365  ======== test se
+00000ee0: 7373 696f 6e20 7374 6172 7473 203d 3d3d  ssion starts ===
+00000ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a63 6f6c 6c65  ==========.colle
+00000f00: 6374 6564 2031 2069 7465 6d0a 0a74 6573  cted 1 item..tes
+00000f10: 742f 7465 7374 5f65 7861 6d70 6c65 2e70  t/test_example.p
+00000f20: 793a 3a74 6573 745f 7363 656e 6172 696f  y::test_scenario
+00000f30: 5f6f 6e65 2046 4149 4c45 440a 0a3d 3d3d  _one FAILED..===
+00000f40: 3d3d 3d3d 3d3d 3d3d 3d3d 2073 686f 7274  ========== short
+00000f50: 2074 6573 7420 7375 6d6d 6172 7920 696e   test summary in
+00000f60: 666f 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  fo =============
+00000f70: 0a46 4149 4c45 4420 7465 7374 2f74 6573  .FAILED test/tes
+00000f80: 745f 6578 616d 706c 652e 7079 3a3a 7465  t_example.py::te
+00000f90: 7374 5f73 6365 6e61 7269 6f5f 6f6e 6520  st_scenario_one 
+00000fa0: 2d20 4173 7365 7274 696f 6e45 7272 6f72  - AssertionError
+00000fb0: 3a20 5365 6e61 7269 6f20 4f6e 6520 2d20  : Senario One - 
+00000fc0: 2743 6f6e 7465 6e74 2d54 7970 6573 7373  'Content-Typesss
+00000fd0: 7327 3a27 7465 7874 2f68 746d 6c3b 2063  s':'text/html; c
+00000fe0: 6861 7273 6574 3d49 534f 2d38 3835 392d  harset=ISO-8859-
+00000ff0: 3127 206e 6f74 2066 6f75 6e64 2069 6e20  1' not found in 
+00001000: 6865 6164 6572 7320 6f6e 2070 6167 6520  headers on page 
+00001010: 2768 7474 7073 3a2f 2f77 7777 2e67 6f6f  'https://www.goo
+00001020: 676c 652e 636f 6d2f 2720 2d20 706c 6561  gle.com/' - plea
+00001030: 7365 2063 6865 636b 2066 696c 6520 272f  se check file '/
+00001040: 746d 702f 746d 7074 616f 7764 3275 3527  tmp/tmptaowd2u5'
+00001050: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2031  .============= 1
+00001060: 2066 6169 6c65 6420 696e 2031 2e32 3273   failed in 1.22s
+00001070: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a   =============..
+00001080: 6060 600a 0a23 2323 2041 6476 616e 6365  ```..### Advance
+00001090: 640a 2323 2323 2043 7573 746f 6d69 7a65  d.#### Customize
+000010a0: 2074 6865 2068 7474 7020 636c 6965 6e74   the http client
+000010b0: 2063 6f6e 6669 6775 7261 7469 6f6e 0a49   configuration.I
+000010c0: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
+000010d0: 2063 7265 6174 6520 6120 6669 7874 7572   create a fixtur
+000010e0: 6520 6068 7474 705f 636c 6965 6e74 6020  e `http_client` 
+000010f0: 746f 2063 7265 6174 6520 796f 7572 206f  to create your o
+00001100: 776e 2068 7474 7020 636c 6965 6e74 2e0a  wn http client..
+00001110: 6060 6070 7974 686f 6e0a 4070 7974 6573  ```python.@pytes
+00001120: 742e 6669 7874 7572 650a 6465 6620 6874  t.fixture.def ht
+00001130: 7470 5f63 6c69 656e 7428 293a 0a20 2020  tp_client():.   
+00001140: 2077 6974 6820 436c 6965 6e74 2876 6572   with Client(ver
+00001150: 6966 793d 4661 6c73 652c 2063 6f6f 6b69  ify=False, cooki
+00001160: 6573 3d7b 2263 6f6f 6b69 655f 3122 3a20  es={"cookie_1": 
+00001170: 2263 6f6f 6b69 655f 7661 6c75 655f 3122  "cookie_value_1"
+00001180: 7d29 2061 7320 636c 6965 6e74 3a0a 2020  }) as client:.  
+00001190: 2020 2020 2020 7969 656c 6420 636c 6965        yield clie
+000011a0: 6e74 0a60 6060 0a0a 2323 2323 2043 7573  nt.```..#### Cus
+000011b0: 746f 6d69 7a65 2074 6865 2062 6173 6520  tomize the base 
+000011c0: 7572 6c0a 4974 2069 7320 706f 7373 6962  url.It is possib
+000011d0: 6c65 2074 6f20 6372 6561 7465 2061 2066  le to create a f
+000011e0: 6978 7475 7265 2060 6261 7365 5f75 726c  ixture `base_url
+000011f0: 6020 746f 206f 7665 7272 6964 6520 7468  ` to override th
+00001200: 6520 6465 6661 756c 7420 636f 6e73 7472  e default constr
+00001210: 7563 7469 6f6e 206f 6620 6261 7365 2075  uction of base u
+00001220: 726c 2e0a 6060 6070 7974 686f 6e0a 6672  rl..```python.fr
+00001230: 6f6d 2068 7474 7078 2069 6d70 6f72 7420  om httpx import 
+00001240: 5552 4c0a 4070 7974 6573 742e 6669 7874  URL.@pytest.fixt
+00001250: 7572 650a 6465 6620 6261 7365 5f75 726c  ure.def base_url
+00001260: 2829 202d 3e20 5552 4c3a 0a20 2020 2072  () -> URL:.    r
+00001270: 6574 7572 6e20 5552 4c28 2268 7474 7073  eturn URL("https
+00001280: 3a2f 2f77 7777 2e67 6f6f 676c 652e 636f  ://www.google.co
+00001290: 6d22 290a 6060 600a 0a                   m").```..
```

