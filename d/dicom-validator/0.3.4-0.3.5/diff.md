# Comparing `tmp/dicom-validator-0.3.4.tar.gz` & `tmp/dicom-validator-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dicom-validator-0.3.4.tar", last modified: Mon Nov 22 20:51:26 2021, max compression
+gzip compressed data, was "dicom-validator-0.3.5.tar", last modified: Mon Jul 24 19:19:09 2023, max compression
```

## Comparing `dicom-validator-0.3.4.tar` & `dicom-validator-0.3.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator/
--rw-rw-rw-   0        0        0     7446 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/dump_dcm_info.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/
--rw-rw-rw-   0        0        0     5377 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/condition.py
--rw-rw-rw-   0        0        0    12124 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/condition_parser.py
--rw-rw-rw-   0        0        0    10477 2021-11-22 20:48:17.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/edition_reader.py
--rw-rw-rw-   0        0        0    13786 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/part3_reader.py
--rw-rw-rw-   0        0        0     2776 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/part4_reader.py
--rw-rw-rw-   0        0        0     5086 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/part6_reader.py
--rw-rw-rw-   0        0        0      276 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/serializer.py
--rw-rw-rw-   0        0        0     2772 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/spec_reader.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/
--rw-rw-rw-   0        0        0     8652 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_condition.py
--rw-rw-rw-   0        0        0    24284 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_condition_parser.py
--rw-rw-rw-   0        0        0     9936 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_edition_reader.py
--rw-rw-rw-   0        0        0     5690 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_part3_reader.py
--rw-rw-rw-   0        0        0     2513 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_part4_reader.py
--rw-rw-rw-   0        0        0     2735 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_part6_reader.py
--rw-rw-rw-   0        0        0     1282 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_spec_reader.py
--rw-rw-rw-   0        0        0        0 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/spec_reader/__init__.py
--rw-rw-rw-   0        0        0      429 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/tag_tools.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator/tests/
--rw-rw-rw-   0        0        0      757 2021-11-22 20:48:17.000000 dicom-validator-0.3.4/dicom_validator/tests/test_cmdline_tools.py
--rw-rw-rw-   0        0        0      408 2021-11-22 20:48:17.000000 dicom-validator-0.3.4/dicom_validator/tests/test_utils.py
--rw-rw-rw-   0        0        0        0 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/tests/__init__.py
--rw-rw-rw-   0        0        0     2226 2021-11-22 20:48:17.000000 dicom-validator-0.3.4/dicom_validator/validate_iods.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator/validator/
--rw-rw-rw-   0        0        0     1826 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/validator/dicom_file_validator.py
--rw-rw-rw-   0        0        0     9902 2021-11-22 20:48:17.000000 dicom-validator-0.3.4/dicom_validator/validator/iod_validator.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator/validator/tests/
--rw-rw-rw-   0        0        0     4851 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/validator/tests/test_dicom_file_validator.py
--rw-rw-rw-   0        0        0    16678 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/validator/tests/test_iod_validator.py
--rw-rw-rw-   0        0        0        0 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/validator/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/dicom_validator/validator/__init__.py
--rw-rw-rw-   0        0        0       23 2021-11-22 20:49:50.000000 dicom-validator-0.3.4/dicom_validator/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/dicom_validator.egg-info/
--rw-rw-rw-   0        0        0        1 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    10783 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        8 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1624 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2021-11-22 20:51:25.000000 dicom-validator-0.3.4/dicom_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2018-02-11 12:57:20.000000 dicom-validator-0.3.4/LICENSE
--rw-rw-rw-   0        0        0    10783 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8330 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/README.md
--rw-rw-rw-   0        0        0      143 2021-11-22 20:51:26.000000 dicom-validator-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1757 2021-11-22 17:32:42.000000 dicom-validator-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.508841 dicom-validator-0.3.5/dicom_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/dump_dcm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.512841 dicom-validator-0.3.5/dicom_validator/spec_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/edition_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/part3_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/part4_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/part6_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/spec_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.512841 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_edition_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_part3_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_part4_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_part6_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_spec_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/tag_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/dicom_validator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/tests/test_cmdline_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validate_iods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/dicom_validator/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/dicom_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/iod_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/dicom_validator/validator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/tests/test_dicom_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/dicom_validator/validator/tests/test_iod_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:19:09.508841 dicom-validator-0.3.5/dicom_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 19:19:09.000000 dicom-validator-0.3.5/dicom_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 19:19:09.516841 dicom-validator-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-24 19:18:58.000000 dicom-validator-0.3.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dicom-validator-0.3.4/dicom_validator/dump_dcm_info.py` & `dicom-validator-0.3.5/dicom_validator/dump_dcm_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-"""
-Dumps tag information from a DICOM file using information in PS3.6.
-"""
-
-import argparse
-import os
-import re
-
-from pydicom import dcmread
-from pydicom.errors import InvalidDicomError
-
-from dicom_validator.spec_reader.edition_reader import EditionReader
-
-
-class DataElementDumper(object):
-    tag_regex = re.compile(
-        r'(\(?[\dabcdefABCDEF]{4}), *([\dabcdefABCDEF]{4})\)?')
-
-    def __init__(self, dict_info, uid_info, max_value_len, show_image_data,
-                 tags):
-        self.dict_info = dict_info
-        self.max_value_len = max_value_len
-        self.level = 0
-        self.show_image_data = show_image_data
-
-        self.uid_info = {}
-        for uid_dict in uid_info.values():
-            self.uid_info.update(uid_dict)
-
-        tags = tags or []
-        self.tags = []
-        for tag in tags:
-            match = self.tag_regex.match(tag)
-            if match:
-                self.tags.append(
-                    '({},{})'.format(match.group(1), match.group(2)))
-            else:
-                matching = [tag_id for tag_id in dict_info
-                            if
-                            dict_info[tag_id]['name'].replace(" ", "") == tag]
-                if matching:
-                    self.tags.append(matching[0])
-                else:
-                    print('{} is not a valid tag expression - '
-                          'ignoring'.format(tag))
-
-    def print_dataset(self, dataset):
-        dataset.walk(
-            lambda data_set, data_elem: self.print_dataelement(data_set,
-                                                               data_elem))
-
-    def print_element(self, tag_id, name, vr, prop, value):
-        if self.tags and tag_id not in self.tags:
-            return False
-        vm = 1 if value else 0
-        if isinstance(value, list):
-            vm = len(value)
-            value = '\\'.join([str(element) for element in value])
-        if isinstance(value, bytes):
-            value = str(value)[2:-1]
-        if isinstance(value, str) and len(value) > self.max_value_len:
-            value = value[:self.max_value_len] + '...'
-
-        indent = 2 * self.level
-        format_string = '{{}}{{}} {{:{}}} {{}} {{:4}} {{}} [{{}}]'.format(
-            40 - indent)
-        print(format_string.format(' ' * indent,
-                                   tag_id,
-                                   name[:40 - indent],
-                                   vr,
-                                   vm,
-                                   prop,
-                                   value))
-        return True
-
-    def print_dataelement(self, _, dataelement):
-        tag_id = '({:04X},{:04X})'.format(dataelement.tag.group,
-                                          dataelement.tag.element)
-        description = self.dict_info.get(tag_id)
-        if description is None:
-            name = '[Unknown]'
-            vr = dataelement.VR
-            prop = ''
-        else:
-            vr = description['vr']
-            name = description['name']
-            prop = description['prop']
-        value = dataelement.value
-        if vr == 'UI':
-            # do not rely on pydicom here - we want to use the
-            # currently loaded DICOM spec
-            value = repr(value)[1:-1]
-            value = self.uid_info.get(value, value)
-        if vr == 'SQ':
-            if self.print_element(tag_id, name, vr, prop,
-                                  'Sequence with {} item(s)'.format(
-                                      len(value))):
-                self.level += 1
-                self.print_sequence(dataelement)
-                self.level -= 1
-        else:
-            self.print_element(tag_id, name, vr, prop, value)
-
-    def print_sequence(self, sequence):
-        indent = 2 * self.level
-        format_string = '{{}}Item {{:<{}}} [Dataset with {{}} element(s)]'\
-            .format(56 - indent)
-        for i, dataset in enumerate(sequence):
-            print(format_string.format(' ' * indent, i + 1, len(dataset)))
-            self.level += 1
-            dataset.walk(lambda data_set, data_elem:
-                         self.print_dataelement(data_set, data_elem))
-            self.level -= 1
-
-    def dump_file(self, file_path):
-        try:
-            print('\n' + file_path)
-            dataset = dcmread(
-                file_path, stop_before_pixels=self.show_image_data, force=True)
-            self.print_dataset(dataset)
-        except (InvalidDicomError, KeyError):
-            print(
-                u'{} is not a valid DICOM file - skipping.'.format(file_path))
-
-    def dump_directory(self, dir_path):
-        for root, _, names in os.walk(dir_path):
-            for name in names:
-                self.dump_file(os.path.join(root, name))
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description='Dumps DICOM information dictionary from '
-                    'DICOM file using PS3.6')
-    parser.add_argument('dicomfiles',
-                        help='Path(s) of DICOM files or directories to parse',
-                        nargs='+')
-    parser.add_argument('--standard-path', '-src',
-                        help='Path with the DICOM specs in docbook '
-                             'and json format',
-                        default=os.path.join(os.path.expanduser("~"),
-                                             'dicom-validator'))
-    parser.add_argument('--revision', '-r',
-                        help='Standard revision (e.g. "2014c"), year of '
-                             'revision, "current" or "local" (latest '
-                             'locally installed)',
-                        default='current')
-    parser.add_argument('--max-value-len', '-ml',
-                        help='Maximum string length of displayed values',
-                        type=int,
-                        default=80)
-    parser.add_argument('--show-tags', '-t',
-                        help='Show only output for the searched tags. '
-                             'Tags can be in the format ####,#### or as the '
-                             'dictionary name (e.g. "PatientName").',
-                        nargs='*')
-    parser.add_argument('--show-image-data', '-id', action='store_false',
-                        help='Also show the image data tag (slower)')
-    args = parser.parse_args()
-
-    edition_reader = EditionReader(args.standard_path)
-    destination = edition_reader.get_revision(args.revision)
-    if destination is None:
-        print(
-            'Failed to get DICOM edition {} - aborting'.format(args.revision))
-        return 1
-
-    json_path = os.path.join(destination, 'json')
-    dict_info = EditionReader.load_dict_info(json_path)
-    uid_info = EditionReader.load_uid_info(json_path)
-    dumper = DataElementDumper(dict_info, uid_info, args.max_value_len,
-                               args.show_image_data,
-                               args.show_tags)
-    for dicom_path in args.dicomfiles:
-        if not os.path.exists(dicom_path):
-            print('\n"%s" does not exist - skipping', dicom_path)
-        else:
-            if os.path.isdir(dicom_path):
-                dumper.dump_directory(dicom_path)
-            else:
-                dumper.dump_file(dicom_path)
-
-    return 0
-
-
-if __name__ == '__main__':
-    exit(main())
+"""
+Dumps tag information from a DICOM file using information in PS3.6.
+"""
+
+import argparse
+import os
+import re
+
+from pydicom import dcmread
+from pydicom.errors import InvalidDicomError
+
+from dicom_validator.spec_reader.edition_reader import EditionReader
+
+
+class DataElementDumper:
+    tag_regex = re.compile(
+        r'(\(?[\dabcdefABCDEF]{4}), *([\dabcdefABCDEF]{4})\)?')
+
+    def __init__(self, dict_info, uid_info, max_value_len, show_image_data,
+                 tags):
+        self.dict_info = dict_info
+        self.max_value_len = max_value_len
+        self.level = 0
+        self.show_image_data = show_image_data
+
+        self.uid_info = {}
+        for uid_dict in uid_info.values():
+            self.uid_info.update(uid_dict)
+
+        tags = tags or []
+        self.tags = []
+        for tag in tags:
+            match = self.tag_regex.match(tag)
+            if match:
+                self.tags.append(
+                    '({},{})'.format(match.group(1), match.group(2)))
+            else:
+                matching = [tag_id for tag_id in dict_info
+                            if
+                            dict_info[tag_id]['name'].replace(" ", "") == tag]
+                if matching:
+                    self.tags.append(matching[0])
+                else:
+                    print('{} is not a valid tag expression - '
+                          'ignoring'.format(tag))
+
+    def print_dataset(self, dataset):
+        dataset.walk(
+            lambda data_set, data_elem: self.print_dataelement(data_set,
+                                                               data_elem))
+
+    def print_element(self, tag_id, name, vr, prop, value):
+        if self.tags and tag_id not in self.tags:
+            return False
+        vm = 1 if value else 0
+        if isinstance(value, list):
+            vm = len(value)
+            value = '\\'.join([str(element) for element in value])
+        if isinstance(value, bytes):
+            value = str(value)[2:-1]
+        if isinstance(value, str) and len(value) > self.max_value_len:
+            value = value[:self.max_value_len] + '...'
+
+        indent = 2 * self.level
+        format_string = '{{}}{{}} {{:{}}} {{}} {{:4}} {{}} [{{}}]'.format(
+            40 - indent)
+        print(format_string.format(' ' * indent,
+                                   tag_id,
+                                   name[:40 - indent],
+                                   vr,
+                                   vm,
+                                   prop,
+                                   value))
+        return True
+
+    def print_dataelement(self, _, dataelement):
+        tag_id = '({:04X},{:04X})'.format(dataelement.tag.group,
+                                          dataelement.tag.element)
+        description = self.dict_info.get(tag_id)
+        if description is None:
+            name = '[Unknown]'
+            vr = dataelement.VR
+            prop = ''
+        else:
+            vr = description['vr']
+            name = description['name']
+            prop = description['prop']
+        value = dataelement.value
+        if vr == 'UI':
+            # do not rely on pydicom here - we want to use the
+            # currently loaded DICOM spec
+            value = repr(value)[1:-1]
+            value = self.uid_info.get(value, value)
+        if vr == 'SQ':
+            if self.print_element(tag_id, name, vr, prop,
+                                  'Sequence with {} item(s)'.format(
+                                      len(value))):
+                self.level += 1
+                self.print_sequence(dataelement)
+                self.level -= 1
+        else:
+            self.print_element(tag_id, name, vr, prop, value)
+
+    def print_sequence(self, sequence):
+        indent = 2 * self.level
+        format_string = '{{}}Item {{:<{}}} [Dataset with {{}} element(s)]'\
+            .format(56 - indent)
+        for i, dataset in enumerate(sequence):
+            print(format_string.format(' ' * indent, i + 1, len(dataset)))
+            self.level += 1
+            dataset.walk(lambda data_set, data_elem:
+                         self.print_dataelement(data_set, data_elem))
+            self.level -= 1
+
+    def dump_file(self, file_path):
+        try:
+            print('\n' + file_path)
+            dataset = dcmread(
+                file_path, stop_before_pixels=self.show_image_data, force=True)
+            self.print_dataset(dataset)
+        except (InvalidDicomError, KeyError):
+            print(
+                '{} is not a valid DICOM file - skipping.'.format(file_path))
+
+    def dump_directory(self, dir_path):
+        for root, _, names in os.walk(dir_path):
+            for name in names:
+                self.dump_file(os.path.join(root, name))
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description='Dumps DICOM information dictionary from '
+                    'DICOM file using PS3.6')
+    parser.add_argument('dicomfiles',
+                        help='Path(s) of DICOM files or directories to parse',
+                        nargs='+')
+    parser.add_argument('--standard-path', '-src',
+                        help='Path with the DICOM specs in docbook '
+                             'and json format',
+                        default=os.path.join(os.path.expanduser("~"),
+                                             'dicom-validator'))
+    parser.add_argument('--revision', '-r',
+                        help='Standard revision (e.g. "2014c"), year of '
+                             'revision, "current" or "local" (latest '
+                             'locally installed)',
+                        default='current')
+    parser.add_argument('--max-value-len', '-ml',
+                        help='Maximum string length of displayed values',
+                        type=int,
+                        default=80)
+    parser.add_argument('--show-tags', '-t',
+                        help='Show only output for the searched tags. '
+                             'Tags can be in the format ####,#### or as the '
+                             'dictionary name (e.g. "PatientName").',
+                        nargs='*')
+    parser.add_argument('--show-image-data', '-id', action='store_false',
+                        help='Also show the image data tag (slower)')
+    args = parser.parse_args()
+
+    edition_reader = EditionReader(args.standard_path)
+    destination = edition_reader.get_revision(args.revision)
+    if destination is None:
+        print(
+            'Failed to get DICOM edition {} - aborting'.format(args.revision))
+        return 1
+
+    json_path = os.path.join(destination, 'json')
+    dict_info = EditionReader.load_dict_info(json_path)
+    uid_info = EditionReader.load_uid_info(json_path)
+    dumper = DataElementDumper(dict_info, uid_info, args.max_value_len,
+                               args.show_image_data,
+                               args.show_tags)
+    for dicom_path in args.dicomfiles:
+        if not os.path.exists(dicom_path):
+            print('\n"%s" does not exist - skipping', dicom_path)
+        else:
+            if os.path.isdir(dicom_path):
+                dumper.dump_directory(dicom_path)
+            else:
+                dumper.dump_file(dicom_path)
+
+    return 0
+
+
+if __name__ == '__main__':
+    exit(main())
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/condition.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/condition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,143 @@
-import json
-
-from dicom_validator.tag_tools import tag_name_from_id
-
-
-class Condition(object):
-    """ Represents a condition for the presence of a specific tag.
-
-    Attributes:
-        type: the type of the related object (tag or module) regarding its
-            existence; possible values:
-            'U': user defined, e.g. both existence or non-existence
-                of the related object is considered legal
-            'MN': the object is mandatory if the condition is fulfilled,
-                otherwise not
-            'MU': the object is mandatory if the condition is fulfilled,
-                otherwise is user defined
-        tag: the ID of the required tag in the form '(####,####)' or None
-        index: the index of the tag for multi-valued tags or 0
-        values: a list of values the tag shall have if the condition
-            is fulfilled, or None
-        operator: the comparison operation used ('=', '<', '>') for the
-            value(s), or None
-
-    """
-
-    def __init__(self, ctype=None, operator=None, tag=None, index=0,
-                 values=None):
-
-        self.type = ctype
-        self.operator = operator
-        self.tag = tag
-        self.index = index
-        self.values = values
-        self.and_conditions = []
-        self.or_conditions = []
-        self.other_condition = None
-
-    def read(self, json_string):
-        condition_dict = json.loads(json_string)
-        self.read_condition(condition_dict, self)
-
-    @classmethod
-    def read_condition(cls, condition_dict, condition=None):
-        condition = condition or Condition()
-        condition.type = condition_dict.get('type')
-        condition.operator = condition_dict.get('op')
-        condition.tag = condition_dict.get('tag')
-        condition.index = int(condition_dict.get('index', '0'))
-        condition.values = condition_dict.get('values')
-        and_list = condition_dict.get('and', [])
-        condition.and_conditions = [
-            cls.read_condition(cond) for cond in and_list]
-        or_list = condition_dict.get('or', [])
-        condition.or_conditions = [
-            cls.read_condition(cond) for cond in or_list
-        ]
-        if 'other_cond' in condition_dict:
-            condition.other_condition = cls.read_condition(
-                condition_dict['other_cond'])
-            condition.other_condition.type = condition_dict['other_cond'].get(
-                'type')
-        return condition
-
-    def dict(self):
-        result = {'type': self.type}
-        result.update(self.write_condition(self))
-        return result
-
-    @classmethod
-    def write_condition(cls, condition):
-        result = {}
-        if condition.operator is not None:
-            result['op'] = condition.operator
-        if condition.tag is not None:
-            result['tag'] = condition.tag
-            result['index'] = condition.index
-        if condition.values:
-            result['values'] = condition.values
-        if condition.and_conditions:
-            result['and'] = []
-            for and_condition in condition.and_conditions:
-                result['and'].append(cls.write_condition(and_condition))
-        if condition.or_conditions:
-            result['or'] = []
-            for or_condition in condition.or_conditions:
-                result['or'].append(cls.write_condition(or_condition))
-        if condition.other_condition:
-            result['other_cond'] = condition.other_condition.dict()
-        return result
-
-    def to_string(self, dict_info):
-        """Return a condition readable as part of a sentence."""
-        result = ''
-        if self.and_conditions:
-            return ' and '.join(
-                cond.to_string(dict_info) for cond in self.and_conditions)
-        if self.or_conditions:
-            return ' or '.join(
-                cond.to_string(dict_info) for cond in self.or_conditions)
-        if self.tag is not None:
-            if dict_info and self.tag in dict_info:
-                result = dict_info[self.tag]['name']
-            else:
-                result = self.tag
-            if self.index:
-                result += '[{}]'.format(self.index)
-        if self.operator == '+':
-            result += ' exists'
-        elif self.operator == '++':
-            result += ' exists and has a value'
-        elif self.operator == '=>':
-            tag_value = int(self.values[0])
-            result += ' points to ' + tag_name_from_id(tag_value, dict_info)
-        elif self.operator == '-':
-            result += ' is not present'
-        elif self.operator == '=':
-            result += ' is equal to '
-            values = ['"' + value + '"' for value in self.values]
-            if len(values) > 1:
-                result += ', '.join(values[:-1]) + ' or '
-            result += values[-1]
-        elif self.operator == '!=':
-            result += ' is not equal to '
-            values = ['"' + value + '"' for value in self.values]
-            if len(values) > 1:
-                result += ', '.join(values[:-1]) + ' and '
-            result += values[-1]
-        elif self.operator == '<':
-            result += ' is less than ' + self.values[0]
-        elif self.operator == '>':
-            result += ' is greater than ' + self.values[0]
-        return result
+from typing import Optional, List, Dict, Any
+
+from dicom_validator.tag_tools import tag_name_from_id
+
+
+class Condition:
+    """ Represents a condition for the presence of a specific tag.
+
+    Attributes:
+        type: the type of the related object (tag or module) regarding its
+            existence; possible values:
+            'U': user defined, e.g. both existence or non-existence
+                of the related object is considered legal
+            'MN': the object is mandatory if the condition is fulfilled,
+                otherwise not
+            'MU': the object is mandatory if the condition is fulfilled,
+                otherwise is user defined
+            'MC': the object is mandatory if the condition is fulfilled,
+                otherwise another condition will be checked
+        tag: the ID of the required tag in the form '(####,####)' or None
+        index: the index of the tag for multi-valued tags or 0
+        values: a list of values the tag shall have if the condition
+            is fulfilled, or None
+        operator: the comparison operation used ('=', '<', '>') for the
+            value(s), or None
+
+    """
+
+    def __init__(self, ctype: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 tag: Optional[str] = None,
+                 index: int = 0,
+                 values: Optional[List[str]] = None) -> None:
+        self.type = ctype
+        self.operator = operator
+        self.tag = tag
+        self.index = index
+        self.values = values or []
+        self.and_conditions: List[Condition] = []
+        self.or_conditions: List[Condition] = []
+        self.other_condition: Optional[Condition] = None
+
+    def __repr__(self):
+        return f"Condition type={self.type} op='{self.operator}' tag={self.tag} values={self.values}"
+
+    @classmethod
+    def read_condition(cls, condition_dict: Dict,
+                       condition: Optional["Condition"] = None) -> "Condition":
+        condition = condition or Condition()
+        condition.type = condition_dict.get('type')
+        condition.operator = condition_dict.get('op')
+        condition.tag = condition_dict.get('tag')
+        condition.index = int(condition_dict.get('index', '0'))
+        condition.values = condition_dict.get('values', [])
+        and_list = condition_dict.get('and', [])
+        condition.and_conditions = [
+            cls.read_condition(cond) for cond in and_list]
+        or_list = condition_dict.get('or', [])
+        condition.or_conditions = [
+            cls.read_condition(cond) for cond in or_list
+        ]
+        if 'other_cond' in condition_dict:
+            condition.other_condition = cls.read_condition(
+                condition_dict['other_cond'])
+            condition.other_condition.type = condition_dict['other_cond'].get(
+                'type')
+        return condition
+
+    def dict(self) -> Dict[str, Any]:
+        result = {'type': self.type}
+        result.update(self.write_condition(self))
+        return result
+
+    @classmethod
+    def write_condition(cls, condition: "Condition") -> Dict[str, Any]:
+        result: Dict[str, Any] = {}
+        if condition.operator is not None:
+            result['op'] = condition.operator
+        if condition.tag is not None:
+            result['tag'] = condition.tag
+            result['index'] = condition.index
+        if condition.values:
+            result['values'] = condition.values
+        if condition.and_conditions:
+            result['and'] = []
+            for and_condition in condition.and_conditions:
+                result['and'].append(cls.write_condition(and_condition))
+        if condition.or_conditions:
+            result['or'] = []
+            for or_condition in condition.or_conditions:
+                result['or'].append(cls.write_condition(or_condition))
+        if condition.other_condition is not None:
+            result['other_cond'] = condition.other_condition.dict()
+        return result
+
+    def to_string(self, dict_info: Dict) -> str:
+        """Return a condition readable as part of a sentence."""
+        result = ''
+        if self.and_conditions:
+            return ' and '.join(
+                cond.to_string(dict_info) for cond in self.and_conditions)
+        if self.or_conditions:
+            return ' or '.join(
+                cond.to_string(dict_info) for cond in self.or_conditions)
+        if self.tag is not None:
+            if dict_info and self.tag in dict_info:
+                result = dict_info[self.tag]['name']
+            else:
+                result = self.tag
+            if self.index:
+                result += '[{}]'.format(self.index)
+        if self.operator is None:
+            return result
+        if self.operator == '+':
+            result += ' exists'
+        elif self.operator == '++':
+            result += ' exists and has a value'
+        elif self.operator == '-':
+            result += ' is not present'
+        elif self.operator == '=>':
+            tag_value = int(self.values[0])
+            result += ' points to ' + tag_name_from_id(tag_value, dict_info)
+        elif not self.values:
+            # if no values are found here, we have some unhandled condition
+            # and ignore it for the time being
+            return result
+        elif self.operator == '=':
+            values = ['"' + value + '"' for value in self.values]
+            result += ' is equal to '
+            if len(values) > 1:
+                result += ', '.join(values[:-1]) + ' or '
+            result += values[-1]
+        elif self.operator == '!=':
+            values = ['"' + value + '"' for value in self.values]
+            result += ' is not equal to '
+            if len(values) > 1:
+                result += ', '.join(values[:-1]) + ' and '
+            result += values[-1]
+        elif self.operator == '<':
+            result += ' is less than ' + self.values[0]
+        elif self.operator == '>':
+            result += ' is greater than ' + self.values[0]
+        return result
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/condition_parser.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/condition_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,286 +1,396 @@
-import re
-from collections import OrderedDict
-
-from dicom_validator.spec_reader.condition import Condition
-
-
-class ConditionParser(object):
-    """Parses the description of type C modules and type 1C and 2C attributes.
-    Creates a Condition object representing the condition(s) in the
-    description provided that:
-    - the condition is related to the value, absence or presence of one
-        or more tags in the data set
-    - the condition is related only to the data set itself
-    All other conditions (including parsable conditions which reference
-    other data sets) are ignored.
-    The following operators are used for conditions:
-    '+' - required if the given tag is present
-    '++' - required if the given tag is present and has a value
-    '-' - required if the given tag is absent
-    '=' - required if the given tag has one of the given values
-    '!=' - required if the given tag does not have one of the given values
-    '>' - required if the given tag value is greater than the given value
-    '<' - required if the given tag value is less than the given value
-    '=>' - required if the given tag points to one of the given tags
-    """
-
-    tag_expression = re.compile(
-        r'(the value of )?(?P<name>[a-zA-Z1-9 \'\-]+)'
-        r'(?P<id>\([\dA-Fa-f]{4},[\dA-Fa-f]{4}\))?(,? Value (?P<index>\d))?$')
-
-    operators = OrderedDict([
-        (' is greater than ', '>'),
-        (' is present and equals ', '='),
-        (' is present with a value of ', '='),
-        (' value is ', '='),
-        (' has a value of more than ', '>'),
-        (' has a value greater than ', '>'),
-        (' has a value of ', '='),
-        (' = ', '='),
-        (' at the image level equals ', '='),
-        (' equals other than ', '!='),
-        (' equals ', '='),
-        (' is other than ', '!='),
-        (' is present and the value is ', '='),
-        (' is present and has a value of ', '='),
-        (' is present and has a value', '++'),
-        (' is present', '+'),
-        (' is sent', '+'),
-        (' is not sent', '-'),
-        (' is not present', '-'),
-        (' is absent', '-'),
-        (' is not equal to ', '!='),
-        (' is not ', '!='),
-        (' is ', '='),
-        (' is: ', '='),
-        (' are not present', '-'),
-        (' are present', '+'),
-        (' points to ', '=>')
-    ])
-
-    logical_ops = OrderedDict([
-        ('and if', 'and'),
-        ('and', 'and'),
-        ('or if', 'or'),
-        ('or', 'or')
-    ])
-
-    def __init__(self, dict_info):
-        self._dict_info = dict_info
-
-    def parse(self, condition):
-        """Parse the given condition string and return a Condition object
-         with the required attributes.
-        """
-        condition_prefixes = ('required if ', 'shall be present if ')
-        for prefix in condition_prefixes:
-            index = condition.lower().find(prefix)
-            if index >= 0:
-                condition = condition[len(prefix) + index:]
-                condition = self._fix_condition(condition)
-                return self._parse_tag_expressions(condition)
-        return Condition(ctype='U')
-
-    def _parse_tag_expression(self, condition):
-        operator_text = None
-        op_offset = None
-        for operator in self.operators:
-            offset = condition.find(operator)
-            if offset > 0 and (op_offset is None or offset < op_offset):
-                op_offset = offset
-                operator_text = operator
-        if operator_text is None:
-            return Condition(ctype='U'), None
-        operator = self.operators[operator_text]
-        rest = condition[op_offset + len(operator_text):]
-        if self.operators[operator_text] in ('=', '!=', '>', '<'):
-            values, rest = self._parse_tag_values(rest)
-        elif self.operators[operator_text] == '=>':
-            value_string, rest = self.extract_value_string(rest)
-            tag, _ = self._parse_tag(value_string)
-            if tag is None:
-                return Condition(ctype='U'), None
-            values, rest = [str(self._tag_id(tag))], rest
-        else:
-            values, rest = None, rest.strip()
-        result = self._parse_tags(condition[:op_offset], operator, values)
-        if not result:
-            return Condition(ctype='U'), None
-
-        result.type = ('MU' if 'may be present otherwise'
-                               in condition[op_offset:].lower() else 'MN')
-        return result, rest
-
-    def _get_other_condition(self, condition_string):
-        other_cond_texts = [
-            'may be present otherwise if ', 'may be present if '
-        ]
-        for condition_marker in other_cond_texts:
-            index = condition_string.lower().find(condition_marker)
-            if index >= 0:
-                return self._parse_tag_expressions(
-                    condition_string[index + len(condition_marker):])
-
-    @staticmethod
-    def _tag_id(tag_id_string):
-        group, element = tag_id_string[1:-1].split(',')
-        return (int(group, 16) << 16) + int(element, 16)
-
-    def _parse_tag(self, tag_string):
-        match = self.tag_expression.match(tag_string.strip())
-        if match:
-            value_index = (0 if match.group('index') is None
-                           else int(match.group('index')) - 1)
-            if match.group('id') is not None:
-                return match.group('id'), value_index
-            tag_name = match.group('name').strip()
-            for tag_id, entry in self._dict_info.items():
-                if entry['name'] == tag_name:
-                    return tag_id, value_index
-        return None, None
-
-    def _parse_tag_values(self, value_string):
-        value_string, rest = self.extract_value_string(value_string)
-        values = value_string.split(', ')
-        tag_values = []
-        for value in values:
-            if ' or ' in value:
-                tag_values.extend(value.split(' or '))
-            elif value.startswith('or '):
-                tag_values.append(value[3:])
-            else:
-                tag_values.append(value)
-        values = []
-        for value in tag_values:
-            value = value.strip()
-            if value.startswith('"') and value.endswith('"'):
-                value = value[1:-1].strip()
-            values.append(value)
-        return values, rest
-
-    def extract_value_string(self, value_string):
-        # remove stuff that breaks parser
-        value_string = value_string.replace('(Legacy Converted)', '')
-        start_index = 0
-        rest = None
-        while True:
-            end_index = -1
-            # todo: handle or
-            for end_char in (';', '.', 'and ', ', or ', ' or '):
-                char_index = value_string.find(end_char, start_index)
-                if end_index < 0 or 0 <= char_index < end_index:
-                    end_index = char_index
-            apo_index = value_string.find('"', start_index)
-            if end_index < 0:
-                break
-            if 0 <= apo_index < end_index:
-                start_index = value_string.find('"', apo_index + 1) + 1
-                continue
-            if end_index > 0:
-                if value_string.find(' or ') in [end_index, end_index + 1]:
-                    # differentiate between several values and several
-                    # conditions - check if the rest is a condition
-                    or_cond = self._parse_tag_expressions(
-                        value_string[end_index + 3:])
-                    if or_cond.type == 'U':
-                        start_index = end_index + 4
-                        continue
-                rest = value_string[end_index:].strip()
-                value_string = value_string[:end_index]
-                break
-        return value_string, rest
-
-    def _parse_tag_expressions(self, condition, nested=False):
-        result, rest = self._parse_tag_expression(condition)
-        if rest is not None:
-            if rest.startswith(', '):
-                rest = rest[2:]
-            logical_op = None
-            for operator in self.logical_ops:
-                if rest.startswith(operator + ' '):
-                    logical_op = self.logical_ops[operator]
-                    condition = rest[len(operator) + 1:]
-                    break
-            if logical_op is not None:
-                next_result = self._parse_tag_expressions(
-                    condition, nested=True)
-                if next_result.type != 'U':
-                    next_result.type = None
-                    new_result = Condition(ctype=result.type)
-                    cond_list = self._condition_list(logical_op, new_result)
-                    cond_list.append(result)
-                    cond_list.append(next_result)
-                    result.type = None
-                    result = new_result
-        if not nested and rest is not None:
-            other_cond = self._get_other_condition(rest)
-            if other_cond is not None and other_cond.type != 'U':
-                result.type = 'MC'
-                result.other_condition = other_cond
-        return result
-
-    def _parse_tags(self, condition, operator, values):
-        # this handles only a few cases that are actually found
-        if ', and ' in condition:
-            return self._parse_tag_composition(
-                condition, operator, values, 'and')
-        if ', or ' in condition:
-            return self._parse_tag_composition(
-                condition, operator, values, 'or')
-        if ' and ' in condition:
-            return self._parse_multiple_tags(
-                condition, operator, values, 'and')
-        if ' or ' in condition:
-            return self._parse_multiple_tags(
-                condition, operator, values, 'or')
-        return self._result_from_tag_string(condition, operator, values)
-
-    def _parse_tag_composition(self, condition, operator, values, logical_op):
-        split_string = ', {} '.format(logical_op)
-        conditions = condition.split(split_string)
-        result0 = self._parse_tags(conditions[0], operator, values)
-        if not result0:
-            result = self._parse_tags(condition.replace(
-                split_string, split_string.replace(',', '')), operator, values)
-        else:
-            result = Condition()
-            cond_list = self._condition_list(logical_op, result)
-            cond_list.append(result0)
-            cond_list.append(self._parse_tags(conditions[1], operator, values))
-        return result
-
-    def _parse_multiple_tags(self, condition, operator, values, logical_op):
-        condition = condition.replace(' {} '.format(logical_op), ', ')
-        result = Condition()
-        cond_list = self._condition_list(logical_op, result)
-        for tag_string in condition.split(', '):
-            tag_result = self._result_from_tag_string(
-                tag_string, operator, values)
-            if tag_result:
-                cond_list.append(tag_result)
-        if len(cond_list) > 1:
-            return result
-
-    @staticmethod
-    def _condition_list(logical_op, result):
-        cond_list = (result.and_conditions if logical_op == 'and'
-                     else result.or_conditions)
-        return cond_list
-
-    def _result_from_tag_string(self, tag_string, operator, values):
-        tag, index = self._parse_tag(tag_string)
-        if tag is not None:
-            result = Condition(tag=tag, index=index, operator=operator)
-            if values:
-                result.values = values
-            return result
-
-    @staticmethod
-    def _fix_condition(condition):
-        index = condition.lower().find(' may be present otherwise')
-        if index > 0:
-            if condition[index - 1] == ',':
-                condition = condition[:index - 1] + '.' + condition[index:]
-            elif condition[index - 1] != '.':
-                condition = condition[:index] + '.' + condition[index:]
-        return condition
+import re
+from collections import OrderedDict
+from typing import Dict, Tuple, Optional, List
+
+from dicom_validator.spec_reader.condition import Condition
+
+
+class ConditionParser:
+    """Parses the description of type C modules and type 1C and 2C attributes.
+    Creates a Condition object representing the condition(s) in the
+    description provided that:
+    - the condition is related to the value, absence or presence of one
+        or more tags in the data set
+    - the condition is related only to the data set itself
+    All other conditions (including parsable conditions which reference
+    other data sets) are ignored.
+    The following operators are used for conditions:
+    '+' - required if the given tag is present
+    '++' - required if the given tag is present and has a value
+    '-' - required if the given tag is absent
+    '=' - required if the given tag has one of the given values
+    '!=' - required if the given tag does not have one of the given values
+    '>' - required if the given tag value is greater than the given value
+    '<' - required if the given tag value is less than the given value
+    '=>' - required if the given tag points to one of the given tags
+    """
+    all_conditions = {}
+
+    tag_expression = re.compile(
+        r'(the value of )?(?P<name>[a-zA-Z1-9 \'\-]+)'
+        r'(?P<id>\([\dA-Fa-f]{4},[\dA-Fa-f]{4}\))?(,? Value (?P<index>\d))?$')
+
+    operators = OrderedDict([
+        (' is present and the value is ', '='),
+        (' is present and has a value of ', '='),
+        (' is greater than ', '>'),
+        (' is present and equals ', '='),
+        (' is present with a value of ', '='),
+        (' is set to ', '='),
+        (' equals one of the following values: ', '='),
+        (' has a value of more than ', '>'),
+        (' has a value greater than ', '>'),
+        (' has a value of ', '='),
+        (' = ', '='),
+        (' at the image level equals ', '='),
+        (' equals other than ', '!='),
+        (' equals ', '='),
+        (' is other than ', '!='),
+        (' is one of the following: ', '='),
+        (' is present and has a value', '++'),
+        (' is present', '+'),
+        (' value is not ', '!='),
+        (' value is ', '='),
+        (' is sent', '+'),
+        (' is not sent', '-'),
+        (' is not present', '-'),
+        (' is absent', '-'),
+        (' is not equal to ', '!='),
+        (' is equal to ', '='),
+        (' is not ', '!='),
+        (' is ', '='),
+        (' is: ', '='),
+        (' are not present', '-'),
+        (' are present', '+'),
+        (' points to ', '=>')
+    ])
+
+    logical_ops = OrderedDict([
+        ('and if', 'and'),
+        ('and whose', 'and'),
+        ('and', 'and'),
+        ('or if', 'or'),
+        ('or', 'or')
+    ])
+
+    def __init__(self, dict_info: Dict) -> None:
+        self._dict_info = dict_info
+        self._uid_dict_info = {}
+        for tag, info in dict_info.items():
+            if info['name'].endswith(' UID'):
+                uid_info = info.copy()
+                uid_info['name'] = uid_info['name'][:-4]
+                self._uid_dict_info[tag] = uid_info
+
+    def parse(self, condition_str: str) -> Condition:
+        """Parse the given condition string and return a Condition object
+         with the required attributes.
+        """
+        condition_prefixes = (
+            'required if ', 'shall be present if ',
+            'required for images where ', 'required only if'
+        )
+        for prefix in condition_prefixes:
+            index = condition_str.lower().find(prefix)
+            if index >= 0:
+                condition_str = condition_str[len(prefix) + index:]
+                condition_str = self._fix_condition(condition_str)
+                condition = self._parse_tag_expressions(condition_str)
+                self.__class__.all_conditions[condition_str] = (
+                    condition.to_string(self._dict_info)
+                )
+                return condition
+        self.__class__.all_conditions[condition_str] = Condition(ctype='U')
+        return Condition(ctype='U')
+
+    def _parse_tag_expression(
+            self, condition: str) -> Tuple[Condition, Optional[str]]:
+        operator_text = None
+        op_offset = None
+        for operator in self.operators:
+            offset = condition.find(operator)
+            if offset > 0 and (op_offset is None or offset < op_offset):
+                op_offset = offset
+                operator_text = operator
+        if operator_text is None or op_offset is None:
+            return Condition(ctype='U'), None
+        operator = self.operators[operator_text]
+        rest = condition[op_offset + len(operator_text):]
+        if operator in ('=', '!=', '>', '<'):
+            values, rest = self._parse_tag_values(rest)
+            # fixup special values
+            if values:
+                if values[0].startswith('non-zero'):
+                    operator = '!='
+                    values = ['0'] if values[0] == 'non-zero' else ['']
+                elif values[0].startswith('non-null'):
+                    operator = '++'
+                    values = []
+                elif values[0].startswith('zero-length'):
+                    values = ['']
+            else:
+                # failed to parse mandatory values - ignore the condition
+                return Condition(ctype='U'), None
+        elif operator == '=>':
+            value_string, rest = self._split_value_part(rest)
+            tag, _ = self._parse_tag(value_string)
+            if tag is None:
+                return Condition(ctype='U'), None
+            values, rest = [str(self._tag_id(tag))], rest
+        else:
+            values, rest = [], rest.strip()
+        result = self._parse_tags(condition[:op_offset], operator, values)
+        if not result:
+            return Condition(ctype='U'), None
+
+        result.type = ('MU' if 'may be present otherwise'
+                               in condition[op_offset:].lower() else 'MN')
+        return result, rest
+
+    def _get_other_condition(
+            self, condition_string: str) -> Optional[Condition]:
+        match = re.match('.*(may be present( [a-z]+( [a-z]+)*)? if ).*',
+                         condition_string.lower())
+        if match is not None:
+            marker = match.group(1)
+            index = condition_string.lower().find(marker)
+            return self._parse_tag_expressions(
+                condition_string[index + len(marker):])
+        return None
+
+    @staticmethod
+    def _tag_id(tag_id_string: str) -> int:
+        group, element = tag_id_string[1:-1].split(',')
+        return (int(group, 16) << 16) + int(element, 16)
+
+    def _parse_tag(
+            self, tag_string: str) -> Tuple[Optional[str], Optional[int]]:
+        match = self.tag_expression.match(tag_string.strip())
+        if match:
+            value_index = (0 if match.group('index') is None
+                           else int(match.group('index')) - 1)
+            if match.group('id') is not None:
+                return match.group('id'), value_index
+            tag_name = match.group('name').strip()
+            for tag_id, entry in self._dict_info.items():
+                if entry['name'] == tag_name:
+                    return tag_id, value_index
+            for tag_id, entry in self._uid_dict_info.items():
+                if entry['name'] == tag_name:
+                    return tag_id, value_index
+        return None, None
+
+    def _parse_tag_values(
+            self, value_string: str) -> Tuple[List[str], str]:
+        value_part, rest = self._split_value_part(value_string)
+        values = []
+        value_index = 0
+        last_or = None
+        while value_index >= 0:
+            value_index = -1
+            current_or = None
+            for or_phrase in self._valid_or_expressions_after_or_expression(
+                last_or
+            ):
+                index = value_part.find(or_phrase)
+                if index >= 0 and (value_index < 0 or index < value_index):
+                    value_index = index
+                    next_index = index + len(or_phrase)
+                    current_or = or_phrase
+            if value_index > 0:
+                value, value_rest = self._get_const_value(
+                    value_part[:value_index])
+                if value is None:
+                    return values, current_or + value_part + rest
+                values.append(value)
+                if value_rest:
+                    return values, current_or + value_rest + rest
+                value_part = value_part[next_index:]
+                last_or = current_or
+        value, value_rest = self._get_const_value(value_part)
+        if value is None:
+            return values, value_part + rest
+        values.append(value)
+        return values, value_rest + rest
+
+    def _split_value_part(self, value_string: str) -> Tuple[str, str]:
+        value_string = value_string.strip()
+        end_index = self._end_index_for_stop_chars(
+            value_string, [';', '.', ', and ', ' and ', ':'])
+        return value_string[:end_index], value_string[end_index:]
+
+    @staticmethod
+    def _valid_or_expressions_after_or_expression(
+            previous_expr: Optional[str]) -> List[str]:
+        if previous_expr is None:
+            return [', ', ' or ']
+        if previous_expr == ' or ':
+            return [' or ']
+        if previous_expr == ', ':
+            return [', or ', ', ', ' or ']
+        return []
+
+    @staticmethod
+    def _index_is_inside_string(value: str, index: int) -> bool:
+        in_string = False
+        apo_index = 0
+        while apo_index >= 0:
+            apo_index = value.find('"', apo_index, index)
+            if apo_index >= 0:
+                apo_index += 1
+                in_string = not in_string
+        return in_string
+
+    def _get_const_value(self, value: str) -> Tuple[Optional[str], str]:
+        value = value.strip()
+        if value[0] == value[-1] == '"':
+            return value[1:-1], ''
+        if re.match('^[A-Z0-9][A-Za-z0-9_ ]*$', value) is not None:
+            return value, ''
+        # sometimes a value explanation is present in scopes
+        match = re.match(r'^([A-Z0-9_ ]+)\([A-Za-z ]+\)+$', value)
+        if match is not None:
+            return match.group(1).strip(), ''
+        if value == 'zero length':
+            return '', ''
+        if value == 'zero':
+            return '0', ''
+        if value in ('non-zero', 'non-zero length', 'non-null', 'zero-length'):
+            return value, ''
+        match = re.match(r'^.* \(\"([\d.]+)\"\)(.*)$', value)
+        if match is not None:
+            return match.group(1), match.group(2)
+        tag, index = self._parse_tag(value)
+        if tag is not None:
+            return value, ''
+        return None, ''
+
+    def _end_index_for_stop_chars(
+            self, value: str, stop_chars: List[str]) -> int:
+        end_index = len(value)
+        for stop_char in stop_chars:
+            start_index = 0
+            stop_index = 0
+            while stop_index >= 0:
+                stop_index = value.find(
+                    stop_char, start_index, end_index)
+                if stop_index < 0:
+                    break
+                if self._index_is_inside_string(value, stop_index):
+                    start_index = stop_index + 1
+                else:
+                    end_index = stop_index
+                    break
+        return end_index
+
+    def _parse_tag_expressions(
+            self, condition: str, nested: bool = False) -> Condition:
+        result, rest = self._parse_tag_expression(condition)
+        if rest is not None:
+            rest = rest.strip()
+            if rest.startswith(', '):
+                rest = rest[2:]
+            logical_op = None
+            for operator in self.logical_ops:
+                if rest.startswith(operator + ' '):
+                    logical_op = self.logical_ops[operator]
+                    condition = rest[len(operator) + 1:]
+                    break
+            if logical_op is not None:
+                next_result = self._parse_tag_expressions(
+                    condition, nested=True)
+                if next_result.type != 'U':
+                    next_result.type = None
+                    new_result = Condition(ctype=result.type)
+                    cond_list = self._condition_list(logical_op, new_result)
+                    cond_list.append(result)
+                    cond_list.append(next_result)
+                    result.type = None
+                    result = new_result
+        if not nested and rest is not None:
+            other_cond = self._get_other_condition(rest)
+            if other_cond is not None and other_cond.type != 'U':
+                result.type = 'MC'
+                result.other_condition = other_cond
+        return result
+
+    def _parse_tags(
+            self, condition: str, operator: str, values: List[str]
+    ) -> Optional[Condition]:
+        # this handles only a few cases that are actually found
+        if ', and ' in condition:
+            return self._parse_tag_composition(
+                condition, operator, values, 'and')
+        if ', or ' in condition:
+            return self._parse_tag_composition(
+                condition, operator, values, 'or')
+        if ' and ' in condition:
+            return self._parse_multiple_tags(
+                condition, operator, values, 'and')
+        if ' or ' in condition:
+            return self._parse_multiple_tags(
+                condition, operator, values, 'or')
+        return self._result_from_tag_string(condition, operator, values)
+
+    def _parse_tag_composition(
+            self, condition_str: str, operator: str,
+            values: List[str], logical_op: str
+    ) -> Optional[Condition]:
+        split_string = ', {} '.format(logical_op)
+        conditions = condition_str.split(split_string)
+        result0 = self._parse_tags(conditions[0], operator, values)
+        if result0 is None:
+            result = self._parse_tags(condition_str.replace(
+                split_string, split_string.replace(',', '')), operator, values)
+        else:
+            result = Condition()
+            cond_list = self._condition_list(logical_op, result)
+            cond_list.append(result0)
+            condition = self._parse_tags(conditions[1], operator, values)
+            if condition is not None:
+                cond_list.append(condition)
+        return result
+
+    def _parse_multiple_tags(
+            self, condition: str, operator: str,
+            values: List[str], logical_op: str
+    ) -> Optional[Condition]:
+        condition = condition.replace(' {} '.format(logical_op), ', ')
+        result = Condition()
+        cond_list = self._condition_list(logical_op, result)
+        for tag_string in condition.split(', '):
+            tag_result = self._result_from_tag_string(
+                tag_string, operator, values)
+            if tag_result:
+                cond_list.append(tag_result)
+        if len(cond_list) > 1:
+            return result
+        return None
+
+    @staticmethod
+    def _condition_list(logical_op: str, result: Condition) -> List[Condition]:
+        cond_list = (result.and_conditions if logical_op == 'and'
+                     else result.or_conditions)
+        return cond_list
+
+    def _result_from_tag_string(
+            self, tag_string: str, operator: str, values: List[str]
+    ) -> Optional[Condition]:
+        tag, index = self._parse_tag(tag_string)
+        if tag is not None:
+            result = Condition(tag=tag, index=index, operator=operator)
+            if values:
+                result.values = values
+            return result
+        return None
+
+    @staticmethod
+    def _fix_condition(condition: str) -> str:
+        condition = condition.replace('(Legacy Converted)', '')
+        index = condition.lower().find(' may be present otherwise')
+        if index > 0:
+            if condition[index - 1] == ',':
+                condition = condition[:index - 1] + '.' + condition[index:]
+            elif condition[index - 1] != '.':
+                condition = condition[:index] + '.' + condition[index:]
+        return condition
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/edition_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/edition_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,274 +1,274 @@
-import datetime
-import json
-import logging
-import os
-import re
-import sys
-from abc import ABC
-
-from dicom_validator import __version__
-from dicom_validator.spec_reader.part3_reader import Part3Reader
-from dicom_validator.spec_reader.part4_reader import Part4Reader
-from dicom_validator.spec_reader.part6_reader import Part6Reader
-from dicom_validator.spec_reader.serializer import DefinitionEncoder
-
-from urllib.request import urlretrieve
-
-import html.parser as html_parser
-
-
-class EditionParser(html_parser.HTMLParser, ABC):
-    edition_re = re.compile(r'\d\d\d\d[a-h]')
-
-    def __init__(self):
-        html_parser.HTMLParser.__init__(self)
-        self._in_anchor = False
-        self.editions = []
-
-    def handle_starttag(self, tag, attrs):
-        if tag == 'a':
-            self._in_anchor = True
-
-    def handle_endtag(self, tag):
-        if tag == 'a':
-            self._in_anchor = False
-
-    def handle_data(self, data):
-        if self._in_anchor and self.edition_re.match(data):
-            self.editions.append(data)
-
-
-class EditionReader(object):
-    base_url = 'http://dicom.nema.org/medical/dicom/'
-    html_filename = 'editions.html'
-    json_filename = 'editions.json'
-    iod_info_json = 'iod_info.json'
-    module_info_json = 'module_info.json'
-    dict_info_json = 'dict_info.json'
-    uid_info_json = 'uid_info.json'
-
-    def __init__(self, path):
-        self.path = path
-        self.logger = logging.getLogger()
-        if not self.logger.handlers:
-            self.logger.addHandler(logging.StreamHandler(sys.stdout))
-
-    def update_edition(self):
-        try:
-            self.logger.info('Getting DICOM editions...')
-            self.retrieve(os.path.join(self.path, self.html_filename))
-            self.write_to_json()
-        except BaseException as exception:
-            self.logger.warning(u'Failed to get DICOM read_from_html: %s',
-                                str(exception))
-
-    def retrieve(self, html_path):
-        if not os.path.exists(os.path.dirname(html_path)):
-            os.makedirs(os.path.dirname(html_path))
-        urlretrieve(self.base_url, html_path)
-
-    def get_editions(self, update=True):
-        editions_path = os.path.join(self.path, self.json_filename)
-        if os.path.exists(editions_path):
-            if update:
-                today = datetime.datetime.today()
-                modified_date = datetime.datetime.fromtimestamp(
-                    os.path.getmtime(editions_path))
-                # no need to update the edition dir more than once a month
-                update = (today - modified_date).days > 30
-            else:
-                with open(editions_path) as f:
-                    update = not json.load(f)
-        else:
-            update = True
-        if update:
-            self.update_edition()
-        if os.path.exists(editions_path):
-            with open(editions_path) as json_file:
-                return json.load(json_file)
-
-    def read_from_html(self):
-        html_path = os.path.join(self.path, self.html_filename)
-        with open(html_path) as html_file:
-            contents = html_file.read()
-        parser = EditionParser()
-        parser.feed(contents)
-        parser.close()
-        return parser.editions
-
-    def write_to_json(self):
-        editions = self.read_from_html()
-        if editions:
-            json_path = os.path.join(self.path, self.json_filename)
-            with open(json_path, 'w') as json_file:
-                json_file.write(json.dumps(editions))
-
-    def get_edition(self, revision):
-        """Get the edition matching the revision or None.
-        The revision can be the edition name, the year of the edition,
-        'current', or 'local'.
-        """
-        editions = sorted(self.get_editions(revision != 'local'))
-        if revision in editions:
-            return revision
-        if len(revision) == 4:
-            for edition in reversed(editions):
-                if edition.startswith(revision):
-                    return edition
-        if revision == 'current' or revision == 'local':
-            return editions[-1]
-
-    def is_current(self, revision):
-        """Get the edition matching the revision or None.
-        The revision can be the edition name, the year of the edition,
-        or 'current'.
-        """
-        if revision is None:
-            return True
-        editions = sorted(self.get_editions(revision != 'local'))
-        if revision in editions:
-            return revision == editions[-1]
-        if len(revision) == 4:
-            return editions[-1].startswith(revision)
-        if revision == 'current':
-            return True
-        return False
-
-    def check_revision(self, revision):
-        # none revision is used if an existing path points to the specs
-        if revision != 'none':
-            revision = self.get_edition(revision)
-            if revision:
-                return revision, os.path.join(self.path, revision)
-            return None, None
-        return None, self.path
-
-    def get_chapter(self, revision, chapter, destination, is_current):
-        file_path = os.path.join(destination, 'part{:02}.xml'.format(chapter))
-        if os.path.exists(file_path):
-            return True
-        elif not revision:
-            print('Chapter {} not present at {}.'.format(chapter, file_path))
-            return False
-        revision_dir = 'current' if is_current else revision
-        url = '{0}{1}/source/docbook/part{2:02}/part{2:02}.xml'.format(
-            self.base_url, revision_dir, chapter)
-        try:
-            print('Downloading DICOM spec {} PS3.{}...'.format(revision,
-                                                               chapter))
-            urlretrieve(url, file_path)
-            return True
-        except BaseException as exception:
-            print(u'Failed to download {}: {}'.format(url, str(exception)))
-            if os.path.exists(file_path):
-                try:
-                    os.remove(file_path)
-                except OSError:
-                    print('Failed to remove incomplete file {}.'.format(
-                        file_path))
-            return False
-
-    @staticmethod
-    def load_info(json_path, info_json):
-        with open(os.path.join(json_path,
-                               info_json)) as info_file:
-            return json.load(info_file)
-
-    @classmethod
-    def load_dict_info(cls, json_path):
-        return cls.load_info(json_path, cls.dict_info_json)
-
-    @classmethod
-    def load_uid_info(cls, json_path):
-        return cls.load_info(json_path, cls.uid_info_json)
-
-    @classmethod
-    def load_iod_info(cls, json_path):
-        return cls.load_info(json_path, cls.iod_info_json)
-
-    @classmethod
-    def load_module_info(cls, json_path):
-        return cls.load_info(json_path, cls.module_info_json)
-
-    @classmethod
-    def json_files_exist(cls, json_path):
-        for filename in (cls.dict_info_json, cls.module_info_json,
-                         cls.iod_info_json, cls.uid_info_json):
-            if not os.path.exists(os.path.join(json_path, filename)):
-                return False
-        return True
-
-    @classmethod
-    def dump_description(cls, description):
-        return json.dumps(description, sort_keys=True,
-                          indent=2, cls=DefinitionEncoder)
-
-    @classmethod
-    def create_json_files(cls, docbook_path, json_path):
-        print('Creating JSON excerpts from docbook files...')
-        part6reader = Part6Reader(docbook_path)
-        dict_info = part6reader.data_elements()
-        part3reader = Part3Reader(docbook_path, dict_info)
-        part4reader = Part4Reader(docbook_path)
-        iod_info = part3reader.iod_descriptions()
-        chapter_info = part4reader.iod_chapters()
-        definition = {}
-        for chapter in iod_info:
-            if chapter in chapter_info:
-                for uid in chapter_info[chapter]:
-                    definition[uid] = iod_info[chapter]
-        with open(os.path.join(json_path, cls.iod_info_json),
-                  'w') as info_file:
-            info_file.write(cls.dump_description(definition))
-        with open(os.path.join(json_path, cls.module_info_json),
-                  'w') as info_file:
-            info_file.write(
-                cls.dump_description(part3reader.module_descriptions()))
-        with open(os.path.join(json_path, cls.dict_info_json),
-                  'w') as info_file:
-            info_file.write(cls.dump_description(dict_info))
-        with open(os.path.join(json_path, cls.uid_info_json),
-                  'w') as info_file:
-            info_file.write(cls.dump_description(part6reader.all_uids()))
-        cls.write_current_version(json_path)
-        print('Done!')
-
-    def get_revision(self, revision):
-        revision, destination = self.check_revision(revision)
-        if destination is None:
-            print('DICOM revision {} not found.'.format(revision))
-            return
-
-        docbook_path = os.path.join(destination, 'docbook')
-        if not os.path.exists(docbook_path):
-            os.makedirs(docbook_path)
-        json_path = os.path.join(destination, 'json')
-        if not os.path.exists(json_path):
-            os.makedirs(json_path)
-
-        # download the docbook files
-        for chapter in [3, 4, 6]:
-            if not self.get_chapter(revision=revision, chapter=chapter,
-                                    destination=docbook_path,
-                                    is_current=self.is_current(revision)):
-                return
-
-        if (not self.json_files_exist(json_path) or
-                not self.is_current_version(json_path)):
-            self.create_json_files(docbook_path, json_path)
-        print('Using DICOM revision {}'.format(revision))
-        return destination
-
-    @staticmethod
-    def is_current_version(json_path):
-        version_path = os.path.join(json_path, 'version')
-        if not os.path.exists(version_path):
-            return False
-        with open(version_path) as f:
-            return f.read() >= __version__
-
-    @staticmethod
-    def write_current_version(json_path):
-        version_path = os.path.join(json_path, 'version')
-        with open(version_path, 'w') as f:
-            f.write(__version__)
+import datetime
+import json
+import logging
+import os
+import re
+import sys
+from abc import ABC
+
+from dicom_validator import __version__
+from dicom_validator.spec_reader.part3_reader import Part3Reader
+from dicom_validator.spec_reader.part4_reader import Part4Reader
+from dicom_validator.spec_reader.part6_reader import Part6Reader
+from dicom_validator.spec_reader.serializer import DefinitionEncoder
+
+from urllib.request import urlretrieve
+
+import html.parser as html_parser
+
+
+class EditionParser(html_parser.HTMLParser, ABC):
+    edition_re = re.compile(r'\d\d\d\d[a-h]')
+
+    def __init__(self):
+        html_parser.HTMLParser.__init__(self)
+        self._in_anchor = False
+        self.editions = []
+
+    def handle_starttag(self, tag, attrs):
+        if tag == 'a':
+            self._in_anchor = True
+
+    def handle_endtag(self, tag):
+        if tag == 'a':
+            self._in_anchor = False
+
+    def handle_data(self, data):
+        if self._in_anchor and self.edition_re.match(data):
+            self.editions.append(data)
+
+
+class EditionReader:
+    base_url = 'https://dicom.nema.org/medical/dicom/'
+    html_filename = 'editions.html'
+    json_filename = 'editions.json'
+    iod_info_json = 'iod_info.json'
+    module_info_json = 'module_info.json'
+    dict_info_json = 'dict_info.json'
+    uid_info_json = 'uid_info.json'
+
+    def __init__(self, path):
+        self.path = path
+        self.logger = logging.getLogger()
+        if not self.logger.hasHandlers():
+            self.logger.addHandler(logging.StreamHandler(sys.stdout))
+
+    def update_edition(self):
+        try:
+            self.logger.info('Getting DICOM editions...')
+            self.retrieve(os.path.join(self.path, self.html_filename))
+            self.write_to_json()
+        except BaseException as exception:
+            self.logger.warning('Failed to get DICOM read_from_html: %s',
+                                str(exception))
+
+    def retrieve(self, html_path):
+        if not os.path.exists(os.path.dirname(html_path)):
+            os.makedirs(os.path.dirname(html_path))
+        urlretrieve(self.base_url, html_path)
+
+    def get_editions(self, update=True):
+        editions_path = os.path.join(self.path, self.json_filename)
+        if os.path.exists(editions_path):
+            if update:
+                today = datetime.datetime.today()
+                modified_date = datetime.datetime.fromtimestamp(
+                    os.path.getmtime(editions_path))
+                # no need to update the edition dir more than once a month
+                update = (today - modified_date).days > 30
+            else:
+                with open(editions_path) as f:
+                    update = not json.load(f)
+        else:
+            update = True
+        if update:
+            self.update_edition()
+        if os.path.exists(editions_path):
+            with open(editions_path) as json_file:
+                return json.load(json_file)
+
+    def read_from_html(self):
+        html_path = os.path.join(self.path, self.html_filename)
+        with open(html_path) as html_file:
+            contents = html_file.read()
+        parser = EditionParser()
+        parser.feed(contents)
+        parser.close()
+        return parser.editions
+
+    def write_to_json(self):
+        editions = self.read_from_html()
+        if editions:
+            json_path = os.path.join(self.path, self.json_filename)
+            with open(json_path, 'w') as json_file:
+                json_file.write(json.dumps(editions))
+
+    def get_edition(self, revision):
+        """Get the edition matching the revision or None.
+        The revision can be the edition name, the year of the edition,
+        'current', or 'local'.
+        """
+        editions = sorted(self.get_editions(revision != 'local'))
+        if revision in editions:
+            return revision
+        if len(revision) == 4:
+            for edition in reversed(editions):
+                if edition.startswith(revision):
+                    return edition
+        if revision == 'current' or revision == 'local':
+            return editions[-1]
+
+    def is_current(self, revision):
+        """Get the edition matching the revision or None.
+        The revision can be the edition name, the year of the edition,
+        or 'current'.
+        """
+        if revision is None:
+            return True
+        editions = sorted(self.get_editions(revision != 'local'))
+        if revision in editions:
+            return revision == editions[-1]
+        if len(revision) == 4:
+            return editions[-1].startswith(revision)
+        if revision == 'current':
+            return True
+        return False
+
+    def check_revision(self, revision):
+        # none revision is used if an existing path points to the specs
+        if revision != 'none':
+            revision = self.get_edition(revision)
+            if revision:
+                return revision, os.path.join(self.path, revision)
+            return None, None
+        return None, self.path
+
+    def get_chapter(self, revision, chapter, destination, is_current):
+        file_path = os.path.join(destination, 'part{:02}.xml'.format(chapter))
+        if os.path.exists(file_path):
+            return True
+        elif not revision:
+            print('Chapter {} not present at {}.'.format(chapter, file_path))
+            return False
+        revision_dir = 'current' if is_current else revision
+        url = '{0}{1}/source/docbook/part{2:02}/part{2:02}.xml'.format(
+            self.base_url, revision_dir, chapter)
+        try:
+            print('Downloading DICOM spec {} PS3.{}...'.format(revision,
+                                                               chapter))
+            urlretrieve(url, file_path)
+            return True
+        except BaseException as exception:
+            print('Failed to download {}: {}'.format(url, str(exception)))
+            if os.path.exists(file_path):
+                try:
+                    os.remove(file_path)
+                except OSError:
+                    print('Failed to remove incomplete file {}.'.format(
+                        file_path))
+            return False
+
+    @staticmethod
+    def load_info(json_path, info_json):
+        with open(os.path.join(json_path,
+                               info_json)) as info_file:
+            return json.load(info_file)
+
+    @classmethod
+    def load_dict_info(cls, json_path):
+        return cls.load_info(json_path, cls.dict_info_json)
+
+    @classmethod
+    def load_uid_info(cls, json_path):
+        return cls.load_info(json_path, cls.uid_info_json)
+
+    @classmethod
+    def load_iod_info(cls, json_path):
+        return cls.load_info(json_path, cls.iod_info_json)
+
+    @classmethod
+    def load_module_info(cls, json_path):
+        return cls.load_info(json_path, cls.module_info_json)
+
+    @classmethod
+    def json_files_exist(cls, json_path):
+        for filename in (cls.dict_info_json, cls.module_info_json,
+                         cls.iod_info_json, cls.uid_info_json):
+            if not os.path.exists(os.path.join(json_path, filename)):
+                return False
+        return True
+
+    @classmethod
+    def dump_description(cls, description):
+        return json.dumps(description, sort_keys=True,
+                          indent=2, cls=DefinitionEncoder)
+
+    @classmethod
+    def create_json_files(cls, docbook_path, json_path):
+        print('Creating JSON excerpts from docbook files...')
+        part6reader = Part6Reader(docbook_path)
+        dict_info = part6reader.data_elements()
+        part3reader = Part3Reader(docbook_path, dict_info)
+        part4reader = Part4Reader(docbook_path)
+        iod_info = part3reader.iod_descriptions()
+        chapter_info = part4reader.iod_chapters()
+        definition = {}
+        for chapter in iod_info:
+            if chapter in chapter_info:
+                for uid in chapter_info[chapter]:
+                    definition[uid] = iod_info[chapter]
+        with open(os.path.join(json_path, cls.iod_info_json),
+                  'w') as info_file:
+            info_file.write(cls.dump_description(definition))
+        with open(os.path.join(json_path, cls.module_info_json),
+                  'w') as info_file:
+            info_file.write(
+                cls.dump_description(part3reader.module_descriptions()))
+        with open(os.path.join(json_path, cls.dict_info_json),
+                  'w') as info_file:
+            info_file.write(cls.dump_description(dict_info))
+        with open(os.path.join(json_path, cls.uid_info_json),
+                  'w') as info_file:
+            info_file.write(cls.dump_description(part6reader.all_uids()))
+        cls.write_current_version(json_path)
+        print('Done!')
+
+    def get_revision(self, revision):
+        revision, destination = self.check_revision(revision)
+        if destination is None:
+            print('DICOM revision {} not found.'.format(revision))
+            return
+
+        docbook_path = os.path.join(destination, 'docbook')
+        if not os.path.exists(docbook_path):
+            os.makedirs(docbook_path)
+        json_path = os.path.join(destination, 'json')
+        if not os.path.exists(json_path):
+            os.makedirs(json_path)
+
+        # download the docbook files
+        for chapter in [3, 4, 6]:
+            if not self.get_chapter(revision=revision, chapter=chapter,
+                                    destination=docbook_path,
+                                    is_current=self.is_current(revision)):
+                return
+
+        if (not self.json_files_exist(json_path) or
+                not self.is_current_version(json_path)):
+            self.create_json_files(docbook_path, json_path)
+        print('Using DICOM revision {}'.format(revision))
+        return destination
+
+    @staticmethod
+    def is_current_version(json_path):
+        version_path = os.path.join(json_path, 'version')
+        if not os.path.exists(version_path):
+            return False
+        with open(version_path) as f:
+            return f.read() >= __version__
+
+    @staticmethod
+    def write_current_version(json_path):
+        version_path = os.path.join(json_path, 'version')
+        with open(version_path, 'w') as f:
+            f.write(__version__)
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/part3_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/part3_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,309 +1,311 @@
-"""
-Chapter3Reader collects DICOM Information Object Definition information
-for specific Storage SOP Classes.
-The information is taken from PS3.3 in docbook format as provided by ACR NEMA.
-"""
-import logging
-from itertools import groupby
-
-import sys
-
-from dicom_validator.spec_reader.condition_parser import ConditionParser
-from dicom_validator.spec_reader.spec_reader import (
-    SpecReader, SpecReaderParseError, SpecReaderLookupError
-)
-
-
-class Part3Reader(SpecReader):
-    """Reads information from PS3.3 in docbook format."""
-
-    def __init__(self, spec_dir, dict_info=None):
-        super(Part3Reader, self).__init__(spec_dir)
-        self.part_nr = 3
-        self._condition_parser = None
-        self._dict_info = dict_info
-        self._iod_descriptions = {}
-        self._iod_nodes = {}
-        self._module_descriptions = {}
-        self._current_refs = []
-        self.logger = logging.getLogger()
-        if not self.logger.handlers:
-            self.logger.addHandler(logging.StreamHandler(sys.stdout))
-        if dict_info is not None:
-            self._condition_parser = ConditionParser(self._dict_info)
-
-    def iod_description(self, chapter):
-        """Return the IOD information for the given chapter.
-
-        The return value is a dict with the entries:
-            'title': The display name of the IOD
-            'modules': A dictionary of the contained IOD modules with the
-                module name as key.
-                A module dict value has the following entries:
-                'ref': The section in PS3.3 describing the module
-                    (e.g. 'C.7.4.2')
-                'use': Usage information (e.g. 'M' for mandatory)
-        Raises SpecReaderLookupError if the chapter is not found.
-        """
-        if chapter not in self._iod_descriptions:
-            iod_node = self._get_iod_nodes().get(chapter)
-            if iod_node:
-                description = self._parse_iod_node(iod_node)
-                self._iod_descriptions[chapter] = description
-        try:
-            return self._iod_descriptions[chapter]
-        except KeyError:
-            raise SpecReaderLookupError(
-                'No definition found for chapter {}'.format(chapter))
-
-    def iod_descriptions(self):
-        """Return the IOD information dict per chapter.
-
-        The dict has the chapter (e.g. 'A.3') as key and the IOD descriptions
-         as value.
-        See iod_description() for the format of the IOD descriptions.
-        Retired IODs (which have no module list) are omitted.
-        """
-        return {chapter: self.iod_description(chapter) for chapter in
-                self._get_iod_nodes()
-                if self.iod_description(chapter)['modules']}
-
-    def module_description(self, section):
-        """Return the module information in the given section.
-
-        The return value is a dict with the entries:
-            'title': The name of the module
-            'attributes': A dictionary of the contained module attributes
-                with the tag as key.
-                An attribute dict value has the following entries:
-                    'name': the tag name
-                    'type': the type (1, 1C, 2, 2C, 3)
-                    'items': only for sequence tags - contains a dictionary
-                        of the module attributes contained in the sequence
-        Raises SpecReaderLookupError if the section is not found.
-        """
-        if section not in self._module_descriptions:
-            section_node = self._get_section_node(section)
-            if section_node:
-                description = self._parse_module_description(section_node)
-                self._module_descriptions[section] = description
-        try:
-            return self._module_descriptions[section]
-        except KeyError:
-            raise SpecReaderLookupError(
-                'No definition found for section {}'.format(section))
-
-    def module_descriptions(self):
-        """Return the module attribute information for all IODs.
-
-        The return value is a dict with the section name as key and
-        a description dict as value.
-        See module_description() for the content of the value dict.
-        """
-        # ensure that all module attributes are read
-        self.iod_descriptions()
-        return self._module_descriptions
-
-    def _get_iod_nodes(self):
-        if not self._iod_nodes:
-            chapter_a = self._find(self._get_doc_root(),
-                                   ['chapter[@label="A"]'])
-            if chapter_a is None:
-                raise SpecReaderParseError('Chapter A in Part 3 not found')
-            # ignore A.1
-            all_iod_nodes = self._findall(chapter_a, ['section'])[1:]
-            iod_def_endings = (
-                ' IOD',
-                ' Information Object Definition',
-                ' Information Objection Definition'  # account for known typo
-            )
-
-            iod_sub_nodes = []
-            nodes_with_subnodes = []
-            for iod_node in all_iod_nodes:
-                sub_nodes = self._find_sections_with_title_endings(
-                    iod_node, iod_def_endings)
-                if sub_nodes:
-                    nodes_with_subnodes.append(iod_node)
-                    iod_sub_nodes.extend(sub_nodes)
-            all_iod_nodes = [node for node in all_iod_nodes if
-                             node not in nodes_with_subnodes]
-            all_iod_nodes.extend(iod_sub_nodes)
-            self._iod_nodes = {node.attrib['label']: node for node in
-                               all_iod_nodes}
-        return self._iod_nodes
-
-    def _get_section_node(self, section):
-        section_parts = section.split('.')
-        section_name = section_parts[0]
-        search_path = ['chapter[@label="{}"]'.format(section_name)]
-        for section_part in section_parts[1:]:
-            section_name = section_name + '.' + section_part
-            search_path.append('section[@label="{}"]'.format(section_name))
-        return self._find(self._get_doc_root(), search_path)
-
-    def _parse_iod_node(self, iod_node):
-        return {'title': self._find(iod_node, ['title']).text,
-                'modules': self._get_iod_modules(iod_node)}
-
-    def _parse_module_description(self, parent_node):
-        table_node = self._find(parent_node, ['table'])
-        # handle the case that the parent node is the table itself
-        if table_node is None:
-            table_node = parent_node
-        table_body_node = self._find(table_node, ['tbody'])
-        if table_body_node is None:
-            return
-        rows = self._findall(table_body_node, ['tr'])
-        current_level = 0
-        current_descriptions = [{}]
-        last_tag_id = None
-        for row in rows:
-            columns = self._findall(row, ['td'])
-            if not columns:
-                continue
-            tag_name, current_level = self._get_tag_name_and_level(
-                columns[0], current_descriptions, current_level, last_tag_id)
-            if len(columns) == 4:
-                last_tag_id = self._handle_regular_attribute(
-                    columns, current_descriptions, last_tag_id, tag_name)
-            elif tag_name.startswith('Include'):
-                self._handle_included_attributes(columns, current_descriptions)
-            else:
-                # todo: other entries
-                pass
-        return current_descriptions[0]
-
-    def _handle_included_attributes(self, columns, current_descriptions):
-        include_node = self._find(columns[0], ['para', 'emphasis', 'xref'])
-        if include_node is None:
-            # todo: functional group macros or similar
-            return
-        include_ref = include_node.attrib['linkend']
-        if self._current_refs and include_ref == self._current_refs[-1]:
-            self.logger.debug('Self reference in %s  - ignoring.', include_ref)
-            return
-        self._current_refs.append(include_ref)
-        element, label = self._get_ref_element_and_label(include_ref)
-        if label not in self._module_descriptions:
-            ref_node = self._get_ref_node(element, label)
-            if ref_node is None:
-                raise SpecReaderLookupError(
-                    'Failed to lookup include reference ' + include_ref)
-            # it is allowed to have no attributes (example: Raw Data)
-            ref_description = self._parse_module_description(ref_node) or {}
-            self._module_descriptions[label] = ref_description
-        current_descriptions[-1].setdefault('include', []).append(label)
-        self._current_refs.pop()
-
-    def _handle_regular_attribute(self, columns, current_descriptions,
-                                  last_tag_id, tag_name):
-        tag_id = self._find_text(columns[1])
-        tag_type = self._find_text(columns[2])
-        if tag_id:
-            current_descriptions[-1][tag_id] = {
-                'name': tag_name,
-                'type': tag_type,
-            }
-            if self._condition_parser and tag_type in ('1C', '2C'):
-                # cond = self._find_all_text(columns[3])
-                # index = cond.find('Required if ')
-                # if index >= 0:
-                #     current_descriptions[-1][tag_id]['desc'] = cond[index:]
-                current_descriptions[-1][tag_id][
-                    'cond'] = self._condition_parser.parse(
-                    self._find_all_text(columns[3]))
-
-            last_tag_id = tag_id
-        return last_tag_id
-
-    def _get_ref_node(self, element, label):
-        return self._get_doc_tree().find(
-            './/{}{}[@label="{}"]'.format(self.docbook_ns, element, label))
-
-    @staticmethod
-    def _get_ref_element_and_label(ref):
-        element, label = ref.split('_')
-        if element == 'sect':
-            element = 'section'
-        return element, label
-
-    def _get_tag_name_and_level(self, column, current_descriptions,
-                                current_level, last_tag_id):
-        tag_name = self._find_text(column)
-        if not tag_name:
-            return '', 0
-        start_chars = next(groupby(tag_name))
-        level = len(list(start_chars[1])) if start_chars[0] == '>' else 0
-        tag_name = tag_name[level:]
-        if level > current_level:
-            sequence_description = {}
-            try:
-                current_descriptions[-1][last_tag_id][
-                    'items'] = sequence_description
-                current_descriptions.append(sequence_description)
-            except KeyError:
-                # silently ignore error in older specs
-                pass
-        elif level < current_level:
-            current_descriptions.pop()
-        return tag_name, level
-
-    def _get_iod_modules(self, iod_node):
-        module_table_sections = self._find_sections_with_title_endings(
-            iod_node, (' Module Table', ' IOD Modules'))
-        if not module_table_sections:
-            module_table_sections = self._find_sections_with_title_endings(
-                iod_node, ('IOD Entity-Relationship Model',))
-        modules = {}
-        if len(module_table_sections) == 1:
-            module_rows = self._findall(module_table_sections[0],
-                                        ['table', 'tbody', 'tr'])
-            row_span = 0
-            for row in module_rows:
-                columns = self._findall(row, ['td'])
-                name_index = 0 if row_span > 0 else 1
-                if row_span == 0:
-                    if 'rowspan' in columns[0].attrib:
-                        row_span = int(columns[0].attrib['rowspan'])
-                    else:
-                        row_span = 1
-                name = self._find_text(columns[name_index])
-                modules[name] = {}
-                try:
-                    ref_section = self._find(columns[name_index + 1],
-                                             ['para', 'xref']).attrib[
-                        'linkend'].split('_')[1]
-                except AttributeError:
-                    try:
-                        ref_section = self._find(
-                            columns[name_index + 1], ['xref']).attrib[
-                            'linkend'].split('_')[1]
-                    except AttributeError:
-                        self.logger.warning(
-                            'Failed to read module table for %s', name)
-                        continue
-                modules[name]['ref'] = ref_section
-                # make sure the module description is loaded
-                self.module_description(ref_section)
-                modules[name]['use'] = self._find_text(columns[name_index + 2])
-                if (self._condition_parser is not None and
-                        modules[name]['use'].startswith('C - ')):
-                    modules[name]['cond'] = self._condition_parser.parse(
-                        modules[name]['use'])
-                else:
-                    modules[name]['use'] = modules[name]['use'][0]
-                row_span -= 1
-        return modules
-
-    def _find_sections_with_title_endings(self, node, title_endings):
-        section_nodes = self._findall(node, ['section'])
-        found_nodes = []
-        for sections_node in section_nodes:
-            title_node = self._find(sections_node, ['title'])
-            if title_node is not None:
-                title = title_node.text
-                if any([title.endswith(title_ending) for title_ending in
-                        title_endings]):
-                    found_nodes.append(sections_node)
-        return found_nodes
+"""
+Chapter3Reader collects DICOM Information Object Definition information
+for specific Storage SOP Classes.
+The information is taken from PS3.3 in docbook format as provided by ACR NEMA.
+"""
+import logging
+from itertools import groupby
+
+import sys
+
+from dicom_validator.spec_reader.condition_parser import ConditionParser
+from dicom_validator.spec_reader.spec_reader import (
+    SpecReader, SpecReaderParseError, SpecReaderLookupError
+)
+
+
+class Part3Reader(SpecReader):
+    """Reads information from PS3.3 in docbook format."""
+
+    def __init__(self, spec_dir, dict_info=None):
+        super(Part3Reader, self).__init__(spec_dir)
+        self.part_nr = 3
+        self._condition_parser = None
+        self._dict_info = dict_info
+        self._iod_descriptions = {}
+        self._iod_nodes = {}
+        self._module_descriptions = {}
+        self._current_refs = []
+        self.logger = logging.getLogger()
+        if not self.logger.hasHandlers():
+            self.logger.addHandler(logging.StreamHandler(sys.stdout))
+        if dict_info is not None:
+            self._condition_parser = ConditionParser(self._dict_info)
+
+    def iod_description(self, chapter):
+        """Return the IOD information for the given chapter.
+
+        The return value is a dict with the entries:
+            'title': The display name of the IOD
+            'modules': A dictionary of the contained IOD modules with the
+                module name as key.
+                A module dict value has the following entries:
+                'ref': The section in PS3.3 describing the module
+                    (e.g. 'C.7.4.2')
+                'use': Usage information (e.g. 'M' for mandatory)
+        Raises SpecReaderLookupError if the chapter is not found.
+        """
+        if chapter not in self._iod_descriptions:
+            iod_node = self._get_iod_nodes().get(chapter)
+            if iod_node:
+                description = self._parse_iod_node(iod_node)
+                self._iod_descriptions[chapter] = description
+        try:
+            return self._iod_descriptions[chapter]
+        except KeyError:
+            raise SpecReaderLookupError(
+                'No definition found for chapter {}'.format(chapter))
+
+    def iod_descriptions(self):
+        """Return the IOD information dict per chapter.
+
+        The dict has the chapter (e.g. 'A.3') as key and the IOD descriptions
+         as value.
+        See iod_description() for the format of the IOD descriptions.
+        Retired IODs (which have no module list) are omitted.
+        """
+        return {chapter: self.iod_description(chapter) for chapter in
+                self._get_iod_nodes()
+                if self.iod_description(chapter)['modules']}
+
+    def module_description(self, section):
+        """Return the module information in the given section.
+
+        The return value is a dict with the entries:
+            'title': The name of the module
+            'attributes': A dictionary of the contained module attributes
+                with the tag as key.
+                An attribute dict value has the following entries:
+                    'name': the tag name
+                    'type': the type (1, 1C, 2, 2C, 3)
+                    'items': only for sequence tags - contains a dictionary
+                        of the module attributes contained in the sequence
+        Raises SpecReaderLookupError if the section is not found.
+        """
+        if section not in self._module_descriptions:
+            section_node = self._get_section_node(section)
+            if section_node:
+                description = self._parse_module_description(section_node)
+                self._module_descriptions[section] = description
+        try:
+            return self._module_descriptions[section]
+        except KeyError:
+            raise SpecReaderLookupError(
+                'No definition found for section {}'.format(section))
+
+    def module_descriptions(self):
+        """Return the module attribute information for all IODs.
+
+        The return value is a dict with the section name as key and
+        a description dict as value.
+        See module_description() for the content of the value dict.
+        """
+        # ensure that all module attributes are read
+        self.iod_descriptions()
+        return self._module_descriptions
+
+    def _get_iod_nodes(self):
+        if not self._iod_nodes:
+            chapter_a = self._find(self._get_doc_root(),
+                                   ['chapter[@label="A"]'])
+            if chapter_a is None:
+                raise SpecReaderParseError('Chapter A in Part 3 not found')
+            # ignore A.1
+            all_iod_nodes = self._findall(chapter_a, ['section'])[1:]
+            iod_def_endings = (
+                ' IOD',
+                ' Information Object Definition',
+                ' Information Objection Definition'  # account for known typo
+            )
+
+            iod_sub_nodes = []
+            nodes_with_subnodes = []
+            for iod_node in all_iod_nodes:
+                sub_nodes = self._find_sections_with_title_endings(
+                    iod_node, iod_def_endings)
+                if sub_nodes:
+                    nodes_with_subnodes.append(iod_node)
+                    iod_sub_nodes.extend(sub_nodes)
+            all_iod_nodes = [node for node in all_iod_nodes if
+                             node not in nodes_with_subnodes]
+            all_iod_nodes.extend(iod_sub_nodes)
+            self._iod_nodes = {node.attrib['label']: node for node in
+                               all_iod_nodes}
+        return self._iod_nodes
+
+    def _get_section_node(self, section):
+        section_parts = section.split('.')
+        section_name = section_parts[0]
+        search_path = ['chapter[@label="{}"]'.format(section_name)]
+        for section_part in section_parts[1:]:
+            section_name = section_name + '.' + section_part
+            search_path.append('section[@label="{}"]'.format(section_name))
+        return self._find(self._get_doc_root(), search_path)
+
+    def _parse_iod_node(self, iod_node):
+        return {'title': self._find(iod_node, ['title']).text,
+                'modules': self._get_iod_modules(iod_node)}
+
+    def _parse_module_description(self, parent_node):
+        table_node = self._find(parent_node, ['table'])
+        # handle the case that the parent node is the table itself
+        if table_node is None:
+            table_node = parent_node
+        table_body_node = self._find(table_node, ['tbody'])
+        if table_body_node is None:
+            return
+        rows = self._findall(table_body_node, ['tr'])
+        current_level = 0
+        current_descriptions = [{}]
+        last_tag_id = None
+        for row in rows:
+            columns = self._findall(row, ['td'])
+            if not columns:
+                continue
+            tag_name, current_level = self._get_tag_name_and_level(
+                columns[0], current_descriptions, current_level, last_tag_id)
+            if len(columns) == 4:
+                last_tag_id = self._handle_regular_attribute(
+                    columns, current_descriptions, last_tag_id, tag_name)
+            elif tag_name.startswith('Include'):
+                self._handle_included_attributes(columns, current_descriptions)
+            else:
+                # todo: other entries
+                pass
+        return current_descriptions[0]
+
+    def _handle_included_attributes(self, columns, current_descriptions):
+        include_node = self._find(columns[0], ['para', 'emphasis', 'xref'])
+        if include_node is None:
+            # todo: functional group macros or similar
+            return
+        include_ref = include_node.attrib['linkend']
+        if self._current_refs and include_ref == self._current_refs[-1]:
+            self.logger.debug('Self reference in %s  - ignoring.', include_ref)
+            return
+        self._current_refs.append(include_ref)
+        element, label = self._get_ref_element_and_label(include_ref)
+        if label not in self._module_descriptions:
+            ref_node = self._get_ref_node(element, label)
+            if ref_node is None:
+                raise SpecReaderLookupError(
+                    'Failed to lookup include reference ' + include_ref)
+            # it is allowed to have no attributes (example: Raw Data)
+            ref_description = self._parse_module_description(ref_node) or {}
+            self._module_descriptions[label] = ref_description
+        current_descriptions[-1].setdefault('include', []).append(label)
+        self._current_refs.pop()
+
+    def _handle_regular_attribute(self, columns, current_descriptions,
+                                  last_tag_id, tag_name):
+        tag_id = self._find_text(columns[1])
+        tag_type = self._find_text(columns[2])
+        if tag_id:
+            current_descriptions[-1][tag_id] = {
+                'name': tag_name,
+                'type': tag_type,
+            }
+            if self._condition_parser and tag_type in ('1C', '2C'):
+                # cond = self._find_all_text(columns[3])
+                # index = cond.find('Required if ')
+                # if index >= 0:
+                #     current_descriptions[-1][tag_id]['desc'] = cond[index:]
+                current_descriptions[-1][tag_id][
+                    'cond'] = self._condition_parser.parse(
+                    self._find_all_text(columns[3]))
+
+            last_tag_id = tag_id
+        return last_tag_id
+
+    def _get_ref_node(self, element, label):
+        return self._get_doc_tree().find(
+            './/{}{}[@label="{}"]'.format(self.docbook_ns, element, label))
+
+    @staticmethod
+    def _get_ref_element_and_label(ref):
+        element, label = ref.split('_')
+        if element == 'sect':
+            element = 'section'
+        return element, label
+
+    def _get_tag_name_and_level(self, column, current_descriptions,
+                                current_level, last_tag_id):
+        tag_name = self._find_text(column)
+        if not tag_name:
+            return '', 0
+        start_chars = next(groupby(tag_name))
+        level = len(list(start_chars[1])) if start_chars[0] == '>' else 0
+        tag_name = tag_name[level:]
+        if level > current_level:
+            sequence_description = {}
+            try:
+                current_descriptions[-1][last_tag_id][
+                    'items'] = sequence_description
+                current_descriptions.append(sequence_description)
+            except KeyError:
+                # silently ignore error in older specs
+                pass
+        elif level < current_level:
+            # Pop off (delete) the last level_delta items.
+            level_delta = current_level - level
+            del current_descriptions[-level_delta:]
+        return tag_name, level
+
+    def _get_iod_modules(self, iod_node):
+        module_table_sections = self._find_sections_with_title_endings(
+            iod_node, (' Module Table', ' IOD Modules'))
+        if not module_table_sections:
+            module_table_sections = self._find_sections_with_title_endings(
+                iod_node, ('IOD Entity-Relationship Model',))
+        modules = {}
+        if len(module_table_sections) == 1:
+            module_rows = self._findall(module_table_sections[0],
+                                        ['table', 'tbody', 'tr'])
+            row_span = 0
+            for row in module_rows:
+                columns = self._findall(row, ['td'])
+                name_index = 0 if row_span > 0 else 1
+                if row_span == 0:
+                    if 'rowspan' in columns[0].attrib:
+                        row_span = int(columns[0].attrib['rowspan'])
+                    else:
+                        row_span = 1
+                name = self._find_text(columns[name_index])
+                modules[name] = {}
+                try:
+                    ref_section = self._find(columns[name_index + 1],
+                                             ['para', 'xref']).attrib[
+                        'linkend'].split('_')[1]
+                except AttributeError:
+                    try:
+                        ref_section = self._find(
+                            columns[name_index + 1], ['xref']).attrib[
+                            'linkend'].split('_')[1]
+                    except AttributeError:
+                        self.logger.warning(
+                            'Failed to read module table for %s', name)
+                        continue
+                modules[name]['ref'] = ref_section
+                # make sure the module description is loaded
+                self.module_description(ref_section)
+                modules[name]['use'] = self._find_text(columns[name_index + 2])
+                if (self._condition_parser is not None and
+                        modules[name]['use'].startswith('C - ')):
+                    modules[name]['cond'] = self._condition_parser.parse(
+                        modules[name]['use'])
+                else:
+                    modules[name]['use'] = modules[name]['use'][0]
+                row_span -= 1
+        return modules
+
+    def _find_sections_with_title_endings(self, node, title_endings):
+        section_nodes = self._findall(node, ['section'])
+        found_nodes = []
+        for sections_node in section_nodes:
+            title_node = self._find(sections_node, ['title'])
+            if title_node is not None:
+                title = title_node.text
+                if any([title.endswith(title_ending) for title_ending in
+                        title_endings]):
+                    found_nodes.append(sections_node)
+        return found_nodes
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/part4_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/part4_reader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-"""
-Chapter4Reader collects SOP Class Information information for specific
-Storage SOP Classes.
-The information is taken from PS3.4 in docbook format as provided by ACR NEMA.
-"""
-from dicom_validator.spec_reader.spec_reader import (
-    SpecReader, SpecReaderLookupError, SpecReaderParseError
-)
-
-
-class Part4Reader(SpecReader):
-    """Reads information from PS3.4 in docbook format."""
-
-    def __init__(self, spec_dir):
-        super(Part4Reader, self).__init__(spec_dir)
-        self.part_nr = 4
-        self._sop_class_uids = {}  # SOP Class UID --> chapter
-        self._chapters = {}  # chapter --> SOP Class UID list
-
-    def iod_chapter(self, sop_class_uid):
-        """Return the chapter in part 3 for the given SOP Class."""
-        if not self._sop_class_uids:
-            self._read_sop_table('B.5')  # standard SOP Classes
-        try:
-            return self._sop_class_uids[sop_class_uid]
-        except KeyError:
-            raise SpecReaderLookupError(
-                'SOP Class {} not found'.format(sop_class_uid))
-
-    def iod_chapters(self):
-        """Return a dict of the chapter in part 3 for each SOP Class
-        listed in table B.5.
-        """
-        if not self._chapters:
-            self._read_sop_table('B.5')
-        return self._chapters
-
-    def _read_sop_table(self, chapter):
-        table = self._find(self._get_doc_root(),
-                           ['chapter[@label="B"]',
-                            'section[@label="{}"]'.format(chapter), 'table',
-                            'tbody'])
-        if table is None:
-            raise SpecReaderParseError('SOP Class table in Part 4 not found')
-        row_nodes = self._findall(table, ['tr'])
-        for row_node in row_nodes:
-            column_nodes = self._findall(row_node, ['td'])
-            if len(column_nodes) in (3, 4):
-                # columns are SOP Class Name, SOP Class UID, IOD Specification
-                # and Specialization (only since 2020c)
-                uid = self.cleaned_value(self._find_text(column_nodes[1]))
-                target_node = self._find(column_nodes[2], ['para', 'olink'])
-                if target_node is not None:
-                    chapter = target_node.attrib['targetptr'].split('_')[1]
-                    self._sop_class_uids[uid] = chapter
-                    self._chapters.setdefault(chapter, []).append(uid)
-        self._patch_incorrect_values()
-
-    def _patch_incorrect_values(self):
-        sc_sop_class_uid = '1.2.840.10008.5.1.4.1.1.7'
-        if self._sop_class_uids.get(sc_sop_class_uid, '') == 'A.8':
-            self._sop_class_uids[sc_sop_class_uid] = 'A.8.1'
-            self._chapters['A.8.1'] = [sc_sop_class_uid]
-            del self._chapters['A.8']
+"""
+Chapter4Reader collects SOP Class Information information for specific
+Storage SOP Classes.
+The information is taken from PS3.4 in docbook format as provided by ACR NEMA.
+"""
+from dicom_validator.spec_reader.spec_reader import (
+    SpecReader, SpecReaderLookupError, SpecReaderParseError
+)
+
+
+class Part4Reader(SpecReader):
+    """Reads information from PS3.4 in docbook format."""
+
+    def __init__(self, spec_dir):
+        super(Part4Reader, self).__init__(spec_dir)
+        self.part_nr = 4
+        self._sop_class_uids = {}  # SOP Class UID --> chapter
+        self._chapters = {}  # chapter --> SOP Class UID list
+
+    def iod_chapter(self, sop_class_uid):
+        """Return the chapter in part 3 for the given SOP Class."""
+        if not self._sop_class_uids:
+            self._read_sop_table('B.5')  # standard SOP Classes
+        try:
+            return self._sop_class_uids[sop_class_uid]
+        except KeyError:
+            raise SpecReaderLookupError(
+                'SOP Class {} not found'.format(sop_class_uid))
+
+    def iod_chapters(self):
+        """Return a dict of the chapter in part 3 for each SOP Class
+        listed in table B.5.
+        """
+        if not self._chapters:
+            self._read_sop_table('B.5')
+        return self._chapters
+
+    def _read_sop_table(self, chapter):
+        table = self._find(self._get_doc_root(),
+                           ['chapter[@label="B"]',
+                            'section[@label="{}"]'.format(chapter), 'table',
+                            'tbody'])
+        if table is None:
+            raise SpecReaderParseError('SOP Class table in Part 4 not found')
+        row_nodes = self._findall(table, ['tr'])
+        for row_node in row_nodes:
+            column_nodes = self._findall(row_node, ['td'])
+            if len(column_nodes) in (3, 4):
+                # columns are SOP Class Name, SOP Class UID, IOD Specification
+                # and Specialization (only since 2020c)
+                uid = self.cleaned_value(self._find_text(column_nodes[1]))
+                target_node = self._find(column_nodes[2], ['para', 'olink'])
+                if target_node is not None:
+                    chapter = target_node.attrib['targetptr'].split('_')[1]
+                    self._sop_class_uids[uid] = chapter
+                    self._chapters.setdefault(chapter, []).append(uid)
+        self._patch_incorrect_values()
+
+    def _patch_incorrect_values(self):
+        sc_sop_class_uid = '1.2.840.10008.5.1.4.1.1.7'
+        if self._sop_class_uids.get(sc_sop_class_uid, '') == 'A.8':
+            self._sop_class_uids[sc_sop_class_uid] = 'A.8.1'
+            self._chapters['A.8.1'] = [sc_sop_class_uid]
+            del self._chapters['A.8']
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/part6_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/part6_reader.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-"""
-Chapter6Reader collects DICOM Data Element information.
-The information is taken from DICOM dictionary (PS3.6) in docbook format
-as provided by ACR NEMA.
-"""
-from dicom_validator.spec_reader.spec_reader import (
-    SpecReader, SpecReaderParseError
-)
-
-
-class Part6Reader(SpecReader):
-    """Reads information from PS3.4 in docbook format."""
-
-    def __init__(self, spec_dir):
-        super(Part6Reader, self).__init__(spec_dir)
-        self.part_nr = 6
-        self._uids = None
-        self._data_elements = None
-
-    def data_elements(self):
-        """Return the information about registered DICOM data elements.
-
-        The return value is a dict with the the tag ID (group/element tuple)
-        as key.
-        See data_element() for the contained value.
-        """
-        if self._data_elements is None:
-            self._read_element_table()
-        return self._data_elements
-
-    def data_element(self, tag_id):
-        """Return the information about the specified tag.
-
-        Arguments:
-            tag_id: The tag ID as string in format (####,####)
-        The return value is a dict with the the tag ID (group/element tuple)
-        as key.
-        The values of the retruned dict are dicts with the following entries:
-            'name': The human readable tag name
-            'vr': The tag value representation (e.g. 'PN')
-            'vm': The tag multiplicity (e.g. '1-N')
-            'prop': Additional properties, like 'RET' for retired
-        """
-        return self.data_elements().get(tag_id)
-
-    def _read_element_table(self):
-        self._data_elements = {}
-        table = self._find(self._get_doc_root(),
-                           ['chapter[@label="6"]', 'table', 'tbody'])
-        if table is None:
-            raise SpecReaderParseError(
-                'Registry of DICOM Data Elements not found in PS3.6')
-        row_nodes = self._findall(table, ['tr'])
-        attrib_indexes = [1, 3, 4, 5]
-        for row_node in row_nodes:
-            column_nodes = self._findall(row_node, ['td'])
-            if len(column_nodes) == 6:
-                tag_id = self._find_text(column_nodes[0])
-                if tag_id:
-                    tag_attributes = [self._find_text(column_nodes[i])
-                                      for i in attrib_indexes]
-                    if tag_attributes is not None:
-                        self._data_elements[tag_id] = {
-                            'name': tag_attributes[0],
-                            'vr': tag_attributes[1],
-                            'vm': tag_attributes[2],
-                            'prop': tag_attributes[3]
-                        }
-
-    def uids(self, uid_type):
-        """Return a dict of UID values (keys) and names for the given UID type.
-        """
-        return self._get_uids().get(uid_type, {})
-
-    def all_uids(self):
-        """Return a dict of UID types with UID value/name dicts for the
-        given UID type as value.
-        """
-        return self._get_uids()
-
-    def sop_class_uids(self):
-        """Return a dict of SOP Class UID values (keys) and names."""
-        return self.uids('SOP Class')
-
-    def sop_class_name(self, uid):
-        """Return the name of SOP Class corresponding to the given UID."""
-        return self.uids('SOP Class').get(uid)
-
-    def sop_class_uid(self, sop_class_name):
-        """Return the name of SOP Class corresponding to the given UID."""
-        for uid, name in self.sop_class_uids().items():
-            if name == sop_class_name:
-                return uid
-
-    def _get_uids(self):
-        if self._uids is None:
-            self._uids = {}
-            table = self._find(self._get_doc_root(),
-                               ['chapter[@label="A"]', 'table', 'tbody'])
-            if table is None:
-                raise SpecReaderParseError(
-                    'Registry of DICOM Unique Identifiers not found in PS3.6')
-
-            row_nodes = self._findall(table, ['tr'])
-            for row_node in row_nodes:
-                column_nodes = self._findall(row_node, ['td'])
-                nr_columns = len(column_nodes)
-                if nr_columns in (4, 5):
-                    # columns are UID Value, UID Name, UID Keyword (only
-                    # since 2020d), UID Type and Part
-                    uid_attributes = [self._find_text(column_nodes[i])
-                                      for i in range(nr_columns - 1)]
-                    if uid_attributes is not None:
-                        uid_type = uid_attributes[nr_columns - 2]
-                        # in PS3.6 xml there are multiple zero width (U+200B)
-                        # spaces inside the UIDs
-                        # we remove them hoping this is the only such problem
-                        uid_value = self.cleaned_value(uid_attributes[0])
-                        self._uids.setdefault(uid_type, {})[
-                            uid_value] = self.cleaned_value(uid_attributes[1])
-        return self._uids
+"""
+Chapter6Reader collects DICOM Data Element information.
+The information is taken from DICOM dictionary (PS3.6) in docbook format
+as provided by ACR NEMA.
+"""
+from dicom_validator.spec_reader.spec_reader import (
+    SpecReader, SpecReaderParseError
+)
+
+
+class Part6Reader(SpecReader):
+    """Reads information from PS3.4 in docbook format."""
+
+    def __init__(self, spec_dir):
+        super(Part6Reader, self).__init__(spec_dir)
+        self.part_nr = 6
+        self._uids = None
+        self._data_elements = None
+
+    def data_elements(self):
+        """Return the information about registered DICOM data elements.
+
+        The return value is a dict with the the tag ID (group/element tuple)
+        as key.
+        See data_element() for the contained value.
+        """
+        if self._data_elements is None:
+            self._read_element_table()
+        return self._data_elements
+
+    def data_element(self, tag_id):
+        """Return the information about the specified tag.
+
+        Arguments:
+            tag_id: The tag ID as string in format (####,####)
+        The return value is a dict with the the tag ID (group/element tuple)
+        as key.
+        The values of the retruned dict are dicts with the following entries:
+            'name': The human readable tag name
+            'vr': The tag value representation (e.g. 'PN')
+            'vm': The tag multiplicity (e.g. '1-N')
+            'prop': Additional properties, like 'RET' for retired
+        """
+        return self.data_elements().get(tag_id)
+
+    def _read_element_table(self):
+        self._data_elements = {}
+        table = self._find(self._get_doc_root(),
+                           ['chapter[@label="6"]', 'table', 'tbody'])
+        if table is None:
+            raise SpecReaderParseError(
+                'Registry of DICOM Data Elements not found in PS3.6')
+        row_nodes = self._findall(table, ['tr'])
+        attrib_indexes = [1, 3, 4, 5]
+        for row_node in row_nodes:
+            column_nodes = self._findall(row_node, ['td'])
+            if len(column_nodes) == 6:
+                tag_id = self._find_text(column_nodes[0])
+                if tag_id:
+                    tag_attributes = [self._find_text(column_nodes[i])
+                                      for i in attrib_indexes]
+                    if tag_attributes is not None:
+                        self._data_elements[tag_id] = {
+                            'name': tag_attributes[0],
+                            'vr': tag_attributes[1],
+                            'vm': tag_attributes[2],
+                            'prop': tag_attributes[3]
+                        }
+
+    def uids(self, uid_type):
+        """Return a dict of UID values (keys) and names for the given UID type.
+        """
+        return self._get_uids().get(uid_type, {})
+
+    def all_uids(self):
+        """Return a dict of UID types with UID value/name dicts for the
+        given UID type as value.
+        """
+        return self._get_uids()
+
+    def sop_class_uids(self):
+        """Return a dict of SOP Class UID values (keys) and names."""
+        return self.uids('SOP Class')
+
+    def sop_class_name(self, uid):
+        """Return the name of SOP Class corresponding to the given UID."""
+        return self.uids('SOP Class').get(uid)
+
+    def sop_class_uid(self, sop_class_name):
+        """Return the name of SOP Class corresponding to the given UID."""
+        for uid, name in self.sop_class_uids().items():
+            if name == sop_class_name:
+                return uid
+
+    def _get_uids(self):
+        if self._uids is None:
+            self._uids = {}
+            table = self._find(self._get_doc_root(),
+                               ['chapter[@label="A"]', 'table', 'tbody'])
+            if table is None:
+                raise SpecReaderParseError(
+                    'Registry of DICOM Unique Identifiers not found in PS3.6')
+
+            row_nodes = self._findall(table, ['tr'])
+            for row_node in row_nodes:
+                column_nodes = self._findall(row_node, ['td'])
+                nr_columns = len(column_nodes)
+                if nr_columns in (4, 5):
+                    # columns are UID Value, UID Name, UID Keyword (only
+                    # since 2020d), UID Type and Part
+                    uid_attributes = [self._find_text(column_nodes[i])
+                                      for i in range(nr_columns - 1)]
+                    if uid_attributes is not None:
+                        uid_type = uid_attributes[nr_columns - 2]
+                        # in PS3.6 xml there are multiple zero width (U+200B)
+                        # spaces inside the UIDs
+                        # we remove them hoping this is the only such problem
+                        uid_value = self.cleaned_value(uid_attributes[0])
+                        self._uids.setdefault(uid_type, {})[
+                            uid_value] = self.cleaned_value(uid_attributes[1])
+        return self._uids
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_condition.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_condition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-import json
-import unittest
-
-import os
-
-from dicom_validator.spec_reader.condition import Condition
-from dicom_validator.spec_reader.edition_reader import EditionReader
-from dicom_validator.tests.test_utils import json_fixture_path
-
-
-class ConditionReadTest(unittest.TestCase):
-    dict_info = None
-
-    @classmethod
-    def setUpClass(cls):
-        with open(os.path.join(json_fixture_path(),
-                               EditionReader.dict_info_json)) as info_file:
-            cls.dict_info = json.load(info_file)
-
-    def check_condition(self, cond_dict, cond_type, index=0, op=None,
-                        tag=None, values=None, nr_and_cond=0, nr_or_cond=0):
-        condition = Condition.read_condition(cond_dict)
-        self.assertEqual(cond_type, condition.type)
-        self.check_sub_condition(condition, index, op, tag, values,
-                                 nr_and_cond, nr_or_cond)
-        return condition
-
-    def check_sub_condition(self, condition, index=0, op=None,
-                            tag=None, values=None, nr_and_cond=0,
-                            nr_or_cond=0):
-        self.assertEqual(index, condition.index)
-        self.assertEqual(op, condition.operator)
-        self.assertEqual(tag, condition.tag)
-        self.assertEqual(values, condition.values)
-        self.assertEqual(nr_and_cond, len(condition.and_conditions))
-        self.assertEqual(nr_or_cond, len(condition.or_conditions))
-
-    def test_read_type_only(self):
-        self.check_condition({"type": "U"}, 'U')
-
-    def test_eq(self):
-        cond_dict = {
-            "index": 0,
-            "op": "=",
-            "tag": "(3004,000A)",
-            "type": "MN",
-            "values": [
-                "BEAM",
-                "BEAM_SESSION",
-                "CONTROL_POINT"
-            ]
-        }
-
-        def test_condition():
-            return self.check_condition(cond_dict, cond_type='MN', op='=',
-                                        tag='(3004,000A)',
-                                        values=['BEAM', 'BEAM_SESSION',
-                                                'CONTROL_POINT'])
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('Dose Summation Type is equal to "BEAM", '
-                         '"BEAM_SESSION" or "CONTROL_POINT"',
-                         condition.to_string(self.dict_info))
-
-    def test_greater(self):
-        cond_dict = {
-            "index": 0,
-            "op": ">",
-            "tag": "(0028,0008)",
-            "type": "MN",
-            "values": ["1"]
-        }
-
-        def test_condition():
-            return self.check_condition(cond_dict, cond_type='MN', op='>',
-                                        tag='(0028,0008)',
-                                        values=['1'])
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('Number of Frames is greater than 1',
-                         condition.to_string(self.dict_info))
-
-    def test_less(self):
-        cond_dict = {
-            "index": 0,
-            "op": "<",
-            "tag": "(0028,0008)",
-            "type": "MN",
-            "values": ["20"]
-        }
-
-        def test_condition():
-            return self.check_condition(cond_dict, cond_type='MN', op='<',
-                                        tag='(0028,0008)',
-                                        values=['20'])
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('Number of Frames is less than 20',
-                         condition.to_string(self.dict_info))
-
-    def test_points_to(self):
-        cond_dict = {
-            "index": 0,
-            "op": "=>",
-            "tag": "(0028,0009)",
-            "type": "MN",
-            "values": [
-                "1577061"
-            ]
-        }
-
-        def test_condition():
-            return self.check_condition(cond_dict, cond_type='MN', op='=>',
-                                        tag='(0028,0009)',
-                                        values=['1577061'])
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('Frame Increment Pointer points to '
-                         '(0018,1065) (Frame Time Vector)',
-                         condition.to_string(self.dict_info))
-
-    def test_exists(self):
-        cond_dict = {
-            "index": 0,
-            "op": "+",
-            "tag": "(7FE0,0010)",
-            "type": "MN"
-        }
-
-        def test_condition():
-            return self.check_condition(cond_dict, cond_type='MN', op='+',
-                                        tag='(7FE0,0010)')
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('Pixel Data exists',
-                         condition.to_string(self.dict_info))
-
-    def test_and_condition(self):
-        cond_dict = {
-            "and": [
-                {
-                    "index": 0,
-                    "op": "-",
-                    "tag": "(0040,E022)"
-                },
-                {
-                    "index": 1,
-                    "op": "+",
-                    "tag": "(0040,E023)"
-                },
-                {
-                    "index": 0,
-                    "op": "!=",
-                    "tag": "(0040,E025)",
-                    "values": ["TEST"]
-                }
-            ],
-            "type": "MU"
-        }
-
-        def test_condition():
-            cond = self.check_condition(
-                cond_dict, cond_type='MU', nr_and_cond=3)
-            self.check_sub_condition(
-                cond.and_conditions[0], op='-', tag='(0040,E022)')
-            self.check_sub_condition(
-                cond.and_conditions[1], op='+', tag='(0040,E023)',
-                index=1)
-            self.check_sub_condition(
-                cond.and_conditions[2], op='!=', tag='(0040,E025)',
-                values=['TEST'])
-            return cond
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('DICOM Media Retrieval Sequence is not present and '
-                         'WADO Retrieval Sequence[1] exists and WADO-RS '
-                         'Retrieval Sequence is not equal to "TEST"',
-                         condition.to_string(self.dict_info))
-
-    def test_or_condition(self):
-        cond_dict = {
-            "or": [
-                {
-                    "index": 0,
-                    "op": "-",
-                    "tag": "(0040,4072)"
-                },
-                {
-                    "index": 0,
-                    "op": "-",
-                    "tag": "(0040,4074)"
-                }
-            ],
-            "type": "MU"
-        }
-
-        def test_condition():
-            cond = self.check_condition(
-                cond_dict, cond_type='MU', nr_or_cond=2)
-            self.check_sub_condition(
-                cond.or_conditions[0], op='-', tag='(0040,4072)')
-            self.check_sub_condition(
-                cond.or_conditions[1], op='-', tag='(0040,4074)')
-            return cond
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
-        self.assertEqual('STOW-RS Storage Sequence is not present or '
-                         'XDS Storage Sequence is not present',
-                         condition.to_string(self.dict_info))
-
-    def test_other_condition(self):
-        cond_dict = {
-            "index": 0,
-            "op": "=",
-            "other_cond": {
-                "index": 0,
-                "op": "+",
-                "tag": "(0072,0704)",
-                "type": "MN"
-            },
-            "tag": "(0072,0704)",
-            "type": "MC",
-            "values": [
-                "PALETTE"
-            ]
-        }
-
-        def test_condition():
-            cond = self.check_condition(
-                cond_dict, cond_type='MC', op='=',
-                tag='(0072,0704)', values=['PALETTE'])
-            self.check_sub_condition(
-                cond.other_condition, op='+', tag='(0072,0704)')
-            self.assertEqual('MN', cond.other_condition.type)
-            return cond
-
-        condition = test_condition()
-        cond_dict = condition.dict()
-        test_condition()
+import json
+import unittest
+
+import os
+
+from dicom_validator.spec_reader.condition import Condition
+from dicom_validator.spec_reader.edition_reader import EditionReader
+from dicom_validator.tests.test_utils import json_fixture_path
+
+
+class ConditionReadTest(unittest.TestCase):
+    dict_info = None
+
+    @classmethod
+    def setUpClass(cls):
+        with open(os.path.join(json_fixture_path(),
+                               EditionReader.dict_info_json)) as info_file:
+            cls.dict_info = json.load(info_file)
+
+    def check_condition(self, cond_dict, cond_type, index=0, op=None,
+                        tag=None, values=None, nr_and_cond=0, nr_or_cond=0):
+        condition = Condition.read_condition(cond_dict)
+        self.assertEqual(cond_type, condition.type)
+        self.check_sub_condition(condition, index, op, tag, values,
+                                 nr_and_cond, nr_or_cond)
+        return condition
+
+    def check_sub_condition(self, condition, index=0, op=None,
+                            tag=None, values=None, nr_and_cond=0,
+                            nr_or_cond=0):
+        self.assertEqual(index, condition.index)
+        self.assertEqual(op, condition.operator)
+        self.assertEqual(tag, condition.tag)
+        self.assertEqual(values or [], condition.values)
+        self.assertEqual(nr_and_cond, len(condition.and_conditions))
+        self.assertEqual(nr_or_cond, len(condition.or_conditions))
+
+    def test_read_type_only(self):
+        self.check_condition({"type": "U"}, 'U')
+
+    def test_eq(self):
+        cond_dict = {
+            "index": 0,
+            "op": "=",
+            "tag": "(3004,000A)",
+            "type": "MN",
+            "values": [
+                "BEAM",
+                "BEAM_SESSION",
+                "CONTROL_POINT"
+            ]
+        }
+
+        def test_condition():
+            return self.check_condition(cond_dict, cond_type='MN', op='=',
+                                        tag='(3004,000A)',
+                                        values=['BEAM', 'BEAM_SESSION',
+                                                'CONTROL_POINT'])
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('Dose Summation Type is equal to "BEAM", '
+                         '"BEAM_SESSION" or "CONTROL_POINT"',
+                         condition.to_string(self.dict_info))
+
+    def test_greater(self):
+        cond_dict = {
+            "index": 0,
+            "op": ">",
+            "tag": "(0028,0008)",
+            "type": "MN",
+            "values": ["1"]
+        }
+
+        def test_condition():
+            return self.check_condition(cond_dict, cond_type='MN', op='>',
+                                        tag='(0028,0008)',
+                                        values=['1'])
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('Number of Frames is greater than 1',
+                         condition.to_string(self.dict_info))
+
+    def test_less(self):
+        cond_dict = {
+            "index": 0,
+            "op": "<",
+            "tag": "(0028,0008)",
+            "type": "MN",
+            "values": ["20"]
+        }
+
+        def test_condition():
+            return self.check_condition(cond_dict, cond_type='MN', op='<',
+                                        tag='(0028,0008)',
+                                        values=['20'])
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('Number of Frames is less than 20',
+                         condition.to_string(self.dict_info))
+
+    def test_points_to(self):
+        cond_dict = {
+            "index": 0,
+            "op": "=>",
+            "tag": "(0028,0009)",
+            "type": "MN",
+            "values": [
+                "1577061"
+            ]
+        }
+
+        def test_condition():
+            return self.check_condition(cond_dict, cond_type='MN', op='=>',
+                                        tag='(0028,0009)',
+                                        values=['1577061'])
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('Frame Increment Pointer points to '
+                         '(0018,1065) (Frame Time Vector)',
+                         condition.to_string(self.dict_info))
+
+    def test_exists(self):
+        cond_dict = {
+            "index": 0,
+            "op": "+",
+            "tag": "(7FE0,0010)",
+            "type": "MN"
+        }
+
+        def test_condition():
+            return self.check_condition(cond_dict, cond_type='MN', op='+',
+                                        tag='(7FE0,0010)')
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('Pixel Data exists',
+                         condition.to_string(self.dict_info))
+
+    def test_and_condition(self):
+        cond_dict = {
+            "and": [
+                {
+                    "index": 0,
+                    "op": "-",
+                    "tag": "(0040,E022)"
+                },
+                {
+                    "index": 1,
+                    "op": "+",
+                    "tag": "(0040,E023)"
+                },
+                {
+                    "index": 0,
+                    "op": "!=",
+                    "tag": "(0040,E025)",
+                    "values": ["TEST"]
+                }
+            ],
+            "type": "MU"
+        }
+
+        def test_condition():
+            cond = self.check_condition(
+                cond_dict, cond_type='MU', nr_and_cond=3)
+            self.check_sub_condition(
+                cond.and_conditions[0], op='-', tag='(0040,E022)')
+            self.check_sub_condition(
+                cond.and_conditions[1], op='+', tag='(0040,E023)',
+                index=1)
+            self.check_sub_condition(
+                cond.and_conditions[2], op='!=', tag='(0040,E025)',
+                values=['TEST'])
+            return cond
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('DICOM Media Retrieval Sequence is not present and '
+                         'WADO Retrieval Sequence[1] exists and WADO-RS '
+                         'Retrieval Sequence is not equal to "TEST"',
+                         condition.to_string(self.dict_info))
+
+    def test_or_condition(self):
+        cond_dict = {
+            "or": [
+                {
+                    "index": 0,
+                    "op": "-",
+                    "tag": "(0040,4072)"
+                },
+                {
+                    "index": 0,
+                    "op": "-",
+                    "tag": "(0040,4074)"
+                }
+            ],
+            "type": "MU"
+        }
+
+        def test_condition():
+            cond = self.check_condition(
+                cond_dict, cond_type='MU', nr_or_cond=2)
+            self.check_sub_condition(
+                cond.or_conditions[0], op='-', tag='(0040,4072)')
+            self.check_sub_condition(
+                cond.or_conditions[1], op='-', tag='(0040,4074)')
+            return cond
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
+        self.assertEqual('STOW-RS Storage Sequence is not present or '
+                         'XDS Storage Sequence is not present',
+                         condition.to_string(self.dict_info))
+
+    def test_other_condition(self):
+        cond_dict = {
+            "index": 0,
+            "op": "=",
+            "other_cond": {
+                "index": 0,
+                "op": "+",
+                "tag": "(0072,0704)",
+                "type": "MN"
+            },
+            "tag": "(0072,0704)",
+            "type": "MC",
+            "values": [
+                "PALETTE"
+            ]
+        }
+
+        def test_condition():
+            cond = self.check_condition(
+                cond_dict, cond_type='MC', op='=',
+                tag='(0072,0704)', values=['PALETTE'])
+            self.check_sub_condition(
+                cond.other_condition, op='+', tag='(0072,0704)')
+            self.assertEqual('MN', cond.other_condition.type)
+            return cond
+
+        condition = test_condition()
+        cond_dict = condition.dict()
+        test_condition()
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_edition_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_edition_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,213 +1,216 @@
-import logging
-import os
-import time
-
-import pyfakefs.fake_filesystem_unittest
-
-from dicom_validator import __version__
-from dicom_validator.spec_reader.edition_reader import EditionReader
-
-
-class MemoryEditionReader(EditionReader):
-    """Mock class that gets the file contents in constructor instead of
-    downloading them. We test this class to avoid real download connections
-    during the test.
-    """
-
-    def __init__(self, path, contents=''):
-        super(MemoryEditionReader, self).__init__(path=path)
-        self.html_contents = contents
-
-    def retrieve(self, html_path):
-        with open(html_path, 'w') as html_file:
-            html_file.write(self.html_contents)
-
-
-class EditionReaderTest(pyfakefs.fake_filesystem_unittest.TestCase):
-    def setUp(self):
-        super(EditionReaderTest, self).setUp()
-        self.setUpPyfakefs()
-        self.base_path = os.path.join('user', 'dicom-validator')
-        self.fs.create_dir(self.base_path)
-        logging.disable(logging.CRITICAL)
-
-    def create_edition_file_over_a_month_old(self, contents):
-        json_path = os.path.join(self.base_path, EditionReader.json_filename)
-        self.fs.create_file(json_path, contents=contents)
-        file_time = time.time() - 32 * 24 * 60 * 60.0
-        os.utime(json_path, (file_time, file_time))
-
-    def create_edition_file_less_than_a_month_old(self, contents):
-        json_path = os.path.join(self.base_path, EditionReader.json_filename)
-        self.fs.create_file(json_path, contents=contents)
-        file_time = time.time() - 27 * 24 * 60 * 60.0
-        os.utime(json_path, (file_time, file_time))
-
-    def test_empty_html(self):
-        reader = MemoryEditionReader(self.base_path, '')
-        self.assertIsNone(reader.get_editions())
-        self.assertFalse(
-            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
-
-    def test_no_html(self):
-        reader = MemoryEditionReader(self.base_path, 'Not html')
-        self.assertIsNone(reader.get_editions())
-        self.assertFalse(
-            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
-
-    def test_no_editions(self):
-        reader = MemoryEditionReader(
-            self.base_path,
-            '<html><A HREF="/medical/dicom/2014a/">test</A><html>')
-        self.assertIsNone(reader.get_editions())
-        self.assertFalse(
-            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
-
-    def test_valid_editions(self):
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2014a</A>'
-                            '2014b'
-                            '<a ref="foo">2015</a>'
-                            '<a ref="foo">2017e</a>')
-        self.assertEqual(['2014a', '2017e'], reader.get_editions())
-        self.assertTrue(
-            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
-
-    def test_keep_old_version(self):
-        self.create_edition_file_less_than_a_month_old('["2014a", "2014c"]')
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2018a</A>')
-        self.assertEqual(['2014a', '2014c'], reader.get_editions())
-
-    def test_replace_old_version(self):
-        self.create_edition_file_over_a_month_old('["2014a", "2014c"]')
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2018a</A>')
-        self.assertEqual(['2018a'], reader.get_editions())
-
-    def test_keep_local_version(self):
-        self.create_edition_file_over_a_month_old('["2014a", "2014c"]')
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2018a</A>')
-        self.assertEqual(['2014a', '2014c'], reader.get_editions(update=False))
-
-    def test_update_if_no_local_version_exists(self):
-        self.create_edition_file_over_a_month_old('[]')
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2018a</A>')
-        self.assertEqual(['2018a'], reader.get_editions(update=False))
-
-    def test_get_existing_revision(self):
-        reader = MemoryEditionReader(
-            self.base_path, '<html><A HREF="/bla/">2014a</A>'
-                            '<a ref="foo">2014e</a>')
-        self.assertEqual('2014a', reader.get_edition('2014a'))
-
-    def test_non_existing_revision(self):
-        reader = MemoryEditionReader(self.base_path,
-                                     '<html><A HREF="/bla/">2014a</A>'
-                                     '<a ref="foo">2014e</a>')
-        self.assertIsNone(reader.get_edition('2015a'))
-
-    def test_last_revision_in_year(self):
-        reader = MemoryEditionReader(self.base_path,
-                                     '<html><A HREF="/bla/">2014a</A>'
-                                     '<a ref="foo">2014c</a>'
-                                     '<a ref="foo">2015e</a>')
-        self.assertEqual('2014c', reader.get_edition('2014'))
-
-    def test_current_revision(self):
-        reader = MemoryEditionReader(self.base_path,
-                                     '<html><A HREF="/bla/">2014a</A>'
-                                     '<a ref="foo">2014c</a>'
-                                     '<a ref="foo">2015e</a>')
-        self.assertEqual('2015e', reader.get_edition('current'))
-
-    def test_check_none_revision(self):
-        reader = MemoryEditionReader('/foo/bar', '')
-        revision, path = reader.check_revision('none')
-        self.assertIsNone(revision)
-        self.assertEqual('/foo/bar', path)
-
-    def test_check_revision_existing(self):
-        base_path = 'base'
-        reader = MemoryEditionReader(base_path, '')
-        json_path = os.path.join(base_path, EditionReader.json_filename)
-        self.fs.create_file(json_path, contents='["2014a", "2014c", "2015a"]')
-        revision, path = reader.check_revision('2014')
-        self.assertEqual('2014c', revision)
-        self.assertEqual(os.path.join(base_path, '2014c'), path)
-
-    def test_check_revision_nonexisting(self):
-        base_path = '/foo/bar'
-        reader = MemoryEditionReader(base_path, '')
-        json_path = os.path.join(base_path, EditionReader.json_filename)
-        self.fs.create_file(json_path, contents='["2014a", "2014c", "2015a"]')
-        revision, path = reader.check_revision('2016')
-        self.assertIsNone(revision)
-        self.assertIsNone(path)
-
-    def test_is_current(self):
-        reader = MemoryEditionReader(self.base_path, '<html>'
-                                                     '<a ref="foo">2014a</a>'
-                                                     '<a ref="foo">2014c</a>'
-                                                     '<a ref="foo">2015a</a>'
-                                                     '<a ref="foo">2015e</a>')
-        self.assertTrue(reader.is_current('2015e'))
-        self.assertTrue(reader.is_current('2015'))
-        self.assertFalse(reader.is_current('2015a'))
-        self.assertFalse(reader.is_current('2015f'))
-        self.assertFalse(reader.is_current('2014'))
-        self.assertFalse(reader.is_current('2016'))
-        self.assertTrue(reader.is_current('current'))
-        self.assertTrue(reader.is_current(None))
-
-    def test_is_current_version(self):
-        json_path = os.path.join(self.base_path, EditionReader.json_filename)
-        self.assertFalse(EditionReader.is_current_version(json_path))
-        version_path = os.path.join(json_path, 'version')
-        self.fs.create_file(version_path, contents='0.2.1')
-        self.assertFalse(EditionReader.is_current_version(json_path))
-        os.remove(version_path)
-        self.fs.create_file(version_path, contents=__version__)
-        self.assertTrue(EditionReader.is_current_version(json_path))
-
-    def test_write_current_version(self):
-        json_path = os.path.join(self.base_path, EditionReader.json_filename)
-        self.fs.create_dir(json_path)
-        self.assertFalse(EditionReader.is_current_version(json_path))
-        EditionReader.write_current_version(json_path)
-        self.assertTrue(EditionReader.is_current_version(json_path))
-
-    def test_recreate_json_if_needed(self):
-        self.create_json_files_called = 0
-
-        def create_json_files(cls, docbook_path, json_path):
-            self.create_json_files_called += 1
-            for name in ('dict_info.json', 'iod_info.json',
-                         'module_info.json', 'uid_info.json'):
-                path = os.path.join(json_path, name)
-                if not os.path.exists(path):
-                    self.fs.create_file(path)
-
-        docbook_path = os.path.join(self.base_path, '2014a', 'docbook')
-        for chapter_name in ('part03.xml', 'part04.xml', 'part06.xml'):
-            self.fs.create_file(os.path.join(docbook_path, chapter_name))
-        orig_create_json_files = MemoryEditionReader.create_json_files
-        try:
-            MemoryEditionReader.create_json_files = create_json_files
-            reader = MemoryEditionReader(self.base_path, '')
-            json_path = os.path.join(self.base_path,
-                                     EditionReader.json_filename)
-            self.fs.create_file(json_path,
-                                contents='["2014a", "2014c", "2015a"]')
-            reader.get_revision("2014a")
-            self.assertEqual(1, self.create_json_files_called)
-            reader.get_revision("2014a")
-            self.assertEqual(2, self.create_json_files_called)
-            json_path = os.path.join(self.base_path, '2014a', 'json')
-            EditionReader.write_current_version(json_path)
-            reader.get_revision("2014a")
-            self.assertEqual(2, self.create_json_files_called)
-        finally:
-            MemoryEditionReader.create_json_files = orig_create_json_files
+import logging
+import os
+import time
+
+import pyfakefs.fake_filesystem_unittest
+
+from dicom_validator import __version__
+from dicom_validator.spec_reader.edition_reader import EditionReader
+
+
+class MemoryEditionReader(EditionReader):
+    """Mock class that gets the file contents in constructor instead of
+    downloading them. We test this class to avoid real download connections
+    during the test.
+    """
+
+    def __init__(self, path, contents=''):
+        super(MemoryEditionReader, self).__init__(path=path)
+        self.html_contents = contents
+
+    def retrieve(self, html_path):
+        with open(html_path, 'w') as html_file:
+            html_file.write(self.html_contents)
+
+
+class EditionReaderTest(pyfakefs.fake_filesystem_unittest.TestCase):
+    def setUp(self):
+        super(EditionReaderTest, self).setUp()
+        self.setUpPyfakefs()
+        self.base_path = os.path.join('user', 'dicom-validator')
+        self.fs.create_dir(self.base_path)
+        logging.disable(logging.CRITICAL)
+
+    def tearDown(self):
+        logging.disable(logging.DEBUG)
+
+    def create_edition_file_over_a_month_old(self, contents):
+        json_path = os.path.join(self.base_path, EditionReader.json_filename)
+        self.fs.create_file(json_path, contents=contents)
+        file_time = time.time() - 32 * 24 * 60 * 60.0
+        os.utime(json_path, (file_time, file_time))
+
+    def create_edition_file_less_than_a_month_old(self, contents):
+        json_path = os.path.join(self.base_path, EditionReader.json_filename)
+        self.fs.create_file(json_path, contents=contents)
+        file_time = time.time() - 27 * 24 * 60 * 60.0
+        os.utime(json_path, (file_time, file_time))
+
+    def test_empty_html(self):
+        reader = MemoryEditionReader(self.base_path, '')
+        self.assertIsNone(reader.get_editions())
+        self.assertFalse(
+            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
+
+    def test_no_html(self):
+        reader = MemoryEditionReader(self.base_path, 'Not html')
+        self.assertIsNone(reader.get_editions())
+        self.assertFalse(
+            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
+
+    def test_no_editions(self):
+        reader = MemoryEditionReader(
+            self.base_path,
+            '<html><A HREF="/medical/dicom/2014a/">test</A><html>')
+        self.assertIsNone(reader.get_editions())
+        self.assertFalse(
+            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
+
+    def test_valid_editions(self):
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2014a</A>'
+                            '2014b'
+                            '<a ref="foo">2015</a>'
+                            '<a ref="foo">2017e</a>')
+        self.assertEqual(['2014a', '2017e'], reader.get_editions())
+        self.assertTrue(
+            os.path.exists(os.path.join(self.base_path, reader.json_filename)))
+
+    def test_keep_old_version(self):
+        self.create_edition_file_less_than_a_month_old('["2014a", "2014c"]')
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2018a</A>')
+        self.assertEqual(['2014a', '2014c'], reader.get_editions())
+
+    def test_replace_old_version(self):
+        self.create_edition_file_over_a_month_old('["2014a", "2014c"]')
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2018a</A>')
+        self.assertEqual(['2018a'], reader.get_editions())
+
+    def test_keep_local_version(self):
+        self.create_edition_file_over_a_month_old('["2014a", "2014c"]')
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2018a</A>')
+        self.assertEqual(['2014a', '2014c'], reader.get_editions(update=False))
+
+    def test_update_if_no_local_version_exists(self):
+        self.create_edition_file_over_a_month_old('[]')
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2018a</A>')
+        self.assertEqual(['2018a'], reader.get_editions(update=False))
+
+    def test_get_existing_revision(self):
+        reader = MemoryEditionReader(
+            self.base_path, '<html><A HREF="/bla/">2014a</A>'
+                            '<a ref="foo">2014e</a>')
+        self.assertEqual('2014a', reader.get_edition('2014a'))
+
+    def test_non_existing_revision(self):
+        reader = MemoryEditionReader(self.base_path,
+                                     '<html><A HREF="/bla/">2014a</A>'
+                                     '<a ref="foo">2014e</a>')
+        self.assertIsNone(reader.get_edition('2015a'))
+
+    def test_last_revision_in_year(self):
+        reader = MemoryEditionReader(self.base_path,
+                                     '<html><A HREF="/bla/">2014a</A>'
+                                     '<a ref="foo">2014c</a>'
+                                     '<a ref="foo">2015e</a>')
+        self.assertEqual('2014c', reader.get_edition('2014'))
+
+    def test_current_revision(self):
+        reader = MemoryEditionReader(self.base_path,
+                                     '<html><A HREF="/bla/">2014a</A>'
+                                     '<a ref="foo">2014c</a>'
+                                     '<a ref="foo">2015e</a>')
+        self.assertEqual('2015e', reader.get_edition('current'))
+
+    def test_check_none_revision(self):
+        reader = MemoryEditionReader('/foo/bar', '')
+        revision, path = reader.check_revision('none')
+        self.assertIsNone(revision)
+        self.assertEqual('/foo/bar', path)
+
+    def test_check_revision_existing(self):
+        base_path = 'base'
+        reader = MemoryEditionReader(base_path, '')
+        json_path = os.path.join(base_path, EditionReader.json_filename)
+        self.fs.create_file(json_path, contents='["2014a", "2014c", "2015a"]')
+        revision, path = reader.check_revision('2014')
+        self.assertEqual('2014c', revision)
+        self.assertEqual(os.path.join(base_path, '2014c'), path)
+
+    def test_check_revision_nonexisting(self):
+        base_path = '/foo/bar'
+        reader = MemoryEditionReader(base_path, '')
+        json_path = os.path.join(base_path, EditionReader.json_filename)
+        self.fs.create_file(json_path, contents='["2014a", "2014c", "2015a"]')
+        revision, path = reader.check_revision('2016')
+        self.assertIsNone(revision)
+        self.assertIsNone(path)
+
+    def test_is_current(self):
+        reader = MemoryEditionReader(self.base_path, '<html>'
+                                                     '<a ref="foo">2014a</a>'
+                                                     '<a ref="foo">2014c</a>'
+                                                     '<a ref="foo">2015a</a>'
+                                                     '<a ref="foo">2015e</a>')
+        self.assertTrue(reader.is_current('2015e'))
+        self.assertTrue(reader.is_current('2015'))
+        self.assertFalse(reader.is_current('2015a'))
+        self.assertFalse(reader.is_current('2015f'))
+        self.assertFalse(reader.is_current('2014'))
+        self.assertFalse(reader.is_current('2016'))
+        self.assertTrue(reader.is_current('current'))
+        self.assertTrue(reader.is_current(None))
+
+    def test_is_current_version(self):
+        json_path = os.path.join(self.base_path, EditionReader.json_filename)
+        self.assertFalse(EditionReader.is_current_version(json_path))
+        version_path = os.path.join(json_path, 'version')
+        self.fs.create_file(version_path, contents='0.2.1')
+        self.assertFalse(EditionReader.is_current_version(json_path))
+        os.remove(version_path)
+        self.fs.create_file(version_path, contents=__version__)
+        self.assertTrue(EditionReader.is_current_version(json_path))
+
+    def test_write_current_version(self):
+        json_path = os.path.join(self.base_path, EditionReader.json_filename)
+        self.fs.create_dir(json_path)
+        self.assertFalse(EditionReader.is_current_version(json_path))
+        EditionReader.write_current_version(json_path)
+        self.assertTrue(EditionReader.is_current_version(json_path))
+
+    def test_recreate_json_if_needed(self):
+        self.create_json_files_called = 0
+
+        def create_json_files(cls, docbook_path, json_path):
+            self.create_json_files_called += 1
+            for name in ('dict_info.json', 'iod_info.json',
+                         'module_info.json', 'uid_info.json'):
+                path = os.path.join(json_path, name)
+                if not os.path.exists(path):
+                    self.fs.create_file(path)
+
+        docbook_path = os.path.join(self.base_path, '2014a', 'docbook')
+        for chapter_name in ('part03.xml', 'part04.xml', 'part06.xml'):
+            self.fs.create_file(os.path.join(docbook_path, chapter_name))
+        orig_create_json_files = MemoryEditionReader.create_json_files
+        try:
+            MemoryEditionReader.create_json_files = create_json_files
+            reader = MemoryEditionReader(self.base_path, '')
+            json_path = os.path.join(self.base_path,
+                                     EditionReader.json_filename)
+            self.fs.create_file(json_path,
+                                contents='["2014a", "2014c", "2015a"]')
+            reader.get_revision("2014a")
+            self.assertEqual(1, self.create_json_files_called)
+            reader.get_revision("2014a")
+            self.assertEqual(2, self.create_json_files_called)
+            json_path = os.path.join(self.base_path, '2014a', 'json')
+            EditionReader.write_current_version(json_path)
+            reader.get_revision("2014a")
+            self.assertEqual(2, self.create_json_files_called)
+        finally:
+            MemoryEditionReader.create_json_files = orig_create_json_files
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_part3_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_part3_reader.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import os
-import unittest
-
-import pyfakefs.fake_filesystem_unittest
-
-from dicom_validator.spec_reader.part3_reader import Part3Reader
-from dicom_validator.spec_reader.spec_reader import (
-    SpecReaderLookupError, SpecReaderParseError, SpecReaderFileError
-)
-from dicom_validator.tests.test_utils import spec_fixture_path
-
-
-class ReadPart3Test(pyfakefs.fake_filesystem_unittest.TestCase):
-    doc_contents = None
-
-    @classmethod
-    def setUpClass(cls):
-        with open(os.path.join(spec_fixture_path(),
-                               'part03.xml'), 'rb') as spec_file:
-            cls.doc_contents = spec_file.read()
-
-    def setUp(self):
-        super(ReadPart3Test, self).setUp()
-        self.setUpPyfakefs()
-        spec_path = os.path.join('dicom', 'specs')
-        part3_path = os.path.join(spec_path, 'part03.xml')
-        self.fs.create_file(part3_path, contents=self.doc_contents)
-        self.reader = Part3Reader(spec_path)
-
-    def test_read_empty_doc_file(self):
-        spec_path = '/var/dicom/specs'
-        os.makedirs(spec_path)
-        self.fs.create_file(os.path.join(spec_path, 'part03.xml'))
-        spec_reader = Part3Reader(spec_path)
-        self.assertRaises(SpecReaderFileError,
-                          spec_reader.iod_description, 'A.16')
-
-    def test_read_invalid_doc_file(self):
-        spec_path = '/var/dicom/specs'
-        os.makedirs(spec_path)
-        self.fs.create_file(os.path.join(spec_path, 'part03.xml'),
-                            contents='Not an xml')
-        spec_reader = Part3Reader(spec_path)
-        self.assertRaises(SpecReaderFileError,
-                          spec_reader.iod_description, 'A.6')
-
-    def test_read_incomplete_doc_file(self):
-        spec_path = '/var/dicom/specs'
-        os.makedirs(spec_path)
-        self.fs.create_file(os.path.join(
-            spec_path, 'part03.xml'),
-            contents='<book xmlns="http://docbook.org/ns/docbook">\n</book>')
-        reader = Part3Reader(spec_path)
-        self.assertRaises(SpecReaderParseError, reader.iod_description, 'A.6')
-
-    def test_lookup_sop_class(self):
-        self.assertRaises(SpecReaderLookupError,
-                          self.reader.iod_description, 'A.0')
-        description = self.reader.iod_description(chapter='A.3')
-        self.assertIsNotNone(description)
-        self.assertTrue('title' in description)
-        self.assertEqual(description['title'], 'Computed Tomography Image IOD')
-
-    def test_get_iod_modules(self):
-        description = self.reader.iod_description(chapter='A.38.1')
-        self.assertIn('modules', description)
-        modules = description['modules']
-        self.assertEqual(27, len(modules))
-        self.assertIn('General Equipment', modules)
-        module = modules['General Equipment']
-        self.assertEqual('C.7.5.1', module['ref'])
-        self.assertEqual('M', module['use'])
-
-    def test_optional_iod_module(self):
-        description = self.reader.iod_description(chapter='A.38.1')
-        self.assertIn('modules', description)
-        modules = description['modules']
-        self.assertIn('Clinical Trial Subject', modules)
-        module = modules['Clinical Trial Subject']
-        self.assertEqual('C.7.1.3', module['ref'])
-        self.assertEqual('U', module['use'])
-
-    def test_iod_descriptions(self):
-        descriptions = self.reader.iod_descriptions()
-        self.assertEqual(4, len(descriptions))
-        self.assertIn('A.3', descriptions)
-        self.assertIn('A.18', descriptions)
-        self.assertIn('A.38.1', descriptions)
-
-    def test_module_description(self):
-        self.assertRaises(SpecReaderLookupError,
-                          self.reader.module_description, 'C.9.9.9')
-        description = self.reader.module_description('C.7.1.3')
-        self.assertEqual(9, len(description))
-        self.assertIn('(0012,0031)', description)
-        self.assertEqual('Clinical Trial Site Name',
-                         description['(0012,0031)']['name'])
-        self.assertEqual('2', description['(0012,0031)']['type'])
-
-    def test_sequence_inside_module_description(self):
-        description = self.reader.module_description('C.7.2.3')
-        self.assertEqual(3, len(description))
-        self.assertIn('(0012,0083)', description)
-        self.assertIn('items', description['(0012,0083)'])
-        sequence_description = description['(0012,0083)']['items']
-        self.assertEqual(3, len(sequence_description))
-        self.assertIn('(0012,0020)', sequence_description)
-        self.assertEqual('Clinical Trial Protocol ID',
-                         sequence_description['(0012,0020)']['name'])
-        self.assertEqual('1C', sequence_description['(0012,0020)']['type'])
-
-    def test_referenced_macro(self):
-        # module has 2 directly included attributes
-        # and 21 attribute in referenced table
-        description = self.reader.module_description('C.7.6.3')
-        self.assertEqual(3, len(description))
-        self.assertIn('(0028,7FE0)', description)
-        self.assertIn('include', description)
-        self.assertIn('C.7-11b', description['include'])
-        description = self.reader.module_description('C.7-11b')
-        self.assertEqual(21, len(description))
-        self.assertIn('(7FE0,0010)', description)
-
-    def test_module_descriptions(self):
-        descriptions = self.reader.module_descriptions()
-        # 42 modules from 3 classes (20/23/26) with overlapping
-        # common modules + 27 referenced macros
-        self.assertEqual(69, len(descriptions))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import os
+import unittest
+
+import pyfakefs.fake_filesystem_unittest
+
+from dicom_validator.spec_reader.part3_reader import Part3Reader
+from dicom_validator.spec_reader.spec_reader import (
+    SpecReaderLookupError, SpecReaderParseError, SpecReaderFileError
+)
+from dicom_validator.tests.test_utils import spec_fixture_path
+
+
+class ReadPart3Test(pyfakefs.fake_filesystem_unittest.TestCase):
+    doc_contents = None
+
+    @classmethod
+    def setUpClass(cls):
+        with open(os.path.join(spec_fixture_path(),
+                               'part03.xml'), 'rb') as spec_file:
+            cls.doc_contents = spec_file.read()
+
+    def setUp(self):
+        super(ReadPart3Test, self).setUp()
+        self.setUpPyfakefs()
+        spec_path = os.path.join('dicom', 'specs')
+        part3_path = os.path.join(spec_path, 'part03.xml')
+        self.fs.create_file(part3_path, contents=self.doc_contents)
+        self.reader = Part3Reader(spec_path)
+
+    def test_read_empty_doc_file(self):
+        spec_path = '/var/dicom/specs'
+        os.makedirs(spec_path)
+        self.fs.create_file(os.path.join(spec_path, 'part03.xml'))
+        spec_reader = Part3Reader(spec_path)
+        self.assertRaises(SpecReaderFileError,
+                          spec_reader.iod_description, 'A.16')
+
+    def test_read_invalid_doc_file(self):
+        spec_path = '/var/dicom/specs'
+        os.makedirs(spec_path)
+        self.fs.create_file(os.path.join(spec_path, 'part03.xml'),
+                            contents='Not an xml')
+        spec_reader = Part3Reader(spec_path)
+        self.assertRaises(SpecReaderFileError,
+                          spec_reader.iod_description, 'A.6')
+
+    def test_read_incomplete_doc_file(self):
+        spec_path = '/var/dicom/specs'
+        os.makedirs(spec_path)
+        self.fs.create_file(os.path.join(
+            spec_path, 'part03.xml'),
+            contents='<book xmlns="http://docbook.org/ns/docbook">\n</book>')
+        reader = Part3Reader(spec_path)
+        self.assertRaises(SpecReaderParseError, reader.iod_description, 'A.6')
+
+    def test_lookup_sop_class(self):
+        self.assertRaises(SpecReaderLookupError,
+                          self.reader.iod_description, 'A.0')
+        description = self.reader.iod_description(chapter='A.3')
+        self.assertIsNotNone(description)
+        self.assertTrue('title' in description)
+        self.assertEqual(description['title'], 'Computed Tomography Image IOD')
+
+    def test_get_iod_modules(self):
+        description = self.reader.iod_description(chapter='A.38.1')
+        self.assertIn('modules', description)
+        modules = description['modules']
+        self.assertEqual(27, len(modules))
+        self.assertIn('General Equipment', modules)
+        module = modules['General Equipment']
+        self.assertEqual('C.7.5.1', module['ref'])
+        self.assertEqual('M', module['use'])
+
+    def test_optional_iod_module(self):
+        description = self.reader.iod_description(chapter='A.38.1')
+        self.assertIn('modules', description)
+        modules = description['modules']
+        self.assertIn('Clinical Trial Subject', modules)
+        module = modules['Clinical Trial Subject']
+        self.assertEqual('C.7.1.3', module['ref'])
+        self.assertEqual('U', module['use'])
+
+    def test_iod_descriptions(self):
+        descriptions = self.reader.iod_descriptions()
+        self.assertEqual(4, len(descriptions))
+        self.assertIn('A.3', descriptions)
+        self.assertIn('A.18', descriptions)
+        self.assertIn('A.38.1', descriptions)
+
+    def test_module_description(self):
+        self.assertRaises(SpecReaderLookupError,
+                          self.reader.module_description, 'C.9.9.9')
+        description = self.reader.module_description('C.7.1.3')
+        self.assertEqual(9, len(description))
+        self.assertIn('(0012,0031)', description)
+        self.assertEqual('Clinical Trial Site Name',
+                         description['(0012,0031)']['name'])
+        self.assertEqual('2', description['(0012,0031)']['type'])
+
+    def test_sequence_inside_module_description(self):
+        description = self.reader.module_description('C.7.2.3')
+        self.assertEqual(3, len(description))
+        self.assertIn('(0012,0083)', description)
+        self.assertIn('items', description['(0012,0083)'])
+        sequence_description = description['(0012,0083)']['items']
+        self.assertEqual(3, len(sequence_description))
+        self.assertIn('(0012,0020)', sequence_description)
+        self.assertEqual('Clinical Trial Protocol ID',
+                         sequence_description['(0012,0020)']['name'])
+        self.assertEqual('1C', sequence_description['(0012,0020)']['type'])
+
+    def test_referenced_macro(self):
+        # module has 2 directly included attributes
+        # and 21 attribute in referenced table
+        description = self.reader.module_description('C.7.6.3')
+        self.assertEqual(3, len(description))
+        self.assertIn('(0028,7FE0)', description)
+        self.assertIn('include', description)
+        self.assertIn('C.7-11b', description['include'])
+        description = self.reader.module_description('C.7-11b')
+        self.assertEqual(21, len(description))
+        self.assertIn('(7FE0,0010)', description)
+
+    def test_module_descriptions(self):
+        descriptions = self.reader.module_descriptions()
+        # 42 modules from 3 classes (20/23/26) with overlapping
+        # common modules + 27 referenced macros
+        self.assertEqual(69, len(descriptions))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_part6_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_part6_reader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import os
-import unittest
-
-import pyfakefs.fake_filesystem_unittest
-
-from dicom_validator.spec_reader.part6_reader import Part6Reader
-from dicom_validator.tests.test_utils import spec_fixture_path
-
-
-class Part6ReaderTest(pyfakefs.fake_filesystem_unittest.TestCase):
-    doc_contents = None
-
-    @classmethod
-    def setUpClass(cls):
-        with open(os.path.join(spec_fixture_path(), 'part06.xml'),
-                  'rb') as spec_file:
-            cls.doc_contents = spec_file.read()
-
-    def setUp(self):
-        super(Part6ReaderTest, self).setUp()
-        self.setUpPyfakefs()
-        spec_path = os.path.join('dicom', 'docbook')
-        part6_path = os.path.join(spec_path, 'part06.xml')
-        self.fs.create_file(part6_path, contents=self.doc_contents)
-        self.reader = Part6Reader(spec_path)
-
-    def test_undefined_id(self):
-        self.assertIsNone(self.reader.data_element('(0011,0011)'))
-
-    def test_data_element(self):
-        element = self.reader.data_element('(0008,0005)')
-        self.assertIsNotNone(element)
-        self.assertEqual('Specific Character Set', element['name'])
-        self.assertEqual('CS', element['vr'])
-        self.assertEqual('1-n', element['vm'])
-
-    def test_data_elements(self):
-        elements = self.reader.data_elements()
-        self.assertEqual(8, len(elements))
-
-    def test_sop_class_uids(self):
-        sop_class_uids = self.reader.sop_class_uids()
-        self.assertEqual(3, len(sop_class_uids))
-        self.assertIn('1.2.840.10008.1.1', sop_class_uids)
-        self.assertEqual('Verification SOP Class',
-                         sop_class_uids['1.2.840.10008.1.1'])
-
-    def test_uid_type(self):
-        xfer_syntax_uids = self.reader.uids('Transfer Syntax')
-        self.assertEqual(2, len(xfer_syntax_uids))
-        self.assertIn('1.2.840.10008.1.2.4.80', xfer_syntax_uids)
-        self.assertEqual('JPEG-LS Lossless Image Compression',
-                         xfer_syntax_uids['1.2.840.10008.1.2.4.80'])
-
-    def test_all_uids(self):
-        uids = self.reader.all_uids()
-        self.assertEqual(2, len(uids))
-        self.assertIn('Transfer Syntax', uids)
-        self.assertIn('SOP Class', uids)
-        uid_nr = sum([len(uid_dict) for uid_dict in uids.values()])
-        self.assertEqual(5, uid_nr)
-
-    def test_sop_class_name(self):
-        self.assertEqual(
-            'Enhanced US Volume Storage',
-            self.reader.sop_class_name('1.2.840.10008.5.1.4.1.1.6.2'))
-
-    def test_sop_class_uid(self):
-        self.assertEqual('1.2.840.10008.5.1.4.1.1.2',
-                         self.reader.sop_class_uid('CT Image Storage'))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import os
+import unittest
+
+import pyfakefs.fake_filesystem_unittest
+
+from dicom_validator.spec_reader.part6_reader import Part6Reader
+from dicom_validator.tests.test_utils import spec_fixture_path
+
+
+class Part6ReaderTest(pyfakefs.fake_filesystem_unittest.TestCase):
+    doc_contents = None
+
+    @classmethod
+    def setUpClass(cls):
+        with open(os.path.join(spec_fixture_path(), 'part06.xml'),
+                  'rb') as spec_file:
+            cls.doc_contents = spec_file.read()
+
+    def setUp(self):
+        super(Part6ReaderTest, self).setUp()
+        self.setUpPyfakefs()
+        spec_path = os.path.join('dicom', 'docbook')
+        part6_path = os.path.join(spec_path, 'part06.xml')
+        self.fs.create_file(part6_path, contents=self.doc_contents)
+        self.reader = Part6Reader(spec_path)
+
+    def test_undefined_id(self):
+        self.assertIsNone(self.reader.data_element('(0011,0011)'))
+
+    def test_data_element(self):
+        element = self.reader.data_element('(0008,0005)')
+        self.assertIsNotNone(element)
+        self.assertEqual('Specific Character Set', element['name'])
+        self.assertEqual('CS', element['vr'])
+        self.assertEqual('1-n', element['vm'])
+
+    def test_data_elements(self):
+        elements = self.reader.data_elements()
+        self.assertEqual(8, len(elements))
+
+    def test_sop_class_uids(self):
+        sop_class_uids = self.reader.sop_class_uids()
+        self.assertEqual(3, len(sop_class_uids))
+        self.assertIn('1.2.840.10008.1.1', sop_class_uids)
+        self.assertEqual('Verification SOP Class',
+                         sop_class_uids['1.2.840.10008.1.1'])
+
+    def test_uid_type(self):
+        xfer_syntax_uids = self.reader.uids('Transfer Syntax')
+        self.assertEqual(2, len(xfer_syntax_uids))
+        self.assertIn('1.2.840.10008.1.2.4.80', xfer_syntax_uids)
+        self.assertEqual('JPEG-LS Lossless Image Compression',
+                         xfer_syntax_uids['1.2.840.10008.1.2.4.80'])
+
+    def test_all_uids(self):
+        uids = self.reader.all_uids()
+        self.assertEqual(2, len(uids))
+        self.assertIn('Transfer Syntax', uids)
+        self.assertIn('SOP Class', uids)
+        uid_nr = sum([len(uid_dict) for uid_dict in uids.values()])
+        self.assertEqual(5, uid_nr)
+
+    def test_sop_class_name(self):
+        self.assertEqual(
+            'Enhanced US Volume Storage',
+            self.reader.sop_class_name('1.2.840.10008.5.1.4.1.1.6.2'))
+
+    def test_sop_class_uid(self):
+        self.assertEqual('1.2.840.10008.5.1.4.1.1.2',
+                         self.reader.sop_class_uid('CT Image Storage'))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dicom-validator-0.3.4/dicom_validator/spec_reader/tests/test_spec_reader.py` & `dicom-validator-0.3.5/dicom_validator/spec_reader/tests/test_spec_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-import os
-import unittest
-
-import pyfakefs.fake_filesystem_unittest
-
-from dicom_validator.spec_reader.spec_reader import (
-    SpecReader, SpecReaderFileError
-)
-
-
-class ReadSpecTest(pyfakefs.fake_filesystem_unittest.TestCase):
-    def setUp(self):
-        super(ReadSpecTest, self).setUp()
-        self.setUpPyfakefs()
-
-    def test_missing_path(self):
-        spec_path = '/var/dicom/specs'
-        self.assertRaises(OSError, SpecReader, spec_path)
-
-    def test_missing_doc_files(self):
-        spec_path = '/var/dicom/specs'
-        os.makedirs(spec_path)
-        self.fs.create_file(os.path.join('notadoc.xml'))
-        self.assertRaises(SpecReaderFileError, SpecReader, spec_path)
-
-    def test_existing_doc_files(self):
-        spec_path = '/var/dicom/specs'
-        os.makedirs(spec_path)
-        self.fs.create_file(os.path.join(spec_path, 'part03.xml'))
-        self.assertTrue(SpecReader(spec_path))
-
-    def test_cleaned_uid(self):
-        orig_value = '1.2.840.10008.5.' \
-                     '\u200b1.\u200b4.\u200b1.\u200b1.\u200b88.\u200b72'
-        self.assertEqual('1.2.840.10008.5.1.4.1.1.88.72',
-                         SpecReader.cleaned_value(orig_value))
-
-        if __name__ == '__main__':
-            unittest.main()
+import os
+import unittest
+
+import pyfakefs.fake_filesystem_unittest
+
+from dicom_validator.spec_reader.spec_reader import (
+    SpecReader, SpecReaderFileError
+)
+
+
+class ReadSpecTest(pyfakefs.fake_filesystem_unittest.TestCase):
+    def setUp(self):
+        super(ReadSpecTest, self).setUp()
+        self.setUpPyfakefs()
+
+    def test_missing_path(self):
+        spec_path = '/var/dicom/specs'
+        self.assertRaises(OSError, SpecReader, spec_path)
+
+    def test_missing_doc_files(self):
+        spec_path = '/var/dicom/specs'
+        os.makedirs(spec_path)
+        self.fs.create_file(os.path.join('notadoc.xml'))
+        self.assertRaises(SpecReaderFileError, SpecReader, spec_path)
+
+    def test_existing_doc_files(self):
+        spec_path = '/var/dicom/specs'
+        os.makedirs(spec_path)
+        self.fs.create_file(os.path.join(spec_path, 'part03.xml'))
+        self.assertTrue(SpecReader(spec_path))
+
+    def test_cleaned_uid(self):
+        orig_value = '1.2.840.10008.5.' \
+                     '\u200b1.\u200b4.\u200b1.\u200b1.\u200b88.\u200b72'
+        self.assertEqual('1.2.840.10008.5.1.4.1.1.88.72',
+                         SpecReader.cleaned_value(orig_value))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dicom-validator-0.3.4/dicom_validator/validator/dicom_file_validator.py` & `dicom-validator-0.3.5/dicom_validator/validator/dicom_file_validator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-import logging
-import os
-import sys
-
-from pydicom import dcmread
-from pydicom.errors import InvalidDicomError
-
-from dicom_validator.validator.iod_validator import IODValidator
-
-
-class DicomFileValidator(object):
-    def __init__(self, iod_info, module_info, dict_info=None,
-                 log_level=logging.INFO):
-        self._module_info = module_info
-        self._iod_info = iod_info
-        self._dict_info = dict_info
-        self.logger = logging.getLogger()
-        self.logger.level = log_level
-        if not self.logger.handlers:
-            self.logger.addHandler(logging.StreamHandler(sys.stdout))
-
-    def validate(self, path):
-        errors = {}
-        if not os.path.exists(path):
-            errors.update({path: {'fatal': 'File missing'}})
-            self.logger.warning('\n"%s" does not exist - skipping', path)
-        else:
-            if os.path.isdir(path):
-                errors.update(self.validate_dir(path))
-            else:
-                errors.update(self.validate_file(path))
-        return errors
-
-    def validate_dir(self, dir_path):
-        errors = {}
-        for root, _, names in os.walk(dir_path):
-            for name in names:
-                errors.update(self.validate(os.path.join(root, name)))
-        return errors
-
-    def validate_file(self, file_path):
-        self.logger.info('\nProcessing DICOM file "%s"', file_path)
-        try:
-            data_set = dcmread(file_path, defer_size=1024)
-        except InvalidDicomError:
-            return {file_path: {'fatal': 'Invalid DICOM file'}}
-        return {
-            file_path: IODValidator(data_set, self._iod_info,
-                                    self._module_info, self._dict_info,
-                                    self.logger.level).validate()
-        }
+import logging
+import os
+import sys
+
+from pydicom import dcmread
+from pydicom.errors import InvalidDicomError
+
+from dicom_validator.validator.iod_validator import IODValidator
+
+
+class DicomFileValidator:
+    def __init__(self, iod_info, module_info, dict_info=None,
+                 log_level=logging.INFO, force_read=False):
+        self._module_info = module_info
+        self._iod_info = iod_info
+        self._dict_info = dict_info
+        self.logger = logging.getLogger()
+        self.logger.level = log_level
+        if not self.logger.hasHandlers():
+            self.logger.addHandler(logging.StreamHandler(sys.stdout))
+        self._force_read = force_read
+
+    def validate(self, path):
+        errors = {}
+        if not os.path.exists(path):
+            errors.update({path: {'fatal': 'File missing'}})
+            self.logger.warning('\n"%s" does not exist - skipping', path)
+        else:
+            if os.path.isdir(path):
+                errors.update(self.validate_dir(path))
+            else:
+                errors.update(self.validate_file(path))
+        return errors
+
+    def validate_dir(self, dir_path):
+        errors = {}
+        for root, _, names in os.walk(dir_path):
+            for name in names:
+                errors.update(self.validate(os.path.join(root, name)))
+        return errors
+
+    def validate_file(self, file_path):
+        self.logger.info('\nProcessing DICOM file "%s"', file_path)
+        try:
+            data_set = dcmread(file_path, defer_size=1024, force=self._force_read)
+        except InvalidDicomError:
+            self.logger.error(f'Invalid DICOM file: {file_path}')
+            return {file_path: {'fatal': 'Invalid DICOM file'}}
+        return {
+            file_path: IODValidator(data_set, self._iod_info,
+                                    self._module_info, self._dict_info,
+                                    self.logger.level).validate()
+        }
```

### Comparing `dicom-validator-0.3.4/dicom_validator/validator/tests/test_dicom_file_validator.py` & `dicom-validator-0.3.5/dicom_validator/validator/tests/test_dicom_file_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,122 @@
-import json
-import logging
-import os
-import unittest
-
-import pyfakefs.fake_filesystem_unittest
-from pydicom import write_file
-from pydicom.dataset import Dataset, FileDataset
-
-from dicom_validator.spec_reader.edition_reader import EditionReader
-from dicom_validator.tests.test_utils import json_fixture_path, \
-    dicom_fixture_path
-from dicom_validator.validator.dicom_file_validator import DicomFileValidator
-
-
-class DicomFileValidatorTestBase(unittest.TestCase):
-    iod_info = None
-    module_info = None
-
-    @classmethod
-    def setUpClass(cls):
-        with open(os.path.join(json_fixture_path(),
-                               EditionReader.iod_info_json)) as info_file:
-            cls.iod_info = json.load(info_file)
-        with open(os.path.join(json_fixture_path(),
-                               EditionReader.module_info_json)) as info_file:
-            cls.module_info = json.load(info_file)
-
-    def setUp(self):
-        logging.disable(logging.CRITICAL)
-        self.validator = DicomFileValidator(self.iod_info, self.module_info)
-
-
-class FakeDicomFileValidatorTest(DicomFileValidatorTestBase,
-                                 pyfakefs.fake_filesystem_unittest.TestCase):
-    iod_info = None
-    module_info = None
-
-    def setUp(self):
-        super(FakeDicomFileValidatorTest, self).setUp()
-        self.setUpPyfakefs()
-
-    @staticmethod
-    def create_metadata():
-        metadata = Dataset()
-        metadata.MediaStorageSOPClassUID = '1.2.840.10008.5.1.4.1.1.7'
-        metadata.MediaStorageSOPInstanceUID = '1.2.3'
-        metadata.TransferSyntaxUID = '1.2.840.10008.1.2'
-        metadata.ImplementationClassUID = '1.3.6.1.4.1.5962.2'
-        return metadata
-
-    def assert_fatal_error(self, filename, error_string):
-        error_dict = self.validator.validate(filename)
-        self.assertEqual(1, len(error_dict))
-        name = list(error_dict.keys())[0]
-        self.assertEqual(filename, name)
-        errors = error_dict[name]
-        self.assertEqual({'fatal': error_string}, errors)
-
-    def test_non_existing_file(self):
-        self.assert_fatal_error('non_existing', error_string='File missing')
-
-    def test_invalid_file(self):
-        self.fs.create_file('test', contents='invalid')
-        self.assert_fatal_error('test', error_string='Invalid DICOM file')
-
-    def test_missing_sop_class(self):
-        filename = 'test.dcm'
-        file_dataset = FileDataset(filename, Dataset(),
-                                   file_meta=self.create_metadata())
-        write_file(filename, file_dataset, write_like_original=False)
-        self.assert_fatal_error(filename, 'Missing SOPClassUID')
-
-    def test_unknown_sop_class(self):
-        dataset = Dataset()
-        dataset.SOPClassUID = 'Unknown'
-        file_dataset = FileDataset('test', dataset,
-                                   file_meta=self.create_metadata())
-        write_file('test', file_dataset, write_like_original=False)
-        self.assert_fatal_error(
-            'test',
-            'Unknown SOPClassUID (probably retired): Unknown')
-
-    def test_validate_dir(self):
-        self.fs.create_dir(os.path.join('foo', 'bar', 'baz'))
-        self.fs.create_dir(os.path.join('foo', 'baz'))
-        self.fs.create_file(os.path.join('foo', '1.dcm'))
-        self.fs.create_file(os.path.join('foo', 'bar', '2.dcm'))
-        self.fs.create_file(os.path.join('foo', 'bar', '3.dcm'))
-        self.fs.create_file(os.path.join('foo', 'bar', 'baz', '4.dcm'))
-        self.fs.create_file(os.path.join('foo', 'baz', '5.dcm'))
-        self.fs.create_file(os.path.join('foo1', '6.dcm'))
-
-        self.assertEqual(5, len(self.validator.validate('foo')))
-
-    def test_non_fatal_errors(self):
-        dataset = Dataset()
-        dataset.SOPClassUID = '1.2.840.10008.5.1.4.1.1.2'  # CT Image Storage
-        file_dataset = FileDataset('test', dataset,
-                                   file_meta=self.create_metadata())
-        write_file('test', file_dataset, write_like_original=False)
-        error_dict = self.validator.validate('test')
-        self.assertEqual(1, len(error_dict))
-        errors = error_dict['test']
-        self.assertNotIn('fatal', errors)
-
-
-class RealDicomFileValidatorTest(DicomFileValidatorTestBase):
-
-    def test_that_pixeldata_is_read(self):
-        # regression test for #6
-        rtdose_path = os.path.join(dicom_fixture_path(), 'rtdose.dcm')
-        error_dict = self.validator.validate(rtdose_path)
-        self.assertEqual(1, len(error_dict))
-        results = error_dict[rtdose_path]
-        self.assertIn('RT Series', results)
-        self.assertIn('Tag (0008,1070) is missing', results['RT Series'])
-        # if PixelData is not read, RT Dose will show errors
-        self.assertNotIn('RT Dose', results)
+import json
+import logging
+import os
+import unittest
+
+import pyfakefs.fake_filesystem_unittest
+from pydicom import write_file
+from pydicom.dataset import Dataset, FileDataset
+
+from dicom_validator.spec_reader.edition_reader import EditionReader
+from dicom_validator.tests.test_utils import json_fixture_path, \
+    dicom_fixture_path
+from dicom_validator.validator.dicom_file_validator import DicomFileValidator
+
+
+class DicomFileValidatorTestBase(unittest.TestCase):
+    iod_info = None
+    module_info = None
+
+    @classmethod
+    def setUpClass(cls):
+        with open(os.path.join(json_fixture_path(),
+                               EditionReader.iod_info_json)) as info_file:
+            cls.iod_info = json.load(info_file)
+        with open(os.path.join(json_fixture_path(),
+                               EditionReader.module_info_json)) as info_file:
+            cls.module_info = json.load(info_file)
+
+    def setUp(self):
+        logging.disable(logging.CRITICAL)
+        self.validator = DicomFileValidator(self.iod_info, self.module_info)
+
+    def tearDown(self):
+        logging.disable(logging.DEBUG)
+
+
+class FakeDicomFileValidatorTest(DicomFileValidatorTestBase,
+                                 pyfakefs.fake_filesystem_unittest.TestCase):
+    iod_info = None
+    module_info = None
+
+    def setUp(self):
+        super(FakeDicomFileValidatorTest, self).setUp()
+        self.setUpPyfakefs()
+
+    @staticmethod
+    def create_metadata():
+        metadata = Dataset()
+        metadata.MediaStorageSOPClassUID = '1.2.840.10008.5.1.4.1.1.7'
+        metadata.MediaStorageSOPInstanceUID = '1.2.3'
+        metadata.TransferSyntaxUID = '1.2.840.10008.1.2'
+        metadata.ImplementationClassUID = '1.3.6.1.4.1.5962.2'
+        return metadata
+
+    def assert_fatal_error(self, filename, error_string):
+        error_dict = self.validator.validate(filename)
+        self.assertEqual(1, len(error_dict))
+        name = list(error_dict.keys())[0]
+        self.assertEqual(filename, name)
+        errors = error_dict[name]
+        self.assertEqual({'fatal': error_string}, errors)
+
+    def test_non_existing_file(self):
+        self.assert_fatal_error('non_existing', error_string='File missing')
+
+    def test_invalid_file(self):
+        self.fs.create_file('test', contents='invalid')
+        self.assert_fatal_error('test', error_string='Invalid DICOM file')
+
+    def test_missing_sop_class(self):
+        filename = 'test.dcm'
+        file_dataset = FileDataset(filename, Dataset(),
+                                   file_meta=self.create_metadata())
+        write_file(filename, file_dataset, write_like_original=False)
+        self.assert_fatal_error(filename, 'Missing SOPClassUID')
+
+    def test_unknown_sop_class(self):
+        dataset = Dataset()
+        dataset.SOPClassUID = 'Unknown'
+        file_dataset = FileDataset('test', dataset,
+                                   file_meta=self.create_metadata())
+        write_file('test', file_dataset, write_like_original=False)
+        self.assert_fatal_error(
+            'test',
+            'Unknown SOPClassUID (probably retired): Unknown')
+
+    def test_validate_dir(self):
+        self.fs.create_dir(os.path.join('foo', 'bar', 'baz'))
+        self.fs.create_dir(os.path.join('foo', 'baz'))
+        self.fs.create_file(os.path.join('foo', '1.dcm'))
+        self.fs.create_file(os.path.join('foo', 'bar', '2.dcm'))
+        self.fs.create_file(os.path.join('foo', 'bar', '3.dcm'))
+        self.fs.create_file(os.path.join('foo', 'bar', 'baz', '4.dcm'))
+        self.fs.create_file(os.path.join('foo', 'baz', '5.dcm'))
+        self.fs.create_file(os.path.join('foo1', '6.dcm'))
+
+        self.assertEqual(5, len(self.validator.validate('foo')))
+
+    def test_non_fatal_errors(self):
+        dataset = Dataset()
+        dataset.SOPClassUID = '1.2.840.10008.5.1.4.1.1.2'  # CT Image Storage
+        file_dataset = FileDataset('test', dataset,
+                                   file_meta=self.create_metadata())
+        write_file('test', file_dataset, write_like_original=False)
+        error_dict = self.validator.validate('test')
+        self.assertEqual(1, len(error_dict))
+        errors = error_dict['test']
+        self.assertNotIn('fatal', errors)
+
+
+class RealDicomFileValidatorTest(DicomFileValidatorTestBase):
+
+    def test_that_pixeldata_is_read(self):
+        # regression test for #6
+        rtdose_path = os.path.join(dicom_fixture_path(), 'rtdose.dcm')
+        error_dict = self.validator.validate(rtdose_path)
+        self.assertEqual(1, len(error_dict))
+        results = error_dict[rtdose_path]
+        self.assertIn('RT Series', results)
+        self.assertIn('Tag (0008,1070) is missing', results['RT Series'])
+        # if PixelData is not read, RT Dose will show errors
+        self.assertNotIn('RT Dose', results)
```

### Comparing `dicom-validator-0.3.4/dicom_validator/validator/tests/test_iod_validator.py` & `dicom-validator-0.3.5/dicom_validator/validator/tests/test_iod_validator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,407 +1,410 @@
-import json
-import logging
-import os
-import unittest
-
-from dicom_validator.spec_reader.edition_reader import EditionReader
-
-from pydicom.dataset import Dataset
-
-from dicom_validator.tests.test_utils import json_fixture_path
-from dicom_validator.validator.iod_validator import IODValidator
-
-
-class IODValidatorTest(unittest.TestCase):
-    """Tests IODValidator.
-    Note: some of the fixture data are not consistent with the DICOM Standard.
-    """
-    iod_specs = None
-    module_specs = None
-
-    @classmethod
-    def setUpClass(cls):
-        with open(os.path.join(json_fixture_path(),
-                               EditionReader.iod_info_json)) as info_file:
-            cls.iod_specs = json.load(info_file)
-        with open(os.path.join(json_fixture_path(),
-                               EditionReader.module_info_json)) as info_file:
-            cls.module_specs = json.load(info_file)
-
-    def setUp(self):
-        super(IODValidatorTest, self).setUp()
-        logging.disable(logging.CRITICAL)
-
-    def validator(self, data_set):
-        return IODValidator(data_set, self.iod_specs, self.module_specs, None,
-                            logging.ERROR)
-
-    @staticmethod
-    def new_data_set(tags):
-        """ Create a DICOM data set with the given attributes """
-        tags = tags or {}
-        data_set = Dataset()
-        for tag_name, value in tags.items():
-            setattr(data_set, tag_name, value)
-        data_set.file_meta = Dataset()
-        data_set.is_implicit_VR = False
-        data_set.is_little_endian = True
-        return data_set
-
-    def test_empty_dataset(self):
-        data_set = self.new_data_set(tags={})
-        validator = self.validator(data_set)
-        result = validator.validate()
-        self.assertIn('fatal', result)
-
-    def test_invalid_sop_class_id(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.3'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-        self.assertIn('fatal', result)
-
-    @staticmethod
-    def has_tag_error(messages, module_name, tag_id_string, error_kind):
-        if module_name not in messages:
-            return False
-        for message in messages[module_name]:
-            if message.startswith(
-                    'Tag {} is {}'.format(tag_id_string, error_kind)):
-                return True
-        return False
-
-    def test_missing_tags(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.2',  # CT
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertNotIn('fatal', result)
-        self.assertIn('CT Image', result)
-
-        # PatientName is set
-        self.assertFalse(
-            self.has_tag_error(result, 'Patient', '(0010,0010)', 'missing'))
-        # PatientSex - type 2, missing
-        self.assertTrue(
-            self.has_tag_error(result, 'Patient', '(0010,0040)', 'missing'))
-        # Clinical Trial Sponsor Name -> type 1, but module usage U
-        self.assertFalse(
-            self.has_tag_error(result, 'Patient', '(0012,0010)', 'missing'))
-        # Patient Breed Description -> type 2C, but no parsable condition
-        self.assertFalse(
-            self.has_tag_error(result, 'Patient', '(0010,2292)', 'missing'))
-
-    def test_empty_tags(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.2',  # CT
-            'PatientName': '',
-            'Modality': None
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertNotIn('fatal', result)
-        self.assertIn('CT Image', result)
-        # Modality - type 1, present but empty
-        self.assertTrue(
-            self.has_tag_error(result, 'Patient', '(0010,0040)', 'missing'))
-        # PatientName - type 2, empty tag is allowed
-        self.assertFalse(
-            self.has_tag_error(result, 'Patient', '(0010,0010)', 'missing'))
-
-    def test_fulfilled_condition_existing_tag(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'CArmPositionerTabletopRelationship': 'YES',
-            'SynchronizationTrigger': 'SET',
-            'FrameOfReferenceUID': '1.2.3.4.5.6.7.8',
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        # Frame Of Reference UID Is and Synchronization Trigger set
-        self.assertFalse(
-            self.has_tag_error(result, 'Enhanced X-Ray Angiographic Image',
-                               '(0020,0052)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Synchronization',
-                                            '(0018,106A)', 'missing'))
-
-    def test_fulfilled_condition_missing_tag(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'CArmPositionerTabletopRelationship': 'YES',
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(result, 'Frame of Reference',
-                                           '(0020,0052)', 'missing'))
-        self.assertTrue(self.has_tag_error(result, 'Synchronization',
-                                           '(0018,106A)', 'missing'))
-
-    def test_condition_not_met_no_tag(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
-                                            '(0020,0052)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
-                                            '(0020,0052)', 'not allowed'))
-
-    def test_condition_not_met_existing_tag(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'FrameOfReferenceUID': '1.2.3.4.5.6.7.8',
-            'SynchronizationTrigger': 'SET',
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        # Frame Of Reference is allowed, Synchronization Trigger not
-        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
-                                            '(0020,0052)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
-                                            '(0020,0052)', 'not allowed'))
-        self.assertTrue(self.has_tag_error(result, 'Synchronization',
-                                           '(0018,106A)', 'not allowed'))
-
-    def test_and_condition_not_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'SECONDARY',
-            'CardiacSynchronizationTechnique': 'OTHER',
-            'HighRRValue': '123'  # 0018,1082
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        # Both Low R-R Value and High R-R Value are not needed but allowed
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1081)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1082)', 'missing'))
-
-    def test_only_one_and_condition_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'PRIMARY',
-            'CardiacSynchronizationTechnique': 'OTHER',
-            'HighRRValue': '123'  # 0018,1082
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        # Both Low R-R Value and High R-R Value are not needed but allowed
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1081)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1082)', 'missing'))
-
-    def test_and_condition_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'MIXED',
-            'CardiacSynchronizationTechnique': 'PROSPECTIVE',
-            'HighRRValue': '123'  # 0018,1082
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        # Both Low R-R Value and High R-R Value are needed
-        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
-                                           '(0018,1081)', 'missing'))
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1082)', 'missing'))
-
-    def test_presence_condition_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'PixelPaddingRangeLimit': '10',
-            'PixelDataProviderURL': 'https://dataprovider'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(result, 'General Equipment',
-                                           '(0028,0120)',
-                                           'missing'))  # Pixel Padding Value
-
-    def test_presence_condition_not_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'PixelPaddingRangeLimit': '10',
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(result, 'General Equipment',
-                                            '(0028,0120)',
-                                            'missing'))  # Pixel Padding Value
-
-    def test_greater_condition_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'SamplesPerPixel': 3
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(result, 'Image Pixel',
-                                           '(0028,0006)',
-                                           'missing'))  # Planar configuration
-
-    def test_greater_condition_not_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'SamplesPerPixel': 1
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(result, 'Image Pixel',
-                                            '(0028,0006)',
-                                            'missing'))  # Planar configuration
-
-    def test_points_to_condition_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'FrameIncrementPointer': 0x00181065
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
-                                           '(0018,1086)',
-                                           'missing'))  # Skip beats
-
-    def test_points_to_condition_not_met(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'FrameIncrementPointer': 0x00181055
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
-                                            '(0018,1086)',
-                                            'missing'))  # Skip beats
-
-    def test_condition_for_not_required_tag_cond1_fulfilled(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'ORIGINAL',
-            'CardiacSynchronizationTechnique': 'ANY'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
-                                           '(0018,9085)',
-                                           'missing'))  # Cardiac signal source
-
-    def test_condition_for_not_required_tag_no_cond_fulfilled(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'ORIGINAL',
-            'CardiacSynchronizationTechnique': 'NONE',
-            'CardiacSignalSource': 'ECG'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertTrue(self.has_tag_error(
-            result, 'Cardiac Synchronization',
-            '(0018,9085)',
-            'not allowed'))  # Cardiac signal source
-
-    def test_condition_for_not_required_tag_cond2_fulfilled_present(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'DERIVED',
-            'CardiacSynchronizationTechnique': 'ANY',
-            'CardiacSignalSource': 'ECG'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(
-            result, 'Cardiac Synchronization',
-            '(0018,9085)',
-            'not allowed'))  # Cardiac signal source
-
-    def test_condition_for_not_required_tag_cond2_fulfilled_not_present(self):
-        data_set = self.new_data_set({
-            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
-            # Enhanced X-Ray Angiographic Image
-            'PatientName': 'XXX',
-            'PatientID': 'ZZZ',
-            'ImageType': 'DERIVED',
-            'CardiacSynchronizationTechnique': 'ANY'
-        })
-        validator = self.validator(data_set)
-        result = validator.validate()
-
-        self.assertFalse(self.has_tag_error(
-            result, 'Cardiac Synchronization',
-            '(0018,9085)',
-            'missing'))  # Cardiac signal source
-
-
-if __name__ == '__main__':
-    unittest.main()
+import json
+import logging
+import os
+import unittest
+
+from dicom_validator.spec_reader.edition_reader import EditionReader
+
+from pydicom.dataset import Dataset
+
+from dicom_validator.tests.test_utils import json_fixture_path
+from dicom_validator.validator.iod_validator import IODValidator
+
+
+class IODValidatorTest(unittest.TestCase):
+    """Tests IODValidator.
+    Note: some of the fixture data are not consistent with the DICOM Standard.
+    """
+    iod_specs = None
+    module_specs = None
+
+    @classmethod
+    def setUpClass(cls):
+        with open(os.path.join(json_fixture_path(),
+                               EditionReader.iod_info_json)) as info_file:
+            cls.iod_specs = json.load(info_file)
+        with open(os.path.join(json_fixture_path(),
+                               EditionReader.module_info_json)) as info_file:
+            cls.module_specs = json.load(info_file)
+
+    def setUp(self):
+        super(IODValidatorTest, self).setUp()
+        logging.disable(logging.CRITICAL)
+
+    def tearDown(self):
+        logging.disable(logging.DEBUG)
+
+    def validator(self, data_set):
+        return IODValidator(data_set, self.iod_specs, self.module_specs, None,
+                            logging.ERROR)
+
+    @staticmethod
+    def new_data_set(tags):
+        """ Create a DICOM data set with the given attributes """
+        tags = tags or {}
+        data_set = Dataset()
+        for tag_name, value in tags.items():
+            setattr(data_set, tag_name, value)
+        data_set.file_meta = Dataset()
+        data_set.is_implicit_VR = False
+        data_set.is_little_endian = True
+        return data_set
+
+    def test_empty_dataset(self):
+        data_set = self.new_data_set(tags={})
+        validator = self.validator(data_set)
+        result = validator.validate()
+        self.assertIn('fatal', result)
+
+    def test_invalid_sop_class_id(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.3'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+        self.assertIn('fatal', result)
+
+    @staticmethod
+    def has_tag_error(messages, module_name, tag_id_string, error_kind):
+        if module_name not in messages:
+            return False
+        for message in messages[module_name]:
+            if message.startswith(
+                    'Tag {} is {}'.format(tag_id_string, error_kind)):
+                return True
+        return False
+
+    def test_missing_tags(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.2',  # CT
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertNotIn('fatal', result)
+        self.assertIn('CT Image', result)
+
+        # PatientName is set
+        self.assertFalse(
+            self.has_tag_error(result, 'Patient', '(0010,0010)', 'missing'))
+        # PatientSex - type 2, missing
+        self.assertTrue(
+            self.has_tag_error(result, 'Patient', '(0010,0040)', 'missing'))
+        # Clinical Trial Sponsor Name -> type 1, but module usage U
+        self.assertFalse(
+            self.has_tag_error(result, 'Patient', '(0012,0010)', 'missing'))
+        # Patient Breed Description -> type 2C, but no parsable condition
+        self.assertFalse(
+            self.has_tag_error(result, 'Patient', '(0010,2292)', 'missing'))
+
+    def test_empty_tags(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.2',  # CT
+            'PatientName': '',
+            'Modality': None
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertNotIn('fatal', result)
+        self.assertIn('CT Image', result)
+        # Modality - type 1, present but empty
+        self.assertTrue(
+            self.has_tag_error(result, 'Patient', '(0010,0040)', 'missing'))
+        # PatientName - type 2, empty tag is allowed
+        self.assertFalse(
+            self.has_tag_error(result, 'Patient', '(0010,0010)', 'missing'))
+
+    def test_fulfilled_condition_existing_tag(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'CArmPositionerTabletopRelationship': 'YES',
+            'SynchronizationTrigger': 'SET',
+            'FrameOfReferenceUID': '1.2.3.4.5.6.7.8',
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        # Frame Of Reference UID Is and Synchronization Trigger set
+        self.assertFalse(
+            self.has_tag_error(result, 'Enhanced X-Ray Angiographic Image',
+                               '(0020,0052)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Synchronization',
+                                            '(0018,106A)', 'missing'))
+
+    def test_fulfilled_condition_missing_tag(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'CArmPositionerTabletopRelationship': 'YES',
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(result, 'Frame of Reference',
+                                           '(0020,0052)', 'missing'))
+        self.assertTrue(self.has_tag_error(result, 'Synchronization',
+                                           '(0018,106A)', 'missing'))
+
+    def test_condition_not_met_no_tag(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
+                                            '(0020,0052)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
+                                            '(0020,0052)', 'not allowed'))
+
+    def test_condition_not_met_existing_tag(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'FrameOfReferenceUID': '1.2.3.4.5.6.7.8',
+            'SynchronizationTrigger': 'SET',
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        # Frame Of Reference is allowed, Synchronization Trigger not
+        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
+                                            '(0020,0052)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Frame of Reference',
+                                            '(0020,0052)', 'not allowed'))
+        self.assertTrue(self.has_tag_error(result, 'Synchronization',
+                                           '(0018,106A)', 'not allowed'))
+
+    def test_and_condition_not_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'SECONDARY',
+            'CardiacSynchronizationTechnique': 'OTHER',
+            'HighRRValue': '123'  # 0018,1082
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        # Both Low R-R Value and High R-R Value are not needed but allowed
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1081)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1082)', 'missing'))
+
+    def test_only_one_and_condition_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'PRIMARY',
+            'CardiacSynchronizationTechnique': 'OTHER',
+            'HighRRValue': '123'  # 0018,1082
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        # Both Low R-R Value and High R-R Value are not needed but allowed
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1081)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1082)', 'missing'))
+
+    def test_and_condition_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'MIXED',
+            'CardiacSynchronizationTechnique': 'PROSPECTIVE',
+            'HighRRValue': '123'  # 0018,1082
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        # Both Low R-R Value and High R-R Value are needed
+        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
+                                           '(0018,1081)', 'missing'))
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1082)', 'missing'))
+
+    def test_presence_condition_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'PixelPaddingRangeLimit': '10',
+            'PixelDataProviderURL': 'https://dataprovider'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(result, 'General Equipment',
+                                           '(0028,0120)',
+                                           'missing'))  # Pixel Padding Value
+
+    def test_presence_condition_not_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'PixelPaddingRangeLimit': '10',
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(result, 'General Equipment',
+                                            '(0028,0120)',
+                                            'missing'))  # Pixel Padding Value
+
+    def test_greater_condition_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'SamplesPerPixel': 3
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(result, 'Image Pixel',
+                                           '(0028,0006)',
+                                           'missing'))  # Planar configuration
+
+    def test_greater_condition_not_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'SamplesPerPixel': 1
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(result, 'Image Pixel',
+                                            '(0028,0006)',
+                                            'missing'))  # Planar configuration
+
+    def test_points_to_condition_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'FrameIncrementPointer': 0x00181065
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
+                                           '(0018,1086)',
+                                           'missing'))  # Skip beats
+
+    def test_points_to_condition_not_met(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'FrameIncrementPointer': 0x00181055
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(result, 'Cardiac Synchronization',
+                                            '(0018,1086)',
+                                            'missing'))  # Skip beats
+
+    def test_condition_for_not_required_tag_cond1_fulfilled(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'ORIGINAL',
+            'CardiacSynchronizationTechnique': 'ANY'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(result, 'Cardiac Synchronization',
+                                           '(0018,9085)',
+                                           'missing'))  # Cardiac signal source
+
+    def test_condition_for_not_required_tag_no_cond_fulfilled(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'ORIGINAL',
+            'CardiacSynchronizationTechnique': 'NONE',
+            'CardiacSignalSource': 'ECG'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertTrue(self.has_tag_error(
+            result, 'Cardiac Synchronization',
+            '(0018,9085)',
+            'not allowed'))  # Cardiac signal source
+
+    def test_condition_for_not_required_tag_cond2_fulfilled_present(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'DERIVED',
+            'CardiacSynchronizationTechnique': 'ANY',
+            'CardiacSignalSource': 'ECG'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(
+            result, 'Cardiac Synchronization',
+            '(0018,9085)',
+            'not allowed'))  # Cardiac signal source
+
+    def test_condition_for_not_required_tag_cond2_fulfilled_not_present(self):
+        data_set = self.new_data_set({
+            'SOPClassUID': '1.2.840.10008.5.1.4.1.1.12.1.1',
+            # Enhanced X-Ray Angiographic Image
+            'PatientName': 'XXX',
+            'PatientID': 'ZZZ',
+            'ImageType': 'DERIVED',
+            'CardiacSynchronizationTechnique': 'ANY'
+        })
+        validator = self.validator(data_set)
+        result = validator.validate()
+
+        self.assertFalse(self.has_tag_error(
+            result, 'Cardiac Synchronization',
+            '(0018,9085)',
+            'missing'))  # Cardiac signal source
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `dicom-validator-0.3.4/dicom_validator.egg-info/PKG-INFO` & `dicom-validator-0.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,193 @@
-Metadata-Version: 2.1
-Name: dicom-validator
-Version: 0.3.4
-Summary: Python DICOM tools using input from DICOM specs in docbook format
-Home-page: http://github.com/pydicom/dicom-validator
-Author: mrbean-bremen
-Author-email: hansemrbean@googlemail.com
-License: UNKNOWN
-Description: # dicom-validator
-        
-        [![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Python%20package/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
-        
-        *dicom-validator* provides the command line tool `validate_iods` that 
-        checks a DICOM file for missing or unexpected attributes. The check is done by
-        comparing the contents of the DICOM file against the modules and 
-        attributes required by the DICOM standard for the SOP class of the given  
-        dataset.
-        
-        The tool gets its input from the newest version of the DICOM standard (or a 
-        specific version given as command line parameter) as provided by
-        [ACR NEMA](http://medical.nema.org/) in docbook format.
-        [pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
-        the DICOM files. 
-        
-        Additionally, the command line tool `dump_dcm_info` is available that displays 
-        the tag values of one or several DICOM files in a readable format. It is
-        provided as a proof of concept of getting information directly from the
-        DICOM standard.
-        
-        *Disclaimer:*  
-        No guarantees are given for the correctness of the results.
-        This is alpha-stage software and mostly thought as a proof of concept.
-        Also check the limitations for `validate_iods` described below.
-        
-        *Note:*
-        The original name of the package (`dcm-spec-tools`) has been 
-        changed to `dicom-validator` together with the move to the `pydicom` 
-        organization to reflect the fact that no other tools are planned, and that the 
-        DICOM validator is the relevant tool.
-        
-        
-        ## Installation
-        
-        The latest version is available on pypi and can be installed via
-        ```
-        pip install dicom-validator
-        ```
-        
-        ## Usage
-        ```
-        dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
-        validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
-        ```
-        Use the `--help` option for each script do get usage info.
-        
-        ## Access to the DICOM standard
-        
-        Upon first start of a tool, part of the latest version of the DICOM standard
-        in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
-        parsed, and the needed information saved in json files. If the `--src` 
-        parameter is not provided, the files are downloaded to and looked up in
-        `<user home>/dicom-validator/`.    
-        These files are then used by the tools. Periodically (once a month), the tools
-        check for a newer version of the DICOM standard and download it if found.
-        
-        It is also possible to use older versions of the standard via the command line 
-        option `--revision` or `-r`, provided they are available for download 
-        (at the time of writing, standards are available since revision 2014a). A 
-        list of currently available editions can be found in
-        *<user home>/dicom-validator/editions.json* after a tool has been called 
-        the first time.
-        
-        ## validate_iods
-        
-        This checks a given DICOM file, or all DICOM files recursively in a given
-        directory, for correct tags for the related SOP class. Only the presence or  
-        absence of the tag, and the presence of a tag value is checked, not the
-        contained value itself (a check for correct enumerated values may be added later).
-        This is done by looking up all required and optional modules for this
-        SOP class, and checking the tags for these modules. Tags that are not allowed or
-        missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
-        to collect the needed information.
-        Conditions for type 1C and 2C modules and tags are evaluated if possible.
-        If the evaluation fails, the respective modules and tags are considered
-        optional. 
-        
-        The output for a single file may look like this:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
-        
-        Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
-        SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
-        
-        Errors
-        ======
-        Module "SR Document Content":
-        Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
-          Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
-        Tag (0040,A300) (Measured Value Sequence) is missing
-        Tag (0040,A168) (Concept Code Sequence) is missing
-        Tag (0008,1199) (Referenced SOP Sequence) is missing
-        Tag (0070,0022) (Graphic Data) is missing
-        Tag (0070,0023) (Graphic Type) is missing
-        Tag (3006,0024) (Referenced Frame of Reference UID) is missing
-        Tag (0040,A130) (Temporal Range Type) is missing
-        Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
-          Referenced Sample Positions is not present and Referenced DateTime is not present
-        Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
-          Referenced Sample Positions is not present and Referenced Time Offsets is not present
-        ```
-        
-        ### Limitations
-        
-        #### Condition evaluation
-        As mentioned, if the evaluation of conditions fails, the related module or 
-        tag is considered optional, which may hide some non-conformity.  
-        Condition evaluation may fail if:
-        - the needed information is not contained in the DICOM file (e.g. verbose
-          descriptions like "if the Patient is an animal")
-        - the information is related to other DICOM files (e.g. referenced images)
-        - the parsing failed because the condition is too complicated, unexpected,
-          or due to a bug (please write an issue if you encounter such a problem)
-          
-        #### Retired tags 
-        Also note that only the given standard is used to evaluate the files. If 
-        the DICOM file has been written using an older standard, it may conform to 
-        that standard, but not to the newest one. Tags that are retired in the 
-        version of the standard used for parsing are not considered at all.
-        
-        #### Unsupported cases (support may be added in future versions)
-        - SOP classes not in the table in PS3.3 such as Presentation States are not 
-          handled
-        - functional groups in EnhancedXXX SOP classes are not handled
-        
-        
-        ## dcm_dump_info
-        
-        This is a very simple DICOM dump tool, which uses 
-        the DICOM dictionary as read from part 6 of the standard. It prints the 
-        DICOM header of the given DICOM file, or of all DICOM files recursively in a 
-        given directory. The output looks like this:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
-        Data\SR\image12.dcm"
-        
-        c:\dev\DICOM Data\SR\image12.dcm
-        (0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-        (0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
-        (0008,0008) Image Type                               CS    0  []
-        (0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
-        (0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
-        (0008,0020) Study Date                               DA    1  [19950119]
-        (0008,0030) Study Time                               TM    1  [092854.0]
-        (0008,0050) Accession Number                         SH    1  [ACN000001]
-        (0008,0060) Modality                                 CS    1  [US]
-        (0008,0070) Manufacturer                             LO    1  [Acuson]
-        (0008,0090) Referring Physician's Name               PN    1  []
-        (0008,1010) Station Name                             SH    1  [QV-00775]
-        (0008,1030) Study Description                        LO    1  [ABDOMEN]
-        (0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
-        (0008,1060) Name of Physician(s) Reading Study       PN    1  []
-        (0008,1070) Operators' Name                          PN    1  [DO]
-        (0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
-        (0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-        ...
-        ```
-        
-        If you want to show only specific tags, you can use the option `--show-tags`:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
-        
-        c:\dev\DICOM Data\SR\image12.dcm
-        (0010,0010) Patient's Name                           PN    1  [DOE^JANE]
-        (0010,0020) Patient ID                               LO    1  [ACN000001]
-        ```
-        
-Keywords: dicom python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: dicom-validator
+Version: 0.3.5
+Summary: Python DICOM tools using input from DICOM specs in docbook format
+Home-page: https://github.com/pydicom/dicom-validator
+Author: mrbean-bremen
+Author-email: hansemrbean@googlemail.com
+Keywords: dicom python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dicom-validator
+
+[![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Testsuite/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
+
+*dicom-validator* provides the command line tool `validate_iods` that 
+checks a DICOM file for missing or unexpected attributes. The check is done by
+comparing the contents of the DICOM file against the modules and 
+attributes required by the DICOM standard for the SOP class of the given  
+dataset.
+
+The tool gets its input from the newest version of the DICOM standard (or a 
+specific version given as command line parameter) as provided by
+[ACR NEMA](http://medical.nema.org/) in docbook format.
+[pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
+the DICOM files. 
+
+Additionally, the command line tool `dump_dcm_info` is available that displays 
+the tag values of one or several DICOM files in a readable format. It is
+provided as a proof of concept of getting information directly from the
+DICOM standard.
+
+*Disclaimer:*  
+No guarantees are given for the correctness of the results.
+This is alpha-stage software and mostly thought as a proof of concept.
+Also check the limitations for `validate_iods` described below.
+
+*Note:*
+The original name of the package (`dcm-spec-tools`) has been 
+changed to `dicom-validator` together with the move to the `pydicom` 
+organization to reflect the fact that no other tools are planned, and that the 
+DICOM validator is the relevant tool.
+
+
+## Installation
+
+The latest version is available on pypi and can be installed via
+```
+pip install dicom-validator
+```
+
+## Usage
+```
+dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
+validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
+```
+Use the `--help` option for each script do get usage info.
+
+## Access to the DICOM standard
+
+Upon first start of a tool, part of the latest version of the DICOM standard
+in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
+parsed, and the needed information saved in json files. If the `--src` 
+parameter is not provided, the files are downloaded to and looked up in
+`<user home>/dicom-validator/`.    
+These files are then used by the tools. Periodically (once a month), the tools
+check for a newer version of the DICOM standard and download it if found.
+
+It is also possible to use older versions of the standard via the command line 
+option `--revision` or `-r`, provided they are available for download 
+(at the time of writing, standards are available since revision 2014a). A 
+list of currently available editions can be found in
+*<user home>/dicom-validator/editions.json* after a tool has been called 
+the first time.
+
+## validate_iods
+
+This checks a given DICOM file, or all DICOM files recursively in a given
+directory, for correct tags for the related SOP class. Only the presence or  
+absence of the tag, and the presence of a tag value is checked, not the
+contained value itself (a check for correct enumerated values may be added later).
+This is done by looking up all required and optional modules for this
+SOP class, and checking the tags for these modules. Tags that are not allowed or
+missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
+to collect the needed information.
+Conditions for type 1C and 2C modules and tags are evaluated if possible.
+If the evaluation fails, the respective modules and tags are considered
+optional. 
+
+The output for a single file may look like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
+
+Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
+SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
+
+Errors
+======
+Module "SR Document Content":
+Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
+  Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
+Tag (0040,A300) (Measured Value Sequence) is missing
+Tag (0040,A168) (Concept Code Sequence) is missing
+Tag (0008,1199) (Referenced SOP Sequence) is missing
+Tag (0070,0022) (Graphic Data) is missing
+Tag (0070,0023) (Graphic Type) is missing
+Tag (3006,0024) (Referenced Frame of Reference UID) is missing
+Tag (0040,A130) (Temporal Range Type) is missing
+Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced DateTime is not present
+Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced Time Offsets is not present
+```
+
+### Limitations
+
+#### Condition evaluation
+As mentioned, if the evaluation of conditions fails, the related module or 
+tag is considered optional, which may hide some non-conformity.  
+Condition evaluation may fail if:
+- the needed information is not contained in the DICOM file (e.g. verbose
+  descriptions like "if the Patient is an animal")
+- the information is related to other DICOM files (e.g. referenced images)
+- the parsing failed because the condition is too complicated, unexpected,
+  or due to a bug (please write an issue if you encounter such a problem)
+  
+#### Retired tags 
+Also note that only the given standard is used to evaluate the files. If 
+the DICOM file has been written using an older standard, it may conform to 
+that standard, but not to the newest one. Tags that are retired in the 
+version of the standard used for parsing are not considered at all.
+
+#### Unsupported cases (support may be added in future versions)
+- SOP classes not in the table in PS3.3 such as Presentation States are not 
+  handled
+- functional groups in EnhancedXXX SOP classes are not handled
+
+
+## dump_dcm_info
+
+This is a very simple DICOM dump tool, which uses 
+the DICOM dictionary as read from part 6 of the standard. It prints the 
+DICOM header of the given DICOM file, or of all DICOM files recursively in a 
+given directory. The output looks like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
+Data\SR\image12.dcm"
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+(0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
+(0008,0008) Image Type                               CS    0  []
+(0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
+(0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
+(0008,0020) Study Date                               DA    1  [19950119]
+(0008,0030) Study Time                               TM    1  [092854.0]
+(0008,0050) Accession Number                         SH    1  [ACN000001]
+(0008,0060) Modality                                 CS    1  [US]
+(0008,0070) Manufacturer                             LO    1  [Acuson]
+(0008,0090) Referring Physician's Name               PN    1  []
+(0008,1010) Station Name                             SH    1  [QV-00775]
+(0008,1030) Study Description                        LO    1  [ABDOMEN]
+(0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
+(0008,1060) Name of Physician(s) Reading Study       PN    1  []
+(0008,1070) Operators' Name                          PN    1  [DO]
+(0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
+(0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+...
+```
+
+If you want to show only specific tags, you can use the option `--show-tags`:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0010,0010) Patient's Name                           PN    1  [DOE^JANE]
+(0010,0020) Patient ID                               LO    1  [ACN000001]
+```
```

### Comparing `dicom-validator-0.3.4/dicom_validator.egg-info/SOURCES.txt` & `dicom-validator-0.3.5/dicom_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.3.4/LICENSE` & `dicom-validator-0.3.5/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2016 
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2016 
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dicom-validator-0.3.4/PKG-INFO` & `dicom-validator-0.3.5/dicom_validator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,193 @@
-Metadata-Version: 2.1
-Name: dicom-validator
-Version: 0.3.4
-Summary: Python DICOM tools using input from DICOM specs in docbook format
-Home-page: http://github.com/pydicom/dicom-validator
-Author: mrbean-bremen
-Author-email: hansemrbean@googlemail.com
-License: UNKNOWN
-Description: # dicom-validator
-        
-        [![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Python%20package/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
-        
-        *dicom-validator* provides the command line tool `validate_iods` that 
-        checks a DICOM file for missing or unexpected attributes. The check is done by
-        comparing the contents of the DICOM file against the modules and 
-        attributes required by the DICOM standard for the SOP class of the given  
-        dataset.
-        
-        The tool gets its input from the newest version of the DICOM standard (or a 
-        specific version given as command line parameter) as provided by
-        [ACR NEMA](http://medical.nema.org/) in docbook format.
-        [pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
-        the DICOM files. 
-        
-        Additionally, the command line tool `dump_dcm_info` is available that displays 
-        the tag values of one or several DICOM files in a readable format. It is
-        provided as a proof of concept of getting information directly from the
-        DICOM standard.
-        
-        *Disclaimer:*  
-        No guarantees are given for the correctness of the results.
-        This is alpha-stage software and mostly thought as a proof of concept.
-        Also check the limitations for `validate_iods` described below.
-        
-        *Note:*
-        The original name of the package (`dcm-spec-tools`) has been 
-        changed to `dicom-validator` together with the move to the `pydicom` 
-        organization to reflect the fact that no other tools are planned, and that the 
-        DICOM validator is the relevant tool.
-        
-        
-        ## Installation
-        
-        The latest version is available on pypi and can be installed via
-        ```
-        pip install dicom-validator
-        ```
-        
-        ## Usage
-        ```
-        dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
-        validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
-        ```
-        Use the `--help` option for each script do get usage info.
-        
-        ## Access to the DICOM standard
-        
-        Upon first start of a tool, part of the latest version of the DICOM standard
-        in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
-        parsed, and the needed information saved in json files. If the `--src` 
-        parameter is not provided, the files are downloaded to and looked up in
-        `<user home>/dicom-validator/`.    
-        These files are then used by the tools. Periodically (once a month), the tools
-        check for a newer version of the DICOM standard and download it if found.
-        
-        It is also possible to use older versions of the standard via the command line 
-        option `--revision` or `-r`, provided they are available for download 
-        (at the time of writing, standards are available since revision 2014a). A 
-        list of currently available editions can be found in
-        *<user home>/dicom-validator/editions.json* after a tool has been called 
-        the first time.
-        
-        ## validate_iods
-        
-        This checks a given DICOM file, or all DICOM files recursively in a given
-        directory, for correct tags for the related SOP class. Only the presence or  
-        absence of the tag, and the presence of a tag value is checked, not the
-        contained value itself (a check for correct enumerated values may be added later).
-        This is done by looking up all required and optional modules for this
-        SOP class, and checking the tags for these modules. Tags that are not allowed or
-        missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
-        to collect the needed information.
-        Conditions for type 1C and 2C modules and tags are evaluated if possible.
-        If the evaluation fails, the respective modules and tags are considered
-        optional. 
-        
-        The output for a single file may look like this:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
-        
-        Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
-        SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
-        
-        Errors
-        ======
-        Module "SR Document Content":
-        Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
-          Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
-        Tag (0040,A300) (Measured Value Sequence) is missing
-        Tag (0040,A168) (Concept Code Sequence) is missing
-        Tag (0008,1199) (Referenced SOP Sequence) is missing
-        Tag (0070,0022) (Graphic Data) is missing
-        Tag (0070,0023) (Graphic Type) is missing
-        Tag (3006,0024) (Referenced Frame of Reference UID) is missing
-        Tag (0040,A130) (Temporal Range Type) is missing
-        Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
-          Referenced Sample Positions is not present and Referenced DateTime is not present
-        Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
-          Referenced Sample Positions is not present and Referenced Time Offsets is not present
-        ```
-        
-        ### Limitations
-        
-        #### Condition evaluation
-        As mentioned, if the evaluation of conditions fails, the related module or 
-        tag is considered optional, which may hide some non-conformity.  
-        Condition evaluation may fail if:
-        - the needed information is not contained in the DICOM file (e.g. verbose
-          descriptions like "if the Patient is an animal")
-        - the information is related to other DICOM files (e.g. referenced images)
-        - the parsing failed because the condition is too complicated, unexpected,
-          or due to a bug (please write an issue if you encounter such a problem)
-          
-        #### Retired tags 
-        Also note that only the given standard is used to evaluate the files. If 
-        the DICOM file has been written using an older standard, it may conform to 
-        that standard, but not to the newest one. Tags that are retired in the 
-        version of the standard used for parsing are not considered at all.
-        
-        #### Unsupported cases (support may be added in future versions)
-        - SOP classes not in the table in PS3.3 such as Presentation States are not 
-          handled
-        - functional groups in EnhancedXXX SOP classes are not handled
-        
-        
-        ## dcm_dump_info
-        
-        This is a very simple DICOM dump tool, which uses 
-        the DICOM dictionary as read from part 6 of the standard. It prints the 
-        DICOM header of the given DICOM file, or of all DICOM files recursively in a 
-        given directory. The output looks like this:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
-        Data\SR\image12.dcm"
-        
-        c:\dev\DICOM Data\SR\image12.dcm
-        (0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-        (0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
-        (0008,0008) Image Type                               CS    0  []
-        (0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
-        (0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
-        (0008,0020) Study Date                               DA    1  [19950119]
-        (0008,0030) Study Time                               TM    1  [092854.0]
-        (0008,0050) Accession Number                         SH    1  [ACN000001]
-        (0008,0060) Modality                                 CS    1  [US]
-        (0008,0070) Manufacturer                             LO    1  [Acuson]
-        (0008,0090) Referring Physician's Name               PN    1  []
-        (0008,1010) Station Name                             SH    1  [QV-00775]
-        (0008,1030) Study Description                        LO    1  [ABDOMEN]
-        (0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
-        (0008,1060) Name of Physician(s) Reading Study       PN    1  []
-        (0008,1070) Operators' Name                          PN    1  [DO]
-        (0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
-        (0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-        ...
-        ```
-        
-        If you want to show only specific tags, you can use the option `--show-tags`:
-        ```
-        (py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
-        
-        c:\dev\DICOM Data\SR\image12.dcm
-        (0010,0010) Patient's Name                           PN    1  [DOE^JANE]
-        (0010,0020) Patient ID                               LO    1  [ACN000001]
-        ```
-        
-Keywords: dicom python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: dicom-validator
+Version: 0.3.5
+Summary: Python DICOM tools using input from DICOM specs in docbook format
+Home-page: https://github.com/pydicom/dicom-validator
+Author: mrbean-bremen
+Author-email: hansemrbean@googlemail.com
+Keywords: dicom python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# dicom-validator
+
+[![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Testsuite/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
+
+*dicom-validator* provides the command line tool `validate_iods` that 
+checks a DICOM file for missing or unexpected attributes. The check is done by
+comparing the contents of the DICOM file against the modules and 
+attributes required by the DICOM standard for the SOP class of the given  
+dataset.
+
+The tool gets its input from the newest version of the DICOM standard (or a 
+specific version given as command line parameter) as provided by
+[ACR NEMA](http://medical.nema.org/) in docbook format.
+[pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
+the DICOM files. 
+
+Additionally, the command line tool `dump_dcm_info` is available that displays 
+the tag values of one or several DICOM files in a readable format. It is
+provided as a proof of concept of getting information directly from the
+DICOM standard.
+
+*Disclaimer:*  
+No guarantees are given for the correctness of the results.
+This is alpha-stage software and mostly thought as a proof of concept.
+Also check the limitations for `validate_iods` described below.
+
+*Note:*
+The original name of the package (`dcm-spec-tools`) has been 
+changed to `dicom-validator` together with the move to the `pydicom` 
+organization to reflect the fact that no other tools are planned, and that the 
+DICOM validator is the relevant tool.
+
+
+## Installation
+
+The latest version is available on pypi and can be installed via
+```
+pip install dicom-validator
+```
+
+## Usage
+```
+dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
+validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
+```
+Use the `--help` option for each script do get usage info.
+
+## Access to the DICOM standard
+
+Upon first start of a tool, part of the latest version of the DICOM standard
+in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
+parsed, and the needed information saved in json files. If the `--src` 
+parameter is not provided, the files are downloaded to and looked up in
+`<user home>/dicom-validator/`.    
+These files are then used by the tools. Periodically (once a month), the tools
+check for a newer version of the DICOM standard and download it if found.
+
+It is also possible to use older versions of the standard via the command line 
+option `--revision` or `-r`, provided they are available for download 
+(at the time of writing, standards are available since revision 2014a). A 
+list of currently available editions can be found in
+*<user home>/dicom-validator/editions.json* after a tool has been called 
+the first time.
+
+## validate_iods
+
+This checks a given DICOM file, or all DICOM files recursively in a given
+directory, for correct tags for the related SOP class. Only the presence or  
+absence of the tag, and the presence of a tag value is checked, not the
+contained value itself (a check for correct enumerated values may be added later).
+This is done by looking up all required and optional modules for this
+SOP class, and checking the tags for these modules. Tags that are not allowed or
+missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
+to collect the needed information.
+Conditions for type 1C and 2C modules and tags are evaluated if possible.
+If the evaluation fails, the respective modules and tags are considered
+optional. 
+
+The output for a single file may look like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
+
+Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
+SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
+
+Errors
+======
+Module "SR Document Content":
+Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
+  Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
+Tag (0040,A300) (Measured Value Sequence) is missing
+Tag (0040,A168) (Concept Code Sequence) is missing
+Tag (0008,1199) (Referenced SOP Sequence) is missing
+Tag (0070,0022) (Graphic Data) is missing
+Tag (0070,0023) (Graphic Type) is missing
+Tag (3006,0024) (Referenced Frame of Reference UID) is missing
+Tag (0040,A130) (Temporal Range Type) is missing
+Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced DateTime is not present
+Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced Time Offsets is not present
+```
+
+### Limitations
+
+#### Condition evaluation
+As mentioned, if the evaluation of conditions fails, the related module or 
+tag is considered optional, which may hide some non-conformity.  
+Condition evaluation may fail if:
+- the needed information is not contained in the DICOM file (e.g. verbose
+  descriptions like "if the Patient is an animal")
+- the information is related to other DICOM files (e.g. referenced images)
+- the parsing failed because the condition is too complicated, unexpected,
+  or due to a bug (please write an issue if you encounter such a problem)
+  
+#### Retired tags 
+Also note that only the given standard is used to evaluate the files. If 
+the DICOM file has been written using an older standard, it may conform to 
+that standard, but not to the newest one. Tags that are retired in the 
+version of the standard used for parsing are not considered at all.
+
+#### Unsupported cases (support may be added in future versions)
+- SOP classes not in the table in PS3.3 such as Presentation States are not 
+  handled
+- functional groups in EnhancedXXX SOP classes are not handled
+
+
+## dump_dcm_info
+
+This is a very simple DICOM dump tool, which uses 
+the DICOM dictionary as read from part 6 of the standard. It prints the 
+DICOM header of the given DICOM file, or of all DICOM files recursively in a 
+given directory. The output looks like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
+Data\SR\image12.dcm"
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+(0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
+(0008,0008) Image Type                               CS    0  []
+(0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
+(0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
+(0008,0020) Study Date                               DA    1  [19950119]
+(0008,0030) Study Time                               TM    1  [092854.0]
+(0008,0050) Accession Number                         SH    1  [ACN000001]
+(0008,0060) Modality                                 CS    1  [US]
+(0008,0070) Manufacturer                             LO    1  [Acuson]
+(0008,0090) Referring Physician's Name               PN    1  []
+(0008,1010) Station Name                             SH    1  [QV-00775]
+(0008,1030) Study Description                        LO    1  [ABDOMEN]
+(0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
+(0008,1060) Name of Physician(s) Reading Study       PN    1  []
+(0008,1070) Operators' Name                          PN    1  [DO]
+(0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
+(0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+...
+```
+
+If you want to show only specific tags, you can use the option `--show-tags`:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0010,0010) Patient's Name                           PN    1  [DOE^JANE]
+(0010,0020) Patient ID                               LO    1  [ACN000001]
+```
```

### Comparing `dicom-validator-0.3.4/README.md` & `dicom-validator-0.3.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-# dicom-validator
-
-[![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Python%20package/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
-
-*dicom-validator* provides the command line tool `validate_iods` that 
-checks a DICOM file for missing or unexpected attributes. The check is done by
-comparing the contents of the DICOM file against the modules and 
-attributes required by the DICOM standard for the SOP class of the given  
-dataset.
-
-The tool gets its input from the newest version of the DICOM standard (or a 
-specific version given as command line parameter) as provided by
-[ACR NEMA](http://medical.nema.org/) in docbook format.
-[pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
-the DICOM files. 
-
-Additionally, the command line tool `dump_dcm_info` is available that displays 
-the tag values of one or several DICOM files in a readable format. It is
-provided as a proof of concept of getting information directly from the
-DICOM standard.
-
-*Disclaimer:*  
-No guarantees are given for the correctness of the results.
-This is alpha-stage software and mostly thought as a proof of concept.
-Also check the limitations for `validate_iods` described below.
-
-*Note:*
-The original name of the package (`dcm-spec-tools`) has been 
-changed to `dicom-validator` together with the move to the `pydicom` 
-organization to reflect the fact that no other tools are planned, and that the 
-DICOM validator is the relevant tool.
-
-
-## Installation
-
-The latest version is available on pypi and can be installed via
-```
-pip install dicom-validator
-```
-
-## Usage
-```
-dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
-validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
-```
-Use the `--help` option for each script do get usage info.
-
-## Access to the DICOM standard
-
-Upon first start of a tool, part of the latest version of the DICOM standard
-in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
-parsed, and the needed information saved in json files. If the `--src` 
-parameter is not provided, the files are downloaded to and looked up in
-`<user home>/dicom-validator/`.    
-These files are then used by the tools. Periodically (once a month), the tools
-check for a newer version of the DICOM standard and download it if found.
-
-It is also possible to use older versions of the standard via the command line 
-option `--revision` or `-r`, provided they are available for download 
-(at the time of writing, standards are available since revision 2014a). A 
-list of currently available editions can be found in
-*<user home>/dicom-validator/editions.json* after a tool has been called 
-the first time.
-
-## validate_iods
-
-This checks a given DICOM file, or all DICOM files recursively in a given
-directory, for correct tags for the related SOP class. Only the presence or  
-absence of the tag, and the presence of a tag value is checked, not the
-contained value itself (a check for correct enumerated values may be added later).
-This is done by looking up all required and optional modules for this
-SOP class, and checking the tags for these modules. Tags that are not allowed or
-missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
-to collect the needed information.
-Conditions for type 1C and 2C modules and tags are evaluated if possible.
-If the evaluation fails, the respective modules and tags are considered
-optional. 
-
-The output for a single file may look like this:
-```
-(py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
-
-Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
-SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
-
-Errors
-======
-Module "SR Document Content":
-Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
-  Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
-Tag (0040,A300) (Measured Value Sequence) is missing
-Tag (0040,A168) (Concept Code Sequence) is missing
-Tag (0008,1199) (Referenced SOP Sequence) is missing
-Tag (0070,0022) (Graphic Data) is missing
-Tag (0070,0023) (Graphic Type) is missing
-Tag (3006,0024) (Referenced Frame of Reference UID) is missing
-Tag (0040,A130) (Temporal Range Type) is missing
-Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
-  Referenced Sample Positions is not present and Referenced DateTime is not present
-Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
-  Referenced Sample Positions is not present and Referenced Time Offsets is not present
-```
-
-### Limitations
-
-#### Condition evaluation
-As mentioned, if the evaluation of conditions fails, the related module or 
-tag is considered optional, which may hide some non-conformity.  
-Condition evaluation may fail if:
-- the needed information is not contained in the DICOM file (e.g. verbose
-  descriptions like "if the Patient is an animal")
-- the information is related to other DICOM files (e.g. referenced images)
-- the parsing failed because the condition is too complicated, unexpected,
-  or due to a bug (please write an issue if you encounter such a problem)
-  
-#### Retired tags 
-Also note that only the given standard is used to evaluate the files. If 
-the DICOM file has been written using an older standard, it may conform to 
-that standard, but not to the newest one. Tags that are retired in the 
-version of the standard used for parsing are not considered at all.
-
-#### Unsupported cases (support may be added in future versions)
-- SOP classes not in the table in PS3.3 such as Presentation States are not 
-  handled
-- functional groups in EnhancedXXX SOP classes are not handled
-
-
-## dcm_dump_info
-
-This is a very simple DICOM dump tool, which uses 
-the DICOM dictionary as read from part 6 of the standard. It prints the 
-DICOM header of the given DICOM file, or of all DICOM files recursively in a 
-given directory. The output looks like this:
-```
-(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
-Data\SR\image12.dcm"
-
-c:\dev\DICOM Data\SR\image12.dcm
-(0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-(0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
-(0008,0008) Image Type                               CS    0  []
-(0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
-(0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
-(0008,0020) Study Date                               DA    1  [19950119]
-(0008,0030) Study Time                               TM    1  [092854.0]
-(0008,0050) Accession Number                         SH    1  [ACN000001]
-(0008,0060) Modality                                 CS    1  [US]
-(0008,0070) Manufacturer                             LO    1  [Acuson]
-(0008,0090) Referring Physician's Name               PN    1  []
-(0008,1010) Station Name                             SH    1  [QV-00775]
-(0008,1030) Study Description                        LO    1  [ABDOMEN]
-(0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
-(0008,1060) Name of Physician(s) Reading Study       PN    1  []
-(0008,1070) Operators' Name                          PN    1  [DO]
-(0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
-(0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
-...
-```
-
-If you want to show only specific tags, you can use the option `--show-tags`:
-```
-(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
-
-c:\dev\DICOM Data\SR\image12.dcm
-(0010,0010) Patient's Name                           PN    1  [DOE^JANE]
-(0010,0020) Patient ID                               LO    1  [ACN000001]
-```
+# dicom-validator
+
+[![PyPI version](https://badge.fury.io/py/dicom-validator.svg)](https://pypi.org/project/dicom-validator) [![Test Suite](https://github.com/pydicom/dicom-validator/workflows/Testsuite/badge.svg)](https://github.com/pydicom/dicom-validator/actions) [![Python version](https://img.shields.io/pypi/pyversions/dicom-validator.svg)](https://pypi.org/project/dicom-validator)
+
+*dicom-validator* provides the command line tool `validate_iods` that 
+checks a DICOM file for missing or unexpected attributes. The check is done by
+comparing the contents of the DICOM file against the modules and 
+attributes required by the DICOM standard for the SOP class of the given  
+dataset.
+
+The tool gets its input from the newest version of the DICOM standard (or a 
+specific version given as command line parameter) as provided by
+[ACR NEMA](http://medical.nema.org/) in docbook format.
+[pydicom](https://github.com/pydicom/pydicom) is used to read and parse 
+the DICOM files. 
+
+Additionally, the command line tool `dump_dcm_info` is available that displays 
+the tag values of one or several DICOM files in a readable format. It is
+provided as a proof of concept of getting information directly from the
+DICOM standard.
+
+*Disclaimer:*  
+No guarantees are given for the correctness of the results.
+This is alpha-stage software and mostly thought as a proof of concept.
+Also check the limitations for `validate_iods` described below.
+
+*Note:*
+The original name of the package (`dcm-spec-tools`) has been 
+changed to `dicom-validator` together with the move to the `pydicom` 
+organization to reflect the fact that no other tools are planned, and that the 
+DICOM validator is the relevant tool.
+
+
+## Installation
+
+The latest version is available on pypi and can be installed via
+```
+pip install dicom-validator
+```
+
+## Usage
+```
+dump_dcm_info [-r <revision>] [-src <spec dir>] <DICOM filename>
+validate_iods [-r <revision>] [-src <spec dir>] [-v] <DICOM files or directories>
+```
+Use the `--help` option for each script do get usage info.
+
+## Access to the DICOM standard
+
+Upon first start of a tool, part of the latest version of the DICOM standard
+in docbook format (specifically, parts 3.3, 3.4 and 3.6) are downloaded, 
+parsed, and the needed information saved in json files. If the `--src` 
+parameter is not provided, the files are downloaded to and looked up in
+`<user home>/dicom-validator/`.    
+These files are then used by the tools. Periodically (once a month), the tools
+check for a newer version of the DICOM standard and download it if found.
+
+It is also possible to use older versions of the standard via the command line 
+option `--revision` or `-r`, provided they are available for download 
+(at the time of writing, standards are available since revision 2014a). A 
+list of currently available editions can be found in
+*<user home>/dicom-validator/editions.json* after a tool has been called 
+the first time.
+
+## validate_iods
+
+This checks a given DICOM file, or all DICOM files recursively in a given
+directory, for correct tags for the related SOP class. Only the presence or  
+absence of the tag, and the presence of a tag value is checked, not the
+contained value itself (a check for correct enumerated values may be added later).
+This is done by looking up all required and optional modules for this
+SOP class, and checking the tags for these modules. Tags that are not allowed or
+missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
+to collect the needed information.
+Conditions for type 1C and 2C modules and tags are evaluated if possible.
+If the evaluation fails, the respective modules and tags are considered
+optional. 
+
+The output for a single file may look like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>validate_iods "c:\dev\DICOM Data\SR\test.dcm"
+
+Processing DICOM file "c:\dev\DICOM Data\SR\test.dcm"
+SOP class is "1.2.840.10008.5.1.4.1.1.88.33" (Comprehensive SR IOD)
+
+Errors
+======
+Module "SR Document Content":
+Tag (0040,A043) (Concept Name Code Sequence) is not allowed due to condition:
+  Value Type is equal to "TEXT", "NUM", "CODE", "DATETIME", "DATE", "TIME", "UIDREF" or "PNAME"
+Tag (0040,A300) (Measured Value Sequence) is missing
+Tag (0040,A168) (Concept Code Sequence) is missing
+Tag (0008,1199) (Referenced SOP Sequence) is missing
+Tag (0070,0022) (Graphic Data) is missing
+Tag (0070,0023) (Graphic Type) is missing
+Tag (3006,0024) (Referenced Frame of Reference UID) is missing
+Tag (0040,A130) (Temporal Range Type) is missing
+Tag (0040,A138) (Referenced Time Offsets) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced DateTime is not present
+Tag (0040,A13A) (Referenced DateTime) is missing due to condition:
+  Referenced Sample Positions is not present and Referenced Time Offsets is not present
+```
+
+### Limitations
+
+#### Condition evaluation
+As mentioned, if the evaluation of conditions fails, the related module or 
+tag is considered optional, which may hide some non-conformity.  
+Condition evaluation may fail if:
+- the needed information is not contained in the DICOM file (e.g. verbose
+  descriptions like "if the Patient is an animal")
+- the information is related to other DICOM files (e.g. referenced images)
+- the parsing failed because the condition is too complicated, unexpected,
+  or due to a bug (please write an issue if you encounter such a problem)
+  
+#### Retired tags 
+Also note that only the given standard is used to evaluate the files. If 
+the DICOM file has been written using an older standard, it may conform to 
+that standard, but not to the newest one. Tags that are retired in the 
+version of the standard used for parsing are not considered at all.
+
+#### Unsupported cases (support may be added in future versions)
+- SOP classes not in the table in PS3.3 such as Presentation States are not 
+  handled
+- functional groups in EnhancedXXX SOP classes are not handled
+
+
+## dump_dcm_info
+
+This is a very simple DICOM dump tool, which uses 
+the DICOM dictionary as read from part 6 of the standard. It prints the 
+DICOM header of the given DICOM file, or of all DICOM files recursively in a 
+given directory. The output looks like this:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM 
+Data\SR\image12.dcm"
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0005,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+(0005,1000) [Unknown]                                UN    1  [\x00\x05 \x08\x00\x00\x00\n  RIGHT   \x00\x05\xc1X\x00\x00\x00\x06 0.09 \x00\x05...]
+(0008,0008) Image Type                               CS    0  []
+(0008,0016) SOP Class UID                            UI    1  [Ultrasound Image Storage (Retired)]
+(0008,0018) SOP Instance UID                         UI    1  [1.2.840.113680.3.103.775.2873347909.282313.2]
+(0008,0020) Study Date                               DA    1  [19950119]
+(0008,0030) Study Time                               TM    1  [092854.0]
+(0008,0050) Accession Number                         SH    1  [ACN000001]
+(0008,0060) Modality                                 CS    1  [US]
+(0008,0070) Manufacturer                             LO    1  [Acuson]
+(0008,0090) Referring Physician's Name               PN    1  []
+(0008,1010) Station Name                             SH    1  [QV-00775]
+(0008,1030) Study Description                        LO    1  [ABDOMEN]
+(0008,1050) Performing Physician's Name              PN    1  [DOE,JOHN]
+(0008,1060) Name of Physician(s) Reading Study       PN    1  []
+(0008,1070) Operators' Name                          PN    1  [DO]
+(0008,1080) Admitting Diagnoses Description          LO    1  [RSNA'95 Data Not Delete]
+(0009,0010) [Unknown]                                LO    1  [AEGIS_DICOM_2.00]
+...
+```
+
+If you want to show only specific tags, you can use the option `--show-tags`:
+```
+(py3_test) c:\dev\GitHub\dicom-validator>dump_dcm_info "c:\dev\DICOM Data\SR\image12.dcm" --show-tags 0010,0010 PatientID
+
+c:\dev\DICOM Data\SR\image12.dcm
+(0010,0010) Patient's Name                           PN    1  [DOE^JANE]
+(0010,0020) Patient ID                               LO    1  [ACN000001]
+```
```

