# Comparing `tmp/mercury-reels-1.4.3.tar.gz` & `tmp/mercury-reels-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-reels-1.4.3.tar", last modified: Tue May 30 10:27:42 2023, max compression
+gzip compressed data, was "mercury-reels-1.4.4.tar", last modified: Mon Jul 24 10:14:26 2023, max compression
```

## Comparing `mercury-reels-1.4.3.tar` & `mercury-reels-1.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.671446 mercury-reels-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.671446 mercury-reels-1.4.3/src/mercury_reels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 10:27:42.000000 mercury-reels-1.4.3/src/mercury_reels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:27:42.675447 mercury-reels-1.4.3/src/reels/
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Intake.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/Targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/imports.in
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/main.dox
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/py_reels.i
--rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/py_reels_wrap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    84431 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    45065 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels.h
--rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_main.h
--rw-r--r--   0 runner    (1001) docker     (123)    56793 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/reels_test.h
--rw-r--r--   0 runner    (1001) docker     (123)   123064 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/reels/thousand_sequences.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-30 10:27:34.000000 mercury-reels-1.4.3/src/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:14:26.985707 mercury-reels-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-07-24 10:14:26.985707 mercury-reels-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:14:26.985707 mercury-reels-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:14:26.981707 mercury-reels-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:14:26.985707 mercury-reels-1.4.4/src/mercury_reels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19000 2023-07-24 10:14:26.000000 mercury-reels-1.4.4/src/mercury_reels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 10:14:26.000000 mercury-reels-1.4.4/src/mercury_reels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:14:26.000000 mercury-reels-1.4.4/src/mercury_reels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 10:14:26.000000 mercury-reels-1.4.4/src/mercury_reels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:14:26.985707 mercury-reels-1.4.4/src/reels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/Clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/Clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/Events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/Intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/Targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/imports.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/main.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/py_reels.i
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/py_reels_wrap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    85083 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    45258 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels_main.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57861 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/reels_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)   123064 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/reels/thousand_sequences.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-24 10:14:20.000000 mercury-reels-1.4.4/src/test_all.py
```

### Comparing `mercury-reels-1.4.3/LICENSE.txt` & `mercury-reels-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/PKG-INFO` & `mercury-reels-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.3
+Version: 1.4.4
 Summary: Reels helps identify patterns in event data and can predict target events.
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mercury-reels-1.4.3/README.md` & `mercury-reels-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/pyproject.toml` & `mercury-reels-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires		= ['setuptools>=61.0']
 build-backend	= 'setuptools.build_meta'
 
 [project]
 name			= 'mercury-reels'
-version			= '1.4.3'
+version			= '1.4.4'
 description		= 'Reels helps identify patterns in event data and can predict target events.'
 license			= {file = "LICENSE.txt"}
 requires-python = '>=3.8'
 classifiers		= ['Programming Language :: Python :: 3',
 					'License :: OSI Approved :: Apache Software License',
 					'Operating System :: OS Independent']
 keywords		= ['event detection', 'event prediction', 'time series']
```

### Comparing `mercury-reels-1.4.3/src/mercury_reels.egg-info/PKG-INFO` & `mercury-reels-1.4.4/src/mercury_reels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-reels
-Version: 1.4.3
+Version: 1.4.4
 Summary: Reels helps identify patterns in event data and can predict target events.
 Author-email: Mercury Team <mercury.group@bbva.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mercury-reels-1.4.3/src/mercury_reels.egg-info/SOURCES.txt` & `mercury-reels-1.4.4/src/mercury_reels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/Clients.py` & `mercury-reels-1.4.4/src/reels/Clients.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/Clips.py` & `mercury-reels-1.4.4/src/reels/Clips.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/Events.py` & `mercury-reels-1.4.4/src/reels/Events.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/Intake.py` & `mercury-reels-1.4.4/src/reels/Intake.py`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/Targets.py` & `mercury-reels-1.4.4/src/reels/Targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,19 +157,25 @@
 
             predict() cannot be called before fit() and can be called any number of times in all overloaded forms after that.
 
             The model can only predict clips, so this will only work for those clients whose clips are stored in the object,
             unlike predict_clips() which is completely general.
 
         Args:
-            clients: The Clients object containing the ids of the clients you want to predict.
+            clients: The Clients object containing the ids of the clients you want to predict or a list of client ids.
 
         Returns:
             An iterator object containing the results. (Empty on error.)
         """
+        if type(clients) == list:
+            cli = Clients()
+            for c in clients:
+                cli.add_client_id(c)
+            return Result(targets_predict_clients(self.tr_id, cli.cl_id))
+
         return Result(targets_predict_clients(self.tr_id, clients.cl_id))
 
     def predict_clips(self, clips: Clips):
         """Predict time to target for a set of clients whose clips are given in a Clips object.
 
             predict() cannot be called before fit() and can be called any number of times in all overloaded forms after that.
```

### Comparing `mercury-reels-1.4.3/src/reels/__init__.py` & `mercury-reels-1.4.4/src/reels/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,14 @@
     return _py_reels.next_binary_image_iterator(image_id)
 
 def destroy_binary_image_iterator(image_id):
     return _py_reels.destroy_binary_image_iterator(image_id)
 
 
 # The source version file is <proj>/src/version.py, anything else is auto generated.
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from reels.Clients import Clients
 from reels.Events import Events
 from reels.Clips import Clips
 from reels.Targets import Targets
 from reels.Intake import Intake
```

### Comparing `mercury-reels-1.4.3/src/reels/main.dox` & `mercury-reels-1.4.4/src/reels/main.dox`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/py_reels.i` & `mercury-reels-1.4.4/src/reels/py_reels.i`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/py_reels_wrap.cpp` & `mercury-reels-1.4.4/src/reels/py_reels_wrap.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/reels.cpp` & `mercury-reels-1.4.4/src/reels/reels.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1958,14 +1958,45 @@
 
 	image[id] = p_bi;
 
 	return id;
 }
 
 
+bool parse_bin_event_pt(char *line, BinEventPt &ev) {
+
+	char *pt = strchr(line, '\t');
+
+	if (pt == nullptr)
+		return false;
+
+	uint64_t l = (uint64_t) pt - (uint64_t) line;
+
+	if (line[0] != '<' || l != 18 || sscanf(line, "<%016lx>\t", &ev.e) != 1)
+		ev.e = MurmurHash64A(line, l);
+
+	char *pt2 = strchr(++pt, '\t');
+
+	if (pt2 == nullptr)
+		return false;
+
+	l = (uint64_t) pt2 - (uint64_t) pt;
+
+	if (pt[0] != '<' || l != 18 || sscanf(pt, "<%016lx>\t", &ev.d) != 1)
+		ev.d = MurmurHash64A(pt, l);
+
+	char *pt3 = strchr(++pt2, '\t');
+
+	if (pt3 == nullptr)
+		return false;
+
+	return sscanf(pt2, "%lf\t", &ev.w) == 1;
+}
+
+
 /** \brief Describes the internal representation of an event. (Iterate through all.)
 
 	\param id		  The id returned by a previous new_events() call.
 	\param prev_event The previous description, either complete or the (emitter, description, weight) triple alone, or empty for the first.
 
 	\return	On success, it will return either tab separated emitter, description, weight, code (if store_strings is true) or
 			the same with hashes corresponding to strings instead of strings if false.
@@ -1977,43 +2008,30 @@
 	EventsServer::iterator it = events.find(id);
 
 	if (it == events.end())
 		return answer_buffer;
 
 	int ll = strlen(prev_event);
 
-	char e[1024];
-	char d[1024];
 	BinEventPt ev;
 	EventMap::iterator it_ev_end = it->second->events_end();
 	EventMap::iterator it_ev = it_ev_end;
 
 	if (ll == 0)
 		it_ev = it->second->events_begin();
-	else if (sscanf(prev_event, "%s\t%s\t%lf", e, d, &ev.w) == 3) {
-		int l = strlen(e);
-
-		if (e[0] != '<' || l != 18 || sscanf(e, "<%016lx>", &ev.e) != 1)
-			ev.e = MurmurHash64A(&e, l);
-
-		l = strlen(d);
-
-		if (d[0] != '<' || l != 18 || sscanf(d, "<%016lx>", &ev.d) != 1)
-			ev.d = MurmurHash64A(&d, l);
-
-		it_ev = it->second->events_next_after_find(ev);
-	}
+	else if (parse_bin_event_pt(prev_event, ev)) it_ev = it->second->events_next_after_find(ev);
 
 	if (it_ev != it_ev_end) {
+		double round_w = round(WEIGHT_PRECISION*it_ev->first.w)/WEIGHT_PRECISION;
 		if (it->second->store_strings) {
 			String e = it->second->get_str(it_ev->first.e);
 			String d = it->second->get_str(it_ev->first.d);
-			sprintf(answer_buffer, "%s\t%s\t%.5f\t%li", e.c_str(), d.c_str(), it_ev->first.w, it_ev->second.code);
+			sprintf(answer_buffer, "%s\t%s\t%.5f\t%li", e.c_str(), d.c_str(), round_w, it_ev->second.code);
 		} else
-			sprintf(answer_buffer, "<%016lx>\t<%016lx>\t%.5f\t%li", it_ev->first.e, it_ev->first.d, it_ev->first.w, it_ev->second.code);
+			sprintf(answer_buffer, "<%016lx>\t<%016lx>\t%.5f\t%li", it_ev->first.e, it_ev->first.d, round_w, it_ev->second.code);
 	}
 
 	return answer_buffer;
 }
 
 
 /** \brief Sets the public property max_num_events in an Events object stored by the EventsServer.
@@ -2128,28 +2146,38 @@
 	if (it != clients.end())
 		sprintf(answer_buffer, "<%016lx>", it->second->hash_client_id(p_cli));
 
 	return answer_buffer;
 }
 
 
-/** \brief Add a client ID to a Clients object stored by the ClientsServer.
+/** \brief Add a client ID to a Clients object stored by the ClientsServer only if new.
 
 	\param id	 The id returned by a previous new_clients() call.
 	\param p_cli The "client". A string representing "the actor".
 
-	\return	 True on success.
+	\return	 True on success. False on id not found or p_cli is empty or already a client.
 */
 bool clients_add_client_id(int id, char *p_cli) {
 
 	ClientsServer::iterator it = clients.find(id);
 
 	if (it == clients.end())
 		return false;
 
+	int ll = strlen(p_cli);
+
+	if (ll == 0)
+		return false;
+
+	ElementHash client_hash = MurmurHash64A(p_cli, ll);
+
+	if (it->second->id_set.find(client_hash) != it->second->id_set.end())
+		return false;
+
 	it->second->add_client_id(p_cli);
 
 	return true;
 }
 
 
 /** \brief Return the hash of a stored client ID by index as a decimal string.
```

### Comparing `mercury-reels-1.4.3/src/reels/reels.h` & `mercury-reels-1.4.4/src/reels/reels.h`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 namespace reels
 {
 
 #define IMAGE_BUFF_SIZE			6136					///< Makes sizeof(ImageBlock) == 6K.
 #define PRIORITY_SEEN_FACTOR	2000000000				///< Close enough to 2^31 increases by 1 on visit, multiplies by this on seen.
 #define DEFAULT_NUM_EVENTS		1000					///< A size to store events in an Events object by default.
 #define MAX_SEQ_LEN_IN_PREDICT	1000					///< The maximum sequence length used in prediction.
-#define PREDICT_MAX_TIME		(10*365.25*24*3600)		///< Ten years when the target was never seen.
+#define PREDICT_MAX_TIME		(100*365.25*24*3600)	///< Hundred years when the target was never seen.
+#define WEIGHT_PRECISION		10000					///< 10^ the number of digits at which weight is rounded
 
 typedef uint64_t 						ElementHash;	///< A binary hash of a string
 typedef std::string						String;			///< A dynamically allocated c++ string
 typedef const char *					pChar;			///< A c string
 
 typedef time_t							TimePoint;		///< A c 8 byte integer time point
 typedef struct tm						TimeStruct;		///< A c structure of integer fields
@@ -97,25 +98,25 @@
 	/** \brief Compare to another BinEventPt for identity to support use as a key in a map.
 
 		\param o Another BinEventPt to which the current object is compared.
 
 		\return	 True if identical.
 	*/
 	bool operator==(const BinEventPt &o) const {
-		return e == o.e && d == o.d && w == o.w;
+		return e == o.e && d == o.d && round(WEIGHT_PRECISION*w) == round(WEIGHT_PRECISION*o.w);
 	}
 
 	/** \brief Compare to another BinEventPt for strict order to support use as a key in a map.
 
 		\param o Another BinEventPt to which the current object is compared.
 
 		\return	 True if strictly smaller (before in the order).
 	*/
 	bool operator<(const BinEventPt &o) const {
-		return e < o.e || (e == o.e && d < o.d) || (e == o.e && d == o.d && w < o.w);
+		return e < o.e || (e == o.e && d < o.d) || (e == o.e && d == o.d && round(WEIGHT_PRECISION*w) < round(WEIGHT_PRECISION*o.w));
 	}
 };
 
 
 /** \brief The binary representation of a transaction in a transaction file.
 
 	The class row converts the many possible source forms into this binary representation.
```

### Comparing `mercury-reels-1.4.3/src/reels/reels_main.cpp` & `mercury-reels-1.4.4/src/reels/reels_main.cpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/reels_main.h` & `mercury-reels-1.4.4/src/reels/reels_main.h`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/reels_test.cpp` & `mercury-reels-1.4.4/src/reels/reels_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -601,46 +601,80 @@
 				REQUIRE(ev_defined.priority.size() == 0);
 			}
 		}
 
 		WHEN("I use the python API server to test events_describe_next_event().") {
 			int ev_id1 = new_events();
 			int ev_id2 = new_events();
+			int ev_id3 = new_events();
 
 			events_set_store_strings(ev_id2, false);
+			events_set_store_strings(ev_id3, true);
 
 			REQUIRE(events_insert_row(ev_id1, (char *) "emi", (char *) "des", 1));
 			REQUIRE(events_insert_row(ev_id1, (char *) "emi2", (char *) "des", 1));
 			REQUIRE(events_insert_row(ev_id2, (char *) "emi", (char *) "des", 1));
 			REQUIRE(events_insert_row(ev_id2, (char *) "emi2", (char *) "des", 1));
+			REQUIRE(events_insert_row(ev_id3, (char *) "a aa", (char *) "x", 2));
+			REQUIRE(events_insert_row(ev_id3, (char *) "b bb", (char *) "y", 2));
 
 			THEN("Everything goes.") {
 				char buff[256];
 
 				sprintf(buff, "%s", events_describe_next_event(ev_id1, (char *) ""));
 
 				REQUIRE(strcmp(buff, (char *) "emi\tdes\t1.00000\t1") == 0);
 
 				sprintf(buff, "%s", events_describe_next_event(ev_id1, buff));
 
 				REQUIRE(strcmp(buff, (char *) "emi2\tdes\t1.00000\t2") == 0);
 
+				sprintf(buff, "%s", events_describe_next_event(ev_id1, buff));
+
+				REQUIRE(strlen(buff) == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id1, (char *) "xxx"));
+
+				REQUIRE(strlen(buff) == 0);
+
 				sprintf(buff, "%s", events_describe_next_event(ev_id1, (char *) "<a0b2fbd5d8ff9c22>\t<0a348b052daf4285>\t1.00000\t1"));
 
 				REQUIRE(strcmp(buff, (char *) "emi2\tdes\t1.00000\t2") == 0);
 
 				sprintf(buff, "%s", events_describe_next_event(ev_id2, (char *) ""));
 
 				REQUIRE(strcmp(buff, (char *) "<a0b2fbd5d8ff9c22>\t<0a348b052daf4285>\t1.00000\t1") == 0);
 
 				sprintf(buff, "%s", events_describe_next_event(ev_id2, buff));
 
 				REQUIRE(strcmp(buff, (char *) "<af06a6d491b4fc8e>\t<0a348b052daf4285>\t1.00000\t2") == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id2, (char *) "xxx\tyyy"));
+
+				REQUIRE(strlen(buff) == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id3, (char *) ""));
+
+				REQUIRE(strcmp(buff, (char *) "b bb\ty\t2.00000\t2") == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id3, buff));
+
+				REQUIRE(strcmp(buff, (char *) "a aa\tx\t2.00000\t1") == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id3, buff));
+
+				REQUIRE(strlen(buff) == 0);
+
+				sprintf(buff, "%s", events_describe_next_event(ev_id3, (char *) "xxx\tyyy\t1"));
+
+				REQUIRE(strlen(buff) == 0);
+
 			}
 
+			destroy_events(ev_id3);
 			destroy_events(ev_id2);
 			destroy_events(ev_id1);
 		}
 
 		WHEN("I build a few OptimizeEval vectors.") {
 			OptimizeEval m_1 = {}, neg = {}, z_0 = {}, pos = {}, p_1 = {};
```

### Comparing `mercury-reels-1.4.3/src/reels/reels_test.h` & `mercury-reels-1.4.4/src/reels/reels_test.h`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/reels/thousand_sequences.hpp` & `mercury-reels-1.4.4/src/reels/thousand_sequences.hpp`

 * *Files identical despite different names*

### Comparing `mercury-reels-1.4.3/src/test_all.py` & `mercury-reels-1.4.4/src/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,27 +61,27 @@
 
 	ev_2 = events_describe_next_event(evn.ev_id, ev_1)
 	ev_x = events_describe_next_event(evn.ev_id, '\t'.join(ll))
 
 	assert ev_2 == 'emi2\tdes\t1.00000\t2'
 	assert ev_2 == ev_x
 
-	ev_x = events_describe_next_event(evn.ev_id, '\t'.join(ll[0:3]))
+	ev_x = events_describe_next_event(evn.ev_id, '\t'.join(ll))
 
 	assert ev_2 == ev_x
 
-	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s' % (cli.hash_client_id(ll[0]), ll[1], ll[2]))
+	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s\t' % (cli.hash_client_id(ll[0]), ll[1], ll[2]))
 
 	assert ev_2 == ev_x
 
-	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s' % (ll[0], cli.hash_client_id(ll[1]), ll[2]))
+	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s\t' % (ll[0], cli.hash_client_id(ll[1]), ll[2]))
 
 	assert ev_2 == ev_x
 
-	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s' % (cli.hash_client_id(ll[0]), cli.hash_client_id(ll[1]), ll[2]))
+	ev_x = events_describe_next_event(evn.ev_id, '%s\t%s\t%s\t' % (cli.hash_client_id(ll[0]), cli.hash_client_id(ll[1]), ll[2]))
 
 	assert ev_2 == ev_x
 
 	assert events_describe_next_event(evn.ev_id, ev_x) == ''
 
 	tc = 0
 	for tp in evn.describe_events():
@@ -181,40 +181,40 @@
 	assert st.endswith(' 5 clients')
 
 	assert len(ll) == 5
 
 	assert ll[0] == cli.hash_client_id('cli1')
 	assert ll[4] == cli.hash_client_id('cli5')
 
-	assert cli.add_client_id('cli4')
-	assert cli.add_client_id('cli5')
+	assert not cli.add_client_id('cli4')
+	assert not cli.add_client_id('cli5')
 
 	ll = list(cli.client_hashes())
 
-	assert len(ll) == 7
+	assert len(ll) == 5
 
-	assert ll[5] == cli.hash_client_id('cli4')
-	assert ll[6] == cli.hash_client_id('cli5')
+	assert ll[3] == cli.hash_client_id('cli4')
+	assert ll[4] == cli.hash_client_id('cli5')
 
 	im = cli.save_as_binary_image()
 
 	cl2 = reels.Clients(im)
 
 	ll2 = list(cl2.client_hashes())
 
-	assert ll2[5] == cl2.hash_client_id('cli4')
-	assert ll2[6] == cl2.hash_client_id('cli5')
+	assert ll2[3] == cl2.hash_client_id('cli4')
+	assert ll2[4] == cl2.hash_client_id('cli5')
 
 	pkk = pickle.dumps(cli)
 	cl3 = pickle.loads(pkk)
 
 	ll3 = list(cl3.client_hashes())
 
-	assert ll3[5] == cl3.hash_client_id('cli4')
-	assert ll3[6] == cl3.hash_client_id('cli5')
+	assert ll3[3] == cl3.hash_client_id('cli4')
+	assert ll3[4] == cl3.hash_client_id('cli5')
 
 	assert not cl3.load_from_binary_image(im)
 
 	assert cl3.num_clients() == 0
 
 	cl4 = reels.Clients()
 
@@ -396,19 +396,19 @@
 	cli = reels.Clients()
 	assert cli.add_client_id('cli1')
 	assert cli.add_client_id('cli2')
 	assert cli.add_client_id('cli3')
 	assert cli.add_client_id('cli4')
 	assert cli.add_client_id('cli5')
 	assert cli.add_client_id('cli6')
-	assert cli.add_client_id('cli5')
-	assert cli.add_client_id('cli4')
-	assert cli.add_client_id('cli1')
+	assert not cli.add_client_id('cli5')
+	assert not cli.add_client_id('cli4')
+	assert not cli.add_client_id('cli1')
 
-	assert cli.num_clients() == 9
+	assert cli.num_clients() == 6
 
 	clp = reels.Clips(cli, evn)
 	assert clp.scan_event('e', 'd1', 1.0, 'cli1', '2022-06-01 00:00:00')
 	assert clp.scan_event('e', 'd2', 1.0, 'cli1', '2022-06-01 01:00:00')
 	assert clp.scan_event('e', 'd3', 1.0, 'cli1', '2022-06-01 02:00:00')
 	assert clp.scan_event('e', 'd4', 1.0, 'cli1', '2022-06-01 03:00:00')
 	assert clp.scan_event('e', 'd5', 1.0, 'cli1', '2022-06-01 04:00:00')
@@ -658,18 +658,22 @@
 	assert 'num_of_has_target_final_node  : 1' in log
 
 	cc = trg.tree_node_children(i)
 	assert cc is None
 
 	t_cli = list(trg.predict_clients(cli))
 
-	assert len(t_cli) == 9
-	assert t_cli[0] == t_cli[8]
-	assert t_cli[3] == t_cli[7]
-	assert t_cli[4] == t_cli[6]
+	assert len(t_cli) == 6
+
+	t_cl2 = list(trg.predict_clients(['cli1', 'cli2', 'cli3', 'cli4', 'cli5', 'cli6']))
+
+	assert len(t_cl2) == 6
+
+	for x, y in zip(t_cli, t_cl2):
+		assert x == y
 
 	t_clp = list(trg.predict_clips(clp))
 
 	assert len(t_clp) == 6
 
 	d_cli = dict(zip(cli.client_hashes(), t_cli))
 	d_clp = dict(zip(clp.clips_client_hashes(), t_clp))
```

