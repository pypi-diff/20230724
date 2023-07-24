# Comparing `tmp/cubicweb-calendar-0.9.0.tar.gz` & `tmp/cubicweb-calendar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-calendar-0.9.0.tar", last modified: Tue Nov 15 17:22:14 2016, max compression
+gzip compressed data, was "cubicweb-calendar-1.0.0.tar", last modified: Mon Jul 24 15:15:54 2023, max compression
```

## Comparing `cubicweb-calendar-0.9.0.tar` & `cubicweb-calendar-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,49 @@
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/
--rw-r--r--   0 narval     (111) narval     (116)     1995 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/schema.py
--rw-r--r--   0 narval     (111) narval     (116)      335 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/MANIFEST.in
--rw-rw-r--   0 narval     (111) narval     (116)       59 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/setup.cfg
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/views/
--rw-r--r--   0 narval     (111) narval     (116)      935 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/secondaries.py
--rw-r--r--   0 narval     (111) narval     (116)     3763 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     2207 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/primaries.py
--rw-r--r--   0 narval     (111) narval     (116)     5669 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/main.py
--rw-r--r--   0 narval     (111) narval     (116)      299 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/views/facets.py
--rw-r--r--   0 narval     (111) narval     (116)      200 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/README
--rw-r--r--   0 narval     (111) narval     (116)     1491 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/__pkginfo__.py
--rw-rw-r--   0 narval     (111) narval     (116)      496 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/PKG-INFO
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/test/
--rw-r--r--   0 narval     (111) narval     (116)      877 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/test/test_calendar.py
--rw-r--r--   0 narval     (111) narval     (116)      238 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     6411 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/setup.py
--rw-r--r--   0 narval     (111) narval     (116)     7668 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/entities.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/i18n/
--rw-r--r--   0 narval     (111) narval     (116)     4689 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/es.po
--rw-r--r--   0 narval     (111) narval     (116)     6727 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/fr.po
--rw-r--r--   0 narval     (111) narval     (116)     5695 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/i18n/en.po
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/data/
--rw-r--r--   0 narval     (111) narval     (116)      616 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/data/office-calendar.png
--rw-r--r--   0 narval     (111) narval     (116)     3831 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/data/cubes.calendar.css
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/
--rw-rw-r--   0 narval     (111) narval     (116)        1 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/top_level.txt
--rw-rw-r--   0 narval     (111) narval     (116)      519 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/SOURCES.txt
--rw-rw-r--   0 narval     (111) narval     (116)        1 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/dependency_links.txt
--rw-rw-r--   0 narval     (111) narval     (116)      496 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/PKG-INFO
--rw-rw-r--   0 narval     (111) narval     (116)       19 2016-11-15 17:22:11.000000 cubicweb-calendar-0.9.0/cubicweb_calendar.egg-info/requires.txt
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-11-15 17:22:14.000000 cubicweb-calendar-0.9.0/migration/
--rw-r--r--   0 narval     (111) narval     (116)     1932 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/migration/postcreate.py
--rw-r--r--   0 narval     (111) narval     (116)     1356 2016-11-15 17:19:06.000000 cubicweb-calendar-0.9.0/migration/0.4.0_Any.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.099796 cubicweb-calendar-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-24 15:15:54.099796 cubicweb-calendar-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.067796 cubicweb-calendar-1.0.0/cubicweb_calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.079796 cubicweb-calendar-1.0.0/cubicweb_calendar/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/data/cubes.calendar.css
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/data/office-calendar.png
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.079796 cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     6236 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     7332 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.079796 cubicweb-calendar-1.0.0/cubicweb_calendar/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/migration/0.11.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/migration/0.4.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.079796 cubicweb-calendar-1.0.0/cubicweb_calendar/views/
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/views/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/views/primaries.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/cubicweb_calendar/views/secondaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.071796 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 15:15:53.000000 cubicweb-calendar-1.0.0/cubicweb_calendar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.095796 cubicweb-calendar-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/debian/copyright
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 15:15:54.099796 cubicweb-calendar-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.095796 cubicweb-calendar-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 15:15:54.095796 cubicweb-calendar-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/test/test_calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6038 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/test/unittest_calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-07-24 15:15:24.000000 cubicweb-calendar-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-calendar-0.9.0/schema.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # cube's specific schema
-from yams.buildobjs import EntityType, SubjectRelation, String, Datetime, Time
+from yams.buildobjs import EntityType, SubjectRelation, String, Datetime, Boolean
 from yams.constraints import BoundaryConstraint, Attribute
 from cubicweb.schema import WorkflowableEntityType
 
-_ = unicode
+from cubicweb import _
+
 
 class Calendar(EntityType):
     """see projman"""
     title = String(required=True, unique=True, maxsize=64)
     weekdays = SubjectRelation('WeekDay', cardinality='**')
     days = SubjectRelation('Recurrentday', cardinality='**')
-    periods = SubjectRelation('Timeperiod', cardinality = '*1', composite='subject')
+    periods = SubjectRelation('Timeperiod', cardinality='*1', composite='subject')
     day_types = SubjectRelation('Daytype', cardinality='**')
     inherits = SubjectRelation('Calendar', cardinality='?*')
 
 
 class Calendaruse(EntityType):
     """see projman"""
     start = Datetime()
@@ -23,14 +24,16 @@
 
 
 class Daytype(EntityType):
     """see projman"""
     title = String(required=True, maxsize=32, internationalizable=True)
     type = String(vocabulary=(_('dt_working'), _('dt_nonworking'),
                               _('dt_working_am'), _('dt_working_pm')))
+    display_in_user_request = Boolean(required=True, default=False)
+
 
 class Timeperiod(WorkflowableEntityType):
     """ """
     start = Datetime(required=True)
     stop = Datetime(required=True,
                     constraints=[BoundaryConstraint('>=', Attribute('start'))],
                     description=_('last day of the timeperiod'))
```

### Comparing `cubicweb-calendar-0.9.0/views/secondaries.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/views/secondaries.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from logilab.mtconverter import xml_escape
 
-from cubicweb.view import EntityView
 from cubicweb.predicates import is_instance
-from cubicweb.web.views import baseviews
+from cubicweb_web.views import baseviews
 
 # out of context  ####################################################################
 
 
 class RecurrentDayOutOfContext(baseviews.OutOfContextView):
     __select__ = is_instance('Recurrentday')
 
     def cell_call(self, row, col):
-        entity = self.cw_rset.get_entity(row,col)
+        entity = self.cw_rset.get_entity(row, col)
         self.w(u'<a href="%s">' % xml_escape(entity.absolute_url(vid='edition')))
         self.wdata(entity.dc_long_title())
         self.w(u'</a>')
 
+
 class TimePeriodOutOfContext(baseviews.OutOfContextView):
     __select__ = is_instance('Timeperiod')
 
     def cell_call(self, row, col):
-        entity = self.cw_rset.get_entity(row,col)
+        entity = self.cw_rset.get_entity(row, col)
         self.w(u'<a href="%s">' % xml_escape(entity.absolute_url(vid='edition')))
         self.wdata(entity.dc_long_title())
         self.w(u'</a>')
-
-
```

### Comparing `cubicweb-calendar-0.9.0/views/__init__.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/views/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """template-specific forms/views/actions/components"""
 import datetime
+import six
 
 from logilab.common.date import todate, last_day
 
 from cubicweb import target
-from cubicweb.view import EntityAdapter
 from cubicweb.predicates import is_instance
-from cubicweb.web import uicfg, action
-from cubicweb.web.views import ibreadcrumbs
+from cubicweb_web import action
+from cubicweb_web.views import uicfg, ibreadcrumbs, calendar
 
-_ = unicode
+from cubicweb import _
 
 _afs = uicfg.autoform_section
 _afs.tag_object_of(('*', 'periods', 'Timeperiod'), 'main', 'attributes')
 _afs.tag_object_of(('*', 'periods', 'Timeperiod'), 'muledit', 'attributes')
 
 _pvs = uicfg.primaryview_section
 _pvs.tag_subject_of(('Calendar', 'weekdays', '*'), 'hidden')
@@ -29,48 +29,49 @@
 _abaa.tag_object_of(('Calendar', 'inherits', '*'), True)
 _abaa.tag_object_of(('*', 'for_calendar', 'Calendar'), True)
 _abaa.tag_object_of(('*', 'for_period', 'Timeperiod'), True)
 
 
 def daytype_choices(form, field, limit=None):
     req = form._cw
-    # FIXME: holidays should have their own type and we shuold not rely
-    #        on application-defined vocabulary
+    rql = u'Any D,DT WHERE D is Daytype, D title DT'
     if 'holidays' in req.form:
-        rset = req.execute(u'Any D,DT WHERE D is Daytype, D title DT, '
-                           u'D title IN ("journée de congés", "matinée de congés", "après-midi de congés", "non travaillé", "journée de mat-paternité")')
-    else:
-        rset = req.execute(u'Any D,DT WHERE D is Daytype, D title DT')
-    return [(e.view('combobox'), unicode(e.eid)) for e in rset.entities()]
+        rql += ', D display_in_user_request TRUE'
+    rset = req.execute(rql)
+    return [(e.view('combobox'), six.text_type(e.eid)) for e in rset.entities()]
+
 
 _affk = uicfg.autoform_field_kwargs
 _affk.tag_subject_of(('Timeperiod', 'day_type', '*'),
                      {'choices': daytype_choices})
 
+
 def _parse_datestr(datestr):
     if datestr.lower() == 'today':
         return todate(datetime.datetime.today())
     if len(datestr) == 4:
         datestr += '0101'
     elif len(datestr) == 6:
         datestr += '01'
     return todate(datetime.datetime.strptime(datestr, '%Y%m%d'))
 
+
 def get_date_range_from_reqform(reqform, autoset_lastday=False):
     lastday = None
     if 'firstday' in reqform:
         firstday = _parse_datestr(reqform['firstday'])
         if 'lastday' in reqform:
             lastday = _parse_datestr(reqform['lastday'])
     else:
         firstday = datetime.date.today()
     if lastday is None and autoset_lastday:
         lastday = last_day(firstday)
     return todate(firstday), lastday
 
+
 class AskOffDays(action.LinkToEntityAction):
     __regid__ = 'ask-off-days'
     title = _('ask_off_days')
     __select__ = action.LinkToEntityAction.__select__ & is_instance('Calendar')
     target_etype = 'Timeperiod'
     role = 'subject'
     rtype = 'periods'
@@ -78,23 +79,27 @@
     def url(self):
         ttype = self.target_etype
         entity = self.cw_rset.get_entity(self.cw_row or 0, self.cw_col or 0)
         linkto = '%s:%s:%s' % (self.rtype, entity.eid, target(self))
         return self._cw.build_url('add/%s' % ttype, __linkto=linkto,
                                   __redirectpath='/', holidays=1)
 
-class TimeperiodICalendarable(EntityAdapter):
-    __regid__ = 'ICalendarable'
+
+class TimeperiodICalendarable(calendar.ICalendarableAdapter):
     __select__ = is_instance('Timeperiod')
+
     @property
     def start(self):
         return self.entity.start
+
     @property
     def stop(self):
         return self.entity.stop
 
+
 class CalendarIBreadCrumbsAdapter(ibreadcrumbs.IBreadCrumbsAdapter):
     __select__ = is_instance('Calendar')
+
     def parent_entity(self):
         parents = self.entity.inherits
         if parents:
             return parents[0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cubicweb-calendar-0.9.0/views/primaries.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/views/primaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from cubicweb import _
 from cubicweb.predicates import is_instance
-from cubicweb.web.views import primary
+from cubicweb_web.views import primary
 from cubicweb.uilib import toggle_link
 
 # calendar  ######################################################################
 
+
 class PrimaryCalendar(primary.PrimaryView):
     __select__ = is_instance('Calendar')
 
     def render_entity_attributes(self, entity):
         entity.view('user_calendar', w=self.w)
         self._show_periods(entity)
         self._show_recurrent_days(entity)
```

### Comparing `cubicweb-calendar-0.9.0/views/main.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/views/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from datetime import timedelta, date as pydate, datetime
+from datetime import timedelta, date as pydate
 
 from logilab.mtconverter import xml_escape
-from logilab.common.date import (date_range, first_day, last_day,
+from logilab.common.date import (date_range, first_day,
                                  previous_month, next_month)
 
-from cubicweb.schema import display_name
-from cubicweb.view import EntityView
+from cubicweb_web.view import EntityView
 from cubicweb.predicates import is_instance
-from cubicweb.web.views.calendar import CalendarItemView, OneMonthCal
 
-from cubes.calendar import NON_WORKING, WORKING, WORKING_AM, WORKING_PM
-from cubes.calendar.views import get_date_range_from_reqform
+from cubicweb_calendar import NON_WORKING, WORKING, WORKING_AM, WORKING_PM
+from cubicweb_calendar.views import get_date_range_from_reqform
 
 CALENDARS_PAGE = u"""<table class="bigCalendars">
 <tr><td class="calendar">%s</td></tr>
 </table>
 """
 
+
 class EuserCalendar(EntityView):
     __select__ = is_instance('Calendar',)
     __regid__ = 'user_calendar'
 
     def cell_call(self, row, col):
         self._cw.add_css('cubes.calendar.css')
         entity = self.cw_rset.get_entity(row, col)
-        _today = pydate.today()
         firstday, lastday = get_date_range_from_reqform(self._cw.form,
                                                         autoset_lastday=True)
         firstday = first_day(firstday)
         # make calendar
         caption = '%s %s' % (self._cw._(firstday.strftime('%B').lower()), firstday.year)
-        prevurl, nexturl = self._prevnext_links(entity,firstday)
+        prevurl, nexturl = self._prevnext_links(entity, firstday)
         prevlink = '<a href="%s">&lt;&lt;</a>' % xml_escape(prevurl)
         nextlink = '<a href="%s">&gt;&gt;</a>' % xml_escape(nexturl)
         self.w(u'<table id="ctid%s" class="userCal">'
                u'<tr><th class="prev">%s</th>'
                u'<th class="calTitle" colspan="6"><span>%s</span></th>'
                u'<th class="next">%s</th></tr>'
                u'<tr><th>&nbsp;</th><th>L</th><th>M</th><th>M</th><th>J</th><th>V</th><th>S</th><th>D</th></tr>'
@@ -44,15 +42,15 @@
         stop = lastday + timedelta(7 - lastday.weekday())
         celldatas = {}
         for date, dtype_eid, state in entity.get_days_type(firstday, lastday):
             dtype = self._cw.entity_from_eid(dtype_eid)
             celldatas[date] = (dtype, state)
         # build cells
         for curdate in date_range(start, stop):
-            if curdate == start or curdate.weekday() == 0: # sunday
+            if curdate == start or curdate.weekday() == 0:  # sunday
                 self.w(u'<tr>')
                 self.w(u'<td class="week">%s<br/> %d</td>' % (self._cw._('week'), curdate.isocalendar()[1]))
             self._build_calendar_cell(curdate, celldatas, firstday)
             if curdate.weekday() == 6:
                 self.w(u'</tr>')
         self.w(u'</table>')
 
@@ -70,15 +68,14 @@
 
     def _build_calendar_cell(self, curdate, celldatas, firstday):
         if curdate.month != firstday.month:
             self.w(u'<td class="outofrange"></td>')
         else:
             daytype, daytype_state = celldatas[curdate]
             stickers = self._cw._(daytype.type)
-            pending = self._cw._('pending')
 
             klasses = []
             am_sticker = u''
             pm_sticker = u''
             _today = pydate.today()
             pending_suffix = '_pending' if daytype_state == 'pending' else ''
             if curdate == _today:
@@ -92,24 +89,31 @@
                 am_sticker = self._cw._(WORKING_AM)
                 pm_sticker = daytype.title
             elif daytype.type == WORKING_PM:
                 klasses.append(daytype.type + pending_suffix)
                 am_sticker = daytype.title
                 pm_sticker = self._cw._(WORKING_PM)
             else:
-                self.error('Unknown daytype class %s', klass)
-            am_cell ='<tr><td class="am"><div class="mday">am</div><div class="stickers">%s</div></td></tr>\n' % am_sticker
-            pm_cell ='<tr><td class="pm"><div class="mday">pm</div><div class="stickers">%s</div></td></tr>\n' % pm_sticker
+                self.error('Unknown daytype class')
+            am_cell = (
+                '<tr><td class="am"><div class="mday">am</div>'
+                '<div class="stickers">%s</div></td></tr>\n'
+            ) % am_sticker
+            pm_cell = (
+                '<tr><td class="pm"><div class="mday">pm</div>'
+                '<div class="stickers">%s</div></td></tr>\n'
+            ) % pm_sticker
             cellcontent = u'<table class="caldata">'
-            cellcontent +='<tr><td class="caldate">%s</td></tr>%s %s</table>' % (curdate.day,  am_cell, pm_cell)
-            self.w(u'<td class="%s" title="%s">%s</td>' %(' '.join(klasses), xml_escape(stickers),  cellcontent))
+            cellcontent += '<tr><td class="caldate">%s</td></tr>%s %s</table>' % (curdate.day,  am_cell, pm_cell)
+            self.w(u'<td class="%s" title="%s">%s</td>' % (' '.join(klasses), xml_escape(stickers),  cellcontent))
 
 
 class TimeperiodCalendarItemView(EntityView):
     __regid__ = 'calendaritem'
     __select__ = is_instance('Timeperiod',)
+
     def cell_call(self, row, col):
         entity = self.cw_rset.complete_entity(row, col)
         day_types = u' '.join(self._cw._(dt.type) for dt in entity.day_type)
         state = entity.cw_adapt_to('IWorkflowable').printable_state
         self.w(xml_escape(u'%s : %s (%s)' % (entity.from_calendar.title,
                                              day_types, state)))
```

### Comparing `cubicweb-calendar-0.9.0/test/test_calendar.py` & `cubicweb-calendar-1.0.0/test/test_calendar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from random import randint
 from datetime import timedelta
 
 from cubicweb.devtools.fill import ValueGenerator
-from cubicweb.devtools.testlib import AutomaticWebTest
+from cubicweb_web.devtools.testlib import AutomaticWebTest
+
 
 class MyValueGenerator(ValueGenerator):
     def generate_Calendaruse_stop(self, entity, index):
         return entity.start + timedelta(days=randint(1, 10))
     generate_Timeperiod_stop = generate_Calendaruse_stop
 
+
 class AutomaticWebTest(AutomaticWebTest):
     no_auto_populate = ('Daytype', 'WeekDay', 'Calendar', 'Calendaruse')
     ignored_relations = set(('use_calendar',))
 
     def to_test_etypes(self):
         return set(('Calendar', 'Calendaruse', 'Daytype',
                     'Timeperiod', 'WeekDay', 'Recurrentday',
                     'CWUser'))
 
     def list_startup_views(self):
         return ()
 
+
 if __name__ == '__main__':
-    from logilab.common.testlib import unittest_main
-    unittest_main()
+    import unittest
+    unittest.main()
```

### Comparing `cubicweb-calendar-0.9.0/entities.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from datetime import timedelta
 
 from logilab.common.date import date_range, todate, todatetime
 
 from cubicweb.entities import AnyEntity, fetch_config
 
-from cubes.calendar import NON_WORKING, WORKING, WORKING_AM, WORKING_PM
+from cubicweb_calendar import NON_WORKING, WORKING, WORKING_AM, WORKING_PM
 
-class BadCalendar(ValueError): pass
 
-def intersect(a,b):
-    c = (max(a[0],b[0]), min(a[1], b[1]))
+class BadCalendar(ValueError):
+    pass
+
+
+def intersect(a, b):
+    c = (max(a[0], b[0]), min(a[1], b[1]))
     return c[0] <= c[1]
 
+
 def use_class_cache(cachename, cachepart):
     def cached(func):
         def wrapper(self, *args):
-            cache = getattr(self.__class__, cachename).setdefault(cachepart,{})
+            cache = getattr(self.__class__, cachename).setdefault(cachepart, {})
             cachekey = (self.eid,) + args
             try:
                 res = cache[cachekey]
             except KeyError:
                 res = func(self, *args)
                 cache[cachekey] = res
             return res
         return wrapper
     return cached
 
+
 class Timeperiod(AnyEntity):
     __regid__ = 'Timeperiod'
     fetch_attrs, cw_fetch_order = fetch_config(('start', 'stop'))
     conges_days = [u'conges_journee', u'conges_matin', u'conges_apresmidi']
 
     def dc_title(self):
         return u'%s-%s' % (self._cw.format_date(self.start),
@@ -89,56 +94,56 @@
                         else:
                             raise BadCalendar('bad calendar definition, '
                                               'missing week days '
                                               'in root calendar for %s'
                                               % self.eid)
             cache[key] = value
 
-    @use_class_cache('daytype_cache','periods')
+    @use_class_cache('daytype_cache', 'periods')
     def _get_timeperiods(self):
         rql = ('Any PA,PO,D,SN WHERE C eid %(c)s, C periods P, P day_type D, '
                'P start PA, P stop PO, P in_state S, S name SN')
         rset = self._cw.execute(rql, {'c': self.eid})
         return tuple(rset)
 
-    @use_class_cache('daytype_cache','recweek')
+    @use_class_cache('daytype_cache', 'recweek')
     def _get_rec_weekdays(self):
         # recurrent days
         rql = 'Any D,DM WHERE C eid %(c)s, C days R, R day_month DM, R day_type D'
         rset = self._cw.execute(rql, {'c': self.eid})
         rec_days = dict((row[1], row[0]) for row in rset)
         # week days
         DAYS = [u'monday', u'tuesday', u'wednesday', u'thursday', u'friday', u'saturday', u'sunday']
         rql = 'Any D,W WHERE C eid %(c)s, C weekdays R, R day_of_week W, R day_type D'
         rset = self._cw.execute(rql, {'c': self.eid})
         week_days = dict((DAYS.index(day), eid) for eid, day in rset)
         return rec_days, week_days
 
-    @use_class_cache('daytype_cache','days_type')
+    @use_class_cache('daytype_cache', 'days_type')
     def _get_days_type(self, start, stop):
         """return [(cal_eid, date, day_type_eid, state), ...]
         with state in ('pending', 'validated')
         """
         day_types = []
         cache = self.daytype_cache.setdefault('cal_date', {})
-        stop += timedelta(days=1) # upper bound excluded by date_range
+        stop += timedelta(days=1)  # upper bound excluded by date_range
         for date in date_range(start, stop):
             key = (self.eid, todate(date))
             if key not in cache:
                 for hole in date_range(date, stop):
                     if (self.eid, hole) in cache:
                         break
                 self._fill_cache(cache, date, hole)
             day_types.append(cache[key])
         return day_types
 
     def _get_daytype_from_titles(self, dtypes):
         """map a set of titles to a set of eids"""
         assert isinstance(dtypes, frozenset), 'dtypes should be a frozenset'
-        cache = self.daytype_cache.setdefault('day_title',{})
+        cache = self.daytype_cache.setdefault('day_title', {})
         if dtypes not in cache:
             types = tuple(dtypes)
             if len(types) == 1:
                 rset = self._cw.execute('Any D WHERE D is Daytype, D title %(title)s',
                                         {'title': types[0]})
             else:
                 rset = self._cw.execute('Any D WHERE D is Daytype, D title IN %s'
@@ -151,52 +156,56 @@
         date varying from start to stop"""
         days_type = self._get_days_type(start, stop)
         if dtypes is None:
             return [item[1:] for item in days_type]
         dtype_eids = self._get_daytype_from_titles(frozenset(dtypes))
         return [item[1:] for item in days_type if item[2] in dtype_eids]
 
+
 class Daytype(AnyEntity):
     __regid__ = 'Daytype'
     fetch_attrs, cw_fetch_order = fetch_config(('title', 'type'))
     worktime_definitions = {NON_WORKING: 0.,
                             WORKING: 1.,
                             WORKING_AM: 0.5,
-                            WORKING_PM: 0.5,}
+                            WORKING_PM: 0.5, }
+
     @property
     def expected_worktime(self):
         return self.worktime_definitions[self.type]
 
     @property
     def day_worked(self):
         return self.type != NON_WORKING
 
+
 class CalendarUse(AnyEntity):
     __regid__ = 'Calendaruse'
     fetch_attrs, cw_fetch_order = fetch_config(('start', 'stop'))
 
     @property
     def calendar(self):
         return self.use_calendar[0]
 
+
 class RecurrentDay(AnyEntity):
     __regid__ = 'Recurrentday'
     fetch_attrs, cw_fetch_order = fetch_config(('day_month', 'day_type'))
 
     def dc_title(self):
         return self._cw._(self.day_month)
 
     def dc_long_title(self):
         day_types = u' '.join(dt.title for dt in self.day_type)
         return u'%s : %s' % (self.dc_title(), day_types)
 
+
 class WeekDay(AnyEntity):
     __regid__ = 'WeekDay'
     fetch_attrs, cw_fetch_order = fetch_config(('day_of_week', 'day_type'))
 
     def dc_title(self):
         return self._cw._(self.day_of_week)
 
     def dc_long_title(self):
         day_types = u' '.join(dt.title for dt in self.day_type)
         return u'%s : %s' % (self.dc_title(), day_types)
-
```

### Comparing `cubicweb-calendar-0.9.0/i18n/es.po` & `cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/es.po`

 * *Files 7% similar despite different names*

```diff
@@ -61,29 +61,47 @@
 
 msgid "Recurrentday_plural"
 msgstr ""
 
 msgid "This Calendar"
 msgstr ""
 
+msgid "This Calendar:"
+msgstr ""
+
 msgid "This Calendaruse"
 msgstr ""
 
+msgid "This Calendaruse:"
+msgstr ""
+
 msgid "This Daytype"
 msgstr ""
 
+msgid "This Daytype:"
+msgstr ""
+
 msgid "This Recurrentday"
 msgstr ""
 
+msgid "This Recurrentday:"
+msgstr ""
+
 msgid "This Timeperiod"
 msgstr ""
 
+msgid "This Timeperiod:"
+msgstr ""
+
 msgid "This WeekDay"
 msgstr ""
 
+msgid "This WeekDay:"
+msgstr ""
+
 msgid "Timeperiod"
 msgstr ""
 
 msgid "Timeperiod_plural"
 msgstr ""
 
 msgid "Week days"
@@ -109,18 +127,33 @@
 
 msgid "add Calendar periods Timeperiod subject"
 msgstr ""
 
 msgid "add Calendar weekdays WeekDay subject"
 msgstr ""
 
-msgid "ask_off_days"
+msgid "add a Calendar"
+msgstr ""
+
+msgid "add a Calendaruse"
 msgstr ""
 
-msgid "calendar (one month)"
+msgid "add a Daytype"
+msgstr ""
+
+msgid "add a Recurrentday"
+msgstr ""
+
+msgid "add a Timeperiod"
+msgstr ""
+
+msgid "add a WeekDay"
+msgstr ""
+
+msgid "ask_off_days"
 msgstr ""
 
 msgid "creating Calendar (Calendar %(linkto)s inherits Calendar)"
 msgstr ""
 
 msgid "creating Calendar (Calendar inherits Calendar %(linkto)s)"
 msgstr ""
@@ -199,14 +232,21 @@
 msgid "days_object"
 msgstr ""
 
 msgctxt "Recurrentday"
 msgid "days_object"
 msgstr ""
 
+msgid "display_in_user_request"
+msgstr ""
+
+msgctxt "Daytype"
+msgid "display_in_user_request"
+msgstr ""
+
 msgid "dt_nonworking"
 msgstr ""
 
 msgid "dt_working"
 msgstr ""
 
 msgid "dt_working_am"
@@ -237,14 +277,17 @@
 msgctxt "Calendar"
 msgid "inherits_object"
 msgstr ""
 
 msgid "last day of the timeperiod"
 msgstr ""
 
+msgid "mm-dd"
+msgstr ""
+
 msgid "monday"
 msgstr ""
 
 msgid "pending"
 msgstr ""
 
 msgid "periods"
```

### Comparing `cubicweb-calendar-0.9.0/i18n/fr.po` & `cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -62,29 +62,47 @@
 
 msgid "Recurrentday_plural"
 msgstr "Journées récurrentes"
 
 msgid "This Calendar"
 msgstr "Ce calendrier"
 
+msgid "This Calendar:"
+msgstr ""
+
 msgid "This Calendaruse"
 msgstr "Cette utilisation de calendrier"
 
+msgid "This Calendaruse:"
+msgstr ""
+
 msgid "This Daytype"
 msgstr "Ce type de journée"
 
+msgid "This Daytype:"
+msgstr ""
+
 msgid "This Recurrentday"
 msgstr "Ce jour récurrent"
 
+msgid "This Recurrentday:"
+msgstr ""
+
 msgid "This Timeperiod"
 msgstr "Cette période"
 
+msgid "This Timeperiod:"
+msgstr ""
+
 msgid "This WeekDay"
 msgstr "Ce jour de la semaine"
 
+msgid "This WeekDay:"
+msgstr ""
+
 msgid "Timeperiod"
 msgstr "Période"
 
 msgid "Timeperiod_plural"
 msgstr "Périodes"
 
 msgid "Week days"
@@ -111,20 +129,35 @@
 
 msgid "add Calendar periods Timeperiod subject"
 msgstr "Période"
 
 msgid "add Calendar weekdays WeekDay subject"
 msgstr "jour de semaine"
 
+msgid "add a Calendar"
+msgstr ""
+
+msgid "add a Calendaruse"
+msgstr ""
+
+msgid "add a Daytype"
+msgstr ""
+
+msgid "add a Recurrentday"
+msgstr ""
+
+msgid "add a Timeperiod"
+msgstr ""
+
+msgid "add a WeekDay"
+msgstr ""
+
 msgid "ask_off_days"
 msgstr "demander des jours de congés"
 
-msgid "calendar (one month)"
-msgstr "calendrier mensuel"
-
 msgid "creating Calendar (Calendar %(linkto)s inherits Calendar)"
 msgstr "création d'un calendrier parent de %(linkto)s"
 
 msgid "creating Calendar (Calendar inherits Calendar %(linkto)s)"
 msgstr "création d'un calendrier héritant de %(linkto)s"
 
 msgid "creating Daytype (Calendar %(linkto)s day_types Daytype)"
@@ -201,14 +234,21 @@
 msgid "days_object"
 msgstr "journée récurrente utilisée par"
 
 msgctxt "Recurrentday"
 msgid "days_object"
 msgstr "journée récurrente utilisée par"
 
+msgid "display_in_user_request"
+msgstr "affiché quand l'utilisateur demande des congés"
+
+msgctxt "Daytype"
+msgid "display_in_user_request"
+msgstr ""
+
 msgid "dt_nonworking"
 msgstr "journée non travaillée"
 
 msgid "dt_working"
 msgstr "journée de travail"
 
 msgid "dt_working_am"
@@ -239,14 +279,17 @@
 msgctxt "Calendar"
 msgid "inherits_object"
 msgstr "hérité par"
 
 msgid "last day of the timeperiod"
 msgstr "dernier jour (inclus) de la période"
 
+msgid "mm-dd"
+msgstr ""
+
 msgid "monday"
 msgstr "lundi"
 
 msgid "pending"
 msgstr "en attente"
 
 msgid "periods"
@@ -347,7 +390,10 @@
 
 msgid "weekdays_object"
 msgstr "jour de semaine de"
 
 msgctxt "WeekDay"
 msgid "weekdays_object"
 msgstr "jour de semaine de"
+
+#~ msgid "calendar (one month)"
+#~ msgstr "calendrier mensuel"
```

### Comparing `cubicweb-calendar-0.9.0/i18n/en.po` & `cubicweb-calendar-1.0.0/cubicweb_calendar/i18n/en.po`

 * *Files 2% similar despite different names*

```diff
@@ -62,29 +62,47 @@
 
 msgid "Recurrentday_plural"
 msgstr "Recurrent days"
 
 msgid "This Calendar"
 msgstr "This calendar"
 
+msgid "This Calendar:"
+msgstr ""
+
 msgid "This Calendaruse"
 msgstr "This calendar use"
 
+msgid "This Calendaruse:"
+msgstr ""
+
 msgid "This Daytype"
 msgstr "This day type"
 
+msgid "This Daytype:"
+msgstr ""
+
 msgid "This Recurrentday"
 msgstr "This recurrent day"
 
+msgid "This Recurrentday:"
+msgstr ""
+
 msgid "This Timeperiod"
 msgstr "This time period"
 
+msgid "This Timeperiod:"
+msgstr ""
+
 msgid "This WeekDay"
 msgstr ""
 
+msgid "This WeekDay:"
+msgstr ""
+
 msgid "Timeperiod"
 msgstr "Time period"
 
 msgid "Timeperiod_plural"
 msgstr "Timeperiods"
 
 msgid "Week days"
@@ -111,18 +129,33 @@
 
 msgid "add Calendar periods Timeperiod subject"
 msgstr "time period"
 
 msgid "add Calendar weekdays WeekDay subject"
 msgstr ""
 
-msgid "ask_off_days"
+msgid "add a Calendar"
+msgstr ""
+
+msgid "add a Calendaruse"
 msgstr ""
 
-msgid "calendar (one month)"
+msgid "add a Daytype"
+msgstr ""
+
+msgid "add a Recurrentday"
+msgstr ""
+
+msgid "add a Timeperiod"
+msgstr ""
+
+msgid "add a WeekDay"
+msgstr ""
+
+msgid "ask_off_days"
 msgstr ""
 
 msgid "creating Calendar (Calendar %(linkto)s inherits Calendar)"
 msgstr "creating child calendar of %(linkto)s"
 
 msgid "creating Calendar (Calendar inherits Calendar %(linkto)s)"
 msgstr "creating calendar inheriting of %(linkto)s"
@@ -201,14 +234,21 @@
 msgid "days_object"
 msgstr "recurrent day of"
 
 msgctxt "Recurrentday"
 msgid "days_object"
 msgstr "recurrent day of"
 
+msgid "display_in_user_request"
+msgstr "Display when user ask off days"
+
+msgctxt "Daytype"
+msgid "display_in_user_request"
+msgstr ""
+
 msgid "dt_nonworking"
 msgstr "non working day"
 
 msgid "dt_working"
 msgstr "working day"
 
 msgid "dt_working_am"
@@ -239,14 +279,17 @@
 msgctxt "Calendar"
 msgid "inherits_object"
 msgstr "base calendar of"
 
 msgid "last day of the timeperiod"
 msgstr ""
 
+msgid "mm-dd"
+msgstr ""
+
 msgid "monday"
 msgstr ""
 
 msgid "pending"
 msgstr ""
 
 msgid "periods"
```

### Comparing `cubicweb-calendar-0.9.0/data/office-calendar.png` & `cubicweb-calendar-1.0.0/cubicweb_calendar/data/office-calendar.png`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.9.0/data/cubes.calendar.css` & `cubicweb-calendar-1.0.0/cubicweb_calendar/data/cubes.calendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-calendar-0.9.0/migration/0.4.0_Any.py` & `cubicweb-calendar-1.0.0/cubicweb_calendar/migration/0.4.0_Any.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from cubes.calendar import WORKING, NON_WORKING, WORKING_AM, WORKING_PM
+from cubicweb_calendar import WORKING, NON_WORKING, WORKING_AM, WORKING_PM
 
 dt_titles = {
     u'working': (u'journée de travail', WORKING),
     u'non_working': (u'non travaillé', NON_WORKING),
     u'working_am':  (u'matinée de travail', WORKING_AM),
     u'working_pm': (u'après-midi de travail', WORKING_PM),
     u'maladie_matin': (u'malade le matin', WORKING_PM),
@@ -20,12 +20,12 @@
                      u'après-midi de grève': WORKING_AM,
                      }
 
 add_attribute('Daytype', 'type')
 for daytype in rql('Any D, DT WHERE D is Daytype, D title DT').entities():
     try:
         new_dt_title, dt_type = dt_titles[daytype.title]
-        daytype.set_attributes(title=new_dt_title, type=dt_type)
+        daytype.cw_set(title=new_dt_title, type=dt_type)
     except KeyError:
         print "Oops, found an unknown daytype (%r) in the database" % daytype.title
 
 drop_entity_type('Timespan')
```

