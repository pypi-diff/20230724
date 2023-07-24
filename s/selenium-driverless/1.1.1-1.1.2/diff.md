# Comparing `tmp/selenium_driverless-1.1.1.tar.gz` & `tmp/selenium_driverless-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_driverless-1.1.1.tar", last modified: Mon Jul 24 18:57:51 2023, max compression
+gzip compressed data, was "selenium_driverless-1.1.2.tar", last modified: Mon Jul 24 20:26:45 2023, max compression
```

## Comparing `selenium_driverless-1.1.1.tar` & `selenium_driverless-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.896141 selenium_driverless-1.1.1/
--rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3757 2023-07-24 18:57:51.896141 selenium_driverless-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2023-07-24 18:55:54.000000 selenium_driverless-1.1.1/README.md
--rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.1.1/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-07-24 18:57:51.897180 selenium_driverless-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.872388 selenium_driverless-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.879987 selenium_driverless-1.1.1/src/selenium_driverless/
--rw-rw-rw-   0        0        0       23 2023-07-24 18:57:33.000000 selenium_driverless-1.1.1/src/selenium_driverless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.886060 selenium_driverless-1.1.1/src/selenium_driverless/files/
--rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.1.1/src/selenium_driverless/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.892140 selenium_driverless-1.1.1/src/selenium_driverless/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/__init__.py
--rw-rw-rw-   0        0        0     2820 2023-07-23 16:18:48.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/alert.py
--rw-rw-rw-   0        0        0    16993 2023-07-23 15:23:23.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/cdp_listener.py
--rw-rw-rw-   0        0        0     2720 2023-07-21 20:13:40.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/mobile.py
--rw-rw-rw-   0        0        0    16797 2023-07-23 12:34:39.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/options.py
--rw-rw-rw-   0        0        0     5281 2023-07-23 16:28:03.000000 selenium_driverless-1.1.1/src/selenium_driverless/scripts/switch_to.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.894144 selenium_driverless-1.1.1/src/selenium_driverless/utils/
--rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.1.1/src/selenium_driverless/utils/__init__.py
--rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.1.1/src/selenium_driverless/utils/utils.py
--rw-rw-rw-   0        0        0    43597 2023-07-24 18:27:59.000000 selenium_driverless-1.1.1/src/selenium_driverless/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.885061 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/
--rw-rw-rw-   0        0        0     3757 2023-07-24 18:57:51.000000 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-07-24 18:57:51.000000 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 18:57:51.000000 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-24 18:57:51.000000 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 18:57:51.000000 selenium_driverless-1.1.1/src/selenium_driverless.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 18:57:51.895142 selenium_driverless-1.1.1/tests/
--rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.1.1/tests/test_driverless.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.731538 selenium_driverless-1.1.2/
+-rw-rw-rw-   0        0        0      688 2023-07-21 13:27:27.000000 selenium_driverless-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0       89 2023-01-11 09:10:16.000000 selenium_driverless-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3757 2023-07-24 20:26:45.731538 selenium_driverless-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2441 2023-07-24 18:55:54.000000 selenium_driverless-1.1.2/README.md
+-rw-rw-rw-   0        0        0      567 2023-07-21 21:05:54.000000 selenium_driverless-1.1.2/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_driverless-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-07-24 20:26:45.733540 selenium_driverless-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1818 2023-07-23 19:27:35.000000 selenium_driverless-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.710384 selenium_driverless-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.718449 selenium_driverless-1.1.2/src/selenium_driverless/
+-rw-rw-rw-   0        0        0       23 2023-07-24 20:26:26.000000 selenium_driverless-1.1.2/src/selenium_driverless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.724491 selenium_driverless-1.1.2/src/selenium_driverless/files/
+-rw-rw-rw-   0        0        0        0 2023-07-21 16:36:38.000000 selenium_driverless-1.1.2/src/selenium_driverless/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.727491 selenium_driverless-1.1.2/src/selenium_driverless/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2868 2023-07-24 19:21:37.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/alert.py
+-rw-rw-rw-   0        0        0    16797 2023-07-23 12:34:39.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/options.py
+-rw-rw-rw-   0        0        0     5596 2023-07-24 19:39:32.000000 selenium_driverless-1.1.2/src/selenium_driverless/scripts/switch_to.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.729491 selenium_driverless-1.1.2/src/selenium_driverless/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-21 21:02:48.000000 selenium_driverless-1.1.2/src/selenium_driverless/utils/__init__.py
+-rw-rw-rw-   0        0        0     3625 2023-07-22 16:31:37.000000 selenium_driverless-1.1.2/src/selenium_driverless/utils/utils.py
+-rw-rw-rw-   0        0        0    44016 2023-07-24 20:22:53.000000 selenium_driverless-1.1.2/src/selenium_driverless/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.723491 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/
+-rw-rw-rw-   0        0        0     3757 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-24 20:26:45.000000 selenium_driverless-1.1.2/src/selenium_driverless.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 20:26:45.730491 selenium_driverless-1.1.2/tests/
+-rw-rw-rw-   0        0        0     3238 2023-01-12 15:12:48.000000 selenium_driverless-1.1.2/tests/test_driverless.py
```

### Comparing `selenium_driverless-1.1.1/LICENSE.md` & `selenium_driverless-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/PKG-INFO` & `selenium_driverless-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_driverless
-Version: 1.1.1
+Version: 1.1.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.1.1/README.md` & `selenium_driverless-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/build_upload.md` & `selenium_driverless-1.1.2/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/setup.py` & `selenium_driverless-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless/scripts/alert.py` & `selenium_driverless-1.1.2/src/selenium_driverless/scripts/alert.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,36 +51,36 @@
 
         :Args:
          - driver: The WebDriver instance which performs user actions.
         """
         self.driver = driver
 
     @property
-    def text(self) -> str:
+    async def text(self) -> str:
         """Gets the text of the Alert."""
-        return self.driver.execute(Command.W3C_GET_ALERT_TEXT)["value"]
+        return await self.driver.execute(Command.W3C_GET_ALERT_TEXT)["value"]
 
-    def dismiss(self) -> None:
+    async def dismiss(self) -> None:
         """Dismisses the alert available."""
         from pycdp import cdp
-        self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=False))
+        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=False))
 
-    def accept(self) -> None:
+    async def accept(self) -> None:
         """Accepts the alert available.
 
         :Usage:
             ::
 
                 Alert(driver).accept() # Confirm a alert dialog.
         """
         from pycdp import cdp
-        self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True))
+        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True))
 
     # noinspection PyPep8Naming
-    def send_keys(self, keysToSend: str) -> None:
+    async def send_keys(self, keysToSend: str) -> None:
         """Send Keys to the Alert.
 
         :Args:
          - keysToSend: The text to be sent to Alert.
         """
         from pycdp import cdp
-        self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True, prompt_text=keysToSend))
+        await self.driver.execute(cmd=cdp.page.handle_java_script_dialog(accept=True, prompt_text=keysToSend))
```

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless/scripts/options.py` & `selenium_driverless-1.1.2/src/selenium_driverless/scripts/options.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless/scripts/switch_to.py` & `selenium_driverless-1.1.2/src/selenium_driverless/scripts/switch_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,62 +19,67 @@
 
 from typing import Optional
 from typing import Union
 import warnings
 
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import NoSuchFrameException
-from selenium_driverless.scripts.alert import Alert
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 
 from selenium.webdriver.remote.command import Command
 
+from selenium_driverless.scripts.alert import Alert
+from selenium_driverless.sync.alert import Alert as SyncAlert
+
 
 class SwitchTo:
     def __init__(self, driver) -> None:
+        self._loop = None
         import weakref
-
         self._driver = weakref.proxy(driver)
 
     @property
     def active_element(self) -> WebElement:
         """Returns the element with focus, or BODY if nothing has focus.
 
         :Usage:
             ::
 
                 element = driver.switch_to.active_element
         """
         raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
 
     @property
-    def alert(self) -> Alert:
+    async def alert(self) -> Alert:
         """Switches focus to an alert on the page.
 
         :Usage:
             ::
 
                 alert = driver.switch_to.alert
         """
-        alert = Alert(self._driver)
+        if self._loop:
+            alert = SyncAlert(self._driver, loop=self._loop)
+        else:
+            alert = Alert(self._driver)
         warnings.warn("can't detect if a alert exists yet")
         return alert
 
-    def default_content(self) -> None:
+    async def default_content(self) -> None:
         """Switch focus to the default frame.
 
         :Usage:
             ::
 
                 driver.switch_to.default_content()
         """
         raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
 
-    def frame(self, frame_reference: Union[str, int, WebElement]) -> None:
+    async def frame(self, frame_reference: Union[str, int, WebElement]) -> None:
         """Switches focus to the specified frame, by index, name, or
         webelement.
 
         :Args:
          - frame_reference: The name of the window to switch to, an integer representing the index,
                             or a webelement that is an (i)frame to switch to.
 
@@ -83,32 +88,32 @@
 
                 driver.switch_to.frame('frame_name')
                 driver.switch_to.frame(1)
                 driver.switch_to.frame(driver.find_elements(By.TAG_NAME, "iframe")[0])
         """
         if isinstance(frame_reference, str):
             try:
-                frame_reference = self._driver.find_element(By.ID, frame_reference)
+                frame_reference = await self._driver.find_element(By.ID, frame_reference)
             except NoSuchElementException:
                 try:
-                    frame_reference = self._driver.find_element(By.NAME, frame_reference)
+                    frame_reference = await self._driver.find_element(By.NAME, frame_reference)
                 except NoSuchElementException:
                     raise NoSuchFrameException(frame_reference)
 
         raise NotImplementedError("You might use driver.switch_to.target(driver.targets[0].target_id)")
 
-    def target(self, target_id):
+    async def target(self, target_id):
         from pycdp import cdp
         self._driver.session.close()
         # noinspection PyProtectedMember
-        self._driver.session = self._driver._loop.run_until_complete(self._driver._conn.connect_session(target_id))
-        self._driver.execute(cmd=cdp.target.activate_target(self._driver.current_window_handle))
+        self._driver.session = await self._driver._conn.connect_session(target_id)
+        await self._driver.execute(cmd=cdp.target.activate_target(await self._driver.current_window_handle))
         return self._driver.session
 
-    def new_window(self, type_hint: Optional[str] = "tab", url="") -> None:
+    async def new_window(self, type_hint: Optional[str] = "tab", url="") -> None:
         """Switches to a new top-level browsing context.
 
         The type hint can be one of "tab" or "window". If not specified the
         browser will automatically select it.
 
         :Usage:
             ::
@@ -119,32 +124,34 @@
         new_tab = False
         if type_hint == "window":
             new_window = True
         if type_hint == "tab":
             new_window = True
         from pycdp import cdp
         cmd = cdp.target.create_target(url=url, new_window=new_window, for_tab=new_tab)
-        return self._driver.execute(cmd=cmd)
+        target_id = await self._driver.execute(cmd=cmd)
+        await self.target(target_id)
+        return target_id
 
-    def parent_frame(self) -> None:
+    async def parent_frame(self) -> None:
         """Switches focus to the parent context. If the current context is the
         top level browsing context, the context remains unchanged.
 
         :Usage:
             ::
 
                 driver.switch_to.parent_frame()
         """
-        self._driver.execute(Command.SWITCH_TO_PARENT_FRAME)
+        await self._driver.execute(Command.SWITCH_TO_PARENT_FRAME)
 
-    def window(self, window_name) -> None:
+    async def window(self, window_name) -> None:
         """Switches focus to the specified window.
 
         :Args:
          - window_name: The name or window handle of the window to switch to.
 
         :Usage:
             ::
 
                 driver.switch_to.window('main')
         """
-        self.target(window_name)
+        await self.target(window_name)
```

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless/utils/utils.py` & `selenium_driverless-1.1.2/src/selenium_driverless/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless/webdriver.py` & `selenium_driverless-1.1.2/src/selenium_driverless/webdriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 from selenium.webdriver.remote.bidi_connection import BidiConnection
 from selenium.webdriver.remote.file_detector import FileDetector
 from selenium.webdriver.remote.file_detector import LocalFileDetector
 from selenium.webdriver.remote.script_key import ScriptKey
 from selenium.webdriver.remote.webdriver import create_matches
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.relative_locator import RelativeBy
+from selenium.webdriver.remote.mobile import Mobile
 
-from selenium_driverless.scripts.mobile import Mobile
 from selenium_driverless.scripts.options import Options
 from selenium_driverless.scripts.switch_to import SwitchTo
+from selenium_driverless.sync.switch_to import SwitchTo as SyncSwitchTo
 
 
 def import_cdp():
     return import_module("selenium.webdriver.common.bidi.cdp")
 
 
 class BaseWebDriver(metaclass=ABCMeta):
@@ -78,16 +79,17 @@
     ) -> None:
         """Creates a new instance of the chrome driver. Starts the service and
         then creates new instance of chrome driver.
 
         :Args:
          - options - this takes an instance of ChromeOptions
         """
-        self._page_load_timeout = None
-        self._script_timeout = None
+        self._loop = None
+        self._page_load_timeout = 300
+        self._script_timeout = 30
         self._conn = None
         self.session = None
         self.browser_pid = None
 
         try:
             options = options or Options()
             self._options = options
@@ -175,14 +177,17 @@
         if not capabilities:
             capabilities = self._capabilities
         del self._capabilities
         from selenium_driverless.utils.utils import IS_POSIX, read
         from pycdp.asyncio import connect_cdp
         from pycdp import cdp
 
+        if self._loop:
+            self._switch_to = SyncSwitchTo(driver=self, loop=self._loop)
+
         options = capabilities["goog:chromeOptions"]
 
         browser = subprocess.Popen(
             [options["binary"], *options["args"]],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
@@ -282,15 +287,15 @@
                 raise JavascriptException("Pinned script could not be found")
 
         script = f"(function(...arguments){{{script}}})(...{json.dumps(args)})"
 
         script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
                                       user_gesture=True, await_promise=False,
                                       allow_unsafe_eval_blocked_by_csp=True, return_by_value=True)
-        result = await self.execute(cmd=script)
+        result = await asyncio.wait_for(self.execute(cmd=script), self._script_timeout)
         if result[1]:
             class JSEvalException(result[1], Exception):
                 pass
 
             raise JSEvalException(result[1].description)
         return result[0].value
 
@@ -310,19 +315,21 @@
         """
         from pycdp import cdp
         import json
         script = """
         (function(...arguments){
             const promise = new Promise((resolve, reject) => {
                 arguments.push(resolve)
-            });""" + script + "return promise})(..." + json.dumps(args) + ")"
+            });""" + script + ";return promise})(..." + json.dumps(args) + ")"
+        timeout = cdp.runtime.TimeDelta
+        timeout = timeout.from_json(self._script_timeout)
         script = cdp.runtime.evaluate(expression=script, include_command_line_api=True,
                                       user_gesture=True, await_promise=True,
-                                      allow_unsafe_eval_blocked_by_csp=True, timeout=self._script_timeout)
-        result = await self.execute(cmd=script)
+                                      allow_unsafe_eval_blocked_by_csp=True, timeout=timeout)
+        result = await asyncio.wait_for(self.execute(cmd=script), timeout=self._script_timeout)
         if result[1]:
             raise Exception(result[1].description)
         return result[0].value
 
     @property
     async def current_url(self) -> str:
         """Gets the URL of the current page.
@@ -351,30 +358,32 @@
 
         :Usage:
             ::
 
                 driver.close()
         """
         from pycdp import cdp
+        window_handles = await self.window_handles
         await self.execute(cmd=cdp.page.close())
+        await self.switch_to.window(window_handles[0])
 
     async def quit(self) -> None:
         """Quits the driver and closes every associated window.
 
         :Usage:
             ::
 
                 driver.quit()
         """
         import os
         import shutil
         # noinspection PyBroadException,PyUnusedLocal
         try:
             try:
-                await self.close()
+                await self._conn.close()
 
                 # wait for process to be killed
                 while True:
                     try:
                         os.kill(self.browser_pid, 15)
                     except OSError:
                         break
@@ -424,26 +433,25 @@
         """Returns the handles of all windows within the current session.
 
         :Usage:
             ::
 
                 driver.window_handles
         """
-        warnings.warn("window_handles aren't ordered by tab position")
         tabs = []
         for target in await self.targets:
             if target.type_ == "page":
                 tabs.append(target.target_id)
         return tabs
 
     async def set_window_state(self, state):
         states = ["normal", "minimized", "maximized", "fullscreen"]
         if state not in states:
             raise ValueError(f"expected one of {states}, but got: {state}")
-        window_id = self.current_window_id
+        window_id = await self.current_window_id
         bounds = {"windowState": state}
         await self.execute_cdp_cmd("Browser.setWindowBounds", {"bounds": bounds, "windowId": window_id})
 
     async def normalize_window(self):
         await self.set_window_state("normal")
 
     async def maximize_window(self) -> None:
```

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless.egg-info/PKG-INFO` & `selenium_driverless-1.1.2/src/selenium_driverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-driverless
-Version: 1.1.1
+Version: 1.1.2
 Summary: Undetected selenium without chromedriver usage
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Driverless
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Driverless/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Driverless
```

### Comparing `selenium_driverless-1.1.1/src/selenium_driverless.egg-info/SOURCES.txt` & `selenium_driverless-1.1.2/src/selenium_driverless.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,12 @@
 src/selenium_driverless.egg-info/SOURCES.txt
 src/selenium_driverless.egg-info/dependency_links.txt
 src/selenium_driverless.egg-info/requires.txt
 src/selenium_driverless.egg-info/top_level.txt
 src/selenium_driverless/files/__init__.py
 src/selenium_driverless/scripts/__init__.py
 src/selenium_driverless/scripts/alert.py
-src/selenium_driverless/scripts/cdp_listener.py
-src/selenium_driverless/scripts/mobile.py
 src/selenium_driverless/scripts/options.py
 src/selenium_driverless/scripts/switch_to.py
 src/selenium_driverless/utils/__init__.py
 src/selenium_driverless/utils/utils.py
 tests/test_driverless.py
```

### Comparing `selenium_driverless-1.1.1/tests/test_driverless.py` & `selenium_driverless-1.1.2/tests/test_driverless.py`

 * *Files identical despite different names*

