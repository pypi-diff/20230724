# Comparing `tmp/easy_deployer-0.1.3.tar.gz` & `tmp/easy_deployer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_deployer-0.1.3.tar", last modified: Mon Jul 24 17:28:19 2023, max compression
+gzip compressed data, was "easy_deployer-0.1.4.tar", last modified: Mon Jul 24 19:54:09 2023, max compression
```

## Comparing `easy_deployer-0.1.3.tar` & `easy_deployer-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.590037 easy_deployer-0.1.3/
--rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2023-07-24 17:28:19.589039 easy_deployer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      185 2022-03-29 22:50:10.000000 easy_deployer-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.573083 easy_deployer-0.1.3/easy_deployer/
--rw-rw-rw-   0        0        0       90 2022-03-30 02:17:42.000000 easy_deployer-0.1.3/easy_deployer/__init__.py
--rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.3/easy_deployer/github.py
--rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.3/easy_deployer/heroku.py
--rw-rw-rw-   0        0        0     9149 2023-07-23 15:19:03.000000 easy_deployer-0.1.3/easy_deployer/main.py
--rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.3/easy_deployer/shared_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-24 17:28:19.588042 easy_deployer-0.1.3/easy_deployer.egg-info/
--rw-rw-rw-   0        0        0      766 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      156 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 17:28:19.000000 easy_deployer-0.1.3/easy_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 17:28:19.591034 easy_deployer-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-07-24 17:25:00.000000 easy_deployer-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.717932 easy_deployer-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2021-07-27 13:30:42.000000 easy_deployer-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      888 2023-07-24 19:54:08.716935 easy_deployer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-24 19:18:25.000000 easy_deployer-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.698983 easy_deployer-0.1.4/easy_deployer/
+-rw-rw-rw-   0        0        0       90 2023-07-24 19:21:46.000000 easy_deployer-0.1.4/easy_deployer/__init__.py
+-rw-rw-rw-   0        0        0    26588 2023-07-24 15:55:57.000000 easy_deployer-0.1.4/easy_deployer/github.py
+-rw-rw-rw-   0        0        0    11211 2023-07-23 15:15:38.000000 easy_deployer-0.1.4/easy_deployer/heroku.py
+-rw-rw-rw-   0        0        0     9304 2023-07-24 19:12:32.000000 easy_deployer-0.1.4/easy_deployer/main.py
+-rw-rw-rw-   0        0        0    12360 2023-07-23 15:28:41.000000 easy_deployer-0.1.4/easy_deployer/shared_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 19:54:08.715938 easy_deployer-0.1.4/easy_deployer.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      156 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-24 19:54:08.000000 easy_deployer-0.1.4/easy_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 19:54:08.718930 easy_deployer-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2023-07-24 19:52:04.000000 easy_deployer-0.1.4/setup.py
```

### Comparing `easy_deployer-0.1.3/LICENSE.txt` & `easy_deployer-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.3/PKG-INFO` & `easy_deployer-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: easy_deployer
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
-Author-email: namelowy_64@hotmail.com
+Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Easy-Deployer:
 Easy-deployer is used to simplify and speed up the deployment process.
 It's mostly still in progress...
 
+## Supported platforms to deploy to:
+- Github
+- ~~Heroku~~
+
 ## OS Support:
 Currently windows is the only supported os.
```

### Comparing `easy_deployer-0.1.3/easy_deployer/github.py` & `easy_deployer-0.1.4/easy_deployer/github.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.3/easy_deployer/heroku.py` & `easy_deployer-0.1.4/easy_deployer/heroku.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.3/easy_deployer/main.py` & `easy_deployer-0.1.4/easy_deployer/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,41 +25,45 @@
             "validate": lambda x: "Invalid path" if not os.path.exists(x) else True
         })["path"]
     elif not os.path.exists(args["path"]):
             print("Invalid path")
             sys.exit(5)
     additional_cmds = handle_additional_cmds(args)
     # runCmd(f"py easy_deployer/{args['to']}.py -p {args['path']} {additional_cmds}") # main command
-    args_to = f"easy-deployer-{args['to']}"
-    current_dir = os.path.dirname(__file__)
+    args_to = f"{args['to']}"
     """
         priorities of execution:
             ¤ this is .exe 
                 ¤ and executables are in same directory -> run 
                 ¤ and executables are not in the same directory 
                     -> run global executables (the ones in the path env variable)
             ¤ this is .py
                 ¤ and python (.py) package(s)/module(s) is in the same directory -> run those .py files
                 ¤ and python (.py) package(s)/module(s) is not in the same directory 
                     -> run global executables (the ones in the path env variable)
     """
     # main command
-    if(re.match(".+\.exe$", __file__)):
-        # This is Executable (*.exe)
-        if(args_to +".exe" in os.listdir(current_dir)):
+    if(getattr(sys, "frozen", False)):
+        current_dir = os.path.dirname(sys.executable)
+        print(current_dir, sys.executable)
+        if(f"easy-deployer-{args_to}.exe" in os.listdir(current_dir)):
             # if local file .exe is in the same directory then it will run it
             runCmd(f"{os.path.join(current_dir, args_to)}.exe -p {args['path']} {additional_cmds}")
         else:
             # else it runs the global one
             run_global_exe(args_to,args['path'],additional_cmds)
+    # if(re.match(".+\.exe$", __file__)):
+        # This is Executable (*.exe)
+        
     else:
+        current_dir = os.path.dirname(__file__)
         # Assuming this is a python file (.py)
-        if(args["to"]+".py" in os.listdir(current_dir)):
+        if(args_to+".py" in os.listdir(current_dir)):
             # if python (.py) package(s)/module(s) is in the same directory then it will run it
-            runCmd(f"py {os.path.join(current_dir, args['to'])}.py -p {args['path']} {additional_cmds}")
+            runCmd(f"py {os.path.join(current_dir, f'{args_to}')}.py -p {args['path']} {additional_cmds}")
         else:
             # else it runs the global one
             run_global_exe(args_to,args['path'],additional_cmds) 
 
 def run_global_exe(to, path, additional_cmds):
     runCmd(f"easy-deployer-{to} -p {path} {additional_cmds}")
```

### Comparing `easy_deployer-0.1.3/easy_deployer/shared_functions.py` & `easy_deployer-0.1.4/easy_deployer/shared_functions.py`

 * *Files identical despite different names*

### Comparing `easy_deployer-0.1.3/easy_deployer.egg-info/PKG-INFO` & `easy_deployer-0.1.4/easy_deployer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: easy-deployer
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/medamine980/easy-deployer
 Author: Mohamed-Amine Benali
-Author-email: namelowy_64@hotmail.com
+Author-email: benali.medamine2002@gmail.com
 License: MIT
 Keywords: python,github,github-deployer,heroku,heroku-deployer,deploy,easy,easy-deployer,simple,simple-deployer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Easy-Deployer:
 Easy-deployer is used to simplify and speed up the deployment process.
 It's mostly still in progress...
 
+## Supported platforms to deploy to:
+- Github
+- ~~Heroku~~
+
 ## OS Support:
 Currently windows is the only supported os.
```

### Comparing `easy_deployer-0.1.3/setup.py` & `easy_deployer-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_desc = f.read()
 setup(
     name="easy_deployer",
-    version="0.1.3",
+    version="0.1.4",
     long_description=long_desc,
     long_description_content_type='text/markdown',
     author="Mohamed-Amine Benali",
-    author_email="namelowy_64@hotmail.com",
+    author_email="benali.medamine2002@gmail.com",
     url="https://github.com/medamine980/easy-deployer",
-    
     packages=find_packages(exclude=["easy_deployer.dist", "easy_deployer.ignore"]),
     license="MIT",
     keywords=["python", "github", "github-deployer", "heroku", 
     "heroku-deployer", "deploy", "easy", "easy-deployer", "simple", "simple-deployer"],
     install_required=["pipreqs"],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6'
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.11'
     ],
     entry_points = {
         'console_scripts': [
             'easy-deployer = easy_deployer.main:main',
             'easy-deployer-github = easy_deployer.github:main',
             'easy-deployer-heroku = easy_deployer.heroku:main'
         ]
```

