# Comparing `tmp/metathing-0.3.3-py3-none-any.whl.zip` & `tmp/metathing-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23042 bytes, number of entries: 14
+Zip file size: 23088 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-16 20:12 metathing/__init__.py
 -rw-r--r--  2.0 unx     2210 b- defN 23-Jul-16 20:12 metathing/alarmer.py
--rw-r--r--  2.0 unx    10640 b- defN 23-Jul-18 18:05 metathing/application.py
+-rw-r--r--  2.0 unx    10859 b- defN 23-Jul-23 22:29 metathing/application.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Jul-16 20:12 metathing/config.py
 -rw-r--r--  2.0 unx    20160 b- defN 23-Jul-18 05:14 metathing/device.py
 -rw-r--r--  2.0 unx    16120 b- defN 23-Jul-17 07:21 metathing/http.py
 -rw-r--r--  2.0 unx     1520 b- defN 23-Jul-17 09:21 metathing/logger.py
 -rw-r--r--  2.0 unx    21631 b- defN 23-Jul-20 01:11 metathing/metathing.py
 -rw-r--r--  2.0 unx     6946 b- defN 23-Jul-17 07:21 metathing/mqtt.py
 -rw-r--r--  2.0 unx     3990 b- defN 23-Jul-17 07:22 metathing/service.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jul-20 01:12 metathing-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 01:12 metathing-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-20 01:12 metathing-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-20 01:12 metathing-0.3.3.dist-info/RECORD
-14 files, 84845 bytes uncompressed, 21288 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx      163 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-23 22:30 metathing-0.3.4.dist-info/RECORD
+14 files, 85064 bytes uncompressed, 21334 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: metathing/mqtt.py
 Comment: 
 
 Filename: metathing/service.py
 Comment: 
 
-Filename: metathing-0.3.3.dist-info/METADATA
+Filename: metathing-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: metathing-0.3.3.dist-info/WHEEL
+Filename: metathing-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: metathing-0.3.3.dist-info/top_level.txt
+Filename: metathing-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: metathing-0.3.3.dist-info/RECORD
+Filename: metathing-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metathing/application.py

```diff
@@ -12,32 +12,36 @@
 
 class Application():
     def __init__(self):
         self.srv = None
         self.Dev = None
         self.event_sender = {}
         self.devs = {}
+        self.status = {'global': {}}
 
     def AddDev(self, model):
         if self.Dev is None:
             raise Exception("Device model not defined!")
         dev_id = model['dev_id']
         if 'init_config' in model:
             config = model['init_config']
         config['dev_id'] = dev_id
         self.devs[dev_id] = self.Dev(self.srv, config)
+        self.devs[dev_id].status = {}
+        self.status[dev_id] = self.devs[dev_id].status
         
     def UpdateDev(self, model):
         self.AddDev(model)
 
     def DeleteDev(self, id):
         if (id in self.devs):
             print("Releasing: "+id)
             self.devs[id].release()
             del self.devs[id]
+            del self.status[id]
 
     def DevsInfo(self):
         devs_info = {}
         for _dev_id, dev in self.devs.items():
             devs_info[_dev_id] = dev.model
         return devs_info
         
@@ -49,15 +53,14 @@
             if fn_name in self.event_sender:
                 for topic in self.event_sender[fn_name]:
                     self.srv.mqtt.publish(topic, json.dumps(result))
             return result
         wrapper.__is_event__ = func
         return wrapper
     
-        
     def BindAction(self, model):
         fn_name = model['tag']
         # Check action
         if hasattr(self, fn_name) == False:
             logger.error("Action not found [{0}]".format(fn_name))
             return False
         fn = getattr(self, fn_name)
@@ -260,8 +263,11 @@
         logger.info(frame)
               
     # Customized functions
     def ping(self):
         return "OK"
           
     def release(self):
-        return {}
+        return {}
+    
+    def status(self):
+        return {"status": self.status}
```

## Comparing `metathing-0.3.3.dist-info/RECORD` & `metathing-0.3.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 metathing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 metathing/alarmer.py,sha256=qXCTl8zw3UTqbDqvvPAHU-a1uJqxlAkxzQWf-5nVB3Q,2210
-metathing/application.py,sha256=g95MWraawiDr5xHbv3anHUqDGno7urry9OpKojiNC0s,10640
+metathing/application.py,sha256=K5juHHwfQ9n9hGkRZ3NJZvazYLVb_w3msT79S7bxEp0,10859
 metathing/config.py,sha256=SZs7VXZeNQ4BwexSjsB_YJk6CPNwNMyvEpaXlztea-s,290
 metathing/device.py,sha256=8HzJv7zCm1FthWrwvPKK823rhY4J3Q7iKtin79lNK5c,20160
 metathing/http.py,sha256=xaTP2BHFxd9BTMHoM_grY_O9kzhip608P0RfivmDo0A,16120
 metathing/logger.py,sha256=ZX1t9Yuibg6Ortkimet3h2DxrnQCpSszvrFrJZQYXPc,1520
 metathing/metathing.py,sha256=eYXA_XNFlTtXonphPH25fo0IStaBuvjtyBntSggRM-k,21631
 metathing/mqtt.py,sha256=05DvcdV46YeWiBFpI3LWL2frQCrvJXqf8_VYPC-iyyY,6946
 metathing/service.py,sha256=OOTjDLb00s1mRSLg2q4egbZDAUevz_IueL63el-I8u4,3990
-metathing-0.3.3.dist-info/METADATA,sha256=0ipoELlBPWpOJIARE1ozJSM90n1LUpB_kae-RhEcyDk,163
-metathing-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-metathing-0.3.3.dist-info/top_level.txt,sha256=O2krbfropyUTFNX_RrOEn4VwPiaKXYRwSNjbuj31gP8,10
-metathing-0.3.3.dist-info/RECORD,,
+metathing-0.3.4.dist-info/METADATA,sha256=D8470azsuXbUkEXdad3lYzUockulrki__ua2b6p6MJQ,163
+metathing-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+metathing-0.3.4.dist-info/top_level.txt,sha256=O2krbfropyUTFNX_RrOEn4VwPiaKXYRwSNjbuj31gP8,10
+metathing-0.3.4.dist-info/RECORD,,
```

