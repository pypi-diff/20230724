# Comparing `tmp/mlpj-0.2.4.tar.gz` & `tmp/mlpj-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpj-0.2.4.tar", last modified: Thu Jul  6 21:32:33 2023, max compression
+gzip compressed data, was "mlpj-0.3.0.tar", last modified: Mon Jul 24 21:13:20 2023, max compression
```

## Comparing `mlpj-0.2.4.tar` & `mlpj-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.444157 mlpj-0.2.4/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.2.4/LICENSE
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-07-06 21:32:33.444157 mlpj-0.2.4/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      965 2023-04-24 11:56:12.000000 mlpj-0.2.4/README.md
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.440823 mlpj-0.2.4/mlpj/
--rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-07-06 21:29:27.000000 mlpj-0.2.4/mlpj/__init__.py
--rw-------   0 bruno     (1000) bruno     (1000)    31419 2023-04-28 07:04:13.000000 mlpj-0.2.4/mlpj/actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    12367 2023-04-27 19:54:42.000000 mlpj-0.2.4/mlpj/ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1276 2023-05-19 10:51:10.000000 mlpj-0.2.4/mlpj/numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    28584 2023-07-06 20:37:39.000000 mlpj-0.2.4/mlpj/pandas_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    29704 2023-04-26 12:54:56.000000 mlpj-0.2.4/mlpj/plot_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)     7792 2023-04-28 06:51:00.000000 mlpj-0.2.4/mlpj/project_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     9444 2023-07-06 21:19:33.000000 mlpj-0.2.4/mlpj/python_utils.py
--rw-------   0 bruno     (1000) bruno     (1000)    18778 2023-04-26 13:30:54.000000 mlpj-0.2.4/mlpj/result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.2.4/mlpj/result_template.html
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1882 2023-04-26 14:13:05.000000 mlpj-0.2.4/mlpj/timeseries_utils.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.440823 mlpj-0.2.4/mlpj.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1758 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      584 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-07-06 21:32:33.000000 mlpj-0.2.4/mlpj.egg-info/top_level.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-07-06 21:32:33.444157 mlpj-0.2.4/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1221 2023-07-06 21:29:38.000000 mlpj-0.2.4/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-06 21:32:33.444157 mlpj-0.2.4/test/
--rw-r--r--   0 bruno     (1000) bruno     (1000)    11486 2023-04-26 14:07:56.000000 mlpj-0.2.4/test/test_actions_looper.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     5570 2023-04-27 19:09:34.000000 mlpj-0.2.4/test/test_ml_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      499 2023-04-26 12:33:47.000000 mlpj-0.2.4/test/test_numpy_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)    17383 2023-07-06 21:05:17.000000 mlpj-0.2.4/test/test_pandas_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     4489 2023-07-06 21:25:45.000000 mlpj-0.2.4/test/test_python_utils.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3102 2023-04-26 14:00:27.000000 mlpj-0.2.4/test/test_result_display.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1564 2023-07-06 21:28:41.000000 mlpj-0.2.4/test/test_timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-24 21:13:20.528238 mlpj-0.3.0/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1069 2023-04-21 13:02:36.000000 mlpj-0.3.0/LICENSE
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3008 2023-07-24 21:13:20.528238 mlpj-0.3.0/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2215 2023-07-18 10:31:50.000000 mlpj-0.3.0/README.md
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-24 21:13:20.524905 mlpj-0.3.0/mlpj/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       72 2023-07-24 21:11:50.000000 mlpj-0.3.0/mlpj/__init__.py
+-rw-------   0 bruno     (1000) bruno     (1000)    31419 2023-04-28 07:04:13.000000 mlpj-0.3.0/mlpj/actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    12367 2023-04-27 19:54:42.000000 mlpj-0.3.0/mlpj/ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1276 2023-05-19 10:51:10.000000 mlpj-0.3.0/mlpj/numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    28584 2023-07-06 20:37:39.000000 mlpj-0.3.0/mlpj/pandas_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    29704 2023-04-26 12:54:56.000000 mlpj-0.3.0/mlpj/plot_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)     7792 2023-04-28 06:51:00.000000 mlpj-0.3.0/mlpj/project_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     9444 2023-07-06 21:19:33.000000 mlpj-0.3.0/mlpj/python_utils.py
+-rw-------   0 bruno     (1000) bruno     (1000)    19014 2023-07-18 19:00:58.000000 mlpj-0.3.0/mlpj/result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     2747 2023-04-21 21:22:44.000000 mlpj-0.3.0/mlpj/result_template.html
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1822 2023-07-18 09:58:51.000000 mlpj-0.3.0/mlpj/stats_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1882 2023-04-26 14:13:05.000000 mlpj-0.3.0/mlpj/timeseries_utils.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-24 21:13:20.524905 mlpj-0.3.0/mlpj.egg-info/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3008 2023-07-24 21:13:20.000000 mlpj-0.3.0/mlpj.egg-info/PKG-INFO
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      629 2023-07-24 21:13:20.000000 mlpj-0.3.0/mlpj.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2023-07-24 21:13:20.000000 mlpj-0.3.0/mlpj.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2023-07-24 21:13:20.000000 mlpj-0.3.0/mlpj.egg-info/requires.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)        5 2023-07-24 21:13:20.000000 mlpj-0.3.0/mlpj.egg-info/top_level.txt
+-rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2023-07-24 21:13:20.528238 mlpj-0.3.0/setup.cfg
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1221 2023-07-24 21:11:40.000000 mlpj-0.3.0/setup.py
+drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2023-07-24 21:13:20.528238 mlpj-0.3.0/test/
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    11486 2023-04-26 14:07:56.000000 mlpj-0.3.0/test/test_actions_looper.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     5570 2023-04-27 19:09:34.000000 mlpj-0.3.0/test/test_ml_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)      499 2023-04-26 12:33:47.000000 mlpj-0.3.0/test/test_numpy_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)    17383 2023-07-06 21:05:17.000000 mlpj-0.3.0/test/test_pandas_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     4489 2023-07-06 21:25:45.000000 mlpj-0.3.0/test/test_python_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     3102 2023-04-26 14:00:27.000000 mlpj-0.3.0/test/test_result_display.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1040 2023-07-18 10:19:40.000000 mlpj-0.3.0/test/test_stats_utils.py
+-rw-r--r--   0 bruno     (1000) bruno     (1000)     1564 2023-07-06 21:28:41.000000 mlpj-0.3.0/test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2.4/LICENSE` & `mlpj-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/actions_looper.py` & `mlpj-0.3.0/mlpj/actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/ml_utils.py` & `mlpj-0.3.0/mlpj/ml_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/numpy_utils.py` & `mlpj-0.3.0/mlpj/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/pandas_utils.py` & `mlpj-0.3.0/mlpj/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/plot_utils.py` & `mlpj-0.3.0/mlpj/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/project_utils.py` & `mlpj-0.3.0/mlpj/project_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/python_utils.py` & `mlpj-0.3.0/mlpj/python_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/result_display.py` & `mlpj-0.3.0/mlpj/result_display.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import contextlib
 import jinja2
 import markupsafe
 import numpy as np
 import pandas as pd
 
+import matplotlib
 import matplotlib.pyplot as plt
 import lockfile
 
 from . import pandas_utils as pdu
 from . import python_utils as pu
 from . import plot_utils as pltu
 
@@ -84,39 +85,39 @@
             self.html_template = jinja2.Template(fin.read())
 
         db_path_dir = os.path.dirname(self.db_path)
         if not os.path.isdir(db_path_dir):
             os.makedirs(db_path_dir)
         self._init_db_if_necessary()
 
-        self.project_name = project_name        
+        self.project_name = project_name
         self.db_path = db_path
-        
+
         self.html_dir = html_dir
         pu.makedir_unless_exists(self.html_dir)
-        
+
         self.image_dir = image_dir
         pu.makedir_unless_exists(self.image_dir)
-        
+
         self.html_index_filename = 'index.html'
         self.default_figsize = default_figsize
         self.further_html_headers = further_html_headers
         self.refresh_how_long = refresh_how_long
         self.refresh_not_started_after = refresh_not_started_after
-    
+
     @contextlib.contextmanager
     def printer(self, key: str, suppl: bool = False, silence_stdout: bool = False,
               preformatted: bool = True) -> None:
         """Context manager to add the output printed in the context manager's
         block to the database under the given key and regenerate the
         corresponding HTML page.
 
         If there's an exception in the user block, the outputs printed so far
         are preserved.
-        
+
         Args:
             key (str): result key
             suppl (bool): If `True`, the database entry isn't replaced but
                 supplemented.
             silence_stdout (bool): If `True`, the content won't be printed but
                 only registered in the database.
             preformatted (bool): If `True`, wrap the content in HTML pre-tags.
@@ -135,15 +136,15 @@
 
     def print(self, key: str, content: str, suppl: bool = False,
             silence_stdout: bool = False, preformatted: bool = False) -> None:
         """Print and add the output to the database under the given key and
         regenerate the corresponding HTML page.
 
         Do nothing if the content is blank.
-        
+
         Args:
             key (str): result key
             content (str): to be printed
             suppl (bool): If `True`, the database entry isn't replaced but
                 supplemented.
             silence_stdout (bool): If `True`, the content won't be printed but
                 only registered in the database.
@@ -152,15 +153,15 @@
         if not content.strip():
             return
         if not silence_stdout:
             print('####', key, content)
         if preformatted:
             content = f"<pre>{content}</pre>"
         self.add_db_entry(key, content, suppl=suppl)
-        
+
     @contextlib.contextmanager
     def savefig(self, key: str, tool: str = 'matplotlib', with_printer: bool = True,
               with_libstyle: bool = True, figsize: Optional[Tuple[float, float]] = None,
               refresh_millisec: Optional[float] = None, tight_layout: bool = True,
               close_all: bool = True
     ) -> None:
         """Context manager to convert the plot created in the context manager's
@@ -168,21 +169,21 @@
 
         The PNG file will be saved under the key in the image directory and
         linked under the key in the corresponding HTML file and the database.
         Printed output will also be added if `with_printer=True`.
 
         If there's an exception in the user block, the old entry in the database
         and the HTML log will remain untouched.
-        
+
         Args:
             key (str): result key
             tool ('matplotlib' | 'system'):
                 For `matplotlib`, `plt.figure(1, figsize=figsize)` is called
                 initially and after executing the block converted to the PNG file.
-        
+
                 For `system`, the PNG filepath is available as a with-variable
                 for saving the plot under this path.
 
                 Further tools such as Bokeh and Plotly will be supported in the
                 future.
             with_printer (bool): If `True`, handle printed output like as in
                 the context manager `printer`.
@@ -190,102 +191,112 @@
                 plot style for the block, see `plot_utils.libstyle`.
             figsize (pair of floats): plot size
             refresh_millisec (float, optional): If a number is given, the HTML
                 page will start Javascript timer to refresh the image
                 periodically.
             tight_layout (bool): If `True`, call `plt.tight_layout()` in the end.
             close_all (bool): If `True`, call `plt.close('all')` in the end.
-            
+
             suppl (bool): If `True`, the database entry isn't replaced but
                 supplemented.
             silence_stdout (bool): If `True`, the content won't be printed but
                 only registered in the database.
             preformatted (bool): If `True`, wrap the content in HTML pre-tags.
         """
         key, plot_filepath = self._get_figure_path(key)
 
         # Make the image creation atomic by using a different filename and
         # moving the image in the end. See the {fu os.rename} call in the end.
         orig_plot_filepath = plot_filepath
         plot_filepath = re.sub(r'(\.[^.]+)$', r'.part\1', plot_filepath)
         description = ""
-        
+
         if figsize is None:
             figsize = self.default_figsize
         elif tool not in ('r', 'matplotlib'):
             raise NotImplementedError('figsize for system')
 
-        if tool == 'matplotlib':
+        old_backend = matplotlib.get_backend()
+
+        def prepare_matplotlib() -> None:
+            if old_backend != 'Agg':
+                matplotlib.use('Agg')
             plt.figure(1, figsize=figsize)
 
-        if with_printer:
-            out = io.StringIO()
-            branched = pu.BranchedOutputStreams((out, sys.stdout))
-            with pu.redirect_stdouterr(branched, branched):
-                with pdu.wide_display():
-                    try:
-                        if tool == 'matplotlib':
-                            if with_libstyle:
-                                with pltu.libstyle():
+        try:
+            if with_printer:
+                out = io.StringIO()
+                branched = pu.BranchedOutputStreams((out, sys.stdout))
+                with pu.redirect_stdouterr(branched, branched):
+                    with pdu.wide_display():
+                        try:
+                            if tool == 'matplotlib':
+                                prepare_matplotlib()
+                                if with_libstyle:
+                                    with pltu.libstyle():
+                                        yield plot_filepath
+                                else:
                                     yield plot_filepath
+                                if tight_layout:
+                                    self._tight_layout()
                             else:
                                 yield plot_filepath
-                            if tight_layout:
-                                self._tight_layout()
-                        else:
+                        finally:
+                            description += out.getvalue()
+            else:
+                #if tool == 'r':
+                #    self._plot_in_r(plot_filepath, pixelsize_args)
+                if tool == 'matplotlib':
+                    prepare_matplotlib()
+                    if with_libstyle:
+                        with pltu.libstyle():
                             yield plot_filepath
-                    finally:
-                        description += out.getvalue()
-        else:
-            #if tool == 'r':
-            #    self._plot_in_r(plot_filepath, pixelsize_args)
-            if tool == 'matplotlib':
-                if with_libstyle:
-                    with pltu.libstyle():
+                    else:
                         yield plot_filepath
+                    if tight_layout:
+                        self._tight_layout()
                 else:
                     yield plot_filepath
-                if tight_layout:
-                    self._tight_layout()
-            else:
-                yield plot_filepath
-        print(f"### new plot arrived: {key}")
-        if tool == 'matplotlib':
-            plt.savefig(plot_filepath)
+            print(f"### new plot arrived: {key}")
+
+        finally:
+            if tool == 'matplotlib':
+                plt.savefig(plot_filepath)
+                matplotlib.rcParams['backend'] = old_backend
 
         # atomic creation of the image (important for refresh)
         os.rename(plot_filepath, orig_plot_filepath)
         plot_filepath = orig_plot_filepath
-        
+
         path = pu.make_path_relative_to(plot_filepath, self.html_dir)
-        
+
         refresh_code = ""
         if refresh_millisec is not None:
             # {p how_long, end_time} are measured in seconds, not milliseconds
             end_time= int(time.time()) + self.refresh_not_started_after
-            
+
             refresh_code = f"""
             <script>
             start_image_refresh_timer(
               {self.refresh_how_long}, {end_time}, '{key}', '{path}',
               {refresh_millisec});
             </script>
             """
         contents = (f'<img src="{path}"><pre>{description}</pre>'
                     f'{refresh_code}')
-            
+
         self.add_db_entry(key, contents)
         if close_all:
             plt.close('all')
 
     def add_db_entry(self, key: str, contents: str, suppl: bool = False) -> None:
         """Add an entry to the Sqlite3 database file for the given key.
 
         After adding the entry, regenerate the result HTML page.
-        
+
         Args:
             key (str): result key
             contents (str): result string (HTML)
             suppl (bool): whether to supplement an existing entry
         """
         with lockfile.LockFile(self.db_path), \
                 pu.sqlite3_conn(self.db_path) as (db, cursor):
@@ -315,19 +326,19 @@
             link_text (str, optional): link text to display, defaults to given
                 filepath
         Returns:
             str: HTML link text
         """
         filepath = pu.make_path_relative_to(filepath, self.html_dir)
         return f'<a target="_blank" href="{filepath}">{link_text}</a>'
-            
+
     def get_keys(self) -> List[str]:
         """Get all distinct result keys from the database, reverse-ordered by
         timestamp.
-        
+
         Returns:
             list of str: list of result keys
         """
         with pu.sqlite3_conn(self.db_path) as (db, cursor):
             return pu.first_of_each_item(
                 cursor.execute('select distinct key from findings '
                                'order by timestamp desc'))
@@ -357,19 +368,19 @@
         if pu.isstring(regex):
             regex = re.compile(regex)
         selected_keys = []
         for key in self.get_keys():
             if regex.search(key):
                 selected_keys.append(key)
         self.del_keys(selected_keys)
-        
+
     def get_findings(self) -> List[Any]:
         """Get the contents of the findings table in the database,
         reverse-ordered by timestamp.
-        
+
         Returns:
             list of tuples: rows of the database table
         """
         with pu.sqlite3_conn(self.db_path) as (db, cursor):
             return list(cursor.execute(
                 'select * from findings order by timestamp desc'))
 
@@ -397,38 +408,38 @@
         all_entries = {}
         # The subquery is necessary for the reverse ordering by timestamp within
         # the groups defined by the keys.
         if descending:
             desc_part = 'desc'
         else:
             desc_part = ''
-            
+
         for key, contents, _ in cursor.execute(f"""
             select key, group_concat(contents, "\n"), max(timestamp) as maxts from (
             select key, contents, timestamp from findings
             order by timestamp desc, ind)
             group by key order by maxts {desc_part}"""
         ):
             contents = re.sub(r'<img src="([^"]*)"',
                               r'<img data-src="\1" class="lazy"', contents)
-            
+
             key_parts = key.split(':', maxsplit=1)
             if len(key_parts) == 1:
                 proper_key = key
                 html_filename = self.html_index_filename
             else:
                 html_filename, proper_key = key_parts
                 html_filename += '.html'
 
             html_filepath = os.path.join(self.html_dir, html_filename)
             existing_entries = all_entries.get(html_filepath, [])
-            
+
             existing_entries.append((proper_key, contents))
             all_entries[html_filepath] = existing_entries
-            
+
         for html_filepath, entries in all_entries.items():
             entries = [
                 (key, markupsafe.Markup(value)) for key, value in entries]
             with pu.open_overwriting_safely(html_filepath, 'w') as fout:
                 fout.write(
                     self.html_template.render(
                         display=self, entries=entries,
@@ -444,15 +455,15 @@
         Args:
             filename_stem (str): filename without directory or extension
         Returns:
             corresponding image filepath
         """
         filename = filename_stem + '.png'
         return os.path.join(self.image_dir, filename)
-        
+
     def _get_figure_path(self, key: str) -> str:
         """Check whether the key is valid and determine the filepath for a plot
         file.
 
         Args:
             key (str): result key
         Returns:
```

### Comparing `mlpj-0.2.4/mlpj/result_template.html` & `mlpj-0.3.0/mlpj/result_template.html`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj/timeseries_utils.py` & `mlpj-0.3.0/mlpj/timeseries_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/mlpj.egg-info/SOURCES.txt` & `mlpj-0.3.0/mlpj.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 mlpj/numpy_utils.py
 mlpj/pandas_utils.py
 mlpj/plot_utils.py
 mlpj/project_utils.py
 mlpj/python_utils.py
 mlpj/result_display.py
 mlpj/result_template.html
+mlpj/stats_utils.py
 mlpj/timeseries_utils.py
 mlpj.egg-info/PKG-INFO
 mlpj.egg-info/SOURCES.txt
 mlpj.egg-info/dependency_links.txt
 mlpj.egg-info/requires.txt
 mlpj.egg-info/top_level.txt
 test/test_actions_looper.py
 test/test_ml_utils.py
 test/test_numpy_utils.py
 test/test_pandas_utils.py
 test/test_python_utils.py
 test/test_result_display.py
+test/test_stats_utils.py
 test/test_timeseries_utils.py
```

### Comparing `mlpj-0.2.4/setup.py` & `mlpj-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 github_url = 'https://github.com/bdanielby/mlpj'
 
 setup(
     name='mlpj',
-    version='0.2.4',
+    version='0.3.0',
     description='Tools for machine learning projects',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url=github_url,
     author='Bruno Daniel',
     license='MIT',
     packages=['mlpj'],
```

### Comparing `mlpj-0.2.4/test/test_actions_looper.py` & `mlpj-0.3.0/test/test_actions_looper.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/test/test_ml_utils.py` & `mlpj-0.3.0/test/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/test/test_pandas_utils.py` & `mlpj-0.3.0/test/test_pandas_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/test/test_python_utils.py` & `mlpj-0.3.0/test/test_python_utils.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/test/test_result_display.py` & `mlpj-0.3.0/test/test_result_display.py`

 * *Files identical despite different names*

### Comparing `mlpj-0.2.4/test/test_timeseries_utils.py` & `mlpj-0.3.0/test/test_timeseries_utils.py`

 * *Files identical despite different names*

