# Comparing `tmp/gardener-cicd-cli-1.2114.0.tar.gz` & `tmp/gardener-cicd-cli-1.2115.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2114.0.tar", last modified: Fri Jul 21 12:31:42 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2115.0.tar", last modified: Mon Jul 24 06:41:41 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2114.0.tar` & `gardener-cicd-cli-1.2115.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:31:42.454051 gardener-cicd-cli-1.2114.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-21 12:31:42.454051 gardener-cicd-cli-1.2114.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:31:42.450051 gardener-cicd-cli-1.2114.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)    11039 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:31:42.454051 gardener-cicd-cli-1.2114.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_release_notes.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    12183 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     8141 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12219 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/productutil_v2.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 12:31:42.454051 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-21 12:31:42.000000 gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 12:31:42.454051 gardener-cicd-cli-1.2114.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-07-21 12:30:00.000000 gardener-cicd-cli-1.2114.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:41:41.948618 gardener-cicd-cli-1.2115.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-24 06:41:41.948618 gardener-cicd-cli-1.2115.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:41:41.940618 gardener-cicd-cli-1.2115.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10534 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:41:41.944618 gardener-cicd-cli-1.2115.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    12183 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/productutil_v2.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 06:41:41.948618 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-24 06:41:41.000000 gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 06:41:41.948618 gardener-cicd-cli-1.2115.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-07-24 06:40:57.000000 gardener-cicd-cli-1.2115.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2114.0/bin/component-cli` & `gardener-cicd-cli-1.2115.0/bin/component-cli`

 * *Files 3% similar despite different names*

```diff
@@ -193,18 +193,14 @@
         relation = 'local'
         is_local = True
         break
     else:
       relation = 'external'
       is_local = False
 
-    # special-case: if images.yaml does not specify a tag, but resource is already present,
-    # use tag from existing resource, but otherwise replace it
-    # in this specific case, do not add extraIdentity to behave exactly as component-cli
-    suppress_extra_id = False
     resource_name = None
     resource = None
     if not tag:
       if resource_id:
         resource_name = resource_id['name']
         image_dict['name'] = resource_name
       else:
@@ -212,31 +208,25 @@
 
       for resource in component.resources:
         if resource.name != resource_name:
           continue
 
         tag = resource.version
         component.resources.remove(resource)
-        suppress_extra_id = True # special-case for compatibility w/ component-cli; might be omitted
         if not 'relation' in image_dict:
           relation = resource.relation.value
           pass
         break
 
     if not tag: # and not resource:
       # special-case: if there is no tag, the image is only added to `images`-label on
       # component-level
       imagevector_label.value['images'].append(image_dict)
       continue
 
-    if not suppress_extra_id:
-      extra_identity |= {
-        'imagevector-gardener-cloud+tag': tag,
-      }
-
     is_current_component = source_repo == component.name
 
     if not is_current_component and is_local:
       # if we have a tag, and repository is "local" (as passed-in via --component-prefixes),
       # then we add a component-reference, and add the image to a label of this reference
       for component_reference in component.componentReferences:
         if component_reference.name == name and component_reference.version == tag:
@@ -294,17 +284,17 @@
     )
 
     component.resources.append(img_resource)
 
   if not imagevector_label.value['images']:
     component.labels.remove(imagevector_label)
 
-  # XXXXX hack (purge signatures) - remove before committing
+  # "normalise" (match component-cli's behaviour)
+  # this could (and should) be removed
   component_descriptor_dict = dataclasses.asdict(component_descriptor)
-  component_descriptor_dict.pop('signatures')
   component_dict = component_descriptor_dict['component']
   component_dict.pop('creationTime', None)
   if not component_dict.get('labels'):
     del component_dict['labels']
   for r in component_dict['resources']:
     r.pop('digest', None)
     r.pop('srcRefs', None)
```

### Comparing `gardener-cicd-cli-1.2114.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2115.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/bin/purge_history` & `gardener-cicd-cli-1.2115.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/_release_notes.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/_release_notes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2115.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2115.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2114.0/setup.py` & `gardener-cicd-cli-1.2115.0/setup.py`

 * *Files identical despite different names*

