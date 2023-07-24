# Comparing `tmp/yplib-2.6.3.tar.gz` & `tmp/yplib-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.6.3.tar", last modified: Mon Jul 24 00:40:39 2023, max compression
+gzip compressed data, was "dist\yplib-2.6.4.tar", last modified: Mon Jul 24 02:06:02 2023, max compression
```

## Comparing `yplib-2.6.3.tar` & `yplib-2.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.280934 yplib-2.6.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-24 00:40:39.280435 yplib-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 00:40:39.281228 yplib-2.6.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-24 00:40:18.000000 yplib-2.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.277541 yplib-2.6.3/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.3/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.3/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    34070 2023-07-24 00:40:02.000000 yplib-2.6.3/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.3/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 00:40:39.279934 yplib-2.6.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 00:40:39.000000 yplib-2.6.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.874649 yplib-2.6.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-24 02:06:02.874649 yplib-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 02:06:02.875265 yplib-2.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-24 02:04:21.000000 yplib-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.864578 yplib-2.6.4/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.4/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.4/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    35649 2023-07-24 02:03:11.000000 yplib-2.6.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.874140 yplib-2.6.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.6.3/LICENSE` & `yplib-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/setup.py` & `yplib-2.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.6.3",
+  version="2.6.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.6.3/yplib/__init__.py` & `yplib-2.6.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/chart.py` & `yplib-2.6.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/chart_html.py` & `yplib-2.6.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/db.py` & `yplib-2.6.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/file.py` & `yplib-2.6.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/http_util.py` & `yplib-2.6.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/index.py` & `yplib-2.6.4/yplib/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 import platform
 from datetime import datetime
 from datetime import timedelta
 
 import xlrd
 import xlwt
+import openpyxl
 
 
 # 是否是 windows 系统
 def is_win():
     return platform.system().lower() == 'windows'
 
 
@@ -513,48 +514,85 @@
                 list_all.append(o)
     if len(list_all) > 0 and list_index[0] is not None:
         list_index[0] = list_all
     # 是否是单 list 类型的数据
     list_only_one = False
     if list_index[0] is not None and len(list_index[0]) == 1:
         list_only_one = True
-    book = xlrd.open_workbook(file_name)  # 打开一个excel
-    sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
-    for i in range(sheet.nrows):  # 0 1 2 3 4 5
-        rows = sheet.row_values(i)
-        row_data = []
-        for j in range(len(rows)):
-            cell_data = str(rows[j]).strip()
-            is_date = False
-            is_datetime = False
-            # 日期格式的列
-            if list_index[1] is not None and j + 1 in list_index[1]:
-                cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
-                is_date = True
-                row_data.append(cell_data)
-                if list_only_one:
-                    row_data = cell_data
-            # 日期时间格式的列
-            if not is_date and list_index[2] is not None and j + 1 in list_index[2]:
-                cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
-                is_datetime = True
-                row_data.append(cell_data)
-                if list_only_one:
-                    row_data = cell_data
-            # 指定需要的列
-            if not is_date and not is_datetime:
-                if list_index[0] is None:
+    # 是 xls 格式
+    if file_name.endswith('.xls'):
+        book = xlrd.open_workbook(file_name)  # 打开一个excel
+        sheet = book.sheet_by_index(sheet_index - 1)  # 根据顺序获取sheet
+        for i in range(sheet.nrows):  # 0 1 2 3 4 5
+            rows = sheet.row_values(i)
+            row_data = []
+            for j in range(len(rows)):
+                cell_data = str(rows[j]).strip()
+                is_date = False
+                is_datetime = False
+                # 日期格式的列
+                if list_index[1] is not None and j + 1 in list_index[1]:
+                    cell_data = to_date(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                    is_date = True
                     row_data.append(cell_data)
-                else:
-                    # 指定需要的列
-                    if j + 1 in list_index[0]:
+                    if list_only_one:
+                        row_data = cell_data
+                # 日期时间格式的列
+                if not is_date and list_index[2] is not None and j + 1 in list_index[2]:
+                    cell_data = to_datetime(xlrd.xldate_as_datetime(to_int(rows[j]), 0))
+                    is_datetime = True
+                    row_data.append(cell_data)
+                    if list_only_one:
+                        row_data = cell_data
+                # 指定需要的列
+                if not is_date and not is_datetime:
+                    if list_index[0] is None:
                         row_data.append(cell_data)
-                        if list_only_one:
-                            row_data = cell_data
-        data_list.append(row_data)
+                    else:
+                        # 指定需要的列
+                        if j + 1 in list_index[0]:
+                            row_data.append(cell_data)
+                            if list_only_one:
+                                row_data = cell_data
+            data_list.append(row_data)
+    # 是 xlsx 格式
+    if file_name.endswith('.xlsx'):
+        wb = openpyxl.load_workbook(filename=file_name, read_only=True)
+        ws = wb[wb.sheetnames[sheet_index - 1]]
+        for rows in ws.rows:
+            row_data = []
+            for j in range(len(rows)):
+                cell_data = str(rows[j].value).strip()
+                is_date = False
+                is_datetime = False
+                # 日期格式的列
+                if list_index[1] is not None and j + 1 in list_index[1]:
+                    cell_data = to_date(cell_data)
+                    is_date = True
+                    row_data.append(cell_data)
+                    if list_only_one:
+                        row_data = cell_data
+                # 日期时间格式的列
+                if not is_date and list_index[2] is not None and j + 1 in list_index[2]:
+                    cell_data = to_datetime(cell_data)
+                    is_datetime = True
+                    row_data.append(cell_data)
+                    if list_only_one:
+                        row_data = cell_data
+                # 指定需要的列
+                if not is_date and not is_datetime:
+                    if list_index[0] is None:
+                        row_data.append(cell_data)
+                    else:
+                        # 指定需要的列
+                        if j + 1 in list_index[0]:
+                            row_data.append(cell_data)
+                            if list_only_one:
+                                row_data = cell_data
+            data_list.append(row_data)
     return data_list
 
 
 # 将一个文件中以空行作为分隔符,
 # 组成一个 list(list) 数据
 # 多行空行,自动合并到一行空行
 def to_list_from_txt_with_blank_line(file_name='a.txt'):
@@ -795,42 +833,35 @@
                 column_datetime=column_datetime)
     return str_join.join(d) if r_str else json.loads(str_join.join(d)) if r_json else d
 
 
 def to_excel(data_list, file_name=None, file_path='excel'):
     if file_name is None:
         file_name = 'excel'
-        sheet_name = 'Sheet1'
-    else:
-        sheet_name = file_name
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
-    # 2. 创建Excel工作薄
-    w_b = xlwt.Workbook()
-    # 3. 添加Excel工作表
-    sh = w_b.add_sheet(sheet_name)
-    # 4. 写入数据
-    # myStyle = xlwt.easyxf('font: name Times New Roman, color-index red, bold on')  # 数据格式
-    m = 0
+    # 实例化对象excel对象
+    excel_obj = openpyxl.Workbook()
+    # excel 内第一个sheet工作表
+    excel_obj_sheet = excel_obj[excel_obj.sheetnames[0]]
+    # 给单元格赋值
     for one_data in data_list:
-        n = 0
-        if isinstance(one_data, list):
+        s_list = []
+        if isinstance(one_data, list) or isinstance(one_data, set):
             for one in one_data:
-                # mySheet.write(n, m, one)  # 写入A3，数值等于1
                 if isinstance(one, dict) or isinstance(one, list):
                     s = json.dumps(one)
                 else:
                     s = str(one)
-                sh.write(m, n, s)  # 写入A3，数值等于1
-                n += 1
+                s_list.append(s)
+            excel_obj_sheet.append(s_list)
         else:
             if can_use_json(one_data):
                 s = json.dumps(one_data)
             else:
                 s = str(one_data)
-            sh.write(m, n, s)  # 写入A3，数值等于1
-        m += 1
-    # 5. 保存
-    # myWorkbook.save('5002200.xls')
-    w_b.save(file_path + '/' + get_file_name(file_name, '.xls'))
+            excel_obj_sheet.append([s])
+
+    # 文件保存
+    excel_obj.save(file_path + '/' + get_file_name(file_name, '.xlsx'))
```

### Comparing `yplib-2.6.3/yplib/mail.py` & `yplib-2.6.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/mail_html.py` & `yplib-2.6.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.3/yplib/markdown.py` & `yplib-2.6.4/yplib/markdown.py`

 * *Files identical despite different names*

