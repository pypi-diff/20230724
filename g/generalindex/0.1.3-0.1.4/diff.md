# Comparing `tmp/generalindex-0.1.3.tar.gz` & `tmp/generalindex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/generalindex-0.1.3.tar", last modified: Mon Oct 24 11:32:47 2022, max compression
+gzip compressed data, was "generalindex-0.1.4.tar", last modified: Mon Jul 24 14:04:56 2023, max compression
```

## Comparing `generalindex-0.1.3.tar` & `generalindex-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2022-10-24 11:32:47.232727 generalindex-0.1.3/
--rw-r--r--   0 Izabella   (502) staff       (20)     1055 2022-10-24 07:32:17.000000 generalindex-0.1.3/LICENSE
--rw-r--r--   0 Izabella   (502) staff       (20)    26675 2022-10-24 11:32:47.232546 generalindex-0.1.3/PKG-INFO
--rw-r--r--   0 Izabella   (502) staff       (20)    26234 2022-10-24 11:32:46.000000 generalindex-0.1.3/README.md
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2022-10-24 11:32:47.231497 generalindex-0.1.3/generalindex/
--rw-r--r--   0 Izabella   (502) staff       (20)     1112 2022-10-24 08:58:15.000000 generalindex-0.1.3/generalindex/Authenticator.py
--rw-r--r--   0 Izabella   (502) staff       (20)     9175 2022-10-24 07:31:58.000000 generalindex-0.1.3/generalindex/DatalakeHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)     6567 2022-10-24 07:32:01.000000 generalindex-0.1.3/generalindex/HTTPCalller.py
--rw-r--r--   0 Izabella   (502) staff       (20)     1792 2022-10-24 07:32:09.000000 generalindex-0.1.3/generalindex/StatusHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)     8501 2022-10-24 07:32:05.000000 generalindex-0.1.3/generalindex/TaskHandler.py
--rw-r--r--   0 Izabella   (502) staff       (20)    11827 2022-10-24 07:32:12.000000 generalindex-0.1.3/generalindex/Timeseries.py
--rw-r--r--   0 Izabella   (502) staff       (20)      535 2022-10-24 09:24:14.000000 generalindex-0.1.3/generalindex/__init__.py
--rw-r--r--   0 Izabella   (502) staff       (20)      112 2022-10-24 11:32:46.000000 generalindex-0.1.3/generalindex/constants.py
-drwxr-xr-x   0 Izabella   (502) staff       (20)        0 2022-10-24 11:32:47.232234 generalindex-0.1.3/generalindex.egg-info/
--rw-r--r--   0 Izabella   (502) staff       (20)    26675 2022-10-24 11:32:47.000000 generalindex-0.1.3/generalindex.egg-info/PKG-INFO
--rw-r--r--   0 Izabella   (502) staff       (20)      431 2022-10-24 11:32:47.000000 generalindex-0.1.3/generalindex.egg-info/SOURCES.txt
--rw-r--r--   0 Izabella   (502) staff       (20)        1 2022-10-24 11:32:47.000000 generalindex-0.1.3/generalindex.egg-info/dependency_links.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       33 2022-10-24 11:32:47.000000 generalindex-0.1.3/generalindex.egg-info/requires.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       13 2022-10-24 11:32:47.000000 generalindex-0.1.3/generalindex.egg-info/top_level.txt
--rw-r--r--   0 Izabella   (502) staff       (20)       38 2022-10-24 11:32:47.232777 generalindex-0.1.3/setup.cfg
--rw-r--r--   0 Izabella   (502) staff       (20)      829 2022-10-24 07:32:23.000000 generalindex-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:04:56.422273 generalindex-0.1.4/
+-rw-rw-rw-   0        0        0     1055 2022-12-19 09:31:56.000000 generalindex-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    27406 2023-07-24 14:04:56.421274 generalindex-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26234 2022-12-19 09:33:34.000000 generalindex-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 14:04:56.370387 generalindex-0.1.4/generalindex/
+-rw-rw-rw-   0        0        0     1112 2022-12-19 09:46:32.000000 generalindex-0.1.4/generalindex/Authenticator.py
+-rw-rw-rw-   0        0        0     9175 2022-12-19 09:32:24.000000 generalindex-0.1.4/generalindex/DatalakeHandler.py
+-rw-rw-rw-   0        0        0     6615 2023-07-24 10:58:43.000000 generalindex-0.1.4/generalindex/HTTPCalller.py
+-rw-rw-rw-   0        0        0     1792 2022-12-19 09:32:24.000000 generalindex-0.1.4/generalindex/StatusHandler.py
+-rw-rw-rw-   0        0        0     8501 2022-12-19 09:32:24.000000 generalindex-0.1.4/generalindex/TaskHandler.py
+-rw-rw-rw-   0        0        0    20965 2022-12-19 09:32:24.000000 generalindex-0.1.4/generalindex/Timeseries.py
+-rw-rw-rw-   0        0        0      535 2022-12-19 09:46:54.000000 generalindex-0.1.4/generalindex/__init__.py
+-rw-rw-rw-   0        0        0      112 2022-12-19 09:33:34.000000 generalindex-0.1.4/generalindex/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:04:56.419273 generalindex-0.1.4/generalindex.egg-info/
+-rw-rw-rw-   0        0        0    27406 2023-07-24 14:04:56.000000 generalindex-0.1.4/generalindex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-24 14:04:56.000000 generalindex-0.1.4/generalindex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:04:56.000000 generalindex-0.1.4/generalindex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-24 14:04:56.000000 generalindex-0.1.4/generalindex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-24 14:04:56.000000 generalindex-0.1.4/generalindex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:04:56.422273 generalindex-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-07-24 14:04:31.000000 generalindex-0.1.4/setup.py
```

### Comparing `generalindex-0.1.3/LICENSE` & `generalindex-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/PKG-INFO` & `generalindex-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: generalindex
-Version: 0.1.3
-Summary: Python SDK for the General Index platform
-Home-page: https://www.general-index.com/
-Author: General Index
-Author-email: info@general-index.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GENERAL INDEX PYTHON SDK #
 
 This document describes the General Index Python SDK which enables external users to use the GX platform tools within their python scripts. 
 
 The Python SDK can be used within:
 
 - a single python script that is ran thanks to the Python Runner task within a pipeline in the GX application
@@ -724,8 +710,8 @@
     Runner().run()
     status.info('Test Pipeline Finished')
 
  ```
 
 
 ### Who do I talk to? ###
-* Admin: General Index info@general-index.com
+* Admin: General Index info@general-index.com
```

### Comparing `generalindex-0.1.3/README.md` & `generalindex-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,717 +1,731 @@
-# GENERAL INDEX PYTHON SDK #
-
-This document describes the General Index Python SDK which enables external users to use the GX platform tools within their python scripts. 
-
-The Python SDK can be used within:
-
-- a single python script that is ran thanks to the Python Runner task within a pipeline in the GX application
-
-- a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the GX application
-
-- an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the GX application
-
- 
-
-Note that the SDK does not cover everything from API documentation but rather commonly used features.
-
-The scope of the SDK:
-
-- **Datalake Handler** - downloading / uploading / reading files from the data lake  
-
-- **Status Handler** - sending statuses about the task run  
-
-- **Task Handler** - enables communication between tasks within a pipeline and reading/writing parameters 
-
-- **Time Series Handler** - retrieves data directly from the time series database
-
-
-
-## How to install and set the package: 
-### Install
-```text
-pip3 install generalindex==0.1.3
-```
-As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
-```text
-generalindex==0.1.3
-```
-The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
-```text
-pip3 install requests==2.25.1
-```
-
-
-### Environment Variables
-The package uses information from the environment variables. They are automatically provided when running a script within a pipeline (as a Task or within the Python/Jupyter Runners).
-If running locally the script, users must set them in the project to be able to run the project locally.
-
- 
-
-Mandatory environment variables to set:
-
-- LOGIN → login received from GX
-
-- PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
-
-- NG_API_ENDPOINT → the URL to the GX platform API (by default, the url is set to https://api.g-x.co)
- 
-
-This allows to pass the authentication process and directs users' requests to the GX environment API.
-
-Other variables may be useful when creating the tasks within the platform:
-
-- NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
-
-- JOBID → any value; when the pipeline is executed, this value is set by the GX platform
-
-- PIPELINE_ID → any value; when the pipeline is created, this value is set by the GX platform
-
-
-
- --- - 
-## Datalake Handler
-### How to download or read a file from data lake by its name ?
-The DatalakeHandler class can be used as follow within a script to download or upload a file:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# download file from data lake with name and group name
-# it will be saved locally with name local_name.csv
-dh.download_by_name(file_name='my_file.csv', 
-                    group_name='My Group', 
-                    file_type='SOURCE',
-                    dest_file_name='folder/local_name.csv',
-                    save=True,
-                    unzip=False)
-
-# OR read file from data lake with name and group name
-# it returns a BytesIO object (kept in the RAM, not saved in the disk)
-fileIO = dh.download_by_name(file_name='my_file.csv', 
-                            group_name='My Group',
-                            file_type='SOURCE',
-                            dest_file_name=None,
-                            save=False,
-                            unzip=False)
-
-# read the object as pandas DataFrame
-df = pd.read_csv(fileIO)
-
-```
-The download methods allows to either:
-- download and save locally the wanted file, if *save=True*
-- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
-
-Note that by default:
-- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
-- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
-
-
-
-### How to download or read a file from data lake by its ID ?
-In the case that the file ID is known, it can be directly downloaded/read as follow:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# download file from data lake by its ID
-# it will be saved locally with name local_name.csv
-dh.download_by_id(file_id='XXXX-XXXX', 
-                  dest_file_name='folder/local_name.csv',
-                  save=True,
-                  unzip=False)
-
-# read file from data lake by its ID
-# it returns a BytesIO object
-fileIO = dh.download_by_id(file_id='XXXX-XXXX', 
-                            dest_file_name=None,
-                            save=False,
-                            unzip=False)
-
-# read the object as pandas DataFrame
-df = pd.read_csv(fileIO)
-
-```
-The download methods allows to either:
-- download and save locally the wanted file, if *save=True*
-- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
-
-Note that by default:
-- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
-- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
-
-
-
-
-
-### How to upload a file to the data lake?
-The uploading method will upload to the given group the file at the specified path, and returns its ID on the lake:
-```python
-import generalindex as gx
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# upload file to data lake
-file_id = dh.upload_file(file='path/local_name.csv', 
-                        group_name='My Group', 
-                        file_upload_name='name_in_the_datalake.csv')
-```
-It is possible as well to stream a python object's content directly to the datalake from memory, without having to save the file on the disk.
-
-The prerequisite is to pass to the uploading method a BytesIO object (not other objects such as pandas Dataframe).
-
-```python
-import generalindex as gx
-import io
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# Turn the pandas DataFrame (df) to BytesIO for streaming
-fileIO = io.BytesIO(df.to_csv().encode()) 
-
-# upload file to data lake
-file_id = dh.upload_file(file=fileIO, 
-                        group_name='My Group', 
-                        file_upload_name='name_in_the_datalake.csv')
-```
---- -
-## Timeseries Queries
-### How to get the list of existing symbols for a given group ?
-Data saved in the time series database is structured by group, keys and timestamp.
-Each set of keys has unique dates entries in the database, with corresponding columns values.
-
-To explore what are the available symbols for a given group, the following method can be used:
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-group = 'My Group'
-group_symbols = ts.get_symbols(group_name=group)
-```
-The default size of the returned list is 1 000 items.
-
-Note that the return object from the get_symbols() method is a JSON (python dict) where the keys and columns are accessible in the *items* key of the JSON.
-
-### How to query by metadata or descriptions?
-
-In order to find the symbols querying by the metadata, column or symbol names, search_for parameter may be used.
-It will look for passed string in the whole time series database and return the JSON with keys and columns where searched string appears.
-
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-search = 'Data description'
-searched_symbols = ts.get_symbols(search_for=search)
-```
-
-Passing both group_name and search_for parameters of the get_symbols() method allows to narrow down the results from selected group.
-The user must provide either group_name or search_for to the method in order to obtain the symbols.
-
-
-If trying to get the list of symbols from a group that contains more than 1 000 items, the results will be paginated (by default into chunks of 1 000 items).
-To navigate in the large results the *get_symbols()* method takes as extra arguments the size of the returned list and the from page:
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-group = 'My Group'
-
-# Get the results into chunks of 200 items for page 5
-# meaning the results from the 1000th till the 1200th 
-group_symbols = ts.get_symbols(group_name=group, _size=200, _from=5)
-```
-By default, these parameters are _size=2000 (the maximum limit for the items lengths) and _from=0.
-
-
-### How to read data from Timeseries database?
-It is possible to use the SDK to directly query the TimeSeries database for data, given the symbol's keys, columns and the datalake group it is stored on.
-
-On the application, it is similar of creating a Dataprep instance, that selects a set of symbols from groups into a basket. 
-
-The retrieved data can be:
-- streamed directly to memory, retrieved as a BytesIO object, by setting *file_name* as None (default value), 
-- saved as a csv file locally with the provided path and name as *file_name*.
-
-The symbols are the keys the data was saved with in the database. For a given symbol, all the keys must be passed, as a dictionary object with the key name and value.
-It is possible to use a wildcard for the symbols values, to have all the values for that key, using *.
-
-The wanted columns are then passed as a list that can contain one or more items.
-If an empty list [ ] is passed to the function, it returns all the available columns.
-
-To read all available data for specific symbols and columns with no time frame, no start or end date are passed to the method.
-
-Extra settings are as well available to query data:
-- Metadata: to either return it in the query of not
-- Format: either get a Normalized CSV (NCSV) or a dataframe format
-- Timezone: get the timestamps in the timezone of the user's account or get the data in a specific timezone
-- Corrections: how to handle corrections to the TimeSeries database (corrections set to 'yes', 'no', 'history' or 'only')
-- Delta: whether to show by datatimestamp file (delta=False) or insert time (delta=True)
-
-
-The following code shows an example of how to query the TimseSeries database: :
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group acccording to keys & columns 
-# and save as query.csv in test/
-ts.retrieve_data_as_csv(file_name='test/query.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group'
-                        )
-
-# The retrieved data can be read as a pandas dataframe
-df = pd.read_csv("test/query.csv")
-
-
-# retrieve all available data from group acccording to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to read data from Timeseries for specific dates?
-To retrieve data the data within specific time frame, user can specify the start and end date.
-
-There are two options how the start and end date may look like:
-
-- only date (e.g., 2021-01-04)
-
-- date and time (e.g., 2021-02-01T12:00:00; ISO format must be followed)
-
-For example, if user specified start_date=2021-02-01 and end_date=2021-02-06, then data will be retrieved like this: from 2021-02-01 00:00:00 till 2021-02-06 23:59:59.
-
-If date and time is specified then data will be retrieved exactly for the specified time frame.
-
-Note that ISO format must be followed: YYYY-MM-DD**T**HH:mm:ss. Pay attention to the "T" letter between date and time.
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = 'Open'
-
-# retrieve data between start_date and end_date
-# data will be retrieved between 2021-01-04 00:00:00 and 2021-02-05 23:59:59
-# saved as a csv file named test.csv
-ts.retrieve_data_as_csv(file_name='test/test.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group',
-                        start_date='2021-01-04',
-                        end_date='2021-02-05'
-                        )
-
-# retrieve data for specific time frame
-# from 2021-01-04 12:30:00
-# to 2021-02-05 09:15:00
-ts.retrieve_data_as_csv(file_name='test/test.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group',
-                        start_date='2021-01-04T12:30:00',
-                        end_date='2021-02-05T09:15:00'
-                        )
-
-
-# For given keys, columns, group and dates range
-# Streaming instead of saving
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 start_date='2021-01-04',
-                                 end_date='2021-02-05'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to use a wildcard for a key's values ?
-To get all the value for one a several keys for the query, the character * can be used as a wildcard.
-The argument *allow_wildcard* should be set to True in the retrieval function to enable the use of wildcard. 
-
-Please note that by default, the use of wildcards is **DISABLED**.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "*"}
-columns = ['Open', 'Close']
-
-# retrieve all history for the symbols with keys and columns
-# all values for Key3 will be returned
-# the data will be streamed to memory
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 allow_wildcard=True
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-
-### How to get all the columns for a given set of keys ?
-To get all the columns values for a given set of keys in the database, the query can take an empty list as the queried columns, as follow:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "Val3"}
-columns = []
-
-# retrieve all history for the symbols with keys and columns
-# all columns for the set of keys will be returned
-# the data will be streamed to memory
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-Note that this configuration can be used with keys wildcards (with *allow_wildacrd=True*) and any other setting.
-
-
-### How to modify the Time Zone of the data ?
-The timestamps in the queried time series are set by default in the timezone of the user's account, who created the script or the pipeline.
-It is described in the Date column header between brackets (for example *Date(UTC)*)
-
-To modify the time zone in the retrieved dataset, the timezone can be passed directly to the retrieval function as follow.
-It must respect the Continent/City format.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 timezone='Europe/London'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to get the metadata along with the data ? 
-It is possible to get extra columns in the retrieved data, along with the keys & columns values, containing the metadata of the symbols.
-It is done by setting the argument *metadata=True* in the retrieval function.
-
-By default, no metadata is included in the queried data.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 metadata=True
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-
-### How to modify the format of the received data ?
-The queried data comes by default as Normalized CSV format (NCSV), with in this order:
-* the keys columns,
-* the date column, with timestamps in either the default timezone or the specified one (*timezone* argument in the function),
-* the values columns,
-* the metadata columns, if wanted (*metadata=True*)
- 
-By setting *NCSV=False* in the retrieval method, the data will be returned as Dataframe format (PANDAS in API docs), as a JSON.
-The JSON (python dict) has timestamps as keys and a dictionary containing pairs of symbols_columns and their value.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-file_json = ts.retrieve_data_as_csv(file_name=None,
-                                    symbols=symbols,
-                                    columns=columns,
-                                    group_name='My Group',
-                                    metadata=True,
-                                    NCSV=False
-                                    )
-
-# read as pandas dataframe
-# Transpose to have datetime as rows index
-df = pd.DataFrame(file_json).T
-```
-
-Note that the dataframe, created from the JSON containing the data, is then transposed to have timestamps as DatetimeIndex (along rows axis). 
-
-
---- - 
-## Task Handler
-Users can extend the existing set of tasks on GX platform by executing scripts or notebooks respectively from the Python Runner Task or the Jupyter Runner Task. 
-
-This task then can be used in a pipeline and be able to communicate with other tasks by:
-
-- reading outputs from other tasks, as inputs
-- writing outputs, that can be used by others tasks as inputs
-
-A task can as well receive inputs directly as a file picked from the datalake, either for a specific file either for the newest available version of a file on the lake, given its name and group.
-
-Whithin a python script, run into either one of the **Python Runner Task**,  this is implemented as follow:
-
-### Read a Task Input
-The input file passed to the Task can be: 
-- either downloaded to the disk,
-- either to be read on the fly (useful when limited space on the disk but not in memory).
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-
-# the current task reads the file passed by a previous task, that is connected to it.
-# The passed file is downloaded and saved on the disk as data.csv
-th.download_from_input_parameter(arg_name='Input #1', 
-                                 dest_file_name='data.csv',
-                                 save=True)
-
-# The passed file is downloaded and kept in the memory (streamed, not saved on the disk)
-file_content = th.download_from_input_parameter(arg_name='Input #2', 
-                                                dest_file_name=None,
-                                                save=False)
-
-# If a csv file was streamed, it can be read as pandas Dataframe for example
-df = pd.read_csv(file_content)
-```
-
-If dest_file_name=None then the file is saved on the disk with its original name from the datalake.
-
-### How to obtain additional file information
-
-There is a possibility to retrieve information related to the input parameters using the DatalakeHandler (```dh.get_info_from_id()```) and TaskHandler (``` th.read_task_parameter_value()```) together.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-dh.get_info_from_id(th.read_task_parameter_value('Input #1'))
-
-``` 
-This can be used to retrieve any metadata associated with the file itself like file name or arrival time (time it was uploaded to the system)
-
-### Set a Task Output
-The output of the Task can be set :
-- either by uploading a file saved on the disk to the datalake,
-- either by streaming the python object content to the datalake as the destination file.
-
-Once uploaded, the Output is set to point to the file on the datalake (by its ID, name ,group name)
-
-
- ```python
-import generalindex as gx
-import io
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-
-# the first task uploads the file dataset.csv to My Final Group and pass the info about this file
-# so that the next task can read this file by connecting its input to the output Prepared Dataset
-th.upload_to_output_parameter(output_name='Output #1', 
-                              file='path/dataset.csv', 
-                              group_name='My Final Group',
-                              file_upload_name=None,
-                              file_type='SOURCE')
-
-# Convert the python object to upload as BytesIO object
-df_io = io.BytesIO(df.to_csv().encode())
-
-# Stream to the datalake as the destination file
-th.upload_to_output_parameter(output_name='Output #1', 
-                              file=df_io, 
-                              group_name='My Final Group',
-                              file_upload_name='dataset.csv',
-                              file_type='SOURCE')
-```
-
-If file_upload_name=None then the saved file will be uploaded with its original name.
-If the file is streamed directly to the datalake, the file_upload_name argument must be set.
-
---- -
-## Statuses
-Sending status can be used to show in the application what is the progress of the task execution. It allows to use 3 different levels: 
-- FINISHED (green),
-- WARNING (orange), 
-- ERROR (red).
-
-Sending statuses remains optional as the GX platform sends general statuses.
-Only if user needs to pass some specific information in the status, this is worth using.
-
-```python
-import generalindex as gx
-
-# Instantiate the Status Handler
-sh = gx.StatusHandler()
-
-# Generic status sender
-sh.send_status(status='INFO', message='Crucial Information')
-
-# there are pre-defined statuses
-sh.info(message='Pipeline Finished Successfully')
-sh.warn(message='Something suspicious is happening ...')
-sh.error(message='Oops, the task failed ...')
-```
-
-Note that the info status is informing the status service that the task executed successfully and is finished.
-
---- -
-## Example
-To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
-
-Below is an example of a class that has 3 methods:
-
-- Download raw data (or take from the previous task)
-- Process the data  
-- Upload the data to datalake and pass it to the next task
-
- ```python
-import io
-import generalindex as gx
-import pandas as pd
-
-class Runner:
-    def __init__(self):
-        # Inherit the methods from the SDK Task Handler class
-        self.handler = gx.TaskHandler()
-        self.df = None
-        
-    def download_data(self):
-        # the method from TaskHandler can be used directly
-        # it downloads the file passed as input Dataset and save it as data.csv
-        self.handler.download_from_input_parameter(arg_name='Dataset', dest_file_name='data.csv', save=True)
-        
-        # Read as pandas dataframe
-        return pd.read_csv("data.csv")
-        
-    
-    def process_data(self, df):
-        # any logic here that processed the downloaded dataset and saves it as processed_data.csv
-        
-        return df_processed
-
-    
-    def upload_data(self, df_processed):
-        # Encode as bytesIO
-        fileIO = io.BytesIO(df_processed.to_csv().encode())
-        
-        # pass the processed data csv file as the output of the task called Processed Data
-        self.handler.upload_to_output_parameter(output_name='Processed Dataset', file=fileIO, group_name='Final Group')
-    
-        
-    def run(self):
-        df = self.download_data()
-        df_processed = self.process_data(df)
-        self.upload_data(df_processed)
-        
-        
-if __name__ == '__main__':
-    status = gx.StatusHandler()
-    Runner().run()
-    status.info('Test Pipeline Finished')
-
- ```
-
-
-### Who do I talk to? ###
-* Admin: General Index info@general-index.com
+Metadata-Version: 2.1
+Name: generalindex
+Version: 0.1.4
+Summary: Python SDK for the General Index platform
+Home-page: https://www.general-index.com/
+Author: General Index
+Author-email: info@general-index.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GENERAL INDEX PYTHON SDK #
+
+This document describes the General Index Python SDK which enables external users to use the GX platform tools within their python scripts. 
+
+The Python SDK can be used within:
+
+- a single python script that is ran thanks to the Python Runner task within a pipeline in the GX application
+
+- a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the GX application
+
+- an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the GX application
+
+ 
+
+Note that the SDK does not cover everything from API documentation but rather commonly used features.
+
+The scope of the SDK:
+
+- **Datalake Handler** - downloading / uploading / reading files from the data lake  
+
+- **Status Handler** - sending statuses about the task run  
+
+- **Task Handler** - enables communication between tasks within a pipeline and reading/writing parameters 
+
+- **Time Series Handler** - retrieves data directly from the time series database
+
+
+
+## How to install and set the package: 
+### Install
+```text
+pip3 install generalindex==0.1.3
+```
+As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
+```text
+generalindex==0.1.3
+```
+The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
+```text
+pip3 install requests==2.25.1
+```
+
+
+### Environment Variables
+The package uses information from the environment variables. They are automatically provided when running a script within a pipeline (as a Task or within the Python/Jupyter Runners).
+If running locally the script, users must set them in the project to be able to run the project locally.
+
+ 
+
+Mandatory environment variables to set:
+
+- LOGIN → login received from GX
+
+- PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
+
+- NG_API_ENDPOINT → the URL to the GX platform API (by default, the url is set to https://api.g-x.co)
+ 
+
+This allows to pass the authentication process and directs users' requests to the GX environment API.
+
+Other variables may be useful when creating the tasks within the platform:
+
+- NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
+
+- JOBID → any value; when the pipeline is executed, this value is set by the GX platform
+
+- PIPELINE_ID → any value; when the pipeline is created, this value is set by the GX platform
+
+
+
+ --- - 
+## Datalake Handler
+### How to download or read a file from data lake by its name ?
+The DatalakeHandler class can be used as follow within a script to download or upload a file:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# download file from data lake with name and group name
+# it will be saved locally with name local_name.csv
+dh.download_by_name(file_name='my_file.csv', 
+                    group_name='My Group', 
+                    file_type='SOURCE',
+                    dest_file_name='folder/local_name.csv',
+                    save=True,
+                    unzip=False)
+
+# OR read file from data lake with name and group name
+# it returns a BytesIO object (kept in the RAM, not saved in the disk)
+fileIO = dh.download_by_name(file_name='my_file.csv', 
+                            group_name='My Group',
+                            file_type='SOURCE',
+                            dest_file_name=None,
+                            save=False,
+                            unzip=False)
+
+# read the object as pandas DataFrame
+df = pd.read_csv(fileIO)
+
+```
+The download methods allows to either:
+- download and save locally the wanted file, if *save=True*
+- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
+
+Note that by default:
+- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
+- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
+
+
+
+### How to download or read a file from data lake by its ID ?
+In the case that the file ID is known, it can be directly downloaded/read as follow:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# download file from data lake by its ID
+# it will be saved locally with name local_name.csv
+dh.download_by_id(file_id='XXXX-XXXX', 
+                  dest_file_name='folder/local_name.csv',
+                  save=True,
+                  unzip=False)
+
+# read file from data lake by its ID
+# it returns a BytesIO object
+fileIO = dh.download_by_id(file_id='XXXX-XXXX', 
+                            dest_file_name=None,
+                            save=False,
+                            unzip=False)
+
+# read the object as pandas DataFrame
+df = pd.read_csv(fileIO)
+
+```
+The download methods allows to either:
+- download and save locally the wanted file, if *save=True*
+- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
+
+Note that by default:
+- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
+- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
+
+
+
+
+
+### How to upload a file to the data lake?
+The uploading method will upload to the given group the file at the specified path, and returns its ID on the lake:
+```python
+import generalindex as gx
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# upload file to data lake
+file_id = dh.upload_file(file='path/local_name.csv', 
+                        group_name='My Group', 
+                        file_upload_name='name_in_the_datalake.csv')
+```
+It is possible as well to stream a python object's content directly to the datalake from memory, without having to save the file on the disk.
+
+The prerequisite is to pass to the uploading method a BytesIO object (not other objects such as pandas Dataframe).
+
+```python
+import generalindex as gx
+import io
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# Turn the pandas DataFrame (df) to BytesIO for streaming
+fileIO = io.BytesIO(df.to_csv().encode()) 
+
+# upload file to data lake
+file_id = dh.upload_file(file=fileIO, 
+                        group_name='My Group', 
+                        file_upload_name='name_in_the_datalake.csv')
+```
+--- -
+## Timeseries Queries
+### How to get the list of existing symbols for a given group ?
+Data saved in the time series database is structured by group, keys and timestamp.
+Each set of keys has unique dates entries in the database, with corresponding columns values.
+
+To explore what are the available symbols for a given group, the following method can be used:
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+group = 'My Group'
+group_symbols = ts.get_symbols(group_name=group)
+```
+The default size of the returned list is 1 000 items.
+
+Note that the return object from the get_symbols() method is a JSON (python dict) where the keys and columns are accessible in the *items* key of the JSON.
+
+### How to query by metadata or descriptions?
+
+In order to find the symbols querying by the metadata, column or symbol names, search_for parameter may be used.
+It will look for passed string in the whole time series database and return the JSON with keys and columns where searched string appears.
+
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+search = 'Data description'
+searched_symbols = ts.get_symbols(search_for=search)
+```
+
+Passing both group_name and search_for parameters of the get_symbols() method allows to narrow down the results from selected group.
+The user must provide either group_name or search_for to the method in order to obtain the symbols.
+
+
+If trying to get the list of symbols from a group that contains more than 1 000 items, the results will be paginated (by default into chunks of 1 000 items).
+To navigate in the large results the *get_symbols()* method takes as extra arguments the size of the returned list and the from page:
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+group = 'My Group'
+
+# Get the results into chunks of 200 items for page 5
+# meaning the results from the 1000th till the 1200th 
+group_symbols = ts.get_symbols(group_name=group, _size=200, _from=5)
+```
+By default, these parameters are _size=2000 (the maximum limit for the items lengths) and _from=0.
+
+
+### How to read data from Timeseries database?
+It is possible to use the SDK to directly query the TimeSeries database for data, given the symbol's keys, columns and the datalake group it is stored on.
+
+On the application, it is similar of creating a Dataprep instance, that selects a set of symbols from groups into a basket. 
+
+The retrieved data can be:
+- streamed directly to memory, retrieved as a BytesIO object, by setting *file_name* as None (default value), 
+- saved as a csv file locally with the provided path and name as *file_name*.
+
+The symbols are the keys the data was saved with in the database. For a given symbol, all the keys must be passed, as a dictionary object with the key name and value.
+It is possible to use a wildcard for the symbols values, to have all the values for that key, using *.
+
+The wanted columns are then passed as a list that can contain one or more items.
+If an empty list [ ] is passed to the function, it returns all the available columns.
+
+To read all available data for specific symbols and columns with no time frame, no start or end date are passed to the method.
+
+Extra settings are as well available to query data:
+- Metadata: to either return it in the query of not
+- Format: either get a Normalized CSV (NCSV) or a dataframe format
+- Timezone: get the timestamps in the timezone of the user's account or get the data in a specific timezone
+- Corrections: how to handle corrections to the TimeSeries database (corrections set to 'yes', 'no', 'history' or 'only')
+- Delta: whether to show by datatimestamp file (delta=False) or insert time (delta=True)
+
+
+The following code shows an example of how to query the TimseSeries database: :
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group acccording to keys & columns 
+# and save as query.csv in test/
+ts.retrieve_data_as_csv(file_name='test/query.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group'
+                        )
+
+# The retrieved data can be read as a pandas dataframe
+df = pd.read_csv("test/query.csv")
+
+
+# retrieve all available data from group acccording to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to read data from Timeseries for specific dates?
+To retrieve data the data within specific time frame, user can specify the start and end date.
+
+There are two options how the start and end date may look like:
+
+- only date (e.g., 2021-01-04)
+
+- date and time (e.g., 2021-02-01T12:00:00; ISO format must be followed)
+
+For example, if user specified start_date=2021-02-01 and end_date=2021-02-06, then data will be retrieved like this: from 2021-02-01 00:00:00 till 2021-02-06 23:59:59.
+
+If date and time is specified then data will be retrieved exactly for the specified time frame.
+
+Note that ISO format must be followed: YYYY-MM-DD**T**HH:mm:ss. Pay attention to the "T" letter between date and time.
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = 'Open'
+
+# retrieve data between start_date and end_date
+# data will be retrieved between 2021-01-04 00:00:00 and 2021-02-05 23:59:59
+# saved as a csv file named test.csv
+ts.retrieve_data_as_csv(file_name='test/test.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group',
+                        start_date='2021-01-04',
+                        end_date='2021-02-05'
+                        )
+
+# retrieve data for specific time frame
+# from 2021-01-04 12:30:00
+# to 2021-02-05 09:15:00
+ts.retrieve_data_as_csv(file_name='test/test.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group',
+                        start_date='2021-01-04T12:30:00',
+                        end_date='2021-02-05T09:15:00'
+                        )
+
+
+# For given keys, columns, group and dates range
+# Streaming instead of saving
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 start_date='2021-01-04',
+                                 end_date='2021-02-05'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to use a wildcard for a key's values ?
+To get all the value for one a several keys for the query, the character * can be used as a wildcard.
+The argument *allow_wildcard* should be set to True in the retrieval function to enable the use of wildcard. 
+
+Please note that by default, the use of wildcards is **DISABLED**.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "*"}
+columns = ['Open', 'Close']
+
+# retrieve all history for the symbols with keys and columns
+# all values for Key3 will be returned
+# the data will be streamed to memory
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 allow_wildcard=True
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+
+### How to get all the columns for a given set of keys ?
+To get all the columns values for a given set of keys in the database, the query can take an empty list as the queried columns, as follow:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "Val3"}
+columns = []
+
+# retrieve all history for the symbols with keys and columns
+# all columns for the set of keys will be returned
+# the data will be streamed to memory
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+Note that this configuration can be used with keys wildcards (with *allow_wildacrd=True*) and any other setting.
+
+
+### How to modify the Time Zone of the data ?
+The timestamps in the queried time series are set by default in the timezone of the user's account, who created the script or the pipeline.
+It is described in the Date column header between brackets (for example *Date(UTC)*)
+
+To modify the time zone in the retrieved dataset, the timezone can be passed directly to the retrieval function as follow.
+It must respect the Continent/City format.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 timezone='Europe/London'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to get the metadata along with the data ? 
+It is possible to get extra columns in the retrieved data, along with the keys & columns values, containing the metadata of the symbols.
+It is done by setting the argument *metadata=True* in the retrieval function.
+
+By default, no metadata is included in the queried data.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 metadata=True
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+
+### How to modify the format of the received data ?
+The queried data comes by default as Normalized CSV format (NCSV), with in this order:
+* the keys columns,
+* the date column, with timestamps in either the default timezone or the specified one (*timezone* argument in the function),
+* the values columns,
+* the metadata columns, if wanted (*metadata=True*)
+ 
+By setting *NCSV=False* in the retrieval method, the data will be returned as Dataframe format (PANDAS in API docs), as a JSON.
+The JSON (python dict) has timestamps as keys and a dictionary containing pairs of symbols_columns and their value.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+file_json = ts.retrieve_data_as_csv(file_name=None,
+                                    symbols=symbols,
+                                    columns=columns,
+                                    group_name='My Group',
+                                    metadata=True,
+                                    NCSV=False
+                                    )
+
+# read as pandas dataframe
+# Transpose to have datetime as rows index
+df = pd.DataFrame(file_json).T
+```
+
+Note that the dataframe, created from the JSON containing the data, is then transposed to have timestamps as DatetimeIndex (along rows axis). 
+
+
+--- - 
+## Task Handler
+Users can extend the existing set of tasks on GX platform by executing scripts or notebooks respectively from the Python Runner Task or the Jupyter Runner Task. 
+
+This task then can be used in a pipeline and be able to communicate with other tasks by:
+
+- reading outputs from other tasks, as inputs
+- writing outputs, that can be used by others tasks as inputs
+
+A task can as well receive inputs directly as a file picked from the datalake, either for a specific file either for the newest available version of a file on the lake, given its name and group.
+
+Whithin a python script, run into either one of the **Python Runner Task**,  this is implemented as follow:
+
+### Read a Task Input
+The input file passed to the Task can be: 
+- either downloaded to the disk,
+- either to be read on the fly (useful when limited space on the disk but not in memory).
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+
+# the current task reads the file passed by a previous task, that is connected to it.
+# The passed file is downloaded and saved on the disk as data.csv
+th.download_from_input_parameter(arg_name='Input #1', 
+                                 dest_file_name='data.csv',
+                                 save=True)
+
+# The passed file is downloaded and kept in the memory (streamed, not saved on the disk)
+file_content = th.download_from_input_parameter(arg_name='Input #2', 
+                                                dest_file_name=None,
+                                                save=False)
+
+# If a csv file was streamed, it can be read as pandas Dataframe for example
+df = pd.read_csv(file_content)
+```
+
+If dest_file_name=None then the file is saved on the disk with its original name from the datalake.
+
+### How to obtain additional file information
+
+There is a possibility to retrieve information related to the input parameters using the DatalakeHandler (```dh.get_info_from_id()```) and TaskHandler (``` th.read_task_parameter_value()```) together.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+dh.get_info_from_id(th.read_task_parameter_value('Input #1'))
+
+``` 
+This can be used to retrieve any metadata associated with the file itself like file name or arrival time (time it was uploaded to the system)
+
+### Set a Task Output
+The output of the Task can be set :
+- either by uploading a file saved on the disk to the datalake,
+- either by streaming the python object content to the datalake as the destination file.
+
+Once uploaded, the Output is set to point to the file on the datalake (by its ID, name ,group name)
+
+
+ ```python
+import generalindex as gx
+import io
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+
+# the first task uploads the file dataset.csv to My Final Group and pass the info about this file
+# so that the next task can read this file by connecting its input to the output Prepared Dataset
+th.upload_to_output_parameter(output_name='Output #1', 
+                              file='path/dataset.csv', 
+                              group_name='My Final Group',
+                              file_upload_name=None,
+                              file_type='SOURCE')
+
+# Convert the python object to upload as BytesIO object
+df_io = io.BytesIO(df.to_csv().encode())
+
+# Stream to the datalake as the destination file
+th.upload_to_output_parameter(output_name='Output #1', 
+                              file=df_io, 
+                              group_name='My Final Group',
+                              file_upload_name='dataset.csv',
+                              file_type='SOURCE')
+```
+
+If file_upload_name=None then the saved file will be uploaded with its original name.
+If the file is streamed directly to the datalake, the file_upload_name argument must be set.
+
+--- -
+## Statuses
+Sending status can be used to show in the application what is the progress of the task execution. It allows to use 3 different levels: 
+- FINISHED (green),
+- WARNING (orange), 
+- ERROR (red).
+
+Sending statuses remains optional as the GX platform sends general statuses.
+Only if user needs to pass some specific information in the status, this is worth using.
+
+```python
+import generalindex as gx
+
+# Instantiate the Status Handler
+sh = gx.StatusHandler()
+
+# Generic status sender
+sh.send_status(status='INFO', message='Crucial Information')
+
+# there are pre-defined statuses
+sh.info(message='Pipeline Finished Successfully')
+sh.warn(message='Something suspicious is happening ...')
+sh.error(message='Oops, the task failed ...')
+```
+
+Note that the info status is informing the status service that the task executed successfully and is finished.
+
+--- -
+## Example
+To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
+
+Below is an example of a class that has 3 methods:
+
+- Download raw data (or take from the previous task)
+- Process the data  
+- Upload the data to datalake and pass it to the next task
+
+ ```python
+import io
+import generalindex as gx
+import pandas as pd
+
+class Runner:
+    def __init__(self):
+        # Inherit the methods from the SDK Task Handler class
+        self.handler = gx.TaskHandler()
+        self.df = None
+        
+    def download_data(self):
+        # the method from TaskHandler can be used directly
+        # it downloads the file passed as input Dataset and save it as data.csv
+        self.handler.download_from_input_parameter(arg_name='Dataset', dest_file_name='data.csv', save=True)
+        
+        # Read as pandas dataframe
+        return pd.read_csv("data.csv")
+        
+    
+    def process_data(self, df):
+        # any logic here that processed the downloaded dataset and saves it as processed_data.csv
+        
+        return df_processed
+
+    
+    def upload_data(self, df_processed):
+        # Encode as bytesIO
+        fileIO = io.BytesIO(df_processed.to_csv().encode())
+        
+        # pass the processed data csv file as the output of the task called Processed Data
+        self.handler.upload_to_output_parameter(output_name='Processed Dataset', file=fileIO, group_name='Final Group')
+    
+        
+    def run(self):
+        df = self.download_data()
+        df_processed = self.process_data(df)
+        self.upload_data(df_processed)
+        
+        
+if __name__ == '__main__':
+    status = gx.StatusHandler()
+    Runner().run()
+    status.info('Test Pipeline Finished')
+
+ ```
+
+
+### Who do I talk to? ###
+* Admin: General Index info@general-index.com
```

### Comparing `generalindex-0.1.3/generalindex/Authenticator.py` & `generalindex-0.1.4/generalindex/Authenticator.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/generalindex/DatalakeHandler.py` & `generalindex-0.1.4/generalindex/DatalakeHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/generalindex/HTTPCalller.py` & `generalindex-0.1.4/generalindex/HTTPCalller.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.user_agent = USER_AGENT
 
     def set_headers(self, headers=None):
         if headers is None:
             headers = {}
         # adding token to the headers
         headers.update(self.token)
+        headers.update({'X-KH-E-ID': self.eid})
         headers.update({'X-KH-JOB-ID': self.jobid})
         headers.update({'User-Agent': self.user_agent})
         return headers
 
     def post(self, path, payload=None, data=None, headers=None):
         headers = self.set_headers(headers)
```

### Comparing `generalindex-0.1.3/generalindex/StatusHandler.py` & `generalindex-0.1.4/generalindex/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/generalindex/TaskHandler.py` & `generalindex-0.1.4/generalindex/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/generalindex/Timeseries.py` & `generalindex-0.1.4/generalindex/Timeseries.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import json
 
 from datetime import datetime
 from . import LOGGER_NAME
 from .HTTPCalller import HTTPCaller
 from .DatalakeHandler import *
+from io import StringIO
 
 log = logging.getLogger(LOGGER_NAME)
 
 
 class Timeseries:
     def __init__(self):
         self.caller = HTTPCaller()
@@ -46,20 +47,21 @@
         r = self.caller.get(path=query_url)
 
         return json.load(io.BytesIO(r.content))
 
     def retrieve_data_as_csv(self, symbols: dict, columns, group_name: str,
                              file_name: str = None, start_date: str = None, end_date: str = None,
                              timezone: str = None,
-                             metadata: bool = False, allow_wildcard: bool = False, NCSV: bool = True,
+                             metadata: bool = False, allow_wildcard: bool = False, output_format: str = 'NCSV',
                              corrections : str = 'false', delta: bool = False):
 
         '''
-        The method retrieves the data from NG Timeseries based on symbols and columns.
+        The method retrieves the data from NG Timeseries based on symbols and columns with streaming function.
         Optionally start and end dates can be specified. If no dates specified, all the available data are taken.
+        * IMPORTANT! Currently in streaming mode NCSV output is available.
 
         :param file_name: the name of file locally to save data to, with the proper extension passed (for example data.csv)
         :param symbols: symbols to identify data in Timeseries. Must dictionary {"symbolName": "symbolValue", ...}
         :param columns: name of column or list of columns to retrieve
         :param group_name: name of the group
         :param start_date: start date of data in the format YYYY-MM-DD. If time is included, it must follow ISO format:
         YYYY-MM-DDTHH:mm:ss (note the 'T' letter separating the date and time part)
@@ -70,14 +72,15 @@
                         if None, it returns the date with the default timezone of the user, set in the application
         :param: corrections: How to handle corrections in time series. Must be either "true", "false" or "only"
         :param: delta: delta will filter timeseries by insertion date instead of the actual timestamp of data
         :param: metadata: boolean to return or not the metadata in the file, default as False
         :param: allow_wildcard: boolean to allow or not the use of wildcards '*' in the keys or columns
         :param: corrections: How to handle corrections in time series. Must be either "true", "false", "history" or "only"
         :param: delta: delta will filter timeseries by insertion date instead of the actual timestamp of data
+        :param; output_format: The method from which "view" the data should be retrieved. Default "NCSV".
 
         :return: saves file with data
         '''
 
         # start_date is optional: if not provided, the data are taken from the very beginning
         if start_date is not None:
             # date only
@@ -123,15 +126,15 @@
                     "groupName": group_name,
                     "columns": columns,
                     "pattern": allow_wildcard
                      }
                 ],
                 "corrections": corrections,
                 "delta": delta,
-                "formatType": "NCSV" if NCSV else 'PANDAS'
+                "formatType": output_format
                 }
 
         # add extra fields in the payload if needed
         if timezone is not None:
             # Check the format for the timezone
             assert '/' in timezone, 'Wrongly formatted timezone argument. Must be for example Europe/London'
  
@@ -148,65 +151,252 @@
 
         # Summary
         log.debug(f'Retrieving data for symbols: {symbols} '
                   f'\nand columns: {columns}'
                   f'\nfrom date: {start_date}'
                   f'\nto date: {end_date}')
 
+        
+        # Request
+        r = self.caller.post(path='/ts/stream', payload=body)
+
+        log.debug(f'Response: {r.text}')
+
+        try:
+
+            # Get file as NCSV API format
+            if output_format == 'NCSV':
+                # return raw bytes directly
+                fileIO = StringIO(str(r.content, encoding='utf-8'))
+
+                if file_name is None:
+                    # return the raw Bytes (streamed)
+                    return fileIO
+
+                else:
+                    # Check that the extension is in the file, else add it as csv by default
+                    file_name = file_name if '.' in file_name else file_name + '.csv'
+
+                    # Save the downloaded data on the disk
+                    with open(file_name, "w") as text_file:
+                        text_file.write(r.text)
+        
+            else:
+                raise ValueError('{} format of the timeseries output is not supported. Please use NCSV, PANDAS or STANDARD'.format(output_format))
+
+        except :
+            # Get unique list of symbols
+            raw_list = self.get_symbols(group_name)['items']
+            symb_list = set([item for sublist in [list(d['symbols'].keys()) for d in raw_list] for item in sublist])
+
+            # Raise error with symbols list
+            raise ValueError('Wrong Symbols or Columns passed to the query . It should match the data structure on the group: {}'.format(symb_list))
+
+        log.debug('Data are saved to file: {}'.format(file_name))
+
+        return
+    
+    def retrieve_data_as_json(self, symbols: dict, columns, group_name: str,
+                             file_name: str = None, start_date: str = None, end_date: str = None,
+                             timezone: str = None,
+                             metadata: bool = False, allow_wildcard: bool = False, output_format: str = 'NCSV',
+                             corrections : str = 'false', delta: bool = False):
+
+        '''
+        The method retrieves the data from NG Timeseries based on symbols and columns with streaming function.
+        Optionally start and end dates can be specified. If no dates specified, all the available data are taken.
+        * IMPORTANT! Currently NCSV output_format returns the same as for streaming functions. STANDARD, PANDAS, UI return json.
+
+        :param file_name: the name of file locally to save data to, with the proper extension passed (for example data.csv)
+        :param symbols: symbols to identify data in Timeseries. Must dictionary {"symbolName": "symbolValue", ...}
+        :param columns: name of column or list of columns to retrieve
+        :param group_name: name of the group
+        :param start_date: start date of data in the format YYYY-MM-DD. If time is included, it must follow ISO format:
+        YYYY-MM-DDTHH:mm:ss (note the 'T' letter separating the date and time part)
+        :param end_date: end date of the data in the format YYYY-MM-DD. If time is included, it must follow ISO format:
+        YYYY-MM-DDTHH:mm:ss (note the 'T' letter separating the date and time part)
+
+        :param: timezone: timezone as string used for the timestamps in the Date column. Continent/City, for example Europe/London
+                        if None, it returns the date with the default timezone of the user, set in the application
+        :param: corrections: How to handle corrections in time series. Must be either "true", "false" or "only"
+        :param: delta: delta will filter timeseries by insertion date instead of the actual timestamp of data
+        :param: metadata: boolean to return or not the metadata in the file, default as False
+        :param: allow_wildcard: boolean to allow or not the use of wildcards '*' in the keys or columns
+        :param: corrections: How to handle corrections in time series. Must be either "true", "false", "history" or "only"
+        :param: delta: delta will filter timeseries by insertion date instead of the actual timestamp of data
+        :param; output_format: The method from which "view" the data should be retrieved. Default "NCSV".
+
+        :return: saves file with data
+        '''
+
+        # start_date is optional: if not provided, the data are taken from the very beginning
+        if start_date is not None:
+            # date only
+            try:
+                datetime.strptime(start_date, "%Y-%m-%d")
+                start_date = start_date + "T00:00:00"
+            except:
+                # if cannot parse to date only, it may contain time
+                try:
+                    datetime.strptime(start_date, "%Y-%m-%dT%H:%M:%S")
+                except:
+                    raise Exception(f'Wrong format of date is passed for start date.'
+                                    f'The accepted datetime formats are: YYYY-MM-DD or YYYY-MM-DDTHH:mm:ss. '
+                                    f'E.g., 2021-02-05 or 2021-02-05T12:30:00')
+
+        # start_date is optional: if not provided, the data are taken from the very beginning
+        if end_date is not None:
+            # date only
+            try:
+                datetime.strptime(end_date, "%Y-%m-%d")
+                # till the end of day
+                end_date = end_date + "T23:59:59"
+            except:
+                # if cannot parse to date only, it may contain time
+                try:
+                    datetime.strptime(end_date, "%Y-%m-%dT%H:%M:%S")
+                except:
+                    raise Exception(f'Wrong format of date is passed for end date.'
+                                    f'The accepted datetime formats are: YYYY-MM-DD or YYYY-MM-DDTHH:mm:ss.'
+                                    f'E.g., 2021-02-05 or 2021-02-05T12:30:00'
+                                    )
+
+        # Cast columns argument as list
+        if not isinstance(columns, list):
+            columns = [columns]
+
+
+        # Payload Body of the REQUEST
+        body = {"startDate": start_date,
+                "endDate": end_date,
+                "keys": [
+                    {"symbols": symbols,
+                    "groupName": group_name,
+                    "columns": columns,
+                    "pattern": allow_wildcard
+                     }
+                ],
+                "corrections": corrections,
+                "delta": delta,
+                "formatType": output_format
+                }
+
+        # add extra fields in the payload if needed
+        if timezone is not None:
+            # Check the format for the timezone
+            assert '/' in timezone, 'Wrongly formatted timezone argument. Must be for example Europe/London'
+ 
+            # return dates in wanted timezone
+            body["timeZone"] = timezone
+
+        # return metadata
+        body['metadata'] = metadata
+
+        # Check that if a wild_card was passed, the patter was set to True
+        if ('*' in body['keys'][0]['symbols'].values()) and (allow_wildcard is False):
+            raise ValueError('If passing a wildcard in the symbols, allow_wildcard must be True')
+
+
+        # Summary
+        log.debug(f'Retrieving data for symbols: {symbols} '
+                  f'\nand columns: {columns}'
+                  f'\nfrom date: {start_date}'
+                  f'\nto date: {end_date}')
+
+        
         # Request
         r = self.caller.post(path='/ts', payload=body)
+
         log.debug(f'Response: {r.text}')
 
         try:
 
             # Get file as NCSV API format
-            if NCSV:
+            if output_format == 'NCSV':
                 # return raw bytes directly
-                fileIO = io.BytesIO(r.content)
+                fileIO = StringIO(str(r.content, encoding='utf-8'))
 
                 if file_name is None:
                     # return the raw Bytes (streamed)
                     return fileIO
 
                 else:
                     # Check that the extension is in the file, else add it as csv by default
                     file_name = file_name if '.' in file_name else file_name + '.csv'
 
                     # Save the downloaded data on the disk
                     with open(file_name, "w") as text_file:
                         text_file.write(r.text)
 
+            # Get file as STANDARD API format
+            elif output_format=='STANDARD':
+                # return the JSON for the Horizontal format
+                file = json.load(io.BytesIO(r.content))['values']
+                
+                if file_name is None:
+                    # return raw JSON format of the data
+                    return file
+
+                else:
+                    # Check that the extension is in the file, else add it as csv by default
+                    file_name = file_name if '.' in file_name else file_name + '.csv'
+
+                    # Save the downloaded data on the disk
+                    with open(file_name, "w") as file_to_write:
+                        json.dump(file, file_to_write)
+            
             # Get file as PANDAS API format
-            else:
+            elif output_format=='PANDAS':
+                # return the JSON for the Horizontal format
+                file = json.load(io.BytesIO(r.content))['data']
+
+                if file_name is None:
+                    # return raw JSON format of the data
+                    return file
+
+                else:
+                    # Check that the extension is in the file, else add it as csv by default
+                    file_name = file_name if '.' in file_name else file_name + '.csv'
+
+                    # Save the downloaded data on the disk
+                    with open(file_name, "w") as file_to_write:
+                        json.dump(file, file_to_write)
+
+            # Get file as UI API format
+            elif output_format=='UI':
                 # return the JSON for the Horizontal format
-                file_json = json.load(io.BytesIO(r.content))['data']
+                file = json.load(io.BytesIO(r.content))['values']
 
                 if file_name is None:
                     # return raw JSON format of the data
-                    return file_json
+                    return file
 
                 else:
                     # Check that the extension is in the file, else add it as csv by default
                     file_name = file_name if '.' in file_name else file_name + '.csv'
 
                     # Save the downloaded data on the disk
                     with open(file_name, "w") as file_to_write:
-                        json.dump(file_json, file_to_write)
+                        json.dump(file, file_to_write)
+        
+            else:
+                raise ValueError('{} format of the timeseries output is not supported. Please use NCSV, PANDAS or STANDARD'.format(output_format))
 
         except :
             # Get unique list of symbols
             raw_list = self.get_symbols(group_name)['items']
             symb_list = set([item for sublist in [list(d['symbols'].keys()) for d in raw_list] for item in sublist])
 
             # Raise error with symbols list
             raise ValueError('Wrong Symbols or Columns passed to the query . It should match the data structure on the group: {}'.format(symb_list))
 
         log.debug('Data are saved to file: {}'.format(file_name))
 
         return
+    
 
     def upload_data(self, file_name, symbols_columns, date_column, group_name):
         '''
         The methods uploads data to Timeseries by re-arranging the columns order and uploading the new file as NCSV.
         :param file_name: csv file to be upload to Timeseries
         :param symbols_columns: columns to be used as symbols
         :param date_column: date column in the file; is renamed to DateTime as expected by NCSV
```

### Comparing `generalindex-0.1.3/generalindex/__init__.py` & `generalindex-0.1.4/generalindex/__init__.py`

 * *Files identical despite different names*

### Comparing `generalindex-0.1.3/generalindex.egg-info/PKG-INFO` & `generalindex-0.1.4/generalindex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,731 +1,731 @@
-Metadata-Version: 2.1
-Name: generalindex
-Version: 0.1.3
-Summary: Python SDK for the General Index platform
-Home-page: https://www.general-index.com/
-Author: General Index
-Author-email: info@general-index.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GENERAL INDEX PYTHON SDK #
-
-This document describes the General Index Python SDK which enables external users to use the GX platform tools within their python scripts. 
-
-The Python SDK can be used within:
-
-- a single python script that is ran thanks to the Python Runner task within a pipeline in the GX application
-
-- a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the GX application
-
-- an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the GX application
-
- 
-
-Note that the SDK does not cover everything from API documentation but rather commonly used features.
-
-The scope of the SDK:
-
-- **Datalake Handler** - downloading / uploading / reading files from the data lake  
-
-- **Status Handler** - sending statuses about the task run  
-
-- **Task Handler** - enables communication between tasks within a pipeline and reading/writing parameters 
-
-- **Time Series Handler** - retrieves data directly from the time series database
-
-
-
-## How to install and set the package: 
-### Install
-```text
-pip3 install generalindex==0.1.3
-```
-As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
-```text
-generalindex==0.1.3
-```
-The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
-```text
-pip3 install requests==2.25.1
-```
-
-
-### Environment Variables
-The package uses information from the environment variables. They are automatically provided when running a script within a pipeline (as a Task or within the Python/Jupyter Runners).
-If running locally the script, users must set them in the project to be able to run the project locally.
-
- 
-
-Mandatory environment variables to set:
-
-- LOGIN → login received from GX
-
-- PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
-
-- NG_API_ENDPOINT → the URL to the GX platform API (by default, the url is set to https://api.g-x.co)
- 
-
-This allows to pass the authentication process and directs users' requests to the GX environment API.
-
-Other variables may be useful when creating the tasks within the platform:
-
-- NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
-
-- JOBID → any value; when the pipeline is executed, this value is set by the GX platform
-
-- PIPELINE_ID → any value; when the pipeline is created, this value is set by the GX platform
-
-
-
- --- - 
-## Datalake Handler
-### How to download or read a file from data lake by its name ?
-The DatalakeHandler class can be used as follow within a script to download or upload a file:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# download file from data lake with name and group name
-# it will be saved locally with name local_name.csv
-dh.download_by_name(file_name='my_file.csv', 
-                    group_name='My Group', 
-                    file_type='SOURCE',
-                    dest_file_name='folder/local_name.csv',
-                    save=True,
-                    unzip=False)
-
-# OR read file from data lake with name and group name
-# it returns a BytesIO object (kept in the RAM, not saved in the disk)
-fileIO = dh.download_by_name(file_name='my_file.csv', 
-                            group_name='My Group',
-                            file_type='SOURCE',
-                            dest_file_name=None,
-                            save=False,
-                            unzip=False)
-
-# read the object as pandas DataFrame
-df = pd.read_csv(fileIO)
-
-```
-The download methods allows to either:
-- download and save locally the wanted file, if *save=True*
-- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
-
-Note that by default:
-- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
-- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
-
-
-
-### How to download or read a file from data lake by its ID ?
-In the case that the file ID is known, it can be directly downloaded/read as follow:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# download file from data lake by its ID
-# it will be saved locally with name local_name.csv
-dh.download_by_id(file_id='XXXX-XXXX', 
-                  dest_file_name='folder/local_name.csv',
-                  save=True,
-                  unzip=False)
-
-# read file from data lake by its ID
-# it returns a BytesIO object
-fileIO = dh.download_by_id(file_id='XXXX-XXXX', 
-                            dest_file_name=None,
-                            save=False,
-                            unzip=False)
-
-# read the object as pandas DataFrame
-df = pd.read_csv(fileIO)
-
-```
-The download methods allows to either:
-- download and save locally the wanted file, if *save=True*
-- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
-
-Note that by default:
-- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
-- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
-
-
-
-
-
-### How to upload a file to the data lake?
-The uploading method will upload to the given group the file at the specified path, and returns its ID on the lake:
-```python
-import generalindex as gx
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# upload file to data lake
-file_id = dh.upload_file(file='path/local_name.csv', 
-                        group_name='My Group', 
-                        file_upload_name='name_in_the_datalake.csv')
-```
-It is possible as well to stream a python object's content directly to the datalake from memory, without having to save the file on the disk.
-
-The prerequisite is to pass to the uploading method a BytesIO object (not other objects such as pandas Dataframe).
-
-```python
-import generalindex as gx
-import io
-
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-# Turn the pandas DataFrame (df) to BytesIO for streaming
-fileIO = io.BytesIO(df.to_csv().encode()) 
-
-# upload file to data lake
-file_id = dh.upload_file(file=fileIO, 
-                        group_name='My Group', 
-                        file_upload_name='name_in_the_datalake.csv')
-```
---- -
-## Timeseries Queries
-### How to get the list of existing symbols for a given group ?
-Data saved in the time series database is structured by group, keys and timestamp.
-Each set of keys has unique dates entries in the database, with corresponding columns values.
-
-To explore what are the available symbols for a given group, the following method can be used:
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-group = 'My Group'
-group_symbols = ts.get_symbols(group_name=group)
-```
-The default size of the returned list is 1 000 items.
-
-Note that the return object from the get_symbols() method is a JSON (python dict) where the keys and columns are accessible in the *items* key of the JSON.
-
-### How to query by metadata or descriptions?
-
-In order to find the symbols querying by the metadata, column or symbol names, search_for parameter may be used.
-It will look for passed string in the whole time series database and return the JSON with keys and columns where searched string appears.
-
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-search = 'Data description'
-searched_symbols = ts.get_symbols(search_for=search)
-```
-
-Passing both group_name and search_for parameters of the get_symbols() method allows to narrow down the results from selected group.
-The user must provide either group_name or search_for to the method in order to obtain the symbols.
-
-
-If trying to get the list of symbols from a group that contains more than 1 000 items, the results will be paginated (by default into chunks of 1 000 items).
-To navigate in the large results the *get_symbols()* method takes as extra arguments the size of the returned list and the from page:
-```python
-import generalindex as gx
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Get the list of symbols for given group
-group = 'My Group'
-
-# Get the results into chunks of 200 items for page 5
-# meaning the results from the 1000th till the 1200th 
-group_symbols = ts.get_symbols(group_name=group, _size=200, _from=5)
-```
-By default, these parameters are _size=2000 (the maximum limit for the items lengths) and _from=0.
-
-
-### How to read data from Timeseries database?
-It is possible to use the SDK to directly query the TimeSeries database for data, given the symbol's keys, columns and the datalake group it is stored on.
-
-On the application, it is similar of creating a Dataprep instance, that selects a set of symbols from groups into a basket. 
-
-The retrieved data can be:
-- streamed directly to memory, retrieved as a BytesIO object, by setting *file_name* as None (default value), 
-- saved as a csv file locally with the provided path and name as *file_name*.
-
-The symbols are the keys the data was saved with in the database. For a given symbol, all the keys must be passed, as a dictionary object with the key name and value.
-It is possible to use a wildcard for the symbols values, to have all the values for that key, using *.
-
-The wanted columns are then passed as a list that can contain one or more items.
-If an empty list [ ] is passed to the function, it returns all the available columns.
-
-To read all available data for specific symbols and columns with no time frame, no start or end date are passed to the method.
-
-Extra settings are as well available to query data:
-- Metadata: to either return it in the query of not
-- Format: either get a Normalized CSV (NCSV) or a dataframe format
-- Timezone: get the timestamps in the timezone of the user's account or get the data in a specific timezone
-- Corrections: how to handle corrections to the TimeSeries database (corrections set to 'yes', 'no', 'history' or 'only')
-- Delta: whether to show by datatimestamp file (delta=False) or insert time (delta=True)
-
-
-The following code shows an example of how to query the TimseSeries database: :
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group acccording to keys & columns 
-# and save as query.csv in test/
-ts.retrieve_data_as_csv(file_name='test/query.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group'
-                        )
-
-# The retrieved data can be read as a pandas dataframe
-df = pd.read_csv("test/query.csv")
-
-
-# retrieve all available data from group acccording to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to read data from Timeseries for specific dates?
-To retrieve data the data within specific time frame, user can specify the start and end date.
-
-There are two options how the start and end date may look like:
-
-- only date (e.g., 2021-01-04)
-
-- date and time (e.g., 2021-02-01T12:00:00; ISO format must be followed)
-
-For example, if user specified start_date=2021-02-01 and end_date=2021-02-06, then data will be retrieved like this: from 2021-02-01 00:00:00 till 2021-02-06 23:59:59.
-
-If date and time is specified then data will be retrieved exactly for the specified time frame.
-
-Note that ISO format must be followed: YYYY-MM-DD**T**HH:mm:ss. Pay attention to the "T" letter between date and time.
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = 'Open'
-
-# retrieve data between start_date and end_date
-# data will be retrieved between 2021-01-04 00:00:00 and 2021-02-05 23:59:59
-# saved as a csv file named test.csv
-ts.retrieve_data_as_csv(file_name='test/test.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group',
-                        start_date='2021-01-04',
-                        end_date='2021-02-05'
-                        )
-
-# retrieve data for specific time frame
-# from 2021-01-04 12:30:00
-# to 2021-02-05 09:15:00
-ts.retrieve_data_as_csv(file_name='test/test.csv',
-                        symbols=symbols,
-                        columns=columns,
-                        group_name='My Group',
-                        start_date='2021-01-04T12:30:00',
-                        end_date='2021-02-05T09:15:00'
-                        )
-
-
-# For given keys, columns, group and dates range
-# Streaming instead of saving
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 start_date='2021-01-04',
-                                 end_date='2021-02-05'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to use a wildcard for a key's values ?
-To get all the value for one a several keys for the query, the character * can be used as a wildcard.
-The argument *allow_wildcard* should be set to True in the retrieval function to enable the use of wildcard. 
-
-Please note that by default, the use of wildcards is **DISABLED**.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "*"}
-columns = ['Open', 'Close']
-
-# retrieve all history for the symbols with keys and columns
-# all values for Key3 will be returned
-# the data will be streamed to memory
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 allow_wildcard=True
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-
-### How to get all the columns for a given set of keys ?
-To get all the columns values for a given set of keys in the database, the query can take an empty list as the queried columns, as follow:
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "Val3"}
-columns = []
-
-# retrieve all history for the symbols with keys and columns
-# all columns for the set of keys will be returned
-# the data will be streamed to memory
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-Note that this configuration can be used with keys wildcards (with *allow_wildacrd=True*) and any other setting.
-
-
-### How to modify the Time Zone of the data ?
-The timestamps in the queried time series are set by default in the timezone of the user's account, who created the script or the pipeline.
-It is described in the Date column header between brackets (for example *Date(UTC)*)
-
-To modify the time zone in the retrieved dataset, the timezone can be passed directly to the retrieval function as follow.
-It must respect the Continent/City format.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 timezone='Europe/London'
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-### How to get the metadata along with the data ? 
-It is possible to get extra columns in the retrieved data, along with the keys & columns values, containing the metadata of the symbols.
-It is done by setting the argument *metadata=True* in the retrieval function.
-
-By default, no metadata is included in the queried data.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-fileIO = ts.retrieve_data_as_csv(file_name=None,
-                                 symbols=symbols,
-                                 columns=columns,
-                                 group_name='My Group',
-                                 metadata=True
-                                 )
-
-# read as pandas dataframe
-df = pd.read_csv(fileIO)
-```
-
-
-### How to modify the format of the received data ?
-The queried data comes by default as Normalized CSV format (NCSV), with in this order:
-* the keys columns,
-* the date column, with timestamps in either the default timezone or the specified one (*timezone* argument in the function),
-* the values columns,
-* the metadata columns, if wanted (*metadata=True*)
- 
-By setting *NCSV=False* in the retrieval method, the data will be returned as Dataframe format (PANDAS in API docs), as a JSON.
-The JSON (python dict) has timestamps as keys and a dictionary containing pairs of symbols_columns and their value.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate Timeseries class
-ts = gx.Timeseries()
-
-# Symbols to query from database
-symbols = {'Key1': "Val1", "Key2": "Val2"}
-columns = ['Open', 'Close']
-
-# retrieve all available data from group according to keys & columns 
-# and stream to memory as BytesIO object
-file_json = ts.retrieve_data_as_csv(file_name=None,
-                                    symbols=symbols,
-                                    columns=columns,
-                                    group_name='My Group',
-                                    metadata=True,
-                                    NCSV=False
-                                    )
-
-# read as pandas dataframe
-# Transpose to have datetime as rows index
-df = pd.DataFrame(file_json).T
-```
-
-Note that the dataframe, created from the JSON containing the data, is then transposed to have timestamps as DatetimeIndex (along rows axis). 
-
-
---- - 
-## Task Handler
-Users can extend the existing set of tasks on GX platform by executing scripts or notebooks respectively from the Python Runner Task or the Jupyter Runner Task. 
-
-This task then can be used in a pipeline and be able to communicate with other tasks by:
-
-- reading outputs from other tasks, as inputs
-- writing outputs, that can be used by others tasks as inputs
-
-A task can as well receive inputs directly as a file picked from the datalake, either for a specific file either for the newest available version of a file on the lake, given its name and group.
-
-Whithin a python script, run into either one of the **Python Runner Task**,  this is implemented as follow:
-
-### Read a Task Input
-The input file passed to the Task can be: 
-- either downloaded to the disk,
-- either to be read on the fly (useful when limited space on the disk but not in memory).
-
- ```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-
-# the current task reads the file passed by a previous task, that is connected to it.
-# The passed file is downloaded and saved on the disk as data.csv
-th.download_from_input_parameter(arg_name='Input #1', 
-                                 dest_file_name='data.csv',
-                                 save=True)
-
-# The passed file is downloaded and kept in the memory (streamed, not saved on the disk)
-file_content = th.download_from_input_parameter(arg_name='Input #2', 
-                                                dest_file_name=None,
-                                                save=False)
-
-# If a csv file was streamed, it can be read as pandas Dataframe for example
-df = pd.read_csv(file_content)
-```
-
-If dest_file_name=None then the file is saved on the disk with its original name from the datalake.
-
-### How to obtain additional file information
-
-There is a possibility to retrieve information related to the input parameters using the DatalakeHandler (```dh.get_info_from_id()```) and TaskHandler (``` th.read_task_parameter_value()```) together.
-
-```python
-import generalindex as gx
-import pandas as pd
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-# Instantiate the Datalake Handler
-dh = gx.DatalakeHandler()
-
-dh.get_info_from_id(th.read_task_parameter_value('Input #1'))
-
-``` 
-This can be used to retrieve any metadata associated with the file itself like file name or arrival time (time it was uploaded to the system)
-
-### Set a Task Output
-The output of the Task can be set :
-- either by uploading a file saved on the disk to the datalake,
-- either by streaming the python object content to the datalake as the destination file.
-
-Once uploaded, the Output is set to point to the file on the datalake (by its ID, name ,group name)
-
-
- ```python
-import generalindex as gx
-import io
-
-# Instantiate TaskHandler class
-th = gx.TaskHandler()
-
-# the first task uploads the file dataset.csv to My Final Group and pass the info about this file
-# so that the next task can read this file by connecting its input to the output Prepared Dataset
-th.upload_to_output_parameter(output_name='Output #1', 
-                              file='path/dataset.csv', 
-                              group_name='My Final Group',
-                              file_upload_name=None,
-                              file_type='SOURCE')
-
-# Convert the python object to upload as BytesIO object
-df_io = io.BytesIO(df.to_csv().encode())
-
-# Stream to the datalake as the destination file
-th.upload_to_output_parameter(output_name='Output #1', 
-                              file=df_io, 
-                              group_name='My Final Group',
-                              file_upload_name='dataset.csv',
-                              file_type='SOURCE')
-```
-
-If file_upload_name=None then the saved file will be uploaded with its original name.
-If the file is streamed directly to the datalake, the file_upload_name argument must be set.
-
---- -
-## Statuses
-Sending status can be used to show in the application what is the progress of the task execution. It allows to use 3 different levels: 
-- FINISHED (green),
-- WARNING (orange), 
-- ERROR (red).
-
-Sending statuses remains optional as the GX platform sends general statuses.
-Only if user needs to pass some specific information in the status, this is worth using.
-
-```python
-import generalindex as gx
-
-# Instantiate the Status Handler
-sh = gx.StatusHandler()
-
-# Generic status sender
-sh.send_status(status='INFO', message='Crucial Information')
-
-# there are pre-defined statuses
-sh.info(message='Pipeline Finished Successfully')
-sh.warn(message='Something suspicious is happening ...')
-sh.error(message='Oops, the task failed ...')
-```
-
-Note that the info status is informing the status service that the task executed successfully and is finished.
-
---- -
-## Example
-To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
-
-Below is an example of a class that has 3 methods:
-
-- Download raw data (or take from the previous task)
-- Process the data  
-- Upload the data to datalake and pass it to the next task
-
- ```python
-import io
-import generalindex as gx
-import pandas as pd
-
-class Runner:
-    def __init__(self):
-        # Inherit the methods from the SDK Task Handler class
-        self.handler = gx.TaskHandler()
-        self.df = None
-        
-    def download_data(self):
-        # the method from TaskHandler can be used directly
-        # it downloads the file passed as input Dataset and save it as data.csv
-        self.handler.download_from_input_parameter(arg_name='Dataset', dest_file_name='data.csv', save=True)
-        
-        # Read as pandas dataframe
-        return pd.read_csv("data.csv")
-        
-    
-    def process_data(self, df):
-        # any logic here that processed the downloaded dataset and saves it as processed_data.csv
-        
-        return df_processed
-
-    
-    def upload_data(self, df_processed):
-        # Encode as bytesIO
-        fileIO = io.BytesIO(df_processed.to_csv().encode())
-        
-        # pass the processed data csv file as the output of the task called Processed Data
-        self.handler.upload_to_output_parameter(output_name='Processed Dataset', file=fileIO, group_name='Final Group')
-    
-        
-    def run(self):
-        df = self.download_data()
-        df_processed = self.process_data(df)
-        self.upload_data(df_processed)
-        
-        
-if __name__ == '__main__':
-    status = gx.StatusHandler()
-    Runner().run()
-    status.info('Test Pipeline Finished')
-
- ```
-
-
-### Who do I talk to? ###
-* Admin: General Index info@general-index.com
+Metadata-Version: 2.1
+Name: generalindex
+Version: 0.1.4
+Summary: Python SDK for the General Index platform
+Home-page: https://www.general-index.com/
+Author: General Index
+Author-email: info@general-index.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GENERAL INDEX PYTHON SDK #
+
+This document describes the General Index Python SDK which enables external users to use the GX platform tools within their python scripts. 
+
+The Python SDK can be used within:
+
+- a single python script that is ran thanks to the Python Runner task within a pipeline in the GX application
+
+- a single Jupyter Notebook that is ran thanks to the Jupyter Runner task within a pipeline in the GX application
+
+- an ensemble of python scripts that are part of a container, for a Task created by the user, used in a pipeline in the GX application
+
+ 
+
+Note that the SDK does not cover everything from API documentation but rather commonly used features.
+
+The scope of the SDK:
+
+- **Datalake Handler** - downloading / uploading / reading files from the data lake  
+
+- **Status Handler** - sending statuses about the task run  
+
+- **Task Handler** - enables communication between tasks within a pipeline and reading/writing parameters 
+
+- **Time Series Handler** - retrieves data directly from the time series database
+
+
+
+## How to install and set the package: 
+### Install
+```text
+pip3 install generalindex==0.1.3
+```
+As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
+```text
+generalindex==0.1.3
+```
+The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
+```text
+pip3 install requests==2.25.1
+```
+
+
+### Environment Variables
+The package uses information from the environment variables. They are automatically provided when running a script within a pipeline (as a Task or within the Python/Jupyter Runners).
+If running locally the script, users must set them in the project to be able to run the project locally.
+
+ 
+
+Mandatory environment variables to set:
+
+- LOGIN → login received from GX
+
+- PASSWORD → password to log in. Credentials are used to generate the token so that each request is authenticated.
+
+- NG_API_ENDPOINT → the URL to the GX platform API (by default, the url is set to https://api.g-x.co)
+ 
+
+This allows to pass the authentication process and directs users' requests to the GX environment API.
+
+Other variables may be useful when creating the tasks within the platform:
+
+- NG_STATUS_GROUP_NAME → the group on the data lake where the pipeline is located, and is used to display the statuses
+
+- JOBID → any value; when the pipeline is executed, this value is set by the GX platform
+
+- PIPELINE_ID → any value; when the pipeline is created, this value is set by the GX platform
+
+
+
+ --- - 
+## Datalake Handler
+### How to download or read a file from data lake by its name ?
+The DatalakeHandler class can be used as follow within a script to download or upload a file:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# download file from data lake with name and group name
+# it will be saved locally with name local_name.csv
+dh.download_by_name(file_name='my_file.csv', 
+                    group_name='My Group', 
+                    file_type='SOURCE',
+                    dest_file_name='folder/local_name.csv',
+                    save=True,
+                    unzip=False)
+
+# OR read file from data lake with name and group name
+# it returns a BytesIO object (kept in the RAM, not saved in the disk)
+fileIO = dh.download_by_name(file_name='my_file.csv', 
+                            group_name='My Group',
+                            file_type='SOURCE',
+                            dest_file_name=None,
+                            save=False,
+                            unzip=False)
+
+# read the object as pandas DataFrame
+df = pd.read_csv(fileIO)
+
+```
+The download methods allows to either:
+- download and save locally the wanted file, if *save=True*
+- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
+
+Note that by default:
+- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
+- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
+
+
+
+### How to download or read a file from data lake by its ID ?
+In the case that the file ID is known, it can be directly downloaded/read as follow:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# download file from data lake by its ID
+# it will be saved locally with name local_name.csv
+dh.download_by_id(file_id='XXXX-XXXX', 
+                  dest_file_name='folder/local_name.csv',
+                  save=True,
+                  unzip=False)
+
+# read file from data lake by its ID
+# it returns a BytesIO object
+fileIO = dh.download_by_id(file_id='XXXX-XXXX', 
+                            dest_file_name=None,
+                            save=False,
+                            unzip=False)
+
+# read the object as pandas DataFrame
+df = pd.read_csv(fileIO)
+
+```
+The download methods allows to either:
+- download and save locally the wanted file, if *save=True*
+- read the file directly from the datalake and get a BytesIO object (kept in memory only, that can for example be read by pandas as a dataframe directly)
+
+Note that by default:
+- the file is NOT saved locally, but returned as a BytesIO object (streamed from the datalake).
+- the argument *dest_file_name=None*, which will save the downloaded file to the root folder with its original name.
+
+
+
+
+
+### How to upload a file to the data lake?
+The uploading method will upload to the given group the file at the specified path, and returns its ID on the lake:
+```python
+import generalindex as gx
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# upload file to data lake
+file_id = dh.upload_file(file='path/local_name.csv', 
+                        group_name='My Group', 
+                        file_upload_name='name_in_the_datalake.csv')
+```
+It is possible as well to stream a python object's content directly to the datalake from memory, without having to save the file on the disk.
+
+The prerequisite is to pass to the uploading method a BytesIO object (not other objects such as pandas Dataframe).
+
+```python
+import generalindex as gx
+import io
+
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+# Turn the pandas DataFrame (df) to BytesIO for streaming
+fileIO = io.BytesIO(df.to_csv().encode()) 
+
+# upload file to data lake
+file_id = dh.upload_file(file=fileIO, 
+                        group_name='My Group', 
+                        file_upload_name='name_in_the_datalake.csv')
+```
+--- -
+## Timeseries Queries
+### How to get the list of existing symbols for a given group ?
+Data saved in the time series database is structured by group, keys and timestamp.
+Each set of keys has unique dates entries in the database, with corresponding columns values.
+
+To explore what are the available symbols for a given group, the following method can be used:
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+group = 'My Group'
+group_symbols = ts.get_symbols(group_name=group)
+```
+The default size of the returned list is 1 000 items.
+
+Note that the return object from the get_symbols() method is a JSON (python dict) where the keys and columns are accessible in the *items* key of the JSON.
+
+### How to query by metadata or descriptions?
+
+In order to find the symbols querying by the metadata, column or symbol names, search_for parameter may be used.
+It will look for passed string in the whole time series database and return the JSON with keys and columns where searched string appears.
+
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+search = 'Data description'
+searched_symbols = ts.get_symbols(search_for=search)
+```
+
+Passing both group_name and search_for parameters of the get_symbols() method allows to narrow down the results from selected group.
+The user must provide either group_name or search_for to the method in order to obtain the symbols.
+
+
+If trying to get the list of symbols from a group that contains more than 1 000 items, the results will be paginated (by default into chunks of 1 000 items).
+To navigate in the large results the *get_symbols()* method takes as extra arguments the size of the returned list and the from page:
+```python
+import generalindex as gx
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Get the list of symbols for given group
+group = 'My Group'
+
+# Get the results into chunks of 200 items for page 5
+# meaning the results from the 1000th till the 1200th 
+group_symbols = ts.get_symbols(group_name=group, _size=200, _from=5)
+```
+By default, these parameters are _size=2000 (the maximum limit for the items lengths) and _from=0.
+
+
+### How to read data from Timeseries database?
+It is possible to use the SDK to directly query the TimeSeries database for data, given the symbol's keys, columns and the datalake group it is stored on.
+
+On the application, it is similar of creating a Dataprep instance, that selects a set of symbols from groups into a basket. 
+
+The retrieved data can be:
+- streamed directly to memory, retrieved as a BytesIO object, by setting *file_name* as None (default value), 
+- saved as a csv file locally with the provided path and name as *file_name*.
+
+The symbols are the keys the data was saved with in the database. For a given symbol, all the keys must be passed, as a dictionary object with the key name and value.
+It is possible to use a wildcard for the symbols values, to have all the values for that key, using *.
+
+The wanted columns are then passed as a list that can contain one or more items.
+If an empty list [ ] is passed to the function, it returns all the available columns.
+
+To read all available data for specific symbols and columns with no time frame, no start or end date are passed to the method.
+
+Extra settings are as well available to query data:
+- Metadata: to either return it in the query of not
+- Format: either get a Normalized CSV (NCSV) or a dataframe format
+- Timezone: get the timestamps in the timezone of the user's account or get the data in a specific timezone
+- Corrections: how to handle corrections to the TimeSeries database (corrections set to 'yes', 'no', 'history' or 'only')
+- Delta: whether to show by datatimestamp file (delta=False) or insert time (delta=True)
+
+
+The following code shows an example of how to query the TimseSeries database: :
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group acccording to keys & columns 
+# and save as query.csv in test/
+ts.retrieve_data_as_csv(file_name='test/query.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group'
+                        )
+
+# The retrieved data can be read as a pandas dataframe
+df = pd.read_csv("test/query.csv")
+
+
+# retrieve all available data from group acccording to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to read data from Timeseries for specific dates?
+To retrieve data the data within specific time frame, user can specify the start and end date.
+
+There are two options how the start and end date may look like:
+
+- only date (e.g., 2021-01-04)
+
+- date and time (e.g., 2021-02-01T12:00:00; ISO format must be followed)
+
+For example, if user specified start_date=2021-02-01 and end_date=2021-02-06, then data will be retrieved like this: from 2021-02-01 00:00:00 till 2021-02-06 23:59:59.
+
+If date and time is specified then data will be retrieved exactly for the specified time frame.
+
+Note that ISO format must be followed: YYYY-MM-DD**T**HH:mm:ss. Pay attention to the "T" letter between date and time.
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = 'Open'
+
+# retrieve data between start_date and end_date
+# data will be retrieved between 2021-01-04 00:00:00 and 2021-02-05 23:59:59
+# saved as a csv file named test.csv
+ts.retrieve_data_as_csv(file_name='test/test.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group',
+                        start_date='2021-01-04',
+                        end_date='2021-02-05'
+                        )
+
+# retrieve data for specific time frame
+# from 2021-01-04 12:30:00
+# to 2021-02-05 09:15:00
+ts.retrieve_data_as_csv(file_name='test/test.csv',
+                        symbols=symbols,
+                        columns=columns,
+                        group_name='My Group',
+                        start_date='2021-01-04T12:30:00',
+                        end_date='2021-02-05T09:15:00'
+                        )
+
+
+# For given keys, columns, group and dates range
+# Streaming instead of saving
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 start_date='2021-01-04',
+                                 end_date='2021-02-05'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to use a wildcard for a key's values ?
+To get all the value for one a several keys for the query, the character * can be used as a wildcard.
+The argument *allow_wildcard* should be set to True in the retrieval function to enable the use of wildcard. 
+
+Please note that by default, the use of wildcards is **DISABLED**.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "*"}
+columns = ['Open', 'Close']
+
+# retrieve all history for the symbols with keys and columns
+# all values for Key3 will be returned
+# the data will be streamed to memory
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 allow_wildcard=True
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+
+### How to get all the columns for a given set of keys ?
+To get all the columns values for a given set of keys in the database, the query can take an empty list as the queried columns, as follow:
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2", "Key3": "Val3"}
+columns = []
+
+# retrieve all history for the symbols with keys and columns
+# all columns for the set of keys will be returned
+# the data will be streamed to memory
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+Note that this configuration can be used with keys wildcards (with *allow_wildacrd=True*) and any other setting.
+
+
+### How to modify the Time Zone of the data ?
+The timestamps in the queried time series are set by default in the timezone of the user's account, who created the script or the pipeline.
+It is described in the Date column header between brackets (for example *Date(UTC)*)
+
+To modify the time zone in the retrieved dataset, the timezone can be passed directly to the retrieval function as follow.
+It must respect the Continent/City format.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 timezone='Europe/London'
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+### How to get the metadata along with the data ? 
+It is possible to get extra columns in the retrieved data, along with the keys & columns values, containing the metadata of the symbols.
+It is done by setting the argument *metadata=True* in the retrieval function.
+
+By default, no metadata is included in the queried data.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+fileIO = ts.retrieve_data_as_csv(file_name=None,
+                                 symbols=symbols,
+                                 columns=columns,
+                                 group_name='My Group',
+                                 metadata=True
+                                 )
+
+# read as pandas dataframe
+df = pd.read_csv(fileIO)
+```
+
+
+### How to modify the format of the received data ?
+The queried data comes by default as Normalized CSV format (NCSV), with in this order:
+* the keys columns,
+* the date column, with timestamps in either the default timezone or the specified one (*timezone* argument in the function),
+* the values columns,
+* the metadata columns, if wanted (*metadata=True*)
+ 
+By setting *NCSV=False* in the retrieval method, the data will be returned as Dataframe format (PANDAS in API docs), as a JSON.
+The JSON (python dict) has timestamps as keys and a dictionary containing pairs of symbols_columns and their value.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate Timeseries class
+ts = gx.Timeseries()
+
+# Symbols to query from database
+symbols = {'Key1': "Val1", "Key2": "Val2"}
+columns = ['Open', 'Close']
+
+# retrieve all available data from group according to keys & columns 
+# and stream to memory as BytesIO object
+file_json = ts.retrieve_data_as_csv(file_name=None,
+                                    symbols=symbols,
+                                    columns=columns,
+                                    group_name='My Group',
+                                    metadata=True,
+                                    NCSV=False
+                                    )
+
+# read as pandas dataframe
+# Transpose to have datetime as rows index
+df = pd.DataFrame(file_json).T
+```
+
+Note that the dataframe, created from the JSON containing the data, is then transposed to have timestamps as DatetimeIndex (along rows axis). 
+
+
+--- - 
+## Task Handler
+Users can extend the existing set of tasks on GX platform by executing scripts or notebooks respectively from the Python Runner Task or the Jupyter Runner Task. 
+
+This task then can be used in a pipeline and be able to communicate with other tasks by:
+
+- reading outputs from other tasks, as inputs
+- writing outputs, that can be used by others tasks as inputs
+
+A task can as well receive inputs directly as a file picked from the datalake, either for a specific file either for the newest available version of a file on the lake, given its name and group.
+
+Whithin a python script, run into either one of the **Python Runner Task**,  this is implemented as follow:
+
+### Read a Task Input
+The input file passed to the Task can be: 
+- either downloaded to the disk,
+- either to be read on the fly (useful when limited space on the disk but not in memory).
+
+ ```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+
+# the current task reads the file passed by a previous task, that is connected to it.
+# The passed file is downloaded and saved on the disk as data.csv
+th.download_from_input_parameter(arg_name='Input #1', 
+                                 dest_file_name='data.csv',
+                                 save=True)
+
+# The passed file is downloaded and kept in the memory (streamed, not saved on the disk)
+file_content = th.download_from_input_parameter(arg_name='Input #2', 
+                                                dest_file_name=None,
+                                                save=False)
+
+# If a csv file was streamed, it can be read as pandas Dataframe for example
+df = pd.read_csv(file_content)
+```
+
+If dest_file_name=None then the file is saved on the disk with its original name from the datalake.
+
+### How to obtain additional file information
+
+There is a possibility to retrieve information related to the input parameters using the DatalakeHandler (```dh.get_info_from_id()```) and TaskHandler (``` th.read_task_parameter_value()```) together.
+
+```python
+import generalindex as gx
+import pandas as pd
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+# Instantiate the Datalake Handler
+dh = gx.DatalakeHandler()
+
+dh.get_info_from_id(th.read_task_parameter_value('Input #1'))
+
+``` 
+This can be used to retrieve any metadata associated with the file itself like file name or arrival time (time it was uploaded to the system)
+
+### Set a Task Output
+The output of the Task can be set :
+- either by uploading a file saved on the disk to the datalake,
+- either by streaming the python object content to the datalake as the destination file.
+
+Once uploaded, the Output is set to point to the file on the datalake (by its ID, name ,group name)
+
+
+ ```python
+import generalindex as gx
+import io
+
+# Instantiate TaskHandler class
+th = gx.TaskHandler()
+
+# the first task uploads the file dataset.csv to My Final Group and pass the info about this file
+# so that the next task can read this file by connecting its input to the output Prepared Dataset
+th.upload_to_output_parameter(output_name='Output #1', 
+                              file='path/dataset.csv', 
+                              group_name='My Final Group',
+                              file_upload_name=None,
+                              file_type='SOURCE')
+
+# Convert the python object to upload as BytesIO object
+df_io = io.BytesIO(df.to_csv().encode())
+
+# Stream to the datalake as the destination file
+th.upload_to_output_parameter(output_name='Output #1', 
+                              file=df_io, 
+                              group_name='My Final Group',
+                              file_upload_name='dataset.csv',
+                              file_type='SOURCE')
+```
+
+If file_upload_name=None then the saved file will be uploaded with its original name.
+If the file is streamed directly to the datalake, the file_upload_name argument must be set.
+
+--- -
+## Statuses
+Sending status can be used to show in the application what is the progress of the task execution. It allows to use 3 different levels: 
+- FINISHED (green),
+- WARNING (orange), 
+- ERROR (red).
+
+Sending statuses remains optional as the GX platform sends general statuses.
+Only if user needs to pass some specific information in the status, this is worth using.
+
+```python
+import generalindex as gx
+
+# Instantiate the Status Handler
+sh = gx.StatusHandler()
+
+# Generic status sender
+sh.send_status(status='INFO', message='Crucial Information')
+
+# there are pre-defined statuses
+sh.info(message='Pipeline Finished Successfully')
+sh.warn(message='Something suspicious is happening ...')
+sh.error(message='Oops, the task failed ...')
+```
+
+Note that the info status is informing the status service that the task executed successfully and is finished.
+
+--- -
+## Example
+To simplify the use of the SDK methods in a script, Python SDK methods can be inherited by the user’s main class. 
+
+Below is an example of a class that has 3 methods:
+
+- Download raw data (or take from the previous task)
+- Process the data  
+- Upload the data to datalake and pass it to the next task
+
+ ```python
+import io
+import generalindex as gx
+import pandas as pd
+
+class Runner:
+    def __init__(self):
+        # Inherit the methods from the SDK Task Handler class
+        self.handler = gx.TaskHandler()
+        self.df = None
+        
+    def download_data(self):
+        # the method from TaskHandler can be used directly
+        # it downloads the file passed as input Dataset and save it as data.csv
+        self.handler.download_from_input_parameter(arg_name='Dataset', dest_file_name='data.csv', save=True)
+        
+        # Read as pandas dataframe
+        return pd.read_csv("data.csv")
+        
+    
+    def process_data(self, df):
+        # any logic here that processed the downloaded dataset and saves it as processed_data.csv
+        
+        return df_processed
+
+    
+    def upload_data(self, df_processed):
+        # Encode as bytesIO
+        fileIO = io.BytesIO(df_processed.to_csv().encode())
+        
+        # pass the processed data csv file as the output of the task called Processed Data
+        self.handler.upload_to_output_parameter(output_name='Processed Dataset', file=fileIO, group_name='Final Group')
+    
+        
+    def run(self):
+        df = self.download_data()
+        df_processed = self.process_data(df)
+        self.upload_data(df_processed)
+        
+        
+if __name__ == '__main__':
+    status = gx.StatusHandler()
+    Runner().run()
+    status.info('Test Pipeline Finished')
+
+ ```
+
+
+### Who do I talk to? ###
+* Admin: General Index info@general-index.com
```

