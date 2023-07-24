# Comparing `tmp/uagents_twilio-1.0.3.tar.gz` & `tmp/uagents_twilio-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio-1.0.3.tar", max compression
+gzip compressed data, was "uagents_twilio-1.0.4.tar", max compression
```

## Comparing `uagents_twilio-1.0.3.tar` & `uagents_twilio-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.3/LICENSE
--rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio-1.0.3/README.rst
--rw-r--r--   0        0        0      872 2023-07-24 11:18:08.646847 uagents_twilio-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.3/uagents_twilio/__init__.py
--rw-r--r--   0        0        0      177 2023-07-24 11:18:24.487175 uagents_twilio-1.0.3/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.3/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-24 11:18:24.631178 uagents_twilio-1.0.3/uagents_twilio/protocols/messages.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.3/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     2251 2023-07-24 11:18:24.519175 uagents_twilio-1.0.3/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 uagents_twilio-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.4/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio-1.0.4/README.rst
+-rw-r--r--   0        0        0      872 2023-07-24 13:59:09.243494 uagents_twilio-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.4/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio-1.0.4/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.4/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio-1.0.4/uagents_twilio/protocols/messages.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.4/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio-1.0.4/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 uagents_twilio-1.0.4/PKG-INFO
```

### Comparing `uagents_twilio-1.0.3/LICENSE` & `uagents_twilio-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.3/README.rst` & `uagents_twilio-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.3/pyproject.toml` & `uagents_twilio-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-twilio"
 #
-version = '1.0.3'
+version = '1.0.4'
 #
 description = ""
 authors = ["Harsh <harsh@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/Github User/uagents-twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
```

### Comparing `uagents_twilio-1.0.3/uagents_twilio/protocols/messages.py` & `uagents_twilio-1.0.4/uagents_twilio/protocols/messages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from decouple import config
 from uagents import Context, Protocol
 
-from uagents_twilio.models import SMS, WhatsAppMsg
+from uagents_twilio.models import Message, MessageType
 from uagents_twilio.wrappers.messageWrapper import MessageClient
 
 service_protocol = Protocol()
 AGENT_ADDRESS = config("AGENT_ADDRESS")
 ACCOUNT_SID = config("ACCOUNT_SID")
 AUTH_TOKEN = config("AUTH_TOKEN")
 FROM_NUMBER = config("FROM_NUMBER")
@@ -19,39 +19,27 @@
     account_sid=ACCOUNT_SID,
     auth_token=AUTH_TOKEN,
     from_number=FROM_NUMBER,
     to_number=TO_NUMBER,
 )
 
 
-@service_protocol.on_query(model=WhatsAppMsg)
-async def receive_wp_msg(ctx: Context, sender: str, message: WhatsAppMsg):
+@service_protocol.on_query(model=Message)
+async def receive_wp_msg(ctx: Context, sender: str, message: Message):
     """Receive message from Twilio Webhook and send starting message on Whatsapp"""
     ctx.storage.set("message", message.msg)
-    if not message.receiver.startswith("whatsapp:"):
-        message.receiver = f"whatsapp:{message.receiver}"
-    message_handler.from_number = WP_FROM_NUMBER
-    message_handler.send_new_wp_message(message.receiver, message.msg)
+    if message.type == MessageType.whatsapp:
+        if not message.receiver.startswith("whatsapp:"):
+            message.receiver = f"whatsapp:{message.receiver}"
+        message_handler.from_number = WP_FROM_NUMBER
+    message_handler.send_message(message.receiver, message.msg, message.type)
 
 
-@service_protocol.on_message(model=WhatsAppMsg)
-async def send_wp_msg(ctx: Context, sender: str, message: WhatsAppMsg):
-    """Send message on Whatsapp using on_interval method"""
+@service_protocol.on_message(model=Message)
+async def send_wp_msg(ctx: Context, sender: str, message: Message):
+    """Send Whatsapp Message or SMS using uagent"""
     ctx.storage.set("message", message.msg)
-    if not message.receiver.startswith("whatsapp:"):
-        message.receiver = f"whatsapp:{message.receiver}"
-    message_handler.from_number = WP_FROM_NUMBER
-    message_handler.send_new_wp_message(message.receiver, message.msg)
-
-
-@service_protocol.on_query(model=SMS)
-async def receive_msg(ctx: Context, sender: str, message: SMS):
-    """Receive message from Twilio Webhook and send starting message on Whatsapp"""
-    ctx.storage.set("message", message.msg)
-    message_handler.send_new_message(message.receiver, message.msg)
-
-
-@service_protocol.on_message(model=SMS)
-async def send_msg(ctx: Context, sender: str, message: SMS):
-    """Send message on Whatsapp using on_interval method"""
-    ctx.storage.set("message", message.msg)
-    message_handler.send_new_message(message.receiver, message.msg)
+    if message.type == MessageType.whatsapp:
+        if not message.receiver.startswith("whatsapp:"):
+            message.receiver = f"whatsapp:{message.receiver}"
+        message_handler.from_number = WP_FROM_NUMBER
+    message_handler.send_message(message.receiver, message.msg, message.type)
```

### Comparing `uagents_twilio-1.0.3/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio-1.0.4/uagents_twilio/wrappers/messageWrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Start writing utility wrapper from here
 import requests
-from uagents import Agent, Context
+from uagents import Agent
+
+from uagents_twilio.models import MessageType
 
 
 class MessageClient:
     """Base class for handling WhatsApp operations"""
 
     def __init__(
         self,
@@ -17,34 +19,21 @@
     ):
         self.agent = agent
         self.to_agent_address = to_agent_address
         self.account_sid = account_sid
         self.auth_token = auth_token
         self.from_number = from_number
         self.to_number = to_number
-        # fund_agent_if_low(agent.wallet.address())
-
-    def listen_for_new_message(self, ctx: Context, sender_no: str, body: str):
-        if sender_no == "" or body == "":
-            return
-        else:
-            ctx.logger.info(
-                f"Received a new message from {sender_no}, message : {body}"
-            )
-            self.send_new_message(body)
-
-    def send_new_message(self, receiver, message: str):
-        body = message
-        twilio = TwilioWrapper(self.account_sid, self.auth_token)
-        twilio.send_message(self.from_number, receiver, body)
 
-    def send_new_wp_message(self, receiver, message: str):
+    def send_message(self, receiver, message: str, message_type):
         body = message
         twilio = TwilioWrapper(self.account_sid, self.auth_token)
-        if not self.from_number.startswith("whatsapp:"):
+        if message_type == MessageType.whatsapp and not self.from_number.startswith(
+            "whatsapp:"
+        ):
             self.from_number = f"whatsapp:{self.from_number}"
         twilio.send_message(self.from_number, receiver, body)
 
 
 class TwilioWrapper:
     def __init__(self, account_sid, auth_token):
         self.account_sid = account_sid
```

### Comparing `uagents_twilio-1.0.3/PKG-INFO` & `uagents_twilio-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-twilio
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Home-page: https://github.com/Github User/uagents-twilio
 Author: Harsh
 Author-email: harsh@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

