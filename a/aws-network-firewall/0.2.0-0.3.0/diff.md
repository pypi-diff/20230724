# Comparing `tmp/aws_network_firewall-0.2.0.tar.gz` & `tmp/aws_network_firewall-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.2.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.3.0.tar", max compression
```

## Comparing `aws_network_firewall-0.2.0.tar` & `aws_network_firewall-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11335 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-07-24 11:12:48.630299 aws_network_firewall-0.2.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0     1191 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      589 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     2730 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1966 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      415 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      353 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1756 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1178 2023-07-24 11:12:48.630299 aws_network_firewall-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-24 11:53:19.590885 aws_network_firewall-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-24 11:53:19.590885 aws_network_firewall-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-24 11:53:20.638930 aws_network_firewall-0.3.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0     1191 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      589 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     3031 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     1994 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2113 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      353 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1756 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1178 2023-07-24 11:53:20.638930 aws_network_firewall-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.3.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.2.0/LICENSE.txt` & `aws_network_firewall-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/README.md` & `aws_network_firewall-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/account.py` & `aws_network_firewall-0.3.0/aws_network_firewall/account.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,7 +33,15 @@
         )
 
         return rule
 
     @property
     def rules(self) -> List[Rule]:
         return self.__rules
+
+    @property
+    def inspection_rules(self) -> List[Rule]:
+        return list(filter(lambda rule: rule.is_inspection_rule, self.rules))
+
+    @property
+    def egress_rules(self) -> List[Rule]:
+        return list(filter(lambda rule: rule.is_egress_rule, self.rules))
```

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.3.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/destination.py` & `aws_network_firewall-0.3.0/aws_network_firewall/destination.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.3.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/rule.py` & `aws_network_firewall-0.3.0/aws_network_firewall/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, ClassVar
 
 from aws_network_firewall.source import Source
 from aws_network_firewall.destination import Destination
 from aws_network_firewall.suricata import SuricataRule, SuricataHost, SuricataOption
 
 
 @dataclass
 class Rule:
     """
     Understands a rule
     """
 
     workload: str
     name: str
+    type: str
     description: str
     sources: List[Source]
     destinations: List[Destination]
 
+    INSPECTION: ClassVar[str] = "Inspection"
+    EGRESS: ClassVar[str] = "Egress"
+
+    @property
+    def is_inspection_rule(self) -> bool:
+        return self.type == self.INSPECTION
+
+    @property
+    def is_egress_rule(self) -> bool:
+        return self.type == self.EGRESS
+
     @property
     def __suricata_source(self) -> List[SuricataHost]:
         def convert_source(source: Source) -> Optional[SuricataHost]:
             return SuricataHost(address=source.cidr) if source.cidr else None
 
         return list(filter(None, map(convert_source, self.sources)))
```

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.3.0/aws_network_firewall/schemas/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         cidr=entry.get("Cidr"),
     )
 
 
 def rule_resolver(workload: str, entry: dict) -> Rule:
     return Rule(
         workload=workload,
+        type=entry["Type"],
         name=entry["Name"],
         description=entry["Description"],
         sources=list(map(source_resolver, entry["Sources"])),
         destinations=list(map(destination_resolver, entry["Destinations"])),
     )
```

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.3.0/aws_network_firewall/schemas/environment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,30 @@
 
 $defs:
   Rule:
     type: object
     properties:
       Name:
         type: string
+      Type:
+        enum: [ "Egress", "Inspection" ]
       Description:
         type: string
       Sources:
         type: array
         items:
           $ref: "#/$defs/Source"
       Destinations:
         type: array
         items:
           $ref: "#/$defs/Destination"
     additionalProperties: False
     required:
       - Name
+      - Type
       - Description
       - Sources
       - Destinations
 
   Source:
     type: object
     properties:
```

### Comparing `aws_network_firewall-0.2.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.3.0/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.2.0/pyproject.toml` & `aws_network_firewall-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.2.0/PKG-INFO` & `aws_network_firewall-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

