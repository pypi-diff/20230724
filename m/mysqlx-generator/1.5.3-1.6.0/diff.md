# Comparing `tmp/mysqlx-generator-1.5.3.tar.gz` & `tmp/mysqlx-generator-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.5.3.tar", last modified: Mon Jul 17 15:11:01 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.6.0.tar", last modified: Mon Jul 24 07:29:34 2023, max compression
```

## Comparing `mysqlx-generator-1.5.3.tar` & `mysqlx-generator-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx/
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.3/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.3/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-generator-1.5.3/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2825 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2825 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2354 2023-07-17 15:10:48.000000 mysqlx-generator-1.5.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-17 15:11:01.000000 mysqlx-generator-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-07-17 15:10:55.000000 mysqlx-generator-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx/
+-rw-rw-rw-   0        0        0     6180 2023-07-24 06:29:00.000000 mysqlx-generator-1.6.0/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.0/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0      125 2023-07-24 01:06:19.000000 mysqlx-generator-1.6.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2826 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2826 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:29:34.000000 mysqlx-generator-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-07-24 07:17:52.000000 mysqlx-generator-1.6.0/setup.py
```

### Comparing `mysqlx-generator-1.5.3/mysqlx/generator.py` & `mysqlx-generator-1.6.0/mysqlx/generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
-from mysqlx import db
-from jinja2 import FileSystemLoader, Environment
+from sqlbatis import db, Engin
 from typing import Union, Iterable
+from jinja2 import FileSystemLoader, Environment
+from sqlbatis.constant import KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
 
 COMMON_COLS = ['create_by', 'create_time']
-ATTRIBUTES = {'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}
+ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
 
 
 class Generator:
     comma1 = ','
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
      WHERE table_schema = (SELECT DATABASE()) AND table_name = ? 
     '''
 
-    def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, use_unicode=True, pool_size=1, show_sql=False,
-            **kwargs):
-        db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
+    def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True, **kwargs):
+        db.init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.MYSQL, pool_size=pool_size, show_sql=show_sql, \
+                   use_unicode=use_unicode, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
         self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
@@ -43,41 +44,46 @@
             # 去重
             base_columns = list(set(columns))
             # 保持原有顺序
             base_columns.sort(key=columns.index)
         else:
             base_columns = columns
 
+        # 设置属性名
+        prefix = '__attribute_name'
+        for item in [KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY]:
+            kwargs[prefix + item] = item
+
         if isinstance(tables, str):
             if self.comma1 in tables:
                 tables = tables.split(self.comma1)
             elif self.comma2 in tables:
                 tables = tables.split(self.comma2)
             else:
                 only_one_table = True
                 metas = [self._get_table_meta(tables, base_columns)]
 
         if not only_one_table:
             if not isinstance(tables, set):
                 tables = set(tables)
             metas = [self._get_table_meta(table.strip(), base_columns) for table in tables]
 
-        no_pk_tables = [meta for meta in metas if isinstance(meta, str)]
-        if len(no_pk_tables) > 0:
-            print("There isn't primary key in the tables %s, it will not generate model class." % no_pk_tables)
+        no_key_tables = [meta for meta in metas if isinstance(meta, str)]
+        if len(no_key_tables) > 0:
+            print("There isn't primary key in the tables %s, it will not generate model class." % no_key_tables)
 
         metas = [meta for meta in metas if isinstance(meta, dict)]
         if len(metas) > 0:
             cols = [col for mata in metas for col in mata['super_columns']]
             col_dict = {col['COLUMN_NAME']: col for col in cols}
 
             def get_type(col):
                 if col in col_dict:
                     return col_dict[col]['DATA_TYPE']
-                elif col == kwargs.get('__pk__') or col == kwargs.get('__update_by__') or col == kwargs.get('__del_flag__'):
+                elif col == kwargs.get(KEY) or col == kwargs.get(UPDATE_BY) or col == kwargs.get(DEL_FLAG):
                     return 'int'
                 elif col == kwargs.get('__update_time__'):
                     return 'datetime'
                 elif col.endswith("_time"):
                     return 'datetime'
                 elif col.endswith("_date"):
                     return 'date'
@@ -99,30 +105,30 @@
             elif col_type in ('char', 'varchar', 'text'):
                 return 'str'
             elif col_type in ('date', 'datetime'):
                 return col_type
             else:
                 return 'None'
 
-        pk = None
+        key = None
         super_columns = []
         columns = db.do_query(self.sql, table)
         for col in columns:
             if col['COLUMN_KEY'] == 'PRI':
-                pk = col['COLUMN_NAME']
+                key = col['COLUMN_NAME']
             if col['COLUMN_NAME'] in base_columns:
                 super_columns.append(col)
             col['DATA_TYPE'] = convert_type(col['DATA_TYPE'])
 
-        if pk is None:
+        if key is None:
             return table
 
         class_name = self._get_class_name(table)
         return {
-            'pk': pk,
+            'key': key,
             'table': table,
             'class_name': class_name,
             'columns': columns,
             'self_columns': [col for col in columns if col['COLUMN_NAME'] not in base_columns],
             'super_columns': super_columns
         }
```

### Comparing `mysqlx-generator-1.5.3/mysqlx/generator.tpl` & `mysqlx-generator-1.6.0/mysqlx/generator.tpl`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from decimal import Decimal
 from datetime import date, datetime
-from mysqlx.orm import Model, PkStrategy
+from mysqlx.orm import Model, KeyStrategy
 
 
 class BaseModel(Model):
-    __pk__ = '{{__pk__}}'
-    __del_flag__ = '{{__del_flag__}}'
-    __update_by__ = '{{__update_by__}}'
-    __update_time__ = '{{__update_time__}}'
-    __pk_strategy__ = PkStrategy.DB_AUTO_INCREMENT
+    {{__attribute_name__key__}} = '{{__key__}}'
+    {{__attribute_name__del_flag__}} = '{{__del_flag__}}'
+    {{__attribute_name__update_by__}} = '{{__update_by__}}'
+    {{__attribute_name__update_time__}} = '{{__update_time__}}'
+    {{__attribute_name__key_strategy__}} = KeyStrategy.DB_AUTO_INCREMENT
 
     def __init__(self,{% for item in base_columns %}{% if loop.last %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %}{% else %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %},{% endif %}{% endfor %}): {% for item in base_columns %}
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% for meta in metas %}
-class {{meta.class_name}}(BaseModel):{% if meta.pk != __pk__ %}
-    __pk__ = '{{meta.pk}}'{% endif %}
-    __table__ = '{{meta.table}}'
+class {{meta.class_name}}(BaseModel):{% if meta.key != __key__ %}
+    {{__attribute_name__key__}} = '{{meta.key}}'{% endif %}
+    {{__attribute_name__table__}} = '{{meta.table}}'
 
     def __init__(self,{% for item in meta.columns %}{% if loop.last %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %}{% else %}{% if item.DATA_TYPE=='None' %} {{item.COLUMN_NAME}}=None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% endif %},{% endif %}{% endfor %}):
         super().__init__({% for item in meta.super_columns %}{% if loop.first %}{{item.COLUMN_NAME}}={{item.COLUMN_NAME}}{% else %}, {{item.COLUMN_NAME}}={{item.COLUMN_NAME}}{% endif %}{% endfor %}) {% for item in meta.self_columns %}
         self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
 
 {% endfor %}
```

### Comparing `mysqlx-generator-1.5.3/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.6.0/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.3
-Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
+Version: 1.6.0
+Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -38,23 +38,23 @@
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
 
    from decimal import Decimal
    from datetime import date, datetime
-   from mysqlx.orm import Model, PkStrategy
+   from mysqlx.orm import Model, KeyStrategy
 
 
    class BaseModel(Model):
-       __pk__ = 'id'
+       __key__ = 'id'
        __del_flag__ = 'del_flag'
        __update_by__ = 'update_by'
        __update_time__ = 'update_time'
-       __pk_strategy__ = PkStrategy.DB_AUTO_INCREMENT
+       __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
 
        def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
                del_flag: int = None):
            self.id = id
            self.create_by = create_by
            self.create_time = create_time
            self.update_by = update_by
```

### Comparing `mysqlx-generator-1.5.3/PKG-INFO` & `mysqlx-generator-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.3
-Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
+Version: 1.6.0
+Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -38,23 +38,23 @@
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
 
    from decimal import Decimal
    from datetime import date, datetime
-   from mysqlx.orm import Model, PkStrategy
+   from mysqlx.orm import Model, KeyStrategy
 
 
    class BaseModel(Model):
-       __pk__ = 'id'
+       __key__ = 'id'
        __del_flag__ = 'del_flag'
        __update_by__ = 'update_by'
        __update_time__ = 'update_time'
-       __pk_strategy__ = PkStrategy.DB_AUTO_INCREMENT
+       __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
 
        def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
                del_flag: int = None):
            self.id = id
            self.create_by = create_by
            self.create_time = create_time
            self.update_by = update_by
```

### Comparing `mysqlx-generator-1.5.3/README.rst` & `mysqlx-generator-1.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,23 @@
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
 
    from decimal import Decimal
    from datetime import date, datetime
-   from mysqlx.orm import Model, PkStrategy
+   from mysqlx.orm import Model, KeyStrategy
 
 
    class BaseModel(Model):
-       __pk__ = 'id'
+       __key__ = 'id'
        __del_flag__ = 'del_flag'
        __update_by__ = 'update_by'
        __update_time__ = 'update_time'
-       __pk_strategy__ = PkStrategy.DB_AUTO_INCREMENT
+       __key_strategy__ = KeyStrategy.DB_AUTO_INCREMENT
 
        def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_by: int = None, update_time: datetime = None,
                del_flag: int = None):
            self.id = id
            self.create_by = create_by
            self.create_time = create_time
            self.update_by = update_by
```

### Comparing `mysqlx-generator-1.5.3/setup.py` & `mysqlx-generator-1.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='mysqlx-generator',
     packages=['mysqlx'],
-    description="mysqlx-generator is a model code generator from db tables for MySqlx.",
+    description="mysqlx-generator is a model code generator from tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'mysqlx>=1.3.9',
+        'sqlx-exec>=1.1.5',
     ],
-    version='1.5.3',
+    version='1.6.0',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

