# Comparing `tmp/polymeasure-0.1.0.tar.gz` & `tmp/polymeasure-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymeasure-0.1.0.tar", last modified: Sat Jul 22 13:08:11 2023, max compression
+gzip compressed data, was "polymeasure-0.1.1.tar", last modified: Mon Jul 24 00:57:18 2023, max compression
```

## Comparing `polymeasure-0.1.0.tar` & `polymeasure-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 13:08:11.908666 polymeasure-0.1.0/
--rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6428 2023-07-22 13:08:11.908666 polymeasure-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5862 2023-07-22 12:44:08.000000 polymeasure-0.1.0/README.md
--rw-rw-rw-   0        0        0      644 2023-07-22 13:04:09.000000 polymeasure-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 13:08:11.909666 polymeasure-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 13:08:11.896666 polymeasure-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 13:08:11.904666 polymeasure-0.1.0/src/polymeasure/
--rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.0/src/polymeasure/__init__.py
--rw-rw-rw-   0        0        0    42030 2023-07-22 13:06:17.000000 polymeasure-0.1.0/src/polymeasure/core.py
-drwxrwxrwx   0        0        0        0 2023-07-22 13:08:11.907666 polymeasure-0.1.0/src/polymeasure.egg-info/
--rw-rw-rw-   0        0        0     6428 2023-07-22 13:08:11.000000 polymeasure-0.1.0/src/polymeasure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-22 13:08:11.000000 polymeasure-0.1.0/src/polymeasure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 13:08:11.000000 polymeasure-0.1.0/src/polymeasure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-22 13:08:11.000000 polymeasure-0.1.0/src/polymeasure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.627510 polymeasure-0.1.1/
+-rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5676 2023-07-24 00:57:18.627510 polymeasure-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5112 2023-07-23 11:15:31.000000 polymeasure-0.1.1/README.md
+-rw-rw-rw-   0        0        0      644 2023-07-23 20:08:15.000000 polymeasure-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 00:57:18.627510 polymeasure-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.617511 polymeasure-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.622509 polymeasure-0.1.1/src/polymeasure/
+-rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.1/src/polymeasure/__init__.py
+-rw-rw-rw-   0        0        0    42670 2023-07-24 00:51:10.000000 polymeasure-0.1.1/src/polymeasure/core.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.626510 polymeasure-0.1.1/src/polymeasure.egg-info/
+-rw-rw-rw-   0        0        0     5676 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/top_level.txt
```

### Comparing `polymeasure-0.1.0/LICENSE` & `polymeasure-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polymeasure-0.1.0/PKG-INFO` & `polymeasure-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymeasure
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python analysis package for building SQL expressions.
 Author-email: Josh Grant <jagmanjg@gmail.com>
 Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
 Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,45 +22,75 @@
 
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
-The function evaluate returns a SQL statement, which will be syntactically valid only subject to
-sensible construction of the "PolyMeasure Tree".
-This evaluation may occur inside the evaluation contexts of other PolyMeasures, so that SQL expressions are
-built up recursively to achieve some complex calculation.
+The function `evaluate()` returns a SQL statement, built recursively from those components.
 
-## How it works
-
-In the following notation we drop the name parameter and write
+In the documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
+
+## How it works in a nutshell
+
+In pseudo-sql, `M( Inner * Dim; Outer; Where, Context )` evaluates as:
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [(
+      select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
+      where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
+  )], Dim
+  
+  from __VIEW__
+  where Where
+  group by Dim
+  <<context>>
+```
+
+There is a simpler presentation when Dim = Rowset(G):
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [Outer], __VIEW__.G
+  
+  from __VIEW__
+  where Where
+  <<context>>
+```
+
+## How it works
+
+
 The context can be parameters like having or order by clauses.
 The where parameter specifies additional filters to apply to the
 
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
 view, where we group once, then group the resulting rowset again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
-Free measures cannot be supplied as the inner measure of a PolyMeasure.
+Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
+their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
 Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
-keyed to any views required.
+keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
@@ -76,22 +106,14 @@
 RowSet means do not group the view. None is a wildcard, which means the measure will default
 to the dimensions of the enclosing measure after dimension promotion.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
-Here are the things you can build with a single PolyMeasure
-
-1) M( Outer ) - Outer measure with no specified dimension - will take on the dimension of the enclosing measure.
-2) M( * Dim ) - A summary table of the dimensions Dim.
-3) M( Outer * Dim ) - A summary table of the dimensions with Outer measures calculated over each group.
-4) M( ; Inner ) - Defaults to M( Inner )
-5) M( Outer * Dim ; Inner ) - A set of aggregated calculations (Outer) grouped by Dim over Inner.
-
 ==========================================
 
 Invalid measures fail on evaluation, not instantiation. Test with where 0 = 1 to validate.....
 
 ==========================================
 
 Bound measures are "inner idempotent", meaning passing them as the sole argument to an inner parameter
@@ -104,38 +126,7 @@
 ```
   B( B( Outer * Dim; Inner: Where) )
 = F( B( Outer * Dim; Inner: Where) )
 = B( F( Outer * Dim; Inner: Where) )
 =    B( Outer * Dim; Inner: Where)
 ```
 all hold. (Note: Inner=None implicitly in the expression F( Outer * Dim; Inner: Where))
-
-==========================================
-
-In pseudo-sql M( Inner * Dim; Outer; Where, Context ) evaluates as:
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [(
-    select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
-    where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
-)], Dim
-
-from __VIEW__
-where Where
-group by Dim
-<<context>>
-
-There is a simpler presentation when Dim = Rowset(G):
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [Outer], __VIEW__.G
-
-from __VIEW__
-where Where
-<<context>>
-
-==========================================
-
-Every outer measure needs to have dimensions that match the inner
-query. Use aliases or the rename function to achieve this.
```

### Comparing `polymeasure-0.1.0/README.md` & `polymeasure-0.1.1/src/polymeasure.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,96 @@
+Metadata-Version: 2.1
+Name: polymeasure
+Version: 0.1.1
+Summary: A python analysis package for building SQL expressions.
+Author-email: Josh Grant <jagmanjg@gmail.com>
+Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
+Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # polymeasure
 ## A python analysis package for building SQL expressions
 
 A PolyMeasure (or measure) represents a SQL "group by one view, evaluate over another" statement, with options
 for supplying the usual SQL operators or modifying the evaluation in other programmatic ways.
 The class provides a framework for creating analysis expressions over SQL database systems, in particular the
 duckdb SQL engine.
 
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
-The function evaluate returns a SQL statement, which will be syntactically valid only subject to
-sensible construction of the "PolyMeasure Tree".
-This evaluation may occur inside the evaluation contexts of other PolyMeasures, so that SQL expressions are
-built up recursively to achieve some complex calculation.
-
-## How it works
+The function `evaluate()` returns a SQL statement, built recursively from those components.
 
-In the following notation we drop the name parameter and write
+In the documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
+
+## How it works in a nutshell
+
+In pseudo-sql, `M( Inner * Dim; Outer; Where, Context )` evaluates as:
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [(
+      select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
+      where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
+  )], Dim
+  
+  from __VIEW__
+  where Where
+  group by Dim
+  <<context>>
+```
+
+There is a simpler presentation when Dim = Rowset(G):
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [Outer], __VIEW__.G
+  
+  from __VIEW__
+  where Where
+  <<context>>
+```
+
+## How it works
+
+
 The context can be parameters like having or order by clauses.
 The where parameter specifies additional filters to apply to the
 
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
 view, where we group once, then group the resulting rowset again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
-Free measures cannot be supplied as the inner measure of a PolyMeasure.
+Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
+their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
 Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
-keyed to any views required.
+keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
@@ -62,22 +106,14 @@
 RowSet means do not group the view. None is a wildcard, which means the measure will default
 to the dimensions of the enclosing measure after dimension promotion.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
-Here are the things you can build with a single PolyMeasure
-
-1) M( Outer ) - Outer measure with no specified dimension - will take on the dimension of the enclosing measure.
-2) M( * Dim ) - A summary table of the dimensions Dim.
-3) M( Outer * Dim ) - A summary table of the dimensions with Outer measures calculated over each group.
-4) M( ; Inner ) - Defaults to M( Inner )
-5) M( Outer * Dim ; Inner ) - A set of aggregated calculations (Outer) grouped by Dim over Inner.
-
 ==========================================
 
 Invalid measures fail on evaluation, not instantiation. Test with where 0 = 1 to validate.....
 
 ==========================================
 
 Bound measures are "inner idempotent", meaning passing them as the sole argument to an inner parameter
@@ -90,38 +126,7 @@
 ```
   B( B( Outer * Dim; Inner: Where) )
 = F( B( Outer * Dim; Inner: Where) )
 = B( F( Outer * Dim; Inner: Where) )
 =    B( Outer * Dim; Inner: Where)
 ```
 all hold. (Note: Inner=None implicitly in the expression F( Outer * Dim; Inner: Where))
-
-==========================================
-
-In pseudo-sql M( Inner * Dim; Outer; Where, Context ) evaluates as:
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [(
-    select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
-    where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
-)], Dim
-
-from __VIEW__
-where Where
-group by Dim
-<<context>>
-
-There is a simpler presentation when Dim = Rowset(G):
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [Outer], __VIEW__.G
-
-from __VIEW__
-where Where
-<<context>>
-
-==========================================
-
-Every outer measure needs to have dimensions that match the inner
-query. Use aliases or the rename function to achieve this.
```

### Comparing `polymeasure-0.1.0/pyproject.toml` & `polymeasure-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polymeasure"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Josh Grant", email="jagmanjg@gmail.com" },
 ]
 description = "A python analysis package for building SQL expressions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `polymeasure-0.1.0/src/polymeasure/core.py` & `polymeasure-0.1.1/src/polymeasure/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,24 +252,24 @@
         else:
             # wildcard dimension
             return_dim =  Dimension(dimensions=None, rowset=False, star=False)
 
         return return_dim
 
 
-    def _get_primitive_expression(self, parent=None, override_name=None, update_columns=False):
+    def _get_primitive_expression(self, inner_alias=None, override_name=None, update_columns=False):
 
         override_name = override_name if override_name is not None else self.name
         if len(self.outer) == 0:
             outer_primitive_expressions = []
         elif isinstance(self.outer[0], FunctionType):
             if update_columns:
-                outer_primitive_expressions = [override_name + ' = ' + self.outer[0](self=self, parent=parent)]
+                outer_primitive_expressions = [override_name + ' = ' + self.outer[0](self=self, inner_alias=inner_alias)]
             else:
-                outer_primitive_expressions = [self.outer[0](self=self, parent=parent) + ' ' + override_name]
+                outer_primitive_expressions = [self.outer[0](self=self, inner_alias=inner_alias) + ' ' + override_name]
         else:
             if update_columns:
                 outer_primitive_expressions = [override_name + ' = ' + self.outer[0]]
             else:
                 outer_primitive_expressions = [self.outer[0] + ' ' + override_name]
         return outer_primitive_expressions
 
@@ -377,15 +377,17 @@
     def __init__(
             self,
             name=None,
             outer=None,
             dim=None,
             inner=None,
             where=None, having=None, order_by=None, postfix=None,
-            include=None, exclude=None, join_nulls=True, acquire_dimensions=False, redirect=None
+            include=None, exclude=None, join_nulls=True,
+            acquire_dimensions=False, redirect=None,
+            suppress_from=False
     ):
         """
         Args:
             name: The name of the measure.
 
             outer: List of PolyMeasures or primitives to evaluate over inner, grouping by dim.
 
@@ -551,14 +553,15 @@
         self.order_by = order_by
         self.postfix = postfix
         self.include = make_as_list(include)
         self.exclude = make_as_list(exclude)
         self.join_nulls = join_nulls
         self.acquire_dimensions = acquire_dimensions
         self.redirect = redirect
+        self.suppress_from = suppress_from
 
         """     
         The function _to_polymeasure processes dummy measure entities into true PolyMeasure objects.
         _primitive indicates that _to_polymeasure isn't needed to interpret the field outer, which stops the recursion.
         In the primitive case outer is a string, or string a function which is passed parent and root as parameters
         Primitives are always free measures
         The outer_dimension is the final dimension set of the measure, which is determined recursively by both self.dim and the 
@@ -720,16 +723,20 @@
 
         star_expression = self.outer_dimension.star
         if star_expression is not None and star_expression:
             groupby_dimensions = [star_expression]
         else:
             groupby_dimensions = evaluate_dimensions if allow_grouping else []
 
+        # null queries have well defined inner measures but they do not have a select statement from them..
+        is_null_query = (wildcard_dimensions.dimensions is None and not wildcard_dimensions.rowset) and (
+            self.outer_dimension.wildcard and not self.outer_dimension.rowset)
+
         # Treat this query as a source query, do not alias the final from statement
-        evaluate_as_source = self._check_primitive(evaluate_inner)
+        evaluate_as_source = self._check_primitive(evaluate_inner) or is_null_query
 
         # filter these where statements using include/exclude and dimensionality
         # These where statements are given to outer and inner measures
         # self.where are added in afterwards..
         passthrough_where = [
             expression for expression in where
             if expression.test_keep_filter(
@@ -757,26 +764,26 @@
         ]
 
         # Calculate the dimensional join objects to be supplied to sub measures
         # This is done inside _evaluate, rather than _generate_primitive_sql, as only one group by is performed no matter
         # how many nested measures are created
         evaluate_redirect_inner = evaluate_inner if self.redirect is None else self.redirect
 
-# lorge change
         dimensional_where = [
             self.dimensional_join_primitive(column, view_alias, evaluate_redirect_inner, self.join_nulls)
             for column in evaluate_dimensions
         ]
 
         # Build the primitive SQL select expression
         # _get_primitive acts recursively here
 
         if self.primitive:
             # If the primitive is a function, it is evaluated now with self as its argument
             outer_primitive_expressions = self._get_primitive_expression(
+                inner_alias=view_name,
                 override_name=override_name
                 # , update_columns=update_columns
             )
         else:
             outer_primitive_expressions = self._get_primitive_sql_list(
                 passthrough_where + dimensional_where,
                 depth,
@@ -827,19 +834,22 @@
             update_expression = f"update {evaluate_inner_string} {view_alias} \nset"
             update_list = make_statement(prefix='', elements=outer_primitive_expressions)
             evaluate_sql = f"""
     {update_expression} {update_list}
     {where_expression}"""
 
         else:
-            if evaluate_inner is None:
+            # the from clause can be supressed, especially if a dynamic outer measure is used
+            if evaluate_inner is None or self.suppress_from or is_null_query:
                 post_select = ''
             else:
+
                 post_select = f"""{from_expression} {where_expression} {groupby_expression}
     {having_expression} {orderby_expression} {postfix_expression}"""
+
             evaluate_sql = f"""
     {with_expression} 
     {select_expression}
     {post_select}"""
 
         if aliased:
             if alias_type == 'set':
@@ -866,15 +876,14 @@
 
         primitive_sql_list = []
 
         # append measure where statements
         # new_where = where + self.where
         # append dimensional filters
 
-        new_depth = depth + 1
         wildcard_inner = self.inner if not self.free else wildcard_inner
         wildcard_dimensions = self.outer_dimension if not self.outer_dimension.wildcard else wildcard_dimensions
 
         passthrough_where = [
             expression for expression in where
             if expression.test_keep_filter(
                 self.include, self.exclude
@@ -901,37 +910,38 @@
 
                     # Lock the passthrough wheres to the current original alias - this is the right place to do it
 
                     locked_where = [
                         expression.fix_outer(original_alias) for expression in passthrough_where
                     ]
 
-                    if measure.free and measure.outer_dimension.wildcard and self.outer_dimension.rowset:
+                    # if measure.free and measure.outer_dimension.wildcard and self.outer_dimension.rowset:
+                    if measure.free and wildcard_inner is None:
                         # Generated when a rowset query doesn't need a subquery expression
                         primitive_sql_list = primitive_sql_list + measure._get_primitive_expression(
-                            parent=self, override_name=override_name, update_columns=update_columns)
+                            inner_alias=original_alias, override_name=override_name, update_columns=update_columns)
                     else:
                         if update_columns:
                             alias_type = 'set'
                         else:
                             alias_type = None
                         primitive_sql_list = primitive_sql_list + [measure._evaluate(
-                            locked_where, new_depth, breadth, wildcard_inner,
+                            locked_where, depth + 1, breadth, wildcard_inner,
                             wildcard_dimensions, aliased=True, allow_grouping=False,
                             override_name=override_name, update_columns=update_columns, alias_type=alias_type
                         )]
 
 
             else:
 
                 primitive_sql_list = primitive_sql_list + measure._get_primitive_sql_list(
                     # This is a non-primitive measure that has no opportunity to evaluate its
                     # own where clauses, so they are appended here.
                     passthrough_where + measure.where,
-                    new_depth, breadth, wildcard_inner, wildcard_dimensions,
+                    depth, breadth, wildcard_inner, wildcard_dimensions,
                     original_alias=original_alias, update_columns=update_columns
                 )
 
         return primitive_sql_list
```

### Comparing `polymeasure-0.1.0/src/polymeasure.egg-info/PKG-INFO` & `polymeasure-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,82 @@
-Metadata-Version: 2.1
-Name: polymeasure
-Version: 0.1.0
-Summary: A python analysis package for building SQL expressions.
-Author-email: Josh Grant <jagmanjg@gmail.com>
-Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
-Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # polymeasure
 ## A python analysis package for building SQL expressions
 
 A PolyMeasure (or measure) represents a SQL "group by one view, evaluate over another" statement, with options
 for supplying the usual SQL operators or modifying the evaluation in other programmatic ways.
 The class provides a framework for creating analysis expressions over SQL database systems, in particular the
 duckdb SQL engine.
 
 PolyMeasures have three main components
 
 - an inner view, also a PolyMeasure
 - a set of outer PolyMeasures to evaluate over that view, and
 - a set of dimensions to group the inner view by when evaluating the outer view(s).
 
-The function evaluate returns a SQL statement, which will be syntactically valid only subject to
-sensible construction of the "PolyMeasure Tree".
-This evaluation may occur inside the evaluation contexts of other PolyMeasures, so that SQL expressions are
-built up recursively to achieve some complex calculation.
-
-## How it works
+The function `evaluate()` returns a SQL statement, built recursively from those components.
 
-In the following notation we drop the name parameter and write
+In the documentation we drop the name parameter and write
 
 `M( Outer * Dim; Inner: Where, Context )`
 
 when describing a PolyMeasure, in line with the order of the other parameters of importance.
+
+## How it works in a nutshell
+
+In pseudo-sql, `M( Inner * Dim; Outer; Where, Context )` evaluates as:
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [(
+      select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
+      where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
+  )], Dim
+  
+  from __VIEW__
+  where Where
+  group by Dim
+  <<context>>
+```
+
+There is a simpler presentation when Dim = Rowset(G):
+
+```
+  with __VIEW__ as ( [select [Inner] from view([Inner])] )
+  
+  select [Outer], __VIEW__.G
+  
+  from __VIEW__
+  where Where
+  <<context>>
+```
+
+## How it works
+
+
 The context can be parameters like having or order by clauses.
 The where parameter specifies additional filters to apply to the
 
 There are two classes of PolyMeasures - those with a free view, where Outer = None, or a bound view
 which already exists in the database.
 A bound measure with the usual arguments will be denoted `B( Inner * Dim; Outer: Where )`
 and a free measure denoted `F( Inner * Dim; Outer: Where )`. Free views become handy expressions like
 "count(*) of any inner table" or "count(*) over dimensions of the inner table".
 
 Free measures take on the context of the inner query in a PolyMeasure, rather than referencing a basic
 view in the schema. This allows a single PolyMeasure object to perform a double aggregation over a given
 view, where we group once, then group the resulting rowset again and perform some aggregation.
 
 If a free measure is supplied to the outer measure list, it will query the corresponding inner measure list.
-Free measures cannot be supplied as the inner measure of a PolyMeasure.
+Free measures should not be supplied as the inner measure of a PolyMeasure, unless the outer measures can supply
+their own inner bindings.
 
 Bound measures should have a default string value for the view, appropriate to the schema.
 Using the supplied factory method BoundedMeasure will return a super-classed PolyMeasure
-keyed to any views required.
+keyed to a specific view, for convenience.
 
 In the following examples, we assume one unique bounded measure exists,
 B = B(dim=Rowset(), inner=main_view), which acts as the ultimate "leaf" measure.
 The class Free is also provided, which defaults the measure view to Free instead, and is aliased F.
 
 The Outer and Inner arguments are PolyMeasure vectors, which each can return tables of any dimension.
 When different dimensions are supplied in the outer measures, self.dim is used to group the inner view,
@@ -76,22 +92,14 @@
 RowSet means do not group the view. None is a wildcard, which means the measure will default
 to the dimensions of the enclosing measure after dimension promotion.
 
 The view and where parameters are applied to the inner query, Inner * Dim.
 For example if you want to apply a filter context to Outer directly (which is the final output aggregation),
 use M( Inner * Dim; F(Outer: Where_Outer): View, Where)
 
-Here are the things you can build with a single PolyMeasure
-
-1) M( Outer ) - Outer measure with no specified dimension - will take on the dimension of the enclosing measure.
-2) M( * Dim ) - A summary table of the dimensions Dim.
-3) M( Outer * Dim ) - A summary table of the dimensions with Outer measures calculated over each group.
-4) M( ; Inner ) - Defaults to M( Inner )
-5) M( Outer * Dim ; Inner ) - A set of aggregated calculations (Outer) grouped by Dim over Inner.
-
 ==========================================
 
 Invalid measures fail on evaluation, not instantiation. Test with where 0 = 1 to validate.....
 
 ==========================================
 
 Bound measures are "inner idempotent", meaning passing them as the sole argument to an inner parameter
@@ -104,38 +112,7 @@
 ```
   B( B( Outer * Dim; Inner: Where) )
 = F( B( Outer * Dim; Inner: Where) )
 = B( F( Outer * Dim; Inner: Where) )
 =    B( Outer * Dim; Inner: Where)
 ```
 all hold. (Note: Inner=None implicitly in the expression F( Outer * Dim; Inner: Where))
-
-==========================================
-
-In pseudo-sql M( Inner * Dim; Outer; Where, Context ) evaluates as:
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [(
-    select [Outer] from (view(Outer) OR __VIEW__) dynamic_view
-    where dynamic_view.dim(Outer) = __VIEW__.dim(Outer)
-)], Dim
-
-from __VIEW__
-where Where
-group by Dim
-<<context>>
-
-There is a simpler presentation when Dim = Rowset(G):
-
-with __VIEW__ as ( [select [Inner] from view([Inner])] )
-
-select [Outer], __VIEW__.G
-
-from __VIEW__
-where Where
-<<context>>
-
-==========================================
-
-Every outer measure needs to have dimensions that match the inner
-query. Use aliases or the rename function to achieve this.
```

