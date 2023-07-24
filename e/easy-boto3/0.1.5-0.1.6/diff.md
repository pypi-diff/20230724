# Comparing `tmp/easy_boto3-0.1.5.tar.gz` & `tmp/easy_boto3-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_boto3-0.1.5.tar", max compression
+gzip compressed data, was "easy_boto3-0.1.6.tar", max compression
```

## Comparing `easy_boto3-0.1.5.tar` & `easy_boto3-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/LICENSE
--rw-r--r--   0        0        0     8710 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/README.md
--rw-r--r--   0        0        0     1030 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/__init__.py
--rw-r--r--   0        0        0     1398 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/create.py
--rw-r--r--   0        0        0     1463 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/delete.py
--rw-r--r--   0        0        0      878 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/cloudwatch/list.py
--rw-r--r--   0        0        0     1015 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/__init__.py
--rw-r--r--   0        0        0     3439 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/config_parser.py
--rw-r--r--   0        0        0     3554 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/connect.py
--rw-r--r--   0        0        0     1724 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/create.py
--rw-r--r--   0        0        0     2586 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ec2_connections_management.py
--rw-r--r--   0        0        0     1494 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ec2_instance_management.py
--rw-r--r--   0        0        0     1741 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/list.py
--rw-r--r--   0        0        0     1487 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/logs.py
--rw-r--r--   0        0        0     3657 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/script.py
--rw-r--r--   0        0        0     2427 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/ssh.py
--rw-r--r--   0        0        0      689 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/start.py
--rw-r--r--   0        0        0      642 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/stop.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/stop_all.py
--rw-r--r--   0        0        0      892 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/ec2/terminate.py
--rw-r--r--   0        0        0    11965 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/main.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/__init__.py
--rw-r--r--   0        0        0     1141 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/active.py
--rw-r--r--   0        0        0     3311 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/ownership.py
--rw-r--r--   0        0        0     1477 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/profile/validation.py
--rw-r--r--   0        0        0      877 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/setup_session.py
--rw-r--r--   0        0        0        0 2023-07-22 21:11:16.948674 easy_boto3-0.1.5/easy_boto3/utilities/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/aws_profile_parser.py
--rw-r--r--   0        0        0     2471 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/decorators.py
--rw-r--r--   0        0        0     1270 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/easy_boto3/utilities/logger_maker.py
--rw-r--r--   0        0        0     1013 2023-07-22 21:11:16.952674 easy_boto3-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     9861 1970-01-01 00:00:00.000000 easy_boto3-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8710 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/README.md
+-rw-r--r--   0        0        0     1030 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/__init__.py
+-rw-r--r--   0        0        0     1398 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/create.py
+-rw-r--r--   0        0        0     1463 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/delete.py
+-rw-r--r--   0        0        0      878 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/cloudwatch/list.py
+-rw-r--r--   0        0        0     1015 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/__init__.py
+-rw-r--r--   0        0        0     3439 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/config_parser.py
+-rw-r--r--   0        0        0     3554 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/connect.py
+-rw-r--r--   0        0        0     1724 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/create.py
+-rw-r--r--   0        0        0     2586 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ec2_connections_management.py
+-rw-r--r--   0        0        0     1494 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ec2_instance_management.py
+-rw-r--r--   0        0        0     1741 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/list.py
+-rw-r--r--   0        0        0     1487 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/logs.py
+-rw-r--r--   0        0        0     3657 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/script.py
+-rw-r--r--   0        0        0     2967 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/ssh.py
+-rw-r--r--   0        0        0      781 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/start.py
+-rw-r--r--   0        0        0      827 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/stop.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/stop_all.py
+-rw-r--r--   0        0        0      998 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/ec2/terminate.py
+-rw-r--r--   0        0        0    13246 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/main.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/__init__.py
+-rw-r--r--   0        0        0     1141 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/active.py
+-rw-r--r--   0        0        0     3948 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/ownership.py
+-rw-r--r--   0        0        0     1477 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/profile/validation.py
+-rw-r--r--   0        0        0      877 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/setup_session.py
+-rw-r--r--   0        0        0        0 2023-07-24 20:46:58.811360 easy_boto3-0.1.6/easy_boto3/utilities/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/aws_profile_parser.py
+-rw-r--r--   0        0        0     2471 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/decorators.py
+-rw-r--r--   0        0        0     1270 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/easy_boto3/utilities/logger_maker.py
+-rw-r--r--   0        0        0     1013 2023-07-24 20:46:58.815361 easy_boto3-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9861 1970-01-01 00:00:00.000000 easy_boto3-0.1.6/PKG-INFO
```

### Comparing `easy_boto3-0.1.5/LICENSE` & `easy_boto3-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/README.md` & `easy_boto3-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/__init__.py` & `easy_boto3-0.1.6/easy_boto3/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/cloudwatch/create.py` & `easy_boto3-0.1.6/easy_boto3/cloudwatch/create.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/cloudwatch/delete.py` & `easy_boto3-0.1.6/easy_boto3/cloudwatch/delete.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/cloudwatch/list.py` & `easy_boto3-0.1.6/easy_boto3/cloudwatch/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/__init__.py` & `easy_boto3-0.1.6/easy_boto3/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/config_parser.py` & `easy_boto3-0.1.6/easy_boto3/ec2/config_parser.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/connect.py` & `easy_boto3-0.1.6/easy_boto3/ec2/connect.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/create.py` & `easy_boto3-0.1.6/easy_boto3/ec2/create.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/ec2_connections_management.py` & `easy_boto3-0.1.6/easy_boto3/ec2/ec2_connections_management.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/ec2_instance_management.py` & `easy_boto3-0.1.6/easy_boto3/ec2/ec2_instance_management.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/list.py` & `easy_boto3-0.1.6/easy_boto3/ec2/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/logs.py` & `easy_boto3-0.1.6/easy_boto3/ec2/logs.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/script.py` & `easy_boto3-0.1.6/easy_boto3/ec2/script.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/ssh.py` & `easy_boto3-0.1.6/easy_boto3/ec2/ssh.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,40 @@
 
         # lookup match for host_name = instance_ip
         if host_data['hostname'] == instance_ip:
             return host_data
 
 
 @session_auth
+def lookup_by_host_data_by_host(host,
+                                session=None):
+    # get ssh config
+    config = create_config_object()
+
+    # lookup host_data config
+    host_data = config.host(host)
+
+    return host_data
+
+
+@session_auth
+def change_host_name_by_host(host,
+                             public_ip,
+                             session=None):
+    # get ssh config
+    config = create_config_object()
+
+    # reset hostname   
+    config.set(host, Hostname=public_ip)
+
+    # save config
+    config.save()
+
+
+@session_auth
 def delete_host_by_hostname(instance_ip,
                             session=None):
     # get ssh config
     config = create_config_object()
 
     # loop over hosts, find host with matching host_name = instance_ip
     host_to_remove = None
```

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/start.py` & `easy_boto3-0.1.6/easy_boto3/ec2/start.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     # Check if instance exists
     response = ec2_controller.describe_instances(InstanceIds=[instance_id])
 
     # start instance if it exists
     if len(response["Reservations"]) > 0:
         # Start instance
-        ec2_controller.start_instances(InstanceIds=[instance_id])
+        instances = ec2_controller.start_instances(InstanceIds=[instance_id])
 
-        message = f"Starting instance {instance_id}"
-        print(message)
+        # wait for the instance to be running
+        waiter = ec2_controller.get_waiter('instance_running')
+        waiter.wait(InstanceIds=[instance_id])
     else:
         message = f"Instance {instance_id} does not exist"
         print(message)
```

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/stop.py` & `easy_boto3-0.1.6/easy_boto3/ec2/stop.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,10 +9,15 @@
     ec2_controller = session.client('ec2')
 
     # check if instance is running
     response = ec2_controller.describe_instances(InstanceIds=[instance_id])
     if response['Reservations'][0]['Instances'][0]['State']['Name'] == 'running':
         # stop instance
         ec2_controller.stop_instances(InstanceIds=[instance_id])
-        print(f'instance {instance_id} stopped')
+
+        # Get the instance stopped waiter
+        stopped_waiter = ec2_controller.get_waiter('instance_stopped')
+        # Wait until the instance is stopped
+        stopped_waiter.wait(InstanceIds=[instance_id])
     else:
+        print('\n')
         print(f'instance {instance_id} already stopped')
```

### Comparing `easy_boto3-0.1.5/easy_boto3/ec2/terminate.py` & `easy_boto3-0.1.6/easy_boto3/ec2/terminate.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,12 +16,14 @@
     if len(response["Reservations"]) > 0:
         # Terminate instance
         ec2_controller.terminate_instances(InstanceIds=[instance_id])
 
         # Delete alarm if it exists
         delete_instance_alarm(instance_id)
 
-        message = f"Terminating instance {instance_id} along with any associated cpu alarms"
-        print(message)
+        # Get the instance stopped waiter
+        terminated_waiter = ec2_controller.get_waiter('instance_terminated')
+        # Wait until the instance is stopped
+        terminated_waiter.wait(InstanceIds=[instance_id])
     else:
         message = f"Instance {instance_id} does not exist"
         print(message)
```

### Comparing `easy_boto3-0.1.5/easy_boto3/main.py` & `easy_boto3-0.1.6/easy_boto3/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
+import time
 from easy_boto3.profile import ownership, validation, active
 from easy_boto3.ec2.config_parser import parse as ec2_config_parser
-from easy_boto3.ec2.ssh import add_host, delete_host_by_hostname, lookup_host_data_by_hostname, delete_host
+from easy_boto3.ec2.ssh import add_host, delete_host_by_hostname, lookup_host_data_by_hostname, delete_host, change_host_name_by_host
 from easy_boto3.ec2.create import create_instance
 from easy_boto3.ec2.stop import stop_instance
 from easy_boto3.ec2.terminate import terminate_instance
 from easy_boto3.ec2.start import start_instance
 from easy_boto3.ec2.list import list_all, list_running, list_stopped
 from easy_boto3.ec2.logs import check_cloud_init_logs, check_syslog
 from easy_boto3.cloudwatch.create import create_cpu_alarm
@@ -34,14 +35,16 @@
     def profile(self, sub_operation, **kwargs):
         if sub_operation == "add":
             return ownership.add_ownership_data(**kwargs)
         if sub_operation == "delete":
             return ownership.delete_ownership_data(**kwargs)
         if sub_operation == "change_state":
             return ownership.change_ownership_state(**kwargs)
+        if sub_operation == "change_ip":
+            return ownership.change_ownership_ip(**kwargs)
         if sub_operation == "validate":
             return validation.validate(**kwargs)
         if sub_operation == "list_all":
             return validation.list_all_profiles(**kwargs)
         if sub_operation == "set":
             return active.set_active_profile(**kwargs)
         if sub_operation == "list_active":
@@ -97,38 +100,63 @@
         if self.args[1] == "ec2":
             if self.args[2] == "create" and ".yaml" in self.args[3]:
                 config = self.args[3]
                 self.create_ec2_instance(config)
             elif self.args[2] == "stop":
                 instance_id = self.args[3]
 
+                # lookup public_ip associated with instance_id
+                instance_ip = get_public_ip(instance_id)
+
                 # stop instance
                 self.stop_ec2_instance(instance_id)
 
                 # adjust instance state in file
                 self.easy_boto3.profile("change_state", instance_id=instance_id, new_state="stopped")
 
+                # print updated instance_ip
+                print(f"Instance stopped - instance {instance_id} stopped with public_ip {instance_ip}")
+
             elif self.args[2] == "terminate":
                 instance_id = self.args[3]
 
+                # lookup public_ip associated with instance_id
+                instance_ip = get_public_ip(instance_id)
+
                 # terminate instance
                 self.terminate_ec2_instance(instance_id)
 
                 # delete profile entry
                 self.easy_boto3.profile("delete", instance_id=instance_id)
 
+                # print updated instance_ip
+                print(f"Instance terminated - instance {instance_id} terminated with public_ip {instance_ip}")
+
             elif self.args[2] == "start":
                 instance_id = self.args[3]
 
                 # start instance
                 self.start_ec2_instance(instance_id)
 
+                # lookup public_ip associated with instance_id
+                instance_ip = get_public_ip(instance_id)
+
+                # print updated instance_ip
+                print(f"Instance started - instance {instance_id} started with public_ip {instance_ip}")
+
                 # adjust instance state in file
                 self.easy_boto3.profile("change_state", instance_id=instance_id, new_state="running")
 
+                # adjust public_ip in pair file
+                self.easy_boto3.profile("change_ip", instance_id=instance_id, public_ip=instance_ip)
+
+                # change host name in ssh config
+                change_host_name_by_host(host=instance_id, 
+                                         public_ip=instance_ip)
+
             elif self.args[2] == "check_cloud_init_logs":
                 instance_id = self.args[3]
                 self.check_cloud_init_logs(instance_id)
             elif self.args[2] == "check_syslog":
                 instance_id = self.args[3]
                 self.check_syslog(instance_id)
         elif self.args[1] == 'alarm':
```

### Comparing `easy_boto3-0.1.5/easy_boto3/profile/active.py` & `easy_boto3-0.1.6/easy_boto3/profile/active.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/profile/ownership.py` & `easy_boto3-0.1.6/easy_boto3/profile/ownership.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,22 @@
     for entry in data:
         if entry["instance_id"] == instance_id:
             entry["state"] = new_state
             return data
     return None
 
 
+def change_entry_public_ip(data, instance_id, new_public_ip):
+    for entry in data:
+        if entry["instance_id"] == instance_id:
+            entry["public_ip"] = new_public_ip
+            return data
+    return None
+
+
 @session_auth
 def add_ownership_data(instance_id: str,
                        public_ip: str,
                        profile_name: str = 'default',
                        session=None) -> None:
     # read in profile data
     data = read_json_file()
@@ -104,14 +112,30 @@
     # save if new_data is not None
     if new_data is not None:
         save_json_file(new_data)
 
     return None
 
 
+@session_auth
+def change_ownership_ip(instance_id: str,
+                        public_ip: str,
+                        session=None) -> None:
+    # read in profile data
+    data = read_json_file()
+
+    # try to change entry state
+    new_data = change_entry_public_ip(data, instance_id, public_ip)
+
+    # save if new_data is not None
+    if new_data is not None:
+        save_json_file(new_data)
+
+    return None
+
 def list() -> list:
     # read in profile data
     data = read_json_file()
 
     # print all profile list
     if len(data) == 0:
         print('No profile / instsance ids')
```

### Comparing `easy_boto3-0.1.5/easy_boto3/profile/validation.py` & `easy_boto3-0.1.6/easy_boto3/profile/validation.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/setup_session.py` & `easy_boto3-0.1.6/easy_boto3/setup_session.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/utilities/aws_profile_parser.py` & `easy_boto3-0.1.6/easy_boto3/utilities/aws_profile_parser.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/utilities/decorators.py` & `easy_boto3-0.1.6/easy_boto3/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/easy_boto3/utilities/logger_maker.py` & `easy_boto3-0.1.6/easy_boto3/utilities/logger_maker.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.5/pyproject.toml` & `easy_boto3-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_boto3"
-version = "0.1.5"
+version = "0.1.6"
 description = "`easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file."
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/easy_boto3"
 packages = [{include = "easy_boto3"}]
 include = ["easy_boto3/.easy_boto3_internal.yaml"]
```

### Comparing `easy_boto3-0.1.5/PKG-INFO` & `easy_boto3-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-boto3
-Version: 0.1.5
+Version: 0.1.6
 Summary: `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 Home-page: https://github.com/jermwatt/easy_boto3
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

