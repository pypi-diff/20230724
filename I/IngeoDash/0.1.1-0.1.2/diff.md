# Comparing `tmp/IngeoDash-0.1.1.tar.gz` & `tmp/IngeoDash-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.1.1.tar", last modified: Thu Jul 20 19:36:39 2023, max compression
+gzip compressed data, was "IngeoDash-0.1.2.tar", last modified: Mon Jul 24 12:22:04 2023, max compression
```

## Comparing `IngeoDash-0.1.1.tar` & `IngeoDash-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.429639 IngeoDash-0.1.1/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.429639 IngeoDash-0.1.1/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 12:22:04.000000 IngeoDash-0.1.2/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-24 12:22:04.000000 IngeoDash-0.1.2/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:22:04.000000 IngeoDash-0.1.2/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 12:22:04.000000 IngeoDash-0.1.2/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 12:22:04.000000 IngeoDash-0.1.2/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:22:04.953738 IngeoDash-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-24 12:20:23.000000 IngeoDash-0.1.2/setup.py
```

### Comparing `IngeoDash-0.1.1/IngeoDash/__init__.py` & `IngeoDash-0.1.2/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

### Comparing `IngeoDash-0.1.1/IngeoDash/__main__.py` & `IngeoDash-0.1.2/IngeoDash/__main__.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/annotate.py` & `IngeoDash-0.1.2/IngeoDash/annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,29 @@
     if mem.label_header in x:
         ele = x[mem.label_header]
         if ele is not None and len(f'{ele}'):
             return True
     return False
 
 
-def model(mem: Config, data: dict, select: bool=True):
+def model(mem: Config, data: dict):
     lang = mem[mem.lang]
     if lang not in CONFIG.denseBoW:
         dense = DenseBoW(lang=lang, voc_size_exponent=mem.voc_size_exponent,
                          voc_selection=mem.voc_selection,
                          n_jobs=mem.n_jobs, dataset=False)
         CONFIG.denseBoW[lang] = dense.text_representations
     dense = DenseBoW(lang=lang, key=mem.text,
                      label_key=mem.label_header,
                      voc_size_exponent=mem.voc_size_exponent,
                      voc_selection=mem.voc_selection,
                      n_jobs=mem.n_jobs,
                      dataset=False, emoji=False, keyword=False)
     dense.text_representations_extend(CONFIG.denseBoW[lang])
-    if select:
+    if mem.dense_select:
         dense.select(D=data)
     _ = np.unique([x[mem.label_header] for x in data],
                   return_counts=True)[1]
     if np.any(_ < 5):
         return dense.fit(data)
     bow = BoW(lang=lang, key=mem.text,
               label_key=mem.label_header,
@@ -53,15 +53,14 @@
               voc_selection=mem.voc_selection)
     stack = StackGeneralization(decision_function_models=[bow, dense],
                                 decision_function_name=mem.decision_function_name,
                                 estimator_class=mem.estimator_class)
     return stack.fit(data)
     
 
-
 def active_learning_selection(mem: Config):
     db = CONFIG.db[mem[mem.username]]
     dense = model(mem, db[mem.permanent])  
     D = db[mem.data] + db.get(mem.original, list())
     hy = dense.decision_function(D)
     if len(mem[mem.labels]) > 2:
         index = np.arange(hy.shape[0])
@@ -75,32 +74,34 @@
         index = np.argsort(np.fabs(hy[:, 0]))[:mem.n_value]
         index.sort()
         labels = np.array(mem[mem.labels])
         klasses = labels[np.where(hy[:, 0][index] > 0, 1, 0)]
     data = []
     for cnt, i in enumerate(index):
         ele = D.pop(i - cnt)
-        ele[mem.label_header] = klasses[cnt]
+        ele[mem.label_header] = ele.get(mem.label_header, klasses[cnt])
         data.append(ele)
     db[mem.original] = D
     db[mem.data] = data
+    return dense
 
 
 def label_column_predict(mem: Config, model=None):
     db = CONFIG.db[mem[mem.username]]
     data = db[mem.data]
     if len(data) == 0 or np.all([has_label(mem, x) for x in data]):
         return   
     if mem.active_learning in mem and mem[mem.active_learning]:
         return active_learning_selection(mem)
     D = db[mem.permanent]
     dense = model(mem, D)    
     hys = dense.predict(data).tolist()
     for ele, hy in zip(data, hys):
-        ele[mem.label_header] = ele.get(mem.label_header, hy)        
+        ele[mem.label_header] = ele.get(mem.label_header, hy)
+    return dense        
 
 
 def label_column(mem: Config, model=model):
     db = CONFIG.db[mem[mem.username]]
     if mem.permanent in db:
         _ = np.unique([x[mem.label_header]
                        for x in db[mem.permanent]])
```

### Comparing `IngeoDash-0.1.1/IngeoDash/app.py` & `IngeoDash-0.1.2/IngeoDash/app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/config.py` & `IngeoDash-0.1.2/IngeoDash/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,27 +49,31 @@
     active_learning: str='active_learning'
     shuffle: str='shuffle'
     labels_proportion: str='labels_proportion'
     voc_size_exponent: int=15
     voc_selection: str='most_common_by_type'
     estimator_class: object=LinearSVC
     decision_function_name: str='decision_function'
+    dense_select: bool=True
 
 
     def __getitem__(self, key):
         return self.mem[key]
     
     def __setitem__(self, key, value):
         self.mem[key] = value
 
     def __call__(self, value):
         cls = deepcopy(self)
         if value is not None:
             cls.mem = json.loads(value) if isinstance(value, str) else value
-        for key in ['label_header', 'text', 'n_value']:
+        for key in ['label_header', 'text', 'n_value',
+                    'voc_size_exponent', 'voc_selection',
+                    'estimator_class', 'decision_function_name',
+                    'dense_select']:
             if key in cls.mem:
                 setattr(cls, key, cls.mem[key])
         return cls
     
     def __contains__(self, key):
         return key in self.mem
```

### Comparing `IngeoDash-0.1.1/IngeoDash/download.py` & `IngeoDash-0.1.2/IngeoDash/download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.1.2/IngeoDash/tests/test_annotate.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.annotate import label_column, flip_label, store, similarity
+from IngeoDash.annotate import label_column, flip_label, store, similarity, model
 from IngeoDash.config import CONFIG
 from microtc.utils import tweet_iterator
 from EvoMSA.tests.test_base import TWEETS
 from EvoMSA import DenseBoW
 import numpy as np
 
 
@@ -87,15 +87,14 @@
     db = CONFIG.db['xxx']
     permanent = db[mem.permanent]
     data = db[mem.data]
     assert [x['id'] for x in permanent] == list(range(10))
     assert [x['id'] for x in data] != list(range(10, 20))
     
 
-
 def test_flip_label():
     data = [dict() for i in range(3)]
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: data}
     db = CONFIG.db['xxx']
     label_column(mem)
     flip_label(mem, k=1)
@@ -121,8 +120,18 @@
 def test_similarity():
     tweets = [dict(nn=tweet['text']) 
               for tweet in tweet_iterator(TWEETS)]
     sim_values = similarity('estoy que muero de', tweets, key='nn')
     _ = sorted([[tweet['nn'], sim]for tweet, (sim, ) in zip(tweets, sim_values)],
                key=lambda x: x[1],
                reverse=True)
-    assert 'Me choca ahorita' in _[0][0]    
+    assert 'Me choca ahorita' in _[0][0]
+
+
+def test_stack_dense():
+    from EvoMSA import BoW, DenseBoW, StackGeneralization
+    mem = CONFIG({CONFIG.lang: 'es'})
+    D = list(tweet_iterator(TWEETS))
+    m = model(mem, D[:15])
+    assert isinstance(m, DenseBoW) and not isinstance(m, StackGeneralization)
+    m = model(mem, D)
+    assert isinstance(m, StackGeneralization)
```

### Comparing `IngeoDash-0.1.1/IngeoDash/tests/test_app.py` & `IngeoDash-0.1.2/IngeoDash/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/tests/test_config.py` & `IngeoDash-0.1.2/IngeoDash/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
+from sklearn.svm import LinearSVC
 
 
 def test_Config():
     conf = Config()
     default = dict(store='store',
                    labels='labels',
                    label_header='klass',
@@ -41,15 +42,20 @@
                    text='text',
                    mem={},
                    prev='previous',
                    batch_size='n_value',
                    checklist='checklist',
                    active_learning='active_learning',
                    shuffle='shuffle',
-                   labels_proportion='labels_proportion')
+                   labels_proportion='labels_proportion',
+                   voc_size_exponent=15,
+                   voc_selection='most_common_by_type',
+                   estimator_class=LinearSVC,
+                   decision_function_name='decision_function',
+                   dense_select=True)
     for k, v in default.items():
         assert v == getattr(conf, k)
 
 
 def test_Config_mem():
     config = Config()
 
@@ -66,17 +72,22 @@
     config['adios'] = 2
     assert 'adios' not in xxx
     xxx['xxx'] = 3
     assert mem['xxx'] == 3
 
 
 def test_Config_call2():
-    mem = CONFIG(dict(label_header='label',
-                      text='texto', n_value=12))
-    assert mem.label_header == 'label'
-    assert mem.text == 'texto'
-    assert mem.n_value == 12
+    kwargs = dict(label_header='label',
+                  text='texto', n_value=12,
+                  voc_size_exponent=15,
+                  voc_selection='most_common_by_type',
+                  estimator_class=LinearSVC,
+                  decision_function_name='decision_function',
+                  dense_select=True)
+    mem = CONFIG(kwargs)
+    for k, v in kwargs.items():
+        assert getattr(mem, k) == v
 
 
 def test_CONFIG():
     from IngeoDash.config import CONFIG
     assert isinstance(CONFIG, Config)
```

### Comparing `IngeoDash-0.1.1/IngeoDash/tests/test_download.py` & `IngeoDash-0.1.2/IngeoDash/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/tests/test_upload.py` & `IngeoDash-0.1.2/IngeoDash/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash/upload.py` & `IngeoDash-0.1.2/IngeoDash/upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.1.2/IngeoDash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.1.1
+Version: 0.1.2
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.1.1/LICENSE` & `IngeoDash-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/PKG-INFO` & `IngeoDash-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.1.1
+Version: 0.1.2
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.1.1/README.rst` & `IngeoDash-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.1/setup.py` & `IngeoDash-0.1.2/setup.py`

 * *Files identical despite different names*

