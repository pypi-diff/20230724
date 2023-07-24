# Comparing `tmp/OKAppleAPI-1.4.2.tar.gz` & `tmp/OKAppleAPI-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OKAppleAPI-1.4.2.tar", last modified: Tue Feb 14 07:49:58 2023, max compression
+gzip compressed data, was "dist/OKAppleAPI-1.4.3.tar", last modified: Mon Jul 24 09:34:06 2023, max compression
```

## Comparing `OKAppleAPI-1.4.2.tar` & `OKAppleAPI-1.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-02-14 07:49:58.031636 OKAppleAPI-1.4.2/
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-02-14 07:49:58.029622 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/
--rw-r--r--   0 shaowei    (501) staff       (20)     3957 2023-02-14 07:49:57.000000 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/PKG-INFO
--rw-r--r--   0 shaowei    (501) staff       (20)      274 2023-02-14 07:49:57.000000 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/SOURCES.txt
--rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-02-14 07:49:57.000000 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/dependency_links.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       49 2023-02-14 07:49:57.000000 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/requires.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       11 2023-02-14 07:49:57.000000 OKAppleAPI-1.4.2/OKAppleAPI.egg-info/top_level.txt
--rw-r--r--   0 shaowei    (501) staff       (20)     3957 2023-02-14 07:49:58.031439 OKAppleAPI-1.4.2/PKG-INFO
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-02-14 07:49:58.030934 OKAppleAPI-1.4.2/okappleapi/
--rw-r--r--   0 shaowei    (501) staff       (20)       78 2022-01-18 07:57:10.000000 OKAppleAPI-1.4.2/okappleapi/__init__.py
--rw-r--r--   0 shaowei    (501) staff       (20)    20244 2023-01-30 08:00:30.000000 OKAppleAPI-1.4.2/okappleapi/apple_api_agent.py
--rw-r--r--   0 shaowei    (501) staff       (20)    10910 2023-02-14 07:38:56.000000 OKAppleAPI-1.4.2/okappleapi/models.py
--rw-r--r--   0 shaowei    (501) staff       (20)     9675 2023-01-11 17:22:17.000000 OKAppleAPI-1.4.2/okappleapi/ok_agent.py
--rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-02-14 07:49:58.031704 OKAppleAPI-1.4.2/setup.cfg
--rw-r--r--   0 shaowei    (501) staff       (20)     1365 2023-02-14 07:46:51.000000 OKAppleAPI-1.4.2/setup.py
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-07-24 09:34:06.826688 OKAppleAPI-1.4.3/
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-07-24 09:34:06.824907 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/
+-rw-r--r--   0 shaowei    (501) staff       (20)     3957 2023-07-24 09:34:06.000000 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/PKG-INFO
+-rw-r--r--   0 shaowei    (501) staff       (20)      274 2023-07-24 09:34:06.000000 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-07-24 09:34:06.000000 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       49 2023-07-24 09:34:06.000000 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/requires.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       11 2023-07-24 09:34:06.000000 OKAppleAPI-1.4.3/OKAppleAPI.egg-info/top_level.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)     3957 2023-07-24 09:34:06.826500 OKAppleAPI-1.4.3/PKG-INFO
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-07-24 09:34:06.826195 OKAppleAPI-1.4.3/okappleapi/
+-rw-r--r--   0 shaowei    (501) staff       (20)       78 2022-01-18 07:57:10.000000 OKAppleAPI-1.4.3/okappleapi/__init__.py
+-rw-r--r--   0 shaowei    (501) staff       (20)    20520 2023-03-08 18:03:53.000000 OKAppleAPI-1.4.3/okappleapi/apple_api_agent.py
+-rw-r--r--   0 shaowei    (501) staff       (20)    10910 2023-02-14 07:38:56.000000 OKAppleAPI-1.4.3/okappleapi/models.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     9664 2023-07-24 09:28:12.000000 OKAppleAPI-1.4.3/okappleapi/ok_agent.py
+-rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-07-24 09:34:06.826762 OKAppleAPI-1.4.3/setup.cfg
+-rw-r--r--   0 shaowei    (501) staff       (20)     1365 2023-07-24 09:33:05.000000 OKAppleAPI-1.4.3/setup.py
```

### Comparing `OKAppleAPI-1.4.2/OKAppleAPI.egg-info/PKG-INFO` & `OKAppleAPI-1.4.3/OKAppleAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OKAppleAPI
-Version: 1.4.2
+Version: 1.4.3
 Summary: OK App Store Connect API
 Home-page: https://github.com/shede333/OKAppleAPI
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
 Description: # OK App Store Connect API
```

### Comparing `OKAppleAPI-1.4.2/PKG-INFO` & `OKAppleAPI-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OKAppleAPI
-Version: 1.4.2
+Version: 1.4.3
 Summary: OK App Store Connect API
 Home-page: https://github.com/shede333/OKAppleAPI
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
 Description: # OK App Store Connect API
```

### Comparing `OKAppleAPI-1.4.2/okappleapi/apple_api_agent.py` & `OKAppleAPI-1.4.3/okappleapi/apple_api_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,23 @@
                 return self._api_call(url=url, method=method, post_data=post_data,
                                       verbose=verbose, retry_num=(retry_num - 1))
 
             raise APIError(str(errors), error_list=errors, status_code=result.status_code)
 
         return json_info
 
+    def test_get_url(self, url: str, verbose=True) -> Dict:
+        """
+        测试get接口
+        @param verbose: 是否打印详细信息，默认False
+        @return:
+        """
+        result_dict = self._api_call(url, verbose=verbose)
+        return result_dict
+
     def list_certificates(self, filters: Dict = None, verbose=False) -> List[Certificate]:
         """
         certificate列表
         https://developer.apple.com/documentation/appstoreconnectapi/list_and_download_certificates
         @param filters: 筛选器
         @param verbose: 是否打印详细信息，默认False
         @return:
@@ -542,7 +551,8 @@
         https://developer.apple.com/documentation/appstoreconnectapi/disable_a_capability
         @param capability_id: 代表capability的id
         @return:
         """
         endpoint = f'/v1/bundleIdCapabilities/{capability_id}'
         url = create_full_url(endpoint)
         self._api_call(url, method=HttpMethod.DELETE)
+
```

### Comparing `OKAppleAPI-1.4.2/okappleapi/models.py` & `OKAppleAPI-1.4.3/okappleapi/models.py`

 * *Files identical despite different names*

### Comparing `OKAppleAPI-1.4.2/okappleapi/ok_agent.py` & `OKAppleAPI-1.4.3/okappleapi/ok_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         print(f'cer: {len(cer_list)}, is_dev: {is_dev}')
         # 创建新的Profile
         result_profile = self.agent.create_a_profile(attrs=attrs, bundle_id=bundle_id,
                                                      devices=device_list, certificates=cer_list)
         if result_profile:
             if is_save:
                 self.save_mobile_provision(result_profile)
-            tmp_list = filter(lambda x: x.name != name, self.profile_list)
-            tmp_list = list(tmp_list).append(result_profile)
+            tmp_list = list(filter(lambda x: x.name != name, self.profile_list))
+            tmp_list.append(result_profile)
             self._profile_list = tmp_list
         print(f'update profile success: {name}')
         return result_profile
 
     @staticmethod
     def save_mobile_provision(profile: Profile):
         """
```

### Comparing `OKAppleAPI-1.4.2/setup.py` & `OKAppleAPI-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("ReadMe.md").read_text()
 
 print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='OKAppleAPI',  # 包名字
-    version='1.4.2',  # 包版本
+    version='1.4.3',  # 包版本
     author='shede333',  # 作者
     author_email='333wshw@163.com',  # 作者邮箱
     keywords='ios ok apple appstore app store connect api appstoreconnectapi',
     description='OK App Store Connect API',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/shede333/OKAppleAPI',  # 包的主页
```

