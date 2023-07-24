# Comparing `tmp/selenium_driverless-1.0.4.tar.gz` & `tmp/selenium_driverless-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.0.4.tar", last modified: Sun Jul 23 12:37:54 2023, max compression
+gzip compressed data, was "selenium_driverless-1.1.tar", last modified: Mon Jul 24 18:48:40 2023, max compression
```

## Comparing `selenium_driverless-1.0.4.tar` & `selenium_driverless-1.1.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.568357 selenium_driverless-1.0.4/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.0.4/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3250 2023-07-23 12:37:54.568357 selenium_driverless-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1934 2023-07-23 12:37:21.000000 selenium_driverless-1.0.4/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.0.4/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-23 12:37:54.569358 selenium_driverless-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1936 2023-07-21 20:56:42.000000 selenium_driverless-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.543040 selenium_driverless-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.553122 selenium_driverless-1.0.4/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-23 12:37:43.000000 selenium_driverless-1.0.4/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.560357 selenium_driverless-1.0.4/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.0.4/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.564357 selenium_driverless-1.0.4/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.0.4/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2720 2023-07-21 20:13:40.000000 selenium_driverless-1.0.4/src/selenium_driverless/scripts/mobile.py
--rw-rw-rw-   0        0        0     1400 2023-01-11 12:23:14.000000 selenium_driverless-1.0.4/src/selenium_driverless/scripts/multi_thread.py
--rw-rw-rw-   0        0        0    16797 2023-07-23 12:34:39.000000 selenium_driverless-1.0.4/src/selenium_driverless/scripts/options.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.565358 selenium_driverless-1.0.4/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.0.4/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.0.4/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    47194 2023-07-23 12:36:44.000000 selenium_driverless-1.0.4/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.559358 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3250 2023-07-23 12:37:54.000000 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-07-23 12:37:54.000000 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 12:37:54.000000 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-07-23 12:37:54.000000 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-23 12:37:54.000000 selenium_driverless-1.0.4/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 12:37:54.567358 selenium_driverless-1.0.4/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.0.4/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.079400 selenium_driverless-1.1/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.1/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3765 2023-07-24 18:48:40.079400 selenium_driverless-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2451 2023-07-24 18:45:43.000000 selenium_driverless-1.1/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.1/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-24 18:48:40.080503 selenium_driverless-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.045887 selenium_driverless-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.055942 selenium_driverless-1.1/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       21 2023-07-24 18:48:14.000000 selenium_driverless-1.1/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.065059 selenium_driverless-1.1/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.1/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.074327 selenium_driverless-1.1/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2820 2023-07-23 16:18:48.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    16993 2023-07-23 15:23:23.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/cdp_listener.py
+-rw-rw-rw-   0        0        0     2720 2023-07-21 20:13:40.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/mobile.py
+-rw-rw-rw-   0        0        0    16797 2023-07-23 12:34:39.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5281 2023-07-23 16:28:03.000000 selenium_driverless-1.1/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.077400 selenium_driverless-1.1/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.1/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.1/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    43597 2023-07-24 18:27:59.000000 selenium_driverless-1.1/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.064008 selenium_driverless-1.1/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3765 2023-07-24 18:48:39.000000 selenium_driverless-1.1/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-07-24 18:48:39.000000 selenium_driverless-1.1/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:48:39.000000 selenium_driverless-1.1/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-24 18:48:39.000000 selenium_driverless-1.1/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 18:48:39.000000 selenium_driverless-1.1/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:40.078405 selenium_driverless-1.1/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.1/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.0.4/LICENSE.md` & `selenium_driverless-1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.4/PKG-INFO` & `selenium_driverless-1.1/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium_driverless
-Version: 1.0.4
+Name: selenium-driverless
+Version: 1.1
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -46,17 +46,40 @@
 
 * [Windows] Install [Chrome-Browser](https://www.google.de/chrome/)
 * ```pip install selenium-driverless```
 
 
 ### Usage
 
-#### example script
+#### with asyncio
 ```python
 from selenium_driverless import webdriver
+import asyncio
+
+
+async def main():
+    options = webdriver.Options()
+    async with webdriver.Chrome(options=options) as driver:
+        await driver.get('http://nowsecure.nl#relax')
+        await driver.implicitly_wait(3)
+
+        title = await driver.title
+        url = await driver.current_url
+        source = await driver.page_source
+        print(title)
+
+
+asyncio.run(main())
+```
+
+#### synchronous
+asyncified, might be buggy
+
+```python
+from selenium_driverless.sync import webdriver
 
 options = webdriver.Options()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
@@ -67,15 +90,15 @@
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- implementations
+- [ ] page-interactions
   - [ ] find element
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.0.4/README.md` & `selenium_driverless-1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,40 @@
 
 * [Windows] Install [Chrome-Browser](https://www.google.de/chrome/)
 * ```pip install selenium-driverless```
 
 
 ### Usage
 
-#### example script
+#### with asyncio
 ```python
 from selenium_driverless import webdriver
+import asyncio
+
+
+async def main():
+    options = webdriver.Options()
+    async with webdriver.Chrome(options=options) as driver:
+        await driver.get('http://nowsecure.nl#relax')
+        await driver.implicitly_wait(3)
+
+        title = await driver.title
+        url = await driver.current_url
+        source = await driver.page_source
+        print(title)
+
+
+asyncio.run(main())
+```
+
+#### synchronous
+asyncified, might be buggy
+
+```python
+from selenium_driverless.sync import webdriver
 
 options = webdriver.Options()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
@@ -37,15 +60,15 @@
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- implementations
+- [ ] page-interactions
   - [ ] find element
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.0.4/build_upload.md` & `selenium_driverless-1.1/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.4/setup.py` & `selenium_driverless-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import setuptools
 
-requirements = ['selenium~=4.6', 'aiohttp==3.8.5', 'websockets==11.0.3',
-                'beautifulsoup4==4.7.1', 'lxml==4.6.2', 'pyyaml==6.0.1',
-                'Pillow==7.1.0']
+requirements = ['selenium~=4.6', "chrome-devtools-protocol"]
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_driverless',
     author='Aurin Aegerter',
```

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless/scripts/mobile.py` & `selenium_driverless-1.1/src/selenium_driverless/scripts/mobile.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.1/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.1/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.1/src/selenium_driverless/webdriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,322 +15,238 @@
 # specific language governing permissions and limitations
 # under the License.
 
 # modified by kaliiiiiiiiii | Aurin Aegerter
 
 """The WebDriver implementation."""
 import asyncio
-import contextlib
-import copy
 import os.path
 import subprocess
 import typing
 import warnings
 from abc import ABCMeta
 from base64 import b64decode
 from base64 import urlsafe_b64encode
 from contextlib import asynccontextmanager
 from importlib import import_module
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pycdp.cdp.target
 from selenium.common.exceptions import InvalidArgumentException
 from selenium.common.exceptions import JavascriptException
-from selenium.common.exceptions import NoSuchCookieException
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.by import By
-from selenium.webdriver.common.html5.application_cache import ApplicationCache
-
-from selenium_driverless.scripts.options import Options as BaseOptions
 from selenium.webdriver.common.print_page_options import PrintOptions
-from selenium.webdriver.common.timeouts import Timeouts
 from selenium.webdriver.common.virtual_authenticator import Credential
 from selenium.webdriver.common.virtual_authenticator import VirtualAuthenticatorOptions
 from selenium.webdriver.common.virtual_authenticator import (
     required_virtual_authenticator,
 )
 from selenium.webdriver.remote.bidi_connection import BidiConnection
-from selenium.webdriver.remote.command import Command
-from selenium.webdriver.remote.errorhandler import ErrorHandler
 from selenium.webdriver.remote.file_detector import FileDetector
 from selenium.webdriver.remote.file_detector import LocalFileDetector
-from selenium_driverless.scripts.mobile import Mobile
 from selenium.webdriver.remote.script_key import ScriptKey
-from selenium.webdriver.remote.shadowroot import ShadowRoot
-from selenium.webdriver.remote.switch_to import SwitchTo
+from selenium.webdriver.remote.webdriver import create_matches
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.relative_locator import RelativeBy
-from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
+
+from selenium_driverless.scripts.mobile import Mobile
 from selenium_driverless.scripts.options import Options
+from selenium_driverless.scripts.switch_to import SwitchTo
 
 
 def import_cdp():
     return import_module("selenium.webdriver.common.bidi.cdp")
 
 
-def _create_caps(caps):
-    """Makes a W3C alwaysMatch capabilities object.
-
-    Filters out capability names that are not in the W3C spec. Spec-compliant
-    drivers will reject requests containing unknown capability names.
-
-    Moves the Firefox profile, if present, from the old location to the new Firefox
-    options object.
-
-    :Args:
-     - caps - A dictionary of capabilities requested by the caller.
-    """
-    caps = copy.deepcopy(caps)
-    always_match = {}
-    for k, v in caps.items():
-        always_match[k] = v
-    return {"capabilities": {"firstMatch": [{}], "alwaysMatch": always_match}}
-
-
-def create_matches(options: List[BaseOptions]) -> Dict:
-    capabilities = {"capabilities": {}}
-    opts = []
-    for opt in options:
-        opts.append(opt.to_capabilities())
-    opts_size = len(opts)
-    samesies = {}
-
-    # Can not use bitwise operations on the dicts or lists due to
-    # https://bugs.python.org/issue38210
-    for i in range(opts_size):
-        min_index = i
-        if i + 1 < opts_size:
-            first_keys = opts[min_index].keys()
-
-            for kys in first_keys:
-                if kys in opts[i + 1].keys():
-                    if opts[min_index][kys] == opts[i + 1][kys]:
-                        samesies.update({kys: opts[min_index][kys]})
-
-    always = {}
-    for k, v in samesies.items():
-        always[k] = v
-
-    for i in opts:
-        for k in always:
-            del i[k]
-
-    capabilities["capabilities"]["alwaysMatch"] = always
-    capabilities["capabilities"]["firstMatch"] = opts
-
-    return capabilities
-
-
 class BaseWebDriver(metaclass=ABCMeta):
     """Abstract Base Class for all Webdriver subtypes.
 
     ABC's allow custom implementations of Webdriver to be registered so
     that isinstance type checks will succeed.
     """
 
 
 class Chrome(BaseWebDriver):
     """Allows you to drive the browser without chromedriver."""
 
-    _web_element_cls = WebElement
-    _shadowroot_cls = ShadowRoot
-
     def __init__(
             self,
             options: Options = None,
-            loop: asyncio.AbstractEventLoop = None
     ) -> None:
         """Creates a new instance of the chrome driver. Starts the service and
         then creates new instance of chrome driver.
 
         :Args:
          - options - this takes an instance of ChromeOptions
         """
+        self._page_load_timeout = None
+        self._script_timeout = None
         self._conn = None
         self.session = None
         self.browser_pid = None
-        if not loop:
-            loop = asyncio.get_event_loop()
-        self._loop = loop
 
         try:
             options = options or Options()
             self._options = options
 
-            browser_name = DesiredCapabilities.CHROME["browserName"],
             vendor_prefix = "goog"
             self.vendor_prefix = vendor_prefix
 
             if isinstance(options, list):
                 self._capabilities = create_matches(options)
             else:
                 self._capabilities = options.to_capabilities()
             self._is_remote = True
             self.target_id = None
             self.caps = {}
             self.pinned_scripts = {}
-            self.error_handler = ErrorHandler()
             self._switch_to = SwitchTo(self)
             self._mobile = Mobile(self)
             self.file_detector = LocalFileDetector()
             self._authenticator_id = None
-            self.start_client()
-            self.start_session(self._capabilities)
 
         except Exception:
             self.quit()
             raise
         self._is_remote = False
 
     def __repr__(self):
         return f'<{type(self).__module__}.{type(self).__name__} (session="{self.target_id}")>'
 
+    async def __aenter__(self):
+        await self.start_session()
+        return self
+
     def __enter__(self):
         return self
 
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.quit()
+
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.quit()
+        pass
+
+    def __await__(self):
+        return self.start_session().__await__()
 
     @property
     def mobile(self) -> Mobile:
-        return self._mobile
+        raise NotImplementedError()
+        # return self._mobile
 
     @property
     def name(self) -> str:
         """Returns the name of the underlying browser for this instance.
 
         :Usage:
             ::
 
                 name = driver.name
         """
         if "browserName" in self.caps:
             return self.caps["browserName"]
         raise KeyError("browserName not specified in session capabilities")
 
-    def start_client(self):
+    async def start_client(self):
         """Called before starting a new session.
 
         This method may be overridden to define custom startup behavior.
         """
         pass
 
-    def stop_client(self):
+    async def stop_client(self):
         """Called after executing a quit command.
 
         This method may be overridden to define custom shutdown
         behavior.
         """
         pass
 
-    def start_session(self, capabilities: dict or None = None):
+    async def start_session(self, capabilities: dict or None = None):
         """Creates a new session with the desired capabilities.
 
         :Args:
          - capabilities - a capabilities dict to start the session with.
         """
+        await self.start_client()
         if not capabilities:
             capabilities = self._capabilities
         del self._capabilities
         from selenium_driverless.utils.utils import IS_POSIX, read
         from pycdp.asyncio import connect_cdp
         from pycdp import cdp
 
         options = capabilities["goog:chromeOptions"]
-        caps = _create_caps(capabilities)
 
         browser = subprocess.Popen(
             [options["binary"], *options["args"]],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             close_fds=IS_POSIX,
         )
 
         if self._options.debugger_address.split(":")[1] == "0":
             path = self._options.user_data_dir + "/DevToolsActivePort"
             while not os.path.isfile(path):
-                self.implicitly_wait(0.1)
+                await self.implicitly_wait(0.1)
             self._options.debugger_address = "localhost:" + read(path, sel_root=False).split("\n")[0]
-        self._conn = self._loop.run_until_complete(connect_cdp(f'http://{self._options.debugger_address}'))
+        self._conn = await connect_cdp(f'http://{self._options.debugger_address}')
         self.browser_pid = browser.pid
-        targets = self._loop.run_until_complete(self._conn.execute(cdp.target.get_targets()))
+        targets = await self._conn.execute(cdp.target.get_targets())
         for target in targets:
             if target.type_ == "page":
                 self.target_id = target.target_id
                 break
-        self.session = self._loop.run_until_complete(self._conn.connect_session(self.target_id))
+        self.session = await self._conn.connect_session(self.target_id)
         self.caps = capabilities
 
-    def _wrap_value(self, value):
-        if isinstance(value, dict):
-            converted = {}
-            for key, val in value.items():
-                converted[key] = self._wrap_value(val)
-            return converted
-        if isinstance(value, self._web_element_cls):
-            return {"element-6066-11e4-a52e-4f735466cecf": value.id}
-        if isinstance(value, self._shadowroot_cls):
-            return {"shadow-6066-11e4-a52e-4f735466cecf": value.id}
-        if isinstance(value, list):
-            return list(self._wrap_value(item) for item in value)
-        return value
-
-    def create_web_element(self, element_id: str) -> WebElement:
+    async def create_web_element(self, element_id: str) -> WebElement:
         """Creates a web element with the specified `element_id`."""
-        return self._web_element_cls(self, element_id)
-
-    def _unwrap_value(self, value):
-        if isinstance(value, dict):
-            if "element-6066-11e4-a52e-4f735466cecf" in value:
-                return self.create_web_element(value["element-6066-11e4-a52e-4f735466cecf"])
-            if "shadow-6066-11e4-a52e-4f735466cecf" in value:
-                return self._shadowroot_cls(self, value["shadow-6066-11e4-a52e-4f735466cecf"])
-            for key, val in value.items():
-                value[key] = self._unwrap_value(val)
-            return value
-        if isinstance(value, list):
-            return list(self._unwrap_value(item) for item in value)
-        return value
+        raise NotImplementedError()
 
-    def execute(self, driver_command: str = None, params: dict = None, cmd=None):
+    async def execute(self, driver_command: str = None, params: dict = None, cmd=None):
         """
         executes on current pycdp.cdp cmd on current session
         driver_command and params aren't used
         """
         if driver_command or params:
             raise NotImplementedError("chrome not started with chromedriver")
-        return self._loop.run_until_complete(self.session.execute(cmd=cmd))
+        return await self.session.execute(cmd=cmd)
 
-    def get(self, url: str) -> None:
+    async def get(self, url: str) -> None:
         """Loads a web page in the current browser session."""
         from pycdp import cdp
-        self.execute(cmd=cdp.page.enable())
+        await self.execute(cmd=cdp.page.enable())
 
         async def get(_url: str):
             with self.session.safe_wait_for(cdp.page.DomContentEventFired) as navigation:
                 await self.session.execute(cmd=cdp.page.navigate(_url))
                 await navigation
 
-        self._loop.run_until_complete(get(url))
+        try:
+            await asyncio.wait_for(get(url), self._page_load_timeout)
+        except asyncio.exceptions.TimeoutError:
+            raise TimeoutError(f"page didn't load within timeout of {self._page_load_timeout}")
 
     @property
-    def title(self) -> str:
+    async def title(self) -> str:
         """Returns the title of the current page.
 
         :Usage:
             ::
 
                 title = driver.title
         """
-        return self.current_target.title
+        target = await self.current_target
+        return target.title
 
     def pin_script(self, script: str, script_key=None) -> ScriptKey:
         """Store common javascript scripts to be executed later by a unique
         hashable ID."""
         script_key_instance = ScriptKey(script_key)
         self.pinned_scripts[script_key_instance.id] = script
         return script_key_instance
@@ -341,15 +257,15 @@
             self.pinned_scripts.pop(script_key.id)
         except KeyError:
             raise KeyError(f"No script with key: {script_key} existed in {self.pinned_scripts}") from None
 
     def get_pinned_scripts(self) -> List[str]:
         return list(self.pinned_scripts)
 
-    def execute_script(self, script, *args):
+    async def execute_script(self, script, *args):
         """Synchronously Executes JavaScript in the current window/frame.
 
         :Args:
          - script: The JavaScript to execute.
          - \\*args: Any applicable arguments for your JavaScript.
 
         :Usage:
@@ -366,23 +282,23 @@
                 raise JavascriptException("Pinned script could not be found")
 
         script = f"(function(...arguments){{{script}}})(...{json.dumps(args)})"
 
         script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
                                       user_gesture=True, await_promise=False,
                                       allow_unsafe_eval_blocked_by_csp=True, return_by_value=True)
-        result = self.execute(cmd=script)
+        result = await self.execute(cmd=script)
         if result[1]:
             class JSEvalException(result[1], Exception):
                 pass
 
             raise JSEvalException(result[1].description)
         return result[0].value
 
-    def execute_async_script(self, script: str, *args):
+    async def execute_async_script(self, script: str, *args):
         """Asynchronously Executes JavaScript in the current window/frame.
 
         :Args:
          - script: The JavaScript to execute.
          - \\*args: Any applicable arguments for your JavaScript.
 
         :Usage:
@@ -397,170 +313,172 @@
         script = """
         (function(...arguments){
             const promise = new Promise((resolve, reject) => {
                 arguments.push(resolve)
             });""" + script + "return promise})(..." + json.dumps(args) + ")"
         script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
                                       user_gesture=True, await_promise=True,
-                                      allow_unsafe_eval_blocked_by_csp=True)
-        result = self.execute(cmd=script)
+                                      allow_unsafe_eval_blocked_by_csp=True, timeout=self._script_timeout)
+        result = await self.execute(cmd=script)
         if result[1]:
             raise Exception(result[1].description)
         return result[0].value
 
     @property
-    def current_url(self) -> str:
+    async def current_url(self) -> str:
         """Gets the URL of the current page.
 
         :Usage:
             ::
 
                 driver.current_url
         """
-        return self.current_target.url
+        target = await self.current_target
+        return target.url
 
     @property
-    def page_source(self) -> str:
+    async def page_source(self) -> str:
         """Gets the source of the current page.
 
         :Usage:
             ::
 
                 driver.page_source
         """
-        return self.execute_script("return document.documentElement.outerHTML")
+        return await self.execute_script("return document.documentElement.outerHTML")
 
-    def close(self) -> None:
+    async def close(self) -> None:
         """Closes the current window.
 
         :Usage:
             ::
 
                 driver.close()
         """
         from pycdp import cdp
-        self.execute(cmd=cdp.page.close())
+        await self.execute(cmd=cdp.page.close())
 
-    def quit(self) -> None:
+    async def quit(self) -> None:
         """Quits the driver and closes every associated window.
 
         :Usage:
             ::
 
                 driver.quit()
         """
         import os
         import shutil
-        # noinspection PyBroadException
+        # noinspection PyBroadException,PyUnusedLocal
         try:
             try:
-                self.close()
+                await self.close()
 
                 # wait for process to be killed
                 while True:
                     try:
                         os.kill(self.browser_pid, 15)
                     except OSError:
                         break
-                    self.implicitly_wait(0.1)
+                    await self.implicitly_wait(0.1)
 
                 shutil.rmtree(self._options.user_data_dir, ignore_errors=True)
             finally:
-                self.stop_client()
+                await self.stop_client()
         except Exception as e:
             # We don't care about the message because something probably has gone wrong
             pass
         finally:
             pass  # self.service.stop()
 
     @property
-    def targets(self):
+    async def targets(self):
         from pycdp import cdp
-        return self.execute(cmd=cdp.target.get_targets())
+        return await self.execute(cmd=cdp.target.get_targets())
 
     @property
-    def current_target(self):
+    async def current_target(self):
         from pycdp import cdp
-        return self.execute(cmd=cdp.target.get_target_info(self.current_window_handle))
+        return await self.execute(cmd=cdp.target.get_target_info(await self.current_window_handle))
 
     @property
-    def current_window_handle(self) -> pycdp.cdp.target.TargetID:
+    async def current_window_handle(self) -> pycdp.cdp.target.TargetID:
         """Returns the handle of the current window.
 
         :Usage:
             ::
 
                 driver.current_window_handle
         """
         # noinspection PyProtectedMember
         return self.session._target_id
 
     @property
-    def current_window_id(self):
+    async def current_window_id(self):
         from pycdp import cdp
-        target_id = self.current_window_handle
+        target_id = await self.current_window_handle
         script = cdp.browser.get_window_for_target(target_id)
-        result = self.execute(cmd=script)
+        result = await self.execute(cmd=script)
         return result[0]
 
     @property
-    def window_handles(self) -> List[str]:
+    async def window_handles(self) -> List[str]:
         """Returns the handles of all windows within the current session.
 
         :Usage:
             ::
 
                 driver.window_handles
         """
         warnings.warn("window_handles aren't ordered by tab position")
         tabs = []
-        for target in self.targets:
+        for target in await self.targets:
             if target.type_ == "page":
                 tabs.append(target.target_id)
         return tabs
 
-    def set_window_state(self, state):
+    async def set_window_state(self, state):
         states = ["normal", "minimized", "maximized", "fullscreen"]
         if state not in states:
             raise ValueError(f"expected one of {states}, but got: {state}")
         window_id = self.current_window_id
         bounds = {"windowState": state}
-        self.execute_cdp_cmd("Browser.setWindowBounds", {"bounds": bounds, "windowId": window_id})
+        await self.execute_cdp_cmd("Browser.setWindowBounds", {"bounds": bounds, "windowId": window_id})
 
-    def normalize_window(self):
-        self.set_window_state("normal")
+    async def normalize_window(self):
+        await self.set_window_state("normal")
 
-    def maximize_window(self) -> None:
+    async def maximize_window(self) -> None:
         """Maximizes the current window that webdriver is using."""
-        self.normalize_window()
-        self.set_window_state("maximized")
+        await self.normalize_window()
+        await self.set_window_state("maximized")
 
-    def fullscreen_window(self) -> None:
+    async def fullscreen_window(self) -> None:
         """Invokes the window manager-specific 'full screen' operation."""
-        self.normalize_window()
-        self.set_window_state("fullscreen")
+        await self.normalize_window()
+        await self.set_window_state("fullscreen")
 
-    def minimize_window(self) -> None:
-        self.normalize_window()
+    async def minimize_window(self) -> None:
         """Invokes the window manager-specific 'minimize' operation."""
-        self.set_window_state("maximized")
+        await self.normalize_window()
+        await self.set_window_state("maximized")
 
-    def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
+    # noinspection PyUnusedLocal
+    async def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
         """Takes PDF of the current page.
 
-        The driver makes a best effort to return a PDF based on the
+        The driver makes the best effort to return a PDF based on the
         provided parameters.
         """
         from pycdp import cdp
         options = {}
         if print_options:
             options = print_options.to_dict()
             raise NotImplementedError()
 
-        page = self.execute(cmd=cdp.page.print_to_pdf())
+        page = await self.execute(cmd=cdp.page.print_to_pdf())
         return page[0]
 
     @property
     def switch_to(self) -> SwitchTo:
         """
         :Returns:
             - SwitchTo: an object containing all options to switch focus into
@@ -573,102 +491,108 @@
                 driver.switch_to.default_content()
                 driver.switch_to.frame('frame_name')
                 driver.switch_to.frame(1)
                 driver.switch_to.frame(driver.find_elements(By.TAG_NAME, "iframe")[0])
                 driver.switch_to.parent_frame()
                 driver.switch_to.window('main')
         """
-        raise NotImplementedError("You might use driver.switch_to_target(driver.targets[0].target_id.) instead")
-        # return self._switch_to
+        return self._switch_to
 
-    def switch_to_target(self, target_id):
-        from pycdp import cdp
-        self.session.close()
-        self.session = self._loop.run_until_complete(self._conn.connect_session(target_id))
-        self.execute(cmd=cdp.target.activate_target(self.current_window_handle))
-        return self.session
+    @property
+    async def _current_history_idx(self):
+        res = await self.execute_cdp_cmd("Page.getNavigationHistory")
+        return res["currentIndex"]
 
     # Navigation
-    def back(self) -> None:
+    async def back(self) -> None:
         """Goes one step backward in the browser history.
 
         :Usage:
             ::
 
                 driver.back()
         """
-        self.execute(Command.GO_BACK)
+        await self.execute_cdp_cmd("Page.navigateToHistoryEntry", {"entryId": await self._current_history_idx - 1})
 
-    def forward(self) -> None:
+    async def forward(self) -> None:
         """Goes one step forward in the browser history.
 
         :Usage:
             ::
 
                 driver.forward()
         """
-        self.execute(Command.GO_FORWARD)
+        await self.execute_cdp_cmd("Page.navigateToHistoryEntry", {"entryId": await self._current_history_idx + 1})
 
     async def refresh(self) -> None:
         """Refreshes the current page.
 
         :Usage:
             ::
 
                 driver.refresh()
         """
         from pycdp import cdp
-        self.execute(cmd=cdp.page.reload())
+        await self.execute(cmd=cdp.page.reload())
 
     # Options
-    def get_cookies(self) -> List[dict]:
+    async def get_cookies(self) -> List[dict]:
         """Returns a set of dictionaries, corresponding to cookies visible in
         the current session.
 
         :Usage:
             ::
 
                 driver.get_cookies()
         """
-        return self.execute(Command.GET_ALL_COOKIES)["value"]
+        cookies = await self.execute_cdp_cmd("Page.getCookies")
+        return cookies["cookies"]
 
-    def get_cookie(self, name) -> typing.Optional[typing.Dict]:
+    async def get_cookie(self, name) -> typing.Optional[typing.Dict]:
         """Get a single cookie by name. Returns the cookie if found, None if
         not.
 
         :Usage:
             ::
 
                 driver.get_cookie('my_cookie')
         """
-        with contextlib.suppress(NoSuchCookieException):
-            return self.execute(Command.GET_COOKIE, {"name": name})["value"]
+        for cookie in await self.get_cookies():
+            if cookie["name"] == name:
+                return cookie
         return None
 
-    def delete_cookie(self, name) -> None:
+    async def delete_cookie(self, name: str, url: str = None, domain: str = None, path: str = None) -> None:
         """Deletes a single cookie with the given name.
 
         :Usage:
             ::
 
                 driver.delete_cookie('my_cookie')
         """
-        self.execute(Command.DELETE_COOKIE, {"name": name})
+        args = {"name": name}
+        if url:
+            args["url"] = url
+        if domain:
+            args["domain"] = domain
+        if path:
+            args["path"] = path
+        await self.execute_cdp_cmd("Network.deleteCookies", args)
 
-    def delete_all_cookies(self) -> None:
+    async def delete_all_cookies(self) -> None:
         """Delete all cookies in the scope of the session.
 
         :Usage:
             ::
 
                 driver.delete_all_cookies()
         """
-        self.execute(Command.DELETE_ALL_COOKIES)
+        await self.execute_cdp_cmd("Network.clearBrowserCookies")
 
-    def add_cookie(self, cookie_dict) -> None:
+    async def add_cookie(self, cookie_dict) -> None:
         """Adds a cookie to your current session.
 
         :Args:
          - cookie_dict: A dictionary object, with required keys - "name" and "value";
             optional keys - "path", "domain", "secure", "httpOnly", "expiry", "sameSite"
 
         :Usage:
@@ -677,156 +601,140 @@
                 driver.add_cookie({'name' : 'foo', 'value' : 'bar'})
                 driver.add_cookie({'name' : 'foo', 'value' : 'bar', 'path' : '/'})
                 driver.add_cookie({'name' : 'foo', 'value' : 'bar', 'path' : '/', 'secure' : True})
                 driver.add_cookie({'name' : 'foo', 'value' : 'bar', 'sameSite' : 'Strict'})
         """
         if "sameSite" in cookie_dict:
             assert cookie_dict["sameSite"] in ["Strict", "Lax", "None"]
-            self.execute(Command.ADD_COOKIE, {"cookie": cookie_dict})
-        else:
-            self.execute(Command.ADD_COOKIE, {"cookie": cookie_dict})
+        await self.execute_cdp_cmd("Network.setCookie", cookie_dict)
 
     # Timeouts
-    def implicitly_wait(self, time_to_wait: float) -> None:
+    async def implicitly_wait(self, time_to_wait: float) -> None:
         """Sets a sticky timeout to implicitly wait for an element to be found,
         or a command to complete. This method only needs to be called one time
         per session. To set the timeout for calls to execute_async_script, see
         set_script_timeout.
 
         :Args:
          - time_to_wait: Amount of time to wait (in seconds)
 
         :Usage:
             ::
 
                 driver.implicitly_wait(30)
         """
-        self._loop.run_until_complete(asyncio.sleep(time_to_wait))
+        await asyncio.sleep(time_to_wait)
 
     def set_script_timeout(self, time_to_wait: float) -> None:
         """Set the amount of time that the script should wait during an
         execute_async_script call before throwing an error.
 
         :Args:
          - time_to_wait: The amount of time to wait (in seconds)
 
         :Usage:
             ::
 
                 driver.set_script_timeout(30)
         """
-        self.execute(Command.SET_TIMEOUTS, {"script": int(float(time_to_wait) * 1000)})
+        self._script_timeout = time_to_wait
 
     def set_page_load_timeout(self, time_to_wait: float) -> None:
         """Set the amount of time to wait for a page load to complete before
         throwing an error.
 
         :Args:
          - time_to_wait: The amount of time to wait
 
         :Usage:
             ::
 
                 driver.set_page_load_timeout(30)
         """
-        try:
-            self.execute(Command.SET_TIMEOUTS, {"pageLoad": int(float(time_to_wait) * 1000)})
-        except WebDriverException:
-            self.execute(Command.SET_TIMEOUTS, {"ms": float(time_to_wait) * 1000, "type": "page load"})
+        self._page_load_timeout = time_to_wait
 
     @property
-    def timeouts(self) -> Timeouts:
+    def timeouts(self) -> dict:
         """Get all the timeouts that have been set on the current session.
 
         :Usage:
             ::
 
                 driver.timeouts
         :rtype: Timeout
         """
-        timeouts = self.execute(Command.GET_TIMEOUTS)["value"]
-        timeouts["implicit_wait"] = timeouts.pop("implicit") / 1000
-        timeouts["page_load"] = timeouts.pop("pageLoad") / 1000
-        timeouts["script"] = timeouts.pop("script") / 1000
-        return Timeouts(**timeouts)
+        return {"page_load": self._page_load_timeout, "script": self._script_timeout}
 
     @timeouts.setter
-    def timeouts(self, timeouts) -> None:
-        # noinspection GrazieInspection
-        """Set all timeouts for the session. This will override any previously
-                set timeouts.
-
-                :Usage:
-                    ::
-                        my_timeouts = Timeouts()
-                        my_timeouts.implicit_wait = 10
-                        driver.timeouts = my_timeouts
-                """
-        _ = self.execute(Command.SET_TIMEOUTS, timeouts._to_json())["value"]
+    def timeouts(self, timeouts):
+        self._page_load_timeout = timeouts["page_load"]
+        self._script_timeout = timeouts["script"]
 
-    def find_element(self, by=By.ID, value: Optional[str] = None) -> WebElement:
+    # noinspection PyUnusedLocal
+    async def find_element(self, by=By.ID, value: Optional[str] = None) -> WebElement:
         """Find an element given a By strategy and locator.
 
         :Usage:
             ::
 
                 element = driver.find_element(By.ID, 'foo')
 
         :rtype: WebElement
         """
         # by = RelativeBy({by: value})
         if isinstance(by, RelativeBy):
-            elements = self.find_elements(by=by, value=value)
+            elements = await self.find_elements(by=by, value=value)
             if not elements:
                 raise NoSuchElementException(f"Cannot locate relative element with: {by.root}")
             return elements[0]
 
         if by == By.ID:
             by = By.CSS_SELECTOR
             value = f'[id="{value}"]'
         elif by == By.CLASS_NAME:
             by = By.CSS_SELECTOR
             value = f".{value}"
         elif by == By.NAME:
             by = By.CSS_SELECTOR
             value = f'[name="{value}"]'
 
-        return self.execute(Command.FIND_ELEMENT, {"using": by, "value": value})["value"]
+        raise NotImplementedError("not started with chromedriver")
 
-    def find_elements(self, by=By.ID, value: Optional[str] = None) -> List[WebElement]:
+    # noinspection PyUnusedLocal
+    async def find_elements(self, by=By.ID, value: Optional[str] = None) -> List[WebElement]:
         """Find elements given a By strategy and locator.
 
         :Usage:
             ::
 
                 elements = driver.find_elements(By.CLASS_NAME, 'foo')
 
         :rtype: list of WebElement
         """
         from selenium_driverless.utils.utils import sel_path, read
-        by = RelativeBy({by: value})
+        # by = RelativeBy({by: value})
         if isinstance(by, RelativeBy):
             _pkg = ".".join(__name__.split(".")[:-1])
             raw_function = read(sel_path() + "webdriver/remote/findElements.js", sel_root=False)
             find_element_js = f"/* findElements */return ({raw_function}).apply(null, arguments);"
-            return self.execute_script(find_element_js, by.to_dict())
+            return await self.execute_script(find_element_js, by.to_dict())
 
         if by == By.ID:
             by = By.CSS_SELECTOR
             value = f'[id="{value}"]'
         elif by == By.CLASS_NAME:
             by = By.CSS_SELECTOR
             value = f".{value}"
         elif by == By.NAME:
             by = By.CSS_SELECTOR
             value = f'[name="{value}"]'
 
         # Return empty list if driver returns null
         # See https://github.com/SeleniumHQ/selenium/issues/4555
-        return self.execute(Command.FIND_ELEMENTS, {"using": by, "value": value})["value"] or []
+        raise NotImplementedError("not started with chromedriver")
 
     @property
     def capabilities(self) -> dict:
         """returns the drivers current capabilities being used."""
         return self.caps
 
     async def get_screenshot_as_file(self, filename) -> bool:
@@ -845,153 +753,153 @@
                         driver.get_screenshot_as_file('/Screenshots/foo.png')
                 """
         if not str(filename).lower().endswith(".png"):
             warnings.warn(
                 "name used for saved screenshot does not match file " "type. It should end with a `.png` extension",
                 UserWarning,
             )
-        png = self.get_screenshot_as_png()
+        png = await self.get_screenshot_as_png()
         try:
             with open(filename, "wb") as f:
                 f.write(png)
         except OSError:
             return False
         finally:
             del png
         return True
 
-    def save_screenshot(self, filename) -> bool:
+    async def save_screenshot(self, filename) -> bool:
         # noinspection GrazieInspection
         """Saves a screenshot of the current window to a PNG image file.
                 Returns False if there is any IOError, else returns True. Use full
                 paths in your filename.
 
                 :Args:
                  - filename: The full path you wish to save your screenshot to. This
                    should end with a `.png` extension.
 
                 :Usage:
                     ::
 
                         driver.save_screenshot('/Screenshots/foo.png')
                 """
-        return self.get_screenshot_as_file(filename)
+        return await self.get_screenshot_as_file(filename)
 
-    def get_screenshot_as_png(self) -> bytes:
+    async def get_screenshot_as_png(self) -> bytes:
         """Gets the screenshot of the current window as a binary data.
 
         :Usage:
             ::
 
                 driver.get_screenshot_as_png()
         """
-        base_64 = self.get_screenshot_as_base64()
+        base_64 = await self.get_screenshot_as_base64()
         return b64decode(base_64.encode("ascii"))
 
-    def get_screenshot_as_base64(self) -> str:
+    async def get_screenshot_as_base64(self) -> str:
         """Gets the screenshot of the current window as a base64 encoded string
         which is useful in embedded images in HTML.
 
         :Usage:
             ::
 
                 driver.get_screenshot_as_base64()
         """
         from pycdp import cdp
-        return self.execute(cmd=cdp.page.capture_screenshot(format_="png"))
+        return await self.execute(cmd=cdp.page.capture_screenshot(format_="png"))
 
     # noinspection PyPep8Naming
-    def set_window_size(self, width, height, windowHandle: str = "current") -> None:
+    async def set_window_size(self, width, height, windowHandle: str = "current") -> None:
         """Sets the width and height of the current window. (window.resizeTo)
 
         :Args:
          - width: the width in pixels to set the window to
          - height: the height in pixels to set the window to
 
         :Usage:
             ::
 
                 driver.set_window_size(800,600)
         """
         if windowHandle != "current":
             warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
-        self.set_window_rect(width=int(width), height=int(height))
+        await self.set_window_rect(width=int(width), height=int(height))
 
     # noinspection PyPep8Naming
-    def get_window_size(self, windowHandle: str = "current") -> dict:
+    async def get_window_size(self, windowHandle: str = "current") -> dict:
         """Gets the width and height of the current window.
 
         :Usage:
             ::
 
                 driver.get_window_size()
         """
 
         if windowHandle != "current":
             warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
-        size = self.get_window_rect()
+        size = await self.get_window_rect()
 
         if size.get("value", None):
             size = size["value"]
 
         return {k: size[k] for k in ("width", "height")}
 
     # noinspection PyPep8Naming
-    def set_window_position(self, x, y, windowHandle: str = "current") -> dict:
+    async def set_window_position(self, x, y, windowHandle: str = "current") -> dict:
         """Sets the x,y position of the current window. (window.moveTo)
 
         :Args:
          - x: the x-coordinate in pixels to set the window position
          - y: the y-coordinate in pixels to set the window position
 
         :Usage:
             ::
 
                 driver.set_window_position(0,0)
         """
         if windowHandle != "current":
             warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
-        return self.set_window_rect(x=int(x), y=int(y))
+        return await self.set_window_rect(x=int(x), y=int(y))
 
     # noinspection PyPep8Naming
-    def get_window_position(self, windowHandle="current") -> dict:
+    async def get_window_position(self, windowHandle="current") -> dict:
         """Gets the x,y position of the current window.
 
         :Usage:
             ::
 
                 driver.get_window_position()
         """
 
         if windowHandle != "current":
             warnings.warn("Only 'current' window is supported for W3C compatible browsers.")
-        position = self.get_window_rect()
+        position = await self.get_window_rect()
 
         return {k: position[k] for k in ("x", "y")}
 
-    def get_window_rect(self) -> dict:
+    async def get_window_rect(self) -> dict:
         """Gets the x, y coordinates of the window as well as height and width
         of the current window.
 
         :Usage:
             ::
 
                 driver.get_window_rect()
         """
         from pycdp import cdp
-        script = cdp.browser.get_window_bounds(self.current_window_id)
-        bounds = self.execute(cmd=script)
+        script = cdp.browser.get_window_bounds(await self.current_window_id)
+        bounds = await self.execute(cmd=script)
         json = bounds.to_json()
         json["x"] = json["left"]
         del json["left"]
         json["y"] = json["top"]
         del json["top"]
         return json
 
-    def set_window_rect(self, x=None, y=None, width=None, height=None) -> dict:
+    async def set_window_rect(self, x=None, y=None, width=None, height=None) -> dict:
         """Sets the x, y coordinates of the window as well as height and width
         of the current window. This method is only supported for W3C compatible
         browsers; other browsers should use `set_window_position` and
         `set_window_size`.
 
         :Usage:
             ::
@@ -1005,16 +913,16 @@
         if (x is None and y is None) and (not height and not width):
             raise InvalidArgumentException("x and y or height and width need values")
 
         json = {"left": x, "top": y, "width": width, 'height': height}
         bounds = cdp.browser.Bounds()
         bounds = bounds.from_json(json=json)
 
-        script = cdp.browser.set_window_bounds(self.current_window_id, bounds)
-        self.execute(cmd=script)
+        script = cdp.browser.set_window_bounds(await self.current_window_id, bounds)
+        await self.execute(cmd=script)
         json["x"] = json["left"]
         del json["left"]
         json["y"] = json["top"]
         del json["top"]
 
         return json
 
@@ -1045,15 +953,15 @@
         """Gets the current orientation of the device.
 
         :Usage:
             ::
 
                 orientation = driver.orientation
         """
-        return self.execute(Command.GET_SCREEN_ORIENTATION)["value"]
+        raise NotImplementedError()
 
     @orientation.setter
     def orientation(self, value) -> None:
         """Sets the current orientation of the device.
 
         :Args:
          - value: orientation to set it to.
@@ -1061,35 +969,29 @@
         :Usage:
             ::
 
                 driver.orientation = 'landscape'
         """
         allowed_values = ["LANDSCAPE", "PORTRAIT"]
         if value.upper() in allowed_values:
-            self.execute(Command.SET_SCREEN_ORIENTATION, {"orientation": value})
+            raise NotImplementedError()
         else:
             raise WebDriverException("You can only set the orientation to 'LANDSCAPE' and 'PORTRAIT'")
 
     @property
-    def application_cache(self):
-        """Returns a ApplicationCache Object to interact with the browser app
-        cache."""
-        return ApplicationCache(self)
-
-    @property
     def log_types(self):
         """Gets a list of the available log types. This only works with w3c
         compliant browsers.
 
         :Usage:
             ::
 
                 driver.log_types
         """
-        return self.execute(Command.GET_AVAILABLE_LOG_TYPES)["value"]
+        raise NotImplementedError("not started with chromedriver")
 
     def get_log(self, log_type):
         """Gets the log for a given log type.
 
         :Args:
          - log_type: type of log that which will be returned
 
@@ -1097,15 +999,15 @@
             ::
 
                 driver.get_log('browser')
                 driver.get_log('driver')
                 driver.get_log('client')
                 driver.get_log('server')
         """
-        return self.execute(Command.GET_LOG, {"type": log_type})["value"]
+        raise NotImplementedError("not started with chromedriver")
 
     @asynccontextmanager
     async def bidi_connection(self):
         cdp = import_cdp()
         if self.caps.get("se:cdp"):
             ws_url = self.caps.get("se:cdp")
             version = self.caps.get("se:cdpVersion").split(".")[0]
@@ -1140,86 +1042,89 @@
         version = re.search(r".*/(\d+)\.", browser_version).group(1)
 
         return version, websocket_url
 
     # Virtual Authenticator Methods
     def add_virtual_authenticator(self, options: VirtualAuthenticatorOptions) -> None:
         """Adds a virtual authenticator with the given options."""
-        self._authenticator_id = self.execute(Command.ADD_VIRTUAL_AUTHENTICATOR, options.to_dict())["value"]
+        # self._authenticator_id = self.execute(Command.ADD_VIRTUAL_AUTHENTICATOR, options.to_dict())["value"]
+        raise NotImplementedError("not started with chromedriver")
 
     @property
     def virtual_authenticator_id(self) -> str:
         """Returns the id of the virtual authenticator."""
-        return self._authenticator_id
+        raise NotImplementedError("not started with chromedriver")
+        # return self._authenticator_id
 
     @required_virtual_authenticator
     def remove_virtual_authenticator(self) -> None:
         """Removes a previously added virtual authenticator.
 
         The authenticator is no longer valid after removal, so no
         methods may be called.
         """
-        self.execute(Command.REMOVE_VIRTUAL_AUTHENTICATOR, {"authenticatorId": self._authenticator_id})
-        self._authenticator_id = None
+        raise NotImplementedError("not started with chromedriver")
+        # self._authenticator_id = None
 
     @required_virtual_authenticator
     def add_credential(self, credential: Credential) -> None:
         """Injects a credential into the authenticator."""
-        self.execute(Command.ADD_CREDENTIAL, {**credential.to_dict(), "authenticatorId": self._authenticator_id})
+        raise NotImplementedError("not started with chromedriver")
 
+    # noinspection PyTypeChecker
     @required_virtual_authenticator
     def get_credentials(self) -> List[Credential]:
         """Returns the list of credentials owned by the authenticator."""
-        credential_data = self.execute(Command.GET_CREDENTIALS, {"authenticatorId": self._authenticator_id})
-        return [Credential.from_dict(credential) for credential in credential_data["value"]]
+        # credential_data = self.execute(Command.GET_CREDENTIALS, {"authenticatorId": self._authenticator_id})
+        raise NotImplementedError("not started with chromedriver")
 
     @required_virtual_authenticator
     def remove_credential(self, credential_id: Union[str, bytearray]) -> None:
         """Removes a credential from the authenticator."""
         # Check if the credential is bytearray converted to b64 string
         if isinstance(credential_id, bytearray):
+            # noinspection PyUnusedLocal
             credential_id = urlsafe_b64encode(credential_id).decode()
 
-        self.execute(
-            Command.REMOVE_CREDENTIAL, {"credentialId": credential_id, "authenticatorId": self._authenticator_id}
-        )
+        raise NotImplementedError("not started with chromedriver")
 
     @required_virtual_authenticator
     def remove_all_credentials(self) -> None:
         """Removes all credentials from the authenticator."""
-        self.execute(Command.REMOVE_ALL_CREDENTIALS, {"authenticatorId": self._authenticator_id})
+        raise NotImplementedError("not started with chromedriver")
 
     @required_virtual_authenticator
     def set_user_verified(self, verified: bool) -> None:
         """Sets whether the authenticator will simulate success or fail on user
         verification.
 
         verified: True if the authenticator will pass user verification, False otherwise.
         """
-        self.execute(Command.SET_USER_VERIFIED, {"authenticatorId": self._authenticator_id, "isUserVerified": verified})
+        raise NotImplementedError("not started with chromedriver")
 
     #
     # selenium.webdriver.chrome.WebDriver props from here on
     #
 
+    # noinspection PyShadowingBuiltins
     def launch_app(self, id):
         """Launches Chromium app specified by id."""
-        return self.execute("launchApp", {"id": id})
+        raise NotImplementedError("not started with chromedriver")
 
-    def get_network_conditions(self):
+    async def get_network_conditions(self):
         """Gets Chromium network emulation settings.
 
         :Returns:
             A dict. For example:
             {'latency': 4, 'download_throughput': 2, 'upload_throughput': 2,
             'offline': False}
         """
-        return self.execute("getNetworkConditions")["value"]
+        raise NotImplementedError("not started with chromedriver")
 
-    def set_network_conditions(self, **network_conditions) -> None:
+    async def set_network_conditions(self, **network_conditions) -> None:
         """Sets Chromium network emulation settings.
 
         :Args:
          - network_conditions: A dict with conditions specification.
 
         :Usage:
             ::
@@ -1229,21 +1134,21 @@
                     latency=5,  # additional latency (ms)
                     download_throughput=500 * 1024,  # maximal throughput
                     upload_throughput=500 * 1024)  # maximal throughput
 
             Note: 'throughput' can be used to set both (for download and upload).
         """
         from pycdp import cdp
-        self.execute(cmd=cdp.network.emulate_network_conditions(**network_conditions))
+        await self.execute(cmd=cdp.network.emulate_network_conditions(**network_conditions))
 
     def delete_network_conditions(self) -> None:
         """Resets Chromium network emulation settings."""
-        self.execute("deleteNetworkConditions")
+        raise NotImplementedError("not started with chromedriver")
 
-    def set_permissions(self, name: str, value: str, origin: str = None) -> None:
+    async def set_permissions(self, name: str, value: str, origin: str = None) -> None:
         """Sets Applicable Permission.
 
         :Args:
          - name: The item to set the permission on.
          - value: The value to set on the item
 
         :Usage:
@@ -1253,18 +1158,17 @@
         """
         settings = ["granted", "denied", "prompt"]
         if value not in settings:
             raise ValueError(f"value needs to be within {settings}, but got {value}")
         args = {"permission": {"name": name}, "setting": value}
         if origin:
             args["origin"] = origin
-        from pycdp import cdp
-        self.execute_cdp_cmd("Browser.setPermission", args)
+        await self.execute_cdp_cmd("Browser.setPermission", args)
 
-    def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None):
+    async def execute_cdp_cmd(self, cmd: str, cmd_args: dict or None = None):
         """Execute Chrome Devtools Protocol command and get returned result The
         command and command args should follow chrome devtools protocol
         domains/commands, refer to link
         https://chromedevtools.github.io/devtools-protocol/
 
         :Args:
          - cmd: A str, command name
@@ -1283,54 +1187,55 @@
 
         def execute_cdp_cmd(_cmd_dict):
             json = yield _cmd_dict
             return json
 
         cmd_dict = dict(method=cmd, params=cmd_args)
         request = execute_cdp_cmd(cmd_dict)
-        return self.execute(cmd=request)
+        return await self.execute(cmd=request)
 
-    def get_sinks(self) -> list:
+    # noinspection PyTypeChecker
+    async def get_sinks(self) -> list:
         """
         :Returns: A list of sinks available for Cast.
         """
-        self.execute_cdp_cmd("Cast.enable")
-        return self.execute("getSinks")["value"]
+        await self.execute_cdp_cmd("Cast.enable")
+        raise NotImplementedError("not started with chromedriver")
 
-    def get_issue_message(self):
+    async def get_issue_message(self):
         """
         :Returns: An error message when there is any issue in a Cast session.
         """
-        return self.execute("getIssueMessage")["value"]
+        raise NotImplementedError("not started with chromedriver")
 
-    def set_sink_to_use(self, sink_name: str) -> dict:
+    async def set_sink_to_use(self, sink_name: str) -> dict:
         """Sets a specific sink, using its name, as a Cast session receiver
         target.
 
         :Args:
          - sink_name: Name of the sink to use as the target.
         """
-        return self.execute_cdp_cmd("Cast.setSinkToUse", {"sinkName": sink_name})
+        return await self.execute_cdp_cmd("Cast.setSinkToUse", {"sinkName": sink_name})
 
-    def start_desktop_mirroring(self, sink_name: str) -> dict:
+    async def start_desktop_mirroring(self, sink_name: str) -> dict:
         """Starts a desktop mirroring session on a specific receiver target.
 
         :Args:
          - sink_name: Name of the sink to use as the target.
         """
-        return self.execute_cdp_cmd("Cast.startDesktopMirrorin", {"sinkName": sink_name})
+        return await self.execute_cdp_cmd("Cast.startDesktopMirrorin", {"sinkName": sink_name})
 
-    def start_tab_mirroring(self, sink_name: str) -> dict:
+    async def start_tab_mirroring(self, sink_name: str) -> dict:
         """Starts a tab mirroring session on a specific receiver target.
 
         :Args:
          - sink_name: Name of the sink to use as the target.
         """
-        return self.execute_cdp_cmd("Cast.startTabMirroring", {"sinkName": sink_name})
+        return await self.execute_cdp_cmd("Cast.startTabMirroring", {"sinkName": sink_name})
 
-    def stop_casting(self, sink_name: str) -> dict:
+    async def stop_casting(self, sink_name: str) -> dict:
         """Stops the existing Cast session on a specific receiver target.
 
         :Args:
          - sink_name: Name of the sink to stop the Cast session.
         """
-        return self.execute_cdp_cmd("Cast.stopCasting", {"sinkName": sink_name})
+        return await self.execute_cdp_cmd("Cast.stopCasting", {"sinkName": sink_name})
```

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium-driverless
-Version: 1.0.4
+Name: selenium_driverless
+Version: 1.1
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
@@ -46,17 +46,40 @@
 
 * [Windows] Install [Chrome-Browser](https://www.google.de/chrome/)
 * ```pip install selenium-driverless```
 
 
 ### Usage
 
-#### example script
+#### with asyncio
 ```python
 from selenium_driverless import webdriver
+import asyncio
+
+
+async def main():
+    options = webdriver.Options()
+    async with webdriver.Chrome(options=options) as driver:
+        await driver.get('http://nowsecure.nl#relax')
+        await driver.implicitly_wait(3)
+
+        title = await driver.title
+        url = await driver.current_url
+        source = await driver.page_source
+        print(title)
+
+
+asyncio.run(main())
+```
+
+#### synchronous
+asyncified, might be buggy
+
+```python
+from selenium_driverless.sync import webdriver
 
 options = webdriver.Options()
 with webdriver.Chrome(options=options) as driver:
     driver.get('http://nowsecure.nl#relax')
     driver.implicitly_wait(3)
     
     title = driver.title
@@ -67,15 +90,15 @@
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- implementations
+- [ ] page-interactions
   - [ ] find element
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
```

### Comparing `selenium_driverless-1.0.4/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.1/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 src/selenium_driverless.egg-info/PKG-INFO
 src/selenium_driverless.egg-info/SOURCES.txt
 src/selenium_driverless.egg-info/dependency_links.txt
 src/selenium_driverless.egg-info/requires.txt
 src/selenium_driverless.egg-info/top_level.txt
 src/selenium_driverless/files/__init__.py
 src/selenium_driverless/scripts/__init__.py
+src/selenium_driverless/scripts/alert.py
+src/selenium_driverless/scripts/cdp_listener.py
 src/selenium_driverless/scripts/mobile.py
-src/selenium_driverless/scripts/multi_thread.py
 src/selenium_driverless/scripts/options.py
+src/selenium_driverless/scripts/switch_to.py
 src/selenium_driverless/utils/__init__.py
 src/selenium_driverless/utils/utils.py
 tests/test_driverless.py
```

### Comparing `selenium_driverless-1.0.4/tests/test_driverless.py` & `selenium_driverless-1.1/tests/test_driverless.py`

 * *Files identical despite different names*

