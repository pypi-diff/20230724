# Comparing `tmp/logkk-0.5.0.tar.gz` & `tmp/logkk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkk-0.5.0.tar", last modified: Thu Apr 13 03:07:10 2023, max compression
+gzip compressed data, was "logkk-0.6.0.tar", last modified: Mon Jul 24 08:04:37 2023, max compression
```

## Comparing `logkk-0.5.0.tar` & `logkk-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.230152 logkk-0.5.0/
--rw-rw-rw-   0        0        0     1267 2023-04-13 03:07:10.225179 logkk-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      833 2023-03-03 10:19:55.000000 logkk-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.202143 logkk-0.5.0/logkk/
--rw-rw-rw-   0        0        0       69 2023-03-03 04:07:46.000000 logkk-0.5.0/logkk/__init__.py
--rw-rw-rw-   0        0        0      206 2023-03-03 04:07:33.000000 logkk-0.5.0/logkk/errors.py
--rw-rw-rw-   0        0        0      896 2023-04-13 03:03:46.000000 logkk-0.5.0/logkk/handlers.py
--rw-rw-rw-   0        0        0      134 2023-03-01 03:30:08.000000 logkk-0.5.0/logkk/level.py
--rw-rw-rw-   0        0        0     2347 2023-03-03 09:07:54.000000 logkk-0.5.0/logkk/logger.py
--rw-rw-rw-   0        0        0     1739 2023-03-03 09:07:54.000000 logkk-0.5.0/logkk/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.223144 logkk-0.5.0/logkk.egg-info/
--rw-rw-rw-   0        0        0     1267 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 03:07:10.000000 logkk-0.5.0/logkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 03:07:10.230152 logkk-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-04-13 03:04:28.000000 logkk-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:37.041709 logkk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-24 08:04:37.041709 logkk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-24 08:04:23.000000 logkk-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:37.041709 logkk-0.6.0/logkk/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-24 08:04:23.000000 logkk-0.6.0/logkk/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 08:04:37.041709 logkk-0.6.0/logkk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-24 08:04:37.000000 logkk-0.6.0/logkk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 08:04:37.000000 logkk-0.6.0/logkk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 08:04:37.000000 logkk-0.6.0/logkk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 08:04:37.000000 logkk-0.6.0/logkk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 08:04:37.041709 logkk-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 08:04:23.000000 logkk-0.6.0/setup.py
```

### Comparing `logkk-0.5.0/logkk/manager.py` & `logkk-0.6.0/logkk/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from logkk.level import Level
-from logkk.logger import Logger
-from logkk.handlers import Handler
-
-DEFAULT_FORMAT = "[{datetime}] [{level}] [{name}] {message}"
-
-
-class LogManager(object):
-
-    def __init__(self,
-                 name="logcc",
-                 level=Level.INFO,
-                 fmt=DEFAULT_FORMAT,
-                 handlers=None):
-        self.name = name
-        self.level = level
-        self.fmt = fmt
-        self.handlers = handlers or []
-        self._default_logger = self.get_logger(self.name)
-
-    def set_format(self, fmt: str):
-        self.fmt = fmt
-
-    def set_level(self, level: int):
-        self.level = level
-
-    def add_handler(self, handler: Handler):
-        self.handlers.append(handler)
-
-    def get_logger(self, name=None) -> Logger:
-        """
-        :param name: 模块名称或者文件名称
-        :return: Logger对象
-        """
-        return Logger(name=name or self.name,
-                      level=self.level,
-                      fmt=self.fmt,
-                      handlers=self.handlers)
-
-    def debug(self, *args, **kwargs):
-        self._default_logger.info(*args, **kwargs)
-
-    def info(self, *args, **kwargs):
-        self._default_logger.info(*args, **kwargs)
-
-    def warn(self, *args, **kwargs):
-        self._default_logger.info(*args, **kwargs)
-
-    def error(self, *args, **kwargs):
-        self._default_logger.info(*args, **kwargs)
-
-
-if __name__ == "__main__":
-    log_manager = LogManager()
-    log_manager.info("this is a info log")
-    log_manager.warn("this is a warn log")
-    logger = log_manager.get_logger(name="hello")
-    logger.info("this is a info log")
-    logger.warn("this is a warn log")
+from logkk.level import Level
+from logkk.logger import Logger
+from logkk.handlers import Handler
+
+DEFAULT_FORMAT = "[{datetime}] [{level}] [{module_name}] [{function_name}] {message}"
+
+
+class LogManager(object):
+
+    def __init__(self,
+                 name="logkk",
+                 level=Level.INFO,
+                 fmt=DEFAULT_FORMAT,
+                 handlers=None):
+        self.name = name
+        self.level = level
+        self.fmt = fmt
+        self.handlers = handlers or []
+        self._default_logger = self.get_logger(self.name)
+
+    def set_format(self, fmt: str):
+        self.fmt = fmt
+
+    def set_level(self, level: int):
+        self.level = level
+
+    def add_handler(self, handler: Handler):
+        self.handlers.append(handler)
+
+    def get_logger(self, module_name=None, function_name=None) -> Logger:
+        """
+        :param module_name: 模块名称或者文件名称
+        :param function_name: 函数名称
+        :return: Logger对象
+        """
+        return Logger(module_name=module_name or self.name,
+                      function_name=function_name,
+                      level=self.level,
+                      fmt=self.fmt,
+                      handlers=self.handlers)
+
+    def debug(self, *args, **kwargs):
+        self._default_logger.info(*args, **kwargs)
+
+    def info(self, *args, **kwargs):
+        self._default_logger.info(*args, **kwargs)
+
+    def warn(self, *args, **kwargs):
+        self._default_logger.info(*args, **kwargs)
+
+    def error(self, *args, **kwargs):
+        self._default_logger.info(*args, **kwargs)
+
+
+if __name__ == "__main__":
+    log_manager = LogManager()
+    log_manager.info("this is a info log")
+    log_manager.warn("this is a warn log")
+    logger = log_manager.get_logger(module_name="main")
+    logger.info("this is a info log")
+    logger.warn("this is a warn log")
```

### Comparing `logkk-0.5.0/setup.py` & `logkk-0.6.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="logkk",  # 模块名称
-    version="0.5.0",  # 当前版本
-    author="olivetree",  # 作者
-    author_email="olivetree123@163.com",  # 作者邮箱
-    description="日志组件",  # 模块简介
-    long_description=long_description,  # 模块详细介绍
-    long_description_content_type="text/markdown",  # 模块详细介绍格式
-    url="https://github.com/olivetree/logkk",  # 模块github地址
-    packages=["logkk"],  # 自动找到项目中导入的模块
-    # 模块相关的元数据（更多的描述）
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    # 依赖模块
-    install_requires=[],
-    # python版本
-    python_requires=">=3.7",
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="logkk",  # 模块名称
+    version="0.6.0",  # 当前版本
+    author="olivetree",  # 作者
+    author_email="olivetree123@163.com",  # 作者邮箱
+    description="日志组件",  # 模块简介
+    long_description=long_description,  # 模块详细介绍
+    long_description_content_type="text/markdown",  # 模块详细介绍格式
+    url="https://github.com/olivetree/logkk",  # 模块github地址
+    packages=["logkk"],  # 自动找到项目中导入的模块
+    # 模块相关的元数据（更多的描述）
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    # 依赖模块
+    install_requires=[],
+    # python版本
+    python_requires=">=3.7",
+)
```

