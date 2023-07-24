# Comparing `tmp/iorodeo-potentiostat-0.0.7.tar.gz` & `tmp/iorodeo-potentiostat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iorodeo-potentiostat-0.0.7.tar", last modified: Wed Mar 15 21:50:23 2023, max compression
+gzip compressed data, was "iorodeo-potentiostat-0.0.8.tar", last modified: Mon Jul 24 16:39:40 2023, max compression
```

## Comparing `iorodeo-potentiostat-0.0.7.tar` & `iorodeo-potentiostat-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-03-15 21:50:23.366618 iorodeo-potentiostat-0.0.7/
--rw-rw-r--   0 wbd       (1000) wbd       (1000)     1126 2023-01-27 18:51:35.000000 iorodeo-potentiostat-0.0.7/LICENSE.txt
--rw-rw-r--   0 wbd       (1000) wbd       (1000)       47 2023-01-27 18:51:35.000000 iorodeo-potentiostat-0.0.7/MANIFEST.in
--rw-rw-r--   0 wbd       (1000) wbd       (1000)     2300 2023-03-15 21:50:23.366618 iorodeo-potentiostat-0.0.7/PKG-INFO
--rw-rw-r--   0 wbd       (1000) wbd       (1000)      881 2023-03-15 00:11:20.000000 iorodeo-potentiostat-0.0.7/README.md
-drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-03-15 21:50:23.366618 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/
--rw-rw-r--   0 wbd       (1000) wbd       (1000)     2300 2023-03-15 21:50:23.000000 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/PKG-INFO
--rw-rw-r--   0 wbd       (1000) wbd       (1000)      325 2023-03-15 21:50:23.000000 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/SOURCES.txt
--rw-rw-r--   0 wbd       (1000) wbd       (1000)        1 2023-03-15 21:50:23.000000 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/dependency_links.txt
--rw-rw-r--   0 wbd       (1000) wbd       (1000)       23 2023-03-15 21:50:23.000000 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/requires.txt
--rw-rw-r--   0 wbd       (1000) wbd       (1000)       13 2023-03-15 21:50:23.000000 iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/top_level.txt
-drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-03-15 21:50:23.366618 iorodeo-potentiostat-0.0.7/potentiostat/
--rw-rw-r--   0 wbd       (1000) wbd       (1000)       75 2023-03-15 21:50:15.000000 iorodeo-potentiostat-0.0.7/potentiostat/__init__.py
--rw-rw-r--   0 wbd       (1000) wbd       (1000)    37666 2023-03-15 21:46:38.000000 iorodeo-potentiostat-0.0.7/potentiostat/potentiostat.py
--rw-rw-r--   0 wbd       (1000) wbd       (1000)       67 2023-03-15 21:50:23.366618 iorodeo-potentiostat-0.0.7/setup.cfg
--rw-rw-r--   0 wbd       (1000) wbd       (1000)     2560 2023-03-15 21:50:02.000000 iorodeo-potentiostat-0.0.7/setup.py
+drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-07-24 16:39:40.099130 iorodeo-potentiostat-0.0.8/
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)     1126 2020-12-28 20:16:11.000000 iorodeo-potentiostat-0.0.8/LICENSE.txt
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)       47 2020-12-28 20:16:11.000000 iorodeo-potentiostat-0.0.8/MANIFEST.in
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)     2300 2023-07-24 16:39:40.099130 iorodeo-potentiostat-0.0.8/PKG-INFO
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)      881 2023-03-15 22:37:01.000000 iorodeo-potentiostat-0.0.8/README.md
+drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-07-24 16:39:40.095130 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)     2300 2023-07-24 16:39:39.000000 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/PKG-INFO
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)      325 2023-07-24 16:39:39.000000 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)        1 2023-07-24 16:39:39.000000 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)       23 2023-07-24 16:39:39.000000 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/requires.txt
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)       13 2023-07-24 16:39:39.000000 iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/top_level.txt
+drwxrwxr-x   0 wbd       (1000) wbd       (1000)        0 2023-07-24 16:39:40.099130 iorodeo-potentiostat-0.0.8/potentiostat/
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)       75 2023-07-18 19:43:21.000000 iorodeo-potentiostat-0.0.8/potentiostat/__init__.py
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)    38878 2023-07-21 15:56:14.000000 iorodeo-potentiostat-0.0.8/potentiostat/potentiostat.py
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)       67 2023-07-24 16:39:40.099130 iorodeo-potentiostat-0.0.8/setup.cfg
+-rw-rw-r--   0 wbd       (1000) wbd       (1000)     2560 2023-07-18 19:43:10.000000 iorodeo-potentiostat-0.0.8/setup.py
```

### Comparing `iorodeo-potentiostat-0.0.7/LICENSE.txt` & `iorodeo-potentiostat-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iorodeo-potentiostat-0.0.7/PKG-INFO` & `iorodeo-potentiostat-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorodeo-potentiostat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Serial interface for the Rodeostat Potentiostat
 Home-page: https://github.com/iorodeo/potentiostat
 Author: Will Dickson
 Author-email: will@iorodeo.com
 License: MIT
 Keywords: Serial interface for IO Rodeo Potentiostat
 Platform: UNKNOWN
```

### Comparing `iorodeo-potentiostat-0.0.7/README.md` & `iorodeo-potentiostat-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `iorodeo-potentiostat-0.0.7/iorodeo_potentiostat.egg-info/PKG-INFO` & `iorodeo-potentiostat-0.0.8/iorodeo_potentiostat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iorodeo-potentiostat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Serial interface for the Rodeostat Potentiostat
 Home-page: https://github.com/iorodeo/potentiostat
 Author: Will Dickson
 Author-email: will@iorodeo.com
 License: MIT
 Keywords: Serial interface for IO Rodeo Potentiostat
 Platform: UNKNOWN
```

### Comparing `iorodeo-potentiostat-0.0.7/potentiostat/potentiostat.py` & `iorodeo-potentiostat-0.0.8/potentiostat/potentiostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,16 +180,17 @@
         timeout (float): serial port ready timeout (seconds)
 
     """
 
     
     ResetSleepDt = 0.0
     Baudrate = 115200
+    DefaultTimeout = 2.0
 
-    def __init__(self, port, timeout=10.0):
+    def __init__(self, port, timeout=DefaultTimeout):
         params = {'baudrate': self.Baudrate, 'timeout': timeout}
         super(Potentiostat,self).__init__(port,**params)
         time.sleep(self.ResetSleepDt)
         self.test_running = False
         atexit.register(self.atexit_cleanup)
         while self.inWaiting() > 0:
             val = self.read()
@@ -206,18 +207,18 @@
 
         """
         cmd_dict = {CommandKey: GetVariantCmd}
         msg_dict = self.send_cmd(cmd_dict)
         return msg_dict[ResponseKey][VariantKey]
 
 
-    def stop_test(self):
+    def stop_test(self,rsp=True):
         """Stops (any) currently running tests. """
         cmd_dict = {CommandKey: StopTestCmd}
-        msg_dict = self.send_cmd(cmd_dict)
+        msg_dict = self.send_cmd(cmd_dict, rsp=rsp)
 
 
     def get_volt(self):
         """Returns the output voltage setting, i.e, the potential between the
         working and reference electrode. 
 
         Returns:
@@ -873,16 +874,16 @@
         """Disconnects all electrodes (reference, counter and working) when
         using the multiplexer expansion hardware.
         """
         cmd_dict = {CommandKey: DisconnAllMuxElectCmd}
         msg_dict = self.send_cmd(cmd_dict)
 
 
-    def run_test(self, testname, 
-            param=None, filename=None, on_data=None, display='pbar', timeunit='s'):
+    def run_test(self, testname, param=None, filename=None, on_data=None, display='pbar', 
+            timeunit='s', max_decode_err=0):
         """Runs the test with specified test name and returns the time, voltage
         and current data.
 
         Args:
             testname (str): name of test to run, e.g., 'cyclic', 'constant', linearSweep'
 
         Keyword Args:
@@ -898,14 +899,20 @@
             display  (str): output display mode, display=='pbar' show a progressbar,  
                 display=='data' shows a text stream and display=='' shows nothing 
 
             timeunit (str): units for time values, if timeunit=='s' then time
                 values are in seconds otherwise if timeunit=='ms' then time values
                 are is milliseconds.
 
+            max_decode_err (int): maximum number of allowed json decode errors during 
+                streaming before an exception (DataDecodeException) is rasied. 
+                If max_decode_err=0 (default) then no decode errors are allowed. 
+                If max_decode_err=None (default) then exceptions will not be triggered 
+                and decode errors will pass silently.  
+
         Returns:
             tuple/dict: data acquired during test. 
             
             When the multiplexer is disabled a tuple (t,volt,curr) of lists is
             returned containing the measurement times (s), voltages (V) and
             currents (uA) respectively
 
@@ -958,54 +965,65 @@
 
         # Start voltammetric test
         cmd_dict = {CommandKey: RunTestCmd, TestKey: testname}
         msg_dict = self.send_cmd(cmd_dict)
         self.test_running = True
 
         done = False
+        num_decode_err = 0
+
         while not done:
 
             # Get data from device
             sample_json = self.readline()
             sample_json = sample_json.strip()
-            sample_dict = json.loads(sample_json.decode())
 
-            if len(sample_dict) > 0:
+            try:
+                sample_dict = json.loads(sample_json.decode())
+            except json.decoder.JSONDecodeError as err:
+                num_decode_err += 1
+                if (max_decode_err is not None) and (num_decode_err > max_decode_err):
+                    err_msg = f'num_decode_err({num_decode_err}) > max_decode_err({max_decode_err})'
+                    raise DataDecodeException(err_msg)
+                else:
+                    continue
+            try:
                 tval = sample_dict[TimeKey]*TimeUnitToScale[timeunit]
                 volt = sample_dict[VoltKey]
                 curr = sample_dict[CurrKey]
-                chan = 0  # Dummy channel used when mux isn't running
-
-                if mux_enabled:
-                    chan = sample_dict[ChanKey]
+            except KeyError:
+                done = True
+                break
 
-                for k,v in [(TimeKey,tval),(VoltKey,volt),(CurrKey,curr)]:
-                    data_dict[chan][k].append(v)
+            chan = 0  # Dummy channel used when mux isn't running
+            if mux_enabled:
+                chan = sample_dict[ChanKey]
 
-                # Write data to file
-                if (filename is not None) and (output_filetype == TxtOutputFileType):
-                    if chan == 0:
-                        fid.write('{0:1.3f}, {1:1.4f}, {2:1.4f}\n'.format(tval,volt,curr))
-                    else:
-                        fid.write('{0}, {1:1.3f}, {2:1.4f}, {3:1.4f}\n'.format(chan,tval,volt,curr))
+            for k,v in [(TimeKey,tval),(VoltKey,volt),(CurrKey,curr)]:
+                data_dict[chan][k].append(v)
 
-                # Handle diplay options
-                if display == 'data':
-                    if chan == 0:
-                        print('{0:1.3f}, {1:1.4f}, {2:1.4f}'.format(tval,volt,curr))
-                    else:
-                        print('ch{0}: {1:1.3f}, {2:1.4f}, {3:1.4f}'.format(chan,tval,volt,curr))
-                elif display == 'pbar':
-                    pbar.update(tval)
-
-                # Pass data to callback function if present
-                if on_data is not None:
-                    on_data(chan, tval, volt, curr)
-            else:
-                done = True
+            # Write data to file
+            if (filename is not None) and (output_filetype == TxtOutputFileType):
+                if chan == 0:
+                    fid.write('{0:1.3f}, {1:1.4f}, {2:1.4f}\n'.format(tval,volt,curr))
+                else:
+                    fid.write('{0}, {1:1.3f}, {2:1.4f}, {3:1.4f}\n'.format(chan,tval,volt,curr))
+
+            # Handle diplay options
+            if display == 'data':
+                if chan == 0:
+                    print('{0:1.3f}, {1:1.4f}, {2:1.4f}'.format(tval,volt,curr))
+                else:
+                    print('ch{0}: {1:1.3f}, {2:1.4f}, {3:1.4f}'.format(chan,tval,volt,curr))
+            elif display == 'pbar':
+                pbar.update(tval)
+
+            # Pass data to callback function if present
+            if on_data is not None:
+                on_data(chan, tval, volt, curr)
 
         self.test_running = False
 
         if display_print:
             print()
             print()
 
@@ -1021,15 +1039,15 @@
 
         if mux_enabled:
             return data_dict 
         else:
             return data_dict[0][TimeKey], data_dict[0][VoltKey], data_dict[0][CurrKey]
 
 
-    def send_cmd(self,cmd_dict):
+    def send_cmd(self, cmd_dict, rsp=True):
         """Sends a command to the device.  Low-level method - command is specified 
         using command dictionary.
 
         Args:
             cmd_dict (dict): commands to be sent to the device, e.g., {'command': 'getVersion'}
 
         Returns:
@@ -1037,20 +1055,20 @@
 
             For example, the response to {'command': 'getVersion'} might be
             {'success': True, 'response': {'command': 'getVersion', 'version': 'FW0.0.8'}}
 
         """
         cmd_json = json.dumps(cmd_dict) + '\n'
         self.write(cmd_json.encode())
-        msg_json = self.readline()
-        #print(msg_json)
-        msg_json = msg_json.strip()
-        msg_dict = json.loads(msg_json.decode())
-        self.check_cmd_msg(cmd_dict,msg_dict)
-        return msg_dict
+        if rsp:
+            msg_json = self.readline()
+            msg_json = msg_json.strip()
+            msg_dict = json.loads(msg_json.decode())
+            self.check_cmd_msg(cmd_dict,msg_dict)
+            return msg_dict
 
 
     def check_cmd_msg(self,cmd_dict,msg_dict):
         """
         Checks the msg response to a given command. 
 
         :meta private:
@@ -1129,22 +1147,34 @@
             hw_version (str): string representing hardware version to check, e.g., 'HW0.2'
 
         """
         if self.hardware_version < hw_version:
             raise RuntimeError('requires hardware version >= {}'.format(HardwareVersion0p2))
 
 
-    def atexit_cleanup(self):
+    def __del__(self):
         """
         :meta private:
         """
         if self.isOpen() and self.test_running:
-            self.stop_test()
-
+            try:
+                self.stop_test(rsp=False)
+            except json.decoder.JSONDecodeError:
+                pass
+        self.close()
 
 
+    def atexit_cleanup(self):
+        """
+        :meta private:
+        """
+        self.__del__()
 
 
+# Custom Exceptions
+# ----------------------------------------------------------------------------------
 
+class DataDecodeException(Exception):
+    pass
```

### Comparing `iorodeo-potentiostat-0.0.7/setup.py` & `iorodeo-potentiostat-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name='iorodeo-potentiostat',
-    version='0.0.7',
+    version='0.0.8',
     description='Serial interface for the Rodeostat Potentiostat',
     long_description=__doc__,
     url='https://github.com/iorodeo/potentiostat',
     author='Will Dickson',
     author_email='will@iorodeo.com',
     license='MIT',
```

