# Comparing `tmp/openai_parallel_toolkit-0.5.2-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18556 bytes, number of entries: 19
--rw-r--r--  2.0 unx      184 b- defN 23-Jun-26 03:34 openai_parallel_toolkit/__init__.py
+Zip file size: 18761 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      184 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
--rw-r--r--  2.0 unx      150 b- defN 23-Jun-26 03:34 openai_parallel_toolkit/api/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     5216 b- defN 23-Jun-19 07:03 openai_parallel_toolkit/api/api.py
 -rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
 -rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
--rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
+-rw-r--r--  2.0 unx     4831 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/core/multithread.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Jun-19 11:22 openai_parallel_toolkit/utils/__init__.py
--rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Jul-24 13:49 openai_parallel_toolkit/utils/logger.py
 -rw-r--r--  2.0 unx     4107 b- defN 23-Jun-26 03:26 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13483 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1783 b- defN 23-Jun-26 03:34 openai_parallel_toolkit-0.5.2.dist-info/RECORD
-19 files, 47300 bytes uncompressed, 15558 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13483 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1783 b- defN 23-Jul-24 13:50 openai_parallel_toolkit-0.6.0.dist-info/RECORD
+19 files, 47627 bytes uncompressed, 15763 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.2.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.2.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.2.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.2.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.5.2.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .api import APIKeyManager, Gpt35Turbo, OpenAIModel, request_openai_api, Gpt35Turbo0613, Gpt4, Gpt35Turbo16K
+from .api import APIKeyManager, Gpt35Turbo, Gpt35Turbo0613, Gpt35Turbo16K, Gpt4, OpenAIModel, request_openai_api
 from .core import ParallelToolkit, multi_process_one, multi_thread_run
```

## openai_parallel_toolkit/api/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .api import OpenAIModel, Gpt35Turbo, Gpt35Turbo0613, Gpt4, Gpt35Turbo16K
+from .api import Gpt35Turbo, Gpt35Turbo0613, Gpt35Turbo16K, Gpt4, OpenAIModel
 from .keys import APIKeyManager
 from .request import request_openai_api
```

## openai_parallel_toolkit/core/multithread.py

```diff
@@ -2,18 +2,17 @@
 import logging
 import multiprocessing
 import os
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from typing import Type
 
-from openai_parallel_toolkit.api import APIKeyManager
-from openai_parallel_toolkit.api import request_openai_api, OpenAIModel
+from openai_parallel_toolkit.api import APIKeyManager, OpenAIModel, request_openai_api
 from openai_parallel_toolkit.config import LOG_LABEL
-from openai_parallel_toolkit.utils import ProgressBar, partition_data, read_folder, logger_init
+from openai_parallel_toolkit.utils import ProgressBar, logger_init, partition_data, read_folder
 
 
 def process_data_chunk(data_chunk, output_path, process_output, process_data):
     """Process a chunk of data and write results to output file.
 
     Args:
         data_chunk (dict): The data chunk to be processed.
@@ -38,14 +37,15 @@
         openai_model_class (Type[OpenAIModel]): The OpenAI model class to use.
         threads (int, optional): The number of threads to use. Defaults to 5 times the number of CPUs.
         **kwargs: Additional arguments for the OpenAI model class.
 
     Returns:
         list: The results from the OpenAI API.
     """
+    logger_init()
     with ThreadPoolExecutor(max_workers=threads) as executor:
         try:
             results = list(
                 executor.map(lambda item: request_openai_api(
                     openai_model_class(prompt=item[0], content=item[1], **kwargs)),
                              data))
         except Exception as e:
@@ -53,28 +53,28 @@
             logging.error(f"{LOG_LABEL}Error occurred while processing data: {e}\n{tb}")
             return None
     return results
 
 
 def multi_thread_run(config_path, input_path, file_count, output_path, process_input, process_output, process_data,
                      num_threads=multiprocessing.cpu_count() * 10, name="Progress"):
-    logger_init()
     """Run the processing task using multiple threads.
 
     Args:
         config_path (str): The path of the configuration file.
         input_path (str): The path of the input file.
         file_count (int): The number of files to be processed.
         output_path (str): The path of the output file.
         process_input (function): The function used to process the input.
         process_output (function): The function used to process the output.
         process_data (function): The function used to process the data.
         num_threads (int, optional): The number of threads to use. Defaults to 10 times the number of CPUs.
         name (str, optional): The name of the progress bar. Defaults to "Progress".
     """
+    logger_init()
     APIKeyManager(config_path=config_path)
     if output_path is not None:
         if not os.path.exists(output_path):
             os.makedirs(output_path)
     data = read_folder(input_path=input_path, file_count=file_count, output_path=output_path,
                        process_input=process_input)
     if data is None:
```

## openai_parallel_toolkit/utils/logger.py

```diff
@@ -14,15 +14,25 @@
         if self.label in record.getMessage():
             record.msg = record.msg.replace(self.label, '')
             return True
         else:
             return False
 
 
+# 创建一个全局变量用于保存logger
+_global_logger = None
+
+
 def logger_init(label=LOG_LABEL, level=logging.INFO, datefmt=None):
+    global _global_logger
+
+    # 检查全局变量是否已经被初始化
+    if _global_logger is not None:
+        return _global_logger
+
     logger = logging.getLogger()
     logger.setLevel(level)
     handler = logging.StreamHandler()
 
     log_colors = {
         'DEBUG': 'cyan',
         'INFO': 'green',
@@ -30,14 +40,19 @@
         'ERROR': 'red',
         'CRITICAL': 'red',
     }
 
     handler.addFilter(LogFilter(label))
 
     formatter = ColoredFormatter(
-        "%(log_color)s%(asctime)s - %(levelname)s - %(message)s",
-        datefmt=datefmt,
-        reset=True,
-        log_colors=log_colors
+            "%(log_color)s%(asctime)s - %(levelname)s - %(message)s",
+            datefmt=datefmt,
+            reset=True,
+            log_colors=log_colors
     )
     handler.setFormatter(formatter)
     logger.addHandler(handler)
+
+    # 将新创建的logger保存在全局变量中，以便后续使用
+    _global_logger = logger
+
+    return logger
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `openai_parallel_toolkit-0.5.2.dist-info/LICENSE` & `openai_parallel_toolkit-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.5.2.dist-info/METADATA` & `openai_parallel_toolkit-0.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.5.2
+Version: 0.6.0
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `openai_parallel_toolkit-0.5.2.dist-info/RECORD` & `openai_parallel_toolkit-0.6.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-openai_parallel_toolkit/__init__.py,sha256=u44miRj78hpYdl4SdE_USz7GLANZzosBMUbPQ9okyzs,184
+openai_parallel_toolkit/__init__.py,sha256=Ib6xSj6bOWlxJwogkm8EIMSr-vFcI_-4xPFx4WDjTsE,184
 openai_parallel_toolkit/config.py,sha256=UvWwqK1cxCx4XId6pswW4jkSF1XDozEg58RftfY8yxU,20
-openai_parallel_toolkit/api/__init__.py,sha256=wAUTdp_SZKJL0yQiRnEIhDo505fAOdLW7UeAg33z9_I,150
+openai_parallel_toolkit/api/__init__.py,sha256=iukhU5GckqphUPHFC3pCdhgELmSuAxYHor4OHYSHq_M,150
 openai_parallel_toolkit/api/api.py,sha256=KJgFQ_fZebwS0jxMiD0kzgPgpPWOH7DeEB7hvVqPBtU,5216
 openai_parallel_toolkit/api/keys.py,sha256=RB9BmU7Qth3QIUWP30KXcfgmyblWVFYUnH0uB538ISs,5809
 openai_parallel_toolkit/api/request.py,sha256=75V3R79jE055WovuwQp7Pp29Ib_NUCDbFFqYVyaBA0w,3034
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
 openai_parallel_toolkit/core/main.py,sha256=omai73kazjZ_8iHOaayG0jlfyPxwGUc8tYQ3M8bhQ2g,4532
-openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
+openai_parallel_toolkit/core/multithread.py,sha256=bfNl2_Eu3edCfo4xbFq4IB0o17DudONKgcbFtMk4x-o,4831
 openai_parallel_toolkit/utils/__init__.py,sha256=CyPVG9jS8tZGfoi5k-tFIyE9OKkyZ10vc7Ri91jOScM,148
-openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
+openai_parallel_toolkit/utils/logger.py,sha256=Xg-s_bWTX5sL_VZubVbdwX_5iMqvZMfHJb01SbOWW74,1390
 openai_parallel_toolkit/utils/reader.py,sha256=dNg4KLWMZI7-6zn2YGOPtCtg9X0Ogr7Qk2m6iYS3Ipg,4107
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.5.2.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.5.2.dist-info/METADATA,sha256=C5Z5FoI2YsPsQciP1abzPMc735Y33_igKnwQ3A5f4gA,13483
-openai_parallel_toolkit-0.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-0.5.2.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.5.2.dist-info/RECORD,,
+openai_parallel_toolkit-0.6.0.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.6.0.dist-info/METADATA,sha256=TRQGdAR__f0imcCQSOwb9e8LvbDCQDd799a-U_S5kVc,13483
+openai_parallel_toolkit-0.6.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-0.6.0.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.6.0.dist-info/RECORD,,
```

