# Comparing `tmp/GOES-3.3.tar.gz` & `tmp/GOES-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GOES-3.3.tar", last modified: Sun Mar 14 04:26:07 2021, max compression
+gzip compressed data, was "GOES-3.4.tar", last modified: Sun Jul 23 23:34:26 2023, max compression
```

## Comparing `GOES-3.3.tar` & `GOES-3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2021-03-14 04:26:07.000000 GOES-3.3/
--rw-rw-r--   0 joao      (1000) joao      (1000)     2937 2021-03-14 04:26:07.000000 GOES-3.3/PKG-INFO
--rw-r--r--   0 joao      (1000) joao      (1000)     1776 2021-03-14 04:22:18.000000 GOES-3.3/README.md
--rw-r--r--   0 joao      (1000) joao      (1000)      843 2021-03-14 02:34:44.000000 GOES-3.3/setup.py
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2021-03-14 04:26:07.000000 GOES-3.3/setup.cfg
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2021-03-14 04:26:07.000000 GOES-3.3/GOES.egg-info/
--rw-rw-r--   0 joao      (1000) joao      (1000)     2937 2021-03-14 04:26:06.000000 GOES-3.3/GOES.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)        5 2021-03-14 04:26:06.000000 GOES-3.3/GOES.egg-info/top_level.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       35 2021-03-14 04:26:06.000000 GOES-3.3/GOES.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2021-03-14 04:26:06.000000 GOES-3.3/GOES.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)      296 2021-03-14 04:26:07.000000 GOES-3.3/GOES.egg-info/SOURCES.txt
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2021-03-14 04:26:07.000000 GOES-3.3/GOES/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2021-03-14 04:26:07.000000 GOES-3.3/GOES/downloads/
--rwxrwxr-x   0 joao      (1000) joao      (1000)       68 2021-03-14 02:39:20.000000 GOES-3.3/GOES/downloads/__init__.py
--rwxrwxr-x   0 joao      (1000) joao      (1000)    13495 2021-03-14 02:39:37.000000 GOES-3.3/GOES/downloads/download_data.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2021-03-14 04:26:07.000000 GOES-3.3/GOES/processing/
--rwxrwxr-x   0 joao      (1000) joao      (1000)       71 2021-03-14 02:38:27.000000 GOES-3.3/GOES/processing/__init__.py
--rwxrwxr-x   0 joao      (1000) joao      (1000)    68287 2021-03-14 02:15:36.000000 GOES-3.3/GOES/processing/processing_data.py
--rw-r--r--   0 joao      (1000) joao      (1000)      547 2021-03-14 02:37:50.000000 GOES-3.3/GOES/__init__.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.962185 GOES-3.4/GOES/
+-rw-r--r--   0 joao      (1000) joao      (1000)      547 2023-07-23 23:26:59.000000 GOES-3.4/GOES/__init__.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/GOES/downloads/
+-rwxrwxr-x   0 joao      (1000) joao      (1000)       68 2023-07-23 22:20:48.000000 GOES-3.4/GOES/downloads/__init__.py
+-rwxr--r--   0 joao      (1000) joao      (1000)    14839 2023-07-23 22:21:15.000000 GOES-3.4/GOES/downloads/download_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.966185 GOES-3.4/GOES/processing/
+-rwxr--r--   0 joao      (1000) joao      (1000)       71 2023-07-23 22:20:05.000000 GOES-3.4/GOES/processing/__init__.py
+-rwxr--r--   0 joao      (1000) joao      (1000)    68347 2023-07-23 22:22:30.000000 GOES-3.4/GOES/processing/processing_data.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2023-07-23 23:34:26.962185 GOES-3.4/GOES.egg-info/
+-rw-rw-r--   0 joao      (1000) joao      (1000)     2503 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      304 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       46 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        5 2023-07-23 23:34:26.000000 GOES-3.4/GOES.egg-info/top_level.txt
+-rw-r--r--   0 joao      (1000) joao      (1000)     1535 2021-04-18 02:25:14.000000 GOES-3.4/LICENSE
+-rw-rw-r--   0 joao      (1000) joao      (1000)     2503 2023-07-23 23:34:26.966185 GOES-3.4/PKG-INFO
+-rw-r--r--   0 joao      (1000) joao      (1000)     1965 2023-07-23 23:13:36.000000 GOES-3.4/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2023-07-23 23:34:26.966185 GOES-3.4/setup.cfg
+-rw-r--r--   0 joao      (1000) joao      (1000)      865 2023-07-23 20:45:57.000000 GOES-3.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `GOES-3.3/README.md` & `GOES-3.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # GOES
-[![pypi](https://img.shields.io/badge/pypi-v3.3-brightgreen.svg)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
+[![pypi](https://img.shields.io/badge/pypi-v3.4-brightgreen)](https://pypi.org/project/GOES/) [![DOI](https://zenodo.org/badge/213261768.svg)](https://zenodo.org/badge/latestdoi/213261768)
 
-Python packages to download and manipulate GOES-16/17 data.
+Python package to download and manipulate GOES-16/17/18 data.
 <br><br>
 
 # Version
-3.3
+3.4
 <br><br>
-If you have already installed the GOES package, check that you have the latest version.
+If you have already installed the GOES package, update it to the latest version.
 <br><br>
 
 # Requirements
+The main packages required are:
 - [numpy](https://numpy.org/)
 - [s3fs](https://s3fs.readthedocs.io/en/latest/install.html)
 - [pyproj](https://github.com/pyproj4/pyproj)
 - [netCDF4](http://unidata.github.io/netcdf4-python/)
 - [requests](https://2.python-requests.org/en/master/)
 
 **Tip**: If you install the GOES package using pip, you don't need to worry about installing these packages because they will be installed automatically.
 <br><br>
 
-# Usage
+# Tutorial
 Find the jupyter notebook examples for the last version [here](https://github.com/joaohenry23/GOES/blob/master/examples/index.ipynb).
 <br><br>
 
 # Installation
-You can install **GOES** on Python 2 or 3 on Linux, Windows or other, using the following commands.
+You can install **GOES** on Python 2 or 3 on Linux, Windows or other using the following commands.
 <br><br>
-**Using PIP** (recommended):
+**Using pip** (recommended):
 ```
 pip install GOES
 
 ```
 
 Check if package was installed with:
 
@@ -53,25 +54,29 @@
 cd GOES
 python setup.py install
 
 ```
 <br>
 
 **Using python**:\
-Download **GOES-master.zip** from github and following the next commands:
+Download the **GOES-master.zip** from github and following the next commands:
 ```
 unzip GOES-master.zip
 cd GOES-master
 python setup.py install
 
 ```
+<br>
+
+# Change log
+All notable changes to this project will be documented in this [file](https://github.com/joaohenry23/GOES/blob/master/CHANGELOG.md).
 <br><br>
 
 # Support
 If you have any questions, do not hesitate to write to:
 ```
 joaohenry23@gmail.com
 
 ```
 You can write to me in spanish, portuguese or english.
-
+<br><br>
```

### Comparing `GOES-3.3/setup.py` & `GOES-3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import setuptools
 
 with open("README.md", "r") as fh:
    long_description = fh.read()
 
 setuptools.setup(
    name="GOES",
-   version="3.3",
+   version="3.4",
    author="Joao Henry Huamán Chinchay",
    author_email="joaohenry23@gmail.com",
-   description="Python packages to download and manipulate GOES-16/17 data.",
+   description="Python package to download and manipulate GOES-16/17/18 data.",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://github.com/joaohenry23/GOES",
    license='BSD 3-Clause',
    packages=setuptools.find_packages(),
    classifiers=[
       "Programming Language :: Python :: 2",
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
       "Operating System :: OS Independent",
    ],
    python_requires='>=2.7',
    install_requires=[
       "numpy",
+      "cftime>1.1",
       "requests",
       "s3fs",
       "pyproj",
       "netCDF4",
    ],
 )
```

### Comparing `GOES-3.3/GOES/downloads/download_data.py` & `GOES-3.4/GOES/downloads/download_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------------------------------------------------------------
 '''
 Description: Downloads GOES-16/17 data from amazon
 Author: Joao Henry Huaman Chinchay
 E-mail: joaohenry23@gmail.com
 Created date: Mar 23, 2020
-Modification date: Feb 23, 2021
+Modification date: Jul 23, 2023
 '''
 #-----------------------------------------------------------------------------------------------------------------------------------
 import numpy as np
 import s3fs
 from datetime import *
 import requests
+import os
 
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 
 #-----------------------------------------------------------------------------------------------------------------------------------
 def show_products():
 
     '''
 
-    Lists the products available from GOES-16 and GOES-17.
+    Lists the products available from GOES-16, GOES-17 and GOES-18.
 
     '''
 
-    Satellite = ['goes16','goes17']
+    Satellite = ['goes16','goes17','goes18']
     print(' ')
     for sat in Satellite:
         print('Products for '+sat+':')
         fs = s3fs.S3FileSystem(anon=True)
         for item in fs.ls('s3://noaa-'+sat+'/'):
             if item.split('/')[-1] == 'index.html':
                 print(' ')
             else:
                 print('\t'+item.split('/')[-1])
 
     print('Descriptions of each product is shown in https://docs.opendata.aws/noaa-goes16/cics-readme.html#about-the-data \n')
 
 #-----------------------------------------------------------------------------------------------------------------------------------
-def download_file(URL, name_file, path_out, retries=10, backoff=10, size_format='Decimal', show_download_progress=True):
+def download_file(URL, name_file, path_out, retries=10, backoff=0.2, size_format='Decimal', show_download_progress=True, overwrite_file=False):
 
     '''
 
     Save data in file.
 
     Parameters
     ----------
@@ -56,28 +57,34 @@
     path_out : str, optional, default ''
         Path of folder where file will be saved.
 
     retries : int, optional, default 10
         Defines the retries number to connect to server.
         See: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
 
-    backoff: int, optional, default 10
+    backoff: int, optional, default 0.2
         A backoff factor to apply between attempts after the second try.
         See: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
 
 
     size_format: str, optional, default 'Decimal'
         Defines how is print the size of file.
         Options are:
             'Decimal' : divide file size (in bytes) by (1000*1000) 
             'Binary' : divide file size (in bytes) by (1024*1024)
 
     show_download_progress : boolean, optional, default True
         Parameter to enable and disable the visualization of download progress.
 
+    overwrite_file : boolean, optional, default False
+        Parameter to overwrite or keep a file already downloaded.
+        If overwrite_file=False the downloaded file is keep.
+        If overwrite_file=True the downloaded file is overwrite (the file is
+        downloaded again).
+
     '''
 
     StartTime = datetime.now()
 
     retries_config = Retry(total=retries, backoff_factor=backoff, status_forcelist=[500, 502, 503, 504])
 
     session = requests.Session()
@@ -88,42 +95,58 @@
     total_size = int(req.headers['content-length'])
     size = 0
     if size_format == 'Binary':
         dsize = 1024*1024
     else:
         dsize = 1000*1000
 
-    with open(path_out+name_file,'wb') as output_file:
-        for chunk in req.iter_content(chunk_size=1024):
-            if chunk:
-                rec_size = output_file.write(chunk)
-                size = rec_size + size
-                if show_download_progress==True:
-                    print('  {} {:3.0f}% {:.1f}MB {}'.format(name_file,100.0*size/total_size, size/dsize, '{}m{}s'.format(round((datetime.now()-StartTime).seconds/60.0),(datetime.now()-StartTime).seconds%60) if (datetime.now()-StartTime).seconds>60 else '{}s'.format((datetime.now()-StartTime).seconds) ), end="\r") #, flush=True)
-                    #print('\t{}\t{:3.0f}%\t{:.2f} min'.format(name_file,100.0*size/total_size, (datetime.now()-StartTime).seconds/60.0), end="\r") #, flush=True)
-                    if size == total_size:
-                        #print('\n')
-                        print('  {} {:3.0f}% {:.1f}MB {}'.format(name_file,100.0*size/total_size, size/dsize, '{}m{}s'.format(round((datetime.now()-StartTime).seconds/60.0),(datetime.now()-StartTime).seconds%60) if (datetime.now()-StartTime).seconds>60 else '{}s'.format((datetime.now()-StartTime).seconds) ))
+
+    make_download = True
+
+    if os.path.isfile(path_out+name_file)==True:
+        if os.path.getsize(path_out+name_file)==total_size:
+            if overwrite_file==False:
+                print('  {} already exists.'.format(name_file))
+                make_download = False
+            else:
+                print('  {} will be overwritten.'.format(name_file))
+                make_download = True
+        else:
+            make_download = True
+
+
+    if make_download == True:
+        with open(path_out+name_file,'wb') as output_file:
+            for chunk in req.iter_content(chunk_size=1024):
+                if chunk:
+                    rec_size = output_file.write(chunk)
+                    size = rec_size + size
+                    if show_download_progress==True:
+                        print('  {} {:3.0f}% {:.1f}MB {}'.format(name_file,100.0*size/total_size, size/dsize, '{}m{}s'.format(round((datetime.now()-StartTime).seconds/60.0),(datetime.now()-StartTime).seconds%60) if (datetime.now()-StartTime).seconds>60 else '{}s'.format((datetime.now()-StartTime).seconds) ), end="\r") #, flush=True)
+                        #print('\t{}\t{:3.0f}%\t{:.2f} min'.format(name_file,100.0*size/total_size, (datetime.now()-StartTime).seconds/60.0), end="\r") #, flush=True)
+                        if size == total_size:
+                            #print('\n')
+                            print('  {} {:3.0f}% {:.1f}MB {}'.format(name_file,100.0*size/total_size, size/dsize, '{}m{}s'.format(round((datetime.now()-StartTime).seconds/60.0),(datetime.now()-StartTime).seconds%60) if (datetime.now()-StartTime).seconds>60 else '{}s'.format((datetime.now()-StartTime).seconds) ))
 
     #print('\b')
 
 #-----------------------------------------------------------------------------------------------------------------------------------
-def download(Satellite, Product, DateTimeIni=None, DateTimeFin=None, domain=None, channel=None, rename_fmt=False, path_out='', retries=10, backoff=10, size_format='Decimal', show_download_progress=True):
+def download(Satellite, Product, DateTimeIni=None, DateTimeFin=None, domain=None, channel=None, rename_fmt=False, path_out='', retries=10, backoff=10, size_format='Decimal', show_download_progress=True, overwrite_file=False):
 
     '''
 
-    Download data of GOES-16 and GOES-17 from Amazon server.
+    Download data of GOES-16, GOES-17 and GOES-18 from Amazon server.
     This function is based on the code of
     blaylockbk https://gist.github.com/blaylockbk/d60f4fce15a7f0475f975fc57da9104d
 
 
     Parameters
     ----------
     Satellite : str
-        Indicates serie of GOES, the options are 'goes16' and 'goes17'
+        Indicates serie of GOES, the options are 'goes16', 'goes17' and 'goes18'
 
 
     Product : str
         Indicates the instrument and level of product. The products
         can be list using: GOES.show_products()
 
 
@@ -189,32 +212,41 @@
         Options are:
             'Decimal' : divide file size (in bytes) by (1000*1000) 
             'Binary' : divide file size (in bytes) by (1024*1024)
 
     show_download_progress : boolean, optional, default True
         Parameter to enable and disable the visualization of download progress.
 
+    overwrite_file : boolean, optional, default False
+        Parameter to overwrite or keep a file already downloaded.
+        If overwrite_file=False the downloaded file is keep.
+        If overwrite_file=True the downloaded file is overwrite (the file is
+        downloaded again).
+
+
     Return
     ------
     Download_files : list
         List with the downloaded files (path+filename).
 
     '''
 
     # ---------- Satellite -------------------
     try:
-        assert Satellite == 'goes16' or Satellite == 'goes17'
+        assert Satellite == 'goes16' or Satellite == 'goes17' or Satellite == 'goes18'
     except AssertionError:
-        print('\nSatellite should be goes16 or goes17\n')
+        print('\nSatellite should be goes16, goes17 or goes18\n')
         return
     else:
         if Satellite == 'goes16':
             Sat = 'G16'
         elif Satellite == 'goes17':
             Sat = 'G17'
+        elif Satellite == 'goes18':
+            Sat = 'G18'
 
     # ---------- Product and Domain -------------------
     if Product[-1] == 'M':
         try:
             assert domain == 'M1' or domain == 'M2'
         except AssertionError:
             print("\nProduct domain is mesoscale so you need define domain='M1' or domain='M2'\n")
@@ -313,30 +345,30 @@
 
                     if rename_fmt == False:
                         NameOut = NameFile
                     else:
                         NameOut = NameFile[:NameFile.find('_s')+2] + DateTimeFile.strftime(rename_fmt) + '.nc'
 
                     #print(ChannelFile, DateTimeFile, NameOut)
-                    download_file('https://noaa-'+Satellite+'.s3.amazonaws.com'+line[len('noaa-'+Satellite):], NameOut, path_out, retries=retries, backoff=backoff, size_format=size_format, show_download_progress=show_download_progress)
+                    download_file('https://noaa-'+Satellite+'.s3.amazonaws.com'+line[len('noaa-'+Satellite):], NameOut, path_out, retries=retries, backoff=backoff, size_format=size_format, show_download_progress=show_download_progress, overwrite_file=overwrite_file)
                     Downloaded_files.append(path_out+NameOut)
 
             else:
                 NameFile = line.split('/')[-1]
                 DateTimeFile = datetime.strptime(NameFile[NameFile.find('_s')+2:NameFile.find('_e')-1], '%Y%j%H%M%S')
 
                 if Product2 in NameFile    and    DateTimeIni <= DateTimeFile <= DateTimeFin:
 
                     if rename_fmt == False:
                         NameOut = NameFile
                     else:
                         NameOut = NameFile[:NameFile.find('_s')+2] + DateTimeFile.strftime(rename_fmt) + '.nc'
 
                     #print(DateTimeFile, NameOut)
-                    download_file('https://noaa-'+Satellite+'.s3.amazonaws.com'+line[len('noaa-'+Satellite):], NameOut, path_out, retries=retries, backoff=backoff, size_format=size_format, show_download_progress=show_download_progress)
+                    download_file('https://noaa-'+Satellite+'.s3.amazonaws.com'+line[len('noaa-'+Satellite):], NameOut, path_out, retries=retries, backoff=backoff, size_format=size_format, show_download_progress=show_download_progress, overwrite_file=overwrite_file)
                     Downloaded_files.append(path_out+NameOut)
 
         DateTimeIniLoop = DateTimeIniLoop + timedelta(minutes=60)
 
     Downloaded_files.sort()
 
     return Downloaded_files;
```

### Comparing `GOES-3.3/GOES/processing/processing_data.py` & `GOES-3.4/GOES/processing/processing_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------------------------------------------------------------
 '''
 Description: Process the GOES-16/17 data
 Author: Joao Henry Huaman Chinchay
 E-mail: joaohenry23@gmail.com
 Created date: Mar 23, 2020
-Modification date: Mar 13, 2021
+Modification date: Jul 23, 2023
 '''
 #-----------------------------------------------------------------------------------------------------------------------------------
 import numpy as np
 from netCDF4 import Dataset, num2date
 from pyproj import Proj
 import datetime
 import glob
@@ -1078,15 +1078,15 @@
         angle in radians.
 
     Y : ndarray
         A scalar 1-D array with the fixed grid North/South scanning
         angle in radians.
 
     PlatformID : str
-        Platform ID of satelite. Example: 'G16' or 'G17'.
+        Platform ID of satelite. Example: 'G16', 'G17' or 'G18'.
 
     SatLon : float
         Longitude of satellite in the nadir.
 
     SatHeight : float
         Height of satellite in meters.
 
@@ -1111,15 +1111,15 @@
 
     X = X[:]*SatHeight
     Y = Y[:]*SatHeight
     X, Y = np.meshgrid(X, Y)
     proj = Proj(proj='geos', h=SatHeight, lon_0=SatLon, sweep=SatSweep)
     Lons, Lats = proj(X, Y, inverse=True)
 
-    if PlatformID == 'G17':
+    if PlatformID == 'G17' or PlatformID == 'G18':
         Lons = np.where(Lons>0,Lons-360,Lons)
 
     Lons = np.where((Lons>=-360.0)&(Lons<=360.0)&(Lats>=-90.0)&(Lats<=90.0),Lons,-999.99).astype(fmt)
     Lats = np.where((Lons>=-360.0)&(Lons<=360.0)&(Lats>=-90.0)&(Lats<=90.0),Lats,-999.99).astype(fmt)
 
     dict_Lons = {'long_name':'Longitude of center of pixels', 'standard_name':'pixels center longitude',
                  'units':'degrees_east', 'undef':-999.99, 'axis':'YX', 'dimensions':('y','x'), 'data':Lons}
@@ -1147,15 +1147,15 @@
         angle in radians.
 
     Y : ndarray
         A scalar 1-D array with the fixed grid North/South scanning
         angle in radians.
 
     PlatformID : str
-        Platform ID of satelite. Example: 'G16' or 'G17'.
+        Platform ID of satelite. Example: 'G16', 'G17' or 'G18'.
 
     SatLon : float
         Longitude of satellite in the nadir.
 
     SatHeight : float
         Height of satellite in meters.
 
@@ -1184,15 +1184,15 @@
     dy = Y[1]-Y[0]
     XCor = np.concatenate([X, [X[-1]+dx]])-dx/2
     YCor = np.concatenate([Y, [Y[-1]+dy]])-dy/2
     XCor, YCor = np.meshgrid(XCor, YCor)
     proj = Proj(proj='geos', h=SatHeight, lon_0=SatLon, sweep=SatSweep)
     Lons, Lats = proj(XCor, YCor, inverse=True)
 
-    if PlatformID == 'G17':
+    if PlatformID == 'G17' or PlatformID == 'G18':
         Lons = np.where(Lons>0,Lons-360,Lons)
 
     Lons = np.where((Lons>=-360.0)&(Lons<=360.0)&(Lats>=-90.0)&(Lats<=90.0),Lons,-999.99).astype(fmt)
     Lats = np.where((Lons>=-360.0)&(Lons<=360.0)&(Lats>=-90.0)&(Lats<=90.0),Lats,-999.99).astype(fmt)
 
     dict_Lons = {'long_name':'Longitude of corners of pixels', 'standard_name':'pixels corners longitude',
                  'units':'degrees_east', 'undef':-999.99, 'axis':'YX', 'dimensions':('y','x'), 'data':Lons}
```

### Comparing `GOES-3.3/GOES/__init__.py` & `GOES-3.4/GOES/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,8 @@
            'GOES', 'open_dataset', 'open_mfdataset',
            'get_lonlat','get_lonlatcorner','corner_size_to_center_size',
            'midpoint_in_x','midpoint_in_y','calculate_corners',
            'find_pixel_of_coordinate',
            'cosine_of_solar_zenith_angle',
            'find_pixels_of_region','create_gridmap',
            'locate_files','accumulate_in_gridmap']
-__version__ = '3.3'
+__version__ = '3.4'
```

