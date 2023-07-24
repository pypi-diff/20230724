# Comparing `tmp/nat_gateway_setup-0.11.0.tar.gz` & `tmp/nat_gateway_setup-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nat_gateway_setup-0.11.0.tar", max compression
+gzip compressed data, was "nat_gateway_setup-0.6.0.tar", max compression
```

## Comparing `nat_gateway_setup-0.11.0.tar` & `nat_gateway_setup-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/LICENSE.md
--rw-r--r--   0        0        0     4153 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/README.md
--rw-r--r--   0        0        0       37 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/__init__.py
--rw-r--r--   0        0        0     5552 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/dnsmasq.py
--rw-r--r--   0        0        0     5422 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/firewall.py
--rw-r--r--   0        0        0     3570 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/nat_gateway_setup.py
--rw-r--r--   0        0        0     3139 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/network_interface.py
--rw-r--r--   0        0        0     4991 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/nat_gateway_setup/utils.py
--rw-r--r--   0        0        0      599 2023-07-24 17:54:23.876121 nat_gateway_setup-0.11.0/pyproject.toml
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 nat_gateway_setup-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-22 20:00:19.123948 nat_gateway_setup-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     4153 2023-07-22 19:52:23.711090 nat_gateway_setup-0.6.0/README.md
+-rw-r--r--   0        0        0       37 2023-07-22 17:54:57.116672 nat_gateway_setup-0.6.0/nat_gateway_setup/__init__.py
+-rw-r--r--   0        0        0     5552 2023-07-22 19:25:33.784083 nat_gateway_setup-0.6.0/nat_gateway_setup/dnsmasq.py
+-rw-r--r--   0        0        0     5284 2023-07-22 19:25:33.784083 nat_gateway_setup-0.6.0/nat_gateway_setup/firewall.py
+-rw-r--r--   0        0        0     3345 2023-07-22 19:25:33.784083 nat_gateway_setup-0.6.0/nat_gateway_setup/nat_gateway_setup.py
+-rw-r--r--   0        0        0     3139 2023-07-22 19:47:47.927946 nat_gateway_setup-0.6.0/nat_gateway_setup/network_interface.py
+-rw-r--r--   0        0        0     4374 2023-07-22 19:35:58.445973 nat_gateway_setup-0.6.0/nat_gateway_setup/utils.py
+-rw-r--r--   0        0        0      598 2023-07-22 20:54:30.087419 nat_gateway_setup-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 nat_gateway_setup-0.6.0/PKG-INFO
```

### Comparing `nat_gateway_setup-0.11.0/LICENSE.md` & `nat_gateway_setup-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nat_gateway_setup-0.11.0/README.md` & `nat_gateway_setup-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nat_gateway_setup-0.11.0/nat_gateway_setup/dnsmasq.py` & `nat_gateway_setup-0.6.0/nat_gateway_setup/dnsmasq.py`

 * *Files identical despite different names*

### Comparing `nat_gateway_setup-0.11.0/nat_gateway_setup/firewall.py` & `nat_gateway_setup-0.6.0/nat_gateway_setup/firewall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 import subprocess
 from datetime import datetime
 from .utils import CustomException, get_linux_distribution
 import glob
 import shutil
 
-# TODO: Check state of firewall.... not really sure how to do this.
-#       Seems like dhcpd and dns is not working with a port on rhel8
-
 def configure_firewall(wlan_interface, lan_interface):
     """
     Configure the firewall to forward traffic from the wlan interface to the eth interface.
 
     :raise: CustomException if the firewall configuration fails
     """
     backup_folder = "/var/cache/nat-linux-gateway"
```

### Comparing `nat_gateway_setup-0.11.0/nat_gateway_setup/nat_gateway_setup.py` & `nat_gateway_setup-0.6.0/nat_gateway_setup/nat_gateway_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 from prompt_toolkit.validation import Validator, ValidationError
 import ipaddress
 from .utils import check_firewall_condition, get_dns_server, enable_ip_forwarding, get_ip_range, get_linux_distribution, get_required_dependencies, check_dependencies, install_missing_dependencies
 from .firewall import configure_firewall
 from .dnsmasq import configure_dnsmasq, check_dnsmasq_configs, restart_dnsmasq
 from .network_interface import configure_interface
 
-# TODO: Check previous configurations
-#       One of the issues is there a wireless connection profile that does not have a mac address assigned. This is
-#       dangerous for other systems.. so what we want to do is make, 
-
 class IPValidator(Validator):
     def validate(self, document):
         try:
             ipaddress.IPv4Address(document.text)
         except ValueError:
             raise ValidationError(message="Please enter a valid IP address", cursor_position=len(document.text))
```

### Comparing `nat_gateway_setup-0.11.0/nat_gateway_setup/network_interface.py` & `nat_gateway_setup-0.6.0/nat_gateway_setup/network_interface.py`

 * *Files identical despite different names*

### Comparing `nat_gateway_setup-0.11.0/nat_gateway_setup/utils.py` & `nat_gateway_setup-0.6.0/nat_gateway_setup/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 import os
 import subprocess
 import distro
 import ipaddress
 import re
 
-def supported_os():
-    return get_linux_distribution() in ['centos', 'redhat', 'rhel', 'ubuntu'] # Tested OS's
-
-def is_debian_based():
-    return get_linux_distribution() in ['centos', 'redhat', 'rhel'] # CHECK TO SEE IF IT IS A REDHAT CHILD OS
-
-def is_redhat_based():
-    return get_linux_distribution() in ['ubuntu', 'debian'] # CHECKS TO SEE IF IT IS A DEBIAN CHILD OS
-
-
 def check_firewall_condition():
     """
     Check and set the correct firewall conditions for redhat systems.
 
     :raise: CustomException if the configuration fails
     """
     try:
         # First check if we are on a redhat system
-        if supported_os():
+        if get_linux_distribution() in ['centos', 'redhat']:
             # Disable iptables
             try:
                 subprocess.check_call(['systemctl', 'stop', 'iptables'])
             except subprocess.CalledProcessError:
                 pass # This is ok to get an error here... we just want to make sure
             try:
                 subprocess.check_call(['systemctl', 'disable', 'iptables'])
@@ -61,19 +51,19 @@
 def enable_ip_forwarding():
     """
     Enable IP forwarding.
     
     :raise: CustomException if the configuration fails
     """
     try:
-        if is_redhat_based(): # CHECK TO SEE IF IT IS A REDHAT CHILD OS
+        if get_linux_distribution() in ['centos', 'redhat']:
             with open('/etc/sysctl.d/99-ipforward.conf', 'w') as f:
                 f.write('net.ipv4.ip_forward = 1\n')
             subprocess.check_call(['sysctl', '-p', '/etc/sysctl.d/99-ipforward.conf'])
-        elif is_debian_based(): # CHECKS TO SEE IF IT IS A DEBIAN CHILD OS
+        elif get_linux_distribution() in ['ubuntu', 'debian']:
             with open('/etc/sysctl.conf', 'a') as f:
                 f.write('\nnet.ipv4.ip_forward=1\n')
             subprocess.check_call(['sysctl', '-p'])
         else:
             raise CustomException("Unsupported Linux distribution for IP forwarding configuration.")
     except subprocess.CalledProcessError as e:
         raise CustomException(f"IP forwarding configuration failed with error: {str(e)}") from None
@@ -97,26 +87,22 @@
 
 
 class CustomException(Exception):
     pass
 
 DEPENDENCIES = {
     'ubuntu': {'firewall': 'ufw', 'dnsmasq': 'dnsmasq', 'network_manager': 'network-manager', 'systemd': 'systemd'},
-    'redhat': {'firewall': 'firewalld', 'dnsmasq': 'dnsmasq', 'network_manager': 'NetworkManager', 'systemd': 'systemd'},
-    'rhel': {'firewall': 'firewalld', 'dnsmasq': 'dnsmasq', 'network_manager': 'NetworkManager', 'systemd': 'systemd'},
-    'centos': {'firewall': 'firewalld', 'dnsmasq': 'dnsmasq', 'network_manager': 'NetworkManager', 'systemd': 'systemd'}
+    'redhat': {'firewall': 'firewalld', 'dnsmasq': 'dnsmasq', 'network_manager': 'NetworkManager', 'systemd': 'systemd'}
 }
 
-
 def get_required_dependencies(linux_distribution):
     return DEPENDENCIES.get(linux_distribution, {})
 
 def check_dependencies(dependencies):
-    return [dep for dep in dependencies.values() if not is_installed(dep)]
-
+    return [dep for dep in dependencies if not is_installed(dep)]
 
 def install_missing_dependencies(missing_dependencies):
     for dep in missing_dependencies:
         install_dependency(dep)
 
 def is_installed(dependency):
     try:
```

### Comparing `nat_gateway_setup-0.11.0/pyproject.toml` & `nat_gateway_setup-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nat_gateway_setup"
-version = "0.11.0"
+version = "0.6.0"
 description = "A utility to configure a Linux machine as a gateway for a private network."
 authors = ["Your Name <youremail@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0.1"
```

### Comparing `nat_gateway_setup-0.11.0/PKG-INFO` & `nat_gateway_setup-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nat-gateway-setup
-Version: 0.11.0
+Version: 0.6.0
 Summary: A utility to configure a Linux machine as a gateway for a private network.
 Author: Your Name
 Author-email: youremail@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

