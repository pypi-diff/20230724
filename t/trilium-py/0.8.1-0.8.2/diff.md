# Comparing `tmp/trilium_py-0.8.1-py3-none-any.whl.zip` & `tmp/trilium_py-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29215 bytes, number of entries: 13
--rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
--rw-r--r--  2.0 unx    33110 b- defN 23-Jul-06 09:30 trilium_py/client.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
--rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
--rw-r--r--  2.0 unx     2066 b- defN 23-Jul-06 09:30 trilium_py/utils/note_util.py
--rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
--rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
--rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    12365 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1076 b- defN 23-Jul-07 06:10 trilium_py-0.8.1.dist-info/RECORD
-13 files, 94054 bytes uncompressed, 27411 bytes compressed:  70.9%
+Zip file size: 30291 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      141 b- defN 23-Jul-07 06:10 trilium_py/__init__.py
+-rw-r--r--  2.0 unx    38251 b- defN 23-Jul-24 06:37 trilium_py/client.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 06:10 trilium_py/utils/__init__.py
+-rw-r--r--  2.0 unx     9328 b- defN 23-Jul-24 06:37 trilium_py/utils/markdown_math.py
+-rw-r--r--  2.0 unx     2099 b- defN 23-Jul-24 06:37 trilium_py/utils/note_util.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Jul-24 06:37 trilium_py/utils/param_util.py
+-rw-r--r--  2.0 unx      208 b- defN 23-Jul-07 06:10 trilium_py/utils/time_util.py
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-24 06:37 trilium_py/utils/url_util.py
+-rwxrwx---  2.0 unx    35184 b- defN 23-Jul-24 06:50 trilium_py-0.8.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    12261 b- defN 23-Jul-24 06:50 trilium_py-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 06:50 trilium_py-0.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-24 06:50 trilium_py-0.8.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1076 b- defN 23-Jul-24 06:50 trilium_py-0.8.2.dist-info/RECORD
+13 files, 99818 bytes uncompressed, 28487 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.8.1.dist-info/LICENSE.txt
+Filename: trilium_py-0.8.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.8.1.dist-info/METADATA
+Filename: trilium_py-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.8.1.dist-info/WHEEL
+Filename: trilium_py-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.8.1.dist-info/top_level.txt
+Filename: trilium_py-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.8.1.dist-info/RECORD
+Filename: trilium_py-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -1,36 +1,48 @@
 import os
 import re
+import string
+import sys
 import urllib.parse
+from collections.abc import Mapping
+from typing import Optional, Union
 
 import magic
 import markdown2
 import requests
 from bs4 import BeautifulSoup
 from loguru import logger
 from natsort import natsort
 
-from .utils.markdown_math import sanitizeInput, reconstructMath
+from .utils.markdown_math import reconstructMath, sanitizeInput
 from .utils.note_util import beautify_content
-from .utils.param_util import format_query_string, clean_param
-from .utils.time_util import get_yesterday, get_today
+from .utils.param_util import clean_param, format_query_string
+from .utils.time_util import get_today, get_yesterday
 
 
 class ETAPI:
+    def __init__(self, server_url: str, token: Optional[str] = None):
+        if sys.version_info < (3, 9):
+            print(
+                (
+                    f'You are using Python {sys.version_info.major}.{sys.version_info.minor}'
+                    ', 3.9+ is required.'
+                ),
+                file=sys.stderr,
+            )
 
-    def __init__(self, server_url: str, token: str = None):
         self.server_url = server_url
-        self.token = token
+        self.token: str = token  # type: ignore
 
     def get_header(self) -> dict:
         return {
             'Authorization': self.token,
         }
 
-    def login(self, password: str) -> str:
+    def login(self, password: str) -> Optional[str]:
         """
         generate token with password
         """
         url = f'{self.server_url}/etapi/auth/login'
 
         data = {'password': password}
 
@@ -38,15 +50,15 @@
         if res.status_code == 201:
             self.token = res.json()['authToken']
             return self.token
         else:
             logger.info(res.json()['message'])
             return None
 
-    def logout(self, token_to_destroy: str = None) -> bool:
+    def logout(self, token_to_destroy: Optional[str] = None) -> bool:
         """
         destroy token
         """
 
         if not token_to_destroy:
             token_to_destroy = self.token
 
@@ -61,32 +73,29 @@
         if res.status_code == 204:
             logger.info('logout successfully')
             return True
         return False
 
     def app_info(self) -> dict:
         """
+        basic info about running Trilium version.
 
         :return:
         """
-        result = []
-
         url = f'{self.server_url}/etapi/app-info'
         res = requests.get(url, headers=self.get_header())
         return res.json()
 
     def search_note(self, search: str, **params) -> dict:
         """
 
         :param search:
         :param params:
         :return:
         """
-        result = []
-
         url = f'{self.server_url}/etapi/notes'
         params['search'] = search
         res = requests.get(url, params=format_query_string(params), headers=self.get_header())
         return res.json()
 
     def get_note(self, noteId: str) -> dict:
         """
@@ -96,20 +105,31 @@
         :param noteId:
         :return:
         """
         url = f'{self.server_url}/etapi/notes/{noteId}'
         res = requests.get(url, headers=self.get_header())
         return res.json()
 
-    def create_note(self, parentNoteId: str, title: str, type: str, mime: str = None, content=None,
-                    notePosition: int = None, prefix: str = None,
-                    isExpanded: str = None, noteId: str = None,
-                    branchId: str = None) -> dict:
+    def create_note(
+        self,
+        parentNoteId: str,
+        title: str,
+        type: str,
+        mime: Optional[str] = None,
+        content=None,
+        notePosition: Optional[int] = None,
+        prefix: Optional[str] = None,
+        isExpanded: Optional[str] = None,
+        noteId: Optional[str] = None,
+        branchId: Optional[str] = None,
+    ) -> dict:
         """
-        Actually it's create or update, if noteId already exists, the corresponding note will be updated
+        Actually it's create or update,
+        if noteId already exists, the corresponding note will be updated
+
         :param parentNoteId:
         :param title:
         :param type:
         :param mime:
         :param content:
         :param notePosition:
         :param prefix:
@@ -126,25 +146,34 @@
             "type": type,
             "mime": mime,
             "content": content,
             "notePosition": notePosition,
             "prefix": prefix,
             "isExpanded": isExpanded,
             "noteId": noteId,
-            "branchId": branchId
+            "branchId": branchId,
         }
         res = requests.post(url, json=clean_param(params), headers=self.get_header())
 
         return res.json()
 
-    def create_file_note(self, parentNoteId: str, title: str, file_path: str,
-                         type: str = 'file', mime: str = "application/octet-stream",
-                         content='<p></p>', notePosition: int = None, prefix: str = None,
-                         isExpanded: str = None, noteId: str = None,
-                         branchId: str = None):
+    def create_file_note(
+        self,
+        parentNoteId: str,
+        title: str,
+        file_path: str,
+        type: str = 'file',
+        mime: str = "application/octet-stream",
+        content='<p></p>',
+        notePosition: Optional[int] = None,
+        prefix: Optional[str] = None,
+        isExpanded: Optional[str] = None,
+        noteId: Optional[str] = None,
+        branchId: Optional[str] = None,
+    ):
         '''
         Upload ordinary file as a sub-note
 
         Create a note
         set file name attribute
         Update its content with raw file binary content
         :param parentNoteId:
@@ -169,46 +198,69 @@
             "type": type,
             "mime": mime,
             "content": content,
             "notePosition": notePosition,
             "prefix": prefix,
             "isExpanded": isExpanded,
             "noteId": noteId,
-            "branchId": branchId
+            "branchId": branchId,
         }
 
-        res_file = requests.post(url, json=clean_param(params),
-                                 headers={'content-type': 'application/json', 'Authorization': self.token, })
+        res_file = requests.post(
+            url,
+            json=clean_param(params),
+            headers={
+                'content-type': 'application/json',
+                'Authorization': self.token,
+            },
+        )
         res_file_json = res_file.json()
         new_noteId = res_file_json['note']['noteId']
 
         # set file name
         file_path_name = os.path.basename(file_path)
-        self.create_attribute(attributeId=None, noteId=new_noteId, type='label', name='originalFileName',
-                              value=file_path_name, isInheritable=False)
+        self.create_attribute(
+            attributeId=None,
+            noteId=new_noteId,
+            type='label',
+            name='originalFileName',
+            value=file_path_name,
+            isInheritable=False,
+        )
 
         # upload file, set note content
         url = f'{self.server_url}/etapi/notes/{new_noteId}/content'
         file_data = open(file_path, 'rb').read()
-        res = requests.put(url, data=file_data,
-                           headers={
-                               'content-type': 'application/octet-stream',
-                               'Content-Transfer-Encoding': 'binary',
-                               'Authorization': self.token,
-                           })
+        res = requests.put(
+            url,
+            data=file_data,
+            headers={
+                'content-type': 'application/octet-stream',
+                'Content-Transfer-Encoding': 'binary',
+                'Authorization': self.token,
+            },
+        )
         if res.status_code == 204:
             return res_file_json
         return
 
-    def create_image_note(self, parentNoteId: str, title: str, image_file: str, type: str = 'image', mime: str = None,
-                          content=None,
-                          notePosition: int = None, prefix: str = None,
-                          isExpanded: str = None, noteId: str = None,
-                          branchId: str = None):
-
+    def create_image_note(
+        self,
+        parentNoteId: str,
+        title: str,
+        image_file: str,
+        type: str = 'image',
+        mime: Optional[str] = None,
+        content=None,
+        notePosition: Optional[int] = None,
+        prefix: Optional[str] = None,
+        isExpanded: Optional[str] = None,
+        noteId: Optional[str] = None,
+        branchId: Optional[str] = None,
+    ):
         '''
         Upload image as a sub-note
 
         Create a note
         set file name attribute
         Update its content with image binary content
 
@@ -242,43 +294,64 @@
             "type": type,
             "mime": mime,
             "content": "image",
             "notePosition": notePosition,
             "prefix": prefix,
             "isExpanded": isExpanded,
             "noteId": noteId,
-            "branchId": branchId
+            "branchId": branchId,
         }
-        res_image = requests.post(url, json=clean_param(params),
-                                  headers={'content-type': 'application/json', 'Authorization': self.token, })
+        res_image = requests.post(
+            url,
+            json=clean_param(params),
+            headers={
+                'content-type': 'application/json',
+                'Authorization': self.token,
+            },
+        )
         res_image_json = res_image.json()
         new_noteId = res_image_json['note']['noteId']
 
         # set file name
         image_file_name = os.path.basename(image_file)
-        self.create_attribute(attributeId=None, noteId=new_noteId, type='label', name='originalFileName',
-                              value=image_file_name, isInheritable=False)
+        self.create_attribute(
+            attributeId=None,
+            noteId=new_noteId,
+            type='label',
+            name='originalFileName',
+            value=image_file_name,
+            isInheritable=False,
+        )
 
         # upload image, set note content
         url = f'{self.server_url}/etapi/notes/{new_noteId}/content'
         image_data = open(image_file, 'rb').read()
         # content-type here will affect the result
         # not working, encoding issue? automated force encoding to utf-8 and lost data
-        res = requests.put(url, data=image_data,
-                           # headers={'content-type': 'text/plain', 'Authorization': self.token, })
-                           headers={
-                               'content-type': 'application/octet-stream',
-                               'Content-Transfer-Encoding': 'binary',
-                               'Authorization': self.token,
-                           })
+        res = requests.put(
+            url,
+            data=image_data,
+            # headers={'content-type': 'text/plain', 'Authorization': self.token, })
+            headers={
+                'content-type': 'application/octet-stream',
+                'Content-Transfer-Encoding': 'binary',
+                'Authorization': self.token,
+            },
+        )
         if res.status_code == 204:
             return res_image_json
         return
 
-    def patch_note(self, noteId: str, title: str = None, type: str = None, mime: str = None) -> dict:
+    def patch_note(
+        self,
+        noteId: str,
+        title: Optional[str] = None,
+        type: Optional[str] = None,
+        mime: Optional[str] = None,
+    ) -> dict:
         url = f'{self.server_url}/etapi/notes/{noteId}'
         params = {
             "title": title,
             "type": type,
             "mime": mime,
         }
         res = requests.patch(url, json=clean_param(params), headers=self.get_header())
@@ -295,37 +368,48 @@
         url = f'{self.server_url}/etapi/notes/{noteId}/content'
         res = requests.get(url, headers=self.get_header())
         return res.content.decode('utf-8')
 
     def update_note_content(self, noteId: str, content: str) -> bool:
         """update note content"""
         url = f'{self.server_url}/etapi/notes/{noteId}/content'
-        res = requests.put(url, data=content.encode('utf-8'),
-                           headers={'content-type': 'text/plain', 'Authorization': self.token})
+        res = requests.put(
+            url,
+            data=content.encode('utf-8'),
+            headers={'content-type': 'text/plain', 'Authorization': self.token},
+        )
         if res.status_code == 204:
             return True
         return False
 
     def get_branch(self, branchId: str) -> dict:
         url = f'{self.server_url}/etapi/branches/{branchId}'
         res = requests.get(url, headers=self.get_header())
         return res.json()
 
-    def create_branch(self, branchId: str, noteId: str, parentNoteId: str, prefix: str, notePosition: int,
-                      isExpanded: bool, utcDateModified) -> dict:
+    def create_branch(
+        self,
+        branchId: str,
+        noteId: str,
+        parentNoteId: str,
+        prefix: str,
+        notePosition: int,
+        isExpanded: bool,
+        utcDateModified,
+    ) -> dict:
         # url = f'{self.server_url}/etapi/branches/{branchId}'
         url = f'{self.server_url}/etapi/branches/'
         params = {
             "branchId": branchId,
             "noteId": noteId,
             "parentNoteId": parentNoteId,
             "prefix": prefix,
             "notePosition": notePosition,
             "isExpanded": isExpanded,
-            "utcDateModified": utcDateModified
+            "utcDateModified": utcDateModified,
         }
         res = requests.post(url, json=clean_param(params), headers=self.get_header())
         return res.json()
 
     def patch_branch(self, branchId: str, notePosition: int, prefix: str, isExpanded: bool) -> dict:
         url = f'{self.server_url}/etapi/branches/{branchId}'
         params = {
@@ -344,16 +428,23 @@
         return False
 
     def get_attribute(self, attributeId: str) -> dict:
         url = f'{self.server_url}/etapi/attributes/{attributeId}'
         res = requests.get(url, headers=self.get_header())
         return res.json()
 
-    def create_attribute(self, attributeId: str, noteId: str, type: str, name: str, value: str,
-                         isInheritable: bool) -> dict:
+    def create_attribute(
+        self,
+        attributeId: Optional[str],
+        noteId: str,
+        type: str,
+        name: str,
+        value: str,
+        isInheritable: bool,
+    ) -> dict:
         url = f'{self.server_url}/etapi/attributes/'
         params = {
             "attributeId": attributeId,
             "noteId": noteId,
             "type": type,
             "name": name,
             "value": value,
@@ -464,82 +555,98 @@
 
     def set_day_note(self, date, content):
         url = f'{self.server_url}/etapi/calendar/days/{date}'
         res = requests.get(url, headers=self.get_header())
         noteId = res.json()['noteId']
         return self.update_note_content(noteId, content)
 
-    def get_todo(self):
-        """get today's todo list"""
+    def get_todo(self) -> list[list[Union[bool, str]]]:
+        """get today's todo list.
 
+        :return: list of todo items, each item is a list of [status, description]
+        """
         content = self.get_today_note_content()
         soup = BeautifulSoup(content, 'html.parser')
-        todo_labels = soup.find_all("label", {"class": "todo-list__label"})
-        todo_list = []
-        for x in todo_labels:
-            description = x.text.strip()
-            checked = x.find("input").get("checked")
-            if checked:
-                status = True
-            else:
-                status = False
-            todo_list.append([status, description])
-        # free mem
-        soup.decompose()
-        del soup
+        try:
+            todo_labels = soup.find_all("label", {"class": "todo-list__label"})
+            todo_list: list[list[Union[bool, str]]] = []
+            for x in todo_labels:
+                description = x.text.strip()
+                checked = x.find("input").get("checked")
+                if checked:
+                    status = True
+                else:
+                    status = False
+                todo_list.append([status, description])
+        finally:
+            # free mem
+            soup.decompose()
+            del soup
         return todo_list
 
-    def todo_check(self, todo_index, check=True):
-        """check/uncheck a todo"""
+    def todo_check(self, todo_index: int, check: bool = True) -> bool:
+        """check/uncheck a todo item by index.
+
+        :param todo_index: index starts from 0
+        :param check: True to check, False to uncheck
+        :return: True if success, False if failed
+        """
         content = self.get_today_note_content()
         soup = BeautifulSoup(content, 'html.parser')
         todo_labels = soup.find_all("label", {"class": "todo-list__label"})
         try:
             label = todo_labels[todo_index]
             check_input = label.find("input")
             if check:
                 check_input['checked'] = 'checked'
             else:
                 del check_input['checked']
 
             new_content = str(soup)
-            # free mem
-            soup.decompose()
-            del soup
-
             return self.set_today_note_content(new_content)
         except IndexError:
+            return False
+        finally:
             # free mem
             soup.decompose()
             del soup
-            return False
 
-    def todo_uncheck(self, todo_index):
-        """uncheck a todo"""
+    def todo_uncheck(self, todo_index: int) -> bool:
+        """uncheck a todo item by index.
+
+        :param todo_index: index starts from 0
+        :return: True if success, False if failed
+        """
         return self.todo_check(todo_index, check=False)
 
-    def add_todo(self, todo_description):
-        """append item to todo list"""
+    def add_todo(self, todo_description: str, todo_caption: str = r'<p>TODO:</p>') -> bool:
+        """append item to todo list.
+
+        :param todo_description: todo item
+        :param todo_caption: caption added to new todo lists, default to '<p>TODO:</p>'
+        :return: True if success, False if failed
+        """
         todo_description = todo_description.strip()
+        soup: Optional[BeautifulSoup] = None
         try:
             content = self.get_today_note_content()
             soup = BeautifulSoup(content, 'html.parser')
             todo_labels = soup.find_all("label", {"class": "todo-list__label"})
             # append todo item after last todo item
             # special case 1: no todo available, add it to the beginning of document
             # special case 2: if last todo item is empty, update it
 
             if "todo-list__label" in todo_description:
                 todo_item_html = f'''<li>{todo_description}</li>'''
             else:
-                todo_item_html = f'''<li><label class="todo-list__label"><input disabled="disabled" type="checkbox"/ > <span class = "todo-list__label__description">{todo_description}</span></label></li>'''
+                todo_item_html = ItemTemplate(todo_description).substitute()
 
             if not todo_labels:
                 logger.info('new empty page')
-                todo_item_html = f'''<p>TODO:</p><ul class="todo-list">{todo_item_html}</ul>'''
+                todo_item_html = ListTemplate(todo_caption).substitute(items=todo_item_html)
                 todo_item = BeautifulSoup(todo_item_html, 'html.parser')
                 soup.insert(0, todo_item)
             else:
                 last_todo_label = todo_labels[-1]
                 if not last_todo_label.text.strip():
                     # replace last empty todo item
                     todo_item = BeautifulSoup(todo_item_html, 'html.parser')
@@ -548,119 +655,146 @@
                     empty_li.replace_with(todo_item)
                 else:
                     # if todo item list exists, append to the end
                     todo_item = BeautifulSoup(todo_item_html, 'html.parser')
                     todo_list_label = soup.find_all("ul", {"class": "todo-list"})[0]
                     todo_list_label.append(todo_item)
             new_content = str(soup)
-            # free mem
-            soup.decompose()
-            del soup
 
             return self.set_today_note_content(new_content)
-
         except Exception as e:
             logger.info(e)
             return False
-
-    def update_todo(self, todo_index, todo_description):
-        """update a todo item description"""
+        finally:
+            # free mem
+            if soup:
+                soup.decompose()
+                del soup
+
+    def update_todo(self, todo_index: int, todo_description: str) -> bool:
+        """update a todo item by index.
+
+        :param todo_index: index starts from 0
+        :param todo_description: new todo item
+        :return: True if success, False if failed"""
         todo_description = todo_description.strip()
+
         content = self.get_today_note_content()
         soup = BeautifulSoup(content, 'html.parser')
         todo_labels = soup.find_all("label", {"class": "todo-list__label"})
         try:
             todo_label = todo_labels[todo_index]
             target_span = todo_label.find_next("span", {"class": "todo-list__label__description"})
             target_span.string = todo_description
             new_content = str(soup)
-            # free mem
-            soup.decompose()
-            del soup
             return self.set_today_note_content(new_content)
-
         except IndexError:
+            return False
+        finally:
             # free mem
             soup.decompose()
             del soup
-            return False
 
-    def delete_todo(self, todo_index):
-        """delete a todo item"""
+    def delete_todo(self, todo_index: int) -> bool:
+        """delete a todo item by index.
+
+        :param todo_index: index starts from 0
+        :return: True if success, False if failed
+        """
         date = get_today()
-        self.delete_date_todo(date, todo_index)
+        return self.delete_date_todo(date, todo_index)
 
-    def delete_yesterday_todo(self, todo_index):
+    def delete_yesterday_todo(self, todo_index: int) -> bool:
+        """delete todo item by index from yesterday's note.
+
+        :param todo_index: index starts from 0
+        :return: True if success, False if failed
+        """
         date = get_yesterday()
-        self.delete_date_todo(date, todo_index)
+        return self.delete_date_todo(date, todo_index)
+
+    def delete_date_todo(self, date: str, todo_index: int) -> bool:
+        """delete todo item by index from a specific date's note.
 
-    def delete_date_todo(self, date, todo_index):
+        :param date: date in format of "%Y-%m-%d", e.g. "2022-02-25"
+        :param todo_index: index starts from 0
+        :return: True if success, False if failed
+        """
         content = self.get_day_note(date)
+
         soup = BeautifulSoup(content, 'html.parser')
         todo_labels = soup.find_all("label", {"class": "todo-list__label"})
-
         try:
             todo_label = todo_labels[todo_index]
             # decompose parent <li> tag
             todo_label.parent.decompose()
-            new_content = str(soup)
 
-            # free mem
-            soup.decompose()
-            del soup
+            new_content = str(soup)
             return self.set_day_note(date, new_content)
-
         except IndexError:
+            return False
+        finally:
             # free mem
             soup.decompose()
             del soup
-            return False
 
-    def get_yesterday_unfinished_todo(self):
+    def get_yesterday_unfinished_todo(self) -> list[list[Union[bool, str]]]:
+        """get yesterday's unfinished todo list.
+
+        :return: list of todo items, each item is a list of [status, description]
+        """
         content = self.get_yesterday_note_content()
-        soup = BeautifulSoup(content, 'html.parser')
-        todo_labels = soup.find_all("label", {"class": "todo-list__label"})
+
         unfinished_todo_list = []
-        for x in todo_labels:
-            checked = x.find("input").get("checked")
-            if not checked:
-                description = x.text.strip()
-                unfinished_todo_list.append([False, description])
-        # free mem
-        soup.decompose()
-        del soup
+        soup = BeautifulSoup(content, 'html.parser')
+        try:
+            todo_labels = soup.find_all("label", {"class": "todo-list__label"})
+            for x in todo_labels:
+                checked = x.find("input").get("checked")
+                if not checked:
+                    description = x.text.strip()
+                    unfinished_todo_list.append([False, description])
+        finally:
+            # free mem
+            soup.decompose()
+            del soup
         return unfinished_todo_list
 
-    def move_yesterday_unfinished_todo_to_today(self):
+    def move_yesterday_unfinished_todo_to_today(self) -> None:
+        """move yesterday's unfinished todo list to today's note."""
         content = self.get_yesterday_note_content()
         soup = BeautifulSoup(content, 'html.parser')
-        todo_labels = soup.find_all("label", {"class": "todo-list__label"})
-        todo_indexes = []
-        todo_descriptions = []
-        for i, x in enumerate(todo_labels):
-            checked = x.find("input").get("checked")
-            if not checked:
-                description = x.text.strip()
-                if not description:
-                    # skip empty todos
-                    continue
-                todo_indexes.append(i)
-                # keep the internal link, text format or what so ever, avoid lost valuable info
-                todo_descriptions.append(str(x))
-
-        if not todo_descriptions:
-            return
-
-        # add todos to today
-        for description in todo_descriptions:
-            self.add_todo(description)
-
-        # remove todos from yesterday
-        for i in reversed(sorted(todo_indexes)):
-            self.delete_yesterday_todo(i)
+        try:
+            todo_labels = soup.find_all("label", {"class": "todo-list__label"})
+            todo_indexes = []
+            todo_descriptions = []
+            for i, x in enumerate(todo_labels):
+                checked = x.find("input").get("checked")
+                if not checked:
+                    description = x.text.strip()
+                    if not description:
+                        # skip empty todos
+                        continue
+                    todo_indexes.append(i)
+                    # keep the internal link, text format or what so ever, avoid lost valuable info
+                    todo_descriptions.append(str(x))
+
+            if not todo_descriptions:
+                return
+
+            # add todos to today
+            for description in todo_descriptions:
+                self.add_todo(description)
+
+            # remove todos from yesterday
+            for i in reversed(sorted(todo_indexes)):
+                self.delete_yesterday_todo(i)
+        finally:
+            soup.decompose()
+            del soup
 
     def upload_md_file(self, file: str, parentNoteId: str):
         md_file = os.path.abspath(file).replace('\\', '/').replace('//', '/')
         md_full_name = os.path.basename(md_file)
         md_name = md_full_name[:-3]
         md_folder = os.path.dirname(md_file)
         logger.info(md_file)
@@ -674,22 +808,27 @@
             # fix logseq image size format
             logseq_image_pat = r'(\!\[.*\]\(.*\))\{.*?:height.*width.*}'
             content = re.sub(logseq_image_pat, r'\1', content)
 
             if not re.search(re.escape("$"), content):
                 # extra format support
                 # https://github.com/trentm/python-markdown2/wiki/Extras
-                html = markdown2.markdown(content, extras=['fenced-code-blocks', 'strike', 'tables', 'task_list'])
+                html = markdown2.markdown(
+                    content, extras=['fenced-code-blocks', 'strike', 'tables', 'task_list']
+                )
                 # logger.info(html)
             else:
                 no_latex_part, latex_code_part = sanitizeInput(content)
-                html = reconstructMath(markdown2.markdown(no_latex_part,
-                                                          extras=['fenced-code-blocks', 'strike', 'tables',
-                                                                  'task_list']),
-                                       latex_code_part)
+                html = reconstructMath(
+                    markdown2.markdown(
+                        no_latex_part,
+                        extras=['fenced-code-blocks', 'strike', 'tables', 'task_list'],
+                    ),
+                    latex_code_part,
+                )
         note_id = ''
 
         # detect images
         pat = '<img (.*?) />'
         images = re.findall(pat, html)
 
         res = self.create_note(
@@ -751,34 +890,43 @@
                 res = self.create_image_note(
                     parentNoteId=note_id,
                     title=image_name,
                     image_file=image_file_path,
                 )
                 # logger.info(res)
                 image_note_id = res['note']['noteId']
-                # fix path with `/` in it, the param should be quoted. e.g. relative url from obsidian
-                image_url = f"api/images/{image_note_id}/{urllib.parse.quote(res['note']['title'], safe='')}"
+                # fix path with `/` in it, the param should be quoted.
+                # e.g. relative url from obsidian
+                image_url = (
+                    f"api/images/{image_note_id}/"
+                    f"{urllib.parse.quote(res['note']['title'], safe='')}"
+                )
                 logger.info(image_url)
 
                 html = html.replace(image_path, image_url)
 
                 # add relation for image
-                self.create_attribute(attributeId=None, noteId=note_id, type='relation', name='imageLink',
-                                      value=image_note_id, isInheritable=False)
+                self.create_attribute(
+                    attributeId=None,
+                    noteId=note_id,
+                    type='relation',
+                    name='imageLink',
+                    value=image_note_id,
+                    isInheritable=False,
+                )
 
             # replace note content
             res = self.update_note_content(note_id, html)
             # logger.info(res)
 
         # detect files
         pat = '<a href="(.*?)">(.*)</a>'
         a_links = re.findall(pat, html)
         logger.info(a_links)
         for link, link_name in a_links:
-
             # fix file path
             file_path = ''
             if link.startswith(('http:', 'https:')):
                 # skip online link
                 continue
             if os.path.exists(link):
                 # absolute file path
@@ -805,28 +953,36 @@
                     title=link_name,
                     file_path=file_path,
                 )
                 logger.info(res)
 
                 # update file link
                 file_note_id = res['note']['noteId']
-                # fix path with `/` in it, the param should be quoted. e.g. relative url from obsidian
+                # fix path with `/` in it, the param should be quoted.
+                # e.g. relative url from obsidian
                 file_url = f"#root/{note_id}/{file_note_id}"
 
                 html = html.replace(link, file_url)
 
             # replace note content
             res = self.update_note_content(note_id, html)
 
         return res
 
-    def upload_md_folder(self, parentNoteId: str, mdFolder: str, includePattern=[],
-                         ignoreFolder=[], ignoreFile=[]):
-        if not includePattern:
-            includePattern = ['.md', ]
+    def upload_md_folder(
+        self,
+        parentNoteId: str,
+        mdFolder: str,
+        includePattern: Optional[list[str]] = None,
+        ignoreFolder: Optional[list[str]] = None,
+        ignoreFile: Optional[list[str]] = None,
+    ):
+        includePattern = includePattern or ['.md']
+        ignoreFolder = ignoreFolder or []
+        ignoreFile = ignoreFile or []
 
         # note tree
         # record for noteId
         note_tree = {'.': parentNoteId}
         logger.info(mdFolder)
 
         mdFolder = os.path.expandvars(os.path.expanduser(mdFolder))
@@ -841,26 +997,26 @@
             logger.info('==============')
             logger.info(f'root {root}')
             logger.info(f'root_folder_name {root_folder_name}')
             logger.info(f'rel_path {rel_path}')
 
             current_parent_note_id = note_tree[rel_path]
 
-            logger.info(f'files')
+            logger.info('files')
             for name in natsort.natsorted(files):
                 # only include markdown files
                 if any(x == name for x in ignoreFile):
                     continue
 
                 if any(x in name for x in includePattern):
                     file_path = os.path.join(root, name)
                     logger.info(file_path)
                     self.upload_md_file(file=file_path, parentNoteId=current_parent_note_id)
 
-            logger.info(f'dirs')
+            logger.info('dirs')
             for name in natsort.natsorted(dirs):
                 if all(x not in name for x in ignoreFolder):
                     dir_path = os.path.join(root, name)
                     logger.info(dir_path)
                     rel_path = os.path.relpath(dir_path, start=mdFolder)
                     logger.info(rel_path)
                     res = self.create_note(
@@ -879,15 +1035,15 @@
 
         res = requests.put(url, headers=self.get_header())
         if res.status_code == 204:
             logger.info('backup successfully')
             return True
         return False
 
-    def beautify_note(self, noteId: str) -> str:
+    def beautify_note(self, noteId: str) -> bool:
         """
         beautify note content, add new lines and remove redundant lines, etc.
 
         :param noteId:
         :return:
         """
         content = self.get_note_content(noteId)
@@ -907,7 +1063,65 @@
 
         if note['type'] == 'text':
             self.beautify_note(noteId)
 
         for x in note['childNoteIds']:
             # logger.info(x)
             self.beautify_sub_notes(x)
+
+    def close(self):
+        """
+        Force sync from server
+
+        .. Code:: python
+
+        with closing(client.get_note(noteId)) as note:
+            pass
+
+        :return:
+        """
+        url = f"{self.server_url}/etapi/sync/now"
+        res = requests.post(url, headers=self.get_header())
+        if res.status_code == 200:
+            logger.info("sync successfully")
+
+
+class ListTemplate(string.Template):
+    """Encapsulate To Do List HTML details
+
+    :param caption: Text to be presented as the To Do list caption. Default: <p>TODO:</p>
+    """
+
+    def __init__(self, caption: str = '<p>TODO:</p>') -> None:
+        self._defaults: dict[str, object] = {
+            'caption': caption,
+        }
+        super().__init__('${caption}<ul class="todo-list">${items}</ul>')
+
+    def substitute(self, mapping: Optional[Mapping[str, object]] = None, **kwds: object) -> str:
+        d = self._defaults.copy()
+        d.update(mapping or {})
+        return super().substitute(d, **kwds)
+
+
+class ItemTemplate(string.Template):
+    """Encapsulate To Do Item HTML details
+
+    :param description: Optional text to be presented as the To Do item
+    :param checked: If True To Do item is presented will filled in check box. Default is False.
+    """
+
+    def __init__(self, description: Optional[str] = None, checked: bool = False) -> None:
+        super().__init__(
+            '<li><label class="todo-list__label">'
+            '<input${checked} disabled="disabled" type="checkbox"/>'
+            '<span class="todo-list__label__description">$description</span></label></li>'
+        )
+        self._defaults: dict[str, object] = {
+            'description': description,
+            'checked': ' checked="checked"' if checked else '',
+        }
+
+    def substitute(self, mapping: Optional[Mapping[str, object]] = None, **kwds: object) -> str:
+        d = self._defaults.copy()
+        d.update(mapping or {})
+        return super().substitute(d, **kwds)
```

## trilium_py/utils/markdown_math.py

```diff
@@ -1,141 +1,188 @@
 import re
+from typing import List, Optional
+
 from markdown2 import markdown
 
-# It's part of https://github.com/constantAmateur/markdown2Mathjax/blob/master/lib/markdown2Mathjax.py
+# It's part of
+#     https://github.com/constantAmateur/markdown2Mathjax/blob/master/lib/markdown2Mathjax.py
+
+
+def break_tie(inline, equation):
+    """If one of the delimiters is a substring of the other (e.g., $ and $$) it is possible that
+    the two will begin at the same location. In this case we need some criteria to break the tie
+    and decide which operation takes precedence. I've gone with the longer of the two delimiters
+    takes priority (for example, $$ over $). This function should return a 2 for the equation
+    block taking precedence, a 1 for the inline block. The magic looking return statement is
+    to map 0->2 and 1->1.
+    """
+    tmp = inline.end() - inline.start() > equation.end() - equation.start()
+    return (tmp * 3 + 2) % 4
 
-def break_tie(inline,equation):
-    """If one of the delimiters is a substring of the other (e.g., $ and $$) it is possible that the two will begin at the same location.  
-    In this case we need some criteria to break the tie and decide which operation takes precedence.  
-    I've gone with the longer of the two delimiters takes priority (for example, $$ over $).  
-    This function should return a 2 for the equation block taking precedence, a 1 for the inline block.  
-    The magic looking return statement is to map 0->2 and 1->1."""
-    tmp=(inline.end()-inline.start() > equation.end()-equation.start())
-    return (tmp*3+2)%4
 
 def markdown_safe(placeholder):
     """Is the placeholder changed by markdown?  If it is, this isn't a valid placeholder."""
-    mdstrip=re.compile("<p>(.*)</p>\n")
-    md=markdown(placeholder)
-    mdp=mdstrip.match(md)
-    if mdp and mdp.group(1)==placeholder:
+    mdstrip = re.compile("<p>(.*)</p>\n")
+    md = markdown(placeholder)
+    mdp = mdstrip.match(md)
+    if mdp and mdp.group(1) == placeholder:
         return True
     return False
 
-def sanitizeInput(string,inline_delims=["$","$"],equation_delims=["$$","$$"],placeholder="$0$"):
-    """Given a string that will be passed to markdown, the content of the different math blocks is stripped out and replaced by a placeholder which MUST be ignored by markdown.  A list is returned containing the text with placeholders and a list of the stripped out equations.  Note that any pre-existing instances of the placeholder are "replaced" with themselves and a corresponding dummy entry is placed in the returned codeblock.  The sanitized string can then be passed safetly through markdown and then reconstructed with reconstructMath.
 
-    There are potential four delimiters that can be specified.  The left and right delimiters for inline and equation mode math.  These can potentially be anything that isn't already used by markdown and is compatible with mathjax (see documentation for both).
+def sanitizeInput(
+    string,
+    inline_delims: Optional[List[str]] = None,
+    equation_delims: Optional[List[str]] = None,
+    placeholder="$0$",
+):
+    """Given a string that will be passed to markdown, the content of the different math blocks
+    is stripped out and replaced by a placeholder which MUST be ignored by markdown.  A list
+    is returned containing the text with placeholders and a list of the stripped out equations.
+    Note that any pre-existing instances of the placeholder are "replaced" with themselves
+    and a corresponding dummy entry is placed in the returned codeblock.  The sanitized string
+    can then be passed safety through markdown and then reconstructed with reconstructMath.
+
+    There are potential four delimiters that can be specified.  The left and right delimiters
+    for inline and equation mode math.  These can potentially be anything that isn't already
+    used by markdown and is compatible with mathjax (see documentation for both).
     """
-    #Check placeholder is valid.
+    inline_delims = inline_delims or ["$", "$"]
+    equation_delims = equation_delims or ["$$", "$$"]
+
+    # Check placeholder is valid.
     if not markdown_safe(placeholder):
         raise ValueError("Placeholder %s altered by markdown processing." % placeholder)
-    #really what we want is a reverse markdown function, but as that's too much work, this will do
-    inline_left=re.compile("(?<!\\\\)"+re.escape(inline_delims[0]))
-    inline_right=re.compile("(?<!\\\\)"+re.escape(inline_delims[1]))
-    equation_left=re.compile("(?<!\\\\)"+re.escape(equation_delims[0]))
-    equation_right=re.compile("(?<!\\\\)"+re.escape(equation_delims[1]))
-    placeholder_re = re.compile("(?<!\\\\)"+re.escape(placeholder))
+    # really what we want is a reverse markdown function, but as that's too much work, this will do
+    inline_left = re.compile("(?<!\\\\)" + re.escape(inline_delims[0]))
+    inline_right = re.compile("(?<!\\\\)" + re.escape(inline_delims[1]))
+    equation_left = re.compile("(?<!\\\\)" + re.escape(equation_delims[0]))
+    equation_right = re.compile("(?<!\\\\)" + re.escape(equation_delims[1]))
+    placeholder_re = re.compile("(?<!\\\\)" + re.escape(placeholder))
     placeholder_scan = placeholder_re.scanner(string)
-    ilscanner=[inline_left.scanner(string),inline_right.scanner(string)]
-    eqscanner=[equation_left.scanner(string),equation_right.scanner(string)]
-    scanners=[placeholder_scan,ilscanner,eqscanner]
-    #There are 3 types of blocks, inline math, equation math and occurances of the placeholder in the text
-    #inBlack is 0 for a placeholder, 1 for inline block, 2 for equation
-    inBlock=0
-    post=-1
-    stlen=len(string)
-    startmatches=[placeholder_scan.search(),ilscanner[0].search(),eqscanner[0].search()]
-    startpoints=[stlen,stlen,stlen]
-    startpoints[0]= startmatches[0].start() if startmatches[0] else stlen
-    startpoints[1]= startmatches[1].start() if startmatches[1] else stlen
-    startpoints[2]= startmatches[2].start() if startmatches[2] else stlen
-    terminator=-1
-    sanitizedString=''
-    codeblocks=[]
+    ilscanner = [inline_left.scanner(string), inline_right.scanner(string)]
+    eqscanner = [equation_left.scanner(string), equation_right.scanner(string)]
+    scanners = [placeholder_scan, ilscanner, eqscanner]
+    # There are 3 types of blocks, inline math, equation math and occurrences of the
+    # placeholder in the text inBlack is 0 for a placeholder, 1 for inline block, 2 for equation
+    inBlock = 0
+    post = -1
+    stlen = len(string)
+    startmatches = [placeholder_scan.search(), ilscanner[0].search(), eqscanner[0].search()]
+    startpoints = [stlen, stlen, stlen]
+    startpoints[0] = startmatches[0].start() if startmatches[0] else stlen
+    startpoints[1] = startmatches[1].start() if startmatches[1] else stlen
+    startpoints[2] = startmatches[2].start() if startmatches[2] else stlen
+    terminator = -1
+    sanitizedString = ''
+    codeblocks = []
     while 1:
-        #find the next point of interest.
-        while startmatches[0] and startmatches[0].start()<post:
-            startmatches[0]=placeholder_scan.search()
-            startpoints[0]= startmatches[0].start() if startmatches[0] else stlen
-        while startmatches[1] and startmatches[1].start()<post:
-            startmatches[1]=ilscanner[0].search()
-            startpoints[1]= startmatches[1].start() if startmatches[1] else stlen
-        while startmatches[2] and startmatches[2].start()<post:
-            startmatches[2]=eqscanner[0].search()
-            startpoints[2]= startmatches[2].start() if startmatches[2] else stlen
-        #Found start of next block of each type
-        #Placeholder type always takes precedence if it exists and is next...
-        if startmatches[0] and min(startpoints)==startpoints[0]:
-            #We can do it all in one!
-            #First add the "stripped" code to the blocks
-            codeblocks.append('0'+placeholder)
-            #Work out where the placeholder ends
-            tmp=startpoints[0]+len(placeholder)
-            #Add the "sanitized" text up to and including the placeholder
-            sanitizedString = sanitizedString + string[post*(post>=0):tmp]
-            #Set the new post
-            post=tmp
-            #Back to start!
+        # find the next point of interest.
+        while startmatches[0] and startmatches[0].start() < post:
+            startmatches[0] = placeholder_scan.search()
+            startpoints[0] = startmatches[0].start() if startmatches[0] else stlen
+        while startmatches[1] and startmatches[1].start() < post:
+            startmatches[1] = ilscanner[0].search()
+            startpoints[1] = startmatches[1].start() if startmatches[1] else stlen
+        while startmatches[2] and startmatches[2].start() < post:
+            startmatches[2] = eqscanner[0].search()
+            startpoints[2] = startmatches[2].start() if startmatches[2] else stlen
+        # Found start of next block of each type
+        # Placeholder type always takes precedence if it exists and is next...
+        if startmatches[0] and min(startpoints) == startpoints[0]:
+            # We can do it all in one!
+            # First add the "stripped" code to the blocks
+            codeblocks.append('0' + placeholder)
+            # Work out where the placeholder ends
+            tmp = startpoints[0] + len(placeholder)
+            # Add the "sanitized" text up to and including the placeholder
+            sanitizedString = sanitizedString + string[post * (post >= 0) : tmp]
+            # Set the new post
+            post = tmp
+            # Back to start!
             continue
         elif startmatches[1] is None and startmatches[2] is None:
-                #No more blocks, add in the rest of string and be done with it...
-            sanitizedString = sanitizedString + string[post*(post>=0):]
+            # No more blocks, add in the rest of string and be done with it...
+            sanitizedString = sanitizedString + string[post * (post >= 0) :]
             return (sanitizedString, codeblocks)
         elif startmatches[1] is None:
-            inBlock=2
+            inBlock = 2
         elif startmatches[2] is None:
-            inBlock=1
+            inBlock = 1
         else:
-            inBlock = (startpoints[1] < startpoints[2]) + (startpoints[1] > startpoints[2])*2
+            inBlock = (startpoints[1] < startpoints[2]) + (startpoints[1] > startpoints[2]) * 2
             if not inBlock:
-                inBlock = break_tie(startmatches[1],startmatches[2])
-            #Magic to ensure minimum index is 0
-        sanitizedString = sanitizedString+string[(post*(post>=0)):startpoints[inBlock]]
+                inBlock = break_tie(startmatches[1], startmatches[2])
+            # Magic to ensure minimum index is 0
+        sanitizedString = sanitizedString + string[(post * (post >= 0)) : startpoints[inBlock]]
         post = startmatches[inBlock].end()
-            #Now find the matching end...
-        while terminator<post:
-            endpoint=scanners[inBlock][1].search()
-                #If we run out of terminators before ending this loop, we're done
+        # Now find the matching end...
+        while terminator < post:
+            endpoint = scanners[inBlock][1].search()
+            # If we run out of terminators before ending this loop, we're done
             if endpoint is None:
-                    #Add the unterminated codeblock to the sanitized string
-                sanitizedString = sanitizedString + string[startpoints[inBlock]:]
+                # Add the unterminated codeblock to the sanitized string
+                sanitizedString = sanitizedString + string[startpoints[inBlock] :]
                 return (sanitizedString, codeblocks)
-            terminator=endpoint.start()
-            #We fonud a matching endpoint, add the bit to the appropriate codeblock...
-        codeblocks.append(str(inBlock)+string[post:endpoint.start()])
-            #Now add in the appropriate placeholder
-        sanitizedString = sanitizedString+placeholder
-            #Fabulous.  Now we can start again once we update post...
+            terminator = endpoint.start()
+            # We fonud a matching endpoint, add the bit to the appropriate codeblock...
+        codeblocks.append(str(inBlock) + string[post : endpoint.start()])
+        # Now add in the appropriate placeholder
+        sanitizedString = sanitizedString + placeholder
+        # Fabulous.  Now we can start again once we update post...
         post = endpoint.end()
 
-def reconstructMath(processedString,codeblocks,inline_delims=['<span class="math-tex">\(','\)</span>'],equation_delims=['<span class="math-tex">\[','\]</span>'],placeholder="$0$"):
-    """This is usually the output of sanitizeInput, after having passed the output string through markdown.  The delimiters given to this function should match those used to construct the string to begin with.
 
-     This will output a string containing html suitable to use with mathjax.
-     
-     "<" and ">" "&" symbols in math can confuse the html interpreter because they mark the begining and end of definition blocks.  To avoid issues, if htmlSafe is set to True these symbols will be replaced by ascii codes in the math blocks. The downside to this is that if anyone is already doing this, there already niced text might be mangled (I think I've taken steps to make sure it won't but not extensively tested...)"""
-    delims=[['',''],inline_delims,equation_delims]
-    placeholder_re = re.compile("(?<!\\\\)"+re.escape(placeholder))
-    #If we've defined some "new" special characters we'll have to process any escapes of them here
-    #Make html substitutions.
-    #if htmlSafe:
+def reconstructMath(
+    processedString,
+    codeblocks,
+    inline_delims: Optional[List[str]] = None,
+    equation_delims: Optional[List[str]] = None,
+    placeholder="$0$",
+):
+    """This is usually the output of sanitizeInput, after having passed the output string through
+    markdown.  The delimiters given to this function should match those used to construct the
+    string to begin with.
+
+    This will output a string containing html suitable to use with mathjax.
+
+    "<" and ">" "&" symbols in math can confuse the html interpreter because they mark the
+    beginning and end of definition blocks.  To avoid issues, if htmlSafe is set to True these
+    symbols will be replaced by ascii codes in the math blocks. The downside to this is that if
+    anyone is already doing this, there already formatted text might be mangled (I think I've taken
+    steps to make sure it won't but not extensively tested...)
+    """
+    inline_delims = inline_delims or ['<span class="math-tex">\\(', '\\)</span>']
+    equation_delims = equation_delims or ['<span class="math-tex">\\[', '\\]</span>']
+
+    delims = [['', ''], inline_delims, equation_delims]
+    placeholder_re = re.compile("(?<!\\\\)" + re.escape(placeholder))
+    # If we've defined some "new" special characters we'll have to process any escapes of them here
+    # Make html substitutions.
+    # if htmlSafe:
     #    safeAmp=re.compile("&(?!(?:amp;|lt;|gt;))")
     #    for i in range(len(codeblocks)):
     #        codeblocks[i]=safeAmp.sub("&amp;",codeblocks[i])
     #        codeblocks[i]=codeblocks[i].replace("<","&lt;")
     #        codeblocks[i]=codeblocks[i].replace(">","&gt;")
-    #Step through the codeblocks one at a time and replace the next occurance of the placeholder.  Extra placeholders are invalid math blocks and ignored...
-    outString=''
+    # Step through the codeblocks one at a time and replace the next occurrence of the placeholder.
+    # Extra placeholders are invalid math blocks and ignored...
+    outString = ''
     scan = placeholder_re.scanner(processedString)
-    post=0
+    post = 0
     for i in range(len(codeblocks)):
-        inBlock=int(codeblocks[i][0])
-        match=scan.search()
+        inBlock = int(codeblocks[i][0])
+        match = scan.search()
         if not match:
             raise ValueError("More codeblocks given than valid placeholders in text.")
-        outString=outString+processedString[post:match.start()]+delims[inBlock][0]+codeblocks[i][1:].strip()+delims[inBlock][1]
+        outString = (
+            outString
+            + processedString[post : match.start()]
+            + delims[inBlock][0]
+            + codeblocks[i][1:].strip()
+            + delims[inBlock][1]
+        )
         post = match.end()
-    #Add the rest of the string (if we need to)
-    if post<len(processedString):
-        outString = outString+processedString[post:]
+    # Add the rest of the string (if we need to)
+    if post < len(processedString):
+        outString = outString + processedString[post:]
     return outString
```

## trilium_py/utils/note_util.py

```diff
@@ -34,16 +34,18 @@
                 back_pos1 = pos - len(key1)
                 key2 = '<p></p>'
                 back_pos2 = pos - len(key2)
 
                 # logger.info(f'pos1 {content[back_pos1:pos]}')
                 # logger.info(f'pos2 {content[back_pos2:pos]}')
 
-                if not ((back_pos1 >= 0 and content[back_pos1:pos] == key1) or (
-                        back_pos2 >= 0 and content[back_pos2:pos] == key2)):
+                if not (
+                    (back_pos1 >= 0 and content[back_pos1:pos] == key1)
+                    or (back_pos2 >= 0 and content[back_pos2:pos] == key2)
+                ):
                     content = content[:pos] + '<p></p>' + content[pos:]
 
     # remove redundant new line in code block
     content = content.replace('\n</code></pre>', '</code></pre>')
 
     # add new line to image
     content = content.replace(' <img', '</p><p><img')
```

## trilium_py/utils/param_util.py

```diff
@@ -1,28 +1,32 @@
-import json
-
-
-def format_query_string(params):
-    """
-
-    convert
-    {"search": "root", "fastSearch": False}
-    to
-    {"search": "root", "fastSearch": "false"}
-
-    cause trilium takes "false" and "true" instead of "False" and "True"
-    :param params:
-    :return:
-    """
-    json_str = str(json.dumps(params, ensure_ascii=False)).replace(': false', ': "false"').replace(': true', ': "true"')
-    params = json.loads(json_str)
-    return params
-
-
-def clean_param(params):
-    clean_list = []
-    for k, v in params.items():
-        if not v:
-            clean_list.append(k)
-    for x in clean_list:
-        params.pop(x)
-    return params
+import json
+
+
+def format_query_string(params):
+    """
+
+    convert
+    {"search": "root", "fastSearch": False}
+    to
+    {"search": "root", "fastSearch": "false"}
+
+    cause trilium takes "false" and "true" instead of "False" and "True"
+    :param params:
+    :return:
+    """
+    json_str = (
+        str(json.dumps(params, ensure_ascii=False))
+        .replace(': false', ': "false"')
+        .replace(': true', ': "true"')
+    )
+    params = json.loads(json_str)
+    return params
+
+
+def clean_param(params):
+    clean_list = []
+    for k, v in params.items():
+        if not v:
+            clean_list.append(k)
+    for x in clean_list:
+        params.pop(x)
+    return params
```

## trilium_py/utils/url_util.py

```diff
@@ -1,18 +1,22 @@
-import json
-
-
-def format_query_string(params):
-    """
-
-    convert
-    {"search": "root", "fastSearch": False}
-    to
-    {"search": "root", "fastSearch": "false"}
-
-    cause trilium takes "false" and "true" instead of "False" and "True"
-    :param params:
-    :return:
-    """
-    json_str = str(json.dumps(params, ensure_ascii=False)).replace(': false', ': "false"').replace(': true', ': "true"')
-    params = json.loads(json_str)
-    return params
+import json
+
+
+def format_query_string(params):
+    """
+
+    convert
+    {"search": "root", "fastSearch": False}
+    to
+    {"search": "root", "fastSearch": "false"}
+
+    cause trilium takes "false" and "true" instead of "False" and "True"
+    :param params:
+    :return:
+    """
+    json_str = (
+        str(json.dumps(params, ensure_ascii=False))
+        .replace(': false', ': "false"')
+        .replace(': true', ': "true"')
+    )
+    params = json.loads(json_str)
+    return params
```

## Comparing `trilium_py-0.8.1.dist-info/LICENSE.txt` & `trilium_py-0.8.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.8.1.dist-info/METADATA` & `trilium_py-0.8.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
 Project-URL: Source, https://github.com/nriver/trilium-py/
 Keywords: trilium,etapi,api client
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: BeautifulSoup4
 Requires-Dist: requests
 Requires-Dist: markdown2[all]
 Requires-Dist: natsort
 Requires-Dist: loguru
@@ -43,68 +40,68 @@
 [![Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)](https://pypi.org/project/trilium-py)
 [![Supported Versions](https://img.shields.io/pypi/v/trilium-py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/trilium-py)
 [![PyPI license](https://img.shields.io/pypi/l/trilium-py.svg)](https://pypi.python.org/pypi/trilium-py/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
 <a href="https://github.com/Nriver"><img align="center" src="https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py"></a><br>
 
-# 🦮 Table of Contents
+## 🦮 Table of Contents
 
 <!--ts-->
 
 - [🐍 trilium-py](#-trilium-py)
-- [🦮 Table of Contents](#-table-of-contents)
-- [🔧 Installation](#-installation)
-- [📖 (Basic) Usage](#-basic-usage)
+  - [🦮 Table of Contents](#-table-of-contents)
+  - [🔧 Installation](#-installation)
+  - [📖 (Basic) Usage](#-basic-usage)
     - [🚀 Initialization](#-initialization)
     - [📊 Application Information](#-application-information)
     - [🔍 Search note](#-search-note)
     - [🏭 Create Note](#-create-note)
-        - [🖼️ Create Image note](#️-create-image-note)
+      - [🖼️ Create Image note](#️-create-image-note)
     - [👀 Get note](#-get-note)
     - [🔄 Update note](#-update-note)
     - [🗑️ Delete note](#️-delete-note)
     - [📅 Day note](#-day-note)
     - [📤 Export note](#-export-note)
-    - [💾Create data backup](#-create-data-backup)
-- [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
+    - [💾 Create data backup](#-create-data-backup)
+  - [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
     - [Add TODO item](#add-todo-item)
     - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
     - [Update a TODO item](#update-a-todo-item)
-    - [Delete a TDOO item](#delete-a-tdoo-item)
+    - [Delete a TODO item](#delete-a-todo-item)
     - [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
-- [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
+  - [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
     - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
     - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
-        - [Import from VNote](#import-from-vnote)
-        - [Import from Joplin](#import-from-joplin)
-        - [Import from Logseq](#import-from-logseq)
-        - [Import from Obsidian](#import-from-obsidian)
-        - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
-        - [Import from Turtl](#import-from-turtl)
-        - [Import from other markdown software](#import-from-other-markdown-software)
-- [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
+      - [Import from VNote](#import-from-vnote)
+      - [Import from Joplin](#import-from-joplin)
+      - [Import from Logseq](#import-from-logseq)
+      - [Import from Obsidian](#import-from-obsidian)
+      - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
+      - [Import from Turtl](#import-from-turtl)
+      - [Import from other markdown software](#import-from-other-markdown-software)
+  - [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
     - [Beautify a note](#beautify-a-note)
     - [Beautify a note and its child notes](#beautify-a-note-and-its-child-notes)
-- [🛠️ Develop](#️-develop)
-- [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
+  - [🛠️ Develop](#️-develop)
+  - [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 
 <!--te-->
 
-# 🔧 Installation
+## 🔧 Installation
 
 ```bash
 python3 -m pip install trilium-py --user
 ```
 
-# 📖 (Basic) Usage
+## 📖 (Basic) Usage
 
 These are basic function that Trilium's ETAPI provides. Down below are some simple example code to use this package.
 
-## 🚀 Initialization
+### 🚀 Initialization
 
 If you have a ETAPI token, change the `server_url` and `token` to yours.
 
 ```python
 from trilium_py.client import ETAPI
 
 server_url = 'http://localhost:8080'
@@ -123,38 +120,38 @@
 ea = ETAPI(server_url)
 token = ea.login(password)
 print(token)
 ```
 
 After initialization, you can use Trilium ETAPI with python now. The following are some examples.
 
-## 📊 Application Information
+### 📊 Application Information
 
 To start with, you can get the application information like this.
 
 ```python
 print(ea.app_info())
 ```
 
 It should give you the version of your server application and some extra information.
 
-## 🔍 Search note
+### 🔍 Search note
 
 Search note with keyword.
 
 ```python
 res = ea.search_note(
     search="python",
 )
 
 for x in res['results']:
     print(x['noteId'], x['title'])
 ```
 
-## 🏭 Create Note
+### 🏭 Create Note
 
 You can create a simple note like this.
 
 ```python
 res = ea.create_note(
     parentNoteId="root",
     title="Simple note 1",
@@ -166,42 +163,42 @@
 
 The `noteId` is not mandatory, if not provided, Trilium will generate a random one. You can retrieve it in the return.
 
 ```python
 noteId = res['note']['noteId']
 ```
 
-### 🖼️ Create Image note
+#### 🖼️ Create Image note
 
 Image note is a special kind of note. You can create an image note with minimal information like this. The `image_file`
 refers to the path of image.
 
 ```python
 res = ea.create_image_note(
     parentNoteId="root",
     title="Image note 1",
     image_file="shield.png",
 )
 ```
 
-## 👀 Get note
+### 👀 Get note
 
 To retrieve the note's content.
 
 ```python
 ea.get_note_content("note1")
 ```
 
 You can get a note metadata by its id.
 
 ```python
 ea.get_note(note_id)
 ```
 
-## 🔄 Update note
+### 🔄 Update note
 
 Update note content
 
 ```python
 ea.update_note_content("note1", "updated by python")
 ```
 
@@ -210,156 +207,156 @@
 ```python
 ea.patch_note(
     noteId="note1",
     title="Python client moded",
 )
 ```
 
-## 🗑️ Delete note
+### 🗑️ Delete note
 
 Simply delete a note by id.
 
 ```python
 ea.delete_note("note1")
 ```
 
-## 📅 Day note
+### 📅 Day note
 
 You can get the content of a certain date with `get_day_note`. The date string should be in format of "%Y-%m-%d", e.g. "
 2022-02-25".
 
 ```python
 es.get_day_note("2022-02-25")
 ```
 
 Then set/update a day note with `set_day_note`. The content should be a (html) string.
 
 ```python
 self.set_day_note(date, new_content)
 ```
 
-## 📤 Export note
+### 📤 Export note
 
 Export note comes in two formats `html` or `markdown`/`md`.
 
 ```python
 res = ea.export_note(
     noteId='sK5fn4T6yZRI',
     format='md',
     savePath='/home/nate/data/1/test.zip',
 )
 ```
 
-## 💾 Create data backup
+### 💾 Create data backup
 
 This example will create a database backup file like this `trilium-data/backup/backup-test.db`.
 
 ```python
 res = ea.backup("test")
 ```
 
-# (Advanced Usage) ✅ TODO List
+## (Advanced Usage) ✅ TODO List
 
 With the power of Python, I have expanded the basic usage of ETAPI. You can do something with todo list now.
 
-## Add TODO item
+### Add TODO item
 
 You can use `add_todo` to add a TODO item, param is the TODO description
 
 ```python
 ea.add_todo("买暖宝宝")
 ```
 
-## Check/Uncheck a TODO item
+### Check/Uncheck a TODO item
 
 param is the index of the TODO item
 
 ```python
 ea.todo_check(0)
 ea.todo_uncheck(1)
 ```
 
-## Update a TODO item
+### Update a TODO item
 
 Use `update_todo` to update a TODO item description at certain index.
 
 ```python
 ea.update_todo(0, "去码头整点薯条")
 ```
 
-## Delete a TDOO item
+### Delete a TODO item
 
 Remove a TODO item by its index.
 
 ```python
 ea.delete_todo(1)
 ```
 
-## Move yesterday's unfinished todo to today
+### Move yesterday's unfinished todo to today
 
-As the title suggests, you can move yesterday's unfinished things to today. Unfinished todos will be deleted from
+As the title suggests, you can move yesterday's unfinished things to today. Unfinished todo's will be deleted from
 yesterday's note.
 
 ```python
 ea.move_yesterday_unfinished_todo_to_today()
 ```
 
-# (Advanced Usage) 🚚 Upload Markdown files
+## (Advanced Usage) 🚚 Upload Markdown files
 
-## Upload single Markdown file with images
+### Upload single Markdown file with images
 
 You can import Markdown file with images into Trilium now! Trilium-py will help you to upload the images and fix the
 links for you!
 
 ```python
 res = ea.upload_md_file(
     parentNoteId="root",
     file="./md-demo/manjaro 修改caps lock.md",
 )
 ```
 
-## Bulk upload Markdown files in a folder
+### Bulk upload Markdown files in a folder
 
 You can upload a folder with lots of Markdown files to Trilium and preserve the folder structure!
 
-### Import from VNote
+#### Import from VNote
 
 Say, upload all the notes from [VNote](https://github.com/vnotex/vnote), simply do this:
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="~/data/vnotebook/",
     ignoreFolder=['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'],
 )
 ```
 
-### Import from Joplin
+#### Import from Joplin
 
 Joplin can be imported effortlessly.
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/joplin_data/",
     ignoreFolder=['_resources', ],
 )
 ```
 
-### Import from Logseq
+#### Import from Logseq
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/logseq_data/",
     ignoreFolder=['assets', 'logseq'],
 )
 ```
 
-### Import from Obsidian
+#### Import from Obsidian
 
 Obsidian has a very unique linking system for files. You should use [obsidian-export
 ](https://github.com/zoni/obsidian-export) to convert a Obsidian vault to regular Markdown files. Then you should be
 able to import the note into Trilium with trilium-py.
 
 Convert it first.
 
@@ -372,42 +369,42 @@
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="E:/data/out",
 )
 ```
 
-### Import from Youdao Note/有道云笔记
+#### Import from Youdao Note/有道云笔记
 
 Youdao does not provide an export feature anymore. Luckily, you can use <https://github.com/DeppWang/youdaonote-pull> to
 download your notes and convert them into markdown files. After that, trilium-py should be able to help you import them.
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/gitRepo/youdaonote-pull/out/",
 )
 ```
 
-### Import from Turtl
+#### Import from Turtl
 
 You need to convert Turtl from json to markdown first.
 See [turtl-to-markdown](https://github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
 
 Then you can import with trilium-py like this:
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/gitRepo/turtl-to-markdown/out/",
     ignoreFolder=['_resources'],
 )
 ```
 
-### Import from other markdown software
+#### Import from other markdown software
 
 In general, markdown files have variety of standards. You can always try import them with
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/your_markdown_files/",
@@ -425,29 +422,29 @@
 
 Here is what you can do to beautify your note.
 
 ### Beautify a note
 
 Specify a note id to beautify note content.
 
-```
+```python
 ea.beautify_note('krm8B9JthNfi')
 ```
 
 ### Beautify a note and its child notes
 
-```
+```python
 ea.beautify_sub_notes('tlPuzU2szLJh')
 ```
 
-# 🛠️ Develop
+## 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
 
 ```python
 python -m pip install --user -e .
 ```
 
-# 🔗 Original OpenAPI Documentation
+## 🔗 Original OpenAPI Documentation
 
 The original OpenAPI document is [here](https://github.com/zadam/trilium/blob/master/src/etapi/etapi.openapi.yaml). You
 can open it with [swagger editor](https://editor.swagger.io/).
```

### html2text {}

```diff
@@ -1,157 +1,156 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.8.1 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.8.2 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
 OSI Approved :: GNU Affero General Public License v3 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
+Only Requires-Python: >=3.9, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: BeautifulSoup4 Requires-Dist: requests
 Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: loguru
 Requires-Dist: minify-html Requires-Dist: python-magic-bin ; platform_system ==
 "Windows" Requires-Dist: python-magic ; sys_platform == "darwin" Requires-Dist:
 python-magic ; sys_platform == "linux" # ð trilium-py Python client for
 ETAPI of Trilium Note. [![Downloads](https://static.pepy.tech/badge/trilium-
 py)](https://pepy.tech/project/trilium-py) [![Supported Versions](https://
 img.shields.io/pypi/pyversions/trilium-py.svg)](https://pypi.org/project/
 trilium-py) [![Supported Versions](https://img.shields.io/pypi/v/trilium-
 py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/trilium-py)
 [![PyPI license](https://img.shields.io/pypi/l/trilium-py.svg)](https://
 pypi.python.org/pypi/trilium-py/) [![Maintenance](https://img.shields.io/badge/
 Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
 commit-activity) [https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py]
-# ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
+## ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
 Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
 (Basic) Usage](#-basic-usage) - [ð Initialization](#-initialization) - [ð
 Application Information](#-application-information) - [ð Search note](#-
 search-note) - [ð­ Create Note](#-create-note) - [ð¼ï¸ Create Image note]
 (#ï¸-create-image-note) - [ð Get note](#-get-note) - [ð Update note](#-
 update-note) - [ðï¸ Delete note](#ï¸-delete-note) - [ð Day note](#-day-
-note) - [ð¤ Export note](#-export-note) - [ð¾Create data backup](#-create-
+note) - [ð¤ Export note](#-export-note) - [ð¾ Create data backup](#-create-
 data-backup) - [(Advanced Usage) â TODO List](#advanced-usage--todo-list) -
 [Add TODO item](#add-todo-item) - [Check/Uncheck a TODO item](#checkuncheck-a-
-todo-item) - [Update a TODO item](#update-a-todo-item) - [Delete a TDOO item]
-(#delete-a-tdoo-item) - [Move yesterday's unfinished todo to today](#move-
+todo-item) - [Update a TODO item](#update-a-todo-item) - [Delete a TODO item]
+(#delete-a-todo-item) - [Move yesterday's unfinished todo to today](#move-
 yesterdays-unfinished-todo-to-today) - [(Advanced Usage) ð Upload Markdown
 files](#advanced-usage--upload-markdown-files) - [Upload single Markdown file
 with images](#upload-single-markdown-file-with-images) - [Bulk upload Markdown
 files in a folder](#bulk-upload-markdown-files-in-a-folder) - [Import from
 VNote](#import-from-vnote) - [Import from Joplin](#import-from-joplin) -
 [Import from Logseq](#import-from-logseq) - [Import from Obsidian](#import-
 from-obsidian) - [Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
 noteæéäºç¬è®°) - [Import from Turtl](#import-from-turtl) - [Import from
 other markdown software](#import-from-other-markdown-software) - [(Advanced
 Usage) ð¨ Beautify notes](#advanced-usage--beautify-notes) - [Beautify a
 note](#beautify-a-note) - [Beautify a note and its child notes](#beautify-a-
 note-and-its-child-notes) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
-OpenAPI Documentation](#-original-openapi-documentation)  # ð§ Installation
-```bash python3 -m pip install trilium-py --user ``` # ð (Basic) Usage These
-are basic function that Trilium's ETAPI provides. Down below are some simple
-example code to use this package. ## ð Initialization If you have a ETAPI
-token, change the `server_url` and `token` to yours. ```python from
+OpenAPI Documentation](#-original-openapi-documentation)  ## ð§ Installation
+```bash python3 -m pip install trilium-py --user ``` ## ð (Basic) Usage
+These are basic function that Trilium's ETAPI provides. Down below are some
+simple example code to use this package. ### ð Initialization If you have a
+ETAPI token, change the `server_url` and `token` to yours. ```python from
 trilium_py.client import ETAPI server_url = 'http://localhost:8080' token =
 'YOUR_TOKEN' ea = ETAPI(server_url, token) ``` If you haven't created ETAPI
 token, you can create one with your password. Please note, you can only see
 this token once, please save it if you want to reuse the token. ```python from
 trilium_py.client import ETAPI server_url = 'http://localhost:8080' password =
 '1234' ea = ETAPI(server_url) token = ea.login(password) print(token) ``` After
 initialization, you can use Trilium ETAPI with python now. The following are
-some examples. ## ð Application Information To start with, you can get the
+some examples. ### ð Application Information To start with, you can get the
 application information like this. ```python print(ea.app_info()) ``` It should
-give you the version of your server application and some extra information. ##
+give you the version of your server application and some extra information. ###
 ð Search note Search note with keyword. ```python res = ea.search_note
 ( search="python", ) for x in res['results']: print(x['noteId'], x['title'])
-``` ## ð­ Create Note You can create a simple note like this. ```python res =
-ea.create_note( parentNoteId="root", title="Simple note 1", type="text",
+``` ### ð­ Create Note You can create a simple note like this. ```python res
+= ea.create_note( parentNoteId="root", title="Simple note 1", type="text",
 content="Simple note example", noteId="note1" ) ``` The `noteId` is not
 mandatory, if not provided, Trilium will generate a random one. You can
-retrieve it in the return. ```python noteId = res['note']['noteId'] ``` ###
+retrieve it in the return. ```python noteId = res['note']['noteId'] ``` ####
 ð¼ï¸ Create Image note Image note is a special kind of note. You can create
 an image note with minimal information like this. The `image_file` refers to
 the path of image. ```python res = ea.create_image_note( parentNoteId="root",
-title="Image note 1", image_file="shield.png", ) ``` ## ð Get note To
+title="Image note 1", image_file="shield.png", ) ``` ### ð Get note To
 retrieve the note's content. ```python ea.get_note_content("note1") ``` You can
-get a note metadata by its id. ```python ea.get_note(note_id) ``` ## ð
+get a note metadata by its id. ```python ea.get_note(note_id) ``` ### ð
 Update note Update note content ```python ea.update_note_content("note1",
 "updated by python") ``` Modify note title ```python ea.patch_note
-( noteId="note1", title="Python client moded", ) ``` ## ðï¸ Delete note
-Simply delete a note by id. ```python ea.delete_note("note1") ``` ## ð Day
+( noteId="note1", title="Python client moded", ) ``` ### ðï¸ Delete note
+Simply delete a note by id. ```python ea.delete_note("note1") ``` ### ð Day
 note You can get the content of a certain date with `get_day_note`. The date
 string should be in format of "%Y-%m-%d", e.g. " 2022-02-25". ```python
 es.get_day_note("2022-02-25") ``` Then set/update a day note with
 `set_day_note`. The content should be a (html) string. ```python
-self.set_day_note(date, new_content) ``` ## ð¤ Export note Export note comes
+self.set_day_note(date, new_content) ``` ### ð¤ Export note Export note comes
 in two formats `html` or `markdown`/`md`. ```python res = ea.export_note
 ( noteId='sK5fn4T6yZRI', format='md', savePath='/home/nate/data/1/test.zip', )
-``` ## ð¾ Create data backup This example will create a database backup file
+``` ### ð¾ Create data backup This example will create a database backup file
 like this `trilium-data/backup/backup-test.db`. ```python res = ea.backup
-("test") ``` # (Advanced Usage) â TODO List With the power of Python, I have
-expanded the basic usage of ETAPI. You can do something with todo list now. ##
+("test") ``` ## (Advanced Usage) â TODO List With the power of Python, I have
+expanded the basic usage of ETAPI. You can do something with todo list now. ###
 Add TODO item You can use `add_todo` to add a TODO item, param is the TODO
-description ```python ea.add_todo("ä¹°æå®å®") ``` ## Check/Uncheck a TODO
+description ```python ea.add_todo("ä¹°æå®å®") ``` ### Check/Uncheck a TODO
 item param is the index of the TODO item ```python ea.todo_check(0)
-ea.todo_uncheck(1) ``` ## Update a TODO item Use `update_todo` to update a TODO
-item description at certain index. ```python ea.update_todo(0,
-"å»ç å¤´æ´ç¹è¯æ¡") ``` ## Delete a TDOO item Remove a TODO item by its
-index. ```python ea.delete_todo(1) ``` ## Move yesterday's unfinished todo to
+ea.todo_uncheck(1) ``` ### Update a TODO item Use `update_todo` to update a
+TODO item description at certain index. ```python ea.update_todo(0,
+"å»ç å¤´æ´ç¹è¯æ¡") ``` ### Delete a TODO item Remove a TODO item by its
+index. ```python ea.delete_todo(1) ``` ### Move yesterday's unfinished todo to
 today As the title suggests, you can move yesterday's unfinished things to
-today. Unfinished todos will be deleted from yesterday's note. ```python
-ea.move_yesterday_unfinished_todo_to_today() ``` # (Advanced Usage) ð Upload
-Markdown files ## Upload single Markdown file with images You can import
-Markdown file with images into Trilium now! Trilium-py will help you to upload
-the images and fix the links for you! ```python res = ea.upload_md_file
-( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ##
+today. Unfinished todo's will be deleted from yesterday's note. ```python
+ea.move_yesterday_unfinished_todo_to_today() ``` ## (Advanced Usage) ð
+Upload Markdown files ### Upload single Markdown file with images You can
+import Markdown file with images into Trilium now! Trilium-py will help you to
+upload the images and fix the links for you! ```python res = ea.upload_md_file
+( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ###
 Bulk upload Markdown files in a folder You can upload a folder with lots of
-Markdown files to Trilium and preserve the folder structure! ### Import from
+Markdown files to Trilium and preserve the folder structure! #### Import from
 VNote Say, upload all the notes from [VNote](https://github.com/vnotex/vnote),
 simply do this: ```python res = ea.upload_md_folder( parentNoteId="root",
 mdFolder="~/data/vnotebook/", ignoreFolder=['vx_notebook', 'vx_recycle_bin',
-'vx_images', '_v_images'], ) ``` ### Import from Joplin Joplin can be imported
+'vx_images', '_v_images'], ) ``` #### Import from Joplin Joplin can be imported
 effortlessly. ```python res = ea.upload_md_folder( parentNoteId="root",
 mdFolder="/home/nate/data/joplin_data/", ignoreFolder=['_resources', ], ) ```
-### Import from Logseq ```python res = ea.upload_md_folder
+#### Import from Logseq ```python res = ea.upload_md_folder
 ( parentNoteId="root", mdFolder="/home/nate/data/logseq_data/", ignoreFolder=
-['assets', 'logseq'], ) ``` ### Import from Obsidian Obsidian has a very unique
-linking system for files. You should use [obsidian-export ](https://github.com/
-zoni/obsidian-export) to convert a Obsidian vault to regular Markdown files.
-Then you should be able to import the note into Trilium with trilium-py.
-Convert it first. ```bash obsidian-export /path/to/your/vault /out ``` Then
-import just like a normal markdown, trilium-py will handle the images for you.
-```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:/data/
-out", ) ``` ### Import from Youdao Note/æéäºç¬è®° Youdao does not provide
-an export feature anymore. Luckily, you can use
+['assets', 'logseq'], ) ``` #### Import from Obsidian Obsidian has a very
+unique linking system for files. You should use [obsidian-export ](https://
+github.com/zoni/obsidian-export) to convert a Obsidian vault to regular
+Markdown files. Then you should be able to import the note into Trilium with
+trilium-py. Convert it first. ```bash obsidian-export /path/to/your/vault /out
+``` Then import just like a normal markdown, trilium-py will handle the images
+for you. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:
+/data/out", ) ``` #### Import from Youdao Note/æéäºç¬è®° Youdao does not
+provide an export feature anymore. Luckily, you can use
 github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
 them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
-home/nate/gitRepo/youdaonote-pull/out/", ) ``` ### Import from Turtl You need
+home/nate/gitRepo/youdaonote-pull/out/", ) ``` #### Import from Turtl You need
 to convert Turtl from json to markdown first. See [turtl-to-markdown](https://
 github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
 Then you can import with trilium-py like this: ```python res =
 ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/gitRepo/turtl-
-to-markdown/out/", ignoreFolder=['_resources'], ) ``` ### Import from other
+to-markdown/out/", ignoreFolder=['_resources'], ) ``` #### Import from other
 markdown software In general, markdown files have variety of standards. You can
 always try import them with ```python res = ea.upload_md_folder
 ( parentNoteId="root", mdFolder="/home/nate/data/your_markdown_files/", ) ```
 If there is any problem, please feel free to create an [issue](https://
 github.com/Nriver/trilium-py/issues/new). ## (Advanced Usage) ð¨ Beautify
 notes Because of the constraints imposed by the library utilized by Trilium,
 imported notes may experience minor formatting problems. These issues include
 an additional line appearing at the end of code blocks, images becoming
 integrated with the note content, and the absence of line breaks between
 headings, resulting in a cramped appearance of the note content. Here is what
 you can do to beautify your note. ### Beautify a note Specify a note id to
-beautify note content. ``` ea.beautify_note('krm8B9JthNfi') ``` ### Beautify a
-note and its child notes ``` ea.beautify_sub_notes('tlPuzU2szLJh') ``` #
-ð ï¸ Develop Install with pip egg link to make package change without
-reinstall. ```python python -m pip install --user -e . ``` # ð Original
-OpenAPI Documentation The original OpenAPI document is [here](https://
-github.com/zadam/trilium/blob/master/src/etapi/etapi.openapi.yaml). You can
-open it with [swagger editor](https://editor.swagger.io/).
+beautify note content. ```python ea.beautify_note('krm8B9JthNfi') ``` ###
+Beautify a note and its child notes ```python ea.beautify_sub_notes
+('tlPuzU2szLJh') ``` ## ð ï¸ Develop Install with pip egg link to make
+package change without reinstall. ```python python -m pip install --user -e .
+``` ## ð Original OpenAPI Documentation The original OpenAPI document is
+[here](https://github.com/zadam/trilium/blob/master/src/etapi/
+etapi.openapi.yaml). You can open it with [swagger editor](https://
+editor.swagger.io/).
```

