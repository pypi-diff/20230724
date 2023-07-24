# Comparing `tmp/alphatims-1.0.7.tar.gz` & `tmp/alphatims-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphatims-1.0.7.tar", last modified: Mon Feb 13 11:44:31 2023, max compression
+gzip compressed data, was "alphatims-1.0.8.tar", last modified: Mon Jul 24 13:39:54 2023, max compression
```

## Comparing `alphatims-1.0.7.tar` & `alphatims-1.0.8.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.743258 alphatims-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    50105 2023-02-13 11:44:03.000000 alphatims-1.0.7/LICENSE-THIRD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-02-13 11:44:03.000000 alphatims-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-13 11:44:03.000000 alphatims-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    36324 2023-02-13 11:44:31.739258 alphatims-1.0.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    34778 2023-02-13 11:44:03.000000 alphatims-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.703257 alphatims-1.0.7/alphatims/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.703257 alphatims-1.0.7/alphatims/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)   123635 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/compiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/dia_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.703257 alphatims-1.0.7/alphatims/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   639880 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/docs/cli_manual.pdf
--rw-r--r--   0 runner    (1001) docker     (123)  1217035 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/docs/gui_manual.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.719258 alphatims-1.0.7/alphatims/ext/
--rw-r--r--   0 runner    (1001) docker     (123) 15865872 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/ext/timsdata.dll
--rw-r--r--   0 runner    (1001) docker     (123) 18668200 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/ext/timsdata.so
--rw-r--r--   0 runner    (1001) docker     (123)    55626 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.739258 alphatims-1.0.7/alphatims/img/
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/img/github.png
--rw-r--r--   0 runner    (1001) docker     (123)   108120 2023-02-13 11:44:03.000000 alphatims-1.0.7/alphatims/img/max-planck-gesellschaft.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1317924 2023-02-13 11:44:04.000000 alphatims-1.0.7/alphatims/img/mpi_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.739258 alphatims-1.0.7/alphatims/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5726 2023-02-13 11:44:04.000000 alphatims-1.0.7/alphatims/lib/interface_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-02-13 11:44:04.000000 alphatims-1.0.7/alphatims/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-02-13 11:44:04.000000 alphatims-1.0.7/alphatims/tempmmap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40571 2023-02-13 11:44:04.000000 alphatims-1.0.7/alphatims/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:44:31.703257 alphatims-1.0.7/alphatims.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36324 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 11:44:31.000000 alphatims-1.0.7/alphatims.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 11:44:31.743258 alphatims-1.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-02-13 11:44:04.000000 alphatims-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.500120 alphatims-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    50105 2023-07-24 13:39:09.000000 alphatims-1.0.8/LICENSE-THIRD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-24 13:39:09.000000 alphatims-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 13:39:09.000000 alphatims-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-07-24 13:39:54.500120 alphatims-1.0.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35391 2023-07-24 13:39:09.000000 alphatims-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.464120 alphatims-1.0.8/alphatims/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.464120 alphatims-1.0.8/alphatims/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)   125641 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/compiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/dia_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.464120 alphatims-1.0.8/alphatims/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   639880 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/docs/cli_manual.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1217035 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/docs/gui_manual.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.480120 alphatims-1.0.8/alphatims/ext/
+-rw-r--r--   0 runner    (1001) docker     (123) 15865872 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/ext/timsdata.dll
+-rw-r--r--   0 runner    (1001) docker     (123) 18668200 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/ext/timsdata.so
+-rw-r--r--   0 runner    (1001) docker     (123)    55626 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.500120 alphatims-1.0.8/alphatims/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/img/github.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108120 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/img/max-planck-gesellschaft.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1317924 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/img/mpi_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.500120 alphatims-1.0.8/alphatims/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5726 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/lib/interface_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/tempmmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40621 2023-07-24 13:39:09.000000 alphatims-1.0.8/alphatims/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.464120 alphatims-1.0.8/alphatims.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36937 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 13:39:54.000000 alphatims-1.0.8/alphatims.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:39:54.500120 alphatims-1.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-07-24 13:39:10.000000 alphatims-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:39:54.500120 alphatims-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-24 13:39:10.000000 alphatims-1.0.8/tests/test_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-24 13:39:10.000000 alphatims-1.0.8/tests/test_utils.py
```

### Comparing `alphatims-1.0.7/LICENSE-THIRD-PARTY.txt` & `alphatims-1.0.8/LICENSE-THIRD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/LICENSE.txt` & `alphatims-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/PKG-INFO` & `alphatims-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphatims
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python package to index Bruker TimsTOF raw data for fast and easy accession and visualization
 Home-page: https://github.com/MannLabs/alphatims
 Author: Sander Willems, Eugenia Voytik
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -51,15 +51,15 @@
   * [**Installation**](#installation)
      * [**One-click GUI**](#one-click-gui)
      * [**Pip installer**](#pip)
      * [**Developer installer**](#developer)
      * [**Installation issues**](#installation-issues)
   * [**Test data**](#test-data)
     * [**Test sample**](#test-sample)
-    * [**LC**](#lc)  
+    * [**LC**](#lc)
     * [**DDA**](#dda)
     * [**DIA**](#dia)
   * [**Usage**](#usage)
     * [**GUI**](#gui)
     * [**CLI**](#cli)
     * [**Python and jupyter notebooks**](#python-and-jupyter-notebooks)
     * [**Other tools**](#other-tools)
@@ -97,14 +97,15 @@
 
 AlphaTims can be installed and used on all major operating systems (Windows, macOS and Linux).
 There are three different types of installation possible:
 
 * [**One-click GUI installer:**](#one-click-gui) Choose this installation if you only want the GUI and/or keep things as simple as possible.
 * [**Pip installer:**](#pip) Choose this installation if you want to use AlphaTims as a Python package in an existing Python 3.8 environment (e.g. a Jupyter notebook). If needed, the GUI and CLI can be installed with pip as well.
 * [**Developer installer:**](#developer) Choose this installation if you are familiar with CLI tools, [conda](https://docs.conda.io/en/latest/) and Python. This installation allows access to all available features of AlphaTims and even allows to modify its source code directly. Generally, the developer version of AlphaTims outperforms the precompiled versions which makes this the installation of choice for high-throughput experiments.
+* [**Docker:**](#docker) Use this installation if you want to use a container based workflow. This is usefull to preserve a clean environment or when running multiple tools that might have conflicting dependencies.
 
 ***IMPORTANT: While AlphaTims is mostly platform independent, some calibration functions require [Bruker libraries](alphatims/ext) which are only available on Windows and Linux.***
 
 ### One-click GUI
 
 The GUI of AlphaTims is a completely stand-alone tool that requires no knowledge of Python or CLI tools. Click on one of the links below to download the latest release for:
 
@@ -210,14 +211,22 @@
   alphatims_bin="$(which alphatims)"
   echo "alias alphatims='"${alphatims_bin}"'" >> ~/.bashrc
   conda deactivate
   ```
   When `zsh` is the default terminal instead of `bash`, replace `~/.bashrc` with `~/.zshrc`. On Windows, the command `where alphatims` can be used to find the location of the binary executable. This path can then be (permanently) added to Windows' path variable.
 * When using Jupyter notebooks and multiple conda environments direcly from the terminal, it is recommended to `conda install nb_conda_kernels` in the conda base environment. Hereafter, running a `jupyter notebook` from the conda base environment should have a `python [conda env: alphatims]` kernel available, in addition to all other conda kernels in which the command `conda install ipykernel` was run.
 
+### Docker
+
+(WIP)
+
+```shell
+docker pull ghcr://MannLabs/alphatims:latest
+```
+
 ### Installation issues
 
 See the general [troubleshooting](#troubleshooting) section.
 
 ---
 ## Test data
 
@@ -349,14 +358,15 @@
 * **AlphaTims is not found.** Make sure you use the right folder. Local folders are best called by prefixing them with `./` (e.g. `pip install "./alphatims"`). On some systems, installation specifically requires (not) to use single quotes `'` around the AlphaTims folder, e.g. `pip install "./alphatims[plotting-stable,development]"`.
 * **Modifications to the AlphaTims source code are not reflected.** Make sure you use the `-e` flag when using `pip install -e alphatims`.
 * **Numpy does not work properly.** On Windows, `numpy==1.19.4` has some issues. After installing AlphaTims, downgrade NumPy with `pip install numpy==1.19.3`.
 * **Exporting PNG images with the CLI or Python package might not work out-of-the-box**. If a conda environment is used, this can be fixed by running `conda install -c conda-forge firefox geckodriver` in the AlphaTims conda environment. Alternatively, a file can be exported as html and opened in a browser. From the browser there is a `save as png` button available.
 * **GUI does not open.** In some cases this can be simply because of using an incompatible (default) browser. AlphaTims has been tested with Google Chrome and Mozilla Firefox. Windows IE and Windows Edge compatibility is not guaranteed.
 * **When older Bruker files need to be processed as well,** the [legacy dependencies](requirements/requirements_legacy.txt) are also needed. However, note that this requires [Microsoft Visual C++](https://visualstudio.microsoft.com/visual-cpp-build-tools) to be manually installed (on Windows machines) prior to AlphaTims installation! To include the legacy dependencies, install AlphaTims with `pip install "alphatims[legacy]"` or `pip install "alphatims[legacy]" --upgrade` if already pre-installed.
 * **When installed through `pip`, the GUI cannot be started.** Make sure you install AlphaTims with `pip install "alphatims[plotting-stable]"` to include the GUI with stable dependancies. If this was done and it still fails to run the GUI, a possible fix might be to run `pip install panel==0.10.3` after AlphaTims was installed.
+* **Some external libraries are missing.** On some OS, there might be libraries missing. As an exmaple, the following error message might pop up: `OSError: libgomp.so.1: cannot open shared object file: No such file or directory`. This can be solved by installing those manually, e.g. on Linux: `apt-get install libgomp1`.
 
 ---
 ## How it works
 
 The basic workflow of AlphaTims looks as follows:
 
 * Read data from a [Bruker `.d` folder](#bruker-raw-data).
```

### Comparing `alphatims-1.0.7/README.md` & `alphatims-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   * [**Installation**](#installation)
      * [**One-click GUI**](#one-click-gui)
      * [**Pip installer**](#pip)
      * [**Developer installer**](#developer)
      * [**Installation issues**](#installation-issues)
   * [**Test data**](#test-data)
     * [**Test sample**](#test-sample)
-    * [**LC**](#lc)  
+    * [**LC**](#lc)
     * [**DDA**](#dda)
     * [**DIA**](#dia)
   * [**Usage**](#usage)
     * [**GUI**](#gui)
     * [**CLI**](#cli)
     * [**Python and jupyter notebooks**](#python-and-jupyter-notebooks)
     * [**Other tools**](#other-tools)
@@ -62,14 +62,15 @@
 
 AlphaTims can be installed and used on all major operating systems (Windows, macOS and Linux).
 There are three different types of installation possible:
 
 * [**One-click GUI installer:**](#one-click-gui) Choose this installation if you only want the GUI and/or keep things as simple as possible.
 * [**Pip installer:**](#pip) Choose this installation if you want to use AlphaTims as a Python package in an existing Python 3.8 environment (e.g. a Jupyter notebook). If needed, the GUI and CLI can be installed with pip as well.
 * [**Developer installer:**](#developer) Choose this installation if you are familiar with CLI tools, [conda](https://docs.conda.io/en/latest/) and Python. This installation allows access to all available features of AlphaTims and even allows to modify its source code directly. Generally, the developer version of AlphaTims outperforms the precompiled versions which makes this the installation of choice for high-throughput experiments.
+* [**Docker:**](#docker) Use this installation if you want to use a container based workflow. This is usefull to preserve a clean environment or when running multiple tools that might have conflicting dependencies.
 
 ***IMPORTANT: While AlphaTims is mostly platform independent, some calibration functions require [Bruker libraries](alphatims/ext) which are only available on Windows and Linux.***
 
 ### One-click GUI
 
 The GUI of AlphaTims is a completely stand-alone tool that requires no knowledge of Python or CLI tools. Click on one of the links below to download the latest release for:
 
@@ -175,14 +176,22 @@
   alphatims_bin="$(which alphatims)"
   echo "alias alphatims='"${alphatims_bin}"'" >> ~/.bashrc
   conda deactivate
   ```
   When `zsh` is the default terminal instead of `bash`, replace `~/.bashrc` with `~/.zshrc`. On Windows, the command `where alphatims` can be used to find the location of the binary executable. This path can then be (permanently) added to Windows' path variable.
 * When using Jupyter notebooks and multiple conda environments direcly from the terminal, it is recommended to `conda install nb_conda_kernels` in the conda base environment. Hereafter, running a `jupyter notebook` from the conda base environment should have a `python [conda env: alphatims]` kernel available, in addition to all other conda kernels in which the command `conda install ipykernel` was run.
 
+### Docker
+
+(WIP)
+
+```shell
+docker pull ghcr://MannLabs/alphatims:latest
+```
+
 ### Installation issues
 
 See the general [troubleshooting](#troubleshooting) section.
 
 ---
 ## Test data
 
@@ -314,14 +323,15 @@
 * **AlphaTims is not found.** Make sure you use the right folder. Local folders are best called by prefixing them with `./` (e.g. `pip install "./alphatims"`). On some systems, installation specifically requires (not) to use single quotes `'` around the AlphaTims folder, e.g. `pip install "./alphatims[plotting-stable,development]"`.
 * **Modifications to the AlphaTims source code are not reflected.** Make sure you use the `-e` flag when using `pip install -e alphatims`.
 * **Numpy does not work properly.** On Windows, `numpy==1.19.4` has some issues. After installing AlphaTims, downgrade NumPy with `pip install numpy==1.19.3`.
 * **Exporting PNG images with the CLI or Python package might not work out-of-the-box**. If a conda environment is used, this can be fixed by running `conda install -c conda-forge firefox geckodriver` in the AlphaTims conda environment. Alternatively, a file can be exported as html and opened in a browser. From the browser there is a `save as png` button available.
 * **GUI does not open.** In some cases this can be simply because of using an incompatible (default) browser. AlphaTims has been tested with Google Chrome and Mozilla Firefox. Windows IE and Windows Edge compatibility is not guaranteed.
 * **When older Bruker files need to be processed as well,** the [legacy dependencies](requirements/requirements_legacy.txt) are also needed. However, note that this requires [Microsoft Visual C++](https://visualstudio.microsoft.com/visual-cpp-build-tools) to be manually installed (on Windows machines) prior to AlphaTims installation! To include the legacy dependencies, install AlphaTims with `pip install "alphatims[legacy]"` or `pip install "alphatims[legacy]" --upgrade` if already pre-installed.
 * **When installed through `pip`, the GUI cannot be started.** Make sure you install AlphaTims with `pip install "alphatims[plotting-stable]"` to include the GUI with stable dependancies. If this was done and it still fails to run the GUI, a possible fix might be to run `pip install panel==0.10.3` after AlphaTims was installed.
+* **Some external libraries are missing.** On some OS, there might be libraries missing. As an exmaple, the following error message might pop up: `OSError: libgomp.so.1: cannot open shared object file: No such file or directory`. This can be solved by installing those manually, e.g. on Linux: `apt-get install libgomp1`.
 
 ---
 ## How it works
 
 The basic workflow of AlphaTims looks as follows:
 
 * Read data from a [Bruker `.d` folder](#bruker-raw-data).
```

### Comparing `alphatims-1.0.7/alphatims/__init__.py` & `alphatims-1.0.8/alphatims/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 
 
 __project__ = "alphatims"
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 __license__ = "Apache"
 __description__ = "A Python package to index Bruker TimsTOF raw data for fast and easy accession and visualization"
 __author__ = "Sander Willems, Eugenia Voytik"
 __author_email__ = "opensource@alphapept.com"
 __github__ = "https://github.com/MannLabs/alphatims"
 __keywords__ = [
     "ms",
```

### Comparing `alphatims-1.0.7/alphatims/__pycache__/__init__.cpython-38.pyc` & `alphatims-1.0.8/alphatims/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Feb 13 11:44:03 2023 UTC, .py size: 1596 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-00000000: 550d 0d0a 0000 0000 8322 ea63 3c06 0000  U........".c<...
+00000000: 550d 0d0a 0000 0000 fd7e be64 3c06 0000  U........~.d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 6408 6409  Z.d.Z.d.Z.d.d.d.
 00000050: 640a 640b 640c 640d 6707 5a07 640e 5a08  d.d.d.d.g.Z.d.Z.
 00000060: 640f 6410 6411 6412 6413 6414 6415 6416  d.d.d.d.d.d.d.d.
 00000070: 6708 5a09 6417 6701 5a0a 6418 6419 6506  g.Z.d.g.Z.d.d.e.
 00000080: 641a 641b 641c 641d 9c06 5a0b 641e 641f  d.d.d.d...Z.d.d.
 00000090: 6420 6421 6422 9c04 5a0c 6423 5300 2924  d d!d"..Z.d#S.)$
 000000a0: da09 616c 7068 6174 696d 737a 0531 2e30  ..alphatimsz.1.0
-000000b0: 2e37 5a06 4170 6163 6865 7a5f 4120 5079  .7Z.Apachez_A Py
+000000b0: 2e38 5a06 4170 6163 6865 7a5f 4120 5079  .8Z.Apachez_A Py
 000000c0: 7468 6f6e 2070 6163 6b61 6765 2074 6f20  thon package to 
 000000d0: 696e 6465 7820 4272 756b 6572 2054 696d  index Bruker Tim
 000000e0: 7354 4f46 2072 6177 2064 6174 6120 666f  sTOF raw data fo
 000000f0: 7220 6661 7374 2061 6e64 2065 6173 7920  r fast and easy 
 00000100: 6163 6365 7373 696f 6e20 616e 6420 7669  accession and vi
 00000110: 7375 616c 697a 6174 696f 6e7a 1e53 616e  sualizationz.San
 00000120: 6465 7220 5769 6c6c 656d 732c 2045 7567  der Willems, Eug
```

### Comparing `alphatims-1.0.7/alphatims/bruker.py` & `alphatims-1.0.8/alphatims/bruker.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,16 @@
     )
 elif sys.platform[:5] == "linux":
     BRUKER_DLL_FILE_NAME = os.path.join(
         alphatims.utils.EXT_PATH,
         "timsdata.so"
     )
 else:
-    logging.warning(
-        "WARNING: "
-        "No Bruker libraries are available for this operating system. "
-        "Mobility and m/z values need to be estimated. "
-        "While this estimation often returns acceptable results with errors "
-        "< 0.02 Th, huge errors (e.g. offsets of 6 Th) have already been "
-        "observed for some samples!"
-    )
-    logging.info("")
     BRUKER_DLL_FILE_NAME = ""
 
-
 def init_bruker_dll(bruker_dll_file_name: str = BRUKER_DLL_FILE_NAME):
     """Open a bruker.dll in Python.
 
     Five functions are defined for this dll:
 
         - tims_open: [c_char_p, c_uint32] -> c_uint64
         - tims_close: [c_char_p, c_uint32] -> c_uint64
@@ -992,14 +982,27 @@
             Default is True.
         convert_polarity_to_int : bool
             Convert the polarity to int (-1 or +1).
             This allows to keep it in numerical form.
             This is ignored if the polarity is dropped.
             Default is True.
         """
+        
+        #Log a warning if there was not a valid DLL filename
+        if BRUKER_DLL_FILE_NAME=="":
+            logging.warning(
+                "WARNING: "
+                "No Bruker libraries are available for this operating system. "
+                "Mobility and m/z values need to be estimated. "
+                "While this estimation often returns acceptable results with errors "
+                "< 0.02 Th, huge errors (e.g. offsets of 6 Th) have already been "
+                "observed for some samples!"
+            )
+            logging.info("")
+
         if bruker_d_folder_name.endswith("/"):
             bruker_d_folder_name = bruker_d_folder_name[:-1]
         logging.info(f"Importing data from {bruker_d_folder_name}")
         if bruker_d_folder_name.endswith(".d"):
             bruker_hdf_file_name = f"{bruker_d_folder_name[:-2]}.hdf"
             hdf_file_exists = os.path.exists(bruker_hdf_file_name)
             if use_hdf_if_available and hdf_file_exists:
@@ -1978,15 +1981,15 @@
         )
         precursor_offsets[0] = 0
         precursor_offsets[1:-1] = np.flatnonzero(
             np.diff(self.precursor_indices[precursor_order]) > 0) + 1
         precursor_offsets[-1] = len(precursor_order)
         offset = precursor_offsets[1]
         offsets = precursor_order[offset:]
-        counts = np.empty(len(offsets) + 1, dtype=np.int)
+        counts = np.empty(len(offsets) + 1, dtype=np.int64)
         counts[0] = 0
         counts[1:] = np.cumsum(
             self.quad_indptr[offsets + 1] - self.quad_indptr[offsets]
         )
         spectrum_indptr = np.empty(
             self.precursor_max_index + 1,
             dtype=np.int64
@@ -2054,30 +2057,31 @@
         )
         return (
             new_spectrum_indptr,
             trimmed_spectrum_tof_indices,
             trimmed_spectrum_intensity_values
         )
 
-    def save_as_mgf(
+    def save_as_spectra(
         self,
         directory: str,
         file_name: str,
         overwrite: bool = False,
         centroiding_window: int = 5,
         keep_n_most_abundant_peaks: int = -1,
+        mgf: bool = True
     ):
-        """Save profile spectra from this TimsTOF object as an mgf file.
+        """Save profile spectra from this TimsTOF object as an spectrum file.
 
         Parameters
         ----------
         directory : str
-            The directory where to save the mgf file.
+            The directory where to save the spectrum file.
         file_name : str
-            The file name of the  mgf file.
+            The file name of the spectrum file.
         overwrite : bool
             If True, an existing file is truncated.
             If False, nothing happens if a file already exists.
             Default is False.
         centroiding_window : int
             The centroiding window to use.
             If 0, no centroiding is performed.
@@ -2086,15 +2090,15 @@
             Keep the n most abundant peaks.
             If -1, all peaks are retained.
             Default is -1.
 
         Returns
         -------
         str
-            The full file name of the mgf file.
+            The full file name of the spectrum file.
         """
         full_file_name = os.path.join(
             directory,
             file_name
         )
         if self.acquisition_mode != "ddaPASEF":
             logging.info(
@@ -2123,38 +2127,44 @@
         charges[np.flatnonzero(np.isnan(charges))] = 0
         charges = charges.astype(np.int64)
         rtinseconds = self.rt_values[self.precursors.Parent.values]
         intensities = self.precursors.Intensity.values
         mobilities = self.mobility_values[
             self.precursors.ScanNumber.values.astype(np.int64)
         ]
-        with open(full_file_name, "w") as infile:
-            logging.info(f"Exporting profile spectra to {full_file_name}...")
-            for index in alphatims.utils.progress_callback(
-                range(1, self.precursor_max_index)
-            ):
-                start = spectrum_indptr[index]
-                end = spectrum_indptr[index + 1]
-                title = (
-                    f"index: {index}, "
-                    f"intensity: {intensities[index - 1]:.1f}, "
-                    f"mobility: {mobilities[index - 1]:.3f}, "
-                    f"average_mz: {average_mzs[index - 1]:.3f}"
-                )
-                infile.write("BEGIN IONS\n")
-                infile.write(f'TITLE="{title}"\n')
-                infile.write(f"PEPMASS={mono_mzs[index - 1]:.6f}\n")
-                infile.write(f"CHARGE={charges[index - 1]}\n")
-                infile.write(f"RTINSECONDS={rtinseconds[index - 1]:.2f}\n")
-                for mz, intensity in zip(
-                    self.mz_values[spectrum_tof_indices[start: end]],
-                    spectrum_intensity_values[start: end],
-                ):
-                    infile.write(f"{mz:.6f} {intensity}\n")
-                infile.write("END IONS\n")
+        logging.info(f"Exporting profile spectra to {full_file_name}...")
+        if mgf:
+            save_as_mgf(
+                full_file_name,
+                spectrum_indptr,
+                intensities,
+                mobilities,
+                average_mzs,
+                mono_mzs,
+                charges,
+                rtinseconds,
+                spectrum_tof_indices,
+                spectrum_intensity_values,
+                self.precursor_max_index,
+                self.mz_values,
+            )
+        else:
+            save_as_spectra(
+                full_file_name,
+                spectrum_indptr,
+                intensities,
+                mobilities,
+                average_mzs,
+                mono_mzs,
+                charges,
+                rtinseconds,
+                spectrum_tof_indices,
+                spectrum_intensity_values,
+                self.mz_values,
+            )
         logging.info(
             f"Succesfully wrote {self.precursor_max_index - 1:,} "
             f"spectra to {full_file_name}."
         )
         return full_file_name
 
     def calculate_global_calibrated_mz_values(
@@ -2322,15 +2332,15 @@
 
 class PrecursorFloatError(TypeError):
     """Used to indicate that a precursor value is not an int but a float."""
     pass
 
 
 @alphatims.utils.pjit(
-    signature_or_function="void(i8,i8[:],i8[:],i8[:],u4[:],u2[:],u4[:],f8[:],i8[:],i8[:])"
+    # signature_or_function="void(i8,i8[:],i8[:],i8[:],u4[:],u2[:],u4[:],f8[:],i8[:],i8[:])"
 )
 def set_precursor(
     precursor_index: int,
     offset_order: np.ndarray,
     precursor_offsets: np.ndarray,
     quad_indptr: np.ndarray,
     tof_indices: np.ndarray,
@@ -3287,7 +3297,73 @@
                     values.append(idx)
                     columns.append(i)
                     break  # TODO what if multiple hits?
                 idx += 1
                 tof_value = tof_indices[idx]
         indptr.append(len(values))
     return np.array(indptr), np.array(values), np.array(columns)
+
+
+def save_as_mgf(
+    full_file_name,
+    spectrum_indptr,
+    intensities,
+    mobilities,
+    average_mzs,
+    mono_mzs,
+    charges,
+    rtinseconds,
+    spectrum_tof_indices,
+    spectrum_intensity_values,
+    precursor_max_index,
+    mz_values,
+):
+    with open(full_file_name, "w") as infile:
+        for index in alphatims.utils.progress_callback(
+            range(1, precursor_max_index)
+        ):
+            start = spectrum_indptr[index]
+            end = spectrum_indptr[index + 1]
+            title = (
+                f"index: {index}, "
+                f"intensity: {intensities[index - 1]:.1f}, "
+                f"mobility: {mobilities[index - 1]:.3f}, "
+                f"average_mz: {average_mzs[index - 1]:.3f}"
+            )
+            infile.write("BEGIN IONS\n")
+            infile.write(f'TITLE="{title}"\n')
+            infile.write(f"PEPMASS={mono_mzs[index - 1]:.6f}\n")
+            infile.write(f"CHARGE={charges[index - 1]}\n")
+            infile.write(f"RTINSECONDS={rtinseconds[index - 1]:.2f}\n")
+            for mz, intensity in zip(
+                mz_values[spectrum_tof_indices[start: end]],
+                spectrum_intensity_values[start: end],
+            ):
+                infile.write(f"{mz:.6f} {intensity}\n")
+            infile.write("END IONS\n")
+
+
+def save_as_spectra(
+    full_file_name,
+    spectrum_indptr,
+    intensities,
+    mobilities,
+    average_mzs,
+    mono_mzs,
+    charges,
+    rtinseconds,
+    spectrum_tof_indices,
+    spectrum_intensity_values,
+    mz_values,
+):
+    with h5py.File(full_file_name, "w") as infile:
+        infile["indptr"] = spectrum_indptr[1:]
+        infile["fragment_mzs"] = mz_values[
+            spectrum_tof_indices
+        ]
+        infile["fragment_intensities"] = spectrum_intensity_values
+        infile["precursor_rt"] = rtinseconds
+        infile["precursor_charge"] = charges
+        infile["precursor_intensity"] = intensities
+        infile["precursor_mobility"] = mobilities
+        infile["precursor_average_mz"] = average_mzs
+        infile["precursor_monoisotopic_mz"] = mono_mzs
```

### Comparing `alphatims-1.0.7/alphatims/cli.py` & `alphatims-1.0.8/alphatims/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -308,20 +308,54 @@
     with parse_cli_settings("export mgf", **kwargs) as parameters:
         import alphatims.bruker
         data = alphatims.bruker.TimsTOF(parameters["bruker_raw_data"])
         if "output_folder" not in parameters:
             directory = data.directory
         else:
             directory = parameters["output_folder"]
-        data.save_as_mgf(
+        data.save_as_spectra(
             overwrite=not parameters["disable_overwrite"],
             directory=directory,
             file_name=f"{data.sample_name}.mgf",
             centroiding_window=parameters["centroiding_window"],
-            keep_n_most_abundant_peaks=parameters["keep_n_most_abundant_peaks"]
+            keep_n_most_abundant_peaks=parameters["keep_n_most_abundant_peaks"],
+            mgf=True,
+        )
+
+
+@export.command(
+    "spectra",
+    help="Export BRUKER_RAW_DATA as (profile) spectra file.",
+    no_args_is_help=True,
+)
+@cli_option("bruker_raw_data", as_argument=True)
+@cli_option("keep_n_most_abundant_peaks")
+@cli_option("centroiding_window")
+@cli_option("disable_overwrite")
+@cli_option("output_folder")
+@cli_option("log_file")
+@cli_option("threads")
+@cli_option("disable_log_stream")
+@cli_option("parameter_file")
+@cli_option("export_parameters")
+def export_spectra(**kwargs):
+    with parse_cli_settings("export spectra", **kwargs) as parameters:
+        import alphatims.bruker
+        data = alphatims.bruker.TimsTOF(parameters["bruker_raw_data"])
+        if "output_folder" not in parameters:
+            directory = data.directory
+        else:
+            directory = parameters["output_folder"]
+        data.save_as_spectra(
+            overwrite=not parameters["disable_overwrite"],
+            directory=directory,
+            file_name=f"{data.sample_name}.spectra.hdf",
+            centroiding_window=parameters["centroiding_window"],
+            keep_n_most_abundant_peaks=parameters["keep_n_most_abundant_peaks"],
+            mgf=False,
         )
 
 
 @export.command(
     "selection",
     help="Load a BRUKER_RAW_DATA and select a data slice for export.",
     no_args_is_help=True,
```

### Comparing `alphatims-1.0.7/alphatims/compiling.py` & `alphatims-1.0.8/alphatims/compiling.py`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/dia_data.py` & `alphatims-1.0.8/alphatims/dia_data.py`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/docs/cli_manual.pdf` & `alphatims-1.0.8/alphatims/docs/cli_manual.pdf`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/docs/gui_manual.pdf` & `alphatims-1.0.8/alphatims/docs/gui_manual.pdf`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/ext/timsdata.dll` & `alphatims-1.0.8/alphatims/ext/timsdata.dll`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/ext/timsdata.so` & `alphatims-1.0.8/alphatims/ext/timsdata.so`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/gui.py` & `alphatims-1.0.8/alphatims/gui.py`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/img/github.png` & `alphatims-1.0.8/alphatims/img/github.png`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/img/max-planck-gesellschaft.jpg` & `alphatims-1.0.8/alphatims/img/max-planck-gesellschaft.jpg`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/img/mpi_logo.png` & `alphatims-1.0.8/alphatims/img/mpi_logo.png`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/lib/interface_parameters.json` & `alphatims-1.0.8/alphatims/lib/interface_parameters.json`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/plotting.py` & `alphatims-1.0.8/alphatims/plotting.py`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/alphatims/tempmmap.py` & `alphatims-1.0.8/alphatims/tempmmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,22 +35,14 @@
 
 
 _TEMP_DIR, TEMP_DIR_NAME = make_temp_dir()
 ARRAYS = {}
 CLOSED = False
 ALLOW_NDARRAY_SUBCLASS = False
 
-logging.warning(
-    f"WARNING: Temp mmap arrays are written to {TEMP_DIR_NAME}. "
-    "Cleanup of this folder is OS dependant, "
-    "and might need to be triggered manually! "
-    f"Current space: {shutil.disk_usage(TEMP_DIR_NAME)[-1]:,}"
-)
-
-
 def empty(shape: tuple, dtype: np.dtype) -> np.ndarray:
     """Create a writable temporary mmapped array.
 
     Parameters
     ----------
     shape : tuple
         A tuple with the shape of the array.
@@ -268,14 +260,22 @@
         del _array
         gc.collect()
         _memmap.close()
         del _memmap
     del _TEMP_DIR
     _TEMP_DIR, TEMP_DIR_NAME = make_temp_dir()
     ARRAYS = {}
+    
+    logging.warning(
+    f"WARNING: Temp mmap arrays were written to {TEMP_DIR_NAME}. "
+    "Cleanup of this folder is OS dependant, "
+    "and might need to be triggered manually! "
+    f"Current space: {shutil.disk_usage(TEMP_DIR_NAME)[-1]:,}"
+    )
+    
     return TEMP_DIR_NAME
 
 
 class TempMMapArray(np.ndarray):
     """A np.ndarray with path attribute for a temporary mmapped buffer."""
 
     def __new__(cls, input_array, _path):
```

### Comparing `alphatims-1.0.7/alphatims/utils.py` & `alphatims-1.0.8/alphatims/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,16 +160,18 @@
     logging.info(f"processor     - {platform.processor()}")
     logging.info(
         f"cpu count     - {psutil.cpu_count()}"
         # f" ({100 - psutil.cpu_percent()}% unused)"
     )
 
     # check if architecture is arm64 as psutil.cpu_freq() is not yet supported on apple silicon
-    if platform.machine() != 'arm64':
+    try:
         logging.info(f"cpu frequency - {psutil.cpu_freq().current:.2f} Mhz")
+    except AttributeError:
+        logging.info("Unable to log cpu frequency")
     logging.info(
         f"ram           - "
         f"{psutil.virtual_memory().available/1024**3:.1f}/"
         f"{psutil.virtual_memory().total/1024**3:.1f} Gb "
         f"(available/total)"
     )
     logging.info("")
```

### Comparing `alphatims-1.0.7/alphatims.egg-info/PKG-INFO` & `alphatims-1.0.8/alphatims.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphatims
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python package to index Bruker TimsTOF raw data for fast and easy accession and visualization
 Home-page: https://github.com/MannLabs/alphatims
 Author: Sander Willems, Eugenia Voytik
 Author-email: opensource@alphapept.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -51,15 +51,15 @@
   * [**Installation**](#installation)
      * [**One-click GUI**](#one-click-gui)
      * [**Pip installer**](#pip)
      * [**Developer installer**](#developer)
      * [**Installation issues**](#installation-issues)
   * [**Test data**](#test-data)
     * [**Test sample**](#test-sample)
-    * [**LC**](#lc)  
+    * [**LC**](#lc)
     * [**DDA**](#dda)
     * [**DIA**](#dia)
   * [**Usage**](#usage)
     * [**GUI**](#gui)
     * [**CLI**](#cli)
     * [**Python and jupyter notebooks**](#python-and-jupyter-notebooks)
     * [**Other tools**](#other-tools)
@@ -97,14 +97,15 @@
 
 AlphaTims can be installed and used on all major operating systems (Windows, macOS and Linux).
 There are three different types of installation possible:
 
 * [**One-click GUI installer:**](#one-click-gui) Choose this installation if you only want the GUI and/or keep things as simple as possible.
 * [**Pip installer:**](#pip) Choose this installation if you want to use AlphaTims as a Python package in an existing Python 3.8 environment (e.g. a Jupyter notebook). If needed, the GUI and CLI can be installed with pip as well.
 * [**Developer installer:**](#developer) Choose this installation if you are familiar with CLI tools, [conda](https://docs.conda.io/en/latest/) and Python. This installation allows access to all available features of AlphaTims and even allows to modify its source code directly. Generally, the developer version of AlphaTims outperforms the precompiled versions which makes this the installation of choice for high-throughput experiments.
+* [**Docker:**](#docker) Use this installation if you want to use a container based workflow. This is usefull to preserve a clean environment or when running multiple tools that might have conflicting dependencies.
 
 ***IMPORTANT: While AlphaTims is mostly platform independent, some calibration functions require [Bruker libraries](alphatims/ext) which are only available on Windows and Linux.***
 
 ### One-click GUI
 
 The GUI of AlphaTims is a completely stand-alone tool that requires no knowledge of Python or CLI tools. Click on one of the links below to download the latest release for:
 
@@ -210,14 +211,22 @@
   alphatims_bin="$(which alphatims)"
   echo "alias alphatims='"${alphatims_bin}"'" >> ~/.bashrc
   conda deactivate
   ```
   When `zsh` is the default terminal instead of `bash`, replace `~/.bashrc` with `~/.zshrc`. On Windows, the command `where alphatims` can be used to find the location of the binary executable. This path can then be (permanently) added to Windows' path variable.
 * When using Jupyter notebooks and multiple conda environments direcly from the terminal, it is recommended to `conda install nb_conda_kernels` in the conda base environment. Hereafter, running a `jupyter notebook` from the conda base environment should have a `python [conda env: alphatims]` kernel available, in addition to all other conda kernels in which the command `conda install ipykernel` was run.
 
+### Docker
+
+(WIP)
+
+```shell
+docker pull ghcr://MannLabs/alphatims:latest
+```
+
 ### Installation issues
 
 See the general [troubleshooting](#troubleshooting) section.
 
 ---
 ## Test data
 
@@ -349,14 +358,15 @@
 * **AlphaTims is not found.** Make sure you use the right folder. Local folders are best called by prefixing them with `./` (e.g. `pip install "./alphatims"`). On some systems, installation specifically requires (not) to use single quotes `'` around the AlphaTims folder, e.g. `pip install "./alphatims[plotting-stable,development]"`.
 * **Modifications to the AlphaTims source code are not reflected.** Make sure you use the `-e` flag when using `pip install -e alphatims`.
 * **Numpy does not work properly.** On Windows, `numpy==1.19.4` has some issues. After installing AlphaTims, downgrade NumPy with `pip install numpy==1.19.3`.
 * **Exporting PNG images with the CLI or Python package might not work out-of-the-box**. If a conda environment is used, this can be fixed by running `conda install -c conda-forge firefox geckodriver` in the AlphaTims conda environment. Alternatively, a file can be exported as html and opened in a browser. From the browser there is a `save as png` button available.
 * **GUI does not open.** In some cases this can be simply because of using an incompatible (default) browser. AlphaTims has been tested with Google Chrome and Mozilla Firefox. Windows IE and Windows Edge compatibility is not guaranteed.
 * **When older Bruker files need to be processed as well,** the [legacy dependencies](requirements/requirements_legacy.txt) are also needed. However, note that this requires [Microsoft Visual C++](https://visualstudio.microsoft.com/visual-cpp-build-tools) to be manually installed (on Windows machines) prior to AlphaTims installation! To include the legacy dependencies, install AlphaTims with `pip install "alphatims[legacy]"` or `pip install "alphatims[legacy]" --upgrade` if already pre-installed.
 * **When installed through `pip`, the GUI cannot be started.** Make sure you install AlphaTims with `pip install "alphatims[plotting-stable]"` to include the GUI with stable dependancies. If this was done and it still fails to run the GUI, a possible fix might be to run `pip install panel==0.10.3` after AlphaTims was installed.
+* **Some external libraries are missing.** On some OS, there might be libraries missing. As an exmaple, the following error message might pop up: `OSError: libgomp.so.1: cannot open shared object file: No such file or directory`. This can be solved by installing those manually, e.g. on Linux: `apt-get install libgomp1`.
 
 ---
 ## How it works
 
 The basic workflow of AlphaTims looks as follows:
 
 * Read data from a [Bruker `.d` folder](#bruker-raw-data).
```

### Comparing `alphatims-1.0.7/alphatims.egg-info/SOURCES.txt` & `alphatims-1.0.8/alphatims.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 alphatims/docs/cli_manual.pdf
 alphatims/docs/gui_manual.pdf
 alphatims/ext/timsdata.dll
 alphatims/ext/timsdata.so
 alphatims/img/github.png
 alphatims/img/max-planck-gesellschaft.jpg
 alphatims/img/mpi_logo.png
-alphatims/lib/interface_parameters.json
+alphatims/lib/interface_parameters.json
+tests/test_bruker.py
+tests/test_utils.py
```

### Comparing `alphatims-1.0.7/alphatims.egg-info/requires.txt` & `alphatims-1.0.8/alphatims.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alphatims-1.0.7/setup.py` & `alphatims-1.0.8/setup.py`

 * *Files identical despite different names*

