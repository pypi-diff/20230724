# Comparing `tmp/aws_network_firewall-0.1.2.tar.gz` & `tmp/aws_network_firewall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.1.2.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.2.0.tar", max compression
```

## Comparing `aws_network_firewall-0.1.2.tar` & `aws_network_firewall-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11335 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-07-20 20:19:00.095717 aws_network_firewall-0.1.2/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0     1191 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      579 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     2730 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1962 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2002 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      320 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      353 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1638 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1178 2023-07-20 20:19:00.095717 aws_network_firewall-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-24 11:12:48.630299 aws_network_firewall-0.2.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0     1191 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      589 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     2730 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     1966 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      353 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1756 2023-07-24 11:12:47.722220 aws_network_firewall-0.2.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1178 2023-07-24 11:12:48.630299 aws_network_firewall-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.2.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.1.2/LICENSE.txt` & `aws_network_firewall-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/README.md` & `aws_network_firewall-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/account.py` & `aws_network_firewall-0.2.0/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.2.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.2.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/destination.py` & `aws_network_firewall-0.2.0/aws_network_firewall/destination.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class Destination:
     """
     Understands a destination
     """
 
     description: str
     protocol: str
-    port: int
+    port: Optional[int]
     endpoint: Optional[str]
     region: Optional[str]
     cidr: Optional[str]
 
     def resolve_region_cidr_ranges(self, ranges: CidrRanges) -> None:
         if self.region and not self.cidr:
             cidr = ranges.by_region(self.region)
```

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.2.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/rule.py` & `aws_network_firewall-0.2.0/aws_network_firewall/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.2.0/aws_network_firewall/schemas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
 
 
 def destination_resolver(entry: dict) -> Destination:
     return Destination(
         description=entry["Description"],
         protocol=entry["Protocol"],
-        port=entry["Port"],
+        port=entry.get("Port"),
         endpoint=entry.get("Endpoint"),
         region=entry.get("Region"),
         cidr=entry.get("Cidr"),
     )
 
 
 def rule_resolver(workload: str, entry: dict) -> Rule:
```

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.2.0/aws_network_firewall/schemas/environment.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -78,24 +78,24 @@
       Endpoint:
         type: string
       Cidr:
         type: string
       Region:
         type: string
       Protocol:
-        enum: [ "TCP", "TLS" ]
+        enum: [ "TCP", "TLS", "ICMP" ]
       Port:
         type: integer
     additionalProperties: False
     required:
       - Description
       - Protocol
-      - Port
     anyOf:
       - required: ["Endpoint", "Cidr"]
         not: { required: ["Region"] }
       - required: ["Endpoint", "Region"]
         not: { required: ["Cidr"] }
       - required: ["Cidr"]
         not: { required: ["Endpoint", "Region"] }
 #      - not: { required: ["Endpoint", "Region", "Cidr"] }
 #      - not: { required: ["Region", "Cidr"] }
+#      Port is not required when Protocol is ICMP
```

### Comparing `aws_network_firewall-0.1.2/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.2.0/aws_network_firewall/suricata/rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     destination: Host
     options: List[Option]
 
     def __post_init__(self):
         self.protocol = self.protocol.lower()
 
     @property
+    def direction(self) -> str:
+        return "<>" if self.protocol == "icmp" else "->"
+
+    @property
     def source(self) -> str:
         addresses = list(map(lambda host: host.address, self.sources))
         sources = ",".join(addresses)
         return f"[{sources}] any" if len(addresses) > 1 else f"{sources} any"
 
     def __str__(self) -> str:
         post_rule = ""
@@ -43,8 +47,8 @@
             flow = Option(name="flow", value="not_established")
             sid = Option(name="sid", value="XXX")
             rev = Option(name="rev", value="1")
             handshake_options = "; ".join(list(map(str, [message, flow, rev, sid])))
 
             post_rule = f"\n{self.action} tcp {self.source} <> {self.destination} ({handshake_options})"
 
-        return f"{self.action} {self.protocol} {self.source} -> {self.destination} ({options}){post_rule}"
+        return f"{self.action} {self.protocol} {self.source} {self.direction} {self.destination} ({options}){post_rule}"
```

### Comparing `aws_network_firewall-0.1.2/pyproject.toml` & `aws_network_firewall-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.1.2/PKG-INFO` & `aws_network_firewall-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

