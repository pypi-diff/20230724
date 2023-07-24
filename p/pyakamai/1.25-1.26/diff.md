# Comparing `tmp/pyakamai-1.25-py3-none-any.whl.zip` & `tmp/pyakamai-1.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 29368 bytes, number of entries: 20
+Zip file size: 29352 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     2239 b- defN 23-Jul-20 07:24 pyakamai/akamaiapidefinition.py
 -rw-r--r--  2.0 unx     3819 b- defN 23-Jul-09 12:14 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
 -rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
 -rw-r--r--  2.0 unx    14193 b- defN 23-May-01 03:54 pyakamai/akamaiksd1.py
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Jul-09 11:44 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx    29604 b- defN 23-Jul-04 02:23 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
--rw-r--r--  2.0 unx     8308 b- defN 23-Jul-20 07:45 pyakamai/http_calls.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jul-24 04:33 pyakamai/http_calls.py
 -rw-r--r--  2.0 unx     2830 b- defN 23-Jul-20 07:10 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx    12832 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1587 b- defN 23-Jul-20 08:29 pyakamai-1.25.dist-info/RECORD
-20 files, 111978 bytes uncompressed, 26818 bytes compressed:  76.1%
+-rw-r--r--  2.0 unx    12832 b- defN 23-Jul-24 04:34 pyakamai-1.26.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 04:34 pyakamai-1.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-24 04:34 pyakamai-1.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1587 b- defN 23-Jul-24 04:34 pyakamai-1.26.dist-info/RECORD
+20 files, 111738 bytes uncompressed, 26802 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.25.dist-info/METADATA
+Filename: pyakamai-1.26.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.25.dist-info/WHEEL
+Filename: pyakamai-1.26.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.25.dist-info/top_level.txt
+Filename: pyakamai-1.26.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.25.dist-info/RECORD
+Filename: pyakamai-1.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyakamai/http_calls.py

```diff
@@ -45,15 +45,14 @@
         """ Executes a GET API call and returns the JSON output """
         path = endpoint
         endpoint_result = self.session.get(parse.urljoin(self.baseurl,path), headers=headers,params=params)
         if self.verbose: print (">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
         status = endpoint_result.status_code
         if self.verbose: print( "LOG: GET %s %s %s" % (endpoint,status,endpoint_result.headers["content-type"]))
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
-        formattedjson = json.dumps(endpoint_result.json(),indent=2)
         return status,endpoint_result.json()
 
 
     def postResult(self, endpoint, body,params=None,headers=None):
         """ Executes a GET API call and returns the JSON output """
         if headers == None:
             headers = {'content-type': 'application/json'}
@@ -65,16 +64,15 @@
             print("LOG: POST %s %s %s" % (path, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return status,{}
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
 
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        formattedjson = json.dumps(endpoint_result.json(),indent=2)
-        return status,formattedjson
+        return status,endpoint_result.json()
     
 
     def patchResult(self, endpoint, body, parameters=None):
         """ Executes a GET API call and returns the JSON output """
         headers = {'content-type': 'application/json-patch+json'}
         path = endpoint
         endpoint_result = self.session.patch(parse.urljoin(self.baseurl, path), data=body, headers=headers, params=parameters)
@@ -83,16 +81,16 @@
             print("LOG: POST %s %s %s" % (path, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return {}
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
 
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        formattedjson = json.dumps(endpoint_result.json(),indent=2)
-        return status,formattedjson
+    
+        return status,endpoint_result.json()
 
     def postFiles(self, endpoint, file):
         """ Executes a POST API call and returns the JSON output """
         path = endpoint
         endpoint_result = self.session.post(parse.urljoin(self.baseurl, path), files=file)
         status = endpoint_result.status_code
         if self.verbose:
@@ -115,16 +113,15 @@
         status = endpoint_result.status_code
         if self.verbose:
             print("LOG: PUT %s %s %s" % (endpoint, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return status,{}
         if self.verbose:
             print(">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
-        formattedjson = json.dumps(endpoint_result.json(),indent=2)
-        return status,formattedjson
+        return status,endpoint_result.json()
 
     def deleteResult(self, endpoint):
         """ Executes a DELETE API call and returns the JSON output """
         endpoint_result = self.session.delete(parse.urljoin(self.baseurl,endpoint))
         status = endpoint_result.status_code
         if self.verbose:
             print("LOG: DELETE %s %s %s" % (endpoint, status, endpoint_result.headers["content-type"]))
```

## Comparing `pyakamai-1.25.dist-info/METADATA` & `pyakamai-1.26.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 1.25
+Version: 1.26
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyakamai-1.25.dist-info/RECORD` & `pyakamai-1.26.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 pyakamai/akamaiehn.py,sha256=aZ2U6YG54IKP5vuQPd5GygalsJqVuEzvCnALjjszRFI,2843
 pyakamai/akamaiksd1.py,sha256=7RslIDB6oR3KA4nyC7infxXqH4Jr7dM0t3znyDfCUPI,14193
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=jh1ooqCel03ADDtKhTOWUoW_F03ez-SH2U5iaqhF3cs,29604
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
-pyakamai/http_calls.py,sha256=S20uXu1_czpu5jUMqsV9sHz91UJDRjtdFv6AHnb3ceQ,8308
+pyakamai/http_calls.py,sha256=tLkWW55z-Ao6xdDQp541TvFPXsGdbGtJgqloXCvdLuM,8068
 pyakamai/pyakamai.py,sha256=pBI6CoOcV0JOBRntQ7YfU_Wn6gKC07LwnDRg4JfqDMQ,2830
-pyakamai-1.25.dist-info/METADATA,sha256=t1DyUKeU-s7c1IJm8UI8awphi3Wccli1Vb2bDmKrbTE,12832
-pyakamai-1.25.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyakamai-1.25.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.25.dist-info/RECORD,,
+pyakamai-1.26.dist-info/METADATA,sha256=WDSz5JMagBFqVXio4cs78j8jb-UsbPRNTqKF3JMlHhE,12832
+pyakamai-1.26.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyakamai-1.26.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.26.dist-info/RECORD,,
```

