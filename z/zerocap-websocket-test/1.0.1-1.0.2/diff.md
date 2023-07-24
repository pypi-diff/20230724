# Comparing `tmp/zerocap_websocket_test-1.0.1.tar.gz` & `tmp/zerocap_websocket_test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_websocket_test-1.0.1.tar", last modified: Fri Jul 21 10:13:57 2023, max compression
+gzip compressed data, was "zerocap_websocket_test-1.0.2.tar", last modified: Mon Jul 24 08:44:18 2023, max compression
```

## Comparing `zerocap_websocket_test-1.0.1.tar` & `zerocap_websocket_test-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.604308 zerocap_websocket_test-1.0.1/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.1/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)      873 2023-07-21 10:13:57.604037 zerocap_websocket_test-1.0.1/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)       18 2023-07-21 10:13:46.000000 zerocap_websocket_test-1.0.1/README.rst
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-21 10:13:57.604385 zerocap_websocket_test-1.0.1/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)     1167 2023-07-21 10:13:46.000000 zerocap_websocket_test-1.0.1/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.600637 zerocap_websocket_test-1.0.1/zerocap_websocket_test/
--rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     2389 2023-07-21 10:05:12.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-21 10:13:57.603654 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)      873 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      281 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-21 10:13:57.000000 zerocap_websocket_test-1.0.1/zerocap_websocket_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-24 08:44:18.515255 zerocap_websocket_test-1.0.2/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.2/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)      404 2023-07-24 08:44:18.514922 zerocap_websocket_test-1.0.2/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)       18 2023-07-21 10:13:46.000000 zerocap_websocket_test-1.0.2/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-24 08:44:18.515343 zerocap_websocket_test-1.0.2/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      781 2023-07-24 08:44:14.000000 zerocap_websocket_test-1.0.2/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-24 08:44:18.512645 zerocap_websocket_test-1.0.2/zerocap_websocket_test/
+-rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     3763 2023-07-24 05:31:57.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-24 08:44:18.514503 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)      404 2023-07-24 08:44:18.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      326 2023-07-24 08:44:18.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-24 08:44:18.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       10 2023-07-24 08:44:18.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-24 08:44:18.000000 zerocap_websocket_test-1.0.2/zerocap_websocket_test.egg-info/top_level.txt
```

### Comparing `zerocap_websocket_test-1.0.1/LICENSE.txt` & `zerocap_websocket_test-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.1/zerocap_websocket_test/main.py` & `zerocap_websocket_test-1.0.2/zerocap_websocket_test/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,83 +5,121 @@
 	- get_orders     Subscribe order updates, and order records
 
 	You can just call each of message, it should work out of the box.
 	It should also very convenient to be modified to call other endpoints.
 
 	Notes:
 	- websokcet-client package is required, you can install by: pip install websocket-client
+	pip install zerocap-websocket-test -i https://www.pypi.org/simple/
 	- API key and secret are required for endpoints that require signature
 
 """
 import hmac
 import json
 import hashlib
-from websocket import create_connection
+import requests
+from websocket import create_connection, WebSocketException
 
 
 class ZerocapWebsocketTest:
-	def __init__(self, apiKey, apiSecret):
+	def __init__(self, apiKey, apiSecret, ):
 		# TODO add your own API key and secret
 		self.apiKey = apiKey
 		self.apiSecret = apiSecret
+		self.market_websocket = None
+		self.order_websocket = None
+		self.base_url = "wss://dma-api.defi.wiki/ws"
+		self.http_url = "https://dma-api.defi.wiki/orders"
+		self.signature = self.hashing()
+		self.verify_identity()
+
+	def verify_identity(self):
+		headers = {'Content-Type': 'application/json'}
+		data = {"api_key": self.apiKey, "signature": self.signature}
+		url = f"{self.http_url}/api_key_signature_valid"
+		response = requests.post(url, data=json.dumps(data), headers=headers)
+		if response.status_code != 200 or response.json().get('status_code') != 200:
+			raise Exception("Authentication failed")
 
-	def hashing(self, query_string):
+	def hashing(self):
 		return hmac.new(
-			self.apiSecret.encode("utf-8"), query_string.encode("utf-8"), hashlib.sha256
+			self.apiSecret.encode("utf-8"), self.apiKey.encode("utf-8"), hashlib.sha256
 		).hexdigest()
 
 	def get_params(self, channel):
 		'''
 		Get request parameters
 		:param channel:
 		:return: params
 		'''
 
 		data_type = ""
 		if channel == "orders":
 			data_type = "order,trader"
 		elif channel == "market":
-			data_type = "price,order_book,k_line"
+			data_type = "price"
 
-		params = {
+		return {
 			"api_key": self.apiKey,
+			"signature": self.signature,
 			"data_type": data_type,
-			"signature": self.hashing(self.apiKey)
 		}
-		return params
+
+	def close(self):
+		if self.order_websocket:
+			self.order_websocket.close()
+		if self.market_websocket:
+			self.market_websocket.close()
+		return
 
 	def get_message(self, ws_recv):
-		'''
-		:param ws_recv:
-		:return: message
-		'''
 		return ws_recv.__next__()
 
 	def get_orders(self):
-		params = self.get_params(channel="orders")
-		wss_url = f'wss://dma-api.defi.wiki/ws/GetOrdersInfo?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
-		ws = create_connection(wss_url)
-		while True:
-			message = ws.recv()
-			yield message
+		try:
+			params = self.get_params(channel="orders")
+			wss_url = f'{self.base_url}/GetOrdersInfo?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
+			self.order_websocket = create_connection(wss_url)
+			while True:
+				message = self.order_websocket.recv()
+				yield message
+		except Exception as e:
+			self.close()
+			raise WebSocketException(500, f'{e}')
 
 	def get_market(self):
-		params = self.get_params(channel="market")
-		wss_url = f'wss://dma-api.defi.wiki/ws/GetMarket?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
-		websocket = create_connection(wss_url)
-		while True:
-			message = websocket.recv()
-			yield message
+		try:
+			params = self.get_params(channel="market")
+			wss_url = f'{self.base_url}/GetMarket?api_key={params["api_key"]}&signature={params["signature"]}&data_type={params["data_type"]}'
+			self.market_websocket = create_connection(wss_url)
+			while True:
+				message = self.market_websocket.recv()
+				yield message
+		except Exception as e:
+			self.close()
+			raise WebSocketException(500, f'{e}')
 
 
 if __name__ == "__main__":
-	apiKey = ""
-	apiSecret = ""
+	apiKey = "coinroutes"
+	apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
 	# ws = ZerocapWebsocketTest(apiKey, apiSecret)
-	# websocket = ws.get_orders()
+	# # websocket = ws.get_orders()
 	# websocket = ws.get_market()
 	# while True:
-	# 	print(ws.get_message(websocket))
+	# 	message = ws.get_message(websocket)
+	# 	if json.loads(message).get('error_code'):
+	# 		print(f"Receiving message from server: \n{message}")
+	# 		print("Connection close")
+	# 		break
+	# 	if not json.loads(message).get('channel'):
+	# 		continue
+	#
+	# 	print(f"Receiving message from server: \n{message}")
+	# 	if not message:
+	# 		print("Connection close")
+	# 		break
+	# ws.close()
 
 
 
-# pip install zerocap-websocket-test -i https://www.pypi.org/simple/
+# pip install zerocap-websocket-test -i https://www.pypi.org/simple/
```

