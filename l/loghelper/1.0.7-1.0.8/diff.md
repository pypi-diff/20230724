# Comparing `tmp/loghelper-1.0.7-py3-none-any.whl.zip` & `tmp/loghelper-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5207 bytes, number of entries: 6
+Zip file size: 5233 bytes, number of entries: 6
 -rw-r--r--  2.0 unx      573 b- defN 80-Jan-01 00:00 loghelper/__init__.py
--rw-r--r--  2.0 unx     8458 b- defN 80-Jan-01 00:00 loghelper/loghelper.py
+-rw-r--r--  2.0 unx     8813 b- defN 80-Jan-01 00:00 loghelper/loghelper.py
 -rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 loghelper/ver.py
--rw-r--r--  2.0 unx     3237 b- defN 80-Jan-01 00:00 loghelper-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loghelper-1.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx      440 b- defN 16-Jan-01 00:00 loghelper-1.0.7.dist-info/RECORD
-6 files, 13035 bytes uncompressed, 4417 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     3237 b- defN 80-Jan-01 00:00 loghelper-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loghelper-1.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx      440 b- defN 16-Jan-01 00:00 loghelper-1.0.8.dist-info/RECORD
+6 files, 13390 bytes uncompressed, 4443 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: loghelper/loghelper.py
 Comment: 
 
 Filename: loghelper/ver.py
 Comment: 
 
-Filename: loghelper-1.0.7.dist-info/METADATA
+Filename: loghelper-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: loghelper-1.0.7.dist-info/WHEEL
+Filename: loghelper-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: loghelper-1.0.7.dist-info/RECORD
+Filename: loghelper-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loghelper/loghelper.py

```diff
@@ -190,48 +190,53 @@
     for _ in logger_handlers:
         if isinstance(_, logging.FileHandler):
             ret.append(_.baseFilename)
     return ret
 
 
 class SensitiveLogger:
-    def __init__(self, logger: logging.Logger, stacklevel=2):
+    def __init__(self, logger: logging.Logger, default_stacklevel=2):
         self.logger = logger
-        self.stacklevel = stacklevel
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
-        self.logger.debug(msg=log_msg, stacklevel=self.stacklevel, *args, **kwargs)
+        stacklevel = kwargs.get('stacklevel', self.default_stacklevel)
+        self.logger.debug(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def info(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.info(msg=log_msg, stacklevel=self.stacklevel, *args, **kwargs)
+        stacklevel = kwargs.get('stacklevel', self.default_stacklevel)
+        self.logger.info(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def warning(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.warning(msg=log_msg, stacklevel=self.stacklevel, *args, **kwargs)
+        stacklevel = kwargs.get('stacklevel', self.default_stacklevel)
+        self.logger.warning(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def error(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.error(msg=log_msg, stacklevel=self.stacklevel, *args, **kwargs)
+        stacklevel = kwargs.get('stacklevel', self.default_stacklevel)
+        self.logger.error(msg=log_msg, stacklevel=stacklevel, *args, **kwargs)
         return ret_msg
 
     def critical(self, msg: object, sensitive_msg: object = None, *args, **kwargs):
         log_msg, ret_msg = self._gen_msg(msg, sensitive_msg)
-        self.logger.critical(msg=log_msg, stacklevel=self.stacklevel, *args, **kwargs)
+        stacklevel = kwargs.get('stacklevel', self.default_stacklevel)
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
 
-__version__ = "1.00.07"
+__version__ = "1.00.08"
 
 if __name__ == "__main__":
     print(__version__)
```

## Comparing `loghelper-1.0.7.dist-info/METADATA` & `loghelper-1.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loghelper
-Version: 1.0.7
+Version: 1.0.8
 Summary: 日志助手，支持多进程，支持json格式，支持flask
 Author: ITXiaoPang
 Author-email: itxiaopang.djh@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

