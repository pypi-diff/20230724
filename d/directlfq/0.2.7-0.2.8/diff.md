# Comparing `tmp/directlfq-0.2.7.tar.gz` & `tmp/directlfq-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directlfq-0.2.7.tar", last modified: Tue Feb 28 17:29:02 2023, max compression
+gzip compressed data, was "directlfq-0.2.8.tar", last modified: Wed Mar  1 11:09:25 2023, max compression
```

## Comparing `directlfq-0.2.7.tar` & `directlfq-0.2.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.828447 directlfq-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-28 17:28:40.000000 directlfq-0.2.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-02-28 17:28:40.000000 directlfq-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-28 17:28:40.000000 directlfq-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-02-28 17:29:02.828447 directlfq-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-02-28 17:28:40.000000 directlfq-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.816447 directlfq-0.2.7/directlfq/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.820447 directlfq-0.2.7/directlfq/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)   111485 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (123)    30415 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.824447 directlfq-0.2.7/directlfq/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/download_links_for_testfiles_all.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/download_links_for_testfiles_quicktest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/intable_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/interface_parameters.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    22544 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_fragion.rs
--rwxr-xr-x   0 runner    (1001) docker     (123)    20608 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_precursor.rs
--rwxr-xr-x   0 runner    (1001) docker     (123)    22528 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_ptm_fragion.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/dashboard_parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.824447 directlfq-0.2.7/directlfq/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14186 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/docs/Empty_manual.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/gui_textfields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.828447 directlfq-0.2.7/directlfq/img/
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/img/github.png
--rw-r--r--   0 runner    (1001) docker     (123)   108120 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/img/max-planck-gesellschaft.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1317924 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/img/mpi_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   522703 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/img/ms_pipeline_visualization.png
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/lfq_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/protein_intensity_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.828447 directlfq-0.2.7/directlfq/style/
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/style/dashboard_style.css
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/testfile_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    53543 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-02-28 17:28:40.000000 directlfq-0.2.7/directlfq/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 17:29:02.816447 directlfq-0.2.7/directlfq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 17:29:02.000000 directlfq-0.2.7/directlfq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-28 17:28:40.000000 directlfq-0.2.7/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 17:29:02.828447 directlfq-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-28 17:28:40.000000 directlfq-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.084099 directlfq-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-01 11:08:53.000000 directlfq-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-03-01 11:08:53.000000 directlfq-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-01 11:08:53.000000 directlfq-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-03-01 11:09:25.084099 directlfq-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-03-01 11:08:53.000000 directlfq-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.072099 directlfq-0.2.8/directlfq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.076099 directlfq-0.2.8/directlfq/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)   111668 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10805 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30415 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.080099 directlfq-0.2.8/directlfq/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/download_links_for_testfiles_all.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/download_links_for_testfiles_quicktest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/intable_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/interface_parameters.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22544 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_fragion.rs
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20608 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_precursor.rs
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22528 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_ptm_fragion.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/dashboard_parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.080099 directlfq-0.2.8/directlfq/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14186 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/docs/Empty_manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/gui_textfields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.080099 directlfq-0.2.8/directlfq/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/img/github.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108120 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/img/max-planck-gesellschaft.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1317924 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/img/mpi_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   522703 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/img/ms_pipeline_visualization.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/lfq_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/protein_intensity_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.084099 directlfq-0.2.8/directlfq/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/style/dashboard_style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/testfile_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51865 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-03-01 11:08:53.000000 directlfq-0.2.8/directlfq/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:09:25.076099 directlfq-0.2.8/directlfq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 11:09:24.000000 directlfq-0.2.8/directlfq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-01 11:08:53.000000 directlfq-0.2.8/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 11:09:25.084099 directlfq-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-01 11:08:53.000000 directlfq-0.2.8/setup.py
```

### Comparing `directlfq-0.2.7/CONTRIBUTING.md` & `directlfq-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/LICENSE` & `directlfq-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/PKG-INFO` & `directlfq-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directlfq
-Version: 0.2.7
+Version: 0.2.8
 Summary: An open-source Python package of the AlphaPept ecosystem
 Home-page: https://github.com/MannLabs/directlfq
 Author: Mann Labs
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -42,14 +42,15 @@
 You can process DIA and DDA data analyzed by [AlphaPept](https://github.com/MannLabs/alphapept), MaxQuant, FragPipe, Spectronaut and DIANN as well as [generic formats](#generic-input-format), using a Graphical User Interface (GUI) or the python package.
 
 
 - [directLFQ](#directlfq)
   - [About](#about)
   - [Installation](#installation)
     - [One-click GUI](#one-click-gui)
+    - [Pip](#pip)
     - [Developer](#developer)
   - [Running directLFQ](#running-directlfq)
     - [GUI](#gui)
     - [CLI](#cli)
     - [Python and Jupyter notebooks](#python-and-jupyter-notebooks)
   - [Troubleshooting](#troubleshooting)
   - [Citations](#citations)
@@ -90,37 +91,43 @@
 
 * [**Windows**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_windows.exe)
 * [**macOS**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_macos.pkg)
 * [**Linux**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_linux.deb)
 
 Older releases remain available on the [release page](https://github.com/MannLabs/directlfq/releases), but no backwards compatibility is guaranteed.
 
-<!---
+-
 ### Pip
 
-directlfq can be installed in an existing Python 3.8 environment with a single `bash` command. *This `bash` command can also be run directly from within a Jupyter notebook by prepending it with a `!`*:
+directLFQ can be installed in an existing Python 3.8 environment with a single `bash` command.
 
 ```bash
 pip install directlfq
 ```
 
-Installing directlfq like this avoids conflicts when integrating it in other tools, as this does not enforce strict versioning of dependencies. However, if new versions of dependencies are released, they are not guaranteed to be fully compatible with directlfq. While this should only occur in rare cases where dependencies are not backwards compatible, you can always force directlfq to use dependancy versions which are known to be compatible with:
+This installs the core directLFQ without graphical user interface (GUI). If you want to install with additional dependencies for GUI support, you can do this with:
+
+```bash
+pip install "directlfq[gui]"
+```
+
+For installation with stable dependencies, use:
 
 ```bash
 pip install "directlfq[stable]"
 ```
 
 NOTE: You might need to run `pip install pip==21.0` before installing directlfq like this. Also note the double quotes `"`.
 
 For those who are really adventurous, it is also possible to directly install any branch (e.g. `@development`) with any extras (e.g. `#egg=directlfq[stable,development-stable]`) from GitHub with e.g.
 
 ```bash
 pip install "git+https://github.com/MannLabs/directlfq.git@development#egg=directlfq[stable,development-stable]"
 ```
--->
+
 ### Developer
 
 directlfq can also be installed in editable (i.e. developer) mode with a few `bash` commands. This allows to fully customize the software and even modify the source code to your specific needs. When an editable Python package is installed, its source code is stored in a transparent location of your choice. While optional, it is advised to first (create and) navigate to e.g. a general software folder:
 
 ```bash
 mkdir ~/folder/where/to/install/software
 cd ~/folder/where/to/install/software
```

### Comparing `directlfq-0.2.7/README.md` & `directlfq-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 You can process DIA and DDA data analyzed by [AlphaPept](https://github.com/MannLabs/alphapept), MaxQuant, FragPipe, Spectronaut and DIANN as well as [generic formats](#generic-input-format), using a Graphical User Interface (GUI) or the python package.
 
 
 - [directLFQ](#directlfq)
   - [About](#about)
   - [Installation](#installation)
     - [One-click GUI](#one-click-gui)
+    - [Pip](#pip)
     - [Developer](#developer)
   - [Running directLFQ](#running-directlfq)
     - [GUI](#gui)
     - [CLI](#cli)
     - [Python and Jupyter notebooks](#python-and-jupyter-notebooks)
   - [Troubleshooting](#troubleshooting)
   - [Citations](#citations)
@@ -63,37 +64,43 @@
 
 * [**Windows**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_windows.exe)
 * [**macOS**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_macos.pkg)
 * [**Linux**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_linux.deb)
 
 Older releases remain available on the [release page](https://github.com/MannLabs/directlfq/releases), but no backwards compatibility is guaranteed.
 
-<!---
+-
 ### Pip
 
-directlfq can be installed in an existing Python 3.8 environment with a single `bash` command. *This `bash` command can also be run directly from within a Jupyter notebook by prepending it with a `!`*:
+directLFQ can be installed in an existing Python 3.8 environment with a single `bash` command.
 
 ```bash
 pip install directlfq
 ```
 
-Installing directlfq like this avoids conflicts when integrating it in other tools, as this does not enforce strict versioning of dependencies. However, if new versions of dependencies are released, they are not guaranteed to be fully compatible with directlfq. While this should only occur in rare cases where dependencies are not backwards compatible, you can always force directlfq to use dependancy versions which are known to be compatible with:
+This installs the core directLFQ without graphical user interface (GUI). If you want to install with additional dependencies for GUI support, you can do this with:
+
+```bash
+pip install "directlfq[gui]"
+```
+
+For installation with stable dependencies, use:
 
 ```bash
 pip install "directlfq[stable]"
 ```
 
 NOTE: You might need to run `pip install pip==21.0` before installing directlfq like this. Also note the double quotes `"`.
 
 For those who are really adventurous, it is also possible to directly install any branch (e.g. `@development`) with any extras (e.g. `#egg=directlfq[stable,development-stable]`) from GitHub with e.g.
 
 ```bash
 pip install "git+https://github.com/MannLabs/directlfq.git@development#egg=directlfq[stable,development-stable]"
 ```
--->
+
 ### Developer
 
 directlfq can also be installed in editable (i.e. developer) mode with a few `bash` commands. This allows to fully customize the software and even modify the source code to your specific needs. When an editable Python package is installed, its source code is stored in a transparent location of your choice. While optional, it is advised to first (create and) navigate to e.g. a general software folder:
 
 ```bash
 mkdir ~/folder/where/to/install/software
 cd ~/folder/where/to/install/software
```

### Comparing `directlfq-0.2.7/directlfq/__init__.py` & `directlfq-0.2.8/directlfq/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 
 
 __project__ = "directlfq"
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 __license__ = "Apache"
 __description__ = "An open-source Python package of the AlphaPept ecosystem"
 __author__ = "Mann Labs"
 __author_email__ = "opensource@alphapept.com"
 __github__ = "https://github.com/MannLabs/directlfq"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `directlfq-0.2.7/directlfq/__pycache__/__init__.cpython-38.pyc` & `directlfq-0.2.8/directlfq/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Feb 28 17:28:40 2023 UTC, .py size: 1405 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 550d 0d0a 0000 0000 c839 fe63 7d05 0000  U........9.c}...
+00000000: 550d 0d0a 0000 0000 4532 ff63 7d05 0000  U.......E2.c}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 6408 6409  Z.d.Z.d.Z.d.d.d.
 00000050: 6703 5a07 640a 5a08 640b 640c 640d 640e  g.Z.d.Z.d.d.d.d.
 00000060: 640f 6410 6706 5a09 6411 6701 5a0a 6412  d.d.g.Z.d.g.Z.d.
 00000070: 6413 6506 6414 9c03 5a0b 6415 6416 6417  d.e.d...Z.d.d.d.
 00000080: 9c02 5a0c 6418 5300 2919 da09 6469 7265  ..Z.d.S.)...dire
-00000090: 6374 6c66 717a 0530 2e32 2e37 5a06 4170  ctlfqz.0.2.7Z.Ap
+00000090: 6374 6c66 717a 0530 2e32 2e38 5a06 4170  ctlfqz.0.2.8Z.Ap
 000000a0: 6163 6865 7a38 416e 206f 7065 6e2d 736f  achez8An open-so
 000000b0: 7572 6365 2050 7974 686f 6e20 7061 636b  urce Python pack
 000000c0: 6167 6520 6f66 2074 6865 2041 6c70 6861  age of the Alpha
 000000d0: 5065 7074 2065 636f 7379 7374 656d 7a09  Pept ecosystemz.
 000000e0: 4d61 6e6e 204c 6162 737a 186f 7065 6e73  Mann Labsz.opens
 000000f0: 6f75 7263 6540 616c 7068 6170 6570 742e  ource@alphapept.
 00000100: 636f 6d7a 2568 7474 7073 3a2f 2f67 6974  comz%https://git
```

### Comparing `directlfq-0.2.7/directlfq/_modidx.py` & `directlfq-0.2.8/directlfq/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,17 +638,14 @@
                                                                                  'directlfq/utils.py'),
                                  'directlfq.utils.merge_protein_cols_and_ion_dict': ( 'utils.html#merge_protein_cols_and_ion_dict',
                                                                                       'directlfq/utils.py'),
                                  'directlfq.utils.merge_sample_id_and_channels': ( 'utils.html#merge_sample_id_and_channels',
                                                                                    'directlfq/utils.py'),
                                  'directlfq.utils.parse_channel_from_peptide_column': ( 'utils.html#parse_channel_from_peptide_column',
                                                                                         'directlfq/utils.py'),
-                                 'directlfq.utils.plot_relative_to_median_fcs': ( 'utils.html#plot_relative_to_median_fcs',
-                                                                                  'directlfq/utils.py'),
-                                 'directlfq.utils.plot_withincond_fcs': ('utils.html#plot_withincond_fcs', 'directlfq/utils.py'),
                                  'directlfq.utils.prepare_loaded_tables': ('utils.html#prepare_loaded_tables', 'directlfq/utils.py'),
                                  'directlfq.utils.process_with_dask': ('utils.html#process_with_dask', 'directlfq/utils.py'),
                                  'directlfq.utils.reformat_and_save_input_file': ( 'utils.html#reformat_and_save_input_file',
                                                                                    'directlfq/utils.py'),
                                  'directlfq.utils.reformat_and_write_longtable_according_to_config': ( 'utils.html#reformat_and_write_longtable_according_to_config',
                                                                                                        'directlfq/utils.py'),
                                  'directlfq.utils.reformat_and_write_wideformat_table': ( 'utils.html#reformat_and_write_wideformat_table',
@@ -722,8 +719,12 @@
                                           'directlfq.visualizations.MultiOrganismMultiMethodBoxPlot': ( 'visualizations.html#multiorganismmultimethodboxplot',
                                                                                                         'directlfq/visualizations.py'),
                                           'directlfq.visualizations.MultiOrganismMultiMethodBoxPlot.__init__': ( 'visualizations.html#multiorganismmultimethodboxplot.__init__',
                                                                                                                  'directlfq/visualizations.py'),
                                           'directlfq.visualizations.MultiOrganismMultiMethodBoxPlot._add_expected_fold_changes': ( 'visualizations.html#multiorganismmultimethodboxplot._add_expected_fold_changes',
                                                                                                                                    'directlfq/visualizations.py'),
                                           'directlfq.visualizations.MultiOrganismMultiMethodBoxPlot.plot_boxplot': ( 'visualizations.html#multiorganismmultimethodboxplot.plot_boxplot',
-                                                                                                                     'directlfq/visualizations.py')}}}
+                                                                                                                     'directlfq/visualizations.py'),
+                                          'directlfq.visualizations.plot_relative_to_median_fcs': ( 'visualizations.html#plot_relative_to_median_fcs',
+                                                                                                    'directlfq/visualizations.py'),
+                                          'directlfq.visualizations.plot_withincond_fcs': ( 'visualizations.html#plot_withincond_fcs',
+                                                                                            'directlfq/visualizations.py')}}}
```

### Comparing `directlfq-0.2.7/directlfq/_nbdev.py` & `directlfq-0.2.8/directlfq/_nbdev.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/benchmarking.py` & `directlfq-0.2.8/directlfq/benchmarking.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/cli.py` & `directlfq-0.2.8/directlfq/cli.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/download_links_for_testfiles_all.yaml` & `directlfq-0.2.8/directlfq/configs/download_links_for_testfiles_all.yaml`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/intable_config.yaml` & `directlfq-0.2.8/directlfq/configs/intable_config.yaml`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/interface_parameters.json` & `directlfq-0.2.8/directlfq/configs/interface_parameters.json`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_fragion.rs` & `directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_fragion.rs`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_precursor.rs` & `directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_precursor.rs`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/configs/spectronaut_tableconfig_ptm_fragion.rs` & `directlfq-0.2.8/directlfq/configs/spectronaut_tableconfig_ptm_fragion.rs`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/dashboard_parts.py` & `directlfq-0.2.8/directlfq/dashboard_parts.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/docs/Empty_manual.pdf` & `directlfq-0.2.8/directlfq/docs/Empty_manual.pdf`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/gui.py` & `directlfq-0.2.8/directlfq/gui.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/gui_textfields.py` & `directlfq-0.2.8/directlfq/gui_textfields.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/img/github.png` & `directlfq-0.2.8/directlfq/img/github.png`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/img/max-planck-gesellschaft.jpg` & `directlfq-0.2.8/directlfq/img/max-planck-gesellschaft.jpg`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/img/mpi_logo.png` & `directlfq-0.2.8/directlfq/img/mpi_logo.png`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/img/ms_pipeline_visualization.png` & `directlfq-0.2.8/directlfq/img/ms_pipeline_visualization.png`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/lfq_manager.py` & `directlfq-0.2.8/directlfq/lfq_manager.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/normalization.py` & `directlfq-0.2.8/directlfq/normalization.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/protein_intensity_estimation.py` & `directlfq-0.2.8/directlfq/protein_intensity_estimation.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/style/dashboard_style.css` & `directlfq-0.2.8/directlfq/style/dashboard_style.css`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/testfile_handling.py` & `directlfq-0.2.8/directlfq/testfile_handling.py`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq/utils.py` & `directlfq-0.2.8/directlfq/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
            'set_mtraq_reduced_ion_column_into_dataframe', 'remove_mtraq_modifications_from_ion_ids', 'is_plexDIA_table',
            'parse_channel_from_peptide_column', 'merge_sample_id_and_channels', 'merge_channel_and_sample_string',
            'reformat_and_write_wideformat_table', 'check_for_processed_runs_in_results_folder', 'import_data',
            'reformat_and_save_input_file', 'add_ion_protein_headers_if_applicable', 'get_input_type_and_config_dict',
            'get_original_file_from_aq_reformat', 'import_config_dict', 'load_samplemap', 'prepare_loaded_tables',
            'LongTableReformater', 'AcquisitionTableHandler', 'AcquisitionTableInfo', 'AcquisitionTableHeaders',
            'AcquisitionTableOutputPaths', 'AcquisitionTableReformater', 'AcquisitionTableHeaderFilter',
-           'merge_acquisition_df_parameter_df', 'plot_withincond_fcs', 'plot_relative_to_median_fcs']
+           'merge_acquisition_df_parameter_df']
 
 # %% ../nbdev_nbs/04_utils.ipynb 2
 import os
 import pathlib
 if "__file__" in globals():#only run in the translated python file, as __file__ is not defined with ipython
     INTABLE_CONFIG = os.path.join(pathlib.Path(__file__).parent.absolute(), "configs", "intable_config.yaml") #the yaml config is located one directory below the python library files
     CONFIG_PATH = os.path.join(pathlib.Path(__file__).parent.absolute(), "configs")
@@ -1186,48 +1186,7 @@
         merged_df = merged_df.groupby('ion').mean().reset_index()
     if groupby_merge_type == 'min':
         merged_df = merged_df.groupby('ion').min().reset_index()
     if groupby_merge_type == 'max':
         merged_df = merged_df.groupby('ion').max().reset_index()
     merged_df = merged_df.dropna(axis=1, how='all')
     return merged_df
-
-# %% ../nbdev_nbs/04_utils.ipynb 54
-import matplotlib.pyplot as plt
-import itertools
-
-def plot_withincond_fcs(normed_intensity_df, cut_extremes = True):
-    """takes a normalized intensity dataframe and plots the fold change distribution between all samples. Column = sample, row = ion"""
-
-    samplecombs = list(itertools.combinations(normed_intensity_df.columns, 2))
-
-    for spair in samplecombs:#compare all pairs of samples
-        s1 = spair[0]
-        s2 = spair[1]
-        diff_fcs = normed_intensity_df[s1].to_numpy() - normed_intensity_df[s2].to_numpy() #calculate fold changes by subtracting log2 intensities of both samples
-
-        if cut_extremes:
-            cutoff = max(abs(np.nanquantile(diff_fcs,0.025)), abs(np.nanquantile(diff_fcs, 0.975))) #determine 2.5% - 97.5% interval, i.e. remove extremes
-            range = (-cutoff, cutoff)
-        else:
-            range = None
-        plt.hist(diff_fcs,80,density=True, histtype='step',range=range) #set the cutoffs to focus the visualization
-        plt.xlabel("log2 peptide fcs")
-
-    plt.show()
-
-# %% ../nbdev_nbs/04_utils.ipynb 55
-import matplotlib.pyplot as plt
-import itertools
-
-def plot_relative_to_median_fcs(normed_intensity_df):
-
-    median_intensities = normed_intensity_df.median(axis=1)
-    median_intensities = median_intensities.to_numpy()
-    
-    diff_fcs = []
-    for col in normed_intensity_df.columns:
-        median_fcs = normed_intensity_df[col].to_numpy() - median_intensities
-        diff_fcs.append(np.nanmedian(median_fcs))
-    plt.hist(diff_fcs,80,density=True, histtype='step')
-    plt.xlabel("log2 peptide fcs")
-    plt.show()
```

### Comparing `directlfq-0.2.7/directlfq.egg-info/PKG-INFO` & `directlfq-0.2.8/directlfq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directlfq
-Version: 0.2.7
+Version: 0.2.8
 Summary: An open-source Python package of the AlphaPept ecosystem
 Home-page: https://github.com/MannLabs/directlfq
 Author: Mann Labs
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -42,14 +42,15 @@
 You can process DIA and DDA data analyzed by [AlphaPept](https://github.com/MannLabs/alphapept), MaxQuant, FragPipe, Spectronaut and DIANN as well as [generic formats](#generic-input-format), using a Graphical User Interface (GUI) or the python package.
 
 
 - [directLFQ](#directlfq)
   - [About](#about)
   - [Installation](#installation)
     - [One-click GUI](#one-click-gui)
+    - [Pip](#pip)
     - [Developer](#developer)
   - [Running directLFQ](#running-directlfq)
     - [GUI](#gui)
     - [CLI](#cli)
     - [Python and Jupyter notebooks](#python-and-jupyter-notebooks)
   - [Troubleshooting](#troubleshooting)
   - [Citations](#citations)
@@ -90,37 +91,43 @@
 
 * [**Windows**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_windows.exe)
 * [**macOS**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_macos.pkg)
 * [**Linux**](https://github.com/MannLabs/directlfq/releases/latest/download/directlfq_gui_installer_linux.deb)
 
 Older releases remain available on the [release page](https://github.com/MannLabs/directlfq/releases), but no backwards compatibility is guaranteed.
 
-<!---
+-
 ### Pip
 
-directlfq can be installed in an existing Python 3.8 environment with a single `bash` command. *This `bash` command can also be run directly from within a Jupyter notebook by prepending it with a `!`*:
+directLFQ can be installed in an existing Python 3.8 environment with a single `bash` command.
 
 ```bash
 pip install directlfq
 ```
 
-Installing directlfq like this avoids conflicts when integrating it in other tools, as this does not enforce strict versioning of dependencies. However, if new versions of dependencies are released, they are not guaranteed to be fully compatible with directlfq. While this should only occur in rare cases where dependencies are not backwards compatible, you can always force directlfq to use dependancy versions which are known to be compatible with:
+This installs the core directLFQ without graphical user interface (GUI). If you want to install with additional dependencies for GUI support, you can do this with:
+
+```bash
+pip install "directlfq[gui]"
+```
+
+For installation with stable dependencies, use:
 
 ```bash
 pip install "directlfq[stable]"
 ```
 
 NOTE: You might need to run `pip install pip==21.0` before installing directlfq like this. Also note the double quotes `"`.
 
 For those who are really adventurous, it is also possible to directly install any branch (e.g. `@development`) with any extras (e.g. `#egg=directlfq[stable,development-stable]`) from GitHub with e.g.
 
 ```bash
 pip install "git+https://github.com/MannLabs/directlfq.git@development#egg=directlfq[stable,development-stable]"
 ```
--->
+
 ### Developer
 
 directlfq can also be installed in editable (i.e. developer) mode with a few `bash` commands. This allows to fully customize the software and even modify the source code to your specific needs. When an editable Python package is installed, its source code is stored in a transparent location of your choice. While optional, it is advised to first (create and) navigate to e.g. a general software folder:
 
 ```bash
 mkdir ~/folder/where/to/install/software
 cd ~/folder/where/to/install/software
```

### Comparing `directlfq-0.2.7/directlfq.egg-info/SOURCES.txt` & `directlfq-0.2.8/directlfq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/directlfq.egg-info/requires.txt` & `directlfq-0.2.8/directlfq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `directlfq-0.2.7/settings.ini` & `directlfq-0.2.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = ammarcsj
 description = sensitive quantification for proteomics
 keywords = quantification, peptides, statistics, bioinformatics, proteomics, mass spectrometry
 author = Constantin Ammar
 author_email = constantin.ammar@gmail.com
 copyright = fast.ai
 branch = master
-version = 0.2.7
+version = 0.2.8
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `directlfq-0.2.7/setup.py` & `directlfq-0.2.8/setup.py`

 * *Files identical despite different names*

