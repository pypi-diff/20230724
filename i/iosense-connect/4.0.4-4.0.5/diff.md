# Comparing `tmp/iosense_connect-4.0.4.tar.gz` & `tmp/iosense_connect-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-4.0.4.tar", last modified: Fri Jun 23 13:49:07 2023, max compression
+gzip compressed data, was "dist\iosense_connect-4.0.5.tar", last modified: Mon Jul 24 09:55:53 2023, max compression
```

## Comparing `iosense_connect-4.0.4.tar` & `iosense_connect-4.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.504855 iosense_connect-4.0.4/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-06-23 13:49:07.498490 iosense_connect-4.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.232468 iosense_connect-4.0.4/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.4/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    28183 2023-06-23 13:46:36.000000 iosense_connect-4.0.4/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:49:07.430477 iosense_connect-4.0.4/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      262 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-23 13:49:06.000000 iosense_connect-4.0.4/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 13:49:07.507918 iosense_connect-4.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-06-23 13:44:34.000000 iosense_connect-4.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:55:53.974011 iosense_connect-4.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-4.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-07-24 09:55:53.972597 iosense_connect-4.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-4.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 09:55:53.936955 iosense_connect-4.0.5/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-4.0.5/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    31851 2023-07-24 09:55:40.000000 iosense_connect-4.0.5/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-07-24 09:55:53.962654 iosense_connect-4.0.5/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-07-24 09:55:53.000000 iosense_connect-4.0.5/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-24 09:55:53.000000 iosense_connect-4.0.5/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 09:55:53.000000 iosense_connect-4.0.5/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      262 2023-07-24 09:55:53.000000 iosense_connect-4.0.5/iosense_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-24 09:55:53.000000 iosense_connect-4.0.5/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 09:55:53.974011 iosense_connect-4.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-07-24 09:45:28.000000 iosense_connect-4.0.5/setup.py
```

### Comparing `iosense_connect-4.0.4/LICENSE.txt` & `iosense_connect-4.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.4/PKG-INFO` & `iosense_connect-4.0.5/iosense_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iosense_connect
-Version: 4.0.4
+Name: iosense-connect
+Version: 4.0.5
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.4/README.md` & `iosense_connect-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.0.4/iosense_connect/data_access.py` & `iosense_connect-4.0.5/iosense_connect/data_access.py`

 * *Files 14% similar despite different names*

```diff
@@ -266,126 +266,199 @@
                     credentials[1] = cipher.decrypt(credentials[1].encode('utf-8')).decode()
                 else:
                     credentials = cipher.decrypt(credentials.encode('utf-8')).decode()
                 return credentials
         except Exception as e:
             print(e)
 
-    def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=datetime.now(), alias=True, IST=True,
-               onpremise=False):
+    def get_userinfo(self,onpremise=False):
         """
+        :return: Json
 
-        :param onpremise:
-        :param alias:
-        :param device_id: string
-        :param sensors: IST of sensors
-        :param n: number of data points (default: 1)
-        :param cal: bool (default: True)
-        :param end_time: 'YYYY:MM:DD HH:MM:SS'
-        :param IST: bool (default: True) Indian Standard Timezone
-        :return: Dataframe with values
-
-        Get Data Point fetches data containing values of last n data points of given sensor at given time.
-
+        Details like phone,name,gender,emailed etc are fetched
         """
         try:
-
-            metadata = {}
-            if sensors is None:
-                metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
-                data_sensor = metadata['sensors']
-                df_sensor = pd.DataFrame(data_sensor)
-                sensor_id_list = list(df_sensor['sensorId'])
-                sensors = sensor_id_list
-
-            end_time = pd.to_datetime(end_time)
-            if IST:
-                end_time = end_time - timedelta(hours=5, minutes=30)
-            else:
-                if end_time == datetime.now:
-                    end_time = datetime.now(timezone.utc)
-            end_time = int(round(end_time.timestamp()))
-            if type(sensors) == list:
-                len_sensors = len(sensors)
-                if len_sensors == 0:
-                    raise Exception('Message: No sensors provided')
-                if n < 1:
-                    raise ValueError('Incorrect number of data points')
-                n = int(n) * len_sensors
-                delimiter = ","
-                sensor_values = delimiter.join(sensors)
+            if str(onpremise).lower() == 'true':
+                url = "http://" + self.url + "/api/metaData/user"
             else:
-                raise Exception('Message: Incorrect type of sensors')
-            header = {}
-            cursor = {'end': end_time, 'limit': n}
+                url = "https://" + self.url + "/api/metaData/user"
+            header = {'userID': self.userid}
             payload = {}
-            df = pd.DataFrame()
-            counter = 0
-            while True:
-                for record in range(counter):
-                    sys.stdout.write('\r')
-                    sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
-                    sys.stdout.flush()
-                if str(onpremise).lower() == "true":
-                    url = "http://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
-                        cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
-                else:
-                    url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
-                        cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
-                response = requests.request("GET", url, headers=header, data=payload)
+            response = requests.request('GET', url, headers=header, data=payload, verify=False)
+
+            if response.status_code != 200:
                 raw = json.loads(response.text)
-                if response.status_code != 200:
-                    raise ValueError(response.status_code)
-                if 'success' in raw:
-                    raise ValueError(raw)
-                else:
-                    raw_data = json.loads(response.text)['data']
-                    cursor = json.loads(response.text)['cursor']
-                    if len(raw_data) != 0:
-                        df = pd.concat([df, pd.DataFrame(raw_data)])
-                    counter = counter + 1
-                if cursor['end'] is None:
-                    break
-            if len(df) != 0:
-                if IST:
-                    df['time'] = pd.to_datetime(df['time'], utc=False)
-                    df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
-                if str(alias).lower() == "true":
-                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
-                df = DataAccess.get_cleaned_table(self, df)
-                if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
-            return df
+                raise ValueError(raw['error'])
+            else:
+                raw_data = json.loads(response.text)['data']
+                return raw_data
+
         except Exception as e:
-            print(e)
+            print('Failed to fetch user Information')
+            print("Error: \t",e)
 
-    def fetch_data(self, device_id, start_time, end_time=datetime.now(), alias=True, sensors=None, echo=True,
-                   onpremise=False, IST=True):
+    def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=None, alias=True, IST=True,
+               onpremise=False):
         """
-        Fetch data from influxdb using apis in given timeslot
+
+        :param device_id: string
+        :param sensors: list/None
+        :param n: int
+        :param cal: bool
+        :param end_time: datetime/string
+        :param alias: bool
+        :param IST: bool
+        :param onpremise: bool
+        :return: DataFrame
         """
         metadata = {}
         if sensors is None:
             metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
 
         rawdata_res = []
         temp = ''
+        time_zone = time.tzname[0]
+        if time_zone == "IST":
+            time_zone = "India Standard Time"
+        if end_time is None:
+            end_time = datetime.now(pytz.timezone("Asia/Kolkata"))
+            end_time = end_time.strftime("%Y-%m-%d %H:%M:%S")
         try:
             end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
-        except:
-            end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
+        except ValueError:
+            try:
+                end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f').strftime('%Y-%m-%d %H:%M:%S')
+            except ValueError:
+                try:
+                    end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S.%f%z").strftime('%Y-%m-%d %H:%M:%S')
+                except:
+                    end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
+        e_time = pd.to_datetime(end_time)
+        if time_zone == "India Standard Time":
+            e_time = e_time - timedelta(hours=5.5)
+        if time_zone == "UTC":
+            e_time = e_time - timedelta(hours=5.5)
+        en_time = int(round(e_time.timestamp())) * 10000
+        if type(sensors) == list:
+            len_sensors = len(sensors)
+            if len_sensors == 0:
+                raise Exception('Message: No sensors provided')
+            if n < 1:
+                raise ValueError('Incorrect number of data points')
+            n = int(n) * len_sensors
+            delimiter = ","
+            sensor_values = delimiter.join(sensors)
+        else:
+            raise Exception('Message: Incorrect type of sensors')
+        header = {}
+        cursor = {'end': en_time, 'limit': n}
+        payload = {}
+        df = pd.DataFrame()
+        counter = 0
+        while True:
+            for record in range(counter):
+                sys.stdout.write('\r')
+                sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
+                sys.stdout.flush()
+            if str(onpremise).lower() == "true":
+                url = "http://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
+                    cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
+            else:
+                url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
+                    cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
+            response = requests.request("GET", url, headers=header, data=payload)
+            raw = json.loads(response.text)
+            if response.status_code != 200:
+                raise ValueError(response.status_code)
+            if 'success' in raw:
+                raise ValueError(raw)
+            else:
+                raw_data = json.loads(response.text)['data']
+                cursor = json.loads(response.text)['cursor']
+                if len(raw_data) != 0:
+                    df = pd.concat([df, pd.DataFrame(raw_data)])
+                counter = counter + 1
+            if cursor['end'] is None:
+                break
+        if len(df) != 0:
+            df['time'] = pd.to_datetime(df['time'])
+            if IST and time_zone == "India Standard Time":
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata')
+            if IST and time_zone == "UTC":
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata')
+            df['time'] = df['time'].dt.strftime('%Y-%m-%d %H:%M:%S')
+            df = DataAccess.get_cleaned_table(self, df)
+            if str(alias).lower() == "true":
+                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
+            if str(cal).lower() == 'true':
+                df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
+        return df
+
+    def influxdb(self, device_id, sensors, start_time, end_time=None, onpremise=False, IST=True,
+                 echo=True):
+        """
+        :param device_id: string
+        :param sensors: list/None
+        :param start_time: datetime/string
+        :param end_time: datetime/string
+        :param onpremise: bool
+        :param IST: bool
+        :param echo: bool
+        :return: DataFrame
+        """
+        metadata = {}
+        if sensors is None:
+            metadata = DataAccess.get_device_metadata(self, device_id, onpremise=onpremise)
+            data_sensor = metadata['sensors']
+            df_sensor = pd.DataFrame(data_sensor)
+            sensor_id_list = list(df_sensor['sensorId'])
+            sensors = sensor_id_list
+        rawdata_res = []
+        temp = ''
+        time_zone = time.tzname[0]
+        if time_zone == "IST":
+            time_zone = "India Standard Time"
+        flag = 0
+        if end_time is None:
+            end_time = datetime.now(pytz.timezone("Asia/Kolkata"))
+            end_time = end_time.strftime("%Y-%m-%d %H:%M:%S")
+            flag = 1
+        try:
+            end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+        except ValueError:
+            try:
+                end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f').strftime('%Y-%m-%d %H:%M:%S')
+            except ValueError:
+                try:
+                    end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S.%f%z").strftime('%Y-%m-%d %H:%M:%S')
+                except:
+                    end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
+        try:
+            start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+        except ValueError:
+            try:
+                start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S.%f').strftime('%Y-%m-%d %H:%M:%S')
+            except ValueError:
+                try:
+                    start_time = datetime.strptime(str(start_time), "%Y-%m-%d %H:%M:%S.%f%z").strftime(
+                        '%Y-%m-%d %H:%M:%S')
+                except:
+                    start_time = str(start_time) + " 00:00:00" if isinstance(start_time, str) else start_time
         s_time = pd.to_datetime(start_time)
         e_time = pd.to_datetime(end_time)
-        if IST:
-            s_time = s_time - timedelta(hours=5, minutes=30)
-            e_time = e_time - timedelta(hours=5, minutes=30)
+        if time_zone == "India Standard Time":
+            s_time = s_time - timedelta(hours=5.5)
+            e_time = e_time - timedelta(hours=5.5)
+        if time_zone == "UTC":
+            s_time = s_time - timedelta(hours=5.5)
+            e_time = e_time - timedelta(hours=5.5)
         st_time = int(round(s_time.timestamp())) * 10000
         en_time = int(round(e_time.timestamp())) * 10000
         header = {}
         payload = {}
         counter = 0
         cursor = {'start': st_time, 'end': en_time}
         while True:
@@ -406,166 +479,166 @@
                         st_time) + "&eTime=" + str(
                         en_time) + "&cursor=true&limit=50000"
                 else:
                     str1 = ","
                     sensor_values = str1.join(sensors)
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         cursor['start']) + "&eTime=" + str(cursor['end']) + "&cursor=true&limit=50000"
-
             response = requests.request("GET", temp, headers=header, data=payload)
             raw = json.loads(response.text)
             if response.status_code != 200:
                 raise ValueError(raw['error'])
             if 'success' in raw:
                 raise ValueError(raw['error'])
-
             else:
                 raw_data = json.loads(response.text)['data']
                 cursor = json.loads(response.text)['cursor']
                 if len(raw_data) != 0:
                     rawdata_res = rawdata_res + raw_data
                 counter = counter + 1
             if cursor['start'] is None or cursor['end'] is None:
                 break
 
         df = pd.DataFrame(rawdata_res)
         if len(df) != 0:
-            if IST:
-                df['time'] = pd.to_datetime(df['time'], utc=False)
-                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
+            df['time'] = pd.to_datetime(df['time'])
+            if IST and time_zone == "India Standard Time":
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata')
+            if IST and time_zone == "UTC":
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata')
+            df['time'] = df['time'].dt.strftime('%Y-%m-%d %H:%M:%S')
             if len(df.columns) == 2:
                 df['sensor'] = sensors[0]
-            if str(alias).lower() == "true":
-                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
             df = DataAccess.get_cleaned_table(self, df)
         return df
 
-    def data_query(self, device_id, sensors, start_time, end_time=datetime.now(), db=None, alias=True, cal=True,
-                   bands=None, onpremise=False, compute=None, api=False, IST=True):
+    def data_query(self, device_id, sensors, start_time, end_time=None, db=None, alias=True, cal=True,
+                   bands=None, onpremise=False, compute=None, IST=True):
         """
-
-        :param api:
-        :param compute:
-        :param onpremise:
-        :param alias:
-        :param db:
-        :param sensors:
         :param device_id: string
-        :param start_time: yyyy-MM-dd HH:MM:SS
-        :param end_time: yyyy-MM-dd HH:MM:SS
+        :param sensors: list
+        :param start_time:datetime/string
+        :param end_time: datetime/string
+        :param db: gcs,s3,az
+        :param alias: bool
         :param cal: bool
-        :param bands: None
-        :param IST: bool Indian Time Zone
-        :return: df
-
+        :param bands:
+        :param onpremise: bool
+        :param compute: mean, min, max functions
+        :param IST: Indian Standard Time
+        :return: Dataframe
         If requested data exists in feature store fetch data from the container.
         IF data is not available the data is fetched from influxdb
-
         """
-        try:
-            def get_month_year(filename):
-                month, year = map(int, filename.split('.')[0].split('-'))
-                return datetime(year, month, 1)
-
-            def generate_month_year_dates(start_date, end_date):
-                end_date = end_date.strftime("%Y-%m-%d %H:%M:%S") if isinstance(end_date, datetime) else str(end_date)
-                start_date = str(start_date) + " 00:00:00" if len(str(start_date).split()) == 1 else str(start_date)
-                end_date = str(end_date) + " 00:00:00" if len(str(end_date).split()) == 1 else str(end_date)
 
-                try:
-                    current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S")
-                    end_date = datetime.strptime(end_date, "%Y-%m-%d %H:%M:%S")
-                except:
-                    current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S.%f")
+        def get_month_year(filename):
+            month, year = map(int, filename.split('.')[0].split('-'))
+            return datetime(year, month, 1)
+
+        def generate_month_year_dates(start_date, end_date):
+            end_date = end_date.strftime("%Y-%m-%d %H:%M:%S") if isinstance(end_date, datetime) else str(end_date)
+            start_date = str(start_date) + " 00:00:00" if len(str(start_date).split()) == 1 else str(start_date)
+            end_date = str(end_date) + " 00:00:00" if len(str(end_date).split()) == 1 else str(end_date)
+
+            try:
+                current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S")
+                end_date = datetime.strptime(end_date, "%Y-%m-%d %H:%M:%S")
+            except:
+                current_date = datetime.strptime(start_date, "%Y-%m-%d %H:%M:%S.%f")
+
+            dates = []
+            while str(current_date) <= str(end_date):
+                month = str(current_date.month)
+                month_year = month + "-" + str(current_date.year) + ".parquet"
+                dates.append(month_year)
+                current_date += relativedelta(months=1)
+                current_date = current_date.replace(day=1)
+
+            return dates
+
+        def read_one(filename):
+            with connector.open(container_name + str(device_id) + "/" + str(filename),
+                                "rb") as src_file:
+                df = pd.read_parquet(src_file)
+            return df
 
-                dates = []
-                while str(current_date) <= str(end_date):
-                    month = str(current_date.month)
-                    month_year = month + "-" + str(current_date.year) + ".parquet"
-                    dates.append(month_year)
-                    current_date += relativedelta(months=1)
-                    current_date = current_date.replace(day=1)
-
-                return dates
-
-            def read_one(filename):
-                with connector.open(container_name + str(device_id) + "/" + str(filename),
-                                    "rb") as src_file:
-                    df = pd.read_parquet(src_file)
-                return df
-
-            def thread_read(filenames_list):
-                if len(filenames_list) != 0:
-                    with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
-                        for record in range(len(filenames_list)):
-                            sys.stdout.write('\r')
-                            sys.stdout.write("Please Wait .. ")
-                            sys.stdout.flush()
-                        results = executor.map(read_one, filenames_list)
-                    fetched_df = pd.concat(results, axis=0)
-                else:
-                    fetched_df = pd.DataFrame()
-                return fetched_df
-            start_time = pd.to_datetime(start_time)
-            if type(end_time) == str:
+        def thread_read(filenames_list):
+            if len(filenames_list) != 0:
+                with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
+                    for record in range(len(filenames_list)):
+                        sys.stdout.write('\r')
+                        sys.stdout.write("Please Wait .. ")
+                        sys.stdout.flush()
+                    results = executor.map(read_one, filenames_list)
+                fetched_df = pd.concat(results, axis=0)
+            else:
+                fetched_df = pd.DataFrame()
+            return fetched_df
+
+        df = pd.DataFrame()
+        metadata = {}
+        connector = None
+        container_name = None
+
+        if db is not None:
+            flag = 0
+            time_zone = time.tzname[0]
+            if time_zone == "IST":
+                time_zone = "India Standard Time"
+            if end_time is None:
+                end_time = datetime.now(pytz.timezone("Asia/Kolkata"))
+                end_time = end_time.strftime("%Y-%m-%d %H:%M:%S")
+                flag = 1
+            try:
+                end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+            except ValueError:
                 try:
-                    end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+                    end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f').strftime('%Y-%m-%d %H:%M:%S')
                 except ValueError:
                     try:
-                        end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f').strftime(
+                        end_time = datetime.strptime(str(end_time), "%Y-%m-%d %H:%M:%S.%f%z").strftime(
                             '%Y-%m-%d %H:%M:%S')
-                    except Exception:
+                    except:
                         end_time = str(end_time) + " 23:59:59" if isinstance(end_time, str) else end_time
-            else:
-                india_timezone = pytz.timezone('Asia/Kolkata')
-                end_time = end_time.astimezone(india_timezone)
-                end_time = end_time.strftime('%Y-%m-%d %H:%M:%S')
-            df = pd.DataFrame()
-            metadata = {}
-            connector = None
-            container_name = None
-            if db is not None:
-                credentials = DataAccess.get_cloud_credentials(self, db)
-                if len(credentials) !=0:
-                    if db == "gcs":
-                        credentials = eval(credentials)
-                        connector = fsspec.filesystem("gs", project=credentials['project_id'],
-                                                      token=credentials)
-                        container_name = "faclon-ds-feature-store/"
-
-                    elif db == "az":
-                        connector = fsspec.filesystem("az", account_name=credentials[0],
-                                                      account_key=credentials[1])
-                        container_name = "feature-store/"
-
-                    elif db == "s3":
-                        connector = fsspec.filesystem("s3", key=credentials[0],
-                                                      secret=credentials[1])
-                        container_name = "faclon-ai-public-bucket/"
-
-                    else:
-                        raise Exception('Enter correct Database name')
-
-                    blobs = connector.ls(container_name)
-                    device_list = [blob.split("/")[1] for blob in blobs]
-                    if device_id in device_list:
-                        blobs = [blob_name.split("/")[2] for blob_name in connector.ls(container_name + str(device_id) + "/")]
-                        dates = generate_month_year_dates(start_time, end_time)
-                        filenames = list(set(dates).intersection(blobs))
-                        filenames = sorted(filenames, key=get_month_year)
-                        df = thread_read(filenames)
+            try:
+                start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S').strftime('%Y-%m-%d %H:%M:%S')
+            except ValueError:
+                try:
+                    start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S.%f').strftime(
+                        '%Y-%m-%d %H:%M:%S')
+                except ValueError:
+                    try:
+                        start_time = datetime.strptime(str(start_time), "%Y-%m-%d %H:%M:%S.%f%z").strftime(
+                            '%Y-%m-%d %H:%M:%S')
+                    except:
+                        start_time = str(start_time) + " 00:00:00" if isinstance(start_time, str) else start_time
+            credentials = DataAccess.get_cloud_credentials(self, db)
+            if len(credentials) != 0:
+                credentials = eval(credentials)
+                connector = fsspec.filesystem("gs", project=credentials['project_id'],
+                                              token=credentials)
+                container_name = "faclon-ds-feature-store/"
+
+                blobs = connector.ls(container_name)
+                device_list = [blob.split("/")[1] for blob in blobs]
+                if device_id in device_list:
+                    blobs = [blob_name.split("/")[2] for blob_name in
+                             connector.ls(container_name + str(device_id) + "/")]
+                    dates = generate_month_year_dates(start_time, end_time)
+                    filenames = list(set(dates).intersection(blobs))
+                    filenames = sorted(filenames, key=get_month_year)
+                    df = thread_read(filenames)
                 if len(df) != 0:
                     try:
                         start_time = datetime.strptime(str(start_time), '%Y-%m-%d %H:%M:%S')
                         end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
                     except ValueError:
                         pass
                     except Exception as e:
                         print('Message:', e)
-
                     df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
                     if len(df) != 0:
                         if sensors is None:
                             sensors = list(df.columns)
                             sensors.remove('time')
 
                         sensors_filtered = list(set(df.columns).intersection(sensors))
@@ -573,41 +646,48 @@
                             sensors_filtered.insert(0, 'time')
                             df = df[sensors_filtered]
                         else:
                             df = pd.DataFrame()
                         df.sort_values(['time'], inplace=True)
                         df.reset_index(drop=True, inplace=True)
                         last_date = df['time'].iloc[-1]
-                        if str(last_date) < str(end_time):
-                            df1 = DataAccess.fetch_data(self, device_id, start_time=last_date, alias=False,
-                                                        end_time=end_time, sensors=sensors, echo=True,
-                                                        onpremise=onpremise, IST=True)
+                        last_date = last_date.to_pydatetime()
+                        date1 = datetime.strptime(str(last_date), '%Y-%m-%d %H:%M:%S.%f')
+                        try:
+                            date2 = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
+                        except:
+                            date2 = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S.%f')
+                        difference = date2 - date1
+                        if difference.seconds >= 3600 or difference.seconds >= 60:
+                            if time_zone == "UTC" and flag == 0:
+                                last_date = last_date + timedelta(hours=5.5)
+                                end_time = end_time + timedelta(hours=5.5)
+                            df1 = DataAccess.influxdb(self, device_id, start_time=last_date,
+                                                      end_time=end_time, sensors=sensors, echo=True,
+                                                      onpremise=False, IST=True)
                             df = pd.concat([df, df1])
                             df.reset_index(drop=True, inplace=True)
+                        if IST is False:
+                            df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5.5)
+        else:
+            df_devices = DataAccess.get_device_details(self, onpremise=onpremise)
+            device_list = df_devices['devID'].tolist()
+            if device_id in device_list:
+                df = DataAccess.influxdb(self, device_id, sensors, start_time, end_time=end_time, onpremise=onpremise,
+                                         IST=IST, echo=True)
             else:
-                df_devices = DataAccess.get_device_details(self,onpremise=onpremise)
-                device_list = df_devices['devID'].tolist()
-                if device_id in device_list:
-                    df = DataAccess.fetch_data(self, device_id, start_time, end_time, alias, sensors=sensors, echo=True,
-                                               onpremise=onpremise, IST=IST)
-                else:
-                    raise Exception('Message: Device not added in account')
+                raise Exception('Message: Device not added in account')
 
-            if len(df) != 0:
-                if str(alias).lower() == "true":
-                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
-
-                if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
-
-                if bands is not None:
-                    df = DataAccess.time_grouping(self, df, bands, compute)
-                df = df.set_index(['time'])
-                df = df.fillna(value=np.nan)
-                df.dropna(axis=0, how='all', inplace=True)
-                df.reset_index(drop=False, inplace=True)
-                df.drop_duplicates(inplace=True)
-                if IST is False and db is not None:
-                    df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5, minutes=30)
-            return df
-        except Exception as e:
-            print(e)
+        if len(df) != 0:
+            df['time'] = pd.to_datetime(df['time'])
+            if str(alias).lower() == "true":
+                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata, onpremise=onpremise)
+            if str(cal).lower() == 'true':
+                df = DataAccess.get_caliberation(self, device_id, metadata, df, onpremise=onpremise)
+            if bands is not None:
+                df = DataAccess.time_grouping(self, df, bands, compute)
+            df = df.set_index(['time'])
+            df = df.fillna(value=np.nan)
+            df.dropna(axis=0, how='all', inplace=True)
+            df.reset_index(drop=False, inplace=True)
+            df.drop_duplicates(inplace=True)
+        return df
```

### Comparing `iosense_connect-4.0.4/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iosense-connect
-Version: 4.0.4
+Name: iosense_connect
+Version: 4.0.5
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-4.0.4/setup.py` & `iosense_connect-4.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "4.0.4",
+    version = "4.0.5",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
```

