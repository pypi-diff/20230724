# Comparing `tmp/chatglm-llm-1.4.6.tar.gz` & `tmp/chatglm-llm-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.4.6.tar", last modified: Wed Jul 19 07:17:41 2023, max compression
+gzip compressed data, was "chatglm-llm-1.4.7.tar", last modified: Mon Jul 24 08:27:53 2023, max compression
```

## Comparing `chatglm-llm-1.4.6.tar` & `chatglm-llm-1.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:17:41.216721 chatglm-llm-1.4.6/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.6/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-19 07:17:41.216576 chatglm-llm-1.4.6/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.6/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:17:41.214845 chatglm-llm-1.4.6/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-19 07:17:40.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      540 2023-07-19 07:17:41.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-19 07:17:40.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-07-19 07:17:41.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      276 2023-07-19 07:17:41.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-07-19 07:17:41.000000 chatglm-llm-1.4.6/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:17:41.215614 chatglm-llm-1.4.6/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.6/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.6/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:17:41.216190 chatglm-llm-1.4.6/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.6/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.6/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.6/chatglm_src/chatglm_utils.py
--rw-r--r--   0 mroy       (501) staff       (20)     2876 2023-07-19 07:04:40.000000 chatglm-llm-1.4.6/chatglm_src/cluster_and_smi.py
--rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.6/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3289 2023-07-19 07:15:24.000000 chatglm-llm-1.4.6/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    41882 2023-07-04 07:12:19.000000 chatglm-llm-1.4.6/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-19 07:17:41.216354 chatglm-llm-1.4.6/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.6/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-19 07:17:41.216775 chatglm-llm-1.4.6/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1103 2023-07-19 07:17:39.000000 chatglm-llm-1.4.6/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-24 08:27:53.431695 chatglm-llm-1.4.7/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.7/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-24 08:27:53.431581 chatglm-llm-1.4.7/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.7/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-24 08:27:53.430215 chatglm-llm-1.4.7/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      540 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      276 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-07-24 08:27:53.000000 chatglm-llm-1.4.7/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-24 08:27:53.430993 chatglm-llm-1.4.7/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.7/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.7/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-24 08:27:53.431273 chatglm-llm-1.4.7/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.7/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.7/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2272 2023-06-28 08:26:21.000000 chatglm-llm-1.4.7/chatglm_src/chatglm_utils.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3023 2023-07-24 08:25:33.000000 chatglm-llm-1.4.7/chatglm_src/cluster_and_smi.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.7/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3445 2023-07-24 08:25:12.000000 chatglm-llm-1.4.7/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    41884 2023-07-24 08:21:31.000000 chatglm-llm-1.4.7/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-07-24 08:27:53.431396 chatglm-llm-1.4.7/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.7/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-07-24 08:27:53.431736 chatglm-llm-1.4.7/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1103 2023-07-24 08:25:59.000000 chatglm-llm-1.4.7/setup.py
```

### Comparing `chatglm-llm-1.4.6/README.md` & `chatglm-llm-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_llm.egg-info/SOURCES.txt` & `chatglm-llm-1.4.7/chatglm_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/__init__.py` & `chatglm-llm-1.4.7/chatglm_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/callbacks.py` & `chatglm-llm-1.4.7/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.4.7/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/chatglm_utils.py` & `chatglm-llm-1.4.7/chatglm_src/chatglm_utils.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/cluster_and_smi.py` & `chatglm-llm-1.4.7/chatglm_src/cluster_and_smi.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,30 @@
     })
     msg = send_and_recv(data, ws)
     return msg
 
 
 def send_and_recv(data, ws):
     try:
-        for i in tqdm.tqdm(range(0, len(data), 1024*102), desc=termcolor.colored(" + sending data","cyan")):
+        T = len(data)// 1024*102
+        bart = tqdm.tqdm(total=T,desc=termcolor.colored(" + sending data","cyan"))
+        for i in range(0, len(data), 1024*102):
+            bart.update(1)
             ws.send(data[i:i+1024*102])
+        bart.clear()
+        # bart.close()
         ws.send("[STOP]")
         message = ""
         total = int(ws.recv())
         bar = tqdm.tqdm(desc=termcolor.colored(" + receiving data","cyan", attrs=["bold"]), total=total)
         while 1:
             res = ws.recv()
             message += res
             bar.update(len(res))
             if message.endswith("[STOP]"):
                 message = message[:-6]
                 break
+        bart.clear()
         msg = json.loads(message)
         return msg
     except Exception as e:
         raise e
```

### Comparing `chatglm-llm-1.4.6/chatglm_src/cmd.py` & `chatglm-llm-1.4.7/chatglm_src/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/chatglm_src/embeding.py` & `chatglm-llm-1.4.7/chatglm_src/embeding.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,33 @@
         if remote_host is None:
             self._emb = HuggingFaceEmbeddings(model_name=model_path)
         else:
             self.remote_host = remote_host
 
     def send_and_recv(self, data, ws):
         try:
-            for i in tqdm.tqdm(range(0, len(data), 1024*102), desc=colored(" + sending data","cyan")):
+            T = len(data)// 1024*102
+            bart = tqdm.tqdm(total=T,desc=colored(" + sending data","cyan"))
+            for i in range(0, len(data), 1024*102):
+                bart.update(1)
                 ws.send(data[i:i+1024*102])
+            bart.clear()
+            
             ws.send("[STOP]")
             message = ""
             total = int(ws.recv())
             bar = tqdm.tqdm(desc=colored(" + receiving data","cyan", attrs=["bold"]), total=total)
             while 1:
                 res = ws.recv()
                 message += res
                 bar.update(len(res))
                 if message.endswith("[STOP]"):
                     message = message[:-6]
                     break
+            bar.clear()
             msg = json.loads(message)
             return msg
         except Exception as e:
             raise e
 
     def embed_documents_remote(self, texts):
         ws = create_connection(f"ws://{self.remote_host}:15000")
```

### Comparing `chatglm-llm-1.4.6/chatglm_src/llm.py` & `chatglm-llm-1.4.7/chatglm_src/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         cache_obj.init(
             pre_embedding_func=get_prompt,
             data_manager=get_data_manager(data_path=cache_path),
         )
         i += 1
     
     langchain.llm_cache = GPTCache(init_gptcache_map)
-    print(colored("init gptcache", "green"))
+    # print(colored("init gptcache", "green"))
 except Exception as e:
     print("use remote ignore this / load transformers failed, please install transformers and accelerate first and torch.")
 from .callbacks import AsyncWebsocketHandler, AsyncWebSocksetCallbackManager
 
 TEXT_EMB_PATH = pathlib.Path("~").expanduser() / ".cache"/"torch"/"sentence_transformers"/"GanymedeNil_text2vec-large-chinese"
 if TEXT_EMB_PATH.exists():
     TEXT_EMB_PATH = str(TEXT_EMB_PATH)
```

### Comparing `chatglm-llm-1.4.6/chatglm_src/loader/__init__.py` & `chatglm-llm-1.4.7/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.6/setup.py` & `chatglm-llm-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.4.6',
+    version='1.4.7',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

