# Comparing `tmp/eagleeyev3-0.0.4.tar.gz` & `tmp/eagleeyev3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagleeyev3-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eagleeyev3-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eagleeyev3-0.0.4.tar` & `eagleeyev3-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      156 2023-07-20 15:32:00.324422 eagleeyev3-0.0.4/.gitignore
--rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.4/LICENSE
--rw-r--r--   0        0        0      375 2023-07-20 04:33:54.569165 eagleeyev3-0.0.4/README.md
--rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    21471 2023-07-20 15:36:26.588054 eagleeyev3-0.0.4/src/EagleEyev3/__init__.py
--rw-r--r--   0        0        0      533 2023-07-11 02:17:41.899184 eagleeyev3-0.0.4/src/EagleEyev3/settings.py
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 eagleeyev3-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-07-20 15:43:05.663721 eagleeyev3-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.5/LICENSE
+-rw-r--r--   0        0        0      375 2023-07-20 04:33:54.569165 eagleeyev3-0.0.5/README.md
+-rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    27534 2023-07-24 16:22:55.160633 eagleeyev3-0.0.5/src/EagleEyev3/__init__.py
+-rw-r--r--   0        0        0      533 2023-07-11 02:17:41.899184 eagleeyev3-0.0.5/src/EagleEyev3/settings.py
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 eagleeyev3-0.0.5/PKG-INFO
```

### Comparing `eagleeyev3-0.0.4/LICENSE` & `eagleeyev3-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.4/src/EagleEyev3/__init__.py` & `eagleeyev3-0.0.5/src/EagleEyev3/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Python client for Eagle Eye Networks APIv3 """
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 import json
 import logging
 import requests
 from .settings import *
 
@@ -17,15 +17,15 @@
 
 
 class EagleEyev3():
     """
     Class representing the EagleEyev3 client.
     """
 
-    __version__ = "0.0.4"
+    __version__ = "0.0.5"
     __all__ = ['EagleEyev3', 'Device', 'Camera']
 
     def __init__(self, config=None):
         """
         Initializes the EagleEyev3 client object.
         """
         self.client_id = None
@@ -57,14 +57,26 @@
 
         if self.lazy_login:
             try:
                 self._load_access_token()
             except FileNotFoundError as e:
                 logging.warn("self.lazy_login is set to {self.lazy_login} but could not find .lazy_login file to load")
 
+        # for use with request calls, can be an int, tuple, or None
+        # preferred would be a tuple with the first value is time to connect, second is time to first byte
+        # https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
+        # called by self._get_timeout_values
+        self.timeout_values = {
+            'default': (3,5),
+            'login': (5, 30),
+            'logout': (5, 15),
+            'list_of_events': (6, 20),
+            'live_preview': (3, 5)
+        }
+
     def _load_vars_from_settings(self, config={}):
         """
         Load variables from the settings module.
         """
         self.client_id = config['client_id']
         self.client_secret = config['client_secret']
         self.server_protocol = config['server_protocol']
@@ -73,15 +85,14 @@
         self.server_path = config['server_path']
 
         # Combine server_protocol, server_host, and server_port to make the redirect_uri
         # Note: Please see the note in settings.py about trailing slashes and modify this line if needed
         
         self.redirect_uri = f"{self.server_protocol}://{self.server_host}:{self.server_port}/{self.server_path}"
 
-
     def _save_access_token(self):
         with open(".lazy_login", "w") as json_file:
             json.dump({
                 'access_token': self.access_token,
                 'refresh_token': self.refresh_token,
                 'current_user': self.current_user
             }, json_file)
@@ -92,30 +103,26 @@
             if 'access_token' in saved:
                 self.access_token = saved['access_token']
             if 'refresh_token' in saved:
                 self.refresh_token = saved['refresh_token']
 
         self.get_base_url(cascade=True)
 
-
     def time_now(self):
         return datetime.now(tz=self.user_tz_obj).isoformat(timespec='milliseconds')
 
-
     def time_before(self, ts=None, hours=6):
         if ts == None:
             ts = datetime.now(tz=self.user_tz_obj)
 
         if type(ts) == str:
             ts = datetime.fromisoformat(ts)
 
         return (ts - timedelta(hours=hours)).isoformat(timespec='milliseconds')
 
-
-
     def login_tokens(self, code=None, cascade=True):
         """
         Obtains login tokens using the authorization code.
 
         Args:
             code (str): The authorization code.
             cascade (bool): Indicates whether to cascade and get the base URL and current user information.
@@ -124,15 +131,15 @@
             dict: Dictionary containing the success status, response HTTP status code, data, and current user information.
         """
         baseUrl = "https://auth.eagleeyenetworks.com/oauth2/token"
         pathUrl = f"?grant_type=authorization_code&scope=vms.all&code={code}&redirect_uri={self.redirect_uri}" # Note the trailing slash, make sure it matches the whitelist
         url = baseUrl + pathUrl
 
         # Send a POST request to obtain login tokens
-        response = requests.post(url, auth=(self.client_id, self.client_secret))
+        response = requests.post(url, auth=(self.client_id, self.client_secret), timeout=self._get_timeout_values('login'))
         response_json = response.json()
 
         logging.info(f"{response.status_code} in login_tokens")
 
         if response.status_code == 200:
             success = True
             self.access_token = response_json['access_token']
@@ -170,15 +177,15 @@
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json",
                     "Content-type": "application/json"
                 }
 
         # Send a POST request to obtain the base URL
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.post(url, json=payload, headers=headers, timeout=self._get_timeout_values('logout'))
         response_json = response.json()
 
         logging.info(f"{response.status_code} in logout")
 
         if response.status_code == 200:
             success = True
         else:
@@ -206,19 +213,36 @@
         """
         url = "https://api.eagleeyenetworks.com/api/v3.0/clientSettings"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        # Send a GET request to obtain the base URL
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            # Send a GET request to obtain the base URL
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('base_url'))
+            response_json = response.json()
+
+            logging.info(f"{response.status_code} in get_base_url")
 
-        logging.info(f"{response.status_code} in get_base_url")
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_base_url()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             if 'httpsBaseUrl' in response_json and 'hostname' in response_json['httpsBaseUrl']:
                 self.user_base_url = response_json['httpsBaseUrl']['hostname']
                 if cascade:
                     self.get_current_user()
@@ -240,19 +264,36 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/users/self?include=timeZone"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        # Send a GET request to obtain the current user information
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            # Send a GET request to obtain the current user information
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('curent_user'))
+            response_json = response.json()
+
+            logging.info(f"{response.status_code} in get_current_user")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_current_user()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
-        logging.info(f"{response.status_code} in get_current_user")
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             self.current_user = response_json
             self.user_tz_obj = timezone(response_json['timeZone']['timeZone'])
         else:
             success = False
@@ -272,18 +313,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/users?include=timeZone"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_users'))
+            response_json = response.json()
+
+            logging.info(f"{response.status_code} in get_list_of_users")
 
-        logging.info(f"{response.status_code} in get_list_of_users")
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_users()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             self.users = [i for i in response_json['results']]
         else:
             success = False
 
@@ -302,18 +360,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/cameras?include=status"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_cameras'))
+            response_json = response.json()
 
-        logging.info(f"{response.status_code} in get_list_of_cameras")
+            logging.info(f"{response.status_code} in get_list_of_cameras")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_cameras()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             self.cameras = [
                     Camera(id=i['id'],\
                            name=i['name'],\
                            status=i['status'],\
@@ -342,18 +417,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/bridges"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_bridges'))
+            response_json = response.json()
 
-        logging.info(f"{response.status_code} in get_list_of_bridges")
+            logging.info(f"{response.status_code} in get_list_of_bridges")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_bridges()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             self.bridges = [i for i in response_json['results']]
         else:
             success = False
 
@@ -372,18 +464,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/switches"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_switches'))
+            response_json = response.json()
 
-        logging.info(f"{response.status_code} in get_list_of_switches")
+            logging.info(f"{response.status_code} in get_list_of_switches")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_switches()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
             self.switches = [i for i in response_json['results']]
         else:
             success = False
 
@@ -402,18 +511,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/availableDevices?deviceType__in={deviceType__in}"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_available_devices'))
+            response_json = response.json()
 
-        logging.info(f"{response.status_code} in get_list_of_available_devices")
+            logging.info(f"{response.status_code} in get_list_of_available_devices")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_available_devices()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
         else:
             success = False
 
         return {
@@ -431,18 +557,35 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/multiCameras"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_multi_cameras'))
+            response_json = response.json()
+
+            logging.info(f"{response.status_code} in get_list_of_multi_cameras")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_multi_cameras()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
-        logging.info(f"{response.status_code} in get_list_of_multi_cameras")
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
         else:
             success = False
 
         return {
@@ -460,50 +603,71 @@
         """
         url = f"https://{self.user_base_url}/api/v3.0/feeds"
         headers = { 
                     "Authorization": f"Bearer {self.access_token}", 
                     "Accept": "application/json"
                 }
 
-        response = requests.get(url, headers=headers)
-        response_json = response.json()
+        try:
+            response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_feeds'))
+            response_json = response.json()
 
-        logging.info(f"{response.status_code} in get_list_of_feeds")
+            logging.info(f"{response.status_code} in get_list_of_feeds")
+
+        except requests.exceptions.Timeout:
+            logging.warn(f"timeout expired for {self.id} get_list_of_feeds()")
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
+
+        except requests.exceptions.RequestException as e:
+            logging.warn(e)
+            return {
+                "success": False,
+                "response_http_status": 0,
+                "data": None
+            }
 
         if response.status_code == 200:
             success = True
         else:
             success = False
 
         return {
             "success": success,
             "response_http_status": response.status_code,
             "data": response_json
         }
 
-
     def get_camera_by_id(self, esn):
         found_camera = None
         for camera in self.cameras:
             if camera.id == esn:
                 found_camera = camera
                 break
 
         if found_camera == None:
             camera = Camera()
 
         logging.debug(f"returning camera {camera} for search query {esn}")
         return camera
 
+    def _get_timeout_values(self, name='default'):
+        if name in self.timeout_values:
+            return self.timeout_values[name]
+        else:
+            return self.timeout_values['default']
 
 
 
 class Device():
 
-    def __init__(self, id=None, name=None, status=None, account_id=None, user_base_url=None, een_instance=None):
+    def __init__(self, id=None, name=None, status=dict(), account_id=None, user_base_url=None, een_instance=None):
 
         self.id = id
         self.name = name
         self.status = status
         self.account_id = account_id
         self.user_base_url = user_base_url,
         self.een_instance = een_instance
@@ -537,23 +701,23 @@
             online = '？'
         return f"{online} [{self.id}] - {self.name}"
 
 
 
 class Camera(Device):
 
-    def __init__(self, id=None, name=None, status=None, account_id=None, bridge_id=None, user_base_url=None, een_instance=None):
+    def __init__(self, id=None, name=None, status=dict(), account_id=None, bridge_id=None, user_base_url=None, een_instance=None):
         super().__init__(id=id, name=name, status=status, account_id=account_id, user_base_url=user_base_url, een_instance=een_instance)
         self.bridge_id = bridge_id
         self.previews = []
         self.videos = []
         self.events = {
                 'status': [],
                 'motion': []
-                } 
+                }
     
     
     def get_list_of_events(self, start_timestamp=None, end_timestamp=None):
         """
         Obtains the list of events.
 
         Returns:
@@ -572,15 +736,15 @@
 
         headers = { 
                     "Authorization": f"Bearer {self.een_instance.access_token}", 
                     "Accept": "application/json"
                 }
 
         try:
-            response = requests.get(url, headers=headers, timeout=(3, 5))
+            response = requests.get(url, headers=headers, timeout=self.een_instance._get_timeout_values('list_of_events'))
             response_json = response.json()
 
             logging.debug(f"{response.status_code} returned from {url} with {headers} and {response.text}")
             logging.info(f"{response.status_code} in get_list_of_events")
 
             if response.status_code == 200:
                 success = True
@@ -630,20 +794,21 @@
 
         headers = { 
                     "Authorization": f"Bearer {self.een_instance.access_token}", 
                     "Accept": "image/jpeg"
                 }
 
         try:
-            response = requests.get(url, headers=headers, timeout=(3, 5))
+            response = requests.get(url, headers=headers, timeout=self.een_instance._get_timeout_values('live_preview'))
             logging.info(f"{response.status_code} in get_live_preview")
 
         except requests.exceptions.Timeout:
             logging.warn(f"timeout expired for {self.id} get_live_preview()")
             response = None
+        
         except requests.exceptions.RequestException as e:
             logging.warn(e)
             response = None
         
         return response
```

### Comparing `eagleeyev3-0.0.4/src/EagleEyev3/settings.py` & `eagleeyev3-0.0.5/src/EagleEyev3/settings.py`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.4/PKG-INFO` & `eagleeyev3-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EagleEyev3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client for Eagle Eye Networks APIv3 
 Author-email: mcotton <mcotton@mcottondesign.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://mcottondesign.com
 
 # EE-status-v3 #
```

