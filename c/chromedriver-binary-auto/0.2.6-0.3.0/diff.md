# Comparing `tmp/chromedriver-binary-auto-0.2.6.tar.gz` & `tmp/chromedriver-binary-auto-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-binary-auto-0.2.6.tar", last modified: Wed May  3 13:04:54 2023, max compression
+gzip compressed data, was "chromedriver-binary-auto-0.3.0.tar", last modified: Mon Jul 24 15:13:53 2023, max compression
```

## Comparing `chromedriver-binary-auto-0.2.6.tar` & `chromedriver-binary-auto-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2722 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/chromedriver_binary/
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4602 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2722 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-03 13:04:54.000000 chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 13:04:54.351110 chromedriver-binary-auto-0.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-05-03 13:04:53.000000 chromedriver-binary-auto-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/chromedriver_binary/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6882 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-24 15:13:53.000000 chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:13:53.602626 chromedriver-binary-auto-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-24 15:13:52.000000 chromedriver-binary-auto-0.3.0/setup.py
```

### Comparing `chromedriver-binary-auto-0.2.6/LICENSE` & `chromedriver-binary-auto-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.6/PKG-INFO` & `chromedriver-binary-auto-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.2.6
+Version: 0.3.0
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.2.6/README.md` & `chromedriver-binary-auto-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.6/chromedriver_binary/__init__.py` & `chromedriver-binary-auto-0.3.0/chromedriver_binary/__init__.py`

 * *Files identical despite different names*

### Comparing `chromedriver-binary-auto-0.2.6/chromedriver_binary/utils.py` & `chromedriver-binary-auto-0.3.0/chromedriver_binary/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
 Helper functions for filename and URL generation.
 """
-
+import json
 import sys
 import os
 import ssl
 import subprocess
 import re
 import platform
 
@@ -36,18 +36,17 @@
     :return: Environment variable separator
     """
     if sys.platform.startswith('win'):
         return ';'
     return ':'
 
 
-def get_chromedriver_url(version):
+def get_legacy_chromedriver_url(version):
     """
-    Generates the download URL for current platform , architecture and the given version.
-    Supports Linux, MacOS and Windows.
+    Generates the download URL for legacy releases
     :param version: chromedriver version string
     :return: Download URL for chromedriver
     """
     base_url = 'https://chromedriver.storage.googleapis.com/'
     if sys.platform.startswith('linux') and sys.maxsize > 2 ** 32:
         _platform = 'linux'
         architecture = '64'
@@ -63,14 +62,42 @@
         _platform = 'win'
         architecture = '32'
     else:
         raise RuntimeError('Could not determine chromedriver download URL for this platform.')
     return base_url + version + '/chromedriver_' + _platform + architecture + '.zip'
 
 
+def get_chromedriver_url(version):
+    """
+    Generates the download URL for current platform, architecture and the given version.
+    Supports Linux, macOS and Windows.
+    :param version: chromedriver version string
+    :return: Download URL for chromedriver
+    """
+    if sys.platform.startswith('linux') and sys.maxsize > 2 ** 32:
+        _platform = 'linux64'
+    elif sys.platform == 'darwin' and platform.machine() == 'arm64':
+        _platform = 'mac-arm64'
+    elif sys.platform == 'darwin':
+        _platform = 'mac-x64'
+    elif sys.platform.startswith('win'):
+        _platform = 'win' + '64' if sys.maxsize > 2 ** 32 else '32'
+    else:
+        raise RuntimeError('Could not determine chromedriver download URL for this platform.')
+    response = urlopen("https://googlechromelabs.github.io/chrome-for-testing/latest-patch-versions-per-build-with-downloads.json", context=ssl_context)
+    if int(version.split('.')[0]) >= 115:
+        version = '.'.join(version.split('.')[:3])  # ensure major.minor.patch
+        for p in json.load(response)["builds"][version]["downloads"]["chromedriver"]:
+            if p["platform"] == _platform:
+                return p["url"]
+    else:
+        return get_legacy_chromedriver_url(version)
+    raise RuntimeError('Could not determine chromedriver download URL for this platform.')
+
+
 def find_binary_in_path(filename):
     """
     Searches for a binary named `filename` in the current PATH. If an executable is found, its absolute path is returned
     else None.
     :param filename: Filename of the binary
     :return: Absolute path or None
     """
@@ -79,18 +106,17 @@
     for directory in os.environ['PATH'].split(get_variable_separator()):
         binary = os.path.abspath(os.path.join(directory, filename))
         if os.path.isfile(binary) and os.access(binary, os.X_OK):
             return binary
     return None
 
 
-def get_latest_release_for_version(version=None):
+def get_latest_legacy_release_for_version(version):
     """
-    Searches for the latest release (complete version string) for a given major `version`. If `version` is None
-    the latest release is returned.
+    Searches for the latest release (complete version string) for a given major `version` in the legacy storage.
     :param version: Major version number or None
     :return: Latest release for given version
     """
     release_url = "https://chromedriver.storage.googleapis.com/LATEST_RELEASE"
     if version:
         release_url += '_{}'.format(version)
     try:
@@ -98,14 +124,33 @@
         if response.getcode() != 200:
             raise URLError('Not Found')
         return response.read().decode('utf-8').strip()
     except URLError:
         raise RuntimeError('Failed to find release information: {}'.format(release_url))
 
 
+def get_latest_release_for_version(version=None):
+    """
+    Searches for the latest release (complete version string) for a given major `version`. If `version` is None
+    the latest Stable release is returned.
+    :param version: Major version number or None
+    :return: Latest release for given version
+    """
+    try:
+        if version is None:
+            response = urlopen("https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions.json", context=ssl_context)
+            return json.load(response)["channels"]["Stable"]["version"]
+        if int(version) < 113:
+            return get_latest_legacy_release_for_version(version)
+        response = urlopen("https://googlechromelabs.github.io/chrome-for-testing/latest-versions-per-milestone-with-downloads.json", context=ssl_context)
+        return json.load(response)["milestones"][str(version)]["version"]
+    except Exception:
+        raise RuntimeError('Failed to find release information for version: {}'.format(version if version else "latest"))
+
+
 def get_chrome_major_version():
     """
     Detects the major version number of the installed chrome/chromium browser.
     :return: The browsers major version number or None
     """
     browser_executables = ['google-chrome', 'chrome', 'chrome-browser', 'google-chrome-stable', 'chromium', 'chromium-browser']
     if sys.platform == "darwin":
```

### Comparing `chromedriver-binary-auto-0.2.6/chromedriver_binary_auto.egg-info/PKG-INFO` & `chromedriver-binary-auto-0.3.0/chromedriver_binary_auto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-binary-auto
-Version: 0.2.6
+Version: 0.3.0
 Summary: Installer for chromedriver.
 Home-page: https://github.com/danielkaiser/python-chromedriver-binary
 Author: Daniel Kaiser
 Author-email: daniel.kaiser94@gmail.com
 License: MIT
 Keywords: chromedriver chrome browser selenium splinter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `chromedriver-binary-auto-0.2.6/setup.py` & `chromedriver-binary-auto-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,25 +49,29 @@
                     response = urlopen(url, context=ssl_context)
                     if response.getcode() != 200:
                         raise URLError('Not Found')
                 except URLError:
                     raise RuntimeError('Failed to download chromedriver archive: {}'.format(url))
                 archive = BytesIO(response.read())
                 with zipfile.ZipFile(archive) as zip_file:
-                    zip_file.extract(chromedriver_bin, chromedriver_dir)
+                    for filename in zip_file.namelist():
+                        zip_file.extract(filename, chromedriver_dir)
+                        path_elements = os.path.split(filename)
+                        if len(path_elements) > 1:
+                            os.rename(os.path.join(chromedriver_dir, filename), os.path.join(chromedriver_dir, path_elements[-1]))
             else:
                 print("\nChromedriver already installed at {}...\n".format(chromedriver_filename))
             if not os.access(chromedriver_filename, os.X_OK):
                 os.chmod(chromedriver_filename, 0o744)
         build_py.run(self)
 
 
 setup(
     name="chromedriver-binary-auto",
-    version="0.2.6",
+    version="0.3.0",
     author="Daniel Kaiser",
     author_email="daniel.kaiser94@gmail.com",
     description="Installer for chromedriver.",
     license="MIT",
     keywords="chromedriver chrome browser selenium splinter",
     url="https://github.com/danielkaiser/python-chromedriver-binary",
     packages=['chromedriver_binary'],
```

