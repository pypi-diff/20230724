# Comparing `tmp/ansible_later-3.3.5.tar.gz` & `tmp/ansible_later-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_later-3.3.5.tar", max compression
+gzip compressed data, was "ansible_later-3.3.7.tar", max compression
```

## Comparing `ansible_later-3.3.5.tar` & `ansible_later-3.3.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1123 2023-06-24 13:43:37.644018 ansible_later-3.3.5/LICENSE
--rw-r--r--   0        0        0     3173 2023-06-24 13:43:37.644018 ansible_later-3.3.5/README.md
--rw-r--r--   0        0        0      120 2023-06-24 13:43:52.684012 ansible_later-3.3.5/ansiblelater/__init__.py
--rwxr-xr-x   0        0        0     2892 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/__main__.py
--rw-r--r--   0        0        0     9843 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/candidate.py
--rw-r--r--   0        0        0      666 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/exceptions.py
--rw-r--r--   0        0        0     5180 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/logger.py
--rw-r--r--   0        0        0      834 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckBecomeUser.py
--rw-r--r--   0        0        0     1636 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckBracesSpaces.py
--rw-r--r--   0        0        0     2346 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckChangedInWhen.py
--rw-r--r--   0        0        0     1079 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckCommandHasChanges.py
--rw-r--r--   0        0        0     2650 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckCommandInsteadOfArgument.py
--rw-r--r--   0        0        0     2031 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckCommandInsteadOfModule.py
--rw-r--r--   0        0        0     1227 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckCompareToEmptyString.py
--rw-r--r--   0        0        0     1229 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckCompareToLiteralBool.py
--rw-r--r--   0        0        0      952 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckDeprecated.py
--rw-r--r--   0        0        0     3822 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckDeprecatedBareVars.py
--rw-r--r--   0        0        0     3764 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckFilePermissionMissing.py
--rw-r--r--   0        0        0     3106 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckFilePermissionOctal.py
--rw-r--r--   0        0        0     1156 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckFilterSeparation.py
--rw-r--r--   0        0        0     1921 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckGitHasVersion.py
--rw-r--r--   0        0        0     1162 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckInstallUseLatest.py
--rw-r--r--   0        0        0      941 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckLiteralBoolFormat.py
--rw-r--r--   0        0        0      737 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckLocalAction.py
--rw-r--r--   0        0        0     1182 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckMetaChangeFromDefault.py
--rw-r--r--   0        0        0     1201 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckMetaMain.py
--rw-r--r--   0        0        0      892 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckNameFormat.py
--rw-r--r--   0        0        0      897 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckNamedTask.py
--rw-r--r--   0        0        0     1679 2023-06-24 13:43:37.644018 ansible_later-3.3.5/ansiblelater/rules/CheckNativeYaml.py
--rw-r--r--   0        0        0     2179 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckNestedJinja.py
--rw-r--r--   0        0        0     1235 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckRelativeRolePaths.py
--rw-r--r--   0        0        0      786 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckScmInSrc.py
--rw-r--r--   0        0        0     1064 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckShellInsteadCommand.py
--rw-r--r--   0        0        0     1601 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckTaskSeparation.py
--rw-r--r--   0        0        0      904 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckUniqueNamedTask.py
--rw-r--r--   0        0        0      590 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckVersion.py
--rw-r--r--   0        0        0      891 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckWhenFormat.py
--rw-r--r--   0        0        0      518 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlColons.py
--rw-r--r--   0        0        0      517 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlDocumentEnd.py
--rw-r--r--   0        0        0      525 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlDocumentStart.py
--rw-r--r--   0        0        0      524 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlEmptyLines.py
--rw-r--r--   0        0        0      684 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlFile.py
--rw-r--r--   0        0        0      627 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlHasContent.py
--rw-r--r--   0        0        0      521 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlHyphens.py
--rw-r--r--   0        0        0      526 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/rules/CheckYamlIndent.py
--rw-r--r--   0        0        0     7899 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/settings.py
--rw-r--r--   0        0        0    11937 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/standard.py
--rw-r--r--   0        0        0        0 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/test/__init__.py
--rw-r--r--   0        0        0        0 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/test/unit/__init__.py
--rw-r--r--   0        0        0     2337 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/test/unit/test_logger.py
--rw-r--r--   0        0        0      527 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/test/unit/test_settings.py
--rw-r--r--   0        0        0     2909 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/utils/__init__.py
--rw-r--r--   0        0        0    19029 2023-06-24 13:43:37.648018 ansible_later-3.3.5/ansiblelater/utils/yamlhelper.py
--rw-r--r--   0        0        0     3475 2023-06-24 13:43:52.680012 ansible_later-3.3.5/pyproject.toml
--rw-r--r--   0        0        0     4876 1970-01-01 00:00:00.000000 ansible_later-3.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-07-24 07:05:29.055510 ansible_later-3.3.7/LICENSE
+-rw-r--r--   0        0        0     3173 2023-07-24 07:05:29.055510 ansible_later-3.3.7/README.md
+-rw-r--r--   0        0        0      120 2023-07-24 07:05:44.063698 ansible_later-3.3.7/ansiblelater/__init__.py
+-rwxr-xr-x   0        0        0     2892 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/__main__.py
+-rw-r--r--   0        0        0     9835 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/candidate.py
+-rw-r--r--   0        0        0      666 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/logger.py
+-rw-r--r--   0        0        0      834 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckBecomeUser.py
+-rw-r--r--   0        0        0     1636 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckBracesSpaces.py
+-rw-r--r--   0        0        0     2553 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckChangedInWhen.py
+-rw-r--r--   0        0        0     1079 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckCommandHasChanges.py
+-rw-r--r--   0        0        0     2650 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckCommandInsteadOfArgument.py
+-rw-r--r--   0        0        0     2031 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckCommandInsteadOfModule.py
+-rw-r--r--   0        0        0     1227 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckCompareToEmptyString.py
+-rw-r--r--   0        0        0     1229 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckCompareToLiteralBool.py
+-rw-r--r--   0        0        0      952 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckDeprecated.py
+-rw-r--r--   0        0        0     3822 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckDeprecatedBareVars.py
+-rw-r--r--   0        0        0     3764 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckFilePermissionMissing.py
+-rw-r--r--   0        0        0     3106 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckFilePermissionOctal.py
+-rw-r--r--   0        0        0     1156 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckFilterSeparation.py
+-rw-r--r--   0        0        0     1921 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckGitHasVersion.py
+-rw-r--r--   0        0        0     1162 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckInstallUseLatest.py
+-rw-r--r--   0        0        0      941 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckLiteralBoolFormat.py
+-rw-r--r--   0        0        0      737 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckLocalAction.py
+-rw-r--r--   0        0        0     1182 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckMetaChangeFromDefault.py
+-rw-r--r--   0        0        0     1201 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckMetaMain.py
+-rw-r--r--   0        0        0      892 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckNameFormat.py
+-rw-r--r--   0        0        0      897 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckNamedTask.py
+-rw-r--r--   0        0        0     1679 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckNativeYaml.py
+-rw-r--r--   0        0        0     2179 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckNestedJinja.py
+-rw-r--r--   0        0        0     1235 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckRelativeRolePaths.py
+-rw-r--r--   0        0        0      786 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckScmInSrc.py
+-rw-r--r--   0        0        0     1064 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckShellInsteadCommand.py
+-rw-r--r--   0        0        0     1601 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckTaskSeparation.py
+-rw-r--r--   0        0        0      904 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckUniqueNamedTask.py
+-rw-r--r--   0        0        0      590 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckVersion.py
+-rw-r--r--   0        0        0      891 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckWhenFormat.py
+-rw-r--r--   0        0        0      518 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlColons.py
+-rw-r--r--   0        0        0      517 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlDocumentEnd.py
+-rw-r--r--   0        0        0      525 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlDocumentStart.py
+-rw-r--r--   0        0        0      524 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlEmptyLines.py
+-rw-r--r--   0        0        0      684 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlFile.py
+-rw-r--r--   0        0        0      627 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlHasContent.py
+-rw-r--r--   0        0        0      521 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlHyphens.py
+-rw-r--r--   0        0        0      526 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/rules/CheckYamlIndent.py
+-rw-r--r--   0        0        0     7902 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/settings.py
+-rw-r--r--   0        0        0    11935 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/standard.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/test/unit/__init__.py
+-rw-r--r--   0        0        0     2337 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/test/unit/test_logger.py
+-rw-r--r--   0        0        0      527 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/test/unit/test_settings.py
+-rw-r--r--   0        0        0     2909 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/utils/__init__.py
+-rw-r--r--   0        0        0    18995 2023-07-24 07:05:29.055510 ansible_later-3.3.7/ansiblelater/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3491 2023-07-24 07:05:44.063698 ansible_later-3.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4878 1970-01-01 00:00:00.000000 ansible_later-3.3.7/PKG-INFO
```

### Comparing `ansible_later-3.3.5/LICENSE` & `ansible_later-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/README.md` & `ansible_later-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/__main__.py` & `ansible_later-3.3.7/ansiblelater/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/candidate.py` & `ansible_later-3.3.7/ansiblelater/candidate.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         return None
 
     def _format_id(self, standard_id):
         sid = standard_id.strip()
         if sid:
             standard_id = f"[{sid}] "
 
-        return standard_id  # noqa
+        return standard_id
 
     def __repr__(self):
         return f"{type(self).__name__} ({self.path})"
 
     def __getitem__(self, item):
         return self.__dict__.get(item)
```

### Comparing `ansible_later-3.3.5/ansiblelater/exceptions.py` & `ansible_later-3.3.7/ansiblelater/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/logger.py` & `ansible_later-3.3.7/ansiblelater/logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckBecomeUser.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckBecomeUser.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckBracesSpaces.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckBracesSpaces.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckChangedInWhen.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckChangedInWhen.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def check(self, candidate, settings):
         tasks, errors = self.get_normalized_tasks(candidate, settings)
 
         if not errors:
             for task in tasks:
                 when = None
 
-                if task["__ansible_action_type__"] == "task":
+                if task["__ansible_action_type__"] in ["task", "meta"]:
                     when = task.get("when")
 
                 if isinstance(when, str):
                     when = [when]
 
                 if isinstance(when, list):
                     for item in when:
@@ -50,10 +50,19 @@
         return self.Result(candidate.path, errors)
 
     @staticmethod
     def _changed_in_when(item):
         if not isinstance(item, str):
             return False
 
+        if not {"and", "or", "not"}.isdisjoint(item.split()):
+            return False
+
         return any(
-            changed in item for changed in [".changed", "|changed", '["changed"]', "['changed']"]
+            changed in item for changed in [
+                ".changed",
+                "|changed",
+                '["changed"]',
+                "['changed']",
+                "is changed",
+            ]
         )
```

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckCommandHasChanges.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckCommandHasChanges.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckCommandInsteadOfArgument.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckCommandInsteadOfArgument.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckCommandInsteadOfModule.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckCommandInsteadOfModule.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckCompareToEmptyString.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckCompareToEmptyString.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckCompareToLiteralBool.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckCompareToLiteralBool.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckDeprecated.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckDeprecated.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckDeprecatedBareVars.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckDeprecatedBareVars.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckFilePermissionMissing.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckFilePermissionMissing.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckFilePermissionOctal.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckFilePermissionOctal.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckFilterSeparation.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckFilterSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckGitHasVersion.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckGitHasVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckInstallUseLatest.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckInstallUseLatest.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckLiteralBoolFormat.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckLiteralBoolFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckLocalAction.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckLocalAction.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckMetaChangeFromDefault.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckMetaChangeFromDefault.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckMetaMain.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckMetaMain.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckNameFormat.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckNameFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckNamedTask.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckNativeYaml.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckNativeYaml.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckNestedJinja.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckNestedJinja.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckRelativeRolePaths.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckRelativeRolePaths.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckScmInSrc.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckScmInSrc.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckShellInsteadCommand.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckShellInsteadCommand.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckTaskSeparation.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckTaskSeparation.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckUniqueNamedTask.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckUniqueNamedTask.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckVersion.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckVersion.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckWhenFormat.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckWhenFormat.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlColons.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlColons.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlDocumentEnd.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlDocumentEnd.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlDocumentStart.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlDocumentStart.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlEmptyLines.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlEmptyLines.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlFile.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlFile.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlHasContent.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlHasContent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlHyphens.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlHyphens.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/rules/CheckYamlIndent.py` & `ansible_later-3.3.7/ansiblelater/rules/CheckYamlIndent.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/settings.py` & `ansible_later-3.3.7/ansiblelater/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     def _validate(self, config):
         try:
             anyconfig.validate(config, self.schema, ac_schema_safe=False)
             return True
         except jsonschema.exceptions.ValidationError as e:
             validator = e.validator
             path = format_as_index(
-                list(e.absolute_path)[0],
+                next(iter(e.absolute_path)),
                 list(e.absolute_path)[1:],
             )
             msg = e.message
 
             utils.sysexit_with_message(
                 "Error while loading configuration:\n"
                 f"Failed validating '{validator}' at {path}: {msg}"
```

### Comparing `ansible_later-3.3.5/ansiblelater/standard.py` & `ansible_later-3.3.7/ansiblelater/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
             self.candidate = candidate
             self.errors = errors or []
 
         def message(self):
             return "\n".join([f"{self.candidate}:{error}" for error in self.errors])
 
 
-class StandardLoader():
+class StandardLoader:
 
     def __init__(self, source):
         self.rules = []
 
         for s in source:
             for p in pathlib.Path(s).glob("*.py"):
                 filename = os.path.splitext(os.path.basename(p))[0]
```

### Comparing `ansible_later-3.3.5/ansiblelater/test/unit/test_logger.py` & `ansible_later-3.3.7/ansiblelater/test/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/test/unit/test_settings.py` & `ansible_later-3.3.7/ansiblelater/test/unit/test_settings.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/utils/__init__.py` & `ansible_later-3.3.7/ansiblelater/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_later-3.3.5/ansiblelater/utils/yamlhelper.py` & `ansible_later-3.3.7/ansiblelater/utils/yamlhelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,19 +205,18 @@
     return results
 
 
 def template(basedir, value, variables, fail_on_undefined=False, **kwargs):
     # Hack to skip the following exception when using to_json filter on a variable.
     # I guess the filter doesn't like empty vars...
     with suppress(AnsibleError, ValueError):
-        value = ansible_template(
+        return ansible_template(
             os.path.abspath(basedir), value, variables,
             **dict(kwargs, fail_on_undefined=fail_on_undefined)
         )
-    return value
 
 
 def play_children(basedir, item, parent_type):
     delegate_map = {
         "tasks": _taskshandlers_children,
         "pre_tasks": _taskshandlers_children,
         "post_tasks": _taskshandlers_children,
@@ -369,16 +368,15 @@
 
 
 def rolename(filepath):
     idx = filepath.find("roles/")
     if idx < 0:
         return ""
     role = filepath[idx + 6:]
-    role = role[:role.find("/")]
-    return role
+    return role[:role.find("/")]
 
 
 def _kv_to_dict(v):
     (command, args, kwargs) = tokenize(v)
     return (dict(__ansible_module__=command, __ansible_arguments__=args, **kwargs))
```

### Comparing `ansible_later-3.3.5/pyproject.toml` & `ansible_later-3.3.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 license = "MIT"
 name = "ansible-later"
 packages = [
   {include = "ansiblelater"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-later/"
-version = "3.3.5"
+version = "3.3.7"
 
 [tool.poetry.dependencies]
-PyYAML = "6.0"
-ansible = {version = "8.1.0", optional = true}
-ansible-core = {version = "2.15.1", optional = true}
+PyYAML = "6.0.1"
+ansible = {version = "8.2.0", optional = true}
+ansible-core = {version = "2.15.2", optional = true}
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
-jsonschema = "4.17.3"
+jsonschema = "4.18.4"
 nested-lookup = "0.2.25"
 pathspec = "0.11.1"
 python = "^3.9.0"
 python-json-logger = "2.0.7"
 toolz = "0.12.0"
 unidiff = "0.7.5"
 yamllint = "1.32.0"
@@ -52,20 +52,20 @@
 ansible = ["ansible"]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-later = "ansiblelater.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.272"
-pytest = "7.3.2"
+ruff = "0.0.280"
+pytest = "7.4.0"
 pytest-mock = "3.11.1"
 pytest-cov = "4.1.0"
 toml = "0.10.2"
-yapf = "0.40.0"
+yapf = "0.40.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
 
 [tool.pytest.ini_options]
@@ -114,14 +114,15 @@
     "D103",
     "D105",
     "D107",
     "D202",
     "D203",
     "D212",
     "UP038",
+    "RUF012",
 ]
 line-length = 99
 select = [
     "D",
     "E",
     "F",
     "Q",
```

### Comparing `ansible_later-3.3.5/PKG-INFO` & `ansible_later-3.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-later
-Version: 3.3.5
+Version: 3.3.7
 Summary: Reviews ansible playbooks, roles and inventories and suggests improvements.
 Home-page: https://ansible-later.geekdocs.de/
 License: MIT
 Keywords: ansible,code,review
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -20,21 +20,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Provides-Extra: ansible
 Provides-Extra: ansible-core
-Requires-Dist: PyYAML (==6.0)
-Requires-Dist: ansible (==8.1.0) ; extra == "ansible"
-Requires-Dist: ansible-core (==2.15.1) ; extra == "ansible-core"
+Requires-Dist: PyYAML (==6.0.1)
+Requires-Dist: ansible (==8.2.0) ; extra == "ansible"
+Requires-Dist: ansible-core (==2.15.2) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.13.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
-Requires-Dist: jsonschema (==4.17.3)
+Requires-Dist: jsonschema (==4.18.4)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: python-json-logger (==2.0.7)
 Requires-Dist: toolz (==0.12.0)
 Requires-Dist: unidiff (==0.7.5)
 Requires-Dist: yamllint (==1.32.0)
 Project-URL: Documentation, https://ansible-later.geekdocs.de/
```

