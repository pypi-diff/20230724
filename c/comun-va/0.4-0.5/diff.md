# Comparing `tmp/comun_va-0.4.tar.gz` & `tmp/comun_va-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-0.4.tar", last modified: Tue Jul 18 05:40:48 2023, max compression
+gzip compressed data, was "comun_va-0.5.tar", last modified: Mon Jul 24 10:12:00 2023, max compression
```

## Comparing `comun_va-0.4.tar` & `comun_va-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:40:48.902835 comun_va-0.4/
--rw-rw-rw-   0        0        0       53 2023-07-18 05:40:48.902835 comun_va-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 05:40:48.901829 comun_va-0.4/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2023-07-18 05:40:48.000000 comun_va-0.4/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-07-18 05:40:48.000000 comun_va-0.4/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:40:48.000000 comun_va-0.4/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-18 05:40:48.000000 comun_va-0.4/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 05:40:48.000000 comun_va-0.4/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4554 2023-07-18 05:40:46.000000 comun_va-0.4/comun_va.py
--rw-rw-rw-   0        0        0       42 2023-07-18 05:40:48.902835 comun_va-0.4/setup.cfg
--rw-rw-rw-   0        0        0      192 2023-07-18 05:40:46.000000 comun_va-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 10:12:00.574479 comun_va-0.5/
+-rw-rw-rw-   0        0        0       53 2023-07-24 10:12:00.574479 comun_va-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 10:12:00.573478 comun_va-0.5/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-07-24 10:12:00.000000 comun_va-0.5/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-24 10:12:00.000000 comun_va-0.5/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 10:12:00.000000 comun_va-0.5/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-24 10:12:00.000000 comun_va-0.5/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 10:12:00.000000 comun_va-0.5/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5058 2023-07-24 10:11:44.000000 comun_va-0.5/comun_va.py
+-rw-rw-rw-   0        0        0       42 2023-07-24 10:12:00.575720 comun_va-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      192 2023-07-24 10:11:44.000000 comun_va-0.5/setup.py
```

### Comparing `comun_va-0.4/comun_va.py` & `comun_va-0.5/comun_va.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,21 +25,32 @@
                 Date: {self.date_time},
                 Endpoint name: {self.endpoint_name},
                 Endpoint received data: {self.endpoint_data_received},
                 Result: {self.result},
                 Prediction: {self.prediction}         
                 """
 
-    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str):
+    def save_log(self, mssql_srv: str, database: str, user: str, passwd: str, rescaled_size: tuple = None):
+        """
+        Save the image in local path and the data into the DB.
+        :param mssql_srv: IP of the MSsql server
+        :param database: Name of the database
+        :param user: User of the database
+        :param passwd: Password of the user
+        :param rescaled_size: example = (224,224)
+        :return: doesn't return anything
+        """
         # SAVE IMAGE:
         if self.img_frame is not None:
             if self.img_name is None:
                 self.img_name = f'{self.date_time.strftime("%Y_%m_%d_%H_%M_%S")}.jpg'
             if self.img_path is None:
                 self.img_path = f'img_save/{self.img_name}'
+            if rescaled_size:
+                self.img_frame = cv2.resize(self.img_frame, rescaled_size)
             cv2.imwrite(self.img_path, self.img_frame)
 
         # SAVE LOG IN DB:
         mssql = comun_sqlsrv.Sql(mssql_srv, database, user, passwd)
         query = f"""
                 INSERT INTO T_VA_API_LOG
                 (FECHA_HORA, ENDPOINT, RESULTADO, DATO_RECIBIDO, PREDICCION_VA, NOMBRE_IMAGEN, COD_BAR, ERROR)
```

