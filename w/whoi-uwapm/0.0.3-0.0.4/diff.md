# Comparing `tmp/whoi_uwapm-0.0.3.tar.gz` & `tmp/whoi_uwapm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoi_uwapm-0.0.3.tar", last modified: Fri Jul 14 14:42:25 2023, max compression
+gzip compressed data, was "whoi_uwapm-0.0.4.tar", last modified: Mon Jul 24 15:23:45 2023, max compression
```

## Comparing `whoi_uwapm-0.0.3.tar` & `whoi_uwapm-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-14 14:42:25.640285 whoi_uwapm-0.0.3/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1496 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.3/LICENSE
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       16 2023-07-13 21:01:53.000000 whoi_uwapm-0.0.3/MANIFEST.in
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1830 2023-07-14 14:42:25.640285 whoi_uwapm-0.0.3/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1579 2023-07-13 21:31:09.000000 whoi_uwapm-0.0.3/README.md
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-14 14:42:25.640285 whoi_uwapm-0.0.3/setup.cfg
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      472 2023-07-14 14:41:39.000000 whoi_uwapm-0.0.3/setup.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-14 14:42:25.640285 whoi_uwapm-0.0.3/whoi_uwapm/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-13 21:08:51.000000 whoi_uwapm-0.0.3/whoi_uwapm/__init__.py
--rwxrwxr-x   0 brennan   (1000) brennan   (1000)  5740896 2023-07-13 21:26:48.000000 whoi_uwapm-0.0.3/whoi_uwapm/bellhopcxx
--rw-rw-r--   0 brennan   (1000) brennan   (1000)    24905 2023-07-13 21:20:43.000000 whoi_uwapm-0.0.3/whoi_uwapm/uwapm.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-14 14:42:25.640285 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1830 2023-07-14 14:42:25.000000 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      272 2023-07-14 14:42:25.000000 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/SOURCES.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-14 14:42:25.000000 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/dependency_links.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-14 14:42:25.000000 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/requires.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       11 2023-07-14 14:42:25.000000 whoi_uwapm-0.0.3/whoi_uwapm.egg-info/top_level.txt
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-24 15:23:45.738774 whoi_uwapm-0.0.4/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1496 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.4/LICENSE
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       16 2023-07-13 21:01:53.000000 whoi_uwapm-0.0.4/MANIFEST.in
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     2478 2023-07-24 15:23:45.738774 whoi_uwapm-0.0.4/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     2227 2023-07-24 15:10:33.000000 whoi_uwapm-0.0.4/README.md
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-24 15:23:45.738774 whoi_uwapm-0.0.4/setup.cfg
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      483 2023-07-24 15:23:39.000000 whoi_uwapm-0.0.4/setup.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-24 15:23:45.738774 whoi_uwapm-0.0.4/whoi_uwapm/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-13 21:08:51.000000 whoi_uwapm-0.0.4/whoi_uwapm/__init__.py
+-rwxrwxr-x   0 brennan   (1000) brennan   (1000)   552336 2023-07-24 15:09:10.000000 whoi_uwapm-0.0.4/whoi_uwapm/bellhop
+-rwxrwxr-x   0 brennan   (1000) brennan   (1000)  5740896 2023-07-24 15:08:46.000000 whoi_uwapm-0.0.4/whoi_uwapm/bellhopcxx
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)    24989 2023-07-24 15:19:58.000000 whoi_uwapm-0.0.4/whoi_uwapm/uwapm.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-24 15:23:45.738774 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     2478 2023-07-24 15:23:45.000000 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      291 2023-07-24 15:23:45.000000 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-24 15:23:45.000000 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-24 15:23:45.000000 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/requires.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       11 2023-07-24 15:23:45.000000 whoi_uwapm-0.0.4/whoi_uwapm.egg-info/top_level.txt
```

### Comparing `whoi_uwapm-0.0.3/LICENSE` & `whoi_uwapm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whoi_uwapm-0.0.3/PKG-INFO` & `whoi_uwapm-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,16 @@
-Metadata-Version: 2.1
-Name: whoi_uwapm
-Version: 0.0.3
-Summary: WHOI Acomms Group uwapm
-Home-page: https://git.whoi.edu/acomms/whoi_uwapm
-Author: WHOI Acomms Group
-License: BSD (3-clause)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # <b>whoi_uwapm</b>
 
 ## <b> Introduction </b>
 whoi_uwapm is a fork of arlpy's uwapm module. It removes all of the graphing features of the original uwapm, and also is updated to support the latest versions of numpy, scipy, and pandas.
 
 ## PyPI
 The PyPI package contains an x86_64 binary of bellhopcuda. If you are using a different architecture, you will need to build bellhopcuda manually.
 
-## Automated building of bellhopcuda
+## Automated building of bellhopcuda and fortran bellhop
 The build.bash script included in this repo can be used to build bellhopcuda
 - Clone whoi_uwapm and navigate to it
 - `./build.bash`
 
 ## Manually building bellhopcuda
 - Clone whoi_uwapm
 - Clone bellhopcuda
@@ -37,11 +27,27 @@
 	- `cmake . -D BHC_ENABLE_CUDA=OFF`
 # Build
 - Run make inside the bellhopcuda directory
 	- `make bellhopcxx`
 
 # Install
 - Move the bellhopcxx binary to the whoi_uwapm directory
-    - `mv bin/bellhopcxx ../whoi_uwapm/whoi_uwapm/`
+    - `mv bin/bellhopcxx ../whoi_uwapm/bellhopcxx`
         - This will need to be adjusted based on where you cloned whoi_uwapm
         - If you cloned bellhopcuda inside of the whoi_uwapm directory, make sure to move it or delete it before running pip install.
     - `pip install .`
+
+## Manually building fortran bellhop
+- Clone whoi_uwapm
+- Clone accoustic_toolbox
+    - `git clone https://git.whoi.edu/dgiaya/acoustic_toolbox.git`
+- Install gfortran
+    - `sudo apt-get install gfortran -y`
+- Run make inside the acoustic_toolbox directory
+	- `make`
+
+# Install
+- Move the bellhopcxx binary to the whoi_uwapm directory
+    - `mv Bellhop/bellhop.exe ../whoi_uwapm/bellhop`
+        - This will need to be adjusted based on where you cloned whoi_uwapm
+        - If you cloned accoustic_toolbox inside of the whoi_uwapm directory, make sure to move it or delete it before running pip install.
+    - `pip install .`
```

### Comparing `whoi_uwapm-0.0.3/README.md` & `whoi_uwapm-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+Metadata-Version: 2.1
+Name: whoi_uwapm
+Version: 0.0.4
+Summary: WHOI Acomms Group uwapm
+Home-page: https://git.whoi.edu/acomms/whoi_uwapm
+Author: WHOI Acomms Group
+License: BSD (3-clause)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # <b>whoi_uwapm</b>
 
 ## <b> Introduction </b>
 whoi_uwapm is a fork of arlpy's uwapm module. It removes all of the graphing features of the original uwapm, and also is updated to support the latest versions of numpy, scipy, and pandas.
 
 ## PyPI
 The PyPI package contains an x86_64 binary of bellhopcuda. If you are using a different architecture, you will need to build bellhopcuda manually.
 
-## Automated building of bellhopcuda
+## Automated building of bellhopcuda and fortran bellhop
 The build.bash script included in this repo can be used to build bellhopcuda
 - Clone whoi_uwapm and navigate to it
 - `./build.bash`
 
 ## Manually building bellhopcuda
 - Clone whoi_uwapm
 - Clone bellhopcuda
@@ -27,11 +37,27 @@
 	- `cmake . -D BHC_ENABLE_CUDA=OFF`
 # Build
 - Run make inside the bellhopcuda directory
 	- `make bellhopcxx`
 
 # Install
 - Move the bellhopcxx binary to the whoi_uwapm directory
-    - `mv bin/bellhopcxx ../whoi_uwapm/whoi_uwapm/`
+    - `mv bin/bellhopcxx ../whoi_uwapm/bellhopcxx`
         - This will need to be adjusted based on where you cloned whoi_uwapm
         - If you cloned bellhopcuda inside of the whoi_uwapm directory, make sure to move it or delete it before running pip install.
-    - `pip install .`
+    - `pip install .`
+
+## Manually building fortran bellhop
+- Clone whoi_uwapm
+- Clone accoustic_toolbox
+    - `git clone https://git.whoi.edu/dgiaya/acoustic_toolbox.git`
+- Install gfortran
+    - `sudo apt-get install gfortran -y`
+- Run make inside the acoustic_toolbox directory
+	- `make`
+
+# Install
+- Move the bellhopcxx binary to the whoi_uwapm directory
+    - `mv Bellhop/bellhop.exe ../whoi_uwapm/bellhop`
+        - This will need to be adjusted based on where you cloned whoi_uwapm
+        - If you cloned accoustic_toolbox inside of the whoi_uwapm directory, make sure to move it or delete it before running pip install.
+    - `pip install .`
```

### Comparing `whoi_uwapm-0.0.3/whoi_uwapm/bellhopcxx` & `whoi_uwapm-0.0.4/whoi_uwapm/bellhopcxx`

 * *Files identical despite different names*

### Comparing `whoi_uwapm-0.0.3/whoi_uwapm/uwapm.py` & `whoi_uwapm-0.0.4/whoi_uwapm/uwapm.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,28 +272,28 @@
             rv.append(m[0])
     return rv
 
 def _select_model(env, task, model):
     if model is not None:
         for m in _models:
             if m[0] == model:
-                return (m[0], m[1]())
+                return (m[0], m[1](m[0]))
         raise ValueError('Unknown model: '+model)
     for m in _models:
         mm = m[1]()
         if mm.supports(env, task):
             return (m[0], mm)
     raise ValueError('No suitable propagation model available')
 
 ### Bellhop propagation model ###
 
 class _Bellhop:
 
-    def __init__(self):
-        pass
+    def __init__(self, model_name):
+        self.model_name = model_name
 
     def supports(self, env=None, task=None):
         if env is not None and env['type'] != '2D':
             return False
         fh, fname = _mkstemp(suffix='.env')
         _os.close(fh)
         fname_base = fname[:-4]
@@ -336,15 +336,15 @@
             self._unlink(fname_base+'.arr')
             self._unlink(fname_base+'.ray')
             self._unlink(fname_base+'.shd')
         return results
 
     def _bellhop(self, *args):
         try: 
-            bellhop_file_path = _os.path.join(_os.path.dirname(__file__), 'bellhopcxx')
+            bellhop_file_path = _os.path.join(_os.path.dirname(__file__), self.model_name)
             _proc.run(f'{bellhop_file_path} {" ".join(list(args))}', 
                       stderr=_proc.STDOUT, stdout=_proc.PIPE,
                       shell=True)
         except OSError:
             return False
         return True
 
@@ -562,8 +562,9 @@
             for ird in range(nrd):
                 recnum = 10 + ird
                 f.seek(recnum*4*recl, 0)
                 temp = _np.array(_unpack('f'*2*nrr, f.read(2*nrr*4)))
                 pressure[ird,:] = temp[::2] + 1j*temp[1::2]
         return _pd.DataFrame(pressure, index=pos_r_depth, columns=pos_r_range)
 
-_models.append(('bellhop', _Bellhop))
+_models.append(('bellhop', _Bellhop))
+_models.append(('bellhopcxx', _Bellhop))
```

