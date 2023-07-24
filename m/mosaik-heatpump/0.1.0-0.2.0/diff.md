# Comparing `tmp/mosaik-heatpump-0.1.0.tar.gz` & `tmp/mosaik-heatpump-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-heatpump-0.1.0.tar", last modified: Wed Jun 30 21:29:03 2021, max compression
+gzip compressed data, was "mosaik-heatpump-0.2.0.tar", last modified: Mon Jul 24 15:38:50 2023, max compression
```

## Comparing `mosaik-heatpump-0.1.0.tar` & `mosaik-heatpump-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      121 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/CHANGES.txt
--rw-rw-rw-   0 root         (0) root         (0)    26478 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11358 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10095 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/controller/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/controller/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4384 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/controller/controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/controller/controller_mosaik.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/
--rw-rw-rw-   0 root         (0) root         (0)   804209 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/COP_m_data.json
--rw-rw-rw-   0 root         (0) root         (0)    14653 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/Heat_Pump_Des.py
--rw-rw-rw-   0 root         (0) root         (0)     4878 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/Heat_Pump_Model.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/Heat_Pump_mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3737 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/data_file.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24542 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/hotwatertank.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/hotwatertank_mosaik.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      851 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-30 21:29:03.000000 mosaik-heatpump-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1549 2021-06-30 21:28:28.000000 mosaik-heatpump-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.317185 mosaik-heatpump-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/CHANGES.txt
+-rw-rw-rw-   0 root         (0) root         (0)    26478 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11869 2023-07-24 15:38:50.317185 mosaik-heatpump-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10100 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.298186 mosaik-heatpump-0.2.0/mosaik_heatpump/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.299186 mosaik-heatpump-0.2.0/mosaik_heatpump/controller/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/controller/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/controller/controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/controller/controller_mosaik.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.316185 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/
+-rw-rw-rw-   0 root         (0) root         (0)    23476 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/Heat_Pump_Des.py
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/Heat_Pump_Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/Heat_Pump_mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0) 22306846 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/cop_m_data.json
+-rw-rw-rw-   0 root         (0) root         (0)    47702 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/eta_s_data.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.317185 mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24440 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/hotwatertank.py
+-rw-rw-rw-   0 root         (0) root         (0)     5814 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/hotwatertank_mosaik.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:38:50.298186 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11869 2023-07-24 15:38:50.000000 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      810 2023-07-24 15:38:50.000000 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:38:50.000000 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-24 15:38:50.000000 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 15:38:50.000000 mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:38:50.317185 mosaik-heatpump-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-07-24 15:38:20.000000 mosaik-heatpump-0.2.0/setup.py
```

### Comparing `mosaik-heatpump-0.1.0/LICENSE` & `mosaik-heatpump-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaik-heatpump-0.1.0/PKG-INFO` & `mosaik-heatpump-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mosaik-heatpump
-Version: 0.1.0
+Version: 0.2.0
 Summary: Mosaik-heatpump provides a model of a residential heatpump system
 Home-page: https://gitlab.com/mosaik/components/energy/mosaik-heatpump
 Author: Pranay Kasturi
 Author-email: mosaik@offis.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 mosaik-heatpump
@@ -107,15 +107,15 @@
 between 30 to 55 (deg. C). For the water source heat pump, the heat source temperature can vary between 4 to 20 (deg. C). and the condenser 
 inlet temperature can vary between 20 to 55 (deg. C). 
 
 Advanced Details of the Model
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The heat pump model available in TESPy's library was modified and the new schematic of the system is shown below.
 
-.. image:: images/system_schematic.png
+.. image:: docs/images/system_schematic.png
    :width: 600
 
 The consumer system and the expansion valve are unchanged. In the evaporator system, the superheater has been eliminated.
 The compressor system consists only of a single compression stage and intercooling is no longer required.
 
 Following the tutorial, the parametrization for the heat pump models provided in this package has been done to match the power requirement
 calculated by the model to that given in the manufacturer's datasheets for a range of heat loads:
@@ -211,20 +211,33 @@
 
 
 
 
 Changelog
 =========
 
+0.2.0 - 2023-07-23
+------------------
+
+- [NEW] Example scenarios
+- [NEW] Model for cooling
+- [NEW] Different control strategies for controller
+- [NEW] Option to use same time loops with controller
+- [NEW] More precalculated heat pump models
+- [NEW] hplib mode
+- [NEW] Scripts to add new heat pump models
+- [CHANGE] Updated parameterization of detailed heat pump model
+- [CHANGE] Removed asynchronous connections
+- [CHANGE] Cleaned up code
+
 0.1.0 - 2021-06-29
 ------------------
 
 - Initial release of the mosaik-heatpump package
 
 
 Authors
 =======
 
 The mosaik-heatpump package was developed by Pranay Kasturi
 
 Additional Contributors: Jan Soeren Schwarz
-
```

### Comparing `mosaik-heatpump-0.1.0/README.rst` & `mosaik-heatpump-0.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 between 30 to 55 (deg. C). For the water source heat pump, the heat source temperature can vary between 4 to 20 (deg. C). and the condenser 
 inlet temperature can vary between 20 to 55 (deg. C). 
 
 Advanced Details of the Model
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The heat pump model available in TESPy's library was modified and the new schematic of the system is shown below.
 
-.. image:: images/system_schematic.png
+.. image:: docs/images/system_schematic.png
    :width: 600
 
 The consumer system and the expansion valve are unchanged. In the evaporator system, the superheater has been eliminated.
 The compressor system consists only of a single compression stage and intercooling is no longer required.
 
 Following the tutorial, the parametrization for the heat pump models provided in this package has been done to match the power requirement
 calculated by the model to that given in the manufacturer's datasheets for a range of heat loads:
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/Heat_Pump_Model.py` & `mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/Heat_Pump_Model.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,44 +19,48 @@
         """Power consumption of the heat pump in W"""
         self.COP = 0
         """COP of the heat pump"""
         self.Q_Demand = 0
         """The heat demand of the consumer in W"""
         self.Q_Supplied = 0
         """The heat supplied to the consumer in W"""
+        self.Q_evap = 0
+        """The heat removed in the evaporator in W"""
         self.cons_T = 0
         """The temperature at which heat is supplied to the consumer (in °C)"""
         self.cond_in_T = 0
         """The temperature at which the water reenters the condenser (in °C)"""
         self.heat_source = 0
         """The source of heat for the heat pump ('water' or 'air')"""
         self.heat_source_T = 0
         """The temperature of the heat source (in °C)"""
-        self.cond_m_in = 0
-        """The mass flow rate on the condenser side inlet of the heat pump (in kg/s)"""
-        self.cond_m_out = 0
-        """The mass flow rate on the condenser side outlet of the heat pump (in kg/s)"""
+        self.T_amb = 0
+        """The ambient temperature (in °C)"""
+        self.cond_m = 0
+        """The mass flow rate of water in the condenser of the heat pump (in kg/s)"""
+        self.cond_m_neg = 0
+        self.step_executed = False
 
 
 class Heat_Pump_Inputs():
     """Inputs variables to the heat pump for each time step"""
-    __slots__ = ['Q_Demand', 'heat_source', 'heat_source_T', 'cons_T', 'step_size', 'cond_in_T']
+    __slots__ = ['Q_Demand', 'heat_source', 'heat_source_T', 'cons_T', 'step_size', 'cond_in_T', 'T_amb']
 
     def __init__(self, params):
         self.Q_Demand = params.get('Q_Demand')
         """The heat demand of the consumer in W"""
 
         self.heat_source = params.get('heat_source')
         """The source of heat ('water' or 'air')"""
 
         self.heat_source_T = params.get('heat_source_T')
         """The temperature of the heat source (in °C)"""
 
-        # self.cons_T = params.get('cons_T')
-        # """The temperature at which heat is supplied to the consumer (in °C)"""
+        self.T_amb = params.get('T_amb')
+        """The ambient temperature (in °C)"""
 
         self.cond_in_T = params.get('cond_in_T')
         """The temperature at which the water reenters the condenser (in °C)"""
 
         self.step_size = None
         """step size in seconds"""
 
@@ -67,23 +71,26 @@
 
     You have to provide the *params* dictionary that contains the parameters
     required for the design of the heat pump. It will look like this::
 
         {
             'cons_T': 35,
             'heat_source_T': 12,
+            'T_amb': 12,
             'heat_source': 'water' or 'air'
         }
 
     -*cons_T* is the temperature, in °C, at which heat is supplied to the consumer. This can
     be changed later in the simulation as well.
 
     -*heat_source_T* is the temperature, in °C, at which the ambient fluid (water or air)
     is available as the heat source.
 
+    -*T_amb* is the ambient temperature, in °C.
+
     -*heat_source* is the fluid, either 'water' or 'air', that acts as the heat source for
     the system.
     """
 
     __slots__ = ['design', 'state', 'inputs']
 
     def __init__(self, params, COP_m_data):
@@ -105,28 +112,35 @@
         is calculated based on the consumer heat demand and the ambient
         fluid temperature.
 
         """
 
         step_inputs = {'heat_source_T': self.inputs.heat_source_T,
                        'Q_Demand': self.inputs.Q_Demand,
-                       # 'cons_T': self.inputs.cons_T,
-                       'cond_in_T': self.inputs.cond_in_T
+                       'cond_in_T': self.inputs.cond_in_T,
+                       'T_amb': self.inputs.T_amb
                        }
 
         if self.inputs.Q_Demand is not None:
             self.state.Q_Demand = self.inputs.Q_Demand
 
         if self.inputs.heat_source_T is not None:
             self.state.heat_source_T = self.inputs.heat_source_T
 
+        if self.inputs.T_amb is not None:
+            self.state.T_amb = self.inputs.T_amb
+
         if self.inputs.cond_in_T is not None:
             self.state.cond_in_T = self.inputs.cond_in_T
 
         self.design.Heat_Pump.step(step_inputs)
 
         self.state.P_Required = self.design.Heat_Pump.P_cons
         self.state.COP = self.design.Heat_Pump.COP
         self.state.Q_Supplied = self.design.Heat_Pump.Q_Supplied
-        self.state.cond_m_out = self.design.Heat_Pump.cond_m
-        self.state.cond_m_in = - self.design.Heat_Pump.cond_m
+        self.state.Q_evap = self.design.Heat_Pump.Q_evap
+        self.state.on_fraction = self.design.Heat_Pump.on_fraction
+        self.state.cond_m = self.design.Heat_Pump.cond_m
+        self.state.cond_m_neg = - self.design.Heat_Pump.cond_m
         self.state.cons_T = self.design.Heat_Pump.cons_T
+        self.state.step_executed = True
+
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump/heatpump/Heat_Pump_mosaik.py` & `mosaik-heatpump-0.2.0/mosaik_heatpump/heatpump/Heat_Pump_mosaik.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,67 +7,77 @@
 META = {
     'type': 'time-based',
     'models': {
         'HeatPump': {
             'public': True,
             'params': ['params'],
             'attrs': ['Q_Demand', 'Q_Supplied', 'heat_source_T', 'heat_source', 'cons_T', 'P_Required', 'COP',
-                      'cond_m_in', 'cond_m_out', 'cond_in_T'],
+                      'cond_m', 'cond_in_T', 'T_amb', 'on_fraction', 'cond_m_neg', 'Q_evap', 'step_executed'],
         },
     },
 }
 
-JSON_COP_DATA = os.path.abspath(os.path.join(os.path.dirname(__file__), 'COP_m_data.json'))
+JSON_COP_DATA = os.path.abspath(os.path.join(os.path.dirname(__file__), 'cop_m_data.json'))
 
 class HeatPumpSimulator(mosaik_api.Simulator):
     def __init__(self):
         super().__init__(META)
         self.time_resolution = None
         self.models = dict()  # contains the model instances
         self.sid = None
         self.eid_prefix = 'HeatPump_'
         self.step_size = None
+        self.time = 0
 
         self.parallelization = False
         self.processes = 1
         # start time of simulation as UTC ISO 8601 time string
 
-    def init(self, sid, time_resolution, step_size):
+    def init(self, sid, time_resolution, step_size, same_time_loop=False):
         self.time_resolution = float(time_resolution)
         if self.time_resolution != 1.0:
             print('WARNING: %s got a time_resolution other than 1.0, which \
                 can not be handled by this simulator.', sid)
         self.sid = sid # simulator id
         self.step_size = step_size
+        if same_time_loop:
+            self.meta['type'] = 'event-based'
+
         return self.meta
 
     def create(self, num, model, params):
         entities = []
 
         if 'processes' in params:
             self.parallelization = True
             self.processes = params['processes']
             if num < self.processes:
                 self.processes = num
 
         COP_m_data = None
-        if params['calc_mode'] == 'fast' or params['calc_mode'] == 'fixed':
+        if params['calc_mode'] == 'fast' or params['calc_mode'] == 'fixed_hl':
             with open(JSON_COP_DATA, "r") as read_file_1:
-                COP_m_data = json.load(read_file_1)
+                COP_m_data_all = json.load(read_file_1)
+                COP_m_data = COP_m_data_all[params['hp_model']]
 
         next_eid = len(self.models)
         for i in range(next_eid, next_eid + num):
             eid = '%s%d' % (self.eid_prefix, i)
             self.models[eid] = Heat_Pump(params, COP_m_data)
             entities.append({'eid': eid, 'type': model})
         return entities
 
     def step(self, time, inputs, max_advance):
         # print('heatpump inputs: %s' % inputs)
+        # print(f"Stepping HP at {time}")
         for eid, attrs in inputs.items():
+            if self.meta['type'] == 'event-based':
+                if time != self.time:
+                    self.time = time
+                    setattr(self.models[eid].state, 'step_executed', False)
             for attr, src_ids in attrs.items():
                 if len(src_ids) > 1:
                     raise ValueError('Two many inputs for attribute %s' % attr)
                 for val in src_ids.values():
                     setattr(self.models[eid].inputs, attr, val)
 
             self.models[eid].inputs.step_size = self.step_size
@@ -78,25 +88,33 @@
                 pool.apply_async(model.step(), args=())
             pool.close()
             pool.join()
         else:
             for eid, model in self.models.items():
                 model.step()
 
-        return time + self.step_size
+        if self.meta['type'] == 'event-based':
+            return None
+        else:
+            return time + self.step_size
 
     def get_data(self, outputs):
         data = {}
         for eid, attrs in outputs.items():
-            data[eid] = {}
-            for attr in attrs:
-                if attr not in self.meta['models']['HeatPump'][
-                        'attrs']:
-                    raise ValueError('Unknown output attribute: %s' % attr)
-                data[eid][attr] = float(getattr(self.models[eid].state, attr))
+            if self.models[eid].state.step_executed:
+                data[eid] = {}
+                for attr in attrs:
+                    if attr not in self.meta['models']['HeatPump'][
+                            'attrs']:
+                        raise ValueError('Unknown output attribute: %s' % attr)
+                    data['time'] = self.time
+                    if attr != 'step_executed':
+                        data[eid][attr] = float(getattr(self.models[eid].state, attr))
+                    else:
+                        data[eid][attr] = getattr(self.models[eid].state, attr)
         return data
 
 def main():
     return mosaik_api.start_simulation(HeatPumpSimulator())
 
 if __name__ == '__main__':
     main()
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/hotwatertank.py` & `mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/hotwatertank.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,21 +154,22 @@
 
         if 'diameter' in params:
             diameter = params['diameter']  # mm
         if 'volume' in params:
             diameter = (params['volume'] * 1e6 / (np.pi * self.height)) ** 0.5 * 2
 
         # only needed during initialization
-        self.surface_between_layers = np.pi * (diameter / 3e3) ** 2  # m2
+        self.surface_between_layers = np.pi * (diameter / 2e3) ** 2  # m2
 
         self.mass = np.pi * (diameter / 2e3) ** 2 * self.height
 
         # create layers
         self.layers = []
         if 'n_layers' in params:
+            n_layers = params['n_layers']
             if isinstance(init_vals['layers']['T'], list):
                 if len(init_vals['layers']['T']) == 2:  # temperature range
                     delta_T = init_vals['layers']['T'][1] - init_vals['layers']['T'][0]
                     T_init = [init_vals['layers']['T'][0] + i * delta_T / (params[
                                                                                'n_layers'] - 1) for i in range(params[
                                                                                                                    'n_layers'])]
                 else:
@@ -213,14 +214,17 @@
                 layer_params['diameter'] = diameter
                 # diameter of each layer is the same, therefore it is specified
                 # on the hotwater tank level
                 layer_params['bottom_top'] = bottom_top
                 layer_params['T'] = T_init[idx]
                 self.layers.append(Layer(layer_params))
 
+        # height of each layer, used in the calculation of heat transfer between layers
+        self.layer_height = self.height / n_layers / 1000
+
         # create connections
         self.connections = dict()
         if 'connections' in params:
             for key, connection_params in params['connections'].items():
                 self.connections[key] = Connection(connection_params,
                                                    self.layers)
                 # reference to layers is needed to have access to layers inside
@@ -323,45 +327,38 @@
                 layer.add_massflow(MassFlow(-netflow,
                                             self.layers[idx + 1].T))
                 self.layers[idx + 1].add_massflow(MassFlow(netflow,
                                                            self.layers[idx + 1].T))
 
         # calculate heatflow to environment
         for idx, layer in enumerate(self.layers):
-            # outer_surface = np.pi * layer.diameter / 1e3 * (layer.top
-            #        - layer.bottom) / 1e3
-            # if idx == 0 or idx == len(self.layers) - 1:
-            #    outer_surface += np.pi * (layer.diameter / 2e3)**2
+
             heatflow = ((self.T_env - layer.T) * layer.outer_surface *
                         self.htc_walls)
-            # print('heatflow_layer_%s: %s' % (idx, heatflow))
             layer.add_heatflow(heatflow)
 
         # calculate heatflow caused by heating rods
         for key, heating_rod in self.heating_rods.items():
             heating_rod.update()
             heating_rod.corresponding_layer.add_heatflow(heating_rod.P_th)
 
         # calculate heatflow between layers
         for layer, upper_layer in zip(self.layers[:-1], self.layers[1:]):
-            # boundary_surface = np.pi * (layer.diameter / 3e3)**2
             heatflow = ((layer.T - upper_layer.T)
-                        * self.surface_between_layers * self.htc_layers)
+                        * self.surface_between_layers * self.htc_layers) / self.layer_height
             upper_layer.add_heatflow(heatflow)
             layer.add_heatflow(-heatflow)
 
         # update temperature of layers
         for layer in self.layers:
             m = layer.volume * RHO
             delta_Q = 0
             for massflow in layer.massflows:
-                # print(massflow.T, massflow.F)
                 delta_Q += (massflow.F * step_size * RHO * (massflow.T + 273)
                             * C_W)
-            # print(layer.heatflows)
             for heatflow in layer.heatflows:
                 delta_Q += heatflow * step_size
             layer.T += delta_Q / (m * C_W)
             layer.empty_massflows()
             layer.empty_heatflows()
 
         # flip temperature if temperature of lower layer is higher
@@ -395,14 +392,19 @@
 
         if_type = getattr(self, self._nested_attrs[nested_attr]['type'])
         return getattr(if_type[name], attr)
 
     @property
     def snapshot(self):
         """serialize to json"""
+        return jsonpickle.encode(self)
+
+    @property
+    def snapshot_connections(self):
+        """serialize connections to json"""
         return jsonpickle.encode(self.connections)
 
     @property
     def T_layers(self):
         T_layers = []
         for layer in self.layers:
             T_layers.append(layer.T)
@@ -524,16 +526,14 @@
     temperatures of the connection or the temperature of the layers changes.
 
     """
 
     def __init__(self, params, layers):
         self.layers = layers  # reference to layers
         self.pos = params['pos']
-        if 'type' in params:
-            self.type = params['type']
         self._F = 0  # flow [l/s]
         self._T = None  # °C
         self._T_buffer = []  # °C
         self.corresponding_layer = None  # reference to corresponding layer
         for idx, layer in enumerate(self.layers):
             if layer.bottom <= self.pos < layer.top:
                 self.corresponding_layer_pos = layer
@@ -614,14 +614,15 @@
 
     """
 
     def __init__(self, params, layers, init_vals=None):
         self.pos = params['pos']
         self.T_max = params['T_max']
         self.P_th_stages = np.array(params['P_th_stages'])  # power stages in W
+        self.eta = params['eta'] # efficiency of the electric heater
         for idx, layer in enumerate(layers):
             if layer.bottom <= self.pos < layer.top:
                 self.corresponding_layer = layer
                 break
         # find corresponding layer
         self.P_th_set = None  # set value for thermal power output in W
         self.P_el = None  # electric power consumption in W
@@ -634,15 +635,15 @@
                     raise AttributeError("init_val %s doesn't match any attribute" % attr)
 
     def update(self):
         if self.corresponding_layer.T < self.T_max:
             idx = np.argmin(abs(self.P_th_stages - self.P_th_set))
             # find closest power stage
             self.P_th = self.P_th_stages[idx]
-            self.P_el = -self.P_th
+            self.P_el = -self.P_th/self.eta
         else:
             self.P_th = 0
             self.P_el = 0
 
     @property
     def P_th_min(self):
         return self.P_th_stages[0]
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump/hotwatertanksim/hotwatertank_mosaik.py` & `mosaik-heatpump-0.2.0/mosaik_heatpump/hotwatertanksim/hotwatertank_mosaik.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,34 +6,35 @@
 import jsonpickle
 from mosaik_heatpump.hotwatertanksim.hotwatertank import HotWaterTank
 
 class HotWaterTankSimulator(mosaik_api.Simulator):
     def __init__(self):
         # dummy metadata, actual metadata is set in init()
         meta = {
-                'type': 'time_based',
+                'type': 'time-based',
                 'models': {},
-                'extra_methods': ['add_async_request']
                 }
         super().__init__(meta)
         self.models = dict()
         self.sid = None
         self.eid_prefix = 'HotWaterTank_'
         self.step_size = None  # [sec]
         self.async_requests = dict()
-        self.i=0
+        self.time = None
+        self.first_iteration = None
+        self.step_executed = False
 
-    def init(self, sid, time_resolution, step_size, config):
+    def init(self, sid, time_resolution, step_size, config, same_time_loop=False):
         self.time_resolution = float(time_resolution)
         if self.time_resolution != 1.0:
             print('WARNING: %s got a time_resolution other than 1.0, which \
                 can not be handled by this simulator.', sid)
         self.sid = sid  # simulator id
         self.step_size = step_size
-        attrs = ['_', 'snapshot', 'sh_supply', 'sh_demand', 'dhw_demand', 'dhw_supply', 'hp_demand', 'T_env', 'T_mean', 'mass']
+        attrs = ['_', 'snapshot', 'snapshot_connections', 'T_env', 'T_mean', 'mass', 'step_executed']
         if 'n_sensors' in config:
             for i in range(config['n_sensors']):
                 attrs.append('sensor_%02d.T' % i)
         elif 'sensors' in config:
             for sensor in config['sensors']:
                 attrs.append('%s.T' % sensor)
 
@@ -49,80 +50,75 @@
                 attrs.append('%s.P_th_min' % heating_rod)
                 attrs.append('%s.P_th_max' % heating_rod)
         self.meta['models']['HotWaterTank'] = {
             'public': True,
             'params': ['params', 'init_vals', 'snapshot'],
             'attrs': attrs
         }
-            
+
+        if same_time_loop:
+            self.meta['type'] = 'event-based'
+
         return self.meta
     
     def create(self, num, model, params=None, init_vals=None, snapshot=None):
         entities = []
 
         next_eid = len(self.models)
         for i in range(next_eid, next_eid + num):
             eid = '%s%d' % (self.eid_prefix, i)
             if params is not None:
                 self.models[eid] = HotWaterTank(params, init_vals)
             else:
                 self.models[eid] = jsonpickle.decode(snapshot)
             entities.append({'eid': eid, 'type': model})
 
-        return entities 
-
-    def add_async_request(self, src_id, dest_id, *attr_pairs):
-        if not src_id in self.async_requests:
-            self.async_requests[src_id] = {dest_id: {}}
-        if not dest_id in self.async_requests[src_id]:
-            self.async_requests[src_id][dest_id] = {}
-        for attr_pair in attr_pairs:
-            src_attr, dest_attr = attr_pair
-            self.async_requests[src_id][dest_id].update({src_attr: dest_attr})
-        #print('async_reqs: %s' % self.async_requests)
-
+        return entities
 
     def step(self, time, inputs, max_advance):
 
-        # print('hwt inputs: %s' % inputs)
+        if self.meta['type'] == 'event-based':
+            if self.time != time:
+                self.first_iteration = True
+                self.step_executed = False
+            else:
+                self.first_iteration = False
+            self.time = time
         for eid, attrs in inputs.items():
             for attr, src_ids in attrs.items():
                 if attr == '_':
                     pass
                 else:
-                    for  src_id, val in src_ids.items():
+                    for src_id, val in src_ids.items():
                         set_nested_attr(self.models[eid], attr, val)
-
-        for eid, model in self.models.items():
-            model.step(self.step_size)
-
-        inputs = {}
-        # print('async_reqs: %s' % self.async_requests)
-        for src_id, dest_ids in self.async_requests.items():
-            eid = src_id.split('.')[1] 
-            inputs[src_id] = {}
-            for dest_id, src_attrs in dest_ids.items():
-                inputs[src_id][dest_id] = {}
-                for src_attr, dest_attr in src_attrs.items():
-                    inputs[src_id][dest_id][dest_attr] = get_nested_attr(
-                            self.models[eid], src_attr)
-
-        # print('hwt inputs: %s' % inputs)
-        yield self.mosaik.set_data(inputs)
-
-        return (time + self.step_size)
+        if self.meta['type'] == 'event-based':
+            if not self.first_iteration and not self.step_executed:
+                for eid, model in self.models.items():
+                    model.step(self.step_size)
+                    self.step_executed = True
+        else:
+            for eid, model in self.models.items():
+                model.step(self.step_size)
+
+        if self.meta['type'] == 'event-based':
+            if self.step_executed and (time + self.step_size) <= self.mosaik.world.until:  #
+                return (time + self.step_size)
+        else:
+            return (time + self.step_size)
 
     def get_data(self, outputs):
         data = {}
         for eid, attrs in outputs.items():
             data[eid] = {}
             for attr in attrs:
                 if attr not in self.meta['models']['HotWaterTank'][
                         'attrs']:
                     raise ValueError('Unknown output attribute: %s' % attr)
+                if self.meta['type'] == 'event-based':
+                    data['time'] = self.time
                 data[eid][attr] = get_nested_attr(self.models[eid], attr)
         return data
 
 def get_nested_attr(hwt, name):
     attr_parts = name.split('.')
     depth = len(attr_parts)
     if depth == 1:
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/PKG-INFO` & `mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mosaik-heatpump
-Version: 0.1.0
+Version: 0.2.0
 Summary: Mosaik-heatpump provides a model of a residential heatpump system
 Home-page: https://gitlab.com/mosaik/components/energy/mosaik-heatpump
 Author: Pranay Kasturi
 Author-email: mosaik@offis.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 mosaik-heatpump
@@ -107,15 +107,15 @@
 between 30 to 55 (deg. C). For the water source heat pump, the heat source temperature can vary between 4 to 20 (deg. C). and the condenser 
 inlet temperature can vary between 20 to 55 (deg. C). 
 
 Advanced Details of the Model
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The heat pump model available in TESPy's library was modified and the new schematic of the system is shown below.
 
-.. image:: images/system_schematic.png
+.. image:: docs/images/system_schematic.png
    :width: 600
 
 The consumer system and the expansion valve are unchanged. In the evaporator system, the superheater has been eliminated.
 The compressor system consists only of a single compression stage and intercooling is no longer required.
 
 Following the tutorial, the parametrization for the heat pump models provided in this package has been done to match the power requirement
 calculated by the model to that given in the manufacturer's datasheets for a range of heat loads:
@@ -211,20 +211,33 @@
 
 
 
 
 Changelog
 =========
 
+0.2.0 - 2023-07-23
+------------------
+
+- [NEW] Example scenarios
+- [NEW] Model for cooling
+- [NEW] Different control strategies for controller
+- [NEW] Option to use same time loops with controller
+- [NEW] More precalculated heat pump models
+- [NEW] hplib mode
+- [NEW] Scripts to add new heat pump models
+- [CHANGE] Updated parameterization of detailed heat pump model
+- [CHANGE] Removed asynchronous connections
+- [CHANGE] Cleaned up code
+
 0.1.0 - 2021-06-29
 ------------------
 
 - Initial release of the mosaik-heatpump package
 
 
 Authors
 =======
 
 The mosaik-heatpump package was developed by Pranay Kasturi
 
 Additional Contributors: Jan Soeren Schwarz
-
```

### Comparing `mosaik-heatpump-0.1.0/mosaik_heatpump.egg-info/SOURCES.txt` & `mosaik-heatpump-0.2.0/mosaik_heatpump.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 MANIFEST.in
 README.rst
 setup.py
 mosaik_heatpump/__init__.py
 mosaik_heatpump.egg-info/PKG-INFO
 mosaik_heatpump.egg-info/SOURCES.txt
 mosaik_heatpump.egg-info/dependency_links.txt
-mosaik_heatpump.egg-info/entry_points.txt
 mosaik_heatpump.egg-info/requires.txt
 mosaik_heatpump.egg-info/top_level.txt
 mosaik_heatpump/controller/__init__.py
 mosaik_heatpump/controller/controller.py
 mosaik_heatpump/controller/controller_mosaik.py
-mosaik_heatpump/heatpump/COP_m_data.json
 mosaik_heatpump/heatpump/Heat_Pump_Des.py
 mosaik_heatpump/heatpump/Heat_Pump_Model.py
 mosaik_heatpump/heatpump/Heat_Pump_mosaik.py
 mosaik_heatpump/heatpump/__init__.py
-mosaik_heatpump/heatpump/data_file.json
+mosaik_heatpump/heatpump/cop_m_data.json
+mosaik_heatpump/heatpump/eta_s_data.json
 mosaik_heatpump/hotwatertanksim/__init__.py
 mosaik_heatpump/hotwatertanksim/hotwatertank.py
 mosaik_heatpump/hotwatertanksim/hotwatertank_mosaik.py
```

### Comparing `mosaik-heatpump-0.1.0/setup.py` & `mosaik-heatpump-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from setuptools import setup, find_packages
-import os
 
 setup(
     name='mosaik-heatpump',
-    version='0.1.0',
+    version='0.2.0',
     author='Pranay Kasturi',
     author_email='mosaik@offis.de',
     description='Mosaik-heatpump provides a model of a residential heatpump system',
     long_description=(open('README.rst', encoding='utf-8').read() + '\n\n' +
                       open('CHANGES.txt', encoding='utf-8').read() + '\n\n' +
                       open('AUTHORS.txt', encoding='utf-8').read()),
     long_description_content_type='text/x-rst',
     url='https://gitlab.com/mosaik/components/energy/mosaik-heatpump',
     install_requires=[
         'mosaik-api>=3.0',
         'tespy>=0.4.2',
-        'jsonpickle'
+        'jsonpickle',
+        'hplib',
     ],
     packages=find_packages(exclude=['tests*']),
+    package_data={
+        "": ["*.json"]
+    },
     include_package_data=True,
     py_modules=['mosaik_heatpump'],
     entry_points={
         'console_scripts': [
         ],
     },
     classifiers=[
@@ -30,13 +33,15 @@
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
         'License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

