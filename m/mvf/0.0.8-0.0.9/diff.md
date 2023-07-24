# Comparing `tmp/mvf-0.0.8.tar.gz` & `tmp/mvf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.8.tar", last modified: Mon Jul 10 16:19:35 2023, max compression
+gzip compressed data, was "mvf-0.0.9.tar", last modified: Thu Jul 20 10:30:34 2023, max compression
```

## Comparing `mvf-0.0.8.tar` & `mvf-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.072981 mvf-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-10 16:19:31.000000 mvf-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3714 2023-07-10 16:19:35.072981 mvf-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3144 2023-07-10 16:19:31.000000 mvf-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.066981 mvf-0.0.8/mvf/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.068981 mvf-0.0.8/mvf/cli/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.068981 mvf-0.0.8/mvf/dag/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/dag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/dag/builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.068981 mvf-0.0.8/mvf/integration/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.069981 mvf-0.0.8/mvf/integration/config/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2862 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/config/validate_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1993 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/mvf_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.070981 mvf-0.0.8/mvf/integration/process/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/preprocess_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/integration/process/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.072981 mvf-0.0.8/mvf/process/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/fit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/predict_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/split_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1379 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/validate.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/process/validate_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.072981 mvf-0.0.8/mvf/template/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-10 16:19:31.000000 mvf-0.0.8/mvf/template/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:19:35.067981 mvf-0.0.8/mvf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3714 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-10 16:19:35.000000 mvf-0.0.8/mvf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 16:19:35.072981 mvf-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-07-10 16:19:31.000000 mvf-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.282232 mvf-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-20 10:30:30.000000 mvf-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-20 10:30:34.281232 mvf-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3144 2023-07-20 10:30:30.000000 mvf-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.273232 mvf-0.0.9/mvf/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.275232 mvf-0.0.9/mvf/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5434 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.275232 mvf-0.0.9/mvf/dag/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/dag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12072 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/dag/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.276232 mvf-0.0.9/mvf/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.277232 mvf-0.0.9/mvf/integration/config/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/config/validate_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/mvf_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.279232 mvf-0.0.9/mvf/integration/process/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/preprocess_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/integration/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.281232 mvf-0.0.9/mvf/process/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/fit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/predict_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/split_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/process/validate_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.281232 mvf-0.0.9/mvf/template/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-20 10:30:30.000000 mvf-0.0.9/mvf/template/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:30:34.274232 mvf-0.0.9/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-20 10:30:34.000000 mvf-0.0.9/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 10:30:34.282232 mvf-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-07-20 10:30:30.000000 mvf-0.0.9/setup.py
```

### Comparing `mvf-0.0.8/LICENSE` & `mvf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/PKG-INFO` & `mvf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.8/README.md` & `mvf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/cli/cli.py` & `mvf-0.0.9/mvf/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,23 +15,76 @@
 
     See the documentation: 
 
         https://tomkimcta.gitlab.io/model-validation-framework
     '''
 )
 def mvf():
-    # '''
-    # CLI entry point.
-    # '''
-    # add working dir to PYTHONPATH to allow import of local modules
+    '''
+    CLI entry point.
+    '''
+    # Add working directory to PYTHONPATH to allow import of local modules
     sys.path.append(os.getcwd())
 
 
 @click.command(
     help='''
+        Try out an example project.
+    '''
+)
+@click.option(
+    '--list',
+    '-l',
+    is_flag=True,
+    default=False,
+    help='List the available projects.'
+)
+@click.option(
+    '--name',
+    '-n',
+    default=None,
+    help='Name of project to download.'
+)
+@click.option(
+    '--output',
+    '-o',
+    default=None,
+    help='Target directory.'
+)
+def examples(list, name, output):
+    # Use this list to manage which examples to expose
+    examples_list = [
+        'feature_scaling',
+        'py_preprocess_train_test',
+        'r_preprocess_kfold'
+    ]
+    if list:
+        # List the examples in the console
+        click.echo('The available examples are\n')
+        for example_name in examples_list:
+            click.echo(f'    {example_name}')
+        click.echo('\nDownload them using `mvf examples -n name_of_project')
+    elif name is None:
+        # Print the help text
+        ctx = click.get_current_context()
+        click.echo(ctx.get_help())
+    else:
+        # Try download the example called name
+        if name in examples_list:
+            click.echo(f'Downloading {name} project...')
+            # Download the example
+            output_dir = output if output is not None else name
+            utils.download_example(name, output_dir)
+        else:
+            click.echo(
+                f'There is no project named {name}. Check the available projects with\n\n  mvf examples -l\n')
+
+
+@click.command(
+    help='''
         Utility for initialising an MVF project. Generates an MVF
         configuration file. Default use will initialise the MVF
         project in the current working directory.
     '''
 )
 @click.option(
     '--directory',
@@ -52,15 +105,16 @@
         else:
             pth = os.path.join(
                 os.getcwd(),
                 directory
             )
         # check if the path provided by the user is already a file
         if os.path.isfile(pth):
-            raise click.ClickException('A file already exists at the location provided!')
+            raise click.ClickException(
+                'A file already exists at the location provided!')
         click.echo(f'Initialising MVF project in {pth}')
     # get confirmation from user
     click.confirm(f'Do you want to continue?', abort=True)
     cfg_builder = ConfigBuilder(pth)
     cfg_builder.write()
 
 
@@ -89,15 +143,15 @@
     default=None,
     help='Force execution of a specific process by name.'
 )
 def run(force, output, process):
     # load project config
     config = utils.load_config(
         os.path.join(
-            os.getcwd(), 
+            os.getcwd(),
             'mvf_conf.yaml'
         )
     )
     # build dag from config
     click.echo('Building MVF project workflow...')
     dag_builder = DagBuilder(config, output_dir=output)
     dag_builder.build()
@@ -129,23 +183,24 @@
     default='output',
     help='Specify the output directory.'
 )
 def plot(output):
     # load project config
     config = utils.load_config(
         os.path.join(
-            os.getcwd(), 
+            os.getcwd(),
             'mvf_conf.yaml'
         )
     )
     # build dag from config
     dag_builder = DagBuilder(config, output_dir=output)
     dag_builder.build()
     click.echo('Plotting workflow...')
     # access the built dag and plot it
     dag_builder.dag.plot('project_workflow.html')
 
 
 # add commands to group
+mvf.add_command(examples)
 mvf.add_command(run)
 mvf.add_command(plot)
 mvf.add_command(init)
```

### Comparing `mvf-0.0.8/mvf/dag/builder.py` & `mvf-0.0.9/mvf/dag/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                         task_name
                     ),
                 ),
             }
         product['process_metadata'] = File(
             os.path.join(
                 self.output_dir,
-                'metadata',
+                '.metadata',
                 f'{task_name}.metadata'
             )
         )
         # define task
         fit_model = PythonCallable(
             source=process.fit_model.fit_model,
             product=product,
@@ -255,15 +255,15 @@
                         'data',
                         f'{task_name}.feather'
                     ),
                 ),
                 'process_metadata': File(
                     os.path.join(
                         self.output_dir,
-                        'metadata',
+                        '.metadata',
                         f'{task_name}.metadata'
                     )
                 )
             },
             dag=self.dag,
             name=task_name,
             params=params
```

### Comparing `mvf-0.0.8/mvf/integration/config/fit_model.py` & `mvf-0.0.9/mvf/integration/config/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/config/predict_model.py` & `mvf-0.0.9/mvf/integration/config/predict_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/config/split_data.py` & `mvf-0.0.9/mvf/integration/config/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/config/validate_model.py` & `mvf-0.0.9/mvf/integration/config/validate_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/mvf_config.py` & `mvf-0.0.9/mvf/integration/mvf_config.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/process/fit_model.py` & `mvf-0.0.9/mvf/integration/process/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/process/predict_model.py` & `mvf-0.0.9/mvf/integration/process/predict_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/integration/process/split_data.py` & `mvf-0.0.9/mvf/integration/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/fit_model.py` & `mvf-0.0.9/mvf/process/fit_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/predict_model.py` & `mvf-0.0.9/mvf/process/predict_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/split_data.py` & `mvf-0.0.9/mvf/process/split_data.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/utils.py` & `mvf-0.0.9/mvf/process/utils.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/validate.py` & `mvf-0.0.9/mvf/process/validate.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/process/validate_model.py` & `mvf-0.0.9/mvf/process/validate_model.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf/template/config.py` & `mvf-0.0.9/mvf/template/config.py`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/mvf.egg-info/PKG-INFO` & `mvf-0.0.9/mvf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package implementing a supervised learning model validation framework.
 Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
 License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
 Platform: UNKNOWN
```

### Comparing `mvf-0.0.8/mvf.egg-info/SOURCES.txt` & `mvf-0.0.9/mvf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvf-0.0.8/setup.py` & `mvf-0.0.9/setup.py`

 * *Files identical despite different names*

