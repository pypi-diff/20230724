# Comparing `tmp/biggo_pms_api_python-1.0.1.tar.gz` & `tmp/biggo_pms_api_python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biggo_pms_api_python-1.0.1.tar", last modified: Mon Jul 24 05:25:33 2023, max compression
+gzip compressed data, was "biggo_pms_api_python-1.0.2.tar", last modified: Mon Jul 24 05:59:37 2023, max compression
```

## Comparing `biggo_pms_api_python-1.0.1.tar` & `biggo_pms_api_python-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.1/LICENSE
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     1823 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.1/README.md
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/biggo_pms_api_python/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        0 2023-07-24 02:38:22.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/__init__.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/error.py
--rw-rw-r--   0 tuo       (1000) tuo       (1000)     7422 2023-07-24 05:25:20.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python/index.py
-drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/PKG-INFO
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 05:25:33.000000 biggo_pms_api_python-1.0.1/biggo_pms_api_python.egg-info/top_level.txt
--rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 05:25:33.509711 biggo_pms_api_python-1.0.1/setup.cfg
--rw-rw-r--   0 tuo       (1000) tuo       (1000)      284 2023-07-24 05:24:55.000000 biggo_pms_api_python-1.0.1/setup.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:59:37.840951 biggo_pms_api_python-1.0.2/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1069 2023-07-24 01:23:02.000000 biggo_pms_api_python-1.0.2/LICENSE
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:59:37.840951 biggo_pms_api_python-1.0.2/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     1795 2023-07-24 05:58:12.000000 biggo_pms_api_python-1.0.2/README.md
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:59:37.840951 biggo_pms_api_python-1.0.2/biggo_pms_api_python/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        0 2023-07-24 02:38:22.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python/__init__.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      451 2023-07-24 01:44:32.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python/error.py
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)     8273 2023-07-24 05:56:33.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python/index.py
+drwxrwxr-x   0 tuo       (1000) tuo       (1000)        0 2023-07-24 05:59:37.840951 biggo_pms_api_python-1.0.2/biggo_pms_api_python.egg-info/
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      261 2023-07-24 05:59:37.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      295 2023-07-24 05:59:37.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)        1 2023-07-24 05:59:37.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       21 2023-07-24 05:59:37.000000 biggo_pms_api_python-1.0.2/biggo_pms_api_python.egg-info/top_level.txt
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)       38 2023-07-24 05:59:37.840951 biggo_pms_api_python-1.0.2/setup.cfg
+-rw-rw-r--   0 tuo       (1000) tuo       (1000)      284 2023-07-24 05:59:21.000000 biggo_pms_api_python-1.0.2/setup.py
```

### Comparing `biggo_pms_api_python-1.0.1/LICENSE` & `biggo_pms_api_python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biggo_pms_api_python-1.0.1/README.md` & `biggo_pms_api_python-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 short future:
 
 - [Getting Started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Initializing](#initializing)
   - [Accessing BigGo API PMS](#accessing-biggo-api-pms)
-- [Typescript](#typescript)
 - [License](#license)
 
 ## Getting Started
 
 ### Installation
 
 Using npm
```

### Comparing `biggo_pms_api_python-1.0.1/biggo_pms_api_python/index.py` & `biggo_pms_api_python-1.0.2/biggo_pms_api_python/index.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,26 +84,52 @@
                 prams['method'],
                 f"{self.baseURL}{prams['path']}",
                 headers=headers,
                 params=prams.get('extraParams'),
                 json=prams.get('body'),
             )
             response.raise_for_status()
-            data = response.json()
+            
+            res_text = response.content.decode('utf-8-sig')
+            data = json.loads(res_text)
 
             if data.get('error_code') or data.get('result') == False:
                 raise BigGoError(f"{data.get('error') or data.get('message')}", data.get('error_code'))
 
             return data
         except requests.exceptions.RequestException as err:
             raise BigGoError(str(err))
         except BigGoError as err:
             raise err
         except Exception as err:
             raise BigGoError(str(err))
+        
+    async def fileRequest(self, prams):
+        headers = {
+            'Authorization': f"{self.tokenType} {await self.get_token()}",
+            **prams.get('extraHeaders', {})
+        }
+
+        try:
+            response = requests.request(
+                prams['method'],
+                f"{self.baseURL}{prams['path']}",
+                headers=headers,
+                params=prams.get('extraParams'),
+                json=prams.get('body'),
+            )
+            response.raise_for_status()
+            return response
+
+        except requests.exceptions.RequestException as err:
+            raise BigGoError(str(err))
+        except BigGoError as err:
+            raise err
+        except Exception as err:
+            raise BigGoError(str(err))
 
     async def get_platform_list(self):
         data = await self.request({
             'path': '/platform',
             'method': 'GET',
         })
         return [
@@ -167,15 +193,15 @@
                 'sampleSize': report['sample_size']
             }
             for report in data['data']
         ]
 
     async def get_report(self, platformID, reportID, fileType, options=None):
         options = options or {}
-        res = await self.request({
+        res = await self.fileRequest({
             'path': f'/export/{reportID}',
             'method': 'GET',
             'extraParams': {
                 'pms_platformid': platformID,
                 'file_type': fileType,
             },
             'responseType': 'arraybuffer' if fileType == 'excel' else None
@@ -197,8 +223,8 @@
         if not os.path.exists(save_dir):
             os.makedirs(save_dir, exist_ok=True)
 
         file_path = os.path.join(save_dir, file_name)
         with open(file_path, 'wb') as file:
             file.write(file_content)
 
-        return file_path
+        return file_path
```

