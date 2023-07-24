# Comparing `tmp/echoss_fileformat-0.1.tar.gz` & `tmp/echoss_fileformat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_fileformat-0.1.tar", last modified: Tue Apr 25 03:39:43 2023, max compression
+gzip compressed data, was "echoss_fileformat-0.2.tar", last modified: Mon Jul 24 06:39:45 2023, max compression
```

## Comparing `echoss_fileformat-0.1.tar` & `echoss_fileformat-0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:39:43.984366 echoss_fileformat-0.1/
--rw-rw-rw-   0        0        0    27030 2023-04-25 02:38:23.000000 echoss_fileformat-0.1/LICENSE
--rw-rw-rw-   0        0        0      268 2023-04-25 03:39:43.983367 echoss_fileformat-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1980 2023-04-25 03:28:00.000000 echoss_fileformat-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 03:39:43.902370 echoss_fileformat-0.1/echoss_fileformat/
--rw-rw-rw-   0        0        0      612 2023-04-24 02:01:28.000000 echoss_fileformat-0.1/echoss_fileformat/__init__.py
--rw-rw-rw-   0        0        0    10620 2023-04-24 07:16:34.000000 echoss_fileformat-0.1/echoss_fileformat/csv_handler.py
--rw-rw-rw-   0        0        0     8299 2023-04-25 03:35:10.000000 echoss_fileformat-0.1/echoss_fileformat/excel_handler.py
--rw-rw-rw-   0        0        0     9160 2023-04-24 07:18:08.000000 echoss_fileformat-0.1/echoss_fileformat/feather_handler.py
--rw-rw-rw-   0        0        0     7087 2023-04-24 07:23:07.000000 echoss_fileformat-0.1/echoss_fileformat/fileformat_base.py
--rw-rw-rw-   0        0        0    16835 2023-04-24 07:18:08.000000 echoss_fileformat-0.1/echoss_fileformat/json_handler.py
--rw-rw-rw-   0        0        0    17953 2023-04-24 07:18:08.000000 echoss_fileformat-0.1/echoss_fileformat/xml_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:39:43.924366 echoss_fileformat-0.1/echoss_fileformat.egg-info/
--rw-rw-rw-   0        0        0      268 2023-04-25 03:39:43.000000 echoss_fileformat-0.1/echoss_fileformat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-04-25 03:39:43.000000 echoss_fileformat-0.1/echoss_fileformat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:39:43.000000 echoss_fileformat-0.1/echoss_fileformat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-25 03:39:43.000000 echoss_fileformat-0.1/echoss_fileformat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 03:39:43.000000 echoss_fileformat-0.1/echoss_fileformat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 03:39:43.984366 echoss_fileformat-0.1/setup.cfg
--rw-rw-rw-   0        0        0      450 2023-04-25 03:36:53.000000 echoss_fileformat-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 03:39:43.979365 echoss_fileformat-0.1/tests/
--rw-rw-rw-   0        0        0     8346 2023-04-25 03:04:35.000000 echoss_fileformat-0.1/tests/test_csv_handler.py
--rw-rw-rw-   0        0        0    10576 2023-04-25 03:04:35.000000 echoss_fileformat-0.1/tests/test_excel_handler.py
--rw-rw-rw-   0        0        0     4400 2023-04-25 03:19:37.000000 echoss_fileformat-0.1/tests/test_feather_handler.py
--rw-rw-rw-   0        0        0     5671 2023-03-02 05:16:27.000000 echoss_fileformat-0.1/tests/test_fileformat_handler.py
--rw-rw-rw-   0        0        0    11599 2023-04-25 03:18:53.000000 echoss_fileformat-0.1/tests/test_json_handler.py
--rw-rw-rw-   0        0        0     6248 2023-03-07 00:58:48.000000 echoss_fileformat-0.1/tests/test_xml_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:39:45.952854 echoss_fileformat-0.2/
+-rw-rw-rw-   0        0        0    27030 2023-04-25 02:38:23.000000 echoss_fileformat-0.2/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-07-24 06:39:45.951852 echoss_fileformat-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1980 2023-04-25 03:28:00.000000 echoss_fileformat-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 06:39:45.789854 echoss_fileformat-0.2/echoss_fileformat/
+-rw-rw-rw-   0        0        0      829 2023-04-25 07:07:21.000000 echoss_fileformat-0.2/echoss_fileformat/__init__.py
+-rw-rw-rw-   0        0        0    10575 2023-04-25 04:52:58.000000 echoss_fileformat-0.2/echoss_fileformat/csv_handler.py
+-rw-rw-rw-   0        0        0     3814 2023-04-25 07:51:03.000000 echoss_fileformat-0.2/echoss_fileformat/dataframe_util.py
+-rw-rw-rw-   0        0        0     8299 2023-04-25 03:35:10.000000 echoss_fileformat-0.2/echoss_fileformat/excel_handler.py
+-rw-rw-rw-   0        0        0     9160 2023-04-24 07:18:08.000000 echoss_fileformat-0.2/echoss_fileformat/feather_handler.py
+-rw-rw-rw-   0        0        0     7087 2023-04-24 07:23:07.000000 echoss_fileformat-0.2/echoss_fileformat/fileformat_base.py
+-rw-rw-rw-   0        0        0    16835 2023-04-24 07:18:08.000000 echoss_fileformat-0.2/echoss_fileformat/json_handler.py
+-rw-rw-rw-   0        0        0    17953 2023-04-24 07:18:08.000000 echoss_fileformat-0.2/echoss_fileformat/xml_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:39:45.825853 echoss_fileformat-0.2/echoss_fileformat.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-07-24 06:39:45.000000 echoss_fileformat-0.2/echoss_fileformat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-07-24 06:39:45.000000 echoss_fileformat-0.2/echoss_fileformat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 06:39:45.000000 echoss_fileformat-0.2/echoss_fileformat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-24 06:39:45.000000 echoss_fileformat-0.2/echoss_fileformat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-24 06:39:45.000000 echoss_fileformat-0.2/echoss_fileformat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 06:39:45.952854 echoss_fileformat-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      468 2023-07-24 06:38:16.000000 echoss_fileformat-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 06:39:45.948854 echoss_fileformat-0.2/tests/
+-rw-rw-rw-   0        0        0     5864 2023-04-25 07:12:38.000000 echoss_fileformat-0.2/tests/test_csv_handler.py
+-rw-rw-rw-   0        0        0    10553 2023-04-25 07:12:38.000000 echoss_fileformat-0.2/tests/test_excel_handler.py
+-rw-rw-rw-   0        0        0    10994 2023-04-25 07:56:09.000000 echoss_fileformat-0.2/tests/test_feather_handler.py
+-rw-rw-rw-   0        0        0     5671 2023-03-02 05:16:27.000000 echoss_fileformat-0.2/tests/test_fileformat_handler.py
+-rw-rw-rw-   0        0        0    11269 2023-04-25 07:12:38.000000 echoss_fileformat-0.2/tests/test_json_handler.py
+-rw-rw-rw-   0        0        0     6294 2023-04-25 04:03:09.000000 echoss_fileformat-0.2/tests/test_xml_handler.py
```

### Comparing `echoss_fileformat-0.1/LICENSE` & `echoss_fileformat-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/README.md` & `echoss_fileformat-0.2/README.md`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat/csv_handler.py` & `echoss_fileformat-0.2/echoss_fileformat/csv_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
                 sep=self.delimiter,
                 quotechar=self.quotechar,
                 escapechar=self.escapechar,
                 header=header,
                 skiprows=skiprows,
                 nrows=nrows,
                 usecols=usecols,
-                infer_datetime_format=True,
                 on_bad_lines='warn',
                 **kwargs
             )
 
             if self.processing_type == FileformatBase.TYPE_OBJECT:
                 return df
             else:
```

### Comparing `echoss_fileformat-0.1/echoss_fileformat/excel_handler.py` & `echoss_fileformat-0.2/echoss_fileformat/excel_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat/feather_handler.py` & `echoss_fileformat-0.2/echoss_fileformat/feather_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat/fileformat_base.py` & `echoss_fileformat-0.2/echoss_fileformat/fileformat_base.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat/json_handler.py` & `echoss_fileformat-0.2/echoss_fileformat/json_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat/xml_handler.py` & `echoss_fileformat-0.2/echoss_fileformat/xml_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/echoss_fileformat.egg-info/SOURCES.txt` & `echoss_fileformat-0.2/echoss_fileformat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 echoss_fileformat/__init__.py
 echoss_fileformat/csv_handler.py
+echoss_fileformat/dataframe_util.py
 echoss_fileformat/excel_handler.py
 echoss_fileformat/feather_handler.py
 echoss_fileformat/fileformat_base.py
 echoss_fileformat/json_handler.py
 echoss_fileformat/xml_handler.py
 echoss_fileformat.egg-info/PKG-INFO
 echoss_fileformat.egg-info/SOURCES.txt
```

### Comparing `echoss_fileformat-0.1/tests/test_csv_handler.py` & `echoss_fileformat-0.2/tests/test_json_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import unittest
 import time
 import logging
 import os
 
-from echoss_fileformat.csv_handler import CsvHandler
-from dataframe_print import print_table, print_dataframe, print_taburate
+from echoss_fileformat.json_handler import JsonHandler
 
 # configure the logger
 LOG_FORMAT = "%(asctime)s %(name)s %(levelname)s - %(message)s"
 logging.basicConfig(level=logging.INFO, format=LOG_FORMAT)
 logger = logging.getLogger(__name__)
 # use the logger
 
-verbose = True
 
 class MyTestCase(unittest.TestCase):
     """
         테스트 설정
     """
     def setUp(self):
         """Before test"""
@@ -30,164 +28,217 @@
         self.end_time = time.perf_counter()
         logger.info(f" tear down test [{self.str_id}] elapsed time {(self.end_time-self.start_time)*1000: .3f}ms \n")
 
     """
     유닛 테스트 
     """
 
-    def test_load_simple_standard_csv(self):
-        expect_pass = 1
-        expect_fail = 0
-        load_filename = 'test_data/simple_standard.csv'
-        dump_filename = 'test_data/simple_standard_to_delete.csv'
-        try:
-            handler = CsvHandler()
-            handler.load(load_filename, header=0, skiprows=0)
-            pass_size = len(handler.pass_list)
-            fail_size = len(handler.fail_list)
-            csv_df = handler.to_pandas()
-            if csv_df is not None:
-                if verbose:
-                    print_taburate(csv_df.head(10), logger.info)
-            else:
-                logger.info('empty dataframe')
-            expect_csv_str = "SEQ_NO,PROMTN_TY_CD,PROMTN_TY_NM,BRAND_NM,SVC_NM,ISSU_CO,PARTCPTN_CO,PSNBY_ISSU_CO,COUPON_CRTFC_CO,COUPON_USE_RT\r\n"+"0,9,대만프로모션발급인증통계,77chocolate,S0013,15,15,1.0,15,1.0"
-            csv_str = handler.dumps()
-            # logger.info("[\n"+csv_str+"]")
-            expect_file_size = 17827
-            self.assertTrue(csv_str.startswith(expect_csv_str), "startswith fail")
-
-            handler.dump(dump_filename)
-            exist = os.path.exists(dump_filename)
-            file_size = os.path.getsize(dump_filename)
-            if exist and 'to_delete' in dump_filename:
-                os.remove(dump_filename)
-
-            logger.info(f"\t {handler} dump expect exist True get {exist}")
-            logger.info(f"\t {handler} dump expect file_size {expect_file_size} get {file_size}")
-
-        except Exception as e:
-            logger.error(f"\t File load fail by {e}")
-            self.assertTrue(True, f"\t File load fail by {e}")
-        else:
-            logger.info(f"\t load expect pass {expect_pass} get {pass_size}")
-            self.assertTrue(pass_size == expect_pass)
-            logger.info(f"\t load expect fail {expect_fail} get {fail_size}")
-            self.assertTrue(fail_size == expect_fail)
-
-    def test_load_simple_standard_csv_by_mode(self):
-        modes = ['text', 'binary']
-        expect_shape = (212, 10)
-
-        load_filename = 'test_data/simple_standard.csv'
-        dump_filename = 'test_data/simple_standard_to_delete.csv'
-        for given_mode in modes:
-            expect_pass = 1
-            expect_fail = 0
-            try:
-                handler = CsvHandler()
-                if 'text' == given_mode:
-                    file_obj = open(load_filename, 'r', encoding='utf-8')
-                else:
-                    file_obj = open(load_filename, 'rb')
-                handler.load(file_obj, header=0, skiprows=0)
-
-                csv_df = handler.to_pandas()
-                if csv_df is not None and len(csv_df) > 0:
-                    df_shape = csv_df.shape
-                    if expect_shape == df_shape:
-                        logger.info(f"load mode={given_mode}, shape={csv_df.shape} are equal")
-                    else:
-                        logger.error(f"load mode={expect_shape}, and get shape={csv_df.shape}")
-                else:
-                    logger.error('empty dataframe')
-            except Exception as e:
-                logger.error(f"\t File load fail by {e}")
-                self.assertTrue(True, f"\t File load fail by {e}")
-            finally:
-                if file_obj:
-                    file_obj.close()
-                    file_obj = None
+    def test_load_complex_by_json_type(self):
+        json_types = ['object', 'array', 'multiline']
+        expect_passes = [0, 0, 0]
+        expect_fails = [0, 1, 1942]
 
+        for processing_type, expect_pass, expect_fail in zip(json_types, expect_passes, expect_fails):
             try:
-                if 'text' == given_mode:
-                    file_obj = open(dump_filename, 'w', encoding='utf-8')
-                else:
-                    file_obj = open(dump_filename, 'wb')
-                handler.dump(file_obj, quoting=0)
-                if file_obj:
-                    file_obj.close()
-                    file_obj = None
-
-                check_csv = CsvHandler()
-                check_csv.load(dump_filename)
-
-                check_df = check_csv.to_pandas()
-                if check_df is not None and len(check_df) > 0:
-                    df_shape = check_df.shape
-                    if expect_shape == df_shape:
-                        logger.info(f"dump mode={given_mode}, shape={check_df.shape} are equal")
-                    else:
-                        logger.error(f"dump mode={given_mode}, {expect_shape=} and get shape={check_df.shape}")
-                else:
-                    logger.error('dump and load make empty dataframe')
+                handler = JsonHandler(processing_type)
+                dict_obj = handler.load('test_data/complex_one_object.json')
+                pass_size = len(handler.pass_list)
+                fail_size = len(handler.fail_list)
+            except Exception as e:
+                self.assertTrue(True, f"\t {processing_type=} File load fail by {e}")
+            else:
+                logger.info(f"\t {processing_type=} assertEqual({expect_pass=}, {pass_size=})")
+                self.assertEqual(pass_size, expect_pass)
+                logger.info(f"\t {processing_type=} assertEqual({expect_fail=}, {fail_size=})")
+                self.assertEqual(fail_size, expect_fail)
 
-                if 'to_delete' in dump_filename:
-                    os.remove(dump_filename)
+    def test_load_complex_by_data_key(self):
+        json_types = ['object', 'array', 'multiline']
+        expect_passes = [0, 102, 0]
+        expect_fails = [0, 0, 1942]
 
+        for processing_type, expect_pass, expect_fail in zip(json_types, expect_passes, expect_fails):
+            try:
+                handler = JsonHandler(processing_type)
+                handler.load('test_data/complex_one_object.json', data_key='main')
+                pass_size = len(handler.pass_list)
+                fail_size = len(handler.fail_list)
             except Exception as e:
-                logger.error(f"\t File dump open mode={given_mode} fail by {e}")
-                self.assertTrue(True, f"\t File dump fail by {e}")
-            finally:
-                if file_obj:
-                    file_obj.close()
+                logger.error(f"\t {processing_type=} File load raise: {e}")
+                self.assertTrue(True, f"\t {processing_type=} File load raise: {e}")
+            else:
+                logger.info(f"\t {processing_type=} load assertEqual({expect_pass=}, {pass_size=})")
+                self.assertEqual(pass_size, expect_pass)
+                logger.info(f"\t {processing_type=} load assertEqual({expect_fail=}, {fail_size=})")
+                self.assertEqual(fail_size, expect_fail)
 
     def test_load_mutliline_by_mode(self):
-        processing_type = 'multiline'
         modes = ['text', 'binary']
-        expect_passes = [1, 1]
+        expect_passes = [15, 15]
         expect_fails = [0, 0]
 
         for mode, expect_pass, expect_fail in zip(modes, expect_passes, expect_fails):
             try:
-                handler = CsvHandler(processing_type)
+                handler = JsonHandler('multiline')
                 if mode == 'text':
                     with open('test_data/simple_multiline_object.json', 'r', encoding='utf-8') as fp:
                         handler.load(fp)
                         pass_size = len(handler.pass_list)
                         fail_size = len(handler.fail_list)
                 elif mode == 'binary':
                     with open('test_data/simple_multiline_object.json', 'rb') as fb:
                         handler.load(fb)
                         pass_size = len(handler.pass_list)
                         fail_size = len(handler.fail_list)
             except Exception as e:
-                logger.error(f"\t assertTrue {mode} multiline File load fail by {e}")
                 self.assertTrue(True, f"\t {mode} multiline File load fail by {e}")
             else:
-                logger.info(f"\t assertEqual({expect_pass}, {pass_size}) at {mode=}, {processing_type=}")
-                self.assertEqual(pass_size, expect_pass)
-                logger.info(f"\t assertEqual({expect_fail}, {fail_size}) at {mode=}, {processing_type=}")
-                self.assertEqual(fail_size, expect_fail)
+                logger.info(f"\t open mode '{mode}' 'multiline' expect pass {expect_pass} get {pass_size}")
+                # self.assertEqual(pass_size == expect_pass)
+                logger.info(f"\t open mode '{mode}' 'multiline' expect fail {expect_fail} get {fail_size}")
+                # self.assertEqual(fail_size == expect_fail)
 
     def test_load_mutliline_by_data_key(self):
-        json_types = ['object', 'array', 'multiline']
+        processing_types = ['object', 'array', 'multiline']
         expect_passes = [0, 0, 15]
         expect_fails = [1, 1, 0]
 
-        for json_type, expect_pass, expect_fail in zip(json_types, expect_passes, expect_fails):
+        for processing_type, expect_pass, expect_fail in zip(processing_types, expect_passes, expect_fails):
             try:
-                handler = CsvHandler(json_type)
+                handler = JsonHandler(processing_type)
                 handler.load('test_data/simple_multiline_object.json', data_key='message')
                 pass_size = len(handler.pass_list)
                 fail_size = len(handler.fail_list)
             except Exception as e:
-                self.assertTrue(True, f"\t {json_type} json_type File load fail by {e}")
+                self.assertTrue(True, f"\t {processing_type} json_type File load fail by {e}")
             else:
-                logger.info(f"\t {json_type} load expect pass {expect_pass} get {pass_size}")
+                logger.info(f"\t {processing_type} load expect pass {expect_pass} get {pass_size}")
                 self.assertTrue(pass_size == expect_pass)
-                logger.info(f"\t {json_type} load expect fail {expect_fail} get {fail_size}")
+                logger.info(f"\t {processing_type} load expect fail {expect_fail} get {fail_size}")
                 self.assertTrue(fail_size == expect_fail)
 
 
+    """
+    dump
+    """
+
+    def test_dump_complex_by_json_type(self):
+        json_types = ['object', 'array']
+        data_keys = ['', 'main']
+        expect_file_sizes = [35248, 32724]
+
+        load_filename = 'test_data/complex_one_object.json'
+        dump_filename = 'test_data/complex_one_object_dump_to_delete.json'
+
+        for processing_type, data_key, expect_file_size  in zip(json_types, data_keys, expect_file_sizes):
+            try:
+                handler = JsonHandler(processing_type)
+                dict_obj = handler.load(load_filename, data_key=data_key)
+                pass_size = len(handler.pass_list)
+
+                if processing_type == 'object':
+                    handler.dump(dump_filename, data=dict_obj)
+                else:
+                    handler.dump(dump_filename)
+                exist = os.path.exists(dump_filename)
+                file_size = os.path.getsize(dump_filename)
+
+                if exist and 'to_delete' in dump_filename:
+                    os.remove(dump_filename)
+
+                logger.info(f"\t assertEqual(True, {exist=}) at {processing_type=} dump")
+                self.assertEqual(True, exist)
+                logger.info(f"\t assertEqual({expect_file_size=}, {file_size=}) at {processing_type=} dump")
+                self.assertEqual(expect_file_size, file_size)
+            except Exception as e:
+                self.assertTrue(True, f"\t {processing_type} json_type File dump fail by {e}")
+
+    def test_dump_mutliline_by_mode(self):
+        # multiline 은 내부적으로 binary 로 동작하여 외부 지정이 의미가 없음
+        modes = ['text', 'binary']
+        expect_file_sizes = [13413, 13413]
+
+        json_type = JsonHandler.TYPE_MULTILINE
+        load_filename = 'test_data/simple_multiline_object.json'
+
+        for mode, expect_file_size in zip(modes, expect_file_sizes):
+            try:
+                handler = JsonHandler('multiline')
+                if mode == 'text':
+                    with open(load_filename, 'r', encoding='utf-8') as fp:
+                        handler.load(fp)
+                        pass_size = len(handler.pass_list)
+                        fail_size = len(handler.fail_list)
+                elif mode == 'binary':
+                    with open(load_filename, 'rb') as fb:
+                        handler.load(fb)
+                        pass_size = len(handler.pass_list)
+                        fail_size = len(handler.fail_list)
+            except Exception as e:
+                self.assertTrue(True, f"\t {mode} multiline File load fail by {e}")
+            else:
+                logger.info(f"\t open mode '{mode}' 'multiline' load {pass_size=}, {fail_size=}")
+
+            try:
+                dump_filename = f'test_data/simple_multiline_{mode}_object_to_delete.json'
+                handler.dump(dump_filename)
+                exist = os.path.exists(dump_filename)
+                file_size = os.path.getsize(dump_filename)
+
+                if exist and '_to_delete' in dump_filename:
+                    os.remove(dump_filename)
+
+                logger.info(f"\t {json_type} dump expect exist True get {exist}")
+                self.assertEqual(True, exist)
+                logger.info(f"\t {json_type} dump expect file_size {expect_file_size} get {file_size}")
+                self.assertEqual(expect_file_size, file_size)
+            except Exception as e:
+                self.assertTrue(True, f"\t {mode} multiline File load fail by {e}")
+
+
+    def test_dump_mutliline_by_data_key(self):
+        modes = ['text', 'binary']
+        data_keys = ['message', 'message']
+        expect_file_sizes = [10513, 10513]
+
+        json_type = JsonHandler.TYPE_MULTILINE
+        load_filename = 'test_data/simple_multiline_object.json'
+
+        for mode, data_key, expect_file_size in zip(modes, data_keys, expect_file_sizes):
+            try:
+                handler = JsonHandler('multiline')
+                if mode == 'text':
+                    with open(load_filename, 'r', encoding='utf-8') as fp:
+                        handler.load(fp, data_key=data_key)
+                        pass_size = len(handler.pass_list)
+                        fail_size = len(handler.fail_list)
+                elif mode == 'binary':
+                    with open(load_filename, 'rb') as fb:
+                        handler.load(fb, data_key=data_key)
+                        pass_size = len(handler.pass_list)
+                        fail_size = len(handler.fail_list)
+            except Exception as e:
+                self.assertTrue(True, f"\t {mode} multiline File load fail by {e}")
+                # logger.error(True, f"\t {mode} multiline File load fail by {e}")
+            else:
+                logger.info(f"\t open mode '{mode}' 'multiline' load {pass_size=}, {fail_size=}")
+
+            try:
+                dump_filename = f'test_data/simple_multiline_{mode}_object_to_delete.json'
+                handler.dump(dump_filename, data_key=data_key)
+                exist = os.path.exists(dump_filename)
+                file_size = os.path.getsize(dump_filename)
+
+                if exist and '_to_delete' in dump_filename:
+                    os.remove(dump_filename)
+
+                logger.info(f"\t {json_type} dump expect exist True get {exist}")
+                self.assertEqual(True, exist)
+                logger.info(f"\t {json_type} dump expect file_size {expect_file_size} get {file_size}")
+                self.assertEqual(expect_file_size, file_size)
+            except Exception as e:
+                self.assertTrue(True, f"\t {mode} multiline File load fail by {e}")
+                # logger.error(f"\t {mode} multiline File load fail by {e}")
+
+
 if __name__ == '__main__':
     unittest.main(verbosity=2)
```

### Comparing `echoss_fileformat-0.1/tests/test_excel_handler.py` & `echoss_fileformat-0.2/tests/test_excel_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import sys
 import pandas as pd
 import xlsxwriter
 
 from echoss_fileformat.excel_handler import ExcelHandler
-from dataframe_print import print_dataframe, print_table, print_taburate
+from echoss_fileformat.dataframe_util import print_table
 
 
 # configure the logger
 LOG_FORMAT = "%(asctime)s %(name)s %(levelname)s - %(message)s"
 logging.basicConfig(level=logging.INFO, format=LOG_FORMAT)
 logger = logging.getLogger(__name__)
 
@@ -91,15 +91,15 @@
             handler = ExcelHandler()
             handler.load(load_filename)
             pass_size = len(handler.pass_list)
             fail_size = len(handler.fail_list)
             df = handler.to_pandas()
             if df is not None:
                 if verbose:
-                    print_dataframe(df, logger.info)
+                    print_table(df, logger.info)
                 load_columns = list(df.columns)
                 load_len = len(df)
                 logger.info(f"\t expect dataframe len={expect_len} and get {len(df)}")
                 self.assertEqual(load_len, expect_len)
             else:
                 logger.info('\t empty dataframe')
 
@@ -131,15 +131,15 @@
         dump_filename = 'test_data/채널지수평가 샘플_v0.1_to_delete.xlsx'
         try:
             handler = ExcelHandler()
             handler.load(load_filename, sheet_name='Youtube생산성', skiprows=1, header=0, nrows=20, usecols='B:D')
             df = handler.to_pandas()
             if df is not None:
                 if verbose:
-                    print_taburate(df, print)
+                    print_table(df, print)
                 load_columns = list(df.columns)
                 load_shape = df.shape
                 logger.info(f"expect dataframe shape={expect_shape} and get {load_shape}")
                 self.assertEqual(expect_shape, load_shape)
             else:
                 logger.error('empty dataframe')
```

### Comparing `echoss_fileformat-0.1/tests/test_fileformat_handler.py` & `echoss_fileformat-0.2/tests/test_fileformat_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_fileformat-0.1/tests/test_xml_handler.py` & `echoss_fileformat-0.2/tests/test_xml_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
     def test_simple_object_load(self):
         processing_types = ['object', 'object']
         file_names = ['test_data/simple_config.xml', 'test_data/simple_pom.xml']
         expect_passes = [0, 0]
         expect_fails = [0, 0]
 
-        for processing_type, file_name, expect_pass, expect_fail in zip(processing_types, file_names, expect_passes, expect_fails):
+        for processing_type, file_name, expect_pass, expect_fail in \
+                zip(processing_types, file_names, expect_passes, expect_fails):
             try:
                 handler = XmlHandler(processing_type)
                 tree_obj = handler.load(file_name)
                 pass_size = len(handler.pass_list)
                 fail_size = len(handler.fail_list)
                 if verbose:
                     logger.info(f"{type(tree_obj)=}, {tree_obj=}")
@@ -99,15 +100,16 @@
             except Exception as e:
                 logger.error(f"\t {processing_type=} File dump raise: {e}")
                 self.assertTrue(True, f"\t {processing_type=} File dump raise: {e}")
 
     def test_load_array_by_data_key(self):
         processing_types = ['array', 'array']
         load_filenames = ['test_data/complex_one_object.xml', 'test_data/complex_one_object.xml']
-        dump_filenames = ['test_data/complex_one_object_to_delete_bndbox.xml', 'test_data/simple_pom_to_delete_object.xml']
+        dump_filenames = ['test_data/complex_one_object_to_delete_bndbox.xml',
+                          'test_data/simple_pom_to_delete_object.xml']
         data_keys = ['.//bndbox', './/object']
         expect_file_sizes = [1132, 11082]
 
         for processing_type, load_filename, dump_filename, data_key, expect_file_size \
                 in zip(processing_types, load_filenames, dump_filenames, data_keys, expect_file_sizes):
             try:
                 handler = XmlHandler(processing_type)
```

