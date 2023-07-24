# Comparing `tmp/triplify_csv-0.5.0.tar.gz` & `tmp/triplify_csv-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.5.0.tar", max compression
+gzip compressed data, was "triplify_csv-0.5.1.tar", max compression
```

## Comparing `triplify_csv-0.5.0.tar` & `triplify_csv-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-07-03 17:07:53.114156 triplify_csv-0.5.0/LICENSE
--rw-r--r--   0        0        0     8007 2023-07-14 16:02:34.486997 triplify_csv-0.5.0/README.md
--rw-r--r--   0        0        0      585 2023-07-07 16:01:20.910360 triplify_csv-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-03 17:07:53.205155 triplify_csv-0.5.0/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    18764 2023-07-06 07:31:04.719065 triplify_csv-0.5.0/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     8836 1970-01-01 00:00:00.000000 triplify_csv-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-07-16 06:51:27.578399 triplify_csv-0.5.1/LICENSE
+-rw-r--r--   0        0        0     8154 2023-07-24 14:40:00.680945 triplify_csv-0.5.1/README.md
+-rw-r--r--   0        0        0      585 2023-07-24 14:45:41.672935 triplify_csv-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-16 06:51:27.655399 triplify_csv-0.5.1/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    19356 2023-07-23 08:52:41.807107 triplify_csv-0.5.1/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     8983 1970-01-01 00:00:00.000000 triplify_csv-0.5.1/PKG-INFO
```

### Comparing `triplify_csv-0.5.0/LICENSE` & `triplify_csv-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.5.0/README.md` & `triplify_csv-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007g - Assigning triples to the default graph
 - R2RMLTC0007h - Assigning triples to a non-IRI named graph
 - R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template
 - R2RMLTC0008b - Generation of triples referencing object map
 - R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap
 - R2RMLTC0009a - Generation of triples from foreign key relations
+	- Testing added about creating triples from foreign key relations, even for self-joins to represent things like hierarchy in the same "table"/csv
 - R2RMLTC0015a - Generation of language tags for plain literals from a CSV 'table' with language information
 	- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses 'rr:sqlQuery' to select tags in each language from a single table.
 - R2RMLTC0016a to R2RMLTC0016d, setting data types as in these tests for string, integer, real, float, date, timestamp and boolean.  
 	- note: instead of deriving the data type from the sql column, as the subset of r2rml used here does not refer to a database the user must use 'explicitly typed literals' as in section [7.6 Typed Literals](https://www.w3.org/TR/r2rml/#typed-literals) (rr:datatype) of the r2rml standard.
 
 Copyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from 'R2RML: RDB to RDF Mapping Language' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and 'R2RML and Direct Mapping Test Cases' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)
```

### Comparing `triplify_csv-0.5.0/pyproject.toml` & `triplify_csv-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "triplify_csv"
-version = "0.5.0"
+version = "0.5.1"
 description = "A tool to generate triples from CSV files according to a configuration file."
 authors = ["Adrian Atley"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/AAtley/triplify_csv"
 
 [tool.poetry.dependencies]
```

### Comparing `triplify_csv-0.5.0/triplify_csv/triplify_csv.py` & `triplify_csv-0.5.1/triplify_csv/triplify_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,23 +305,29 @@
 				#	print('found csvinfo: ' + csvinfo.tablename)
 			
 			# check we have a csv file with the same name as the logical_table in rml
 			if csvinfo is None:
 				self.errors.append('A csv for table {} was not found'.format(logical_table))
 				continue
 				
+			 
+			# bookmark the row we are on as if csv 'table' has foreign key to itself the row position of the 'child' table will be lost
+			# this allows the return the the original row after the same 'table' is scanned as a look up for that FK value
+			rowbookmark = 0
 			
 			# only continue if fieldnames in cols named of template all appear in column names of table in csv
 			if set(cols).issubset(csvinfo.columnNames):
 				# construct URIRef for subject
 				rdr = csvinfo.get_restarted_reader()
 				
 				
 				next(rdr) # skip the headers
+				rowbookmark = rowbookmark + 1
 				for row in rdr:				
+					rowbookmark = rowbookmark + 1
 					# if subjectmap's graph given by template, col names by row values
 					if rr('graphMap') in tmaps[tk][rr('subjectMap')]:
 						if rr('template') in tmaps[tk][rr('subjectMap')][rr('graphMap')]:
 							context = self.get_Uri_From_Template(context,row)
 					
 					# replace subject template's col names with values from csv
 					s = re.sub('[{"}]','',subjmap_template)
@@ -401,14 +407,23 @@
 											for fkrow in fkrdr:
 												if fkrow[parent] ==  childval:
 													record = fkrow
 											# get uri from fk csv's template and fk row
 											ptmSubjectTemplate = tmaps[ptm][rr('subjectMap')][rr('template')]
 											
 											object = URIRef(self.get_Uri_From_Template(ptmSubjectTemplate,record))
+											
+											# point row back at the row it was looking at
+											rdr = csvinfo.get_restarted_reader()
+											resetrow = 0
+											
+											while resetrow < rowbookmark:
+												next(rdr) # skip the headers
+												resetrow = resetrow + 1
+											
 							
 							# R2RMLTC0003c
 							elif rr('objectMap') in pom and rr('template') in pom[rr('objectMap')]:
 								ocols = []
 								objmap_template = pom[rr('objectMap')][rr('template')]
 								for match in re.finditer(r'{"([^>]+?)"}',objmap_template):
 									ocols.append(match.group(0).strip('{}"'))
@@ -427,15 +442,14 @@
 									print('object is ' + object)
 								
 							elif len(pom_column) > 0 and pom_column in row.keys():
 								print('in elif')
 								
 								object = self.get_literal(row[pom_column],csvinfo.options.dateformat, literal_lang, lit_datatype)
 							else:
-								print('in else')
 								object = URIRef(pom_object)
 	
 							# add to Dataset for quads if non-default graph else add just add triple
 							if making_quads:
 								gc = self.triples.graph(URIRef(context))
 								self.triples.add((subject, predicate, object, gc))
```

### Comparing `triplify_csv-0.5.0/PKG-INFO` & `triplify_csv-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplify-csv
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool to generate triples from CSV files according to a configuration file.
 Home-page: https://github.com/AAtley/triplify_csv
 License: BSD-3-Clause
 Author: Adrian Atley
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -105,14 +105,15 @@
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007g - Assigning triples to the default graph
 - R2RMLTC0007h - Assigning triples to a non-IRI named graph
 - R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template
 - R2RMLTC0008b - Generation of triples referencing object map
 - R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap
 - R2RMLTC0009a - Generation of triples from foreign key relations
+	- Testing added about creating triples from foreign key relations, even for self-joins to represent things like hierarchy in the same "table"/csv
 - R2RMLTC0015a - Generation of language tags for plain literals from a CSV 'table' with language information
 	- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses 'rr:sqlQuery' to select tags in each language from a single table.
 - R2RMLTC0016a to R2RMLTC0016d, setting data types as in these tests for string, integer, real, float, date, timestamp and boolean.  
 	- note: instead of deriving the data type from the sql column, as the subset of r2rml used here does not refer to a database the user must use 'explicitly typed literals' as in section [7.6 Typed Literals](https://www.w3.org/TR/r2rml/#typed-literals) (rr:datatype) of the r2rml standard.
 
 Copyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from 'R2RML: RDB to RDF Mapping Language' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and 'R2RML and Direct Mapping Test Cases' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)
```

