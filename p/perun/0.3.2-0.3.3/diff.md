# Comparing `tmp/perun-0.3.2.tar.gz` & `tmp/perun-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun-0.3.2.tar", max compression
+gzip compressed data, was "perun-0.3.3.tar", max compression
```

## Comparing `perun-0.3.2.tar` & `perun-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1527 2023-06-02 08:25:25.606819 perun-0.3.2/LICENSE
--rw-r--r--   0        0        0     8581 2023-06-02 08:25:25.606819 perun-0.3.2/README.md
--rw-r--r--   0        0        0      319 2023-06-02 08:25:26.370831 perun-0.3.2/perun/__init__.py
--rw-r--r--   0        0        0       88 2023-06-02 08:25:25.606819 perun-0.3.2/perun/__main__.py
--rw-r--r--   0        0        0      190 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/__init__.py
--rw-r--r--   0        0        0     1963 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/backend.py
--rw-r--r--   0        0        0     7673 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/intel_rapl.py
--rw-r--r--   0        0        0     3404 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/nvml.py
--rw-r--r--   0        0        0     4435 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/psutil.py
--rw-r--r--   0        0        0     7550 2023-06-02 08:25:25.606819 perun-0.3.2/perun/cli.py
--rw-r--r--   0        0        0     1992 2023-06-02 08:25:25.606819 perun-0.3.2/perun/comm.py
--rw-r--r--   0        0        0     3044 2023-06-02 08:25:25.606819 perun-0.3.2/perun/configuration.py
--rw-r--r--   0        0        0     3793 2023-06-02 08:25:25.606819 perun-0.3.2/perun/coordination.py
--rw-r--r--   0        0        0       26 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/__init__.py
--rw-r--r--   0        0        0     7136 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/data.py
--rw-r--r--   0        0        0     1900 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/measurement_type.py
--rw-r--r--   0        0        0      988 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/sensor.py
--rw-r--r--   0        0        0      878 2023-06-02 08:25:25.606819 perun-0.3.2/perun/decorator.py
--rw-r--r--   0        0        0       21 2023-06-02 08:25:25.606819 perun-0.3.2/perun/extras/__init__.py
--rw-r--r--   0        0        0     1863 2023-06-02 08:25:25.606819 perun-0.3.2/perun/extras/horeka.py
--rw-r--r--   0        0        0       18 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/__init__.py
--rw-r--r--   0        0        0     1544 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/bench.py
--rw-r--r--   0        0        0     6458 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/hdf5.py
--rw-r--r--   0        0        0     4384 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/io.py
--rw-r--r--   0        0        0     1414 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/json.py
--rw-r--r--   0        0        0     2612 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/pandas.py
--rw-r--r--   0        0        0      536 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/pickle.py
--rw-r--r--   0        0        0     3983 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/text_report.py
--rw-r--r--   0        0        0      828 2023-06-02 08:25:25.606819 perun-0.3.2/perun/logging.py
--rw-r--r--   0        0        0    12011 2023-06-02 08:25:25.606819 perun-0.3.2/perun/perun.py
--rw-r--r--   0        0        0     7253 2023-06-02 08:25:25.606819 perun-0.3.2/perun/processing.py
--rw-r--r--   0        0        0     4189 2023-06-02 08:25:25.610819 perun-0.3.2/perun/util.py
--rw-r--r--   0        0        0     1873 2023-06-02 08:25:26.374831 perun-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9505 1970-01-01 00:00:00.000000 perun-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-07-24 14:52:05.806384 perun-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8734 2023-07-24 14:52:05.806384 perun-0.3.3/README.md
+-rw-r--r--   0        0        0      365 2023-07-24 14:52:05.806384 perun-0.3.3/perun/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-24 14:52:05.806384 perun-0.3.3/perun/__main__.py
+-rw-r--r--   0        0        0      190 2023-07-24 14:52:05.806384 perun-0.3.3/perun/backend/__init__.py
+-rw-r--r--   0        0        0     1963 2023-07-24 14:52:05.806384 perun-0.3.3/perun/backend/backend.py
+-rw-r--r--   0        0        0     7673 2023-07-24 14:52:05.810384 perun-0.3.3/perun/backend/intel_rapl.py
+-rw-r--r--   0        0        0     3420 2023-07-24 14:52:05.810384 perun-0.3.3/perun/backend/nvml.py
+-rw-r--r--   0        0        0     4435 2023-07-24 14:52:05.810384 perun-0.3.3/perun/backend/psutil.py
+-rw-r--r--   0        0        0     7550 2023-07-24 14:52:05.810384 perun-0.3.3/perun/cli.py
+-rw-r--r--   0        0        0     1992 2023-07-24 14:52:05.810384 perun-0.3.3/perun/comm.py
+-rw-r--r--   0        0        0     3044 2023-07-24 14:52:05.810384 perun-0.3.3/perun/configuration.py
+-rw-r--r--   0        0        0     3793 2023-07-24 14:52:05.810384 perun-0.3.3/perun/coordination.py
+-rw-r--r--   0        0        0       26 2023-07-24 14:52:05.810384 perun-0.3.3/perun/data_model/__init__.py
+-rw-r--r--   0        0        0     7136 2023-07-24 14:52:05.810384 perun-0.3.3/perun/data_model/data.py
+-rw-r--r--   0        0        0     1900 2023-07-24 14:52:05.810384 perun-0.3.3/perun/data_model/measurement_type.py
+-rw-r--r--   0        0        0      988 2023-07-24 14:52:05.810384 perun-0.3.3/perun/data_model/sensor.py
+-rw-r--r--   0        0        0      878 2023-07-24 14:52:05.810384 perun-0.3.3/perun/decorator.py
+-rw-r--r--   0        0        0       21 2023-07-24 14:52:05.810384 perun-0.3.3/perun/extras/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-24 14:52:05.810384 perun-0.3.3/perun/extras/horeka.py
+-rw-r--r--   0        0        0       18 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/__init__.py
+-rw-r--r--   0        0        0     1544 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/bench.py
+-rw-r--r--   0        0        0     6458 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/hdf5.py
+-rw-r--r--   0        0        0     4384 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/io.py
+-rw-r--r--   0        0        0     1414 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/json.py
+-rw-r--r--   0        0        0     2612 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/pandas.py
+-rw-r--r--   0        0        0      536 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/pickle.py
+-rw-r--r--   0        0        0     3983 2023-07-24 14:52:05.810384 perun-0.3.3/perun/io/text_report.py
+-rw-r--r--   0        0        0      828 2023-07-24 14:52:05.810384 perun-0.3.3/perun/logging.py
+-rw-r--r--   0        0        0    12039 2023-07-24 14:52:05.810384 perun-0.3.3/perun/perun.py
+-rw-r--r--   0        0        0     7253 2023-07-24 14:52:05.810384 perun-0.3.3/perun/processing.py
+-rw-r--r--   0        0        0     4189 2023-07-24 14:52:05.810384 perun-0.3.3/perun/util.py
+-rw-r--r--   0        0        0     1916 2023-07-24 14:52:06.934388 perun-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9660 1970-01-01 00:00:00.000000 perun-0.3.3/PKG-INFO
```

### Comparing `perun-0.3.2/LICENSE` & `perun-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/README.md` & `perun-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <div align="center">
   <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
 &nbsp;
 &nbsp;
 
-[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7253/badge)](https://bestpractices.coreinfrastructure.org/projects/7253)
 [![DOI](https://zenodo.org/badge/523363424.svg)](https://zenodo.org/badge/latestdoi/523363424)
 ![PyPI](https://img.shields.io/pypi/v/perun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `perun-0.3.2/perun/backend/backend.py` & `perun-0.3.3/perun/backend/backend.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/backend/intel_rapl.py` & `perun-0.3.3/perun/backend/intel_rapl.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/backend/nvml.py` & `perun-0.3.3/perun/backend/nvml.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 return np.uint32(pynvml.nvmlDeviceGetPowerUsage(handle))
 
             return func
 
         devices = []
         for deviceId in deviceList:
             try:
-                handle = pynvml.nvmlDeviceGetHandleByUUID(deviceId.encode())
+                handle = pynvml.nvmlDeviceGetHandleByUUID(deviceId)
                 index = pynvml.nvmlDeviceGetIndex(handle)
 
                 name = f"CUDA:{index}"
                 device_type = DeviceType.GPU
                 device_metadata = {
                     "uuid": deviceId,
                     "name": pynvml.nvmlDeviceGetName(handle),
@@ -102,14 +102,15 @@
                         device_type,
                         device_metadata,
                         data_type,
                         getCallback(handle),
                     )
                 )
             except NVMLError as e:
+                print(e)
                 log.warning(f"Could not find device {deviceId}")
                 log.warning(e)
 
         return devices
 
 
 NVMLBackend()
```

### Comparing `perun-0.3.2/perun/backend/psutil.py` & `perun-0.3.3/perun/backend/psutil.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/cli.py` & `perun-0.3.3/perun/cli.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/comm.py` & `perun-0.3.3/perun/comm.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/configuration.py` & `perun-0.3.3/perun/configuration.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/coordination.py` & `perun-0.3.3/perun/coordination.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/data_model/data.py` & `perun-0.3.3/perun/data_model/data.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/data_model/measurement_type.py` & `perun-0.3.3/perun/data_model/measurement_type.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/data_model/sensor.py` & `perun-0.3.3/perun/data_model/sensor.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/decorator.py` & `perun-0.3.3/perun/decorator.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/extras/horeka.py` & `perun-0.3.3/perun/extras/horeka.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/bench.py` & `perun-0.3.3/perun/io/bench.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/hdf5.py` & `perun-0.3.3/perun/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/io.py` & `perun-0.3.3/perun/io/io.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/json.py` & `perun-0.3.3/perun/io/json.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/pandas.py` & `perun-0.3.3/perun/io/pandas.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/pickle.py` & `perun-0.3.3/perun/io/pickle.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/io/text_report.py` & `perun-0.3.3/perun/io/text_report.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/logging.py` & `perun-0.3.3/perun/logging.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/perun.py` & `perun-0.3.3/perun/perun.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
         sampling_rate (int): Sampling rate in s
     """
     from perun.backend import backends
 
     lSensors: List[Sensor] = []
     for backend in backends:
         if backend.name in backendConfig:
+            backend.setup()
             lSensors += backend.getSensors(backendConfig[backend.name])
 
     timesteps = []
     t_mT = MetricMetaData(
         Unit.SECOND,
         Magnitude.ONE,
         np.dtype("float32"),
```

### Comparing `perun-0.3.2/perun/processing.py` & `perun-0.3.3/perun/processing.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/perun/util.py` & `perun-0.3.3/perun/util.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.2/pyproject.toml` & `perun-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "perun"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Gutiérrez Hermosillo Muriedas, Juan Pedro <juanpedroghm@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Helmholtz-AI-Energy/perun"
 
 [tool.poetry.scripts]
 perun = "perun.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-pynvml = "^11.0.0"
 click = "^8.0.0"
-py-cpuinfo = "^5.0.0"
+py-cpuinfo = ">=5.0.0"
 numpy = "^1.20.0"
 psutil = "^5.9.0"
 h5py = "^3.5.9"
 pandas = ">=1.3"
+nvidia-ml-py = "^12.535.77"
 
 [tool.poetry.extras]
 dev = ["pytest", "flake8", "mypy", "black", "pre-commit", "pytest-cov"]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autoapi"]
 mpi = ["mpi4py"]
 
 [tool.poetry.group.dev]
@@ -53,24 +53,23 @@
 # [tool.poetry.group.horeka]
 # optional = true
 #
 # [tool.poetry.group.horeka.dependencies]
 # influxdb-client = "*"
 
 [tool.semantic_release]
-version_variable = [
-    "perun/__init__.py:__version__",
-    "pyproject.toml:version"
-]
-branch = "release"
-upload_to_pypi = true
-upload_to_release = true
+version_variable = [ "perun/__init__.py:__version__" ]
+version_toml = ["pyproject.toml:tool.poetry.version"]
 commit_message = "{version} [skip ci]"
 build_command = "pip install poetry && poetry build"
 
+[tool.semantic_release.branches.release]
+match = "release"
+prerelease = false
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.isort]
 skip = ["perun/__init__.py"]
 known_third_party = ["click", "cpuinfo", "h5py", "influxdb_client", "numpy", "pandas", "psutil", "pynvml", "pytest"]
 profile = "black"
```

### Comparing `perun-0.3.2/PKG-INFO` & `perun-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Home-page: https://github.com/Helmholtz-AI-Energy/perun
 License: BSD-3-Clause
 Author: Gutiérrez Hermosillo Muriedas, Juan Pedro
 Author-email: juanpedroghm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -15,28 +15,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: mpi
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: h5py (>=3.5.9,<4.0.0)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
+Requires-Dist: nvidia-ml-py (>=12.535.77,<13.0.0)
 Requires-Dist: pandas (>=1.3)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
-Requires-Dist: py-cpuinfo (>=5.0.0,<6.0.0)
-Requires-Dist: pynvml (>=11.0.0,<12.0.0)
+Requires-Dist: py-cpuinfo (>=5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
 &nbsp;
 &nbsp;
 
-[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7253/badge)](https://bestpractices.coreinfrastructure.org/projects/7253)
 [![DOI](https://zenodo.org/badge/523363424.svg)](https://zenodo.org/badge/latestdoi/523363424)
 ![PyPI](https://img.shields.io/pypi/v/perun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
```

