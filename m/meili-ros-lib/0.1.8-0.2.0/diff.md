# Comparing `tmp/meili_ros_lib-0.1.8.tar.gz` & `tmp/meili_ros_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili_ros_lib-0.1.8.tar", last modified: Tue Jun 13 12:36:55 2023, max compression
+gzip compressed data, was "meili_ros_lib-0.2.0.tar", last modified: Mon Jul 24 12:41:25 2023, max compression
```

## Comparing `meili_ros_lib-0.1.8.tar` & `meili_ros_lib-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 12:36:55.097264 meili_ros_lib-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/meili_ros_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21298 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/agent_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/config_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/docking.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/maths.py
--rw-rw-rw-   0 root         (0) root         (0)    11990 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/offline.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9864 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/sdk_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-13 12:36:55.097264 meili_ros_lib-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.972608 meili_ros_lib-0.2.0/meili_ros_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22757 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/agent_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/config_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/docking.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/maths.py
+-rw-rw-rw-   0 root         (0) root         (0)    11990 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12925 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/sdk_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/meili_ros_lib/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 12:41:25.000000 meili_ros_lib-0.2.0/meili_ros_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-24 12:41:25.973608 meili_ros_lib-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-24 12:41:16.000000 meili_ros_lib-0.2.0/setup.py
```

### Comparing `meili_ros_lib-0.1.8/LICENSE.txt` & `meili_ros_lib-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/agent.py` & `meili_ros_lib-0.2.0/meili_ros_lib/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import math
 import sys
+import time
 import datetime
 import threading
-from math import sqrt
+from math import sqrt, dist
 
 from meili_sdk.websockets.models.message import Message
 from meili_sdk.websockets import constants
 
 from geometry_msgs.msg import PoseWithCovarianceStamped, Pose, Twist
 from sensor_msgs.msg import NavSatFix
 from nav_msgs.msg import Odometry
@@ -14,14 +14,15 @@
 from meili_ros_lib.config_agent import ConfigAgent
 from meili_ros_lib.maths import quaternion_to_euler
 from meili_ros_lib.parse_data import parse_battery_data
 from meili_ros_lib.sentry import initialize_sentry, agent_sentry
 
 from sentry_sdk import capture_exception, capture_message
 
+
 initialize_sentry()
 
 
 def update_capacity_lipo(voltage):
     # Calculate current capacity of lipo batteries taking into account voltage/capacity estimation using regression
     capacity = 47.6 * voltage - 500
     return capacity
@@ -141,15 +142,14 @@
 
             self.task_started.append(0)
             self.waypoints.append(False)
             self.waypoints_goal_id.append(None)
             self.goal_id_rerouted.append(None)
             self.pause_paths[i] = False
 
-
             self.max_vel_x.append(0)
             self.max_vel_theta.append(0)
             self.goal_id.append(0)
 
     ################################################
     def check_topic_streaming_mode(self):
         """Check Topic Streaming"""
@@ -185,15 +185,15 @@
             self.ping_gps()
         else:
             self.ping_location()
 
         if self.node.battery_present:
             self.ping_battery()
 
-        if self.node.traffic_control:
+        if self.node.traffic_control and not self.node.v2:
             self.ping_trajectory()
 
     def ping_location(self):
         """Ping Location """
         try:
             for index, msg in enumerate(self.msg_pose):
                 if isinstance(msg, PoseWithCovarianceStamped):
@@ -213,29 +213,30 @@
 
                 yaw = round(quaternion_to_euler(
                     orientation.x, orientation.y, orientation.z, orientation.w
                 ),
                     3)
                 self.send_message_client(
                     constants.EVENT_LOCATION,
-                    {"xm": x, "ym": y, "rotation": yaw},
+                    {"timestamp": time.time(), "xm": x, "ym": y, "rotation": yaw},
                     self.vehicle_list[index],
                 )
 
         except Exception as error:
             self.log_info(f"[ROSAgent] Ping location error: {error}")
             capture_exception(error)
 
     def ping_battery(self):
         """Sending Battery message via websocket"""
         try:
             for index, msg in enumerate(self.msg_battery):
                 if self.node.lipo_battery:
                     msg.capacity = update_capacity_lipo(msg.voltage)
                 battery_data = parse_battery_data(msg)
+                battery_data["timestamp"] = time.time()
                 self.send_message_client(
                     constants.EVENT_BATTERY,
                     {**battery_data},
                     self.vehicle_list[index],
                 )
         except Exception as error:
             capture_exception(error)
@@ -248,19 +249,19 @@
             for index, msg in enumerate(self.arr_plan):
                 if self.task_started[index] and not self.pause_paths[index]:
                     now = datetime.datetime.now()
                     current_time = now.strftime("%H:%M:%S")
                     # self.log_info(f"[ROSAgent] Sending path of vehicle {self.vehicle_names[index]}: {current_time}")
                     start = msg[0]
                     end = msg[-1]
-                    dist = math.dist(start, end)
-                    #self.log_info(f"{start}-- {end} ={dist} vehicle {self.vehicle_list[index]}")
+                    dist = dist(start, end)
+                    # self.log_info(f"{start}-- {end} ={dist} vehicle {self.vehicle_list[index]}")
                     self.send_message_client(
                         constants.EVENT_PATH_DATA,
-                        {"path": msg},
+                        {"timestamp": time.time(), "path": msg},
                         self.vehicle_list[index],
                     )
         except Exception as error:
             self.log_info(
                 f"[ROSAgent] Ping Trajectory Error: {error} "
             )
             self.log_info(f"{index} {self.arr_plan}")
@@ -272,28 +273,28 @@
             for index, msg in enumerate(self.msg_gps):
                 if isinstance(msg, NavSatFix):
                     lat = msg.latitude
                     lon = msg.longitude
                     rotation = 0
                     self.send_message_client(
                         constants.EVENT_LOCATION,
-                        {"lat": lat, "lon": lon, "rotation": rotation},
+                        {"timestamp": time.time(), "lat": lat, "lon": lon, "rotation": rotation},
                         self.vehicle_list[index],
                     )
         except Exception as e:
             self.log_info(
                 "[ROSAgent] Ping GPS Error: %s ", e)
             capture_exception(e)
 
     def ping_docking_routine(self, vehicle, path, rotation_angles):
         # send the trajectory as an array of poses
         try:
             self.send_message_client(
                 constants.EVENT_DOCKING_ROUTINE,
-                {"path": path, "rotation_angles": rotation_angles},
+                {"timestamp": time.time(), "path": path, "rotation_angles": rotation_angles},
                 vehicle,
             )
             self.log_info("[ROSAgent] Docking Routine Sent")
         except Exception as e:
             self.log_info(f"[ROSAgent] Ping Docking Routine Error: {e} ")
             capture_exception(e)
 
@@ -302,21 +303,21 @@
         try:
             for index, msg in enumerate(self.msg_speed):
                 if isinstance(msg, Odometry):
                     speed = msg.twist.twist.linear.x
                     speed = round(speed, 3)
                     self.send_message_client(
                         constants.EVENT_SPEED,
-                        {"speed": speed},
+                        {"timestamp": time.time(), "speed": speed},
                         self.vehicle_list[index]
                     )
 
                 else:
-                    # self.log_info(f"[ROSAgent] Robot {self.vehicle_names[index]} speed is not available")
-                    # capture_message("[ROSAgent] Robot speed is not available")
+                    #self.log_info(f"[ROSAgent] Robot {self.vehicle_names[index]} speed is not available")
+                    #capture_message("[ROSAgent] Robot speed is not available")
                     break
 
         except Exception as e:
             self.log_info(f"[ROSAgent] Ping speed Error: {e} ")
             capture_exception(e)
 
     ################################################
@@ -339,15 +340,15 @@
         if self.node.battery_present:
             vehicle_position = self.return_vehicle_position(vehicle_uuid)
             self.msg_battery[vehicle_position] = msg
 
             if self.node.topic_streaming_mode == "REALTIME" and self.ws_open:
                 self.ping_battery()
 
-    def callback_rosoutagg(self, msg, type_msg, time_stamp):
+    def callback_rosoutagg(self, msg, type_msg):
         rosout_message = msg.msg
 
         count = 0
         # Find the vehicle uuid that corresponds to the message.
         if rosout_message.find('vehicle') != -1:
             for vehicle_uuid in self.vehicle_list:
                 if (rosout_message.find(vehicle_uuid)) != -1:
@@ -385,23 +386,36 @@
 
             self.goal_id[vehicle_position] = goal_id
             self.send_message_client(
                 constants.EVENT_GOAL_STATUS,
                 {"goal_id": goal_id, "status_id": status_id},
                 vehicle_uuid,
             )
-            self.log_info(
-                f"[ROSAgent] Sending {goal_id} in progress<<{status_id}>> of vehicle {vehicle_position} ")
+            #self.log_info(
+            #    f"[ROSAgent] Sending {goal_id} in progress<<{status_id}>> of vehicle {vehicle_position} ")
 
         else:
             now = datetime.datetime.now()
             dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
             self.start_time = dt_string
         return 1
 
+    def action_in_progress(self, goal_id, status_id, vehicle_uuid):
+        if self.ws_open:
+            vehicle_position = self.return_vehicle_position(vehicle_uuid)
+            self.goal_id[vehicle_position] = goal_id
+            self.send_message_client(
+                constants.EVENT_GOAL_STATUS,
+                {"goal_id": goal_id, "status_id": status_id},
+                vehicle_uuid,
+            )
+            self.log_info(
+                f"[ROSAgent] Sending action {goal_id} in progress<<{status_id}>> of vehicle {vehicle_position} ")
+        return 1
+
     def callback_status(self, msg, goal_id, status_id, vehicle_uuid):
         # Status of navigation task is parsed and send to FMS task_msg_server
         vehicle_position = self.return_vehicle_position(vehicle_uuid)
 
         if (
                 self.waypoints_goal_id[vehicle_position] is None
                 and self.waypoints[vehicle_position]
@@ -448,16 +462,16 @@
 
         return 0
 
     def task_finished(self, goal_id, status_id, vehicle_uuid):
         vehicle_position = self.return_vehicle_position(vehicle_uuid)
         # TASK ONLINE
         if self.ws_open:
-            self.log_info(
-                f"[ROSAgent] Task {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
+           # self.log_info(
+           #     f"[ROSAgent] Task {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
             if not self.waypoints[vehicle_position]:
 
                 if self.waypoints_goal_id[vehicle_position] is not None:
                     goal_id = self.waypoints_goal_id[vehicle_position]
                     self.waypoints_goal_id[vehicle_position] = None
                     if self.goal_id_rerouted[vehicle_position] is not None:
                         goal_id = self.goal_id_rerouted[vehicle_position]
@@ -466,17 +480,16 @@
                 self.goal_id[vehicle_position] = goal_id
                 self.send_message_client(
                     constants.EVENT_GOAL_STATUS,
                     {"goal_id": goal_id, "status_id": status_id},
                     vehicle_uuid,
                 )
 
-                self.log_info(
-                    f"[ROSAgent] Sending {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
-
+              #  self.log_info(
+              #      f"[ROSAgent] Sending {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
 
         # OFFLINE TASK
         if self.connection.offline_agent.offline:
             success = True
 
             for task in self.connection.offline_agent.offline_tasks:
                 if self.connection.offline_agent.current_task_uuid == task[0]:
@@ -489,22 +502,38 @@
                             self.start_time,
                             success=success,
                         )
                         self.start_time = None
                         self.connection.offline_agent.task_offline_started = False
         return 0
 
+    def action_finished(self, goal_id, status_id, vehicle_uuid):
+        # TASK ONLINE
+        if self.ws_open:
+            vehicle_position = self.return_vehicle_position(vehicle_uuid)
+            self.log_info(
+                f"[ROSAgent] Task {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
+            self.goal_id[vehicle_position] = goal_id
+            self.send_message_client(
+                constants.EVENT_GOAL_STATUS,
+                {"goal_id": goal_id, "status_id": status_id},
+                vehicle_uuid,
+            )
+
+            self.log_info(
+                f"[ROSAgent] Sending action {goal_id} finished<<{status_id}>> of vehicle {vehicle_position} ")
+
     def check_distance_of_array(self, msg):
         path = []
         first = None
         for pose in msg.poses:
             if first is None:
                 first = [pose.pose.position.x, pose.pose.position.y]
             point = [pose.pose.position.x, pose.pose.position.y]
-            distance = math.dist(first, point)
+            distance = dist(first, point)
             path.append(point)
             if distance > self.path_length:
                 yield path
         yield path
 
     def callback_plan(self, msg, vehicle_uuid):
         """Callback Plan"""
```

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/agent_setup.py` & `meili_ros_lib-0.2.0/meili_ros_lib/agent_setup.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/config_agent.py` & `meili_ros_lib-0.2.0/meili_ros_lib/config_agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/connection.py` & `meili_ros_lib-0.2.0/meili_ros_lib/connection.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/docking.py` & `meili_ros_lib-0.2.0/meili_ros_lib/docking.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/maths.py` & `meili_ros_lib-0.2.0/meili_ros_lib/maths.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/offline.py` & `meili_ros_lib-0.2.0/meili_ros_lib/offline.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/parse_data.py` & `meili_ros_lib-0.2.0/meili_ros_lib/parse_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,47 @@
         rotation = data["location"]["rotation"]
     except KeyError:
         rotation = 0
     rotation_quaternion = rotation_setup(rotation)
 
     return x_meters, y_meters, rotation_quaternion
 
+def goal_setup_v2(data):
+    """Set up the goal with rotation, x and y"""
+    x_meters = data["metric"]["x"]
+    y_meters = data["metric"]["y"]
+    try:
+        rotation = data["rotation"]
+    except KeyError:
+        rotation = 0
+    rotation_quaternion = rotation_setup(rotation)
+    return x_meters, y_meters, rotation_quaternion
+
 
 def parse_waypoints(data):
     pose = []
     rotation_angle = data["rotation_angles"]
     waypoints = data["metric_waypoints"]
 
     for index, waypoint in enumerate(waypoints):
         x = waypoint[0]
         y = waypoint[1]
         rotation = rotation_angle[index]
         pose.append([x, y, rotation])
 
     return pose
 
+def parse_waypoints_v2(waypoints, rotation_angles):
+    pose = []
+    for index, waypoint in enumerate(waypoints):
+        x = waypoint[0]
+        y = waypoint[1]
+        rotation = rotation_angles[index]
+        pose.append([x, y, rotation])
+    return pose
 
 def parse_battery_data(msg):
     # creating dictionary for storing battery data
     battery_data = {}
 
     if hasattr(msg, "capacity"):
         battery_data["value"] = round(msg.capacity, 2)
```

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/sdk_handlers.py` & `meili_ros_lib-0.2.0/meili_ros_lib/sdk_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from meili_sdk.websockets.client import MeiliWebsocketClient
 from sentry_sdk import capture_exception, capture_message
-from meili_ros_lib.parse_data import parse_waypoints, parse_docking_routine
+from meili_ros_lib.parse_data import parse_waypoints, parse_waypoints_v2, parse_docking_routine
 from meili_ros_lib.sentry import agent_sentry
 
 from std_msgs.msg import Bool
 
 import time
 
 
@@ -26,94 +26,161 @@
             self.agent.client = MeiliWebsocketClient(
                 self.agent.token,
                 override_host=self.agent.server_instance.replace("http", "ws"),
                 fleet=self.agent.fleet,
                 open_handler=self.open_handler,
                 close_handler=self.close_handler,
                 error_handler=self.error_handler,
+                task_v2_handler=self.task_v2_handler,
                 task_handler=self.task_handler,
                 task_cancellation_handler=self.task_cancellation_handler,
                 move_action_handler=self.move_action_handler,
                 slow_down_handler=self.slow_down_handler,
                 topic_list_initializer_handler=self.topic_handler,
                 path_rerouting_handler=self.path_rerouting_handler,
                 docking_routine_request_handler=self.docking_routine_request_handler,
                 docking_routine_finalize_handler=self.docking_routine_finalize_handler,
                 collision_clearance_handler=self.collision_clearance_handler,
+                update_map_handler=self.update_map_handler,
             )
         except KeyError as error:
             self.agent.log_info(f"[ROSHandler] No handler named {error}")
             capture_exception(error)
         return self.agent.client
 
     def check_fleet_get_vehicle_position(self, vehicle):
         if self.agent.fleet:
             return self.agent.return_vehicle_position(vehicle)
         return 0
 
-    def move_action_handler(self, _, data: dict, vehicle: str):
+    def move_action_handler(self, move_msg, data: dict, vehicle: str):
         """When a task is received, goal is generated and sent to the specific robot"""
         try:
             vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
-            self.send_goal(data, vehicle_position)
+            # For v2 testing--> will deprecate it
+            if "metric_waypoints" in data["data"]["location"]:
+                data = data["data"]["location"]
+                pose = parse_waypoints(data)
+                current_task_uuid = "uuid"
+                self.waypoints_handler(
+                    vehicle_position=vehicle_position,
+                    pose=pose,
+                )
+            else:
+                self.send_goal(data, vehicle_position)
+
             self.rate.sleep()
 
             # If the robot is moving the task will be automatically cancelled to go to the
             # charging station.
             self.agent.log_info(
                 f"[ROSHandler] Sending vehicle {self.agent.vehicle_list[vehicle_position]}: "
-                f"{self.agent.vehicle_names[vehicle_position]} to CHARGING STATION"
+                f"{self.agent.vehicle_names[vehicle_position]} to RESTING/CHARGING STATION"
             )
 
         except Exception as error:
             self.agent.log_error(
                 "[ROSHandler] Error move_action_handler: %s" % (error,)
             )
             agent_sentry(error, "[ROSHandler] Error move_action_handler")
 
     def task_handler(self, _, data: dict, vehicle: str):
         """When a task is received, goal is generated and sent to the specific robot"""
-        try:
-            vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
-            current_task_uuid = data["uuid"]
-
-            self.agent.number_of_tasks = self.agent.number_of_tasks + 1
-
-            self.agent.log_info(
-                f"[ROSHandler] Number of received task is: {self.agent.number_of_tasks}"
-            )
-            self.agent.log_info(
-                f"[ROSHandler] Received task assigned to vehicle: {self.agent.vehicle_names[vehicle_position]}"
-            )
-            if not data["metric_waypoints"]:
-                # Case when only one task is sent
-                self.send_goal(data, vehicle_position)
-            else:
-                # This is batch-task vehicle
-                if self.agent.node.path_planning:
-                    pose = parse_waypoints(data)
-                    # self.agent.total_waypoints = len(x_meters)
-                    self.waypoints_handler(
-                        vehicle_position=vehicle_position,
-                        pose=pose,
-                        current_task_uuid=current_task_uuid,
-                    )
-                else:
+        if self.agent.node.v2:
+            return 0
+        else:
+            try:
+                vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
+                current_task_uuid = data["uuid"]
+
+                self.agent.number_of_tasks = self.agent.number_of_tasks + 1
+
+                self.agent.log_info(
+                    f"[ROSHandler] Number of received task is: {self.agent.number_of_tasks}"
+                )
+                self.agent.log_info(
+                    f"[ROSHandler] Received task assigned to vehicle: {self.agent.vehicle_names[vehicle_position]}"
+                )
+                if not data["metric_waypoints"]:
+                    # Case when only one task is sent
                     self.send_goal(data, vehicle_position)
+                else:
+                    # This is batch-task vehicle
+                    if self.agent.node.path_planning:
+                        pose = parse_waypoints(data)
+                        # self.agent.total_waypoints = len(x_meters)
+                        self.waypoints_handler(
+                            vehicle_position=vehicle_position,
+                            pose=pose,
+                        )
+                    else:
+                        self.send_goal(data, vehicle_position)
+
+                self.rate.sleep()
+
+            except KeyError as error:
+                self.agent.log_error(
+                    f"[ROSHandler] Error task_handler: {error}"
+                )
+                agent_sentry(error, "[ROSHandler] Error task_handler")
 
-            self.rate.sleep()
+    def task_v2_handler(self, task, vehicle_uuid: str):
+        """When a task is received, goal is generated and sent to the specific robot"""
+        if not self.agent.node.v2:
+            return 0
+        else:
+            try:
+                vehicle_position = self.check_fleet_get_vehicle_position(vehicle_uuid)
+                self.agent.number_of_tasks = self.agent.number_of_tasks + 1
+
+                self.agent.log_info(
+                    f"[ROSHandler] Number of received v2 task is: {self.agent.number_of_tasks}"
+                )
+                self.agent.log_info(
+                    f"[ROSHandler] Received v2 task assigned to vehicle: {self.agent.vehicle_names[vehicle_position]}"
+                )
+                self.action_handler(task, vehicle_uuid)
+                self.rate.sleep()
+
+            except KeyError as error:
+                self.agent.log_error(
+                    f"[ROSHandler] Error task v2_handler: {error}"
+                )
+                agent_sentry(error, "[ROSHandler] Error task_v2handler")
+    
+    def action_handler(self, task, vehicle_uuid):
+        vehicle_position = self.check_fleet_get_vehicle_position(vehicle_uuid)
+        action_type=task.action.action_type
+        point=task.action.point
+        form_values = task.action.values
+        metric_waypoints=task.metric_waypoints
+        rotation_angles= task.rotation_angles
+
+        if (action_type=="move_to_point" or action_type=="go_to_charge" or action_type=="follow_path"):
+            if metric_waypoints:
+                pose = parse_waypoints_v2(metric_waypoints, rotation_angles)
+                self.waypoints_handler(
+                    vehicle_position=vehicle_position,
+                    pose=pose,
+                )
+            else:
+                self.send_goal_v2(point, vehicle_position)
 
-        except KeyError as error:
-            self.agent.log_error(
-                f"[ROSHandler] Error task_handler: {error}"
-            )
-            agent_sentry(error, "[ROSHandler] Error task_handler")
+        #Handling actions TO BE COMPLETED BY USER FOR THE SPECIFICS ACTIONS
+        else:
+            goal_id=task.uuid
+            status_id=1
+            self.agent.action_in_progress(goal_id, status_id, vehicle_uuid)
+            time.sleep(0.05)
+            status_id=3
+            self.agent.action_finished(goal_id, status_id, vehicle_uuid)
 
-    def task_cancellation_handler(self, goal_id, vehicle):
+    def task_cancellation_handler(self, cancel_msg, vehicle):
         """Handles task cancellation info to specific robot"""
+        goal_id=cancel_msg.goal_id
         vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
         self.agent.log_info(
             f"[ROSHandler] Cancelling task with of vehicle: {self.agent.vehicle_names[vehicle_position]} goal id: {goal_id}")
 
         # if cancellation is received cancel goal
         # Refresh variables (it has to be before the cancel_goal so the path stops being sent and there is no delay
         # for the traffic control)
@@ -121,33 +188,33 @@
             # This line should be first to cancel the waypoints thread in ROS1
             self.agent.waypoints[vehicle_position] = False
             self.cancel_goal_waypoints(goal_id, vehicle_position)
         else:
             self.cancel_goal(goal_id, vehicle_position)
 
     def waypoints_handler(
-            self, vehicle_position, pose, current_task_uuid
+            self, vehicle_position, pose
     ):
         """Handles offline waypoints and sends to specific robot"""
         # ROS2
         try:
             self.agent.waypoints[vehicle_position] = True
             self.send_waypoints(pose, vehicle_position)
         except KeyError as error:
             self.agent.log_error(
                 f"[ROSHandler] Error waypoints_handler:{error}"
             )
 
             agent_sentry(error, "[ROSHandler] Error waypoints_handler")
 
     # def get_list_of_topic():
-    #    """Getting the list of topics available with specified namespace"""
-    #    # getting  topics available
-    #    topic_list = rospy.get_published_topics(namespace="/robot1")
-    #    return topic_list
+    #     """Getting the list of topics available with specified namespace"""
+    #     # getting  topics available
+    #     topic_list = rospy.get_published_topics(namespace="/robot1")
+    #     return topic_list
 
     def topic_request_handler(self, _):
         """logging information"""
         self.agent.log_info("[ROSHandler] Received topic request")
         # get_list_of_topic()
 
     def close_handler(self, *_):
@@ -163,37 +230,38 @@
             capture_message("[ROSHandler] WS error")
 
     def open_handler(self, *_, **__):
         """Opens the websocket connection"""
         self.agent.log_info("[ROSHandler] WS open")
         self.agent.ws_open = True
 
-    def path_rerouting_handler(self, _, data: dict, vehicle: str):
+    def path_rerouting_handler(self, path_rerouting_msg, data: dict, vehicle: str):
+        path=path_rerouting_msg["path"]
         vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
         
-        if data["path"] is not None:
+        if path is not None:
             self.agent.pause_paths[vehicle_position] = True
             self.agent.log_info(f"[ROSHandler] Path Rerouting vehicle: {self.agent.vehicle_names[vehicle_position]}")
             self.agent.goal_id_rerouted[vehicle_position] = self.agent.goal_id[vehicle_position]
             self.task_cancellation_handler(goal_id=self.agent.goal_id_rerouted[vehicle_position], vehicle=vehicle)
 
             data_new_path = {"rotation_angles": data["rotation_angles"], "metric_waypoints": data["path"]}
             current_task_uuid = "Rerouted_task"
 
             pose = parse_waypoints(data_new_path)
             self.agent.waypoints[vehicle_position] = True # To Test
             self.waypoints_handler(
                 vehicle_position=vehicle_position,
                 pose=pose,
-                current_task_uuid=current_task_uuid,
             )
         else:
             self.agent.log_error("[ROSHandler] Received empty path from path rerouting message.No action is done.")
 
-    def docking_routine_finalize_handler(self, data: dict, vehicle: str):
+
+    def docking_routine_finalize_handler(self, dock_msg: dict, vehicle: str):
         self.agent.log_info("[ROSHandler] Docking Routine FINALIZING request")
         vehicle_position = self.check_fleet_get_vehicle_position(vehicle)
 
         try:
             vehicle = self.agent.vehicles[vehicle_position]
             vehicle_prefix = str(vehicle["prefix"])
             if vehicle_prefix == "None":
@@ -216,18 +284,22 @@
                 path, rotation_angles = parse_docking_routine(result.plan)
                 self.agent.ping_docking_routine(vehicle["uuid"], path, rotation_angles)
             else:
                 self.agent.log_error(f"[ROSHandler] Docking output is None. Try again.")
         except Exception as e:
             self.agent.log_error(f"[ROSHandler] Error on Docking Routine Finalize: {e}")
 
-    def slow_down_handler(self, _, data: dict, vehicle: str):
+    def slow_down_handler(self, slow_down_msg, data: dict, vehicle: str):
+        # Method should be written in the particular ROS Handler
+        pass
+
+    def docking_routine_request_handler(self, dock_msg: dict, vehicle: str):
         # Method should be written in the particular ROS Handler
         pass
 
-    def docking_routine_request_handler(self, data: dict, vehicle: str):
+    def collision_clearance_handler(self, collision_clearance_msg: dict, vehicle: str):
         # Method should be written in the particular ROS Handler
         pass
 
-    def collision_clearance_handler(self, data: dict, vehicle: str):
+    def update_map_handler(self, data: dict, vehicle: str):
         # Method should be written in the particular ROS Handler
         pass
```

### Comparing `meili_ros_lib-0.1.8/meili_ros_lib/sentry.py` & `meili_ros_lib-0.2.0/meili_ros_lib/sentry.py`

 * *Files identical despite different names*

