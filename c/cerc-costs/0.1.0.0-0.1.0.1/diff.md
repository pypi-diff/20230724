# Comparing `tmp/cerc-costs-0.1.0.0.tar.gz` & `tmp/cerc-costs-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-costs-0.1.0.0.tar", last modified: Tue Jul 18 14:02:04 2023, max compression
+gzip compressed data, was "cerc-costs-0.1.0.1.tar", last modified: Mon Jul 24 16:40:49 2023, max compression
```

## Comparing `cerc-costs-0.1.0.0.tar` & `cerc-costs-0.1.0.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-18 14:02:04.398106 cerc-costs-0.1.0.0/
--rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-07-18 14:02:04.398106 cerc-costs-0.1.0.0/PKG-INFO
-drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-18 14:02:04.394106 cerc-costs-0.1.0.0/cerc_costs.egg-info/
--rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-07-18 14:02:04.000000 cerc-costs-0.1.0.0/cerc_costs.egg-info/PKG-INFO
--rw-r--r--   0 guille    (1000) guille    (1000)      488 2023-07-18 14:02:04.000000 cerc-costs-0.1.0.0/cerc_costs.egg-info/SOURCES.txt
--rw-r--r--   0 guille    (1000) guille    (1000)        1 2023-07-18 14:02:04.000000 cerc-costs-0.1.0.0/cerc_costs.egg-info/dependency_links.txt
--rw-r--r--   0 guille    (1000) guille    (1000)       43 2023-07-18 14:02:04.000000 cerc-costs-0.1.0.0/cerc_costs.egg-info/requires.txt
--rw-r--r--   0 guille    (1000) guille    (1000)        6 2023-07-18 14:02:04.000000 cerc-costs-0.1.0.0/cerc_costs.egg-info/top_level.txt
-drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-18 14:02:04.398106 cerc-costs-0.1.0.0/costs/
--rw-r--r--   0 guille    (1000) guille    (1000)      305 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/__init__.py
--rw-r--r--   0 guille    (1000) guille    (1000)      243 2023-07-14 20:27:56.000000 cerc-costs-0.1.0.0/costs/__main__.py
--rw-r--r--   0 guille    (1000) guille    (1000)    11507 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/capital_costs.py
--rw-r--r--   0 guille    (1000) guille    (1000)     4945 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/configuration.py
--rw-r--r--   0 guille    (1000) guille    (1000)      253 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/constants.py
--rw-r--r--   0 guille    (1000) guille    (1000)     5978 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/cost.py
--rw-r--r--   0 guille    (1000) guille    (1000)     1201 2023-07-18 13:13:20.000000 cerc-costs-0.1.0.0/costs/cost_base.py
--rw-r--r--   0 guille    (1000) guille    (1000)     1147 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/end_of_life_costs.py
--rw-r--r--   0 guille    (1000) guille    (1000)     2035 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/total_maintenance_costs.py
--rw-r--r--   0 guille    (1000) guille    (1000)     4163 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/total_operational_costs.py
--rw-r--r--   0 guille    (1000) guille    (1000)     1500 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/total_operational_incomes.py
--rw-r--r--   0 guille    (1000) guille    (1000)       52 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/costs/version.py
--rw-r--r--   0 guille    (1000) guille    (1000)      166 2023-07-18 14:00:08.000000 cerc-costs-0.1.0.0/pyproject.toml
--rw-r--r--   0 guille    (1000) guille    (1000)       31 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/requirements.txt
--rw-r--r--   0 guille    (1000) guille    (1000)       38 2023-07-18 14:02:04.398106 cerc-costs-0.1.0.0/setup.cfg
--rw-r--r--   0 guille    (1000) guille    (1000)     1018 2023-07-18 13:10:39.000000 cerc-costs-0.1.0.0/setup.py
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-24 16:40:49.922968 cerc-costs-0.1.0.1/
+-rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-07-24 16:40:49.922968 cerc-costs-0.1.0.1/PKG-INFO
+-rw-r--r--   0 guille    (1000) guille    (1000)      754 2023-07-20 15:46:39.000000 cerc-costs-0.1.0.1/README.md
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-24 16:40:49.922968 cerc-costs-0.1.0.1/cerc_costs.egg-info/
+-rw-r--r--   0 guille    (1000) guille    (1000)      386 2023-07-24 16:40:49.000000 cerc-costs-0.1.0.1/cerc_costs.egg-info/PKG-INFO
+-rw-r--r--   0 guille    (1000) guille    (1000)      517 2023-07-24 16:40:49.000000 cerc-costs-0.1.0.1/cerc_costs.egg-info/SOURCES.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)        1 2023-07-24 16:40:49.000000 cerc-costs-0.1.0.1/cerc_costs.egg-info/dependency_links.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)       43 2023-07-24 16:40:49.000000 cerc-costs-0.1.0.1/cerc_costs.egg-info/requires.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)        6 2023-07-24 16:40:49.000000 cerc-costs-0.1.0.1/cerc_costs.egg-info/top_level.txt
+drwxr-xr-x   0 guille    (1000) guille    (1000)        0 2023-07-24 16:40:49.922968 cerc-costs-0.1.0.1/costs/
+-rw-r--r--   0 guille    (1000) guille    (1000)      596 2023-07-20 15:41:31.000000 cerc-costs-0.1.0.1/costs/__init__.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      243 2023-07-20 15:41:31.000000 cerc-costs-0.1.0.1/costs/__main__.py
+-rw-r--r--   0 guille    (1000) guille    (1000)    11799 2023-07-24 15:27:56.000000 cerc-costs-0.1.0.1/costs/capital_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     5238 2023-07-20 15:41:31.000000 cerc-costs-0.1.0.1/costs/configuration.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      572 2023-07-20 15:41:31.000000 cerc-costs-0.1.0.1/costs/constants.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     6625 2023-07-24 15:39:52.000000 cerc-costs-0.1.0.1/costs/cost.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1443 2023-07-24 14:07:10.000000 cerc-costs-0.1.0.1/costs/cost_base.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1439 2023-07-24 15:29:01.000000 cerc-costs-0.1.0.1/costs/end_of_life_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     2434 2023-07-24 15:28:52.000000 cerc-costs-0.1.0.1/costs/peak_load.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     2327 2023-07-24 15:29:12.000000 cerc-costs-0.1.0.1/costs/total_maintenance_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     4651 2023-07-24 15:29:17.000000 cerc-costs-0.1.0.1/costs/total_operational_costs.py
+-rw-r--r--   0 guille    (1000) guille    (1000)     1792 2023-07-24 15:28:40.000000 cerc-costs-0.1.0.1/costs/total_operational_incomes.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      344 2023-07-24 16:40:17.000000 cerc-costs-0.1.0.1/costs/version.py
+-rw-r--r--   0 guille    (1000) guille    (1000)      166 2023-07-19 16:56:07.000000 cerc-costs-0.1.0.1/pyproject.toml
+-rw-r--r--   0 guille    (1000) guille    (1000)       31 2023-07-19 16:56:07.000000 cerc-costs-0.1.0.1/requirements.txt
+-rw-r--r--   0 guille    (1000) guille    (1000)       38 2023-07-24 16:40:49.922968 cerc-costs-0.1.0.1/setup.cfg
+-rw-r--r--   0 guille    (1000) guille    (1000)     1018 2023-07-19 16:56:07.000000 cerc-costs-0.1.0.1/setup.py
```

### Comparing `cerc-costs-0.1.0.0/costs/capital_costs.py` & `cerc-costs-0.1.0.1/costs/capital_costs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """
 Capital costs module
+SPDX - License - Identifier: LGPL - 3.0 - or -later
+Copyright © 2023 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
+Code contributor Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Code contributor Oriol Gavalda Torrellas oriol.gavalda@concordia.ca
 """
 import math
 
 import pandas as pd
 import numpy_financial as npf
 from hub.city_model_structure.building import Building
 import hub.helpers.constants as cte
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cerc-costs-0.1.0.0/costs/configuration.py` & `cerc-costs-0.1.0.1/costs/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """
 Configuration module
+SPDX - License - Identifier: LGPL - 3.0 - or -later
+Copyright © 2023 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
+Code contributor Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Code contributor Oriol Gavalda Torrellas oriol.gavalda@concordia.ca
 """
 from hub.catalog_factories.costs_catalog_factory import CostsCatalogFactory
 from hub.catalog_factories.catalog import Catalog
 
 
 class Configuration:
   """
@@ -218,8 +222,8 @@
     return self._fuel_type
 
   @property
   def dictionary(self):
     """
     Get hub function to cost function dictionary
     """
-    return self._dictionary
+    return self._dictionary
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cerc-costs-0.1.0.0/costs/cost.py` & `cerc-costs-0.1.0.1/costs/cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """
 Cost module
+SPDX - License - Identifier: LGPL - 3.0 - or -later
+Copyright © 2023 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
+Code contributor Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Code contributor Oriol Gavalda Torrellas oriol.gavalda@concordia.ca
 """
-import hub.helpers.dictionaries
 import pandas as pd
 import numpy_financial as npf
 from hub.city_model_structure.building import Building
+from hub.helpers.dictionaries import Dictionaries
 
 from costs.configuration import Configuration
 from costs import CapitalCosts, EndOfLifeCosts, TotalMaintenanceCosts, TotalOperationalCosts, TotalOperationalIncomes
 from costs.constants import CURRENT_STATUS
 
 
 class Cost:
@@ -26,15 +30,17 @@
                electricity_peak_index=0.05,
                electricity_price_index=0.05,
                gas_price_index=0.05,
                discount_rate=0.03,
                retrofitting_year_construction=2020,
                factories_handler='montreal_custom',
                retrofit_scenario=CURRENT_STATUS,
-               dictionary=hub.helpers.dictionaries.Dictionaries().hub_function_to_montreal_custom_costs_function):
+               dictionary=None):
+    if dictionary is None:
+      dictionary = Dictionaries().hub_function_to_montreal_custom_costs_function
     self._building = building
     fuel_type = 0
     if "gas" in building.energy_systems_archetype_name:
       fuel_type = 1
     self._configuration = Configuration(number_of_years,
                                         percentage_credit,
                                         interest_rate, credit_years,
@@ -88,14 +94,15 @@
     df_capital_costs_systems = (
         global_capital_costs['D3020_heat_generating_systems'] +
         global_capital_costs['D3030_cooling_generation_systems'] +
         global_capital_costs['D3080_other_hvac_ahu'] +
         global_capital_costs['D5020_lighting_and_branch_wiring'] +
         global_capital_costs['D301010_photovoltaic_system']
     )
+
     df_end_of_life_costs = global_end_of_life_costs['End_of_life_costs']
     df_operational_costs = (
         global_operational_costs['Fixed_costs_electricity_peak'] +
         global_operational_costs['Fixed_costs_electricity_monthly'] +
         global_operational_costs['Fixed_costs_electricity_peak'] +
         global_operational_costs['Fixed_costs_electricity_monthly'] +
         global_operational_costs['Variable_costs_electricity'] +
@@ -125,19 +132,33 @@
     results[f'Scenario {self._configuration.retrofit_scenario}'] = [
       life_cycle_costs_capital_skin,
       life_cycle_costs_capital_systems,
       life_cycle_costs_end_of_life_costs,
       life_cycle_operational_costs,
       life_cycle_maintenance_costs,
       life_cycle_operational_incomes,
-      life_cycle_capital_incomes
+      life_cycle_capital_incomes,
+      global_capital_costs,
+      global_capital_incomes,
+      global_end_of_life_costs,
+      global_operational_costs,
+      global_maintenance_costs,
+      global_operational_incomes
     ]
 
-    results.index = ['total_capital_costs_skin',
-                     'total_capital_costs_systems',
-                     'end_of_life_costs',
-                     'total_operational_costs',
-                     'total_maintenance_costs',
-                     'operational_incomes',
-                     'capital_incomes']
+    results.index = [
+      'total_capital_costs_skin',
+      'total_capital_costs_systems',
+      'end_of_life_costs',
+      'total_operational_costs',
+      'total_maintenance_costs',
+      'operational_incomes',
+      'capital_incomes',
+      'global_capital_costs',
+      'global_capital_incomes',
+      'global_end_of_life_costs',
+      'global_operational_costs',
+      'global_maintenance_costs',
+      'global_operational_incomes'
+    ]
 
     return results
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cerc-costs-0.1.0.0/costs/total_maintenance_costs.py` & `cerc-costs-0.1.0.1/costs/total_maintenance_costs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 """
 Total maintenance costs module
+SPDX - License - Identifier: LGPL - 3.0 - or -later
+Copyright © 2023 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
+Code contributor Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Code contributor Oriol Gavalda Torrellas oriol.gavalda@concordia.ca
 """
 import math
 import pandas as pd
 from hub.city_model_structure.building import Building
 import hub.helpers.constants as cte
 
 from costs.configuration import Configuration
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cerc-costs-0.1.0.0/costs/total_operational_costs.py` & `cerc-costs-0.1.0.1/costs/total_operational_costs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """
 Total operational costs module
+SPDX - License - Identifier: LGPL - 3.0 - or -later
+Copyright © 2023 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
+Code contributor Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
+Code contributor Oriol Gavalda Torrellas oriol.gavalda@concordia.ca
 """
 import math
 import pandas as pd
 
 from hub.city_model_structure.building import Building
 import hub.helpers.constants as cte
 
 from costs.configuration import Configuration
 from costs.cost_base import CostBase
+from costs.peak_load import PeakLoad
 
 
 class TotalOperationalCosts(CostBase):
   """
   End of life costs class
   """
   def __init__(self, building: Building, configuration: Configuration):
@@ -59,15 +64,17 @@
     electricity_distribution = 0
     total_electricity_consumption = (
         electricity_heating + electricity_cooling + electricity_lighting + domestic_hot_water_electricity +
         electricity_plug_loads + electricity_distribution
     )
 
     # todo: change when peak electricity demand is coded. Careful with factor residential
-    peak_electricity_demand = 100  # self._peak_electricity_demand
+    peak_electricity_load = PeakLoad(building).electricity_peak_load
+    peak_load_value = peak_electricity_load.max(axis=1)
+    peak_electricity_demand = peak_load_value[1]/1000  # self._peak_electricity_demand adapted to kW
     variable_electricity_cost_year_0 = total_electricity_consumption * archetype.operational_cost.fuels[0].variable[0]
     peak_electricity_cost_year_0 = peak_electricity_demand * archetype.operational_cost.fuels[0].fixed_power * 12
     monthly_electricity_cost_year_0 = archetype.operational_cost.fuels[0].fixed_monthly * 12 * factor_residential
 
     for year in range(1, self._configuration.number_of_years + 1):
       price_increase_electricity = math.pow(1 + self._configuration.electricity_price_index, year)
       price_increase_peak_electricity = math.pow(1 + self._configuration.electricity_peak_index, year)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cerc-costs-0.1.0.0/setup.py` & `cerc-costs-0.1.0.1/setup.py`

 * *Files identical despite different names*

