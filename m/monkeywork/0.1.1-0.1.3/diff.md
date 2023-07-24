# Comparing `tmp/monkeywork-0.1.1.tar.gz` & `tmp/monkeywork-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkeywork-0.1.1.tar", last modified: Sun Jul 23 11:51:03 2023, max compression
+gzip compressed data, was "monkeywork-0.1.3.tar", last modified: Mon Jul 24 01:11:22 2023, max compression
```

## Comparing `monkeywork-0.1.1.tar` & `monkeywork-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 11:51:03.050101 monkeywork-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-07-23 11:00:58.000000 monkeywork-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     2643 2023-07-23 11:51:03.050101 monkeywork-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2177 2023-07-23 11:48:49.000000 monkeywork-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 11:51:03.038807 monkeywork-0.1.1/monkeywork/
--rw-rw-rw-   0        0        0        0 2023-07-23 10:15:15.000000 monkeywork-0.1.1/monkeywork/__init__.py
--rw-rw-rw-   0        0        0     9657 2023-07-23 11:07:50.000000 monkeywork-0.1.1/monkeywork/monkeywork.py
-drwxrwxrwx   0        0        0        0 2023-07-23 11:51:03.048905 monkeywork-0.1.1/monkeywork.egg-info/
--rw-rw-rw-   0        0        0     2643 2023-07-23 11:51:02.000000 monkeywork-0.1.1/monkeywork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-23 11:51:03.000000 monkeywork-0.1.1/monkeywork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 11:51:02.000000 monkeywork-0.1.1/monkeywork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-23 11:51:02.000000 monkeywork-0.1.1/monkeywork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 11:51:03.050101 monkeywork-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-07-23 11:50:23.000000 monkeywork-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:22.027529 monkeywork-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-23 11:00:58.000000 monkeywork-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0     2675 2023-07-24 01:11:22.026470 monkeywork-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2023-07-24 01:10:33.000000 monkeywork-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:22.014117 monkeywork-0.1.3/monkeywork/
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:15:15.000000 monkeywork-0.1.3/monkeywork/__init__.py
+-rw-rw-rw-   0        0        0     9714 2023-07-24 01:09:29.000000 monkeywork-0.1.3/monkeywork/monkeywork.py
+drwxrwxrwx   0        0        0        0 2023-07-24 01:11:22.026470 monkeywork-0.1.3/monkeywork.egg-info/
+-rw-rw-rw-   0        0        0     2675 2023-07-24 01:11:21.000000 monkeywork-0.1.3/monkeywork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-24 01:11:21.000000 monkeywork-0.1.3/monkeywork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 01:11:21.000000 monkeywork-0.1.3/monkeywork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-24 01:11:21.000000 monkeywork-0.1.3/monkeywork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 01:11:22.027529 monkeywork-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-07-24 01:03:54.000000 monkeywork-0.1.3/setup.py
```

### Comparing `monkeywork-0.1.1/LICENCE` & `monkeywork-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `monkeywork-0.1.1/PKG-INFO` & `monkeywork-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkeywork
-Version: 0.1.1
+Version: 0.1.3
 Summary: Write and edit random files in a given directory
 Home-page: https://github.com/pylomatic/monkeywork
 Author: Pylomatic
 Author-email: pylomatic@conelab.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,28 +32,29 @@
 
 ## !!! CAUTION !!!
 
 The program can and will destroy files in the selected work directory. Be sure to select a dedicated work directory and **review the code before executing it on your system**!
 
 ## Run in console
 
-You can run the `monkeywork.py`directly from from the console with:
+You can run the `monkeywork.py` directly from from the console with:
 
 ```bash
 python monkeywork.py "<Path to your workdir>" [OPTIONS]
 ```
 
 example:
 ```bash
 python monkeywork.py "L:\monkeywork-test\"
 ```
 
 Options are:
 
 -f | force selected direcotry and delete all contents in set directory
+-y | skip start confirmation
 
 ## Installation
 
 Use it as a package
 
 ```bash
 pip install monkeywork
@@ -75,8 +76,8 @@
 |workdir:str| must be set to a valid path |
 |interval_min_s:float | shortest interval |
 |interval_max_s:float | longest interval |
 |max_file_size_mb:int | maximum file size in MB |
 |max_file_amount:int | maximumg file count
 |target_file_amount:int | program targets this amount of files |
 |path_length_limit:int | program should not exceed set path length |
-|logging_to_file_enabled:bool | enable loggin to file |
+|logging_to_file_enabled:bool | enable logging to file |
```

### Comparing `monkeywork-0.1.1/README.md` & `monkeywork-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 
 ## !!! CAUTION !!!
 
 The program can and will destroy files in the selected work directory. Be sure to select a dedicated work directory and **review the code before executing it on your system**!
 
 ## Run in console
 
-You can run the `monkeywork.py`directly from from the console with:
+You can run the `monkeywork.py` directly from from the console with:
 
 ```bash
 python monkeywork.py "<Path to your workdir>" [OPTIONS]
 ```
 
 example:
 ```bash
 python monkeywork.py "L:\monkeywork-test\"
 ```
 
 Options are:
 
 -f | force selected direcotry and delete all contents in set directory
+-y | skip start confirmation
 
 ## Installation
 
 Use it as a package
 
 ```bash
 pip install monkeywork
@@ -61,8 +62,8 @@
 |workdir:str| must be set to a valid path |
 |interval_min_s:float | shortest interval |
 |interval_max_s:float | longest interval |
 |max_file_size_mb:int | maximum file size in MB |
 |max_file_amount:int | maximumg file count
 |target_file_amount:int | program targets this amount of files |
 |path_length_limit:int | program should not exceed set path length |
-|logging_to_file_enabled:bool | enable loggin to file |
+|logging_to_file_enabled:bool | enable logging to file |
```

### Comparing `monkeywork-0.1.1/monkeywork/monkeywork.py` & `monkeywork-0.1.3/monkeywork/monkeywork.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,27 +231,28 @@
                 logger.handlers.clear()
                 logging.shutdown()
                 exit()
 
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         if os.path.exists(sys.argv[1]):
-            if sys.argv[1][0] == '"' and sys.argv[1][-1] == '"':
-                workdir = Path(sys.argv[1])
-            else:
-                print(f"Use Quotation marks for your path. Ex. \"L:\\monkey work\\test\\\"")
-                exit()
+            workdir = Path(sys.argv[1])
 
             if not os.listdir(workdir) or '-f' in sys.argv[2:]:
                 print (f"Target directory is empty or '-f' was set. {workdir} will be used\n!! FILES IN TARGET DIRECTORY WILL BE DELETED !!")
-                sleep(5)
-
-                monkey = Monkey(workdir=workdir)
-                print ("start")
-                monkey.run()
+                if '-y' in sys.argv[2:]:
+                    monkey = Monkey(workdir=workdir)
+                    print ("start")
+                    monkey.run()
+                elif input("Type 'y' to confirm...") == 'y':
+                    monkey = Monkey(workdir=workdir)
+                    print ("start")
+                    monkey.run()
+                else:
+                    exit()
 
             else:
                 print(f"Target directory is not empty!\nUse empty target or option '-f'\n!! FILES IN TARGET DIRECTORY WILL BE DELETED !!")
                 exit()
         else:
             print ("The target direcotry does not exists")
             exit()
```

### Comparing `monkeywork-0.1.1/monkeywork.egg-info/PKG-INFO` & `monkeywork-0.1.3/monkeywork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkeywork
-Version: 0.1.1
+Version: 0.1.3
 Summary: Write and edit random files in a given directory
 Home-page: https://github.com/pylomatic/monkeywork
 Author: Pylomatic
 Author-email: pylomatic@conelab.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,28 +32,29 @@
 
 ## !!! CAUTION !!!
 
 The program can and will destroy files in the selected work directory. Be sure to select a dedicated work directory and **review the code before executing it on your system**!
 
 ## Run in console
 
-You can run the `monkeywork.py`directly from from the console with:
+You can run the `monkeywork.py` directly from from the console with:
 
 ```bash
 python monkeywork.py "<Path to your workdir>" [OPTIONS]
 ```
 
 example:
 ```bash
 python monkeywork.py "L:\monkeywork-test\"
 ```
 
 Options are:
 
 -f | force selected direcotry and delete all contents in set directory
+-y | skip start confirmation
 
 ## Installation
 
 Use it as a package
 
 ```bash
 pip install monkeywork
@@ -75,8 +76,8 @@
 |workdir:str| must be set to a valid path |
 |interval_min_s:float | shortest interval |
 |interval_max_s:float | longest interval |
 |max_file_size_mb:int | maximum file size in MB |
 |max_file_amount:int | maximumg file count
 |target_file_amount:int | program targets this amount of files |
 |path_length_limit:int | program should not exceed set path length |
-|logging_to_file_enabled:bool | enable loggin to file |
+|logging_to_file_enabled:bool | enable logging to file |
```

### Comparing `monkeywork-0.1.1/setup.py` & `monkeywork-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="monkeywork",
-    version="0.1.1",
+    version="0.1.3",
     packages=find_packages(),
     author="Pylomatic",
     author_email="pylomatic@conelab.ch",
     description="Write and edit random files in a given directory",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/pylomatic/monkeywork",
```

