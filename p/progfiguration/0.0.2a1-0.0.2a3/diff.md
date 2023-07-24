# Comparing `tmp/progfiguration-0.0.2a1.tar.gz` & `tmp/progfiguration-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progfiguration-0.0.2a1.tar", last modified: Wed Jul 12 20:07:47 2023, max compression
+gzip compressed data, was "progfiguration-0.0.2a3.tar", last modified: Mon Jul 24 04:15:21 2023, max compression
```

## Comparing `progfiguration-0.0.2a1.tar` & `progfiguration-0.0.2a3.tar`

### file list

```diff
@@ -1,60 +1,48 @@
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.884193 progfiguration-0.0.2a1/
--rw-------   0 mrled      (501) staff       (20)     1180 2023-07-12 20:07:47.883654 progfiguration-0.0.2a1/PKG-INFO
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.845552 progfiguration-0.0.2a1/progfiguration/
--rw-------   0 mrled      (501) staff       (20)      504 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/__init__.py
--rw-------   0 mrled      (501) staff       (20)     2908 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/age.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.851546 progfiguration-0.0.2a1/progfiguration/cli/
--rw-------   0 mrled      (501) staff       (20)     3713 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/cli/__init__.py
--rw-------   0 mrled      (501) staff       (20)    21793 2023-07-12 19:14:06.000000 progfiguration-0.0.2a1/progfiguration/cli/progfiguration_cmd.py
--rw-------   0 mrled      (501) staff       (20)     5023 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/cmd.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.855663 progfiguration-0.0.2a1/progfiguration/example_site/
--rw-r--r--   0 mrled      (501) staff       (20)      345 2023-07-11 17:14:18.000000 progfiguration-0.0.2a1/progfiguration/example_site/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.858852 progfiguration-0.0.2a1/progfiguration/example_site/groups/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:30.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      172 2023-07-11 17:29:06.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/group1.py
--rw-r--r--   0 mrled      (501) staff       (20)      397 2023-07-11 17:32:05.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/universal.py
--rw-r--r--   0 mrled      (501) staff       (20)     1007 2023-07-11 17:29:52.000000 progfiguration-0.0.2a1/progfiguration/example_site/inventory.yml
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.860547 progfiguration-0.0.2a1/progfiguration/example_site/nodes/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:37.000000 progfiguration-0.0.2a1/progfiguration/example_site/nodes/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      395 2023-07-12 19:12:41.000000 progfiguration-0.0.2a1/progfiguration/example_site/nodes/node1.py
--rw-r--r--   0 mrled      (501) staff       (20)      244 2023-07-12 03:27:25.000000 progfiguration-0.0.2a1/progfiguration/example_site/readme.md
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.862360 progfiguration-0.0.2a1/progfiguration/example_site/roles/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:43.000000 progfiguration-0.0.2a1/progfiguration/example_site/roles/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      515 2023-07-11 17:26:59.000000 progfiguration-0.0.2a1/progfiguration/example_site/roles/settz.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.863565 progfiguration-0.0.2a1/progfiguration/example_site/sitelib/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:37:09.000000 progfiguration-0.0.2a1/progfiguration/example_site/sitelib/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.866672 progfiguration-0.0.2a1/progfiguration/inventory/
--rw-------   0 mrled      (501) staff       (20)    14074 2023-07-12 19:13:35.000000 progfiguration-0.0.2a1/progfiguration/inventory/__init__.py
--rw-------   0 mrled      (501) staff       (20)      835 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/inventory/nodes.py
--rw-------   0 mrled      (501) staff       (20)     4431 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/inventory/roles.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.871391 progfiguration-0.0.2a1/progfiguration/localhost/
--rw-------   0 mrled      (501) staff       (20)    11080 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1184 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/authorized_keys.py
--rw-------   0 mrled      (501) staff       (20)     6062 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/disks.py
--rw-------   0 mrled      (501) staff       (20)     3044 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/localusers.py
--rw-------   0 mrled      (501) staff       (20)      593 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/progfigtypes.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.872860 progfiguration-0.0.2a1/progfiguration/remotebrute/
--rw-------   0 mrled      (501) staff       (20)     3067 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remotebrute/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.875850 progfiguration-0.0.2a1/progfiguration/remoting/
--rw-------   0 mrled      (501) staff       (20)     6265 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remoting/__init__.py
--rw-------   0 mrled      (501) staff       (20)      222 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remoting/rfuncs.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.877620 progfiguration-0.0.2a1/progfiguration/sitewrapper/
--rw-r--r--   0 mrled      (501) staff       (20)     2271 2023-07-12 20:00:14.000000 progfiguration-0.0.2a1/progfiguration/sitewrapper/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1072 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/ssh.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.878906 progfiguration-0.0.2a1/progfiguration/temple/
--rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/temple/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1406 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/version.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.849623 progfiguration-0.0.2a1/progfiguration.egg-info/
--rw-------   0 mrled      (501) staff       (20)     1180 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/PKG-INFO
--rw-------   0 mrled      (501) staff       (20)     1458 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/SOURCES.txt
--rw-------   0 mrled      (501) staff       (20)        1 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/dependency_links.txt
--rw-------   0 mrled      (501) staff       (20)       78 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/entry_points.txt
--rw-------   0 mrled      (501) staff       (20)       82 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/requires.txt
--rw-------   0 mrled      (501) staff       (20)       15 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/top_level.txt
--rw-------   0 mrled      (501) staff       (20)      740 2023-07-12 20:06:27.000000 progfiguration-0.0.2a1/pyproject.toml
--rw-------   0 mrled      (501) staff       (20)      823 2023-07-12 20:07:27.000000 progfiguration-0.0.2a1/readme.md
--rw-------   0 mrled      (501) staff       (20)       38 2023-07-12 20:07:47.884378 progfiguration-0.0.2a1/setup.cfg
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.882249 progfiguration-0.0.2a1/tests/
--rw-------   0 mrled      (501) staff       (20)     1170 2023-06-28 22:11:56.000000 progfiguration-0.0.2a1/tests/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1332 2023-06-28 22:11:56.000000 progfiguration-0.0.2a1/tests/test_cmd.py
--rw-------   0 mrled      (501) staff       (20)     1088 2023-07-12 04:46:25.000000 progfiguration-0.0.2a1/tests/test_site.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.742926 progfiguration-0.0.2a3/
+-rw-------   0 mrled      (501) staff       (20)     2108 2023-07-24 04:15:21.742426 progfiguration-0.0.2a3/PKG-INFO
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.720476 progfiguration-0.0.2a3/progfiguration/
+-rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a3/progfiguration/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a3/progfiguration/age.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.725284 progfiguration-0.0.2a3/progfiguration/builddata/
+-rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a3/progfiguration/builddata/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.729733 progfiguration-0.0.2a3/progfiguration/cli/
+-rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a3/progfiguration/cli/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     6705 2023-07-24 03:58:20.000000 progfiguration-0.0.2a3/progfiguration/cli/progfiguration_core_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)    21295 2023-07-23 23:30:07.000000 progfiguration-0.0.2a3/progfiguration/cli/progfiguration_site_cmd.py
+-rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a3/progfiguration/cli/util.py
+-rw-------   0 mrled      (501) staff       (20)     5927 2023-07-22 05:27:56.000000 progfiguration-0.0.2a3/progfiguration/cmd.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.732409 progfiguration-0.0.2a3/progfiguration/inventory/
+-rw-------   0 mrled      (501) staff       (20)    17722 2023-07-23 23:22:00.000000 progfiguration-0.0.2a3/progfiguration/inventory/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a3/progfiguration/inventory/nodes.py
+-rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a3/progfiguration/inventory/roles.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.736630 progfiguration-0.0.2a3/progfiguration/localhost/
+-rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a3/progfiguration/localhost/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a3/progfiguration/localhost/authorized_keys.py
+-rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a3/progfiguration/localhost/disks.py
+-rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a3/progfiguration/localhost/localusers.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.737320 progfiguration-0.0.2a3/progfiguration/progfigbuild/
+-rw-r--r--   0 mrled      (501) staff       (20)    17408 2023-07-24 04:09:57.000000 progfiguration-0.0.2a3/progfiguration/progfigbuild/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a3/progfiguration/progfigsite_validator.py
+-rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a3/progfiguration/progfigtypes.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.738344 progfiguration-0.0.2a3/progfiguration/remotebrute/
+-rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a3/progfiguration/remotebrute/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.739054 progfiguration-0.0.2a3/progfiguration/sitewrapper/
+-rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a3/progfiguration/sitewrapper/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a3/progfiguration/ssh.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.739686 progfiguration-0.0.2a3/progfiguration/temple/
+-rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a3/progfiguration/temple/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-23 22:41:01.000000 progfiguration-0.0.2a3/progfiguration/util.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.724654 progfiguration-0.0.2a3/progfiguration.egg-info/
+-rw-------   0 mrled      (501) staff       (20)     2108 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/PKG-INFO
+-rw-------   0 mrled      (501) staff       (20)     1100 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/SOURCES.txt
+-rw-------   0 mrled      (501) staff       (20)        1 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/dependency_links.txt
+-rw-------   0 mrled      (501) staff       (20)       83 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/entry_points.txt
+-rw-------   0 mrled      (501) staff       (20)       43 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/requires.txt
+-rw-------   0 mrled      (501) staff       (20)       15 2023-07-24 04:15:21.000000 progfiguration-0.0.2a3/progfiguration.egg-info/top_level.txt
+-rw-------   0 mrled      (501) staff       (20)      712 2023-07-24 04:14:18.000000 progfiguration-0.0.2a3/pyproject.toml
+-rw-------   0 mrled      (501) staff       (20)     1771 2023-07-23 20:27:37.000000 progfiguration-0.0.2a3/readme.md
+-rw-------   0 mrled      (501) staff       (20)       38 2023-07-24 04:15:21.743080 progfiguration-0.0.2a3/setup.cfg
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-24 04:15:21.741635 progfiguration-0.0.2a3/tests/
+-rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a3/tests/test_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a3/tests/test_packaging.py
+-rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a3/tests/test_site.py
```

### Comparing `progfiguration-0.0.2a1/progfiguration/age.py` & `progfiguration-0.0.2a3/progfiguration/age.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,48 @@
-"""A wrapper for the age binary to encrypt and decrypt secret values"""
+"""A wrapper for the age binary to encrypt and decrypt secret values
+
+Progfiguration uses age for secret management.
+All nodes must have an age keypair.
+"""
 
 from dataclasses import dataclass
 import datetime
 import subprocess
 from typing import List
 
 
 class AgeParseException(Exception):
     pass
 
 
 class AgeKey:
+    """An age keypair
+
+    Attributes:
+        secret: The secret key
+        public: The public key
+        created: The datetime the key was created
+    """
+
     def __init__(self, secret: str, public: str, created: datetime.datetime):
         self.secret = secret
         self.public = public
         self.created = created
 
     @classmethod
     def from_output(cls, output: str) -> "AgeKey":
-        example_stdout = """
+        """Parse the output of age-keygen into an AgeKey
+
+        Here's example output from age-keygen -y:
+
             # created: 2022-09-28T16:01:22-05:00
             # public key: age14e42u048nehghjj3ch9mmnkdh4nsujn774klqxn02mznppx3gflsuj6y5m
             AGE-SECRET-KEY-1ASKGXED4DVGUH7SA50DHE2UHAYQ00PV87N2RQ5J5S6AUN9MLNSGQ3TKFGJ
+
+        This function parses that output and returns an AgeKey object.
         """
         outlines = [l for l in output.split("\n") if l]
         if len(outlines) == 3:
             created = datetime.datetime.fromisoformat(outlines[0][11:])
             public = outlines[1][14:]
             secret = outlines[2]
         elif len(outlines) == 1:
@@ -35,47 +52,55 @@
             created = datetime.datetime.now()
         else:
             raise AgeParseException(f"Could not parse age output")
         return cls(secret, public, created)
 
     @classmethod
     def generate(cls) -> "AgeKey":
+        """Generate a new age keypair using the age-keygen binary"""
         result = subprocess.run(["age-keygen"], check=True, capture_output=True)
-        return cls.from_output(result.stdout)
+        return cls.from_output(result.stdout.decode())
 
     @classmethod
     def from_file(cls, path: str) -> "AgeKey":
+        """Load an age keypair from a file"""
         with open(path) as fp:
             content = fp.read()
         try:
             return cls.from_output(content)
         except AgeParseException:
             raise AgeParseException(f"Could not parse age key file at {path}")
 
 
 @dataclass
 class AgeSecret:
     """An age-encrypted secret value"""
 
     secret: str
+    """The encrypted secret value"""
 
     _decrypted: str = ""
 
     def decrypt(self, privkey_path: str):
-        """Decrypt a secret and cache the result."""
+        """Decrypt the secret and cache the result."""
         if not self._decrypted:
             self._decrypted = decrypt(self.secret, privkey_path)
         return self._decrypted
 
 
 @dataclass
 class AgeSecretReference:
-    """A reference to a secret by name"""
+    """A reference to a secret by name
+
+    This is a wrapper type that allows us to pass around a reference to a secret
+    without having to know the secret's value.
+    """
 
     name: str
+    """The name of the secret"""
 
 
 def encrypt(value: str, pubkeys: List[str]):
     """Encrypt a value to a list of public age keys"""
     age_cmd = ["age", "--armor"]
     for pubkey in pubkeys:
         age_cmd.append("--recipient")
```

### Comparing `progfiguration-0.0.2a1/progfiguration/cli/progfiguration_cmd.py` & `progfiguration-0.0.2a3/progfiguration/cli/progfiguration_site_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 """The command line interface for progfiguration"""
 
 import argparse
+import datetime
 import importlib
+import importlib.metadata
+import json
 import logging
 import os
 import pathlib
-import pdb
 import subprocess
 import sys
 import tempfile
 import time
-from typing import List, Union
+from typing import List, Optional
 
-from progfiguration import logger, progfiguration_build_path, remotebrute, sitewrapper, version
-from progfiguration.cli import (
-    progfiguration_error_handler,
+import progfiguration
+from progfiguration import logger, progfigbuild, remotebrute, sitewrapper
+from progfiguration.cli.util import (
+    CommaSeparatedStrList,
     configure_logging,
+    get_command_help,
     idb_excepthook,
+    progfiguration_error_handler,
     progfiguration_log_levels,
     syslog_excepthook,
-    yaml_dump_str,
 )
 from progfiguration.inventory import Inventory
+from progfiguration.progfigsite_validator import validate
 
-try:
-    from progfiguration import remoting
 
-    REMOTING = True
-except ModuleNotFoundError:
-    REMOTING = False
+def _action_version_core():
+    """Retrieve the version of progfiguration core"""
 
+    coreversion = importlib.metadata.version("progfiguration")
+    result = [
+        f"progfiguration core:",
+        f"    path: {pathlib.Path(progfiguration.__file__).parent}",
+        f"    version: {coreversion}",
+    ]
+    print("\n".join(result))
 
-def ResolvedPath(p: str) -> str:
-    """Convert a user-input path to an absolute path"""
-    return os.path.realpath(os.path.normpath(os.path.expanduser(p)))
 
+def _action_version_all(inventory: Inventory):
+    """Retrieve the version of progfiguration core and the progfigsite"""
 
-def CommaSeparatedStrList(cssl: str) -> List[str]:
-    """Convert a string with commas into a list of strings"""
-    return cssl.split(",")
+    progfigsite = sitewrapper.get_progfigsite()
 
+    try:
+        builddata_version = sitewrapper.site_submodule("builddata.version")
+        version = builddata_version.version
+        builddate = builddata_version.builddate
+    except ModuleNotFoundError:
+        version = progfigsite.get_version()
+        builddate = datetime.datetime.utcnow()
 
-def import_progfiguration_build():
-    """Import the progfiguration_build module
+    result = [
+        f"progfigsite:",
+        f"    path: {sitewrapper.get_progfigsite_path()}",
+        f"    name: {progfigsite.site_name}",
+        f"    description: {progfigsite.site_description}",
+        f"    build date: {version}",
+        f"    version: {builddate}",
+    ]
 
-    This module is also used outside of the progfiguration CLI, which is why we do this.
-    """
-    spec = importlib.util.spec_from_file_location("progfiguration_build", progfiguration_build_path)
-    progfiguration_build = importlib.util.module_from_spec(spec)
-    sys.modules["progfiguration_build"] = progfiguration_build
-    spec.loader.exec_module(progfiguration_build)
-    return progfiguration_build
+    _action_version_core()
+    print("\n".join(result))
 
 
-def action_apply(inventory: Inventory, nodename: str, roles: list[str] = None, force: bool = False):
+def _action_apply(inventory: Inventory, nodename: str, roles: Optional[List[str]] = None, force: bool = False):
     """Apply configuration for the node 'nodename' to localhost"""
 
     if roles is None:
         roles = []
 
     node = inventory.node(nodename).node
 
@@ -77,29 +91,29 @@
                 raise
         else:
             logging.info(f"Skipping role {role.name}.")
 
     logging.info(f"Finished running all roles")
 
 
-def action_list(inventory: Inventory, collection: str):
+def _action_list(inventory: Inventory, collection: str):
     if collection == "nodes":
         for node in inventory.nodes:
             print(node)
     elif collection == "groups":
         for group in inventory.groups:
             print(group)
     elif collection == "functions":
         for function in inventory.functions:
             print(function)
     else:
         raise Exception(f"Unknown collection {collection}")
 
 
-def action_info(inventory: Inventory, nodes: List[str], groups: List[str], functions: List[str]):
+def _action_info(inventory: Inventory, nodes: List[str], groups: List[str], functions: List[str]):
     if not any([nodes, groups, functions]):
         print("Request info on a node, group, or function. (See also the 'list' subcommand.)")
     for nodename in nodes:
         node_groups = inventory.node_groups[nodename]
         node_group_commas = ", ".join(node_groups)
         node_function = inventory.node_function[nodename]
         node_roles = inventory.function_roles[node_function]
@@ -116,15 +130,15 @@
         function_nodes = ", ".join(inventory.function_nodes[funcname])
         function_roles = ", ".join(inventory.function_roles[funcname])
         print(f"Function {funcname}:")
         print(f"  Nodes: {function_nodes}")
         print(f"  Roles: {function_roles}")
 
 
-def action_encrypt(
+def _action_encrypt(
     inventory: Inventory,
     name: str,
     value: str,
     nodes: List[str],
     groups: List[str],
     controller_key: bool,
     store: bool,
@@ -134,86 +148,62 @@
     print("Encrypted for all of these recipients:")
     for pk in recipients:
         print(pk)
     if stdout:
         print(encrypted_value)
 
 
-def action_decrypt(inventory: Inventory, nodes: List[str], groups: List[str], controller_key: bool):
+def _action_decrypt(inventory: Inventory, nodes: List[str], groups: List[str], controller_key: bool):
+    age_path = inventory.age_path
+    if not age_path:
+        raise Exception("Could not find age key")
     for node in nodes:
         print(f"Secrets for node {node}:")
         print("---")
-        decrypted_secrets = {k: v.decrypt(inventory.age_path) for k, v in inventory.get_node_secrets(node).items()}
-        print(yaml_dump_str(decrypted_secrets, {"default_style": "|"}))
+        decrypted_secrets = {k: v.decrypt(age_path) for k, v in inventory.get_node_secrets(node).items()}
+        print(json.dumps(decrypted_secrets, indent=2, sort_keys=True))
         print("---")
     for group in groups:
         print(f"Secrets for group {group}:")
         print("---")
-        decrypted_secrets = {k: v.decrypt(inventory.age_path) for k, v in inventory.get_group_secrets(group).items()}
-        print(yaml_dump_str(decrypted_secrets, {"default_style": "|"}))
+        decrypted_secrets = {k: v.decrypt(age_path) for k, v in inventory.get_group_secrets(group).items()}
+        print(json.dumps(decrypted_secrets, indent=2, sort_keys=True))
         print("---")
     if controller_key:
         print(f"Secrets for the controller:")
         print("---")
-        decrypted_secrets = {k: v.decrypt(inventory.age_path) for k, v in inventory.get_controller_secrets().items()}
-        print(yaml_dump_str(decrypted_secrets, {"default_style": "|"}))
+        decrypted_secrets = {k: v.decrypt(age_path) for k, v in inventory.get_controller_secrets().items()}
+        print(json.dumps(decrypted_secrets, indent=2, sort_keys=True))
         print("---")
 
 
-def action_build(parsed: argparse.Namespace):
-    """Build the progfiguration package
-
-    Must pass in the parsed arguments from the main command.
-    """
-
-    progfiguration_build = import_progfiguration_build()
-
-    if parsed.buildaction == "apk":
-        progfiguration_build.build_alpine(parsed.apkdir)
-    elif parsed.buildaction == "pyz":
-        progfiguration_build.build_zipapp(parsed.pyzfile)
-    elif parsed.buildaction == "save-version":
-        if not version:
-            version = progfiguration_build.get_epoch_build_version()
-        progfiguration_build.set_build_version(version)
-        print("Saved APKBUILD and package version files:")
-        print(progfiguration_build.APKBUILD_FILE)
-        print(progfiguration_build.PKG_VERSION_FILE)
-        print("Take care not to commit these files to git")
-    else:
-        raise Exception(f"Unknown buildaction {parsed.buildaction}")
-
-
-def action_rcmd(inventory: Inventory, nodes: List[str], groups: List[str], cmd: str):
-    remoting.command(inventory, nodes, groups, cmd)
-
-
-def action_deploy_apply(
+def _action_deploy_apply(
     inventory: Inventory,
     nodenames: List[str],
     groupnames: List[str],
     roles: List[str],
     remote_debug: bool,
     force_apply: bool,
     keep_remote_file: bool,
 ):
 
     if roles is None:
         roles = []
 
-    progfiguration_build = import_progfiguration_build()
+    for group in groupnames:
+        nodenames += inventory.group_members[group]
+    nodenames = list(set(nodenames))
 
-    nodenames = set(nodenames + [inventory.group_members(g) for g in groupnames])
     nodes = {n: inventory.node(n).node for n in nodenames}
 
     errors: list[dict[str, str]] = []
 
     with tempfile.TemporaryDirectory() as tmpdir:
-        pyzfile = os.path.join(tmpdir, "progfiguration.pyz")
-        progfiguration_build.build_zipapp(pyzfile)
+        pyzfile = pathlib.Path(os.path.join(tmpdir, "progfiguration.pyz"))
+        progfigbuild.build_progfigsite_zipapp(sitewrapper.get_progfigsite_path(), pyzfile)
         for nname, node in nodes.items():
             args = []
             if remote_debug:
                 args.append("--debug")
             args += ["apply", nname]
             if force_apply:
                 args.append("--force-apply")
@@ -225,15 +215,15 @@
             # * To ask sshd to create a tty with -tt
             # * To redirect stdin to /dev/null,
             #   which fixes some weird issues with bad newlines in the output for reasons I don't understand.
             # The result isn't perfect, as some lines are not printed exactly as they were in the output, but it's ok.
             try:
                 remotebrute.cpexec(
                     f"{node.user}@{node.address}",
-                    pyzfile,
+                    pyzfile.as_posix(),
                     args,
                     interpreter=["python3", "-u"],
                     ssh_tty=True,
                     ssh_stdin=subprocess.DEVNULL,
                     keep_remote_file=keep_remote_file,
                 )
             # except subprocess.CalledProcessError as exc:
@@ -245,34 +235,47 @@
     if errors:
         print("====================")
         print("Errors running progfiguration on {len(errors)} node(s):")
         for error in errors:
             print(f"  {error['node']}: {error['error']}")
 
 
-def action_deploy_copy(
+def _action_deploy_copy(
     inventory: Inventory,
     nodenames: List[str],
     groupnames: List[str],
     remotepath: str,
 ):
-    progfiguration_build = import_progfiguration_build()
+    for group in groupnames:
+        nodenames += inventory.group_members[group]
+    nodenames = list(set(nodenames))
 
-    nodenames = set(nodenames + [inventory.group_members(g) for g in groupnames])
     nodes = {n: inventory.node(n).node for n in nodenames}
 
     with tempfile.TemporaryDirectory() as tmpdir:
-        pyzfile = os.path.join(tmpdir, "progfiguration.pyz")
-        progfiguration_build.build_zipapp(pyzfile)
+        pyzfile = pathlib.Path(os.path.join(tmpdir, "progfiguration.pyz"))
+        progfigbuild.build_progfigsite_zipapp(sitewrapper.get_progfigsite_path(), pyzfile)
         for nname, node in nodes.items():
-            remotebrute.scp(f"{node.user}@{node.address}", pyzfile, remotepath)
+            remotebrute.scp(f"{node.user}@{node.address}", pyzfile.as_posix(), remotepath)
+
+
+def _action_validate():
+    validation = validate(progfiguration.progfigsite_module_path)
+    if validation.is_valid:
+        print(f"Progfigsite (Python path: '{progfiguration.progfigsite_module_path}') is valid.")
+    else:
+        print(
+            f"Progfigsite (Python path: '{progfiguration.progfigsite_module_path}') has {len(validation.errors)} errors:"
+        )
+    for attrib in validation.errors:
+        print(attrib.errstr)
 
 
-def parseargs(arguments: List[str]):
-    parser = argparse.ArgumentParser("psyopsOS programmatic configuration")
+def _make_parser():
+    parser = argparse.ArgumentParser("progfiguration site management tool")
 
     group_onerr = parser.add_mutually_exclusive_group()
     group_onerr.add_argument(
         "--debug",
         "-d",
         action="store_true",
         help="Open the debugger if an unhandled exception is encountered",
@@ -297,32 +300,15 @@
 
     parser.add_argument(
         "--log-syslog",
         default=syslog_default(),
         choices=progfiguration_log_levels,
         help="Log level to send to syslog. Defaults to INFO if /dev/log exists, otherwise NONE. NONE to disable. If a value other than NONE is passed explicitly and /dev/log does not exist, an exception will be raised.",
     )
-    parser.add_argument(
-        "--mitogen-log-stderr",
-        default="CRITICAL",
-        choices=progfiguration_log_levels,
-        help="Log level for mitogen messages to stderr. Only used for remote commands from the controller.",
-    )
-    parser.add_argument(
-        "--mitogen-io-log-stderr",
-        default="CRITICAL",
-        choices=progfiguration_log_levels,
-        help="Log level for mitogen IO messages to stderr. Only used for remote commands from the controller.",
-    )
-    parser.add_argument(
-        "--inventory-file",
-        "-f",
-        default=sitewrapper.site.package_inventory_file,
-        help="The path to an inventory yaml file. By default, use the one in the package",
-    )
+
     parser.add_argument(
         "--age-private-key", "-k", help="The path to an age private key that decrypts inventory secrets"
     )
 
     # node/group related options
     node_opts = argparse.ArgumentParser(add_help=False)
     node_opts.add_argument(
@@ -358,28 +344,28 @@
         type=CommaSeparatedStrList,
         help="A role, or list of roles separated by commas. The role(s) must be defined in the inventory for the node(s).",
     )
 
     subparsers = parser.add_subparsers(dest="action", required=True)
 
     # version subcommand
-    svn = subparsers.add_parser("version", description="Show progfiguration version")
+    svn_all = subparsers.add_parser("version", description="Show progfiguration core and progfigsite versions")
 
     # apply subcommand
     sub_apply = subparsers.add_parser("apply", parents=[roles_opts], description="Apply configuration")
     sub_apply.add_argument("nodename", help="The name of a node in the progfiguration inventory")
     sub_apply.add_argument(
         "--force-apply", action="store_true", help="Force apply, even if the node has TESTING_DO_NOT_APPLY set."
     )
 
     # deploy subcommand
     sub_deploy = subparsers.add_parser(
         "deploy",
         parents=[node_opts],
-        description="Deploy progfiguration to remote system in inventory as a pyz package (NOT a pip or apk package!); requires passwordless SSH configured",
+        description="Deploy progfiguration to remote system in inventory as a pyz package; requires passwordless SSH configured",
     )
     sub_deploy_subparsers = sub_deploy.add_subparsers(dest="deploy_action", required=True)
     sub_deploy_sub_apply = sub_deploy_subparsers.add_parser(
         "apply", parents=[roles_opts], description="Deploy and apply configuration"
     )
     sub_deploy_sub_apply.add_argument(
         "--remote-debug",
@@ -431,135 +417,158 @@
     sub_encrypt.add_argument("--stdout", action="store_true", help="Print encrypted value to stdout")
 
     # decrypt subcommand
     sub_decrypt = subparsers.add_parser(
         "decrypt", parents=[node_opts, ctrl_opts], description="Decrypt secrets from the secret store"
     )
 
-    # build subcommand
-    sub_build = subparsers.add_parser("build", description="Build the package")
-    sub_build_subparsers = sub_build.add_subparsers(dest="buildaction", required=True)
-    sub_build_sub_apk = sub_build_subparsers.add_parser(
-        "apk",
-        description="Build an Alpine APK package. Must be run from an editable install on an Alpine linux system with the appropriate signing keys.",
-    )
-    sub_build_sub_apk.add_argument("apkdir", type=ResolvedPath, help="Save the resulting package to this directory")
-    sub_build_sub_pyz = sub_build_subparsers.add_parser(
-        "pyz",
-        description="Build a zipapp .pyz file containing the Python module. Must be run from an editable install.",
-    )
-    sub_build_sub_pyz.add_argument("pyzfile", type=ResolvedPath, help="Save the resulting pyz file to this path")
-    sub_build_sub_version = sub_build_subparsers.add_parser(
-        "save-version", description="Save the Python module and APKBUILD file with a version number"
-    )
-    sub_build_sub_version.add_argument(
-        "--version", help="Set the version to this string. If not present, use a version based on the epoch."
-    )
-
-    # rcmd subcommand
-    sub_rcmd = subparsers.add_parser(
-        "rcmd",
-        parents=[node_opts],
-        description="Run a command on remote nodes. Intended to be run from the controller.",
+    # validate subcommand
+    sub_validate = subparsers.add_parser(
+        "validate", description="Validate the progfigsite that it matches the required API"
     )
-    sub_rcmd.add_argument(
-        "--sh", action="store_true", help="Run the command inside a shell, rather than directly on the host"
-    )
-    sub_rcmd.add_argument("command", help="A command to run remotely")
 
     # debugger subcommand
+    # This is useful for debugging a pyz deployment,
+    # since you can't just 'import progfiguration' inside a python3 interpreter
+    # because the pyz is not on the PYTHONPATH.
     sub_debugger = subparsers.add_parser(
         "debugger",
         description="Open a debugger on localhost.",
     )
 
-    # Parse and return
-    parsed = parser.parse_args(arguments)
-    return parser, parsed
+    # Return
+    return parser
 
 
-def main_implementation(*arguments):
-    parser, parsed = parseargs(arguments[1:])
+def _main_implementation(*arguments):
+    parser = _make_parser()
+    parsed = parser.parse_args(arguments[1:])
 
     if parsed.debug:
         sys.excepthook = idb_excepthook
     elif parsed.syslog_exception:
         sys.excepthook = syslog_excepthook
     configure_logging(parsed.log_stderr, parsed.log_syslog)
 
-    if REMOTING:
-        mitogen_core_level = logging._nameToLevel[parsed.mitogen_log_stderr]
-        mitogen_io_level = logging._nameToLevel[parsed.mitogen_io_log_stderr]
-        remoting.configure_mitogen_logging(mitogen_core_level, mitogen_io_level)
-
-    inventory_file = parsed.inventory_file
-    if not hasattr(inventory_file, "open"):
-        inventory_file = pathlib.Path(inventory_file)
-    inventory = Inventory(parsed.inventory_file, parsed.age_private_key)
+    # Later actions do require an inventory
+
+    # Get a nodename, if we have one
+    try:
+        nodename = parsed.nodename
+    except AttributeError:
+        nodename = None
+
+    inventory = Inventory(
+        sitewrapper.site_submodule_resource("", "inventory.conf"),
+        progfiguration.progfigsite_module_path,
+        age_privkey=parsed.age_private_key,
+        current_node=nodename,
+    )
+
+    validation = validate(progfiguration.progfigsite_module_path)
+    if not validation.is_valid:
+        print(
+            f"Progfigsite (Python path: '{progfiguration.progfigsite_module_path}') has {len(validation.errors)} errors:"
+        )
+        for attrib in validation.errors:
+            print(attrib.errstr)
 
     if parsed.action == "version":
-        print(version.VersionInfo.from_build_version_or_default().verbose())
+        _action_version_all(inventory)
     elif parsed.action == "apply":
-        action_apply(inventory, parsed.nodename, roles=parsed.roles, force=parsed.force_apply)
+        _action_apply(inventory, parsed.nodename, roles=parsed.roles, force=parsed.force_apply)
     elif parsed.action == "deploy":
         if not parsed.nodes and not parsed.groups:
             parser.error("You must pass at least one of --nodes or --groups")
         if parsed.deploy_action == "apply":
-            action_deploy_apply(
+            _action_deploy_apply(
                 inventory,
                 parsed.nodes,
                 parsed.groups,
                 roles=parsed.roles,
                 remote_debug=parsed.remote_debug,
                 force_apply=parsed.force_apply,
                 keep_remote_file=parsed.keep_remote_file,
             )
         elif parsed.deploy_action == "copy":
-            action_deploy_copy(inventory, parsed.nodes, parsed.groups, parsed.destination)
+            _action_deploy_copy(inventory, parsed.nodes, parsed.groups, parsed.destination)
             print(f"Copied to remote host(s) at {parsed.destination}")
         else:
-            raise ValueError(f"Unknown deploy action {parsed.deploy_action}")
+            parser.error(f"Unknown deploy action {parsed.deploy_action}")
     elif parsed.action == "list":
-        action_list(inventory, parsed.collection)
+        _action_list(inventory, parsed.collection)
     elif parsed.action == "info":
-        action_info(inventory, parsed.nodes, parsed.groups, parsed.functions)
+        _action_info(inventory, parsed.nodes, parsed.groups, parsed.functions)
     elif parsed.action == "encrypt":
         if not parsed.nodes and not parsed.groups and not parsed.controller:
             parser.error("You must pass at least one of --nodes, --groups, or --controller")
         if not parsed.value and not parsed.file:
             parser.error("You must pass one of --value or --file")
         if parsed.file:
             with open(parsed.file) as fp:
                 value = fp.read()
         else:
             value = parsed.value
-        action_encrypt(
+        _action_encrypt(
             inventory,
             parsed.save_as or "",
             value,
             parsed.nodes,
             parsed.groups,
             parsed.controller,
             bool(parsed.save_as),
             parsed.stdout,
         )
     elif parsed.action == "decrypt":
         if not parsed.nodes and not parsed.groups and not parsed.controller:
             parser.error("You must pass at least one of --nodes, --groups, or --controller")
-        action_decrypt(inventory, parsed.nodes, parsed.groups, parsed.controller)
-    elif parsed.action == "rcmd":
-        if not REMOTING:
-            raise Exception("Could not import remoting module - make sure mitogen is installed")
-        if not parsed.nodes and not parsed.groups:
-            parser.error("You must pass at least one of --nodes or --groups")
-        action_rcmd(inventory, parsed.nodes, parsed.groups, parsed.command)
-        # remoting.mitogen_example()
-    elif parsed.action == "build":
-        action_build(parsed)
-    elif parsed.action == "debugger":
-        pdb.set_trace()
+        _action_decrypt(inventory, parsed.nodes, parsed.groups, parsed.controller)
+    elif parsed.action == "validate":
+        # We always validate but this shows a nice message even if validation succeeds
+        _action_validate()
     else:
-        raise Exception(f"Unknown action {parsed.action}")
+        parser.error(f"Unknown action {parsed.action}")
+
+
+def main(progfigsite_modpath: str):
+    """The main function for the progfigsite command-line interface
+
+    While this file exists in the core progfiguration package,
+    it is not installed as a command-line script there.
+    Instead, progfigsite packages are expected to add a shim file that calls this function,
+    and configure their Python project to install that shim file as a command-line script.
+
+    This function expects an argument that is the Python module path to the progfigsite package.
+    For instance, if the progfigsite package is installed as 'my_progfigsite',
+    then this argument should be 'my_progfigsite'.
+    This package is expected to be installed in the same Python environment as the progfiguration package.
+    Building a pip package with `progfiguration build pip`
+    will use that shim file to call this function.
+    Building a pyz package with `progfiguration build pyz`
+    will install the site package as `progfigsite` in the pyz regardless of what the site package is called,
+    and will call this function with `progfigsite` as the argument.
+
+    TODO: document how the modpath thing works
+    """
+    progfiguration.progfigsite_module_path = progfigsite_modpath
+    progfiguration_error_handler(_main_implementation, sys.argv)
+
+
+__doc__ = f"""
+The command-line interface for a progfigsite.
+
+This command is installed with a progfigsite package.
+When packaging a progfigsite in a pyz,
+running the pyz will run this command.
+
+This command can interact with site nodes,
+encrypt and decrypt secrets (if an appropriate private key is available),
+and apply a node's roles to the local machine.
+
+## Command line help
 
+The program's command-line help is reproduced here:
 
-def main():
-    progfiguration_error_handler(main_implementation, *sys.argv)
+```text
+{get_command_help("progfigsite", _make_parser())}
+```
+"""
```

### Comparing `progfiguration-0.0.2a1/progfiguration/cmd.py` & `progfiguration-0.0.2a3/progfiguration/cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,56 +4,78 @@
 import select
 import subprocess
 import sys
 
 from progfiguration import logger
 
 
-def run(cmd: str | list, print_output=True, log_output=False, check=True, *args, **kwargs) -> subprocess.Popen:
+class MagicPopen(subprocess.Popen):
+    """A subprocess.Popen with superpowers
+
+    This is a wrapper for subprocess.Popen,
+    which is guaranteed to have a .stdout and .stderr property,
+    which will always be StringIO objects (not bytes).
+
+    It's the return value for magicrun(),
+    and shouldn't be used elsewhere.
+    """
+
+    stdout: io.StringIO
+    stderr: io.StringIO
+
+
+def magicrun(cmd: str | list, print_output=True, log_output=False, check=True, *args, **kwargs) -> MagicPopen:
     """Run a command, with superpowers
 
-    * cmd: The command to run. If a string, it will be passed to a shell.
-    * print_output: Print the command's stdout/stderr in to the controlling terminal's stdout/stderr in real time.
+    Params:
+
+    * `cmd`: The command to run. If a string, it will be passed to a shell.
+    * `print_output`: Print the command's stdout/stderr in to the controlling terminal's stdout/stderr in real time.
         stdout/stderr is always captured and returned, whether this is True or False (superpowers).
         The .stdout and .stderr properties are always strings, not bytes
         (which is required because we must use universal_newlines=True).
         * <https://gist.github.com/nawatts/e2cdca610463200c12eac2a14efc0bfb>
         * <https://stackoverflow.com/questions/4417546/constantly-print-subprocess-output-while-process-is-running>
-    * log_output: Log the command's stdout/stderr in a single log message (each) after the command completes.
-    * check: Raise an exception if the command returns a non-zero exit code.
+    * `log_output`: Log the command's stdout/stderr in a single log message (each) after the command completes.
+    * `check`: Raise an exception if the command returns a non-zero exit code.
         Unlike subprocess.run, this is True by default.
-    * *args, **kwargs: Passed to subprocess.Popen
+    * `*args, **kwargs`: Passed to subprocess.Popen
         Do not pass the following arguments, as they are used internally:
         * shell: Determined automatically based on the type of cmd
         * stdout: Always subprocess.PIPE
         * stderr: Always subprocess.PIPE
         * universal_newlines: Always True
         * bufsize: Always 1
 
-    The Popen object is always returned.
+    A `MagicPopen` object is always returned.
     """
     shell = isinstance(cmd, str)
 
     logger.debug(f"Running command: {cmd}")
-    process = subprocess.Popen(
+
+    # ignore mypy errors because *args and **kwargs confuses it
+    process = subprocess.Popen(  # type: ignore
         cmd,
         shell=shell,
         bufsize=1,  # Output is line buffered, required to print output in real time
         universal_newlines=True,  # Required for line buffering
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         *args,
         **kwargs,
     )
 
     stdoutbuf = io.StringIO()
     stderrbuf = io.StringIO()
 
-    stdout_fileno = process.stdout.fileno()
-    stderr_fileno = process.stderr.fileno()
+    # Ignore mypy errors related to stdout/stderrbuf not being file objects.
+    # We know they're file objects because we set them to subprocess.PIPE.
+
+    stdout_fileno = process.stdout.fileno()  # type: ignore
+    stderr_fileno = process.stderr.fileno()  # type: ignore
 
     # This returns None until the process terminates
     while process.poll() is None:
 
         # select() waits until there is data to read (or an "exceptional case") on any of the streams
         readready, writeready, exceptionready = select.select(
             [process.stdout, process.stderr],
@@ -63,20 +85,20 @@
         )
 
         # Check if what is ready is a stream, and if so, which stream.
         # Copy the stream to the buffer so we can use it,
         # and print it to stdout/stderr in real time if print_output is True.
         for stream in readready:
             if stream.fileno() == stdout_fileno:
-                line = process.stdout.readline()
+                line = process.stdout.readline()  # type: ignore
                 stdoutbuf.write(line)
                 if print_output:
                     sys.stdout.write(line)
             elif stream.fileno() == stderr_fileno:
-                line = process.stderr.readline()
+                line = process.stderr.readline()  # type: ignore
                 stderrbuf.write(line)
                 if print_output:
                     sys.stderr.write(line)
             else:
                 raise Exception(f"Unknown file descriptor in select result. Fileno: {stream.fileno()}")
 
         # If what is ready is an exceptional situation, blow up I guess;
@@ -87,18 +109,18 @@
             elif stream.fileno() == stderr_fileno:
                 raise Exception("Exception on stderr")
             else:
                 raise Exception(f"Unknown exception in select result. Fileno: {stream.fileno()}")
 
     # We'd like to just seek(0) on the stdout/stderr buffers, but "underlying stream is not seekable",
     # So we create new buffers above, write to them line by line, and replace the old ones with these.
-    process.stdout.close()
+    process.stdout.close()  # type: ignore
     stdoutbuf.seek(0)
     process.stdout = stdoutbuf
-    process.stderr.close()
+    process.stderr.close()  # type: ignore
     stderrbuf.seek(0)
     process.stderr = stderrbuf
 
     if check and process.returncode != 0:
         msg = f"Command failed with exit code {process.returncode}: {cmd}"
         logger.error(msg)
         logger.info(f"stdout: {process.stdout.getvalue()}")
@@ -112,8 +134,12 @@
     if log_output:
         # Note that .getvalue() is not (always?) available on normal Popen stdout/stderr,
         # but it is available on our StringIO objects.
         # .getvalue() doesn't change the seek position.
         logger.info(f"stdout: {process.stdout.getvalue()}")
         logger.info(f"stderr: {process.stderr.getvalue()}")
 
-    return process
+    # Now that we've set stdout/err to StringIO objects,
+    # we can return the Popen object as a MagicPopen object.
+    magic_process: MagicPopen = process
+
+    return magic_process
```

### Comparing `progfiguration-0.0.2a1/progfiguration/inventory/nodes.py` & `progfiguration-0.0.2a3/progfiguration/inventory/nodes.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     flavortext: str
     age_pubkey: str
     ssh_host_fingerprint: str
     psy0mac: str
     serial: str
     roles: Bunch
     network_interfaces: Optional[str] = None
+    age_key_path: Optional[str] = None
 
     # If this is True, 'progfiguration apply' will refuse to run.
     # Useful for inspecting early state after a reboot during development.
     TESTING_DO_NOT_APPLY: bool = False
 
     @property
     def known_hosts_entry(self) -> str:
```

### Comparing `progfiguration-0.0.2a1/progfiguration/inventory/roles.py` & `progfiguration-0.0.2a3/progfiguration/inventory/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-"""Applying and working with roles"""
+"""Applying and working with roles
+
+Note that we have to ignore type checking on string references to Inventory here.
+The inventory module imports this module,
+so we cannot import it,
+or we will get a circular import.
+"""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from importlib.abc import Traversable
 from importlib.resources import files as importlib_resources_files
 from types import ModuleType
-from typing import Any, Dict, List, Optional, Type
+from typing import Any, Dict, Optional
 
 from progfiguration import age
-
 from progfiguration.inventory.nodes import InventoryNode
-from progfiguration.localhost import LocalhostLinuxPsyopsOs
+from progfiguration.localhost import LocalhostLinux
 
 
 @dataclass
 class RoleResultReference:
     """A reference to a result from a role
 
     This is used to allow roles to reference results from other roles
@@ -45,16 +50,16 @@
     * results(): Return a dict of results that may be used by other roles
 
     Note that you cannot override properties in a subclass of a dataclass.
     Take care when adding new attributes here.
     """
 
     name: str
-    localhost: LocalhostLinuxPsyopsOs
-    inventory: "Inventory"
+    localhost: LocalhostLinux
+    inventory: "Inventory"  # type: ignore
     rolepkg: str
 
     # This is just a cache
     _rolefiles: Optional[Any] = None
 
     @abstractmethod
     def apply(self, **kwargs):
@@ -69,15 +74,20 @@
         This works whether we're installed from pip, checked out from git, or running from a pyz file.
         """
         if not self._rolefiles:
             self._rolefiles = importlib_resources_files(self.rolepkg)
         return self._rolefiles.joinpath(filename)
 
 
-def dereference_rolearg(nodename: str, argument: Any, inventory: "Inventory", secrets: Dict[str, Any]) -> Any:
+def dereference_rolearg(
+    nodename: str,
+    argument: Any,
+    inventory: "Inventory",  # type: ignore
+    secrets: Dict[str, Any],
+) -> Any:
     """Get the final value of a role argument for a node.
 
     Arguments to this method:
 
     * nodename:     The name of the node that the argument is being applied to
     * argument:     The role argument to get the final value of
     * inventory:    The inventory object
@@ -99,20 +109,19 @@
         value = secret.decrypt(inventory.age_path)
     elif isinstance(argument, RoleResultReference):
         value = inventory.node_role(nodename, argument.role).results()[argument.result]
     return value
 
 
 def collect_role_arguments(
-    inventory: "Inventory",
+    inventory: "Inventory",  # type: ignore
     nodename: str,
     node: InventoryNode,
     nodegroups: dict[str, ModuleType],
     rolename: str,
-    role_cls: Type[ProgfigurationRole],
 ):
     """Collect all the arguments for a role
 
     Find the arguments in the following order:
 
     * Default role arguments from the ProgfigurationRole subclass
     * Arguments from the universal group
```

### Comparing `progfiguration-0.0.2a1/progfiguration/localhost/__init__.py` & `progfiguration-0.0.2a3/progfiguration/localhost/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import shutil
 import string
 import subprocess
 import tempfile
 from typing import Any, Dict, List, Optional
 
 from progfiguration import temple
-from progfiguration.cmd import run
+from progfiguration.cmd import magicrun
 from progfiguration.localhost.localusers import LocalhostUsers
-from progfiguration.progfigtypes import AnyPathOrStr
+from progfiguration.progfigtypes import AnyPathOrStr, PathOrStr
 
 
 class LocalhostLinux:
     """An interface to localhost running Linux.
 
     Maintains a cache of files it has read before.
     """
@@ -69,14 +69,30 @@
         else:
             contents = self._cache_files[path]
         if chomp:
             return contents.strip()
         else:
             return contents
 
+    def chown(self, path: PathOrStr, owner: Optional[int | str], group: Optional[int | str]):
+        """Change the owner and/or group of a file or directory
+
+        A convenience function that can handle any combination of owner and group.
+        """
+        if not isinstance(path, str):
+            path = str(path)
+        if owner and group:
+            shutil.chown(path, owner, group)
+        elif owner:
+            shutil.chown(path, owner)
+        elif group:
+            # ... why is this not a thing in the stdlib?
+            uid = os.stat(path).st_uid
+            shutil.chown(path, uid, group)
+
     def set_file_contents(
         self,
         path: AnyPathOrStr,
         contents: str,
         owner: Optional[str] = None,
         group: Optional[str] = None,
         mode: Optional[int] = None,
@@ -85,22 +101,21 @@
         if not isinstance(path, str):
             path = str(path)
         self.makedirs(os.path.dirname(path), owner, group, dirmode)
         if path in self._cache_files:
             del self._cache_files[path]
         with open(path, "w") as fp:
             fp.write(contents)
-        if owner or group:
-            shutil.chown(path, owner, group)
+        self.chown(path, owner, group)
         if mode:
             os.chmod(path, mode)
 
     def makedirs(
         self,
-        path: AnyPathOrStr,
+        path: PathOrStr,
         owner: Optional[str] = None,
         group: Optional[str] = None,
         mode: Optional[int] = None,
     ):
         if isinstance(path, str):
             path = Path(os.path.abspath(path))
         if path.exists():
@@ -113,50 +128,51 @@
         # while os.path.islink(head):
         #     head = os.readlink(head)
         if not head.is_dir():
             raise Exception(f"Path component {head} exists but it is not a directory")
         # We have to set the mode separately, as os.mkdir()'s mode argument is umasked
         # <https://stackoverflow.com/questions/37118558/python3-os-mkdir-does-not-enforce-correct-mode>
         os.mkdir(str(path))
-        path.chmod(mode)
-        if owner or group:
-            shutil.chown(str(path), user=owner, group=group)
+        if mode is not None:
+            path.chmod(mode)
+        self.chown(path, owner, group)
 
     def cp(
         self,
-        src: AnyPathOrStr,
-        dest: AnyPathOrStr,
+        src: PathOrStr,
+        dest: PathOrStr,
         owner: Optional[str] = None,
         group: Optional[str] = None,
         mode: Optional[int] = None,
         dirmode: Optional[int] = None,
     ):
+        if isinstance(src, str):
+            src = Path(src)
         if isinstance(dest, str):
             dest = Path(dest)
         self.makedirs(dest.parent, owner, group, dirmode)
         if os.path.exists(str(src)):
             shutil.copy(src, dest)
         elif hasattr(src, "open"):
             if dest.is_dir():
                 dest = dest.joinpath(src.name)
             with src.open("r") as srcfp:
                 with dest.open("w") as destfp:
                     shutil.copyfileobj(srcfp, destfp)
         else:
             raise Exception(f"Not sure how to copy src (type: {type(src)}) at {src} (does it exist?)")
-        if owner or group:
-            shutil.chown(str(dest), user=owner, group=group)
+        self.chown(dest, owner, group)
         if mode:
             dest.chmod(mode)
 
     def _template_backend(
         self,
         template: type,
-        src: AnyPathOrStr,
-        dest: AnyPathOrStr,
+        src: PathOrStr,
+        dest: PathOrStr,
         template_args: Dict[str, Any],
         owner: Optional[str] = None,
         group: Optional[str] = None,
         mode: Optional[int] = None,
         dirmode: Optional[int] = None,
     ):
         """Template a file using the appropriate backend"""
@@ -192,15 +208,15 @@
         mode: Optional[int] = None,
         dirmode: Optional[int] = None,
     ):
         return self._template_backend(temple.Temple, src, dest, template_args, owner, group, mode, dirmode)
 
     def linesinfile(
         self,
-        file: AnyPathOrStr,
+        file: PathOrStr,
         lines: List[str],
         create_owner: Optional[str] = None,
         create_group: Optional[str] = None,
         create_mode: Optional[int] = None,
         create_dirmode: Optional[int] = None,
         trailing_newline: bool = True,
     ):
@@ -237,18 +253,18 @@
         contents_str = "\n".join(newlines)
         if trailing_newline:
             contents_str += "\n"
         self.set_file_contents(file, contents_str)
 
     def touch(
         self,
-        file: AnyPathOrStr,
+        file: PathOrStr,
         owner: Optional[str] = None,
         group: Optional[str] = None,
-        mode: Optional[int] = None,
+        mode: int = 0o666,
         dirmode: Optional[int] = None,
     ):
         """Create an empty file.
 
         If the file already exists, update its mtime.
 
         Set the owner/group/mode, if specified, regardless of whether the file already exists.
@@ -257,55 +273,37 @@
         (If parent dirs do exist, do not change their owners.)
         """
         if not isinstance(file, Path):
             file = Path(file)
         if not file.parent.exists():
             self.makedirs(file.parent, owner, group, dirmode)
         file.touch(mode=mode, exist_ok=True)
-        shutil.chown(str(file), user=owner, group=group)
+        self.chown(file, owner, group)
 
     def get_user_primary_group(self, user: str):
         """Get the primary group for a user.
 
         Use the `id` command because it is POSIX compliant
         and works with non-local users and groups like LDAP etc.
         """
         result = subprocess.run(["id", "-g", "-n", user], capture_output=True, check=True)
         return result.stdout.decode().strip()
 
-    def write_sudoers(self, path: AnyPathOrStr, contents: str):
+    def write_sudoers(self, path: PathOrStr, contents: str):
         """Write a sudoers file.
 
         The file is written to a temporary file and then moved into place.
 
         You can write to /etc/sudoers this way, but it is recommended to write to /etc/sudoers.d/SOMEFILE instead.
         """
         if isinstance(path, str):
             path = Path(path)
         with tempfile.TemporaryDirectory() as tmpdir:
             tmpfile = Path(tmpdir) / "sudoers"
             self.set_file_contents(tmpfile, contents, owner="root", group="root", mode=0o640)
-            validation = run(["visudo", "-cf", str(tmpfile)], check=False, print_output=False)
+            validation = magicrun(["visudo", "-cf", str(tmpfile)], check=False, print_output=False)
             if validation.returncode == 0:
                 self.cp(tmpfile, path, owner="root", group="root", mode=0o440)
             else:
                 raise Exception(
                     f"Failed to write sudoers file {path}: validation failed with code {validation.returncode}"
                 )
-
-
-class LocalhostLinuxPsyopsOs(LocalhostLinux):
-    """An interface to localhost running psyopsOS"""
-
-    @property
-    def alpine_release_str(self) -> str:
-        return self.get_file_contents("/etc/alpine-release")
-
-    @property
-    def alpine_release(self) -> List[int]:
-        return [int(n) for n in self.alpine_release_str.split(".")]
-
-    @property
-    def alpine_release_v(self) -> str:
-        """If /etc/alpine-release is '3.16.0', this returns 'v3.16'."""
-        maj, min, _ = self.alpine_release
-        return f"v{maj}.{min}"
```

### Comparing `progfiguration-0.0.2a1/progfiguration/localhost/authorized_keys.py` & `progfiguration-0.0.2a3/progfiguration/localhost/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a1/progfiguration/localhost/disks.py` & `progfiguration-0.0.2a3/progfiguration/localhost/disks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Working with disks, filesystems, etc"""
 
 
 import os
 import subprocess
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional
+from typing import List, Optional
 
 from progfiguration import logger
 
 
 @dataclass
 class FilesystemSpec:
     # The type of filesystem -- requires a mkfs.{fstype} binary on the target system.
```

### Comparing `progfiguration-0.0.2a1/progfiguration/localhost/localusers.py` & `progfiguration-0.0.2a3/progfiguration/localhost/localusers.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a1/progfiguration/remotebrute/__init__.py` & `progfiguration-0.0.2a3/progfiguration/remotebrute/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 * Implement ControlMaster for faster repeated copies/commands
 """
 
 import os.path
 import secrets
 import shlex
 import string
-from typing import Any, List, Union
+from typing import Any, List, Optional, Union
 
 from progfiguration import logger
-from progfiguration.cmd import run
+from progfiguration.cmd import magicrun
 
 
 def generate_random_string(length):
     """Generate a secure random string of the specified length."""
     alphabet = string.ascii_letters + string.digits
     return "".join(secrets.choice(alphabet) for i in range(length))
 
@@ -33,23 +33,23 @@
 
     if isinstance(sources, str):
         sources = [sources]
 
     cmd = ["scp", "-r"]
     cmd += sources
     cmd += [f"{host}:{dest}"]
-    run(cmd)
+    magicrun(cmd)
 
 
 def cpexec(
     host: str,
     source: str,
-    args: List[str] = None,
+    args: Optional[List[str]] = None,
     dest: str = "",
-    interpreter: list[str] = None,
+    interpreter: Optional[List[str]] = None,
     ssh_tty: bool = True,
     ssh_stdin: Any = None,
     keep_remote_file: bool = False,
 ):
     """Copy a file to a remote host, then execute and delete the remote copy
 
     host: the remote host to connect to
@@ -85,18 +85,18 @@
             ssh_cmd_run_args["stdin"] = ssh_stdin
 
         ssh_cmd = ["ssh"]
         if ssh_tty:
             ssh_cmd += ["-tt"]
         ssh_cmd += [host, remote_cmd]
 
-        execresult = run(ssh_cmd, **ssh_cmd_run_args)
+        execresult = magicrun(ssh_cmd, **ssh_cmd_run_args)
 
         logger.debug(f"Finished ssh command to {host}")
     finally:
         if keep_remote_file:
             print(f"Kept the remote file at {dest}")
         else:
             # We don't need to fuck with ttys/fds here because rm is simple
-            run(["ssh", host, f"rm -f {dest}"])
+            magicrun(["ssh", host, f"rm -f {dest}"])
 
     return execresult
```

### Comparing `progfiguration-0.0.2a1/progfiguration/temple/__init__.py` & `progfiguration-0.0.2a3/progfiguration/temple/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a1/progfiguration.egg-info/SOURCES.txt` & `progfiguration-0.0.2a3/progfiguration.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 pyproject.toml
 readme.md
 progfiguration/__init__.py
 progfiguration/age.py
 progfiguration/cmd.py
+progfiguration/progfigsite_validator.py
 progfiguration/progfigtypes.py
 progfiguration/ssh.py
-progfiguration/version.py
+progfiguration/util.py
 progfiguration.egg-info/PKG-INFO
 progfiguration.egg-info/SOURCES.txt
 progfiguration.egg-info/dependency_links.txt
 progfiguration.egg-info/entry_points.txt
 progfiguration.egg-info/requires.txt
 progfiguration.egg-info/top_level.txt
+progfiguration/builddata/__init__.py
 progfiguration/cli/__init__.py
-progfiguration/cli/progfiguration_cmd.py
-progfiguration/example_site/__init__.py
-progfiguration/example_site/inventory.yml
-progfiguration/example_site/readme.md
-progfiguration/example_site/groups/__init__.py
-progfiguration/example_site/groups/group1.py
-progfiguration/example_site/groups/universal.py
-progfiguration/example_site/nodes/__init__.py
-progfiguration/example_site/nodes/node1.py
-progfiguration/example_site/roles/__init__.py
-progfiguration/example_site/roles/settz.py
-progfiguration/example_site/sitelib/__init__.py
+progfiguration/cli/progfiguration_core_cmd.py
+progfiguration/cli/progfiguration_site_cmd.py
+progfiguration/cli/util.py
 progfiguration/inventory/__init__.py
 progfiguration/inventory/nodes.py
 progfiguration/inventory/roles.py
 progfiguration/localhost/__init__.py
 progfiguration/localhost/authorized_keys.py
 progfiguration/localhost/disks.py
 progfiguration/localhost/localusers.py
+progfiguration/progfigbuild/__init__.py
 progfiguration/remotebrute/__init__.py
-progfiguration/remoting/__init__.py
-progfiguration/remoting/rfuncs.py
 progfiguration/sitewrapper/__init__.py
 progfiguration/temple/__init__.py
-tests/__init__.py
 tests/test_cmd.py
+tests/test_packaging.py
 tests/test_site.py
```

### Comparing `progfiguration-0.0.2a1/pyproject.toml` & `progfiguration-0.0.2a3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 [build-system]
 requires = [
+    "pdoc",
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "progfiguration"
-version = "0.0.2a1"
+version = "0.0.2a3"
 description = "PROGramatic conFIGURATION for your infrastructure"
 license = {text = "MIT"}
 readme = "readme.md"
 requires-python = ">=3.10"
-dependencies = [
-    "PyYAML",
-    "pytz",
-    "requests",
-]
 
 [[project.authors]]
 name = "Micah R Ledbetter"
 email = "me@micahrl.com"
 
 [project.scripts]
-progfiguration = "progfiguration.cli.progfiguration_cmd:main"
+progfiguration = "progfiguration.cli.progfiguration_core_cmd:main"
 
 [project.optional-dependencies]
-ssh = [
-    "mitogen",
-]
 development = [
     "black",
     "build",
-    "mitogen",
     "mypy",
+    "pdoc",
     "twine",
 ]
 
 [project.urls]
 Homepage = "https://github.com/mrled/progfiguration"
 
 [tool.black]
 line-length = 120
+
+[tool.setuptools.package-data]
+"*" = ["*"]
```

### Comparing `progfiguration-0.0.2a1/tests/test_cmd.py` & `progfiguration-0.0.2a3/tests/test_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,35 @@
 
 from progfiguration import cmd
 
 
 class TestRun(unittest.TestCase):
     def test_run_basic_stdout_stderr(self):
         """Test stdout/err redirection"""
-        result = cmd.run(["sh", "-c", "(echo hello); (echo world >&2)"], print_output=False)
+        result = cmd.magicrun(["sh", "-c", "(echo hello); (echo world >&2)"], print_output=False)
         self.assertEqual(result.stdout.read(), "hello\n")
         self.assertEqual(result.stderr.read(), "world\n")
 
     def test_run_with_print_output(self):
         """Test simultaneous stdout/err redirection and printing to the terminal"""
 
         # Redirect stdout/err to a buffer so that we can test that it's writing to it correctly
         # This tests our magic print_output=True functionality :)
         outbuf = io.StringIO()
         sys.stdout = outbuf
         errbuf = io.StringIO()
         sys.stderr = errbuf
 
-        result = cmd.run(["sh", "-c", "(echo hello); (echo world >&2)"])
+        result = cmd.magicrun(["sh", "-c", "(echo hello); (echo world >&2)"])
 
         self.assertEqual(result.stdout.read(), "hello\n")
         self.assertEqual(result.stderr.read(), "world\n")
 
         terminal_out = outbuf.getvalue()
         terminal_err = errbuf.getvalue()
 
         # Reset stdout/err
         sys.stdout = sys.__stdout__
         sys.stderr = sys.__stderr__
 
         self.assertEqual(terminal_out, "hello\n")
         self.assertEqual(terminal_err, "world\n")
-
-
-if __name__ == "__main__":
-    unittest.main()
```

