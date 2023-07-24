# Comparing `tmp/cubicweb-workorder-0.9.0.tar.gz` & `tmp/cubicweb-workorder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-workorder-0.9.0.tar", last modified: Sun Oct 17 19:37:23 2010, max compression, from Unix
+gzip compressed data, was "cubicweb-workorder-1.0.0.tar", last modified: Mon Jul 24 15:34:33 2023, max compression
```

## Comparing `cubicweb-workorder-0.9.0.tar` & `cubicweb-workorder-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/
--rw-rw-r--   0 syt       (1004) syt       (1004)     2924 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/entities.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     5628 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/setup.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1212 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/views.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/i18n/
--rw-rw-r--   0 syt       (1004) syt       (1004)     3604 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/i18n/fr.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     2927 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/i18n/en.po
--rw-rw-r--   0 syt       (1004) syt       (1004)     1522 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/__pkginfo__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/PKG-INFO
--rw-rw-r--   0 syt       (1004) syt       (1004)      335 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/MANIFEST.in
--rw-rw-r--   0 syt       (1004) syt       (1004)      143 2010-01-27 12:33:55.000000 cubicweb-workorder-0.9.0/__init__.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       45 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/sobjects.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       96 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/README
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/test/
--rw-rw-r--   0 syt       (1004) syt       (1004)     1148 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/test/pytestconf.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      372 2009-06-24 11:42:42.000000 cubicweb-workorder-0.9.0/test/test_workorder.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1106 2008-10-28 14:23:23.000000 cubicweb-workorder-0.9.0/test/realdb_test_workorder.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     2216 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/hooks.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1225 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/schema.py
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/
--rw-rw-r--   0 syt       (1004) syt       (1004)       18 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/requires.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)       10 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/top_level.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)        1 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/dependency_links.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)      624 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/SOURCES.txt
--rw-rw-r--   0 syt       (1004) syt       (1004)      387 2010-10-17 19:37:22.000000 cubicweb-workorder-0.9.0/cubicweb_workorder.egg-info/PKG-INFO
-drwxrwxr-x   0 syt       (1004) syt       (1004)        0 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/migration/
--rw-rw-r--   0 syt       (1004) syt       (1004)     1144 2009-08-18 14:21:56.000000 cubicweb-workorder-0.9.0/migration/0.6.0_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)     1254 2010-01-27 12:33:55.000000 cubicweb-workorder-0.9.0/migration/postcreate.py
--rw-rw-r--   0 syt       (1004) syt       (1004)      176 2010-10-15 09:52:07.000000 cubicweb-workorder-0.9.0/migration/0.9.0_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       33 2010-06-07 11:15:34.000000 cubicweb-workorder-0.9.0/migration/0.6.2_Any.py
--rw-rw-r--   0 syt       (1004) syt       (1004)       59 2010-10-17 19:37:23.000000 cubicweb-workorder-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.146577 cubicweb-workorder-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-24 15:34:33.142577 cubicweb-workorder-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.126577 cubicweb-workorder-1.0.0/cubicweb_workorder/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4415 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2292 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.134577 cubicweb-workorder-1.0.0/cubicweb_workorder/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     3604 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.138577 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.11.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.13.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.6.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.6.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.9.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/cubicweb_workorder/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.130577 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-24 15:34:33.000000 cubicweb-workorder-1.0.0/cubicweb_workorder.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.142577 cubicweb-workorder-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/debian/copyright
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:34:33.146577 cubicweb-workorder-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.142577 cubicweb-workorder-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:34:33.142577 cubicweb-workorder-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     2384 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/test/test_workorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2023-07-24 15:34:12.000000 cubicweb-workorder-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-workorder-0.9.0/entities.py` & `cubicweb-workorder-1.0.0/cubicweb_workorder/entities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,153 @@
 from datetime import date
 
 from cubicweb.entities import AnyEntity, fetch_config
-from cubicweb.entities.adapters import IMileStoneAdapter
-from cubicweb.selectors import is_instance
+from cubicweb.predicates import is_instance
+
+from cubicweb_iprogress.entities import IMileStoneAdapter, IProgressAdapter
+
 
 class Order(AnyEntity):
-    __regid__ = 'Order'
-    fetch_attrs, fetch_order = fetch_config(('title', 'date'))
+    __regid__ = "Order"
+    fetch_attrs, cw_fetch_order = fetch_config(("title", "date"))
 
     def update_progress(self, compute=True):
         """callable only on the server side"""
         if compute:
             workorders = self.split_into
-            self.set_attributes(
+            self.cw_set(
                 budget=sum(wod.budget or 0 for wod in workorders),
                 progress_done=sum(wod.progress_done or 0 for wod in workorders),
-                progress_todo=sum(wod.progress_todo or 0 for wod in workorders))
+                progress_todo=sum(wod.progress_todo or 0 for wod in workorders),
+            )
 
-    # XXX used somewhere? If so must be in an adapter
-    def progress_info(self):
-        return {'estimated': self.budget,
-                'estimatedcorrected': self.budget,
-                'done': self.progress_done,
-                'todo': self.progress_todo,
-                }
 
 class WorkOrder(AnyEntity):
-    __regid__ = 'WorkOrder'
+    __regid__ = "WorkOrder"
 
-    fetch_attrs, fetch_order = fetch_config(('title', 'description_format',
-                                             'description', 'budget',
-                                             'begin_date', 'end_date', 'in_state'))
+    fetch_attrs, cw_fetch_order = fetch_config(
+        (
+            "title",
+            "description_format",
+            "description",
+            "budget",
+            "begin_date",
+            "end_date",
+            "in_state",
+        )
+    )
 
     def dc_title(self):
         return self.title
 
     def dc_long_title(self):
-        return u'%s - %s' % (self.order.dc_title(), self.title)
+        return "%s - %s" % (self.order.dc_title(), self.title)
 
     @property
     def order(self):
         return self.reverse_split_into[0]
 
     def update_progress(self, compute=True):
         """callable only on the server side"""
         for order in self.reverse_split_into:
             order.update_progress(True)
 
 
 class WorkOrderIMileStoneAdapter(IMileStoneAdapter):
-    __select__ = is_instance('WorkOrder')
-    parent_type = 'Order'
+    __select__ = is_instance("WorkOrder")
+    parent_type = "Order"
 
     def get_main_task(self):
         return self.entity.order
 
     def initial_prevision_date(self):
-        """returns the initial expected end of the milestone"""
-        return date.today()
+        """returns the initial expected end of the milestone
+
+        Warning: not taken into accound WorkOrder transition/state.
+        """
+        return self.entity.end_date or date.today()
 
     def eta_date(self):
         """returns expected date of completion based on what remains
         to be done
+
+        Warning: not taken into accound WorkOrder transition/state.
         """
-        return date.today()
+        if not self.entity.end_date or date.today() > self.entity.end_date:
+            return date.today()
+        return self.entity.end_date
 
     def completion_date(self):
         """returns date on which the subtask has been completed"""
         return date.today()
 
     def contractors(self):
         """returns the list of persons supposed to work on this task"""
         return []
 
     def in_progress(self):
-        return self.entity.cw_adapt_to('IWorkflowable').state == u'in progress'
+        return self.entity.cw_adapt_to("IWorkflowable").state == "in progress"
 
     def progress_info(self):
-        return {'estimated': self.entity.budget,
-                'estimatedcorrected': self.entity.budget,
-                'done': self.entity.progress_done,
-                'todo': self.entity.progress_todo,}
+        return {
+            "estimated": self.entity.budget,
+            "estimatedcorrected": self.entity.budget,
+            "done": self.entity.progress_done,
+            "todo": self.entity.progress_todo,
+        }
+
 
 # XXX IMileStone / IProgress inheritance stink
 class WorkOrderProgressAdapter(WorkOrderIMileStoneAdapter):
-    __regid__ = 'IProgress'
-    __select__ = is_instance('WorkOrder')
+    __regid__ = "IProgress"
+    __select__ = is_instance("WorkOrder")
+
 
+class OrderProgressAdapter(IProgressAdapter):
+    __select__ = is_instance("Order")
+
+    def progress_info(self):
+        return {
+            "estimated": self.entity.budget,
+            "estimatedcorrected": self.entity.budget,
+            "done": self.entity.progress_done,
+            "todo": self.entity.progress_todo,
+        }
+
+    def in_progress(self):
+        return True  # FIXME
+
+
+class OrderIMileStoneAdapter(IMileStoneAdapter):
+    __select__ = is_instance("Order")
+
+    def get_main_task(self):
+        return self.entity
+
+    def initial_prevision_date(self):
+        """returns the initial expected end of the milestone"""
+        return date.today()
+
+    def eta_date(self):
+        """returns expected date of completion based on what remains
+        to be done
+        """
+        return date.today()
+
+    def completion_date(self):
+        """returns date on which the subtask has been completed"""
+        return date.today()
+
+    def contractors(self):
+        """returns the list of persons supposed to work on this task"""
+        return []
+
+    def in_progress(self):
+        return self.entity.cw_adapt_to("IWorkflowable").state == "in progress"
+
+    def progress_info(self):
+        return {
+            "estimated": self.entity.budget,
+            "estimatedcorrected": self.entity.budget,
+            "done": self.entity.progress_done,
+            "todo": self.entity.progress_todo,
+        }
```

### Comparing `cubicweb-workorder-0.9.0/i18n/fr.po` & `cubicweb-workorder-1.0.0/cubicweb_workorder/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.9.0/i18n/en.po` & `cubicweb-workorder-1.0.0/cubicweb_workorder/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-workorder-0.9.0/hooks.py` & `cubicweb-workorder-1.0.0/cubicweb_workorder/hooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 """workorder hooks: compute progress"""
 
 __docformat__ = "restructuredtext en"
 
-from cubicweb.selectors import is_instance
+from cubicweb.predicates import is_instance
 from cubicweb.server import hook
 
+WORKORDER_FINAL_STATES = set(("done",))
+
 
 class UpdateProgressOp(hook.DataOperationMixIn, hook.Operation):
     def precommit_event(self):
         for eid, compute in self.get_data():
-            entity = self.session.entity_from_eid(eid)
-            entity.update_progress(compute)
+            if not self.cnx.deleted_in_transaction(eid):
+                entity = self.cnx.entity_from_eid(eid)
+                entity.update_progress(compute)
 
 
 class UpdateProgressOnWorkOrderStatusChange(hook.Hook):
     """when a ticket status change and it's identical to another one, change the
     state of the other one as well
     """
-    __regid__ = 'workorder.progress.status_change'
-    __select__ = hook.Hook.__select__ & is_instance('TrInfo')
-    events = ('after_add_entity',)
+
+    __regid__ = "workorder.progress.status_change"
+    __select__ = hook.Hook.__select__ & is_instance("TrInfo")
+    events = ("after_add_entity",)
 
     def __call__(self):
         trinfo = self.entity
         forentity = trinfo.for_entity
-        if forentity.e_schema == 'WorkOrder' and trinfo.new_state.name == 'done':
-            forentity.set_attributes(progress_done=forentity.budget,
-                                     progress_todo=0)
+        if (
+            forentity.e_schema == "WorkOrder"
+            and trinfo.new_state.name in WORKORDER_FINAL_STATES
+        ):
+            forentity.cw_set(progress_todo=0)
 
 
 class UpdateProgressOnWorkOrderModification(hook.Hook):
-    __regid__ = 'workorder.progress.workorder'
-    __select__ = hook.Hook.__select__ & is_instance('WorkOrder')
-    events = ('before_add_entity', 'before_update_entity', )
+    __regid__ = "workorder.progress.workorder"
+    __select__ = hook.Hook.__select__ & is_instance("WorkOrder")
+    events = (
+        "before_add_entity",
+        "before_update_entity",
+    )
 
     def __call__(self):
         edited = self.entity.cw_edited
-        if 'budget' in edited:
+        if "budget" in edited:
             if self.entity.progress_done is None:
-                edited['progress_done'] = 0
+                edited["progress_done"] = 0
             if self.entity.progress_todo is None:
-                edited['progress_todo'] = edited['budget']
-            UpdateProgressOp.get_instance(self._cw).add_data(
-                (self.entity.eid, False) )
-        elif 'progress_todo' in edited or 'progress_done' in edited:
-            UpdateProgressOp.get_instance(self._cw).add_data(
-                (self.entity.eid, False) )
+                edited["progress_todo"] = edited["budget"]
+            UpdateProgressOp.get_instance(self._cw).add_data((self.entity.eid, True))
+        elif "progress_todo" in edited or "progress_done" in edited:
+            UpdateProgressOp.get_instance(self._cw).add_data((self.entity.eid, False))
 
 
 class UpdateProgressOnSplitIntoChange(hook.Hook):
-    __regid__ = 'workorder.progress.split_into'
-    __select__ = (hook.Hook.__select__
-                  & hook.match_rtype('split_into', frometypes=('Order',)))
-    events = ('after_add_relation', 'after_delete_relation',)
+    __regid__ = "workorder.progress.split_into"
+    __select__ = hook.Hook.__select__ & hook.match_rtype(
+        "split_into", frometypes=("Order",)
+    )
+    events = (
+        "after_add_relation",
+        "after_delete_relation",
+    )
 
     def __call__(self):
-        UpdateProgressOp.get_instance(self._cw).add_data( (self.eidfrom, True) )
-
+        UpdateProgressOp.get_instance(self._cw).add_data((self.eidfrom, True))
```

### Comparing `cubicweb-workorder-0.9.0/migration/0.6.0_Any.py` & `cubicweb-workorder-1.0.0/cubicweb_workorder/migration/0.6.0_Any.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # add attributes
-add_attribute('Order','budget')
-for attr in ('progress_target', 'progress_done', 'progress_todo'):
-    add_attribute('Order', attr)
-    add_attribute('WorkOrder', attr)
+add_attribute("Order", "budget")
+for attr in ("progress_target", "progress_done", "progress_todo"):
+    add_attribute("Order", attr)
+    add_attribute("WorkOrder", attr)
 checkpoint()
 
 from logilab.common.shellutils import ProgressBar
-workorders = rql('Any X WHERE X is WorkOrder', ask_confirm=False)
-bar = ProgressBar(len(workorders), title='Updating progress information ')
+
+workorders = rql("Any X WHERE X is WorkOrder", ask_confirm=False)
+bar = ProgressBar(len(workorders), title="Updating progress information ")
 bar.refresh()
 for entity in workorders.entities():
     entity.update_progress()
     bar.update()
 print
 checkpoint()
 
 # add states
-reserve = rql('Any S WHERE S is State, S name "not started", '
-              'S state_of W, W name "WorkOrder"', ask_confirm=False)[0][0]
-annule = add_state(_(u'canceled'), 'WorkOrder')
-add_transition(_(u'cancel'), 'WorkOrder', (reserve,), annule)
+reserve = rql(
+    'Any S WHERE S is State, S name "not started", ' 'S state_of W, W name "WorkOrder"',
+    ask_confirm=False,
+)[0][0]
+annule = add_state(_("canceled"), "WorkOrder")
+add_transition(_("cancel"), "WorkOrder", (reserve,), annule)
 
-planned = rql('Any S WHERE S is State, S name "planned", '
-              'S state_of W, W name "Order"', ask_confirm=False)[0][0]
-sent = rql('Any S WHERE S is State, S name "sent", '
-           'S state_of W, W name "Order"', ask_confirm=False)[0][0]
-canceled = add_state(_(u'canceled'), 'Order')
-add_transition(_(u'cancel'), 'Order', (planned,sent), canceled)
+planned = rql(
+    'Any S WHERE S is State, S name "planned", ' 'S state_of W, W name "Order"',
+    ask_confirm=False,
+)[0][0]
+sent = rql(
+    'Any S WHERE S is State, S name "sent", ' 'S state_of W, W name "Order"',
+    ask_confirm=False,
+)[0][0]
+canceled = add_state(_("canceled"), "Order")
+add_transition(_("cancel"), "Order", (planned, sent), canceled)
 checkpoint()
```

### Comparing `cubicweb-workorder-0.9.0/migration/postcreate.py` & `cubicweb-workorder-1.0.0/cubicweb_workorder/migration/postcreate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # postcreate script. You could setup a workflow here for example
+from cubicweb import _
 
 # XXX missing correct permissions configuration
 
 # WorkOrder workflow
-wwf = add_workflow(_('default workorder workflow'), 'WorkOrder')
+wwf = add_workflow(_("default workorder workflow"), "WorkOrder")
 
-reserve = wwf.add_state(_(u'not started'), initial=True)
-encours = wwf.add_state(_(u'in progress'))
-attente = wwf.add_state(_(u'client validation'))
-garantie = wwf.add_state(_(u'warranty'))
-recette = wwf.add_state(_(u'validated'))
-annule = wwf.add_state(_(u'canceled'))
-
-wwf.add_transition(_(u'cancel'), (reserve,), annule)
-wwf.add_transition(_(u'start'), (reserve,), encours)
-wwf.add_transition(_(u'done'), (encours,), attente)
-wwf.add_transition(_(u'warrant'), (attente,), garantie)
-wwf.add_transition(_(u'validated'), (attente, garantie), recette)
+reserve = wwf.add_state(_("not started"), initial=True)
+encours = wwf.add_state(_("in progress"))
+attente = wwf.add_state(_("client validation"))
+garantie = wwf.add_state(_("warranty"))
+recette = wwf.add_state(_("validated"))
+annule = wwf.add_state(_("canceled"))
+
+wwf.add_transition(_("cancel"), (reserve,), annule)
+wwf.add_transition(_("start"), (reserve,), encours)
+wwf.add_transition(_("done"), (encours,), attente)
+wwf.add_transition(_("warrant"), (attente,), garantie)
+wwf.add_transition(_("validated"), (attente, garantie), recette)
 
 
 # Order workflow
-owf = add_workflow(_('default order workflow'), 'Order')
+owf = add_workflow(_("default order workflow"), "Order")
 
-planned = owf.add_state(_(u'planned'), initial=True)
-canceled = owf.add_state(_(u'canceled'))
-sent = owf.add_state(_(u'sent'))
-in_progress = owf.add_state(_(u'in progress'))
-done = owf.add_state(_(u'done'))
-owf.add_transition(_(u'cancel'), (planned,sent), canceled)
-owf.add_transition(_(u'send'), (planned,), sent)
-owf.add_transition(_(u'receive'), (sent,), in_progress)
-owf.add_transition(_(u'done'), (in_progress,), done)
+planned = owf.add_state(_("planned"), initial=True)
+canceled = owf.add_state(_("canceled"))
+sent = owf.add_state(_("sent"))
+in_progress = owf.add_state(_("in progress"))
+done = owf.add_state(_("done"))
+owf.add_transition(_("cancel"), (planned, sent), canceled)
+owf.add_transition(_("send"), (planned,), sent)
+owf.add_transition(_("receive"), (sent,), in_progress)
+owf.add_transition(_("done"), (in_progress,), done)
```

