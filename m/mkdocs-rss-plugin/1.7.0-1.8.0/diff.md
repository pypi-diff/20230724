# Comparing `tmp/mkdocs-rss-plugin-1.7.0.tar.gz` & `tmp/mkdocs-rss-plugin-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-rss-plugin-1.7.0.tar", last modified: Sun May 28 15:15:13 2023, max compression
+gzip compressed data, was "mkdocs-rss-plugin-1.8.0.tar", last modified: Mon Jul 24 17:11:15 2023, max compression
```

## Comparing `mkdocs-rss-plugin-1.7.0.tar` & `mkdocs-rss-plugin-1.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/customtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_pre39.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_py39.py
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 15:15:13.000000 mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 15:15:13.102958 mkdocs-rss-plugin-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_rss_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-28 15:14:57.000000 mkdocs-rss-plugin-1.7.0/tests/test_timezoner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.327236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/customtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_pre39.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.327236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_build_no_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_rss_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_timezoner.py
```

### Comparing `mkdocs-rss-plugin-1.7.0/LICENSE` & `mkdocs-rss-plugin-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/PKG-INFO` & `mkdocs-rss-plugin-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rss-plugin
-Version: 1.7.0
+Version: 1.8.0
 Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
 Author: Julien Moura
 Author-email: dev@ingeoveritas.com
 License: MIT
 Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
 Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
 Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
```

### Comparing `mkdocs-rss-plugin-1.7.0/README.md` & `mkdocs-rss-plugin-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/__about__.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__about__.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 __summary__ = (
     "MkDocs plugin which generates a static RSS feed using git log and page.meta."
 )
 __title__ = "MkDocs RSS plugin"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/Guts/mkdocs-rss-plugin/"
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
     ]
 )
```

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/customtypes.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/customtypes.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/git_manager/ci.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/plugin.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,20 +54,19 @@
         ("enabled", config_options.Type(bool, default=True)),
         ("feed_ttl", config_options.Type(int, default=1440)),
         ("image", config_options.Type(str, default=None)),
         ("length", config_options.Type(int, default=20)),
         ("match_path", config_options.Type(str, default=".*")),
         ("pretty_print", config_options.Type(bool, default=False)),
         ("url_parameters", config_options.Type(dict, default=None)),
+        ("use_git", config_options.Type(bool, default=True)),
     )
 
     def __init__(self):
         """Instanciation."""
-        # tooling
-        self.util = Util()
         # dates source
         self.src_date_created = self.src_date_updated = "git"
         self.meta_datetime_format = None
         self.meta_default_timezone = "UTC"
         self.meta_default_time = None
         # pages storage
         self.pages_to_filter = []
@@ -90,14 +89,17 @@
         :rtype: dict
         """
 
         # Skip if disabled
         if not self.config.get("enabled"):
             return config
 
+        # instanciate plugin tooling
+        self.util = Util(use_git=self.config.get("use_git", True))
+
         # check template dirs
         if not Path(DEFAULT_TEMPLATE_FILENAME).is_file():
             raise FileExistsError(DEFAULT_TEMPLATE_FILENAME)
         self.tpl_file = Path(DEFAULT_TEMPLATE_FILENAME)
         self.tpl_folder = DEFAULT_TEMPLATE_FOLDER
 
         # start a feed dictionary using global config vars
@@ -148,18 +150,25 @@
                 except ValueError as err:
                     raise PluginError(
                         "[rss-plugin] Config error: `date_from_meta.default_time` value "
                         f"'{self.meta_default_time}' format doesn't match the expected "
                         f"format %H:%M. Trace: {err}"
                     )
 
-            logger.debug(
-                "[rss-plugin] Dates will be retrieved from page meta (yaml "
-                "frontmatter). The git log will be used as fallback."
-            )
+            if self.config.get("use_git", True):
+                logger.debug(
+                    "[rss-plugin] Dates will be retrieved FIRSTLY from page meta (yaml "
+                    "frontmatter). The git log will be used as fallback."
+                )
+            else:
+                logger.debug(
+                    "[rss-plugin] Dates will be retrieved ONLY from page meta (yaml "
+                    "frontmatter). The build date will be used as fallback, without any "
+                    "call to Git."
+                )
         else:
             logger.debug("[rss-plugin] Dates will be retrieved from git log.")
 
         # create 2 final dicts
         self.feed_created = deepcopy(base_feed)
         self.feed_updated = deepcopy(base_feed)
```

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/templates/rss.xml.jinja2` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/rss.xml.jinja2`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_pre39.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_pre39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/timezoner_py39.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_py39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin/util.py` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,34 +48,61 @@
 
 # ############################################################################
 # ########## Classes #############
 # ################################
 
 
 class Util:
-    def __init__(self, path: str = "."):
+    """Plugin logic."""
+
+    git_is_valid: bool = False
+
+    def __init__(self, path: str = ".", use_git: bool = True):
         """Class hosting the plugin logic.
 
         :param str path: path tot the git repository to use. Defaults to: "." - optional
+        :param bool use_git: flag to use git under the hood or not, defaults to True
         """
-        try:
-            git_repo = Repo(path, search_parent_directories=True)
-            self.repo = git_repo.git
-            self.git_is_valid = 1
-        except InvalidGitRepositoryError as err:
-            logging.warning(
-                f"[rss-plugin] Path '{path}' is not a valid git directory. Trace: {err}"
+        if use_git:
+            logger.debug("[rss-plugin] Git use is disabled.")
+            try:
+                git_repo = Repo(path, search_parent_directories=True)
+                self.repo = git_repo.git
+                self.git_is_valid = True
+            except InvalidGitRepositoryError as err:
+                logger.warning(
+                    f"[rss-plugin] Path '{path}' is not a valid git directory. "
+                    "Only page.meta (YAML frontmatter will be used). "
+                    "To disable this warning, set 'use_git: false' in plugin options. "
+                    f"Trace: {err}"
+                )
+                self.git_is_valid = False
+                use_git = False
+            except Exception as err:
+                logger.warning(
+                    f"[rss-plugin] Unrecognized git issue. "
+                    "Only page.meta (YAML frontmatter will be used). "
+                    "To disable this warning, set 'use_git: false' in plugin options. "
+                    f"Trace: {err}"
+                )
+                self.git_is_valid = False
+                use_git = False
+
+            # Checks if user is running builds on CI and raise appropriate warnings
+            if self.git_is_valid:
+                CiHandler(git_repo.git).raise_ci_warnings()
+        else:
+            self.git_is_valid = False
+            logger.debug(
+                "[rss-plugin] Git use is disabled. "
+                "Only page.meta (YAML frontmatter will be used). "
             )
-            self.git_is_valid = 0
-        except Exception as err:
-            logging.warning(f"[rss-plugin] Git issue: {err}")
-            self.git_is_valid = 0
 
-        # Checks if user is running builds on CI and raise appropriate warnings
-        CiHandler(git_repo.git).raise_ci_warnings()
+        # save git enable/disable status
+        self.use_git = use_git
 
     def build_url(self, base_url: str, path: str, args_dict: dict = None) -> str:
         """Build URL using base URL, cumulating existing and passed path, \
         then adding URL arguments.
 
         :param base_url: base URL with existing path to use
         :type base_url: str
@@ -131,35 +158,56 @@
         :return: tuple of timestamps (creation date, last commit date)
         :rtype: Tuple[datetime, datetime]
         """
         # empty vars
         dt_created = dt_updated = None
 
         # if enabled, try to retrieve dates from page metadata
-        if source_date_creation != "git" and in_page.meta.get(source_date_creation):
+        if not self.use_git or (
+            source_date_creation != "git" and in_page.meta.get(source_date_creation)
+        ):
             dt_created = self.get_date_from_meta(
                 date_metatag_value=in_page.meta.get(source_date_creation),
                 meta_datetime_format=meta_datetime_format,
                 meta_datetime_timezone=meta_default_timezone,
                 meta_default_time=meta_default_time,
             )
             if isinstance(dt_created, str):
-                logger.error(f"Creation date is a string: {dt_created}")
-                dt_created = None
+                logger.info(
+                    f"[rss-plugin] Creation date of {in_page.file.abs_src_path} is an "
+                    f"a character string: {dt_created} ({type(dt_created)})"
+                )
+
+            elif dt_created is None:
+                logger.info(
+                    f"[rss-plugin] Creation date of {in_page.file.abs_src_path} has not "
+                    "been recognized."
+                )
 
-        if source_date_update != "git" and in_page.meta.get(source_date_update):
+        if not self.use_git or (
+            source_date_update != "git" and in_page.meta.get(source_date_update)
+        ):
             dt_updated = self.get_date_from_meta(
                 date_metatag_value=in_page.meta.get(source_date_update),
                 meta_datetime_format=meta_datetime_format,
                 meta_datetime_timezone=meta_default_timezone,
                 meta_default_time=meta_default_time,
             )
+
             if isinstance(dt_updated, str):
-                logger.error(f"Update date is a string: {dt_updated}")
-                dt_updated = None
+                logger.info(
+                    f"[rss-plugin] Update date of {in_page.file.abs_src_path} is an "
+                    f"a character string: {dt_updated} ({type(dt_updated)})"
+                )
+
+            elif dt_updated is None:
+                logger.info(
+                    f"[rss-plugin] Update date of {in_page.file.abs_src_path} is an "
+                    f"unrecognized type: {dt_updated} ({type(dt_updated)})"
+                )
 
         # explore git log
         if self.git_is_valid:
             try:
                 # only if dates have not been retrieved from page meta
                 if not dt_created:
                     dt_created = self.repo.log(
@@ -176,20 +224,22 @@
                         date="short",
                         format="%at",
                     )
             except GitCommandError as err:
                 logging.warning(
                     f"[rss-plugin] Unable to read git logs of '{in_page.file.abs_src_path}'. "
                     "Is git log readable? Falling back to build date. "
+                    "To disable this warning, set 'use_git: false' in plugin options. "
                     f"Trace: {err}"
                 )
             except GitCommandNotFound as err:
                 logging.error(
                     "[rss-plugin] Unable to perform command 'git log'. Is git installed? "
-                    " Falling back to build date. "
+                    "Falling back to build date. "
+                    "To disable this warning, set 'use_git: false' in plugin options. "
                     f"Trace: {err}"
                 )
                 self.git_is_valid = 0
             # convert timestamps into datetimes
             if isinstance(dt_created, (str, float, int)) and dt_created:
                 dt_created = set_datetime_zoneinfo(
                     datetime.fromtimestamp(float(dt_created)), meta_default_timezone
@@ -330,19 +380,30 @@
             elif isinstance(date_metatag_value, (date, datetime)):
                 if isinstance(meta_default_time, datetime):
                     time_to_add = meta_default_time.time()
                 else:
                     time_to_add = datetime.min.time()
                 out_date = datetime.combine(date_metatag_value, time_to_add)
             else:
-                return "[rss-plugin] Incompatible date type."
+                logger.debug(
+                    f"[rss-plugin] Incompatible date type: {type(date_metatag_value)}"
+                )
+                return out_date
         except ValueError as err:
-            return f"[rss-plugin] Incompatible date found. Trace: {err}"
+            logger.error(
+                f"[rss-plugin] Incompatible date found: {date_metatag_value=} "
+                f"{type(date_metatag_value)}. Trace: {err}"
+            )
+            return out_date
         except Exception as err:
-            return f"[rss-plugin] Unable to retrieve creation date. Trace: {err}"
+            logger.error(
+                f"[rss-plugin] Unable to retrieve creation date: {date_metatag_value=} "
+                f"{type(date_metatag_value)}. Trace: {err}"
+            )
+            return out_date
 
         if not out_date.tzinfo:
             out_date = set_datetime_zoneinfo(out_date, meta_datetime_timezone)
 
         return out_date
 
     def get_description_or_abstract(
```

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/PKG-INFO` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rss-plugin
-Version: 1.7.0
+Version: 1.8.0
 Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
 Author: Julien Moura
 Author-email: dev@ingeoveritas.com
 License: MIT
 Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
 Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
 Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
```

### Comparing `mkdocs-rss-plugin-1.7.0/mkdocs_rss_plugin.egg-info/SOURCES.txt` & `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 mkdocs_rss_plugin.egg-info/entry_points.txt
 mkdocs_rss_plugin.egg-info/requires.txt
 mkdocs_rss_plugin.egg-info/top_level.txt
 mkdocs_rss_plugin/git_manager/__init__.py
 mkdocs_rss_plugin/git_manager/ci.py
 mkdocs_rss_plugin/templates/rss.xml.jinja2
 tests/test_build.py
+tests/test_build_no_git.py
 tests/test_config.py
 tests/test_rss_util.py
 tests/test_timezoner.py
```

### Comparing `mkdocs-rss-plugin-1.7.0/setup.cfg` & `mkdocs-rss-plugin-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/setup.py` & `mkdocs-rss-plugin-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/tests/test_build.py` & `mkdocs-rss-plugin-1.8.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/tests/test_config.py` & `mkdocs-rss-plugin-1.8.0/tests/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             "enabled": True,
             "feed_ttl": 1440,
             "image": None,
             "length": 20,
             "pretty_print": False,
             "match_path": ".*",
             "url_parameters": None,
+            "use_git": True,
         }
 
         # load
         plugin = GitRssPlugin()
         errors, warnings = plugin.load_config({})
         self.assertEqual(plugin.config, expected)
         self.assertEqual(errors, [])
@@ -88,29 +89,32 @@
             "enabled": True,
             "feed_ttl": 1440,
             "image": self.feed_image,
             "length": 20,
             "pretty_print": False,
             "match_path": ".*",
             "url_parameters": None,
+            "use_git": True,
         }
 
         # custom config
         custom_cfg = {"image": self.feed_image}
 
         # load
         plugin = GitRssPlugin()
         errors, warnings = plugin.load_config(custom_cfg)
         self.assertEqual(plugin.config, expected)
         self.assertEqual(errors, [])
         self.assertEqual(warnings, [])
 
     def test_plugin_config_through_mkdocs(self):
-        plg_cfg = self.get_plugin_config_from_mkdocs(Path("mkdocs.yml"), "rss")
-        self.assertIsInstance(plg_cfg, Config)
+        for config_filepath in self.config_files:
+            plg_cfg = self.get_plugin_config_from_mkdocs(config_filepath, "rss")
+            print(config_filepath)
+            self.assertIsInstance(plg_cfg, Config)
 
 
 # ##############################################################################
 # ##### Stand alone program ########
 # ##################################
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mkdocs-rss-plugin-1.7.0/tests/test_rss_util.py` & `mkdocs-rss-plugin-1.8.0/tests/test_rss_util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.7.0/tests/test_timezoner.py` & `mkdocs-rss-plugin-1.8.0/tests/test_timezoner.py`

 * *Files identical despite different names*

