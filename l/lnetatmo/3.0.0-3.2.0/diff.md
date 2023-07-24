# Comparing `tmp/lnetatmo-3.0.0.tar.gz` & `tmp/lnetatmo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnetatmo-3.0.0.tar", last modified: Wed Jul 12 16:56:44 2023, max compression
+gzip compressed data, was "lnetatmo-3.2.0.tar", last modified: Mon Jul 24 09:59:47 2023, max compression
```

## Comparing `lnetatmo-3.0.0.tar` & `lnetatmo-3.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:56:44.695891 lnetatmo-3.0.0/
--rw-r--r--   0 root         (0) root         (0)    35147 2020-03-16 08:41:16.000000 lnetatmo-3.0.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-12 16:56:44.695891 lnetatmo-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-12 16:34:00.000000 lnetatmo-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:56:44.695891 lnetatmo-3.0.0/lnetatmo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      585 2023-07-12 16:56:44.000000 lnetatmo-3.0.0/lnetatmo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-12 16:56:44.000000 lnetatmo-3.0.0/lnetatmo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 16:56:44.000000 lnetatmo-3.0.0/lnetatmo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-12 16:56:44.000000 lnetatmo-3.0.0/lnetatmo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    33167 2023-07-12 16:15:07.000000 lnetatmo-3.0.0/lnetatmo.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-12 16:56:44.695891 lnetatmo-3.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      760 2023-07-12 16:23:53.000000 lnetatmo-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:59:47.339207 lnetatmo-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2020-03-16 08:41:16.000000 lnetatmo-3.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-24 09:59:47.339207 lnetatmo-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-07-24 09:29:43.000000 lnetatmo-3.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 09:59:47.339207 lnetatmo-3.2.0/lnetatmo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-24 09:59:47.000000 lnetatmo-3.2.0/lnetatmo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-24 09:59:47.000000 lnetatmo-3.2.0/lnetatmo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 09:59:47.000000 lnetatmo-3.2.0/lnetatmo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-24 09:59:47.000000 lnetatmo-3.2.0/lnetatmo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    34716 2023-07-24 09:29:23.000000 lnetatmo-3.2.0/lnetatmo.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 09:59:47.339207 lnetatmo-3.2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      760 2023-07-24 09:29:37.000000 lnetatmo-3.2.0/setup.py
```

### Comparing `lnetatmo-3.0.0/LICENSE.txt` & `lnetatmo-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lnetatmo-3.0.0/PKG-INFO` & `lnetatmo-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lnetatmo
-Version: 3.0.0
+Version: 3.2.0
 Summary: Simple API to access Netatmo weather station data from any python script.
 Home-page: https://github.com/philippelt/netatmo-api-python
-Download-URL: https://github.com/philippelt/netatmo-api-python/archive/v3.0.0.tar.gz
+Download-URL: https://github.com/philippelt/netatmo-api-python/archive/v3.2.0.tar.gz
 Author: Philippe Larduinat
 Author-email: ph.larduinat@wanadoo.fr
 License: GPL V3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnetatmo-3.0.0/README.md` & `lnetatmo-3.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 Following the implementation of "Home" everywhere in the Netatmo API with various behavior, the library has been adjusted to include the home parameters in most calls.
 If you are using a single account with a single home and single weather station, the library has been implemented so that your code should continue to run without change.
 
 If you have multiple homes or were supplying a station name in some method calls, you will have to adapt your code :
  - to supply a home name when looking for data for most class initializers
  - to use the new station name set by Netatmo (which is not your previously set value)
-   
   
 >BREAKING CHANGE: Netatmo seems no longer (july 2023) to allow grant_type "password", even for an app credentials that belong to the same account than the home. They have added the capability of creating access_token/refresh_token couple from the dev page (the location where app are created). As a consequence, the username/password credentials can no longer be used and you must replace them with a new parameter REFRESH_TOKEN that you will get from the web interface. To get this token, you are required to specify the scope you want to allow to this token. Select all that apply for your library use.
 
 >SHORT VERSION TO UPGRADE: If you where using a netatmo_credentials file, juste remove USERNAME and PASSWORD fields and add a REFRESH_TOKEN field which value is the one you will obtain from the https://dev.netatmo.com in MyApps selecting you app and using "Token Generator" after selecting required scopes.
 
 ### Install ###
```

### Comparing `lnetatmo-3.0.0/lnetatmo.egg-info/PKG-INFO` & `lnetatmo-3.2.0/lnetatmo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lnetatmo
-Version: 3.0.0
+Version: 3.2.0
 Summary: Simple API to access Netatmo weather station data from any python script.
 Home-page: https://github.com/philippelt/netatmo-api-python
-Download-URL: https://github.com/philippelt/netatmo-api-python/archive/v3.0.0.tar.gz
+Download-URL: https://github.com/philippelt/netatmo-api-python/archive/v3.2.0.tar.gz
 Author: Philippe Larduinat
 Author-email: ph.larduinat@wanadoo.fr
 License: GPL V3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnetatmo-3.0.0/lnetatmo.py` & `lnetatmo-3.2.0/lnetatmo.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,22 +152,25 @@
     pass
 
 
 class AuthFailure( Exception ):
     pass
 
 
+class outOfScope( Exception ):
+    pass
+
 class ClientAuth:
     """
     Request authentication and keep access token available through token method. Renew it automatically if necessary
 
     Args:
         clientId (str): Application clientId delivered by Netatmo on dev.netatmo.com
         clientSecret (str): Application Secret key delivered by Netatmo on dev.netatmo.com
-        refresh_token (str) : Scoped refresh token
+        refreshToken (str) : Scoped refresh token
     """
 
     def __init__(self, clientId=_CLIENT_ID,
                        clientSecret=_CLIENT_SECRET,
                        refreshToken=_REFRESH_TOKEN):
         
         self._clientId = clientId
@@ -184,15 +187,15 @@
     def renew_token(self):
         postParams = {
                 "grant_type" : "refresh_token",
                 "refresh_token" : self.refreshToken,
                 "client_id" : self._clientId,
                 "client_secret" : self._clientSecret
                 }
-        resp = postRequest(_AUTH_REQ, postParams)
+        resp = postRequest("authentication", _AUTH_REQ, postParams)
         if self.refreshToken != resp['refresh_token']:
             print("New refresh token:", resp['refresh_token'])
         self._accessToken = resp['access_token']
         self.refreshToken = resp['refresh_token']
         self.expiration = int(resp['expire_in'] + time.time())
 
 
@@ -205,15 +208,15 @@
     """
     warnings.warn("The 'User' class is no longer maintained by Netatmo",
             DeprecationWarning )
     def __init__(self, authData):
         postParams = {
                 "access_token" : authData.accessToken
                 }
-        resp = postRequest(_GETSTATIONDATA_REQ, postParams)
+        resp = postRequest("Weather station", _GETSTATIONDATA_REQ, postParams)
         self.rawData = resp['body']
         self.devList = self.rawData['devices']
         self.ownerMail = self.rawData['user']['mail']
 
 
 class UserInfo:
     """
@@ -239,15 +242,15 @@
                       "Please report found issues (https://github.com/philippelt/netatmo-api-python/issues)",
                        RuntimeWarning )
 
         self.getAuthToken = authData.accessToken
         postParams = {
                 "access_token" : self.getAuthToken
                 }
-        resp = postRequest(_GETTHERMOSTATDATA_REQ, postParams)
+        resp = postRequest("Thermostat", _GETTHERMOSTATDATA_REQ, postParams)
         self.rawData = resp['body']['devices']
         if not self.rawData : raise NoDevice("No thermostat available")
         self.thermostatData = filter_home_data(self.rawData, home)
         if not self.thermostatData : raise NoHome("No home %s found" % home)
         self.thermostatData['name'] = self.thermostatData['home_name']
         for m in self.thermostatData['modules']:
             m['name'] = m['module_name']
@@ -279,26 +282,36 @@
         authData (ClientAuth): Authentication information with a working access Token
     """
     def __init__(self, authData, home=None, station=None):
         self.getAuthToken = authData.accessToken
         postParams = {
                 "access_token" : self.getAuthToken
                 }
-        resp = postRequest(_GETSTATIONDATA_REQ, postParams)
+        resp = postRequest("Weather station", _GETSTATIONDATA_REQ, postParams)
         self.rawData = resp['body']['devices']
         # Weather data
         if not self.rawData : raise NoDevice("No weather station in any homes")
         # Stations are no longer in the Netatmo API, keeping them for compatibility
         self.stations = { d['station_name'] : d for d in self.rawData }
+        self.stationIds = { d['_id'] : d for d in self.rawData }
         self.homes = { d['home_name'] : d["station_name"] for d in self.rawData }
         # Keeping the old behavior for default station name
         if home and home not in self.homes : raise NoHome("No home with name %s" % home)
         self.default_home = home or list(self.homes.keys())[0]
-        if station and station not in self.stations: raise NoDevice("No station with name %s" % station)
-        self.default_station = station or [v["station_name"] for k,v in self.stations.items() if v["home_name"] == self.default_home][0]
+        if station:
+            if station not in self.stations:
+                # May be a station_id convert it to corresponding station name
+                s = self.stationById(station)
+                if s :
+                    station = s["station_name"]
+                else:
+                    raise NoDevice("No station with name or id %s" % station)
+            self.default_station = station
+        else:
+            self.default_station =  [v["station_name"] for k,v in self.stations.items() if v["home_name"] == self.default_home][0]
         self.modules = dict()
         self.default_station_data = self.stationByName(self.default_station)
         if 'modules' in self.default_station_data:
             for m in self.default_station_data['modules']:
                 self.modules[ m['_id'] ] = m
         # User data
         userData = resp['body']['user']
@@ -309,39 +322,40 @@
                 setattr(self.user, k, UNITS[k][v])
             else:
                 setattr(self.user, k, v)
 
 
     def modulesNamesList(self, station=None, home=None):
         res = [m['module_name'] for m in self.modules.values()]
+        station = self.stationByName(station) or self.stationById(station)
         res.append(self.stationByName(station)['module_name'])
         return res
 
     def stationByName(self, station=None):
         if not station : station = self.default_station
-        for i,s in self.stations.items():
-            if s['station_name'] == station :
-                return self.stations[i]
-        return None
+        if station not in self.stations : return None
+        return self.stations[station]
 
     def stationById(self, sid):
-        return self.stations.get(sid)
+        if not sid : return self.stations[self.default_station]
+        if sid not in self.stationIds : return None
+        return self.stationIds[sid]
 
     def moduleByName(self, module):
         for m in self.modules:
             mod = self.modules[m]
             if mod['module_name'] == module :
                 return mod
         return None
 
     def moduleById(self, mid):
         return self.modules.get(mid)
 
-    def lastData(self, exclude=0):
-        s = self.default_station_data
+    def lastData(self, station=None, exclude=0):
+        s = self.stationByName(station) or self.stationById(station)
         # Breaking change from Netatmo : dashboard_data no longer available if station lost
         if not s or 'dashboard_data' not in s : return None
         lastD = dict()
         # Define oldest acceptable sensor measure event
         limit = (time.time() - exclude) if exclude else 0
         ds = s['dashboard_data']
         if ds.get('time_utc',limit+10) > limit :
@@ -384,15 +398,15 @@
         postParams['scale']      = scale
         postParams['type']       = mtype
         if date_begin : postParams['date_begin'] = date_begin
         if date_end : postParams['date_end'] = date_end
         if limit : postParams['limit'] = limit
         postParams['optimize'] = "true" if optimize else "false"
         postParams['real_time'] = "true" if real_time else "false"
-        return postRequest(_GETMEASURE_REQ, postParams)
+        return postRequest("Weather station", _GETMEASURE_REQ, postParams)
 
     def MinMaxTH(self, module=None, frame="last24"):
         s = self.default_station_data
         if frame == "last24":
             end = time.time()
             start = end - 24*3600 # 24 hours ago
         elif frame == "day":
@@ -438,15 +452,15 @@
         authData (ClientAuth): Authentication information with a working access Token
     """
     def __init__(self, authData, home=None):
         self.getAuthToken = authData.accessToken
         postParams = {
             "access_token" : self.getAuthToken
             }
-        resp = postRequest(_GETHOMEDATA_REQ, postParams)
+        resp = postRequest("Home data", _GETHOMEDATA_REQ, postParams)
         self.rawData = resp['body']
         # Collect homes
         self.homes = { d['id'] : d for d in self.rawData['homes'] }
         if not self.homes : raise NoDevice("No home available")
         self.default_home = home or list(self.homes.values())[0]['name']
         # Split homes data by category
         self.persons = dict()
@@ -519,18 +533,18 @@
         vpn_url = None
         if cid:
             camera_data=self.cameraById(cid)
         else:
             camera_data=self.cameraByName(camera=camera, home=home)
         if camera_data:
             vpn_url = camera_data['vpn_url']
-            resp = postRequest(vpn_url + '/command/ping')
+            resp = postRequest("Camera", vpn_url + '/command/ping')
             temp_local_url=resp['local_url']
             try:
-                resp = postRequest(temp_local_url + '/command/ping',timeout=1)
+                resp = postRequest("Camera", temp_local_url + '/command/ping',timeout=1)
                 if resp and temp_local_url == resp['local_url']:
                     local_url = temp_local_url
             except:  # On this particular request, vithout errors from previous requests, error is timeout
                 local_url = None
         return vpn_url, local_url
 
     def url(self, camera=None, home=None, cid=None):
@@ -557,15 +571,15 @@
         Download a specific image (of an event or user face) from the camera
         """
         postParams = {
             "access_token" : self.getAuthToken,
             "image_id" : image_id,
             "key" : key
             }
-        resp = postRequest(_GETCAMERAPICTURE_REQ, postParams)
+        resp = postRequest("Camera", _GETCAMERAPICTURE_REQ, postParams)
         image_type = imghdr.what('NONE.FILE',resp)
         return resp, image_type
 
     def getProfileImage(self, name):
         """
         Retrieve the face of a given person
         """
@@ -591,15 +605,15 @@
 
         home_data = self.homeByName(home)
         postParams = {
             "access_token" : self.getAuthToken,
             "home_id" : home_data['id'],
             "event_id" : event['id']
         }
-        resp = postRequest(_GETEVENTSUNTIL_REQ, postParams)
+        resp = postRequest("Camera", _GETEVENTSUNTIL_REQ, postParams)
         eventList = resp['body']['events_list']
         for e in eventList:
             self.events[ e['camera_id'] ][ e['time'] ] = e
         for camera in self.events:
             self.lastEvent[camera]=self.events[camera][sorted(self.events[camera])[-1]]
 
     def personSeenByCamera(self, name, home=None, camera=None):
@@ -696,15 +710,15 @@
         if eventType not in _PRES_DETECTION_KIND or \
            action not in _PRES_DETECTION_SETUP : return None
         camera = self.cameraByName(home=home, camera=camera) or self.cameraById(cid=cid)
         postParams = { "access_token" : self.getAuthToken,
                        "home_id" : camera["home_id"],
                        "presence_settings[presence_record_%s]" % eventType : _PRES_DETECTION_SETUP.index(action)
                      }
-        resp = postRequest(_POST_UPDATE_HOME_REQ, postParams)
+        resp = postRequest("Camera", _POST_UPDATE_HOME_REQ, postParams)
         self.rawData = resp['body']
 
     def getLiveSnapshot(self, camera=None, home=None, cid=None):
         camera = self.cameraByName(home=home, camera=camera) or self.cameraById(cid=cid)
         vpnUrl, localUrl = self.cameraUrls(cid=camera["id"])
         url = localUrl or vpnUrl
         return cameraCommand(url, _PRES_CDE_GET_SNAP)
@@ -714,52 +728,66 @@
     """
     This class is now deprecated. Use HomeData instead
     Home can handle many devices, not only Welcome cameras
     """
     warnings.warn("The 'WelcomeData' class was renamed 'HomeData' to handle new Netatmo Home capabilities",
             DeprecationWarning )
     pass
-
 # Utilities routines
 
+def rawAPI(authData, url, parameters={}):
+    fullUrl = _BASE_URL + "api/" + url
+    parameters["access_token"] = authData.accessToken
+    resp = postRequest("rawAPI", fullUrl, parameters)
+    return resp["body"] if "body" in resp else None
 
 def filter_home_data(rawData, home):
     if home:
         # Find a home who's home id or name is the one requested
         for h in rawData:
             if h["home_name"] == home or h["home_id"] == home:
                 return h
         return None
     # By default, the first home is returned
     return rawData[0]
 
 def cameraCommand(cameraUrl, commande, parameters=None, timeout=3):
     url = cameraUrl + ( commande % parameters if parameters else commande)
-    return postRequest(url, timeout=timeout)
+    return postRequest("Camera", url, timeout=timeout)
     
-def postRequest(url, params=None, timeout=10):
+def postRequest(topic, url, params=None, timeout=10):
     if PYTHON3:
         req = urllib.request.Request(url)
         if params:
             req.add_header("Content-Type","application/x-www-form-urlencoded;charset=utf-8")
+            if "access_token" in params:
+                req.add_header("Authorization","Bearer %s" % params.pop("access_token"))
             params = urllib.parse.urlencode(params).encode('utf-8')
         try:
             resp = urllib.request.urlopen(req, params, timeout=timeout) if params else urllib.request.urlopen(req, timeout=timeout)
         except urllib.error.HTTPError as err:
-            logger.error("code=%s, reason=%s, body=%s" % (err.code, err.reason, err.fp.read()))
+            if err.code == 403:
+                logger.warning("Your current token scope do not allow access to %s" % topic)
+            else:
+                logger.error("code=%s, reason=%s, body=%s" % (err.code, err.reason, err.fp.read()))
             return None
     else:
         if params:
             params = urlencode(params)
-            headers = {"Content-Type" : "application/x-www-form-urlencoded;charset=utf-8"}
+            headers = {"Content-Type"  : "application/x-www-form-urlencoded;charset=utf-8"}
+            if "access_token" in params:
+                headers["Authorization"] = "Bearer %s" % params.pop("access_token")
         req = urllib2.Request(url=url, data=params, headers=headers) if params else urllib2.Request(url)
         try:
             resp = urllib2.urlopen(req, timeout=timeout)
         except urllib2.HTTPError as err:
-            logger.error("code=%s, reason=%s" % (err.code, err.reason))
+            if err.code == 403:
+                logger.warning("Your current token scope do not allow access to %s" % topic)
+            else:
+                logger.error("code=%s, reason=%s" % (err.code, err.reason))
             return None
     data = b""
     for buff in iter(lambda: resp.read(65535), b''): data += buff
     # Return values in bytes if not json data to handle properly camera images
     returnedContentType = resp.getheader("Content-Type") if PYTHON3 else resp.info()["Content-Type"]
     return json.loads(data.decode("utf-8")) if "application/json" in returnedContentType else data
```

### Comparing `lnetatmo-3.0.0/setup.py` & `lnetatmo-3.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # python setup.py --dry-run --verbose install
 
 from distutils.core import setup
 
 setup(
     name='lnetatmo',
-    version='3.0.0',
+    version='3.2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3'
         ],
     author='Philippe Larduinat',
     author_email='ph.larduinat@wanadoo.fr',
     py_modules=['lnetatmo'],
     scripts=[],
     data_files=[],
     url='https://github.com/philippelt/netatmo-api-python',
-    download_url='https://github.com/philippelt/netatmo-api-python/archive/v3.0.0.tar.gz',
+    download_url='https://github.com/philippelt/netatmo-api-python/archive/v3.2.0.tar.gz',
     license='GPL V3',
     description='Simple API to access Netatmo weather station data from any python script.'
 )
```

