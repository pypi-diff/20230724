# Comparing `tmp/api4jenkins-1.9.tar.gz` & `tmp/api4jenkins-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api4jenkins-1.9.tar", last modified: Sat Mar 12 09:29:20 2022, max compression
+gzip compressed data, was "api4jenkins-1.9.1.tar", last modified: Tue Mar 29 02:49:05 2022, max compression
```

## Comparing `api4jenkins-1.9.tar` & `api4jenkins-1.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 09:29:20.637009 api4jenkins-1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-12 09:29:06.000000 api4jenkins-1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-12 09:29:20.637009 api4jenkins-1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-03-12 09:29:06.000000 api4jenkins-1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 09:29:20.637009 api4jenkins-1.9/api4jenkins/
--rw-r--r--   0 runner    (1001) docker     (121)    11252 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/credential.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/item.py
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/mix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4754 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/report.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/requester.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-03-12 09:29:06.000000 api4jenkins-1.9/api4jenkins/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 09:29:20.637009 api4jenkins-1.9/api4jenkins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-12 09:29:20.000000 api4jenkins-1.9/api4jenkins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-12 09:29:20.000000 api4jenkins-1.9/api4jenkins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 09:29:20.000000 api4jenkins-1.9/api4jenkins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-12 09:29:20.000000 api4jenkins-1.9/api4jenkins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-12 09:29:20.000000 api4jenkins-1.9/api4jenkins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-12 09:29:20.637009 api4jenkins-1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-03-12 09:29:06.000000 api4jenkins-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 02:49:05.820314 api4jenkins-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-03-29 02:49:05.816314 api4jenkins-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 02:49:05.816314 api4jenkins-1.9.1/api4jenkins/
+-rw-r--r--   0 runner    (1001) docker     (121)    11284 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/credential.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/item.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/mix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4754 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/requester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/api4jenkins/view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-29 02:49:05.816314 api4jenkins-1.9.1/api4jenkins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-03-29 02:49:05.000000 api4jenkins-1.9.1/api4jenkins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-29 02:49:05.000000 api4jenkins-1.9.1/api4jenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-29 02:49:05.000000 api4jenkins-1.9.1/api4jenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-03-29 02:49:05.000000 api4jenkins-1.9.1/api4jenkins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-29 02:49:05.000000 api4jenkins-1.9.1/api4jenkins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-29 02:49:05.820314 api4jenkins-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-03-29 02:48:53.000000 api4jenkins-1.9.1/setup.py
```

### Comparing `api4jenkins-1.9/LICENSE` & `api4jenkins-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/PKG-INFO` & `api4jenkins-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api4jenkins
-Version: 1.9
+Version: 1.9.1
 Summary: Jenkins Python Client
 Home-page: https://github.com/joelee2012/api4jenkins
 Author: Joe Lee
 Author-email: lj_2005@163.com
 License: Apache 2.0
 Project-URL: Documentation, https://api4jenkins.readthedocs.io
 Project-URL: Source, https://github.com/joelee2012/api4jenkins
```

### Comparing `api4jenkins-1.9/README.md` & `api4jenkins-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/__init__.py` & `api4jenkins-1.9.1/api4jenkins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             >>> from api4jenkins import Jenkins
             >>> j = Jenkins('http://127.0.0.1:8080/', auth=('admin', 'admin'))
             >>> job = j.get_job('freestylejob')
             >>> print(job)
             <FreeStyleProject: http://127.0.0.1:8080/job/freestylejob/>
         '''
         folder, name = self._resolve_name(full_name)
-        return folder.get(name)
+        if folder.exists():
+            return folder.get(name)
 
     def iter_jobs(self, depth=0):
         '''Iterate jobs with depth
 
         :param depth: ``int``, depth to iterate, default is 0
         :returns: iterator of jobs
```

### Comparing `api4jenkins-1.9/api4jenkins/artifact.py` & `api4jenkins-1.9.1/api4jenkins/artifact.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/build.py` & `api4jenkins-1.9.1/api4jenkins/build.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/credential.py` & `api4jenkins-1.9.1/api4jenkins/credential.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/input.py` & `api4jenkins-1.9.1/api4jenkins/input.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/item.py` & `api4jenkins-1.9.1/api4jenkins/item.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/job.py` & `api4jenkins-1.9.1/api4jenkins/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,30 +104,30 @@
     def __call__(self, depth):
         yield from self.iter(depth)
 
     def __getitem__(self, name):
         return self.get(name)
 
 
-class OrganizationFolder(Folder):
-    pass
-
-
 class WorkflowMultiBranchProject(Folder, EnableMixIn):
 
     def scan(self, delay=0):
         return self.handle_req('POST', 'build', params={'delay': delay})
 
     def get_scan_log(self, stream=False):
         with self.handle_req('GET', 'indexing/consoleText',
                              stream=stream) as resp:
             for line in resp.iter_lines():
                 yield line
 
 
+class OrganizationFolder(WorkflowMultiBranchProject):
+    pass
+
+
 class Project(Job, EnableMixIn):
 
     def __init__(self, jenkins, url):
         super().__init__(jenkins, url)
 
         def _get_build_by_key(key):
             item = self.api_json(tree=f'{key}[url]')[key]
```

### Comparing `api4jenkins-1.9/api4jenkins/mix.py` & `api4jenkins-1.9.1/api4jenkins/mix.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/node.py` & `api4jenkins-1.9.1/api4jenkins/node.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/plugin.py` & `api4jenkins-1.9.1/api4jenkins/plugin.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/queue.py` & `api4jenkins-1.9.1/api4jenkins/queue.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/report.py` & `api4jenkins-1.9.1/api4jenkins/report.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/requester.py` & `api4jenkins-1.9.1/api4jenkins/requester.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/system.py` & `api4jenkins-1.9.1/api4jenkins/system.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/user.py` & `api4jenkins-1.9.1/api4jenkins/user.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins/view.py` & `api4jenkins-1.9.1/api4jenkins/view.py`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/api4jenkins.egg-info/PKG-INFO` & `api4jenkins-1.9.1/api4jenkins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api4jenkins
-Version: 1.9
+Version: 1.9.1
 Summary: Jenkins Python Client
 Home-page: https://github.com/joelee2012/api4jenkins
 Author: Joe Lee
 Author-email: lj_2005@163.com
 License: Apache 2.0
 Project-URL: Documentation, https://api4jenkins.readthedocs.io
 Project-URL: Source, https://github.com/joelee2012/api4jenkins
```

### Comparing `api4jenkins-1.9/api4jenkins.egg-info/SOURCES.txt` & `api4jenkins-1.9.1/api4jenkins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api4jenkins-1.9/setup.py` & `api4jenkins-1.9.1/setup.py`

 * *Files identical despite different names*

