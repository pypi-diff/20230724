# Comparing `tmp/losscape-1.5.2.tar.gz` & `tmp/losscape-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.5.2.tar", last modified: Sat Jul 22 18:00:23 2023, max compression
+gzip compressed data, was "losscape-1.5.3.tar", last modified: Mon Jul 24 08:41:21 2023, max compression
```

## Comparing `losscape-1.5.2.tar` & `losscape-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 18:00:23.700175 losscape-1.5.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 18:00:23.700175 losscape-1.5.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 18:00:23.700175 losscape-1.5.2/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.2/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.2/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.2/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16290 2023-07-22 17:53:16.000000 losscape-1.5.2/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5.2/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-22 18:00:23.700175 losscape-1.5.2/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-22 18:00:23.000000 losscape-1.5.2/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-22 18:00:23.000000 losscape-1.5.2/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-22 18:00:23.000000 losscape-1.5.2/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-22 18:00:23.000000 losscape-1.5.2/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-22 18:00:23.000000 losscape-1.5.2/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-22 18:00:23.700175 losscape-1.5.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-22 18:00:16.000000 losscape-1.5.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 08:41:21.043837 losscape-1.5.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-24 08:41:21.043837 losscape-1.5.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 08:41:21.043837 losscape-1.5.3/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.3/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.3/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.3/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16383 2023-07-24 08:40:22.000000 losscape-1.5.3/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5.3/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 08:41:21.043837 losscape-1.5.3/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-24 08:41:21.000000 losscape-1.5.3/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-24 08:41:21.000000 losscape-1.5.3/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-24 08:41:21.000000 losscape-1.5.3/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-24 08:41:21.000000 losscape-1.5.3/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-24 08:41:21.000000 losscape-1.5.3/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-24 08:41:21.043837 losscape-1.5.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-24 08:40:39.000000 losscape-1.5.3/setup.py
```

### Comparing `losscape-1.5.2/PKG-INFO` & `losscape-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.2
+Version: 1.5.3
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.2/README.md` & `losscape-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.5.2/losscape/compute_loss.py` & `losscape-1.5.3/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.2/losscape/create_directions.py` & `losscape-1.5.3/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.2/losscape/create_landscape.py` & `losscape-1.5.3/losscape/create_landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,16 @@
     for i in range(X.shape[0]):
         for j in range(X.shape[1]):
             _set_weights(model, init_weights, directions, np.array([X[i, j], Y[i, j]]))
 
             loss = compute_loss(model, train_loader_unshuffled, get_batch, criterion, num_batches)
             losses[i, j] = loss
 
+            print("LOSS COMPUTED FOR x={} AND y={} IS : {}".format(X[i, j], Y[i, j], loss))
+
             count += 1
             if count%(total/10) == 0:
                 print("{}%".format(count/total * 100.))
 
     _reset_weights(model, init_weights)
 
     cp = plt.contour(X, Y, losses, cmap='summer')
```

### Comparing `losscape-1.5.2/losscape/train.py` & `losscape-1.5.3/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.2/losscape.egg-info/PKG-INFO` & `losscape-1.5.3/losscape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.2
+Version: 1.5.3
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.2/setup.py` & `losscape-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.5.2',
+    version='1.5.3',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

