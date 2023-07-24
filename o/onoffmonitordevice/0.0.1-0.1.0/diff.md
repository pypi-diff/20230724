# Comparing `tmp/onoffmonitordevice-0.0.1-py3-none-any.whl.zip` & `tmp/onoffmonitordevice-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5667 bytes, number of entries: 11
+Zip file size: 6386 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 16:55 onoffmonitordevice/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 23-Jul-06 16:55 onoffmonitordevice/__main__.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Jul-07 10:59 onoffmonitordevice/device.py
+-rw-r--r--  2.0 unx     1523 b- defN 23-Jul-24 15:42 onoffmonitordevice/__main__.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-22 16:31 onoffmonitordevice/device.py
 -rw-r--r--  2.0 unx       43 b- defN 23-Jul-06 16:55 onoffmonitordevice/exceptions.py
--rw-r--r--  2.0 unx     3244 b- defN 23-Jul-07 10:52 onoffmonitordevice/monitor.py
--rw-r--r--  2.0 unx     1687 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      914 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      974 b- defN 23-Jul-07 11:24 onoffmonitordevice-0.0.1.dist-info/RECORD
-11 files, 8804 bytes uncompressed, 3981 bytes compressed:  54.8%
+-rw-r--r--  2.0 unx     4280 b- defN 23-Jul-24 15:37 onoffmonitordevice/monitor.py
+-rw-r--r--  2.0 unx     1687 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-24 15:51 onoffmonitordevice-0.1.0.dist-info/RECORD
+11 files, 11165 bytes uncompressed, 4700 bytes compressed:  57.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: onoffmonitordevice/exceptions.py
 Comment: 
 
 Filename: onoffmonitordevice/monitor.py
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/LICENSE
+Filename: onoffmonitordevice-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/METADATA
+Filename: onoffmonitordevice-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/WHEEL
+Filename: onoffmonitordevice-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/entry_points.txt
+Filename: onoffmonitordevice-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/top_level.txt
+Filename: onoffmonitordevice-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onoffmonitordevice-0.0.1.dist-info/RECORD
+Filename: onoffmonitordevice-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onoffmonitordevice/__main__.py

```diff
@@ -1,30 +1,57 @@
 """
 Module for entry to program
 """
 from argparse import ArgumentParser
-import sys
+import logging
 
 from .monitor import Monitor
 from .exceptions import ValidationError
 
 
+_logger = logging.getLogger(__name__)
+
+
 def main():
     """
     Main entry point: parse args and start monitor
     """
     parser = ArgumentParser(
         prog='onoffmonitor',
         description='Monitor the on/off status of devices and report to the server'
     )
     parser.add_argument('path', help='The path to the configuration JSON file')
+    parser.add_argument(
+        '-ll', '-loglevel',
+        help='Logging level {debug, info, warning (default), error, critical}',
+        type=int,
+        choices=[logging.DEBUG, logging.INFO, logging.WARNING, logging.ERROR, logging.CRITICAL],
+        default=logging.WARNING,
+    )
+    parser.add_argument(
+        '-lf', '-logfile',
+        help='Log output file path (defaults to stdout)',
+        type=str,
+        default=None,
+    )
     args = parser.parse_args()
+    logging.basicConfig(
+        format='%(levelname)s: %(asctime)s: %(name)s: %(funcName)s: %(message)s',
+        level=args.ll,
+        filename=args.lf,
+    )
+    monitor = None
     try:
-        Monitor(args.path).run()
+        monitor = Monitor(args.path)
+        monitor.run()
     except ValidationError as exc:
-        print('\n'.join(exc.args), file=sys.stderr)
+        _logger.critical('Validation error: %s', '\n'.join(exc.args))
     except KeyboardInterrupt:
         pass
+    finally:
+        if monitor is not None:
+            monitor.stop()
+        _logger.debug('Finished')
 
 
 if __name__ == '__main__':
     main()
```

## onoffmonitordevice/device.py

```diff
@@ -1,33 +1,41 @@
 # pylint:disable=no-member
+import logging
 from typing import Callable
 
 import RPi.GPIO as gpio
 
 from .exceptions import ValidationError
 
 
 class Device:
+    _logger = logging.getLogger(__name__)
+
     def __init__(self, setup: dict):
-        if isinstance(setup, dict) and isinstance(setup.get('id'), int) and isinstance(setup.get('pin'), int):
+        self._logger.debug('Initialising (%s)', str(setup))
+        if isinstance(setup, dict) and isinstance(setup.get('id'), int) and isinstance(setup.get('gpio_pin'), int):
             self._device_id: int = setup['id']
-            self._pin: int = setup['pin']
+            self._pin: int = setup['gpio_pin']
             self._state = 0
             self._event = None
         else:
             raise ValidationError(f'Invalid device: {setup}')
 
     def _on_state_change(self, pin):
-        print('on state change', pin)
+        self._logger.debug('Pin %i state change', pin)
         self._state = 1 - self._state
         print(self._state, gpio.input(pin))
         if self._event is not None:
             self._event({'device': self._device_id, 'status': self._state})
 
     def begin(self, event: Callable):
+        self._logger.debug('Pin %i: begin', self._pin)
         self._event = event
-        gpio.setup(self._pin, gpio.IN) # type: ignore
-        gpio.add_event_detect( # type: ignore
+        gpio.setup(self._pin, gpio.IN)  # type: ignore
+        gpio.add_event_detect(  # type: ignore
             self._pin,
-            gpio.BOTH, # type: ignore
+            gpio.BOTH,  # type: ignore
             callback=self._on_state_change
         )
+
+    def __repr__(self):
+        return f'Device({{"id": {self._device_id}, "gpio_pin": {self._pin}}})'
```

## onoffmonitordevice/monitor.py

```diff
@@ -1,13 +1,13 @@
 """
 Module containing the main monitor program
 """
 import getpass
 import json
-import sys
+import logging
 from time import sleep
 from pathlib import Path
 
 import keyring
 import requests
 import RPi.GPIO as gpio
 
@@ -16,81 +16,101 @@
 
 
 class Monitor:
     """
     Starts a new monitor program
     """
     keyring_service = 'onoffmonitor'
+    _logger = logging.getLogger(__name__)
 
     def __init__(self, settings_path: str):
+        self._logger.debug('Initialising (%s)', settings_path)
         path = self._get_path(settings_path)
+        self._request_headers = {}
+        self._devices: list[Device] = []
         self._process_settings(json.loads(path.read_text()))
-        self._token = None
 
     def run(self):
+        self._logger.debug('Running')
         self._login()
+        self._fetch_devices()
         self._monitor()
 
     @staticmethod
     def _get_path(settings_path: str):
         path = Path(settings_path)
         if not path.exists():
             raise ValidationError(f'The file {settings_path} doesn\'t exist')
         if not path.is_file():
             raise ValidationError(f'{settings_path} is not a file')
         return path
 
     def _process_settings(self, settings: dict):
+        self._logger.debug('Processing settings')
         errors = []
-        devices: list[Device] = []
         if not isinstance(settings.get('host'), str):
             errors.append('"host" property missing or not a string')
         if not isinstance(settings.get('username'), str):
             errors.append('"username" property missing or not a string')
-        if isinstance(settings.get('devices'), list):
-            for device in settings['devices']:
-                devices.append(Device(device))
-        else:
-            errors.append('"devices" property missing or not a list')
+        if not isinstance(settings.get('id'), int):
+            errors.append('"id" property missing or not an integer')
         if len(errors) != 0:
             raise ValidationError(*errors)
         self._host = settings['host']
         self._username = settings['username']
-        self._devices = devices
+        self._monitor_id = settings['id']
         self._monitor_path = settings.get('monitorapi', '/api/onoffmonitor/')
         self._login_path = settings.get('loginapi', '/api/')
 
     def _login(self):
+        self._logger.debug('Logging in')
         password = keyring.get_password(self.keyring_service, self._username)
         while True:
             if password is None:
                 password = getpass.getpass(
                     f'Enter password for {self._username}: ')
             request = requests.post(
                 self._host + self._login_path + 'login/', auth=(self._username, password), timeout=10)
             response = request.json()
             if 'token' in response:
-                self._token = response['token']
+                self._request_headers['Authorization'] = f'Token {response["token"]}'
                 keyring.set_password(self.keyring_service,
                                      self._username, password)
-                print('Logged in')
+                self._logger.info('Logged in as %s', self._username)
                 break
             password = None
             if 'detail' in response:
-                print(response['detail'], file=sys.stderr)
+                self._logger.error(response['detail'])
             else:
-                print('Response from server:', response, file=sys.stderr)
+                self._logger.error('Response from server: %s', response)
+
+    def _fetch_devices(self):
+        self._logger.debug('Fetching device configuration')
+        request = requests.get('%s%smonitor/%i/conf/' % (self._host, self._monitor_path, self._monitor_id), headers=self._request_headers)
+        response = request.json()
+        for device in response:
+            self._devices.append(Device(device))
+        self._logger.debug('Devices: %s', str(self._devices))
 
     def _monitor(self):
         gpio.setmode(gpio.BOARD)
         for device in self._devices:
             device.begin(self.on_device_state_change)
         print('Sleeping')
         sleep(20)
 
     def on_device_state_change(self, data):
-        print('Sending', data)
-        request = requests.post(self._host + self._monitor_path + 'status/', json=data, headers={'Authorization': 'Token ' + self._token})
-        print(request.text)
-
-    def __del__(self):
-        print('del')
+        self._logger.debug('Sending %s', str(data))
+        request = requests.post(self._host + self._monitor_path + 'status/', json=data, headers=self._request_headers)
+        self._logger.debug(request.text)
+
+    def stop(self):
+        self._logger.debug('Stopping')
+        self._logout()
+
+    def _logout(self):
+        if 'Authorization' not in self._request_headers:
+            self._logger.debug('Already logged out')
+            return
+        self._logger.debug('Logging out')
+        requests.post(self._host + self._login_path + 'logout/', headers=self._request_headers)
+        self._request_headers.clear()
```

## Comparing `onoffmonitordevice-0.0.1.dist-info/LICENSE` & `onoffmonitordevice-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `onoffmonitordevice-0.0.1.dist-info/METADATA` & `onoffmonitordevice-0.1.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: onoffmonitordevice
-Version: 0.0.1
+Version: 0.1.0
 Summary: Monitor the on/off status of devices and report to the server
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/onoffmonitordevice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: <4,>=3.9
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.31.0)
 Requires-Dist: keyring (>=24.2.0)
 Requires-Dist: RPi.GPIO (>=0.7.1)
 Requires-Dist: keyrings.alt (>=4.2.0)
 
 # On/Off Monitor Device
 ## Installation
 ### Cryptography
 On Linux you might need to install Rust to compile the Cryptography library. See their [installation instructions](https://cryptography.io/en/latest/installation/)  
 For installing Rust on Raspberry Pi see https://forums.raspberrypi.com/viewtopic.php?t=289963
+## For when testing on a non-Raspberry Pi
+Instead of installing the `RPi.GPIO` module, you can install `rpi-gpio-emu`.
+Installing with pipenv won't work as `RPi.GPIO` only works with Raspberry Pi.
```

