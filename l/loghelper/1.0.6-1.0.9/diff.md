# Comparing `tmp/loghelper-1.0.6-py3-none-any.whl.zip` & `tmp/loghelper-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5180 bytes, number of entries: 6
+Zip file size: 5233 bytes, number of entries: 6
 -rw-r--r--  2.0 unx      573 b- defN 80-Jan-01 00:00 loghelper/__init__.py
--rw-r--r--  2.0 unx     8267 b- defN 80-Jan-01 00:00 loghelper/loghelper.py
+-rw-r--r--  2.0 unx     8813 b- defN 80-Jan-01 00:00 loghelper/loghelper.py
 -rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 loghelper/ver.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loghelper-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx     3287 b- defN 80-Jan-01 00:00 loghelper-1.0.6.dist-info/METADATA
-?rw-r--r--  2.0 unx      440 b- defN 16-Jan-01 00:00 loghelper-1.0.6.dist-info/RECORD
-6 files, 12894 bytes uncompressed, 4390 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     3237 b- defN 80-Jan-01 00:00 loghelper-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loghelper-1.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx      440 b- defN 16-Jan-01 00:00 loghelper-1.0.9.dist-info/RECORD
+6 files, 13390 bytes uncompressed, 4443 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: loghelper/loghelper.py
 Comment: 
 
 Filename: loghelper/ver.py
 Comment: 
 
-Filename: loghelper-1.0.6.dist-info/WHEEL
+Filename: loghelper-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: loghelper-1.0.6.dist-info/METADATA
+Filename: loghelper-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: loghelper-1.0.6.dist-info/RECORD
+Filename: loghelper-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loghelper/loghelper.py

```diff
@@ -190,47 +190,53 @@
     for _ in logger_handlers:
         if isinstance(_, logging.FileHandler):
             ret.append(_.baseFilename)
     return ret
 
 
 class SensitiveLogger:
-    def __init__(self, logger: logging.Logger):
+    def __init__(self, logger: logging.Logger, default_stacklevel=2):
         self.logger = logger
+        self.default_stacklevel = default_stacklevel
 
     def _gen_msg(self, msg, sensitive_msg, with_logger_file_path: bool = True):
         if sensitive_msg:
             _log_msg = f'{msg} (内容详情:{sensitive_msg})'
             if with_logger_file_path:
                 _ret_msg = f'{msg} (详见日志:{get_logger_file_handler_path(self.logger)})'
             else:
                 _ret_msg = f'{msg} (详见日志)'
         else:
             _log_msg = msg
             _ret_msg = msg
 
         return _log_msg, _ret_msg
 
-    def debug(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
+    def debug(self, msg: object, sensitive_msg: object = None,  *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.debug(msg=log_msg, *args, **kwargs)
+        stacklevel = kwargs.pop('stacklevel', self.default_stacklevel)
+        self.logger.debug(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def info(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.info(msg=log_msg, *args, **kwargs)
+        stacklevel = kwargs.pop('stacklevel', self.default_stacklevel)
+        self.logger.info(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def warning(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.warning(msg=log_msg, *args, **kwargs)
+        stacklevel = kwargs.pop('stacklevel', self.default_stacklevel)
+        self.logger.warning(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def error(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.error(msg=log_msg, *args, **kwargs)
+        stacklevel = kwargs.pop('stacklevel', self.default_stacklevel)
+        self.logger.error(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def critical(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.critical(msg=log_msg, *args, **kwargs)
+        stacklevel = kwargs.pop('stacklevel', self.default_stacklevel)
+        self.logger.critical(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
```

## loghelper/ver.py

```diff
@@ -3,11 +3,11 @@
 
 __author__ = "ITXiaoPang"
 __mtime__ = "2019/10/10"
 __project__ = "LogHelper"
 __file__ = "ver.py"
 __IDE__ = "PyCharm"
 
-__version__ = "1.00.06"
+__version__ = "1.00.09"
 
 if __name__ == "__main__":
     print(__version__)
```

## Comparing `loghelper-1.0.6.dist-info/METADATA` & `loghelper-1.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: loghelper
-Version: 1.0.6
+Version: 1.0.9
 Summary: 日志助手，支持多进程，支持json格式，支持flask
 Author: ITXiaoPang
 Author-email: itxiaopang.djh@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: concurrent
 Provides-Extra: flask
 Provides-Extra: json
```

